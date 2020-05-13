<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `memcached`

-	[`memcached:1`](#memcached1)
-	[`memcached:1.6`](#memcached16)
-	[`memcached:1.6.6`](#memcached166)
-	[`memcached:1.6.6-alpine`](#memcached166-alpine)
-	[`memcached:1.6-alpine`](#memcached16-alpine)
-	[`memcached:1-alpine`](#memcached1-alpine)
-	[`memcached:alpine`](#memcachedalpine)
-	[`memcached:latest`](#memcachedlatest)

## `memcached:1`

```console
$ docker pull memcached@sha256:b0f382f16271ffe9dce89bc4d47b8627ae4b491286bec220dadaee3862cdc1e2
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
$ docker pull memcached@sha256:e8c935cf0dfa9eecf9129d9039cfbe12f55c1cecc86902998d4c7c369f5b5a57
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.5 MB (30493690 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9bb369dc76dc6e22e495a01681b1d1c428701d8a06f7304ef333b36f13469e8a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 23 Apr 2020 00:20:32 GMT
ADD file:9b8be2b52ee0fa31da1b6256099030b73546253a57e94cccb24605cd888bb74d in / 
# Thu, 23 Apr 2020 00:20:32 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 03:48:31 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Thu, 23 Apr 2020 03:48:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 13 May 2020 20:57:07 GMT
ENV MEMCACHED_VERSION=1.6.6
# Wed, 13 May 2020 20:57:07 GMT
ENV MEMCACHED_SHA1=d8895b12dc9fc82b389f1713e2c09cc6ca3d03e4
# Wed, 13 May 2020 21:06:31 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 13 May 2020 21:06:31 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 13 May 2020 21:06:32 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 13 May 2020 21:06:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 13 May 2020 21:06:32 GMT
USER memcache
# Wed, 13 May 2020 21:06:32 GMT
EXPOSE 11211
# Wed, 13 May 2020 21:06:32 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:54fec2fa59d0a0de9cd2dec9850b36c43de451f1fd1c0a5bf8f1cf26a61a5da4`  
		Last Modified: Thu, 23 Apr 2020 00:25:10 GMT  
		Size: 27.1 MB (27098254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73a546564c749aeaf996f91019e9cf37b5e395b661aec0dcf2e2c20c11bbda96`  
		Last Modified: Thu, 23 Apr 2020 03:58:00 GMT  
		Size: 5.0 KB (4979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2b17108b143c42eeda6a8587b36cfd6e30c7783fb09e565feb06d09f4172525`  
		Last Modified: Thu, 23 Apr 2020 03:58:01 GMT  
		Size: 2.2 MB (2196403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a1e9dd08a002476ba6cade3017e17f464968c8e94877292d07c5b899a9e8d3a`  
		Last Modified: Wed, 13 May 2020 21:16:44 GMT  
		Size: 1.2 MB (1193645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09cafd6239484b297ad595f395a878b6ce07eefcca9de92a17910aa735abe6d5`  
		Last Modified: Wed, 13 May 2020 21:16:44 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48b6890ea4c000ff4ec7834a60a4422aaa4e75ac040f107523b1a2c653b6a4b4`  
		Last Modified: Wed, 13 May 2020 21:16:43 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1` - linux; arm variant v5

```console
$ docker pull memcached@sha256:d430d81aec7724f5662cd0dad2554d354921139f129ec60d96fcd97d835a68e5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.9 MB (27901495 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d38f156a5705d867b8698bf28f60397b2ccaa27ebd90a3a370e641ea8836fea3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 23 Apr 2020 00:52:22 GMT
ADD file:62a9732be4e3237ccc896f724a34606e01f351c4877e52c9a9cd85029c06b956 in / 
# Thu, 23 Apr 2020 00:52:23 GMT
CMD ["bash"]
# Mon, 27 Apr 2020 20:31:39 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Mon, 27 Apr 2020 20:31:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 13 May 2020 20:49:55 GMT
ENV MEMCACHED_VERSION=1.6.6
# Wed, 13 May 2020 20:49:56 GMT
ENV MEMCACHED_SHA1=d8895b12dc9fc82b389f1713e2c09cc6ca3d03e4
# Wed, 13 May 2020 21:01:00 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 13 May 2020 21:01:01 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 13 May 2020 21:01:03 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 13 May 2020 21:01:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 13 May 2020 21:01:05 GMT
USER memcache
# Wed, 13 May 2020 21:01:06 GMT
EXPOSE 11211
# Wed, 13 May 2020 21:01:07 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:a8c46e5952878f9f324df86c5a2b45b2e0020f6721e820981e74461d77a100dd`  
		Last Modified: Thu, 23 Apr 2020 00:59:50 GMT  
		Size: 24.8 MB (24836319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0e09e82475aef1e3124cd928ab36f48dd86a0421490ff8d8eab1ae848dbf6e6`  
		Last Modified: Mon, 27 Apr 2020 20:41:52 GMT  
		Size: 4.9 KB (4901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ed2c941c8d2e3eb09c1ec4cf66006155ff9774d385e99a0fe1de44269bfcb8a`  
		Last Modified: Mon, 27 Apr 2020 20:41:53 GMT  
		Size: 1.9 MB (1896804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:114ca507809768dd949fd745f46978c84751747b86a1b70e2d2e8681f85bb5c7`  
		Last Modified: Wed, 13 May 2020 21:01:32 GMT  
		Size: 1.2 MB (1163062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8325227257270f7e70028b55a4b9824a561441cc464ec94298af0caeb3ae7c7`  
		Last Modified: Wed, 13 May 2020 21:01:32 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65eb2dfc473e854cbe271a2fa75b0ee74363953ba9d80a4dfefc1954d1430c0f`  
		Last Modified: Wed, 13 May 2020 21:01:31 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1` - linux; arm variant v7

```console
$ docker pull memcached@sha256:8c0e9908733d5c2401b24e506567ca9ad0b6756c2c92d04b46e2d58eeff0b944
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.7 MB (25656893 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c9b4186eea9043000afc5ff47c169dae434c62ad0d68ef804b36ec022967aeec`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 23 Apr 2020 01:03:26 GMT
ADD file:db6122b36f3e70c5f490b50afba99d49fa345f11d0f5c77bb3c6749f8e2a4f81 in / 
# Thu, 23 Apr 2020 01:03:28 GMT
CMD ["bash"]
# Mon, 27 Apr 2020 20:31:45 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Mon, 27 Apr 2020 20:31:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 13 May 2020 20:49:59 GMT
ENV MEMCACHED_VERSION=1.6.6
# Wed, 13 May 2020 20:49:59 GMT
ENV MEMCACHED_SHA1=d8895b12dc9fc82b389f1713e2c09cc6ca3d03e4
# Wed, 13 May 2020 21:00:32 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 13 May 2020 21:00:33 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 13 May 2020 21:00:35 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 13 May 2020 21:00:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 13 May 2020 21:00:36 GMT
USER memcache
# Wed, 13 May 2020 21:00:37 GMT
EXPOSE 11211
# Wed, 13 May 2020 21:00:38 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:50fb0052086928803f00724ca465c89c45dde5b082b1e59dadb8101286dd5ab6`  
		Last Modified: Thu, 23 Apr 2020 01:11:08 GMT  
		Size: 22.7 MB (22705377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ae844ffae38c0aae3794728fe7c89bff09b70d2226e7b0775beab756cc93856`  
		Last Modified: Mon, 27 Apr 2020 20:50:45 GMT  
		Size: 4.9 KB (4898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6003a4985eba124dc101599be1daf743ce2f44e09d30ea54bf909540aa150a8`  
		Last Modified: Mon, 27 Apr 2020 20:50:45 GMT  
		Size: 1.8 MB (1811519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23bc49c42147e3c6c4bae63d2570761c08ef7aaefc2c07b43258c53f9e8865c9`  
		Last Modified: Wed, 13 May 2020 21:11:35 GMT  
		Size: 1.1 MB (1134692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea93b4316081dba615b7e4d490934ed3ec3cf7979bf5200d7455309149f554c2`  
		Last Modified: Wed, 13 May 2020 21:11:35 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c26e78f516132b9ab5e5b47948d2171d973044571df9d3fcfef732b08086425`  
		Last Modified: Wed, 13 May 2020 21:11:34 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:d423b2ef6d053c533639c07693e0cfca1ccb8715b1825c9dd09a5e8754ab1af7
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.1 MB (29102138 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d2b62ffbdd70a7d226f91ebe12b68d7ad5b580ea2fdb690621b441e7a64b2ab`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 23 Apr 2020 00:54:55 GMT
ADD file:581ee9c3c19f0d971aeda008fd399f59171cae75e8936b967dbf3888db4fc0d0 in / 
# Thu, 23 Apr 2020 00:54:58 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 03:03:20 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Thu, 23 Apr 2020 03:03:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 13 May 2020 20:56:07 GMT
ENV MEMCACHED_VERSION=1.6.6
# Wed, 13 May 2020 20:56:08 GMT
ENV MEMCACHED_SHA1=d8895b12dc9fc82b389f1713e2c09cc6ca3d03e4
# Wed, 13 May 2020 21:06:19 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 13 May 2020 21:06:20 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 13 May 2020 21:06:22 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 13 May 2020 21:06:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 13 May 2020 21:06:23 GMT
USER memcache
# Wed, 13 May 2020 21:06:24 GMT
EXPOSE 11211
# Wed, 13 May 2020 21:06:24 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:bdc84a41f2513e28e99efeff9fcbb196b7df9883fb30532184bd67ca415b4673`  
		Last Modified: Thu, 23 Apr 2020 01:03:27 GMT  
		Size: 25.9 MB (25857800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b8ed987f36e3ad8893c5c7ce9e42aeb35d67e90daf262dde60d86dfa94814f5`  
		Last Modified: Thu, 23 Apr 2020 03:32:22 GMT  
		Size: 5.0 KB (5028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:360e6a91a753e3a018e26a9d22b25766c2ebd2231cbc3e245648aead98ddde08`  
		Last Modified: Thu, 23 Apr 2020 03:32:23 GMT  
		Size: 2.1 MB (2074961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9beea1961eacb995614a88fb9793f9a187c12a86f94a6be75130effc76976768`  
		Last Modified: Wed, 13 May 2020 21:17:27 GMT  
		Size: 1.2 MB (1163938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b48ab287b49fd3b8a7f96050d1d72454c2581bae20dbdd2d52ec0d9766d2d56`  
		Last Modified: Wed, 13 May 2020 21:17:26 GMT  
		Size: 290.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dce9e28ac95b05cd478c90cb28edf8e74c70f8fc79bd3acde6d5104bd563f32b`  
		Last Modified: Wed, 13 May 2020 21:17:25 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1` - linux; 386

```console
$ docker pull memcached@sha256:4cd7c8a145c4b502f84c55f41e0ae4971614a237b96076093edb951df16af86f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.2 MB (31163013 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66532fde035d2034732c7b657027f1f342acdb811b1d859d9f6ed3bc370262e2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 23 Apr 2020 00:39:36 GMT
ADD file:ca6a74f6b738c738c033152fab2a9aacf22bec5f19a994e6a02b5f919ee33ee9 in / 
# Thu, 23 Apr 2020 00:39:36 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 01:29:35 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Thu, 23 Apr 2020 01:29:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 01:29:42 GMT
ENV MEMCACHED_VERSION=1.6.5
# Thu, 23 Apr 2020 01:29:42 GMT
ENV MEMCACHED_SHA1=1ddb5f37f69946b63512ad0f89dc448ff7ba5713
# Thu, 23 Apr 2020 01:38:20 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 23 Apr 2020 01:38:20 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 23 Apr 2020 01:38:21 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 23 Apr 2020 01:38:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Apr 2020 01:38:21 GMT
USER memcache
# Thu, 23 Apr 2020 01:38:21 GMT
EXPOSE 11211
# Thu, 23 Apr 2020 01:38:21 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:5d3da8f33b97fc107a05b3255a55836b76df9f817de632b1fb63c6e9c024f0df`  
		Last Modified: Thu, 23 Apr 2020 00:44:35 GMT  
		Size: 27.8 MB (27753972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c3cb2639d5e9c8ab44fd2bbe5bedbb5c4d33378f9781d558d2ac27611ecd673`  
		Last Modified: Thu, 23 Apr 2020 01:38:35 GMT  
		Size: 4.9 KB (4898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6f2f84fd6631cbca67ed46fd3b380a42475afb287d8e990ded3d3a91fded71a`  
		Last Modified: Thu, 23 Apr 2020 01:38:35 GMT  
		Size: 2.2 MB (2208055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae882751a1fc445bebd4d4f545c0c69529396863b7ac0b3fc3137b2c3cecbfaa`  
		Last Modified: Thu, 23 Apr 2020 01:38:35 GMT  
		Size: 1.2 MB (1195679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d53c7886eeb4da4192fe5caceac337d1fa31afc20be46a9476fd10e35bd4d81e`  
		Last Modified: Thu, 23 Apr 2020 01:38:35 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43f9bc6252b62803993a04eff4ad6e08d728474f2c446e92d32b5ab3ac38ab08`  
		Last Modified: Thu, 23 Apr 2020 01:38:35 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1` - linux; mips64le

```console
$ docker pull memcached@sha256:2b4b9c9aba5b7a352d4f631bfdf5b38489d2e2ea2bb40ce5c0d592d2f3beb517
```

-	Docker Version: 19.03.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.7 MB (28725203 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:53b77428fcdf16a094d4463e769da9547573740a8f4723c8951289da773cd5a4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 23 Apr 2020 00:09:47 GMT
ADD file:7509945bd8a224048260e88b466aa3b156615e16b64e0a6702da277052fcb98b in / 
# Thu, 23 Apr 2020 00:09:48 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 01:41:19 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Thu, 23 Apr 2020 01:41:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 01:41:33 GMT
ENV MEMCACHED_VERSION=1.6.5
# Thu, 23 Apr 2020 01:41:33 GMT
ENV MEMCACHED_SHA1=1ddb5f37f69946b63512ad0f89dc448ff7ba5713
# Sun, 26 Apr 2020 13:18:16 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Sun, 26 Apr 2020 13:18:17 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Sun, 26 Apr 2020 13:18:19 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Sun, 26 Apr 2020 13:18:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sun, 26 Apr 2020 13:18:20 GMT
USER memcache
# Sun, 26 Apr 2020 13:18:20 GMT
EXPOSE 11211
# Sun, 26 Apr 2020 13:18:20 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:ae8f0fa6cb0d971b4b8fedf7fc9b00f61f780b383fe7d64e6c2e4be8d20c3987`  
		Last Modified: Thu, 23 Apr 2020 00:17:46 GMT  
		Size: 25.8 MB (25762125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af60fd257f6555ca6e3d16a15d8ffa2104ab04985a4ed8086673ea9a801fd4e3`  
		Last Modified: Sun, 26 Apr 2020 13:18:38 GMT  
		Size: 5.0 KB (4983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f1056e8039be8264aef0eb2e4da6fc056a4ca433ef9c12b2249c56daa5c80d1`  
		Last Modified: Sun, 26 Apr 2020 13:18:40 GMT  
		Size: 1.8 MB (1775978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11395212b0482ecc9c692dec8ec4b925f6a00bf9e1221b5346ee0e0adaf15bcf`  
		Last Modified: Sun, 26 Apr 2020 13:18:39 GMT  
		Size: 1.2 MB (1181708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b73dfa2d44a3c35a22d2140a094f6791462908f7643607468b7ab494ba8466e`  
		Last Modified: Sun, 26 Apr 2020 13:18:38 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a944298863ce1f89b5fd93b096bb2353280d7b5cd6f08d6e370b80a8624ebe8a`  
		Last Modified: Sun, 26 Apr 2020 13:18:38 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1` - linux; ppc64le

```console
$ docker pull memcached@sha256:72020baf7b956f0e50b60da653793669acfe24dab1c0e03c92e4101756c69870
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.1 MB (34070273 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:13679844e3928d60db09df9f08012634fe562bf0bbe2755d7e8bdfc5a8843dee`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 23 Apr 2020 00:36:00 GMT
ADD file:5b3c3d2945800e1743dc02a4f68bd830fe2f67ca437223692eb460147c158c2b in / 
# Thu, 23 Apr 2020 00:36:04 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 05:29:22 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Thu, 23 Apr 2020 05:29:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 05:29:41 GMT
ENV MEMCACHED_VERSION=1.6.5
# Thu, 23 Apr 2020 05:29:43 GMT
ENV MEMCACHED_SHA1=1ddb5f37f69946b63512ad0f89dc448ff7ba5713
# Thu, 23 Apr 2020 05:39:43 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 23 Apr 2020 05:39:44 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 23 Apr 2020 05:39:48 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 23 Apr 2020 05:39:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Apr 2020 05:39:51 GMT
USER memcache
# Thu, 23 Apr 2020 05:39:53 GMT
EXPOSE 11211
# Thu, 23 Apr 2020 05:39:55 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:012c6cdbd1af202bbfbea5945fafbb9aca9097f1fa3cb493a29155fdc02cc43c`  
		Last Modified: Thu, 23 Apr 2020 00:50:14 GMT  
		Size: 30.5 MB (30524638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca611c057695089b7850ed3bf7f38c5979756d58e7de7d6c7307568e0ac9000d`  
		Last Modified: Thu, 23 Apr 2020 05:40:21 GMT  
		Size: 5.0 KB (4988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e22a29cab6d03b4f3f09bf64881923227d5fc4d38aa6a1c8367751663ed3694a`  
		Last Modified: Thu, 23 Apr 2020 05:40:21 GMT  
		Size: 2.3 MB (2322671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b265c0fd772a3a696cd9c7860788c4e3b7287f882955c5e459a6c41b64a7e531`  
		Last Modified: Thu, 23 Apr 2020 05:40:22 GMT  
		Size: 1.2 MB (1217568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a05552e552ebc4b7164ee3b7161d37f2672294b65d98445aa530535ec57dd7f5`  
		Last Modified: Thu, 23 Apr 2020 05:40:21 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce1f225499a970ebb67b042406d96bb81fe400cc061e7e275de90e73499ca5db`  
		Last Modified: Thu, 23 Apr 2020 05:40:21 GMT  
		Size: 120.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1` - linux; s390x

```console
$ docker pull memcached@sha256:267df373701f14c0f868a2a95f6690723010071a8982a2b6a87f9e4afafb89dc
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.8 MB (28788396 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:be9e90914277188f44c6a29fec5f783023e7665d98f610dc36b3087ae622a8ac`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 23 Apr 2020 00:51:48 GMT
ADD file:f6c2560f9185c1bcaff95e576e57449f606d51b85fad02646c1b0962bc9353c9 in / 
# Thu, 23 Apr 2020 00:51:50 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 00:58:53 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Thu, 23 Apr 2020 00:58:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 13 May 2020 20:34:57 GMT
ENV MEMCACHED_VERSION=1.6.6
# Wed, 13 May 2020 20:34:57 GMT
ENV MEMCACHED_SHA1=d8895b12dc9fc82b389f1713e2c09cc6ca3d03e4
# Wed, 13 May 2020 20:43:55 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 13 May 2020 20:43:55 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 13 May 2020 20:43:56 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 13 May 2020 20:43:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 13 May 2020 20:43:56 GMT
USER memcache
# Wed, 13 May 2020 20:43:56 GMT
EXPOSE 11211
# Wed, 13 May 2020 20:43:57 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:d89dc3741ad42b79c3d8545495c429f3100d3f22234ff993bd04017b0675e868`  
		Last Modified: Thu, 23 Apr 2020 00:56:00 GMT  
		Size: 25.7 MB (25712105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed7b337870b6c06d26297cc61114e98f8d23b6cfd7ceda5779286b09d85058e8`  
		Last Modified: Wed, 13 May 2020 20:53:33 GMT  
		Size: 5.0 KB (5028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c35c02588420fb9764d4f49d302f8e0d38aa8665a3f567a238a90c3be58b6b46`  
		Last Modified: Wed, 13 May 2020 20:53:33 GMT  
		Size: 1.9 MB (1886010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8781268196c7fca5682511a33b8fa3847b89e8a56b81d4a95e45c914b19dbb74`  
		Last Modified: Wed, 13 May 2020 20:53:32 GMT  
		Size: 1.2 MB (1184846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:926216811f65028b36b78fac4d9bd85fa41c2b6b8f07b8bd466207403e99cb38`  
		Last Modified: Wed, 13 May 2020 20:53:38 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6de9b312d644cc1f4014c4aceb68cdca1cc2a710fadeaf50d94511ba356784e`  
		Last Modified: Wed, 13 May 2020 20:53:38 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:1.6`

```console
$ docker pull memcached@sha256:b0f382f16271ffe9dce89bc4d47b8627ae4b491286bec220dadaee3862cdc1e2
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
$ docker pull memcached@sha256:e8c935cf0dfa9eecf9129d9039cfbe12f55c1cecc86902998d4c7c369f5b5a57
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.5 MB (30493690 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9bb369dc76dc6e22e495a01681b1d1c428701d8a06f7304ef333b36f13469e8a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 23 Apr 2020 00:20:32 GMT
ADD file:9b8be2b52ee0fa31da1b6256099030b73546253a57e94cccb24605cd888bb74d in / 
# Thu, 23 Apr 2020 00:20:32 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 03:48:31 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Thu, 23 Apr 2020 03:48:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 13 May 2020 20:57:07 GMT
ENV MEMCACHED_VERSION=1.6.6
# Wed, 13 May 2020 20:57:07 GMT
ENV MEMCACHED_SHA1=d8895b12dc9fc82b389f1713e2c09cc6ca3d03e4
# Wed, 13 May 2020 21:06:31 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 13 May 2020 21:06:31 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 13 May 2020 21:06:32 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 13 May 2020 21:06:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 13 May 2020 21:06:32 GMT
USER memcache
# Wed, 13 May 2020 21:06:32 GMT
EXPOSE 11211
# Wed, 13 May 2020 21:06:32 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:54fec2fa59d0a0de9cd2dec9850b36c43de451f1fd1c0a5bf8f1cf26a61a5da4`  
		Last Modified: Thu, 23 Apr 2020 00:25:10 GMT  
		Size: 27.1 MB (27098254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73a546564c749aeaf996f91019e9cf37b5e395b661aec0dcf2e2c20c11bbda96`  
		Last Modified: Thu, 23 Apr 2020 03:58:00 GMT  
		Size: 5.0 KB (4979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2b17108b143c42eeda6a8587b36cfd6e30c7783fb09e565feb06d09f4172525`  
		Last Modified: Thu, 23 Apr 2020 03:58:01 GMT  
		Size: 2.2 MB (2196403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a1e9dd08a002476ba6cade3017e17f464968c8e94877292d07c5b899a9e8d3a`  
		Last Modified: Wed, 13 May 2020 21:16:44 GMT  
		Size: 1.2 MB (1193645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09cafd6239484b297ad595f395a878b6ce07eefcca9de92a17910aa735abe6d5`  
		Last Modified: Wed, 13 May 2020 21:16:44 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48b6890ea4c000ff4ec7834a60a4422aaa4e75ac040f107523b1a2c653b6a4b4`  
		Last Modified: Wed, 13 May 2020 21:16:43 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6` - linux; arm variant v5

```console
$ docker pull memcached@sha256:d430d81aec7724f5662cd0dad2554d354921139f129ec60d96fcd97d835a68e5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.9 MB (27901495 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d38f156a5705d867b8698bf28f60397b2ccaa27ebd90a3a370e641ea8836fea3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 23 Apr 2020 00:52:22 GMT
ADD file:62a9732be4e3237ccc896f724a34606e01f351c4877e52c9a9cd85029c06b956 in / 
# Thu, 23 Apr 2020 00:52:23 GMT
CMD ["bash"]
# Mon, 27 Apr 2020 20:31:39 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Mon, 27 Apr 2020 20:31:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 13 May 2020 20:49:55 GMT
ENV MEMCACHED_VERSION=1.6.6
# Wed, 13 May 2020 20:49:56 GMT
ENV MEMCACHED_SHA1=d8895b12dc9fc82b389f1713e2c09cc6ca3d03e4
# Wed, 13 May 2020 21:01:00 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 13 May 2020 21:01:01 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 13 May 2020 21:01:03 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 13 May 2020 21:01:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 13 May 2020 21:01:05 GMT
USER memcache
# Wed, 13 May 2020 21:01:06 GMT
EXPOSE 11211
# Wed, 13 May 2020 21:01:07 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:a8c46e5952878f9f324df86c5a2b45b2e0020f6721e820981e74461d77a100dd`  
		Last Modified: Thu, 23 Apr 2020 00:59:50 GMT  
		Size: 24.8 MB (24836319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0e09e82475aef1e3124cd928ab36f48dd86a0421490ff8d8eab1ae848dbf6e6`  
		Last Modified: Mon, 27 Apr 2020 20:41:52 GMT  
		Size: 4.9 KB (4901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ed2c941c8d2e3eb09c1ec4cf66006155ff9774d385e99a0fe1de44269bfcb8a`  
		Last Modified: Mon, 27 Apr 2020 20:41:53 GMT  
		Size: 1.9 MB (1896804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:114ca507809768dd949fd745f46978c84751747b86a1b70e2d2e8681f85bb5c7`  
		Last Modified: Wed, 13 May 2020 21:01:32 GMT  
		Size: 1.2 MB (1163062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8325227257270f7e70028b55a4b9824a561441cc464ec94298af0caeb3ae7c7`  
		Last Modified: Wed, 13 May 2020 21:01:32 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65eb2dfc473e854cbe271a2fa75b0ee74363953ba9d80a4dfefc1954d1430c0f`  
		Last Modified: Wed, 13 May 2020 21:01:31 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6` - linux; arm variant v7

```console
$ docker pull memcached@sha256:8c0e9908733d5c2401b24e506567ca9ad0b6756c2c92d04b46e2d58eeff0b944
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.7 MB (25656893 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c9b4186eea9043000afc5ff47c169dae434c62ad0d68ef804b36ec022967aeec`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 23 Apr 2020 01:03:26 GMT
ADD file:db6122b36f3e70c5f490b50afba99d49fa345f11d0f5c77bb3c6749f8e2a4f81 in / 
# Thu, 23 Apr 2020 01:03:28 GMT
CMD ["bash"]
# Mon, 27 Apr 2020 20:31:45 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Mon, 27 Apr 2020 20:31:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 13 May 2020 20:49:59 GMT
ENV MEMCACHED_VERSION=1.6.6
# Wed, 13 May 2020 20:49:59 GMT
ENV MEMCACHED_SHA1=d8895b12dc9fc82b389f1713e2c09cc6ca3d03e4
# Wed, 13 May 2020 21:00:32 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 13 May 2020 21:00:33 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 13 May 2020 21:00:35 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 13 May 2020 21:00:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 13 May 2020 21:00:36 GMT
USER memcache
# Wed, 13 May 2020 21:00:37 GMT
EXPOSE 11211
# Wed, 13 May 2020 21:00:38 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:50fb0052086928803f00724ca465c89c45dde5b082b1e59dadb8101286dd5ab6`  
		Last Modified: Thu, 23 Apr 2020 01:11:08 GMT  
		Size: 22.7 MB (22705377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ae844ffae38c0aae3794728fe7c89bff09b70d2226e7b0775beab756cc93856`  
		Last Modified: Mon, 27 Apr 2020 20:50:45 GMT  
		Size: 4.9 KB (4898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6003a4985eba124dc101599be1daf743ce2f44e09d30ea54bf909540aa150a8`  
		Last Modified: Mon, 27 Apr 2020 20:50:45 GMT  
		Size: 1.8 MB (1811519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23bc49c42147e3c6c4bae63d2570761c08ef7aaefc2c07b43258c53f9e8865c9`  
		Last Modified: Wed, 13 May 2020 21:11:35 GMT  
		Size: 1.1 MB (1134692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea93b4316081dba615b7e4d490934ed3ec3cf7979bf5200d7455309149f554c2`  
		Last Modified: Wed, 13 May 2020 21:11:35 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c26e78f516132b9ab5e5b47948d2171d973044571df9d3fcfef732b08086425`  
		Last Modified: Wed, 13 May 2020 21:11:34 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:d423b2ef6d053c533639c07693e0cfca1ccb8715b1825c9dd09a5e8754ab1af7
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.1 MB (29102138 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d2b62ffbdd70a7d226f91ebe12b68d7ad5b580ea2fdb690621b441e7a64b2ab`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 23 Apr 2020 00:54:55 GMT
ADD file:581ee9c3c19f0d971aeda008fd399f59171cae75e8936b967dbf3888db4fc0d0 in / 
# Thu, 23 Apr 2020 00:54:58 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 03:03:20 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Thu, 23 Apr 2020 03:03:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 13 May 2020 20:56:07 GMT
ENV MEMCACHED_VERSION=1.6.6
# Wed, 13 May 2020 20:56:08 GMT
ENV MEMCACHED_SHA1=d8895b12dc9fc82b389f1713e2c09cc6ca3d03e4
# Wed, 13 May 2020 21:06:19 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 13 May 2020 21:06:20 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 13 May 2020 21:06:22 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 13 May 2020 21:06:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 13 May 2020 21:06:23 GMT
USER memcache
# Wed, 13 May 2020 21:06:24 GMT
EXPOSE 11211
# Wed, 13 May 2020 21:06:24 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:bdc84a41f2513e28e99efeff9fcbb196b7df9883fb30532184bd67ca415b4673`  
		Last Modified: Thu, 23 Apr 2020 01:03:27 GMT  
		Size: 25.9 MB (25857800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b8ed987f36e3ad8893c5c7ce9e42aeb35d67e90daf262dde60d86dfa94814f5`  
		Last Modified: Thu, 23 Apr 2020 03:32:22 GMT  
		Size: 5.0 KB (5028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:360e6a91a753e3a018e26a9d22b25766c2ebd2231cbc3e245648aead98ddde08`  
		Last Modified: Thu, 23 Apr 2020 03:32:23 GMT  
		Size: 2.1 MB (2074961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9beea1961eacb995614a88fb9793f9a187c12a86f94a6be75130effc76976768`  
		Last Modified: Wed, 13 May 2020 21:17:27 GMT  
		Size: 1.2 MB (1163938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b48ab287b49fd3b8a7f96050d1d72454c2581bae20dbdd2d52ec0d9766d2d56`  
		Last Modified: Wed, 13 May 2020 21:17:26 GMT  
		Size: 290.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dce9e28ac95b05cd478c90cb28edf8e74c70f8fc79bd3acde6d5104bd563f32b`  
		Last Modified: Wed, 13 May 2020 21:17:25 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6` - linux; 386

```console
$ docker pull memcached@sha256:4cd7c8a145c4b502f84c55f41e0ae4971614a237b96076093edb951df16af86f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.2 MB (31163013 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66532fde035d2034732c7b657027f1f342acdb811b1d859d9f6ed3bc370262e2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 23 Apr 2020 00:39:36 GMT
ADD file:ca6a74f6b738c738c033152fab2a9aacf22bec5f19a994e6a02b5f919ee33ee9 in / 
# Thu, 23 Apr 2020 00:39:36 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 01:29:35 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Thu, 23 Apr 2020 01:29:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 01:29:42 GMT
ENV MEMCACHED_VERSION=1.6.5
# Thu, 23 Apr 2020 01:29:42 GMT
ENV MEMCACHED_SHA1=1ddb5f37f69946b63512ad0f89dc448ff7ba5713
# Thu, 23 Apr 2020 01:38:20 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 23 Apr 2020 01:38:20 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 23 Apr 2020 01:38:21 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 23 Apr 2020 01:38:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Apr 2020 01:38:21 GMT
USER memcache
# Thu, 23 Apr 2020 01:38:21 GMT
EXPOSE 11211
# Thu, 23 Apr 2020 01:38:21 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:5d3da8f33b97fc107a05b3255a55836b76df9f817de632b1fb63c6e9c024f0df`  
		Last Modified: Thu, 23 Apr 2020 00:44:35 GMT  
		Size: 27.8 MB (27753972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c3cb2639d5e9c8ab44fd2bbe5bedbb5c4d33378f9781d558d2ac27611ecd673`  
		Last Modified: Thu, 23 Apr 2020 01:38:35 GMT  
		Size: 4.9 KB (4898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6f2f84fd6631cbca67ed46fd3b380a42475afb287d8e990ded3d3a91fded71a`  
		Last Modified: Thu, 23 Apr 2020 01:38:35 GMT  
		Size: 2.2 MB (2208055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae882751a1fc445bebd4d4f545c0c69529396863b7ac0b3fc3137b2c3cecbfaa`  
		Last Modified: Thu, 23 Apr 2020 01:38:35 GMT  
		Size: 1.2 MB (1195679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d53c7886eeb4da4192fe5caceac337d1fa31afc20be46a9476fd10e35bd4d81e`  
		Last Modified: Thu, 23 Apr 2020 01:38:35 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43f9bc6252b62803993a04eff4ad6e08d728474f2c446e92d32b5ab3ac38ab08`  
		Last Modified: Thu, 23 Apr 2020 01:38:35 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6` - linux; mips64le

```console
$ docker pull memcached@sha256:2b4b9c9aba5b7a352d4f631bfdf5b38489d2e2ea2bb40ce5c0d592d2f3beb517
```

-	Docker Version: 19.03.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.7 MB (28725203 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:53b77428fcdf16a094d4463e769da9547573740a8f4723c8951289da773cd5a4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 23 Apr 2020 00:09:47 GMT
ADD file:7509945bd8a224048260e88b466aa3b156615e16b64e0a6702da277052fcb98b in / 
# Thu, 23 Apr 2020 00:09:48 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 01:41:19 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Thu, 23 Apr 2020 01:41:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 01:41:33 GMT
ENV MEMCACHED_VERSION=1.6.5
# Thu, 23 Apr 2020 01:41:33 GMT
ENV MEMCACHED_SHA1=1ddb5f37f69946b63512ad0f89dc448ff7ba5713
# Sun, 26 Apr 2020 13:18:16 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Sun, 26 Apr 2020 13:18:17 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Sun, 26 Apr 2020 13:18:19 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Sun, 26 Apr 2020 13:18:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sun, 26 Apr 2020 13:18:20 GMT
USER memcache
# Sun, 26 Apr 2020 13:18:20 GMT
EXPOSE 11211
# Sun, 26 Apr 2020 13:18:20 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:ae8f0fa6cb0d971b4b8fedf7fc9b00f61f780b383fe7d64e6c2e4be8d20c3987`  
		Last Modified: Thu, 23 Apr 2020 00:17:46 GMT  
		Size: 25.8 MB (25762125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af60fd257f6555ca6e3d16a15d8ffa2104ab04985a4ed8086673ea9a801fd4e3`  
		Last Modified: Sun, 26 Apr 2020 13:18:38 GMT  
		Size: 5.0 KB (4983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f1056e8039be8264aef0eb2e4da6fc056a4ca433ef9c12b2249c56daa5c80d1`  
		Last Modified: Sun, 26 Apr 2020 13:18:40 GMT  
		Size: 1.8 MB (1775978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11395212b0482ecc9c692dec8ec4b925f6a00bf9e1221b5346ee0e0adaf15bcf`  
		Last Modified: Sun, 26 Apr 2020 13:18:39 GMT  
		Size: 1.2 MB (1181708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b73dfa2d44a3c35a22d2140a094f6791462908f7643607468b7ab494ba8466e`  
		Last Modified: Sun, 26 Apr 2020 13:18:38 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a944298863ce1f89b5fd93b096bb2353280d7b5cd6f08d6e370b80a8624ebe8a`  
		Last Modified: Sun, 26 Apr 2020 13:18:38 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6` - linux; ppc64le

```console
$ docker pull memcached@sha256:72020baf7b956f0e50b60da653793669acfe24dab1c0e03c92e4101756c69870
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.1 MB (34070273 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:13679844e3928d60db09df9f08012634fe562bf0bbe2755d7e8bdfc5a8843dee`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 23 Apr 2020 00:36:00 GMT
ADD file:5b3c3d2945800e1743dc02a4f68bd830fe2f67ca437223692eb460147c158c2b in / 
# Thu, 23 Apr 2020 00:36:04 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 05:29:22 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Thu, 23 Apr 2020 05:29:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 05:29:41 GMT
ENV MEMCACHED_VERSION=1.6.5
# Thu, 23 Apr 2020 05:29:43 GMT
ENV MEMCACHED_SHA1=1ddb5f37f69946b63512ad0f89dc448ff7ba5713
# Thu, 23 Apr 2020 05:39:43 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 23 Apr 2020 05:39:44 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 23 Apr 2020 05:39:48 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 23 Apr 2020 05:39:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Apr 2020 05:39:51 GMT
USER memcache
# Thu, 23 Apr 2020 05:39:53 GMT
EXPOSE 11211
# Thu, 23 Apr 2020 05:39:55 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:012c6cdbd1af202bbfbea5945fafbb9aca9097f1fa3cb493a29155fdc02cc43c`  
		Last Modified: Thu, 23 Apr 2020 00:50:14 GMT  
		Size: 30.5 MB (30524638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca611c057695089b7850ed3bf7f38c5979756d58e7de7d6c7307568e0ac9000d`  
		Last Modified: Thu, 23 Apr 2020 05:40:21 GMT  
		Size: 5.0 KB (4988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e22a29cab6d03b4f3f09bf64881923227d5fc4d38aa6a1c8367751663ed3694a`  
		Last Modified: Thu, 23 Apr 2020 05:40:21 GMT  
		Size: 2.3 MB (2322671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b265c0fd772a3a696cd9c7860788c4e3b7287f882955c5e459a6c41b64a7e531`  
		Last Modified: Thu, 23 Apr 2020 05:40:22 GMT  
		Size: 1.2 MB (1217568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a05552e552ebc4b7164ee3b7161d37f2672294b65d98445aa530535ec57dd7f5`  
		Last Modified: Thu, 23 Apr 2020 05:40:21 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce1f225499a970ebb67b042406d96bb81fe400cc061e7e275de90e73499ca5db`  
		Last Modified: Thu, 23 Apr 2020 05:40:21 GMT  
		Size: 120.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6` - linux; s390x

```console
$ docker pull memcached@sha256:267df373701f14c0f868a2a95f6690723010071a8982a2b6a87f9e4afafb89dc
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.8 MB (28788396 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:be9e90914277188f44c6a29fec5f783023e7665d98f610dc36b3087ae622a8ac`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 23 Apr 2020 00:51:48 GMT
ADD file:f6c2560f9185c1bcaff95e576e57449f606d51b85fad02646c1b0962bc9353c9 in / 
# Thu, 23 Apr 2020 00:51:50 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 00:58:53 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Thu, 23 Apr 2020 00:58:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 13 May 2020 20:34:57 GMT
ENV MEMCACHED_VERSION=1.6.6
# Wed, 13 May 2020 20:34:57 GMT
ENV MEMCACHED_SHA1=d8895b12dc9fc82b389f1713e2c09cc6ca3d03e4
# Wed, 13 May 2020 20:43:55 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 13 May 2020 20:43:55 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 13 May 2020 20:43:56 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 13 May 2020 20:43:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 13 May 2020 20:43:56 GMT
USER memcache
# Wed, 13 May 2020 20:43:56 GMT
EXPOSE 11211
# Wed, 13 May 2020 20:43:57 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:d89dc3741ad42b79c3d8545495c429f3100d3f22234ff993bd04017b0675e868`  
		Last Modified: Thu, 23 Apr 2020 00:56:00 GMT  
		Size: 25.7 MB (25712105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed7b337870b6c06d26297cc61114e98f8d23b6cfd7ceda5779286b09d85058e8`  
		Last Modified: Wed, 13 May 2020 20:53:33 GMT  
		Size: 5.0 KB (5028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c35c02588420fb9764d4f49d302f8e0d38aa8665a3f567a238a90c3be58b6b46`  
		Last Modified: Wed, 13 May 2020 20:53:33 GMT  
		Size: 1.9 MB (1886010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8781268196c7fca5682511a33b8fa3847b89e8a56b81d4a95e45c914b19dbb74`  
		Last Modified: Wed, 13 May 2020 20:53:32 GMT  
		Size: 1.2 MB (1184846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:926216811f65028b36b78fac4d9bd85fa41c2b6b8f07b8bd466207403e99cb38`  
		Last Modified: Wed, 13 May 2020 20:53:38 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6de9b312d644cc1f4014c4aceb68cdca1cc2a710fadeaf50d94511ba356784e`  
		Last Modified: Wed, 13 May 2020 20:53:38 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:1.6.6`

```console
$ docker pull memcached@sha256:1d85c975741d4681e8e2bc4f3d1f4dbc0ce48875fa079bdb4aa912a1d9fd6dc7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; s390x

### `memcached:1.6.6` - linux; amd64

```console
$ docker pull memcached@sha256:e8c935cf0dfa9eecf9129d9039cfbe12f55c1cecc86902998d4c7c369f5b5a57
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.5 MB (30493690 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9bb369dc76dc6e22e495a01681b1d1c428701d8a06f7304ef333b36f13469e8a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 23 Apr 2020 00:20:32 GMT
ADD file:9b8be2b52ee0fa31da1b6256099030b73546253a57e94cccb24605cd888bb74d in / 
# Thu, 23 Apr 2020 00:20:32 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 03:48:31 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Thu, 23 Apr 2020 03:48:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 13 May 2020 20:57:07 GMT
ENV MEMCACHED_VERSION=1.6.6
# Wed, 13 May 2020 20:57:07 GMT
ENV MEMCACHED_SHA1=d8895b12dc9fc82b389f1713e2c09cc6ca3d03e4
# Wed, 13 May 2020 21:06:31 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 13 May 2020 21:06:31 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 13 May 2020 21:06:32 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 13 May 2020 21:06:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 13 May 2020 21:06:32 GMT
USER memcache
# Wed, 13 May 2020 21:06:32 GMT
EXPOSE 11211
# Wed, 13 May 2020 21:06:32 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:54fec2fa59d0a0de9cd2dec9850b36c43de451f1fd1c0a5bf8f1cf26a61a5da4`  
		Last Modified: Thu, 23 Apr 2020 00:25:10 GMT  
		Size: 27.1 MB (27098254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73a546564c749aeaf996f91019e9cf37b5e395b661aec0dcf2e2c20c11bbda96`  
		Last Modified: Thu, 23 Apr 2020 03:58:00 GMT  
		Size: 5.0 KB (4979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2b17108b143c42eeda6a8587b36cfd6e30c7783fb09e565feb06d09f4172525`  
		Last Modified: Thu, 23 Apr 2020 03:58:01 GMT  
		Size: 2.2 MB (2196403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a1e9dd08a002476ba6cade3017e17f464968c8e94877292d07c5b899a9e8d3a`  
		Last Modified: Wed, 13 May 2020 21:16:44 GMT  
		Size: 1.2 MB (1193645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09cafd6239484b297ad595f395a878b6ce07eefcca9de92a17910aa735abe6d5`  
		Last Modified: Wed, 13 May 2020 21:16:44 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48b6890ea4c000ff4ec7834a60a4422aaa4e75ac040f107523b1a2c653b6a4b4`  
		Last Modified: Wed, 13 May 2020 21:16:43 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.6` - linux; arm variant v5

```console
$ docker pull memcached@sha256:d430d81aec7724f5662cd0dad2554d354921139f129ec60d96fcd97d835a68e5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.9 MB (27901495 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d38f156a5705d867b8698bf28f60397b2ccaa27ebd90a3a370e641ea8836fea3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 23 Apr 2020 00:52:22 GMT
ADD file:62a9732be4e3237ccc896f724a34606e01f351c4877e52c9a9cd85029c06b956 in / 
# Thu, 23 Apr 2020 00:52:23 GMT
CMD ["bash"]
# Mon, 27 Apr 2020 20:31:39 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Mon, 27 Apr 2020 20:31:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 13 May 2020 20:49:55 GMT
ENV MEMCACHED_VERSION=1.6.6
# Wed, 13 May 2020 20:49:56 GMT
ENV MEMCACHED_SHA1=d8895b12dc9fc82b389f1713e2c09cc6ca3d03e4
# Wed, 13 May 2020 21:01:00 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 13 May 2020 21:01:01 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 13 May 2020 21:01:03 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 13 May 2020 21:01:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 13 May 2020 21:01:05 GMT
USER memcache
# Wed, 13 May 2020 21:01:06 GMT
EXPOSE 11211
# Wed, 13 May 2020 21:01:07 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:a8c46e5952878f9f324df86c5a2b45b2e0020f6721e820981e74461d77a100dd`  
		Last Modified: Thu, 23 Apr 2020 00:59:50 GMT  
		Size: 24.8 MB (24836319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0e09e82475aef1e3124cd928ab36f48dd86a0421490ff8d8eab1ae848dbf6e6`  
		Last Modified: Mon, 27 Apr 2020 20:41:52 GMT  
		Size: 4.9 KB (4901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ed2c941c8d2e3eb09c1ec4cf66006155ff9774d385e99a0fe1de44269bfcb8a`  
		Last Modified: Mon, 27 Apr 2020 20:41:53 GMT  
		Size: 1.9 MB (1896804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:114ca507809768dd949fd745f46978c84751747b86a1b70e2d2e8681f85bb5c7`  
		Last Modified: Wed, 13 May 2020 21:01:32 GMT  
		Size: 1.2 MB (1163062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8325227257270f7e70028b55a4b9824a561441cc464ec94298af0caeb3ae7c7`  
		Last Modified: Wed, 13 May 2020 21:01:32 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65eb2dfc473e854cbe271a2fa75b0ee74363953ba9d80a4dfefc1954d1430c0f`  
		Last Modified: Wed, 13 May 2020 21:01:31 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.6` - linux; arm variant v7

```console
$ docker pull memcached@sha256:8c0e9908733d5c2401b24e506567ca9ad0b6756c2c92d04b46e2d58eeff0b944
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.7 MB (25656893 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c9b4186eea9043000afc5ff47c169dae434c62ad0d68ef804b36ec022967aeec`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 23 Apr 2020 01:03:26 GMT
ADD file:db6122b36f3e70c5f490b50afba99d49fa345f11d0f5c77bb3c6749f8e2a4f81 in / 
# Thu, 23 Apr 2020 01:03:28 GMT
CMD ["bash"]
# Mon, 27 Apr 2020 20:31:45 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Mon, 27 Apr 2020 20:31:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 13 May 2020 20:49:59 GMT
ENV MEMCACHED_VERSION=1.6.6
# Wed, 13 May 2020 20:49:59 GMT
ENV MEMCACHED_SHA1=d8895b12dc9fc82b389f1713e2c09cc6ca3d03e4
# Wed, 13 May 2020 21:00:32 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 13 May 2020 21:00:33 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 13 May 2020 21:00:35 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 13 May 2020 21:00:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 13 May 2020 21:00:36 GMT
USER memcache
# Wed, 13 May 2020 21:00:37 GMT
EXPOSE 11211
# Wed, 13 May 2020 21:00:38 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:50fb0052086928803f00724ca465c89c45dde5b082b1e59dadb8101286dd5ab6`  
		Last Modified: Thu, 23 Apr 2020 01:11:08 GMT  
		Size: 22.7 MB (22705377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ae844ffae38c0aae3794728fe7c89bff09b70d2226e7b0775beab756cc93856`  
		Last Modified: Mon, 27 Apr 2020 20:50:45 GMT  
		Size: 4.9 KB (4898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6003a4985eba124dc101599be1daf743ce2f44e09d30ea54bf909540aa150a8`  
		Last Modified: Mon, 27 Apr 2020 20:50:45 GMT  
		Size: 1.8 MB (1811519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23bc49c42147e3c6c4bae63d2570761c08ef7aaefc2c07b43258c53f9e8865c9`  
		Last Modified: Wed, 13 May 2020 21:11:35 GMT  
		Size: 1.1 MB (1134692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea93b4316081dba615b7e4d490934ed3ec3cf7979bf5200d7455309149f554c2`  
		Last Modified: Wed, 13 May 2020 21:11:35 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c26e78f516132b9ab5e5b47948d2171d973044571df9d3fcfef732b08086425`  
		Last Modified: Wed, 13 May 2020 21:11:34 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.6` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:d423b2ef6d053c533639c07693e0cfca1ccb8715b1825c9dd09a5e8754ab1af7
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.1 MB (29102138 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d2b62ffbdd70a7d226f91ebe12b68d7ad5b580ea2fdb690621b441e7a64b2ab`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 23 Apr 2020 00:54:55 GMT
ADD file:581ee9c3c19f0d971aeda008fd399f59171cae75e8936b967dbf3888db4fc0d0 in / 
# Thu, 23 Apr 2020 00:54:58 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 03:03:20 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Thu, 23 Apr 2020 03:03:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 13 May 2020 20:56:07 GMT
ENV MEMCACHED_VERSION=1.6.6
# Wed, 13 May 2020 20:56:08 GMT
ENV MEMCACHED_SHA1=d8895b12dc9fc82b389f1713e2c09cc6ca3d03e4
# Wed, 13 May 2020 21:06:19 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 13 May 2020 21:06:20 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 13 May 2020 21:06:22 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 13 May 2020 21:06:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 13 May 2020 21:06:23 GMT
USER memcache
# Wed, 13 May 2020 21:06:24 GMT
EXPOSE 11211
# Wed, 13 May 2020 21:06:24 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:bdc84a41f2513e28e99efeff9fcbb196b7df9883fb30532184bd67ca415b4673`  
		Last Modified: Thu, 23 Apr 2020 01:03:27 GMT  
		Size: 25.9 MB (25857800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b8ed987f36e3ad8893c5c7ce9e42aeb35d67e90daf262dde60d86dfa94814f5`  
		Last Modified: Thu, 23 Apr 2020 03:32:22 GMT  
		Size: 5.0 KB (5028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:360e6a91a753e3a018e26a9d22b25766c2ebd2231cbc3e245648aead98ddde08`  
		Last Modified: Thu, 23 Apr 2020 03:32:23 GMT  
		Size: 2.1 MB (2074961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9beea1961eacb995614a88fb9793f9a187c12a86f94a6be75130effc76976768`  
		Last Modified: Wed, 13 May 2020 21:17:27 GMT  
		Size: 1.2 MB (1163938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b48ab287b49fd3b8a7f96050d1d72454c2581bae20dbdd2d52ec0d9766d2d56`  
		Last Modified: Wed, 13 May 2020 21:17:26 GMT  
		Size: 290.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dce9e28ac95b05cd478c90cb28edf8e74c70f8fc79bd3acde6d5104bd563f32b`  
		Last Modified: Wed, 13 May 2020 21:17:25 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.6` - linux; s390x

```console
$ docker pull memcached@sha256:267df373701f14c0f868a2a95f6690723010071a8982a2b6a87f9e4afafb89dc
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.8 MB (28788396 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:be9e90914277188f44c6a29fec5f783023e7665d98f610dc36b3087ae622a8ac`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 23 Apr 2020 00:51:48 GMT
ADD file:f6c2560f9185c1bcaff95e576e57449f606d51b85fad02646c1b0962bc9353c9 in / 
# Thu, 23 Apr 2020 00:51:50 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 00:58:53 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Thu, 23 Apr 2020 00:58:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 13 May 2020 20:34:57 GMT
ENV MEMCACHED_VERSION=1.6.6
# Wed, 13 May 2020 20:34:57 GMT
ENV MEMCACHED_SHA1=d8895b12dc9fc82b389f1713e2c09cc6ca3d03e4
# Wed, 13 May 2020 20:43:55 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 13 May 2020 20:43:55 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 13 May 2020 20:43:56 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 13 May 2020 20:43:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 13 May 2020 20:43:56 GMT
USER memcache
# Wed, 13 May 2020 20:43:56 GMT
EXPOSE 11211
# Wed, 13 May 2020 20:43:57 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:d89dc3741ad42b79c3d8545495c429f3100d3f22234ff993bd04017b0675e868`  
		Last Modified: Thu, 23 Apr 2020 00:56:00 GMT  
		Size: 25.7 MB (25712105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed7b337870b6c06d26297cc61114e98f8d23b6cfd7ceda5779286b09d85058e8`  
		Last Modified: Wed, 13 May 2020 20:53:33 GMT  
		Size: 5.0 KB (5028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c35c02588420fb9764d4f49d302f8e0d38aa8665a3f567a238a90c3be58b6b46`  
		Last Modified: Wed, 13 May 2020 20:53:33 GMT  
		Size: 1.9 MB (1886010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8781268196c7fca5682511a33b8fa3847b89e8a56b81d4a95e45c914b19dbb74`  
		Last Modified: Wed, 13 May 2020 20:53:32 GMT  
		Size: 1.2 MB (1184846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:926216811f65028b36b78fac4d9bd85fa41c2b6b8f07b8bd466207403e99cb38`  
		Last Modified: Wed, 13 May 2020 20:53:38 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6de9b312d644cc1f4014c4aceb68cdca1cc2a710fadeaf50d94511ba356784e`  
		Last Modified: Wed, 13 May 2020 20:53:38 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:1.6.6-alpine`

```console
$ docker pull memcached@sha256:912bacbe6fb85388691cb0b4376f8b16e770afb586482d4dfb1f2df129b0297e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; s390x

### `memcached:1.6.6-alpine` - linux; amd64

```console
$ docker pull memcached@sha256:7aff4ef05d45a680295a97643acd5c8fd1b306697df52b9b99d3c5665cc91520
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.4 MB (4383824 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:35acd9837d07e6369afd8683ae08f7da10de93ea5d50e74050abbdeece1e6754`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:03 GMT
ADD file:b91adb67b670d3a6ff9463e48b7def903ed516be66fc4282d22c53e41512be49 in / 
# Fri, 24 Apr 2020 01:05:03 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 17:02:57 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Fri, 24 Apr 2020 17:02:58 GMT
RUN apk add --no-cache cyrus-sasl-plain
# Wed, 13 May 2020 21:06:46 GMT
ENV MEMCACHED_VERSION=1.6.6
# Wed, 13 May 2020 21:06:46 GMT
ENV MEMCACHED_SHA1=d8895b12dc9fc82b389f1713e2c09cc6ca3d03e4
# Wed, 13 May 2020 21:16:24 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		dpkg-dev dpkg 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		tar 		wget 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& make test 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Wed, 13 May 2020 21:16:24 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 13 May 2020 21:16:25 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 13 May 2020 21:16:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 13 May 2020 21:16:25 GMT
USER memcache
# Wed, 13 May 2020 21:16:25 GMT
EXPOSE 11211
# Wed, 13 May 2020 21:16:25 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:cbdbe7a5bc2a134ca8ec91be58565ec07d037386d1f1d8385412d224deafca08`  
		Last Modified: Thu, 23 Apr 2020 14:07:19 GMT  
		Size: 2.8 MB (2813316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b534c8dcbed02f81e7238c6977e5e3c22aa347c9d8967b7c12c392ee7a9f548b`  
		Last Modified: Fri, 24 Apr 2020 17:11:25 GMT  
		Size: 1.2 KB (1229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f82e93b65d94a9b03ff2f6758b7ad7c93eceeecf3e1310ba5c7160af4fd59962`  
		Last Modified: Fri, 24 Apr 2020 17:11:25 GMT  
		Size: 15.1 KB (15096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea07733e4053c9b83448decf54f501b7f1fc49e3dcd8d3765c66f476df674fab`  
		Last Modified: Wed, 13 May 2020 21:16:49 GMT  
		Size: 1.6 MB (1553777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa95676f933fd0bbc2cc1615e9449e9122b4a5129fbdaff414a28df5cad88222`  
		Last Modified: Wed, 13 May 2020 21:16:49 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2198a28066da8054936ad286e306fb5694ee81c36f612760266d1ca33e9563b`  
		Last Modified: Wed, 13 May 2020 21:16:49 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.6-alpine` - linux; arm variant v6

```console
$ docker pull memcached@sha256:cdedb0318507c578a21a481fbac96717787aaea12acc53f151332ad36dc72a3e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4153141 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:84637e955a61c7f56159f60a65b17b892fe5ac952e43227f0d2725ae342bbd90`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 23 Apr 2020 15:51:24 GMT
ADD file:cc0770cddff6b50d5e31f39886420eb8a0b4af55664d6f7599207c9aeaf6a501 in / 
# Thu, 23 Apr 2020 15:51:25 GMT
CMD ["/bin/sh"]
# Thu, 23 Apr 2020 18:17:02 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Thu, 23 Apr 2020 18:17:05 GMT
RUN apk add --no-cache cyrus-sasl-plain
# Wed, 13 May 2020 20:48:09 GMT
ENV MEMCACHED_VERSION=1.6.6
# Wed, 13 May 2020 20:48:09 GMT
ENV MEMCACHED_SHA1=d8895b12dc9fc82b389f1713e2c09cc6ca3d03e4
# Wed, 13 May 2020 20:58:49 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		dpkg-dev dpkg 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		tar 		wget 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& make test 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Wed, 13 May 2020 20:58:50 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 13 May 2020 20:58:51 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 13 May 2020 20:58:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 13 May 2020 20:58:53 GMT
USER memcache
# Wed, 13 May 2020 20:58:53 GMT
EXPOSE 11211
# Wed, 13 May 2020 20:58:54 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:b9e3228833e92f0688e0f87234e75965e62e47cfbb9ca8cc5fa19c2e7cd13f80`  
		Last Modified: Thu, 23 Apr 2020 15:52:05 GMT  
		Size: 2.6 MB (2619936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93317744ae21705795946b5f7ccb9e69cd54b0d5b2bdbf48e38bc24ab2037dd4`  
		Last Modified: Thu, 23 Apr 2020 18:26:46 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22d5a6e65917b2d4ecdcd28e7178c79f43bd5cceabca1d40ef2708e66642b656`  
		Last Modified: Thu, 23 Apr 2020 18:26:47 GMT  
		Size: 14.7 KB (14705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55286676201b8c21a4a24628ece19d15221ee259c5df155ebcd0793841211612`  
		Last Modified: Wed, 13 May 2020 20:59:13 GMT  
		Size: 1.5 MB (1516837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c924249be839e9ffa60f403cf731eca93b38caa4e09dc57769e4cc25bcb5ca1`  
		Last Modified: Wed, 13 May 2020 20:59:13 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ded1f200c6c3b6d497cbb1a7fc81bd1ee1dd0cf53a43a8b068ce134ec3c7ab1`  
		Last Modified: Wed, 13 May 2020 20:59:12 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.6-alpine` - linux; arm variant v7

```console
$ docker pull memcached@sha256:b8d5715c8f0905fd1d24efc8254baa1ccf6933d9942b0b84c66750a5662bb811
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3841215 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:331fbc8dc15f015e7fdd524a348b69696983085d2badb3a9a53cb7424a30567d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 23 Apr 2020 22:04:19 GMT
ADD file:33578d3cacfab86c195d99396dd012ec511796a1d2d8d6f0a02b8a055673c294 in / 
# Thu, 23 Apr 2020 22:04:22 GMT
CMD ["/bin/sh"]
# Mon, 27 Apr 2020 20:41:10 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Mon, 27 Apr 2020 20:41:12 GMT
RUN apk add --no-cache cyrus-sasl-plain
# Wed, 13 May 2020 21:00:46 GMT
ENV MEMCACHED_VERSION=1.6.6
# Wed, 13 May 2020 21:00:47 GMT
ENV MEMCACHED_SHA1=d8895b12dc9fc82b389f1713e2c09cc6ca3d03e4
# Wed, 13 May 2020 21:11:09 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		dpkg-dev dpkg 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		tar 		wget 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& make test 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Wed, 13 May 2020 21:11:10 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 13 May 2020 21:11:12 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 13 May 2020 21:11:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 13 May 2020 21:11:13 GMT
USER memcache
# Wed, 13 May 2020 21:11:13 GMT
EXPOSE 11211
# Wed, 13 May 2020 21:11:14 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:3cfb62949d9d8613854db4d5fe502a9219c2b55a153043500078a64e880ae234`  
		Last Modified: Thu, 23 Apr 2020 22:05:12 GMT  
		Size: 2.4 MB (2422063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea5eed70290b5b33d1d0a27554b33b5998613f63667c5797fee672c96ea93df4`  
		Last Modified: Mon, 27 Apr 2020 20:50:54 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea75d9462432267b72327c7684218d1e4d40ec6d9b6578b0e8b79fdc50e2f99b`  
		Last Modified: Mon, 27 Apr 2020 20:50:54 GMT  
		Size: 13.6 KB (13633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e2c49241690acb15f16b690b318be68612c6665317e6f7f8b4cc57b57df0d59`  
		Last Modified: Wed, 13 May 2020 21:11:45 GMT  
		Size: 1.4 MB (1403856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b9dc2878fb274ac6ea5501d45e6a552af904357136bc2c90cfdd5c0a18e445e`  
		Last Modified: Wed, 13 May 2020 21:11:45 GMT  
		Size: 283.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:684fd6b097cf009d3e00a45e92d47256b86881e70726707607ba29c24ec95f3f`  
		Last Modified: Wed, 13 May 2020 21:11:45 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.6-alpine` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:84ab0fed3c7720f4b9d131bcbdc1df458b99a5e9950ea32ae9c139e5e874c877
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.3 MB (4298272 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f21d64f8b964ecd80325828de3f81900ab258b90d021c999c8db169e9dc75790`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 24 Apr 2020 00:14:18 GMT
ADD file:85ae77bc1e43353ff14e6fe1658be1ed4ecbf4330212ac3d7ab7462add32dd39 in / 
# Fri, 24 Apr 2020 00:14:21 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 11:04:28 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Fri, 24 Apr 2020 11:04:30 GMT
RUN apk add --no-cache cyrus-sasl-plain
# Wed, 13 May 2020 21:06:36 GMT
ENV MEMCACHED_VERSION=1.6.6
# Wed, 13 May 2020 21:06:36 GMT
ENV MEMCACHED_SHA1=d8895b12dc9fc82b389f1713e2c09cc6ca3d03e4
# Wed, 13 May 2020 21:17:01 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		dpkg-dev dpkg 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		tar 		wget 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& make test 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Wed, 13 May 2020 21:17:02 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 13 May 2020 21:17:05 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 13 May 2020 21:17:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 13 May 2020 21:17:07 GMT
USER memcache
# Wed, 13 May 2020 21:17:08 GMT
EXPOSE 11211
# Wed, 13 May 2020 21:17:10 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:29e5d40040c18c692ed73df24511071725b74956ca1a61fe6056a651d86a13bd`  
		Last Modified: Fri, 24 Apr 2020 00:15:41 GMT  
		Size: 2.7 MB (2724424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fe5c53c35221a3533be681a0b6993aafc24fb08c1669f6e2cc3a14ae53ec625`  
		Last Modified: Fri, 24 Apr 2020 11:14:02 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8563552dafaf43a304948c84a7acc248f525f7112d769119ce9c6a68a5e3691`  
		Last Modified: Fri, 24 Apr 2020 11:14:02 GMT  
		Size: 15.5 KB (15487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e025d7a35db9442b2a837e76a39855504aabc39e7e3f988809d349af719667a`  
		Last Modified: Wed, 13 May 2020 21:17:37 GMT  
		Size: 1.6 MB (1556696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcaab3e6609fb2db6c7f55beb904fead407e5d2b97b6acafb93c96c03e56799e`  
		Last Modified: Wed, 13 May 2020 21:17:36 GMT  
		Size: 283.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6109ee9cf8d24da13ee3db362111fdb6fad712167f7a2df5c40282502c86c9c`  
		Last Modified: Wed, 13 May 2020 21:17:36 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.6-alpine` - linux; s390x

```console
$ docker pull memcached@sha256:e67fbfdb16b98451a2479f1b8ac1253153c1a0207446cd0b96ac3acbc8388374
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4167257 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:172a7a8f96030a5bb34744dedb5dc60f06194a5967f790a4507f2f6a123a1e52`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 23 Apr 2020 17:50:57 GMT
ADD file:a59a30c2fd43c9f3b820751a6f5a54688c14440a1ddace1ab255475f46e6ba2d in / 
# Thu, 23 Apr 2020 17:50:58 GMT
CMD ["/bin/sh"]
# Thu, 23 Apr 2020 19:00:40 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Thu, 23 Apr 2020 19:00:41 GMT
RUN apk add --no-cache cyrus-sasl-plain
# Wed, 13 May 2020 20:44:10 GMT
ENV MEMCACHED_VERSION=1.6.6
# Wed, 13 May 2020 20:44:10 GMT
ENV MEMCACHED_SHA1=d8895b12dc9fc82b389f1713e2c09cc6ca3d03e4
# Wed, 13 May 2020 20:53:11 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		dpkg-dev dpkg 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		tar 		wget 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& make test 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Wed, 13 May 2020 20:53:11 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 13 May 2020 20:53:12 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 13 May 2020 20:53:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 13 May 2020 20:53:12 GMT
USER memcache
# Wed, 13 May 2020 20:53:13 GMT
EXPOSE 11211
# Wed, 13 May 2020 20:53:13 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:7184c046fdf17da4c16ca482e5ede36e1f2d41ac8cea9c036e488fd149d6e8e7`  
		Last Modified: Thu, 23 Apr 2020 17:51:38 GMT  
		Size: 2.6 MB (2582859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca2971d466d139c0291506e9e9a74874f9720887c9d7589ac53625b827b4ddcb`  
		Last Modified: Wed, 13 May 2020 20:53:44 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dba5e1242654650bd369b46ebc84b7619dad9b2965728812cd6c53fbe412447`  
		Last Modified: Wed, 13 May 2020 20:53:50 GMT  
		Size: 15.4 KB (15364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56c7a93509f92f968102940c5f29e41a5246d13ff2ca46d1b943913e1bdb0156`  
		Last Modified: Wed, 13 May 2020 20:53:45 GMT  
		Size: 1.6 MB (1567372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f782215b5f873e287c10ac50cd1ffafe9a48a11bce170ccb5ff224692251297a`  
		Last Modified: Wed, 13 May 2020 20:53:44 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91c50080fccd2633d9e531227847ff62435c70da07804426afede4469d4c11a2`  
		Last Modified: Wed, 13 May 2020 20:53:44 GMT  
		Size: 120.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:1.6-alpine`

```console
$ docker pull memcached@sha256:844545820553dec0bfa5d90f16e723df8533863de045d7d2cae07f892a9708b5
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
$ docker pull memcached@sha256:7aff4ef05d45a680295a97643acd5c8fd1b306697df52b9b99d3c5665cc91520
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.4 MB (4383824 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:35acd9837d07e6369afd8683ae08f7da10de93ea5d50e74050abbdeece1e6754`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:03 GMT
ADD file:b91adb67b670d3a6ff9463e48b7def903ed516be66fc4282d22c53e41512be49 in / 
# Fri, 24 Apr 2020 01:05:03 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 17:02:57 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Fri, 24 Apr 2020 17:02:58 GMT
RUN apk add --no-cache cyrus-sasl-plain
# Wed, 13 May 2020 21:06:46 GMT
ENV MEMCACHED_VERSION=1.6.6
# Wed, 13 May 2020 21:06:46 GMT
ENV MEMCACHED_SHA1=d8895b12dc9fc82b389f1713e2c09cc6ca3d03e4
# Wed, 13 May 2020 21:16:24 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		dpkg-dev dpkg 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		tar 		wget 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& make test 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Wed, 13 May 2020 21:16:24 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 13 May 2020 21:16:25 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 13 May 2020 21:16:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 13 May 2020 21:16:25 GMT
USER memcache
# Wed, 13 May 2020 21:16:25 GMT
EXPOSE 11211
# Wed, 13 May 2020 21:16:25 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:cbdbe7a5bc2a134ca8ec91be58565ec07d037386d1f1d8385412d224deafca08`  
		Last Modified: Thu, 23 Apr 2020 14:07:19 GMT  
		Size: 2.8 MB (2813316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b534c8dcbed02f81e7238c6977e5e3c22aa347c9d8967b7c12c392ee7a9f548b`  
		Last Modified: Fri, 24 Apr 2020 17:11:25 GMT  
		Size: 1.2 KB (1229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f82e93b65d94a9b03ff2f6758b7ad7c93eceeecf3e1310ba5c7160af4fd59962`  
		Last Modified: Fri, 24 Apr 2020 17:11:25 GMT  
		Size: 15.1 KB (15096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea07733e4053c9b83448decf54f501b7f1fc49e3dcd8d3765c66f476df674fab`  
		Last Modified: Wed, 13 May 2020 21:16:49 GMT  
		Size: 1.6 MB (1553777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa95676f933fd0bbc2cc1615e9449e9122b4a5129fbdaff414a28df5cad88222`  
		Last Modified: Wed, 13 May 2020 21:16:49 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2198a28066da8054936ad286e306fb5694ee81c36f612760266d1ca33e9563b`  
		Last Modified: Wed, 13 May 2020 21:16:49 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-alpine` - linux; arm variant v6

```console
$ docker pull memcached@sha256:cdedb0318507c578a21a481fbac96717787aaea12acc53f151332ad36dc72a3e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4153141 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:84637e955a61c7f56159f60a65b17b892fe5ac952e43227f0d2725ae342bbd90`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 23 Apr 2020 15:51:24 GMT
ADD file:cc0770cddff6b50d5e31f39886420eb8a0b4af55664d6f7599207c9aeaf6a501 in / 
# Thu, 23 Apr 2020 15:51:25 GMT
CMD ["/bin/sh"]
# Thu, 23 Apr 2020 18:17:02 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Thu, 23 Apr 2020 18:17:05 GMT
RUN apk add --no-cache cyrus-sasl-plain
# Wed, 13 May 2020 20:48:09 GMT
ENV MEMCACHED_VERSION=1.6.6
# Wed, 13 May 2020 20:48:09 GMT
ENV MEMCACHED_SHA1=d8895b12dc9fc82b389f1713e2c09cc6ca3d03e4
# Wed, 13 May 2020 20:58:49 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		dpkg-dev dpkg 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		tar 		wget 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& make test 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Wed, 13 May 2020 20:58:50 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 13 May 2020 20:58:51 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 13 May 2020 20:58:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 13 May 2020 20:58:53 GMT
USER memcache
# Wed, 13 May 2020 20:58:53 GMT
EXPOSE 11211
# Wed, 13 May 2020 20:58:54 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:b9e3228833e92f0688e0f87234e75965e62e47cfbb9ca8cc5fa19c2e7cd13f80`  
		Last Modified: Thu, 23 Apr 2020 15:52:05 GMT  
		Size: 2.6 MB (2619936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93317744ae21705795946b5f7ccb9e69cd54b0d5b2bdbf48e38bc24ab2037dd4`  
		Last Modified: Thu, 23 Apr 2020 18:26:46 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22d5a6e65917b2d4ecdcd28e7178c79f43bd5cceabca1d40ef2708e66642b656`  
		Last Modified: Thu, 23 Apr 2020 18:26:47 GMT  
		Size: 14.7 KB (14705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55286676201b8c21a4a24628ece19d15221ee259c5df155ebcd0793841211612`  
		Last Modified: Wed, 13 May 2020 20:59:13 GMT  
		Size: 1.5 MB (1516837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c924249be839e9ffa60f403cf731eca93b38caa4e09dc57769e4cc25bcb5ca1`  
		Last Modified: Wed, 13 May 2020 20:59:13 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ded1f200c6c3b6d497cbb1a7fc81bd1ee1dd0cf53a43a8b068ce134ec3c7ab1`  
		Last Modified: Wed, 13 May 2020 20:59:12 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-alpine` - linux; arm variant v7

```console
$ docker pull memcached@sha256:b8d5715c8f0905fd1d24efc8254baa1ccf6933d9942b0b84c66750a5662bb811
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3841215 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:331fbc8dc15f015e7fdd524a348b69696983085d2badb3a9a53cb7424a30567d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 23 Apr 2020 22:04:19 GMT
ADD file:33578d3cacfab86c195d99396dd012ec511796a1d2d8d6f0a02b8a055673c294 in / 
# Thu, 23 Apr 2020 22:04:22 GMT
CMD ["/bin/sh"]
# Mon, 27 Apr 2020 20:41:10 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Mon, 27 Apr 2020 20:41:12 GMT
RUN apk add --no-cache cyrus-sasl-plain
# Wed, 13 May 2020 21:00:46 GMT
ENV MEMCACHED_VERSION=1.6.6
# Wed, 13 May 2020 21:00:47 GMT
ENV MEMCACHED_SHA1=d8895b12dc9fc82b389f1713e2c09cc6ca3d03e4
# Wed, 13 May 2020 21:11:09 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		dpkg-dev dpkg 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		tar 		wget 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& make test 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Wed, 13 May 2020 21:11:10 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 13 May 2020 21:11:12 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 13 May 2020 21:11:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 13 May 2020 21:11:13 GMT
USER memcache
# Wed, 13 May 2020 21:11:13 GMT
EXPOSE 11211
# Wed, 13 May 2020 21:11:14 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:3cfb62949d9d8613854db4d5fe502a9219c2b55a153043500078a64e880ae234`  
		Last Modified: Thu, 23 Apr 2020 22:05:12 GMT  
		Size: 2.4 MB (2422063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea5eed70290b5b33d1d0a27554b33b5998613f63667c5797fee672c96ea93df4`  
		Last Modified: Mon, 27 Apr 2020 20:50:54 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea75d9462432267b72327c7684218d1e4d40ec6d9b6578b0e8b79fdc50e2f99b`  
		Last Modified: Mon, 27 Apr 2020 20:50:54 GMT  
		Size: 13.6 KB (13633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e2c49241690acb15f16b690b318be68612c6665317e6f7f8b4cc57b57df0d59`  
		Last Modified: Wed, 13 May 2020 21:11:45 GMT  
		Size: 1.4 MB (1403856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b9dc2878fb274ac6ea5501d45e6a552af904357136bc2c90cfdd5c0a18e445e`  
		Last Modified: Wed, 13 May 2020 21:11:45 GMT  
		Size: 283.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:684fd6b097cf009d3e00a45e92d47256b86881e70726707607ba29c24ec95f3f`  
		Last Modified: Wed, 13 May 2020 21:11:45 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-alpine` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:84ab0fed3c7720f4b9d131bcbdc1df458b99a5e9950ea32ae9c139e5e874c877
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.3 MB (4298272 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f21d64f8b964ecd80325828de3f81900ab258b90d021c999c8db169e9dc75790`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 24 Apr 2020 00:14:18 GMT
ADD file:85ae77bc1e43353ff14e6fe1658be1ed4ecbf4330212ac3d7ab7462add32dd39 in / 
# Fri, 24 Apr 2020 00:14:21 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 11:04:28 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Fri, 24 Apr 2020 11:04:30 GMT
RUN apk add --no-cache cyrus-sasl-plain
# Wed, 13 May 2020 21:06:36 GMT
ENV MEMCACHED_VERSION=1.6.6
# Wed, 13 May 2020 21:06:36 GMT
ENV MEMCACHED_SHA1=d8895b12dc9fc82b389f1713e2c09cc6ca3d03e4
# Wed, 13 May 2020 21:17:01 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		dpkg-dev dpkg 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		tar 		wget 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& make test 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Wed, 13 May 2020 21:17:02 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 13 May 2020 21:17:05 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 13 May 2020 21:17:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 13 May 2020 21:17:07 GMT
USER memcache
# Wed, 13 May 2020 21:17:08 GMT
EXPOSE 11211
# Wed, 13 May 2020 21:17:10 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:29e5d40040c18c692ed73df24511071725b74956ca1a61fe6056a651d86a13bd`  
		Last Modified: Fri, 24 Apr 2020 00:15:41 GMT  
		Size: 2.7 MB (2724424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fe5c53c35221a3533be681a0b6993aafc24fb08c1669f6e2cc3a14ae53ec625`  
		Last Modified: Fri, 24 Apr 2020 11:14:02 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8563552dafaf43a304948c84a7acc248f525f7112d769119ce9c6a68a5e3691`  
		Last Modified: Fri, 24 Apr 2020 11:14:02 GMT  
		Size: 15.5 KB (15487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e025d7a35db9442b2a837e76a39855504aabc39e7e3f988809d349af719667a`  
		Last Modified: Wed, 13 May 2020 21:17:37 GMT  
		Size: 1.6 MB (1556696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcaab3e6609fb2db6c7f55beb904fead407e5d2b97b6acafb93c96c03e56799e`  
		Last Modified: Wed, 13 May 2020 21:17:36 GMT  
		Size: 283.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6109ee9cf8d24da13ee3db362111fdb6fad712167f7a2df5c40282502c86c9c`  
		Last Modified: Wed, 13 May 2020 21:17:36 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-alpine` - linux; 386

```console
$ docker pull memcached@sha256:9b0c9b3db5efc1811bdade3e907762b3b280a2c0f691e21879042891d354b9ac
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4474699 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:17e684669b8ae068d4803cd8c284ed9dd369fa7f17e389be1aa8e150279e3552`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 23 Apr 2020 21:16:04 GMT
ADD file:63bd8a316cba8c404cc2e32a5120406c24aee8db3224c469a6077b941d900863 in / 
# Thu, 23 Apr 2020 21:16:04 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 05:40:17 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Fri, 24 Apr 2020 05:40:18 GMT
RUN apk add --no-cache cyrus-sasl-plain
# Fri, 24 Apr 2020 05:40:18 GMT
ENV MEMCACHED_VERSION=1.6.5
# Fri, 24 Apr 2020 05:40:18 GMT
ENV MEMCACHED_SHA1=1ddb5f37f69946b63512ad0f89dc448ff7ba5713
# Fri, 24 Apr 2020 05:48:50 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		dpkg-dev dpkg 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		tar 		wget 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& make test 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Fri, 24 Apr 2020 05:48:50 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 24 Apr 2020 05:48:51 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 24 Apr 2020 05:48:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 05:48:51 GMT
USER memcache
# Fri, 24 Apr 2020 05:48:52 GMT
EXPOSE 11211
# Fri, 24 Apr 2020 05:48:52 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:2826c1e79865da7e0da0a993a2a38db61c3911e05b5df617439a86d4deac90fb`  
		Last Modified: Thu, 23 Apr 2020 21:16:32 GMT  
		Size: 2.8 MB (2808418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99c8f50e3ca0c1433cc286bd4e0a3745ecca7885db26d6589ed10f87bbaab945`  
		Last Modified: Fri, 24 Apr 2020 05:49:15 GMT  
		Size: 1.2 KB (1230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fc013a10731c30303c911d27a87fd13538c35f156dd04c77830fd6aae807373`  
		Last Modified: Fri, 24 Apr 2020 05:49:16 GMT  
		Size: 16.2 KB (16152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37a786658d91db927acd12a837dc612825e43975a8796487411a1c288e3c653f`  
		Last Modified: Fri, 24 Apr 2020 05:49:16 GMT  
		Size: 1.6 MB (1648494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b19c40ceca97a50d53a37fcda076bdfb9abd55944502678c779cf4ffd3cdfeee`  
		Last Modified: Fri, 24 Apr 2020 05:49:16 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22ddfad80624d91b3218e2b53a566c1ac45e3adf5acef7f1313a0a24c43bcb1b`  
		Last Modified: Fri, 24 Apr 2020 05:49:15 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-alpine` - linux; ppc64le

```console
$ docker pull memcached@sha256:90c4016f3fda33920862008a5278d874f8383633bad2e865fff01ed7d900d1c0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4450322 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2edb83f0573ab043b0d92c05a4c7aeb17036f6bd9fa98c65ed0ce3a53cfd4f1b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 23 Apr 2020 20:39:04 GMT
ADD file:1aaebe252dfb1885e066fcbc84aaa915bae149c3608f19600855ad1d4f7450c1 in / 
# Thu, 23 Apr 2020 20:39:06 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 06:58:53 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Fri, 24 Apr 2020 06:59:15 GMT
RUN apk add --no-cache cyrus-sasl-plain
# Fri, 24 Apr 2020 06:59:21 GMT
ENV MEMCACHED_VERSION=1.6.5
# Fri, 24 Apr 2020 06:59:28 GMT
ENV MEMCACHED_SHA1=1ddb5f37f69946b63512ad0f89dc448ff7ba5713
# Fri, 24 Apr 2020 07:08:21 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		dpkg-dev dpkg 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		tar 		wget 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& make test 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Fri, 24 Apr 2020 07:08:26 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 24 Apr 2020 07:08:44 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 24 Apr 2020 07:08:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 07:08:58 GMT
USER memcache
# Fri, 24 Apr 2020 07:09:04 GMT
EXPOSE 11211
# Fri, 24 Apr 2020 07:09:11 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:9a8fdc5b698322331ee7eba7dd6f66f3a4e956554db22dd1e834d519415b4f8e`  
		Last Modified: Thu, 23 Apr 2020 20:41:33 GMT  
		Size: 2.8 MB (2821843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8003ab8fdd2231d50550cbe8a4e5715a79d4707174e50e5208a3525a93b88d58`  
		Last Modified: Fri, 24 Apr 2020 07:09:36 GMT  
		Size: 1.3 KB (1264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cf79da4de605128ba727e77467d72e9e1045bdd33fef6b7e4be6beb023816b1`  
		Last Modified: Fri, 24 Apr 2020 07:09:36 GMT  
		Size: 16.1 KB (16137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b747ed97ad4df5a4b7c87e75b9df6cbd8e80cca2318b6ba49f6565e0a13abc29`  
		Last Modified: Fri, 24 Apr 2020 07:09:37 GMT  
		Size: 1.6 MB (1610672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eddfdbf0368225d39442c7fd411ae489ac0e211fc2ac682b75d3023084110aca`  
		Last Modified: Fri, 24 Apr 2020 07:09:36 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06a46a063e5e1e9324bacfb85d49c5f48b921b80e935a96ae0283bbd65c21a11`  
		Last Modified: Fri, 24 Apr 2020 07:09:37 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-alpine` - linux; s390x

```console
$ docker pull memcached@sha256:e67fbfdb16b98451a2479f1b8ac1253153c1a0207446cd0b96ac3acbc8388374
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4167257 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:172a7a8f96030a5bb34744dedb5dc60f06194a5967f790a4507f2f6a123a1e52`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 23 Apr 2020 17:50:57 GMT
ADD file:a59a30c2fd43c9f3b820751a6f5a54688c14440a1ddace1ab255475f46e6ba2d in / 
# Thu, 23 Apr 2020 17:50:58 GMT
CMD ["/bin/sh"]
# Thu, 23 Apr 2020 19:00:40 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Thu, 23 Apr 2020 19:00:41 GMT
RUN apk add --no-cache cyrus-sasl-plain
# Wed, 13 May 2020 20:44:10 GMT
ENV MEMCACHED_VERSION=1.6.6
# Wed, 13 May 2020 20:44:10 GMT
ENV MEMCACHED_SHA1=d8895b12dc9fc82b389f1713e2c09cc6ca3d03e4
# Wed, 13 May 2020 20:53:11 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		dpkg-dev dpkg 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		tar 		wget 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& make test 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Wed, 13 May 2020 20:53:11 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 13 May 2020 20:53:12 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 13 May 2020 20:53:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 13 May 2020 20:53:12 GMT
USER memcache
# Wed, 13 May 2020 20:53:13 GMT
EXPOSE 11211
# Wed, 13 May 2020 20:53:13 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:7184c046fdf17da4c16ca482e5ede36e1f2d41ac8cea9c036e488fd149d6e8e7`  
		Last Modified: Thu, 23 Apr 2020 17:51:38 GMT  
		Size: 2.6 MB (2582859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca2971d466d139c0291506e9e9a74874f9720887c9d7589ac53625b827b4ddcb`  
		Last Modified: Wed, 13 May 2020 20:53:44 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dba5e1242654650bd369b46ebc84b7619dad9b2965728812cd6c53fbe412447`  
		Last Modified: Wed, 13 May 2020 20:53:50 GMT  
		Size: 15.4 KB (15364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56c7a93509f92f968102940c5f29e41a5246d13ff2ca46d1b943913e1bdb0156`  
		Last Modified: Wed, 13 May 2020 20:53:45 GMT  
		Size: 1.6 MB (1567372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f782215b5f873e287c10ac50cd1ffafe9a48a11bce170ccb5ff224692251297a`  
		Last Modified: Wed, 13 May 2020 20:53:44 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91c50080fccd2633d9e531227847ff62435c70da07804426afede4469d4c11a2`  
		Last Modified: Wed, 13 May 2020 20:53:44 GMT  
		Size: 120.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:1-alpine`

```console
$ docker pull memcached@sha256:844545820553dec0bfa5d90f16e723df8533863de045d7d2cae07f892a9708b5
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
$ docker pull memcached@sha256:7aff4ef05d45a680295a97643acd5c8fd1b306697df52b9b99d3c5665cc91520
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.4 MB (4383824 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:35acd9837d07e6369afd8683ae08f7da10de93ea5d50e74050abbdeece1e6754`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:03 GMT
ADD file:b91adb67b670d3a6ff9463e48b7def903ed516be66fc4282d22c53e41512be49 in / 
# Fri, 24 Apr 2020 01:05:03 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 17:02:57 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Fri, 24 Apr 2020 17:02:58 GMT
RUN apk add --no-cache cyrus-sasl-plain
# Wed, 13 May 2020 21:06:46 GMT
ENV MEMCACHED_VERSION=1.6.6
# Wed, 13 May 2020 21:06:46 GMT
ENV MEMCACHED_SHA1=d8895b12dc9fc82b389f1713e2c09cc6ca3d03e4
# Wed, 13 May 2020 21:16:24 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		dpkg-dev dpkg 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		tar 		wget 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& make test 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Wed, 13 May 2020 21:16:24 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 13 May 2020 21:16:25 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 13 May 2020 21:16:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 13 May 2020 21:16:25 GMT
USER memcache
# Wed, 13 May 2020 21:16:25 GMT
EXPOSE 11211
# Wed, 13 May 2020 21:16:25 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:cbdbe7a5bc2a134ca8ec91be58565ec07d037386d1f1d8385412d224deafca08`  
		Last Modified: Thu, 23 Apr 2020 14:07:19 GMT  
		Size: 2.8 MB (2813316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b534c8dcbed02f81e7238c6977e5e3c22aa347c9d8967b7c12c392ee7a9f548b`  
		Last Modified: Fri, 24 Apr 2020 17:11:25 GMT  
		Size: 1.2 KB (1229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f82e93b65d94a9b03ff2f6758b7ad7c93eceeecf3e1310ba5c7160af4fd59962`  
		Last Modified: Fri, 24 Apr 2020 17:11:25 GMT  
		Size: 15.1 KB (15096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea07733e4053c9b83448decf54f501b7f1fc49e3dcd8d3765c66f476df674fab`  
		Last Modified: Wed, 13 May 2020 21:16:49 GMT  
		Size: 1.6 MB (1553777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa95676f933fd0bbc2cc1615e9449e9122b4a5129fbdaff414a28df5cad88222`  
		Last Modified: Wed, 13 May 2020 21:16:49 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2198a28066da8054936ad286e306fb5694ee81c36f612760266d1ca33e9563b`  
		Last Modified: Wed, 13 May 2020 21:16:49 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-alpine` - linux; arm variant v6

```console
$ docker pull memcached@sha256:cdedb0318507c578a21a481fbac96717787aaea12acc53f151332ad36dc72a3e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4153141 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:84637e955a61c7f56159f60a65b17b892fe5ac952e43227f0d2725ae342bbd90`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 23 Apr 2020 15:51:24 GMT
ADD file:cc0770cddff6b50d5e31f39886420eb8a0b4af55664d6f7599207c9aeaf6a501 in / 
# Thu, 23 Apr 2020 15:51:25 GMT
CMD ["/bin/sh"]
# Thu, 23 Apr 2020 18:17:02 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Thu, 23 Apr 2020 18:17:05 GMT
RUN apk add --no-cache cyrus-sasl-plain
# Wed, 13 May 2020 20:48:09 GMT
ENV MEMCACHED_VERSION=1.6.6
# Wed, 13 May 2020 20:48:09 GMT
ENV MEMCACHED_SHA1=d8895b12dc9fc82b389f1713e2c09cc6ca3d03e4
# Wed, 13 May 2020 20:58:49 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		dpkg-dev dpkg 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		tar 		wget 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& make test 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Wed, 13 May 2020 20:58:50 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 13 May 2020 20:58:51 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 13 May 2020 20:58:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 13 May 2020 20:58:53 GMT
USER memcache
# Wed, 13 May 2020 20:58:53 GMT
EXPOSE 11211
# Wed, 13 May 2020 20:58:54 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:b9e3228833e92f0688e0f87234e75965e62e47cfbb9ca8cc5fa19c2e7cd13f80`  
		Last Modified: Thu, 23 Apr 2020 15:52:05 GMT  
		Size: 2.6 MB (2619936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93317744ae21705795946b5f7ccb9e69cd54b0d5b2bdbf48e38bc24ab2037dd4`  
		Last Modified: Thu, 23 Apr 2020 18:26:46 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22d5a6e65917b2d4ecdcd28e7178c79f43bd5cceabca1d40ef2708e66642b656`  
		Last Modified: Thu, 23 Apr 2020 18:26:47 GMT  
		Size: 14.7 KB (14705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55286676201b8c21a4a24628ece19d15221ee259c5df155ebcd0793841211612`  
		Last Modified: Wed, 13 May 2020 20:59:13 GMT  
		Size: 1.5 MB (1516837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c924249be839e9ffa60f403cf731eca93b38caa4e09dc57769e4cc25bcb5ca1`  
		Last Modified: Wed, 13 May 2020 20:59:13 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ded1f200c6c3b6d497cbb1a7fc81bd1ee1dd0cf53a43a8b068ce134ec3c7ab1`  
		Last Modified: Wed, 13 May 2020 20:59:12 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-alpine` - linux; arm variant v7

```console
$ docker pull memcached@sha256:b8d5715c8f0905fd1d24efc8254baa1ccf6933d9942b0b84c66750a5662bb811
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3841215 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:331fbc8dc15f015e7fdd524a348b69696983085d2badb3a9a53cb7424a30567d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 23 Apr 2020 22:04:19 GMT
ADD file:33578d3cacfab86c195d99396dd012ec511796a1d2d8d6f0a02b8a055673c294 in / 
# Thu, 23 Apr 2020 22:04:22 GMT
CMD ["/bin/sh"]
# Mon, 27 Apr 2020 20:41:10 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Mon, 27 Apr 2020 20:41:12 GMT
RUN apk add --no-cache cyrus-sasl-plain
# Wed, 13 May 2020 21:00:46 GMT
ENV MEMCACHED_VERSION=1.6.6
# Wed, 13 May 2020 21:00:47 GMT
ENV MEMCACHED_SHA1=d8895b12dc9fc82b389f1713e2c09cc6ca3d03e4
# Wed, 13 May 2020 21:11:09 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		dpkg-dev dpkg 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		tar 		wget 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& make test 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Wed, 13 May 2020 21:11:10 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 13 May 2020 21:11:12 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 13 May 2020 21:11:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 13 May 2020 21:11:13 GMT
USER memcache
# Wed, 13 May 2020 21:11:13 GMT
EXPOSE 11211
# Wed, 13 May 2020 21:11:14 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:3cfb62949d9d8613854db4d5fe502a9219c2b55a153043500078a64e880ae234`  
		Last Modified: Thu, 23 Apr 2020 22:05:12 GMT  
		Size: 2.4 MB (2422063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea5eed70290b5b33d1d0a27554b33b5998613f63667c5797fee672c96ea93df4`  
		Last Modified: Mon, 27 Apr 2020 20:50:54 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea75d9462432267b72327c7684218d1e4d40ec6d9b6578b0e8b79fdc50e2f99b`  
		Last Modified: Mon, 27 Apr 2020 20:50:54 GMT  
		Size: 13.6 KB (13633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e2c49241690acb15f16b690b318be68612c6665317e6f7f8b4cc57b57df0d59`  
		Last Modified: Wed, 13 May 2020 21:11:45 GMT  
		Size: 1.4 MB (1403856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b9dc2878fb274ac6ea5501d45e6a552af904357136bc2c90cfdd5c0a18e445e`  
		Last Modified: Wed, 13 May 2020 21:11:45 GMT  
		Size: 283.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:684fd6b097cf009d3e00a45e92d47256b86881e70726707607ba29c24ec95f3f`  
		Last Modified: Wed, 13 May 2020 21:11:45 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-alpine` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:84ab0fed3c7720f4b9d131bcbdc1df458b99a5e9950ea32ae9c139e5e874c877
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.3 MB (4298272 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f21d64f8b964ecd80325828de3f81900ab258b90d021c999c8db169e9dc75790`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 24 Apr 2020 00:14:18 GMT
ADD file:85ae77bc1e43353ff14e6fe1658be1ed4ecbf4330212ac3d7ab7462add32dd39 in / 
# Fri, 24 Apr 2020 00:14:21 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 11:04:28 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Fri, 24 Apr 2020 11:04:30 GMT
RUN apk add --no-cache cyrus-sasl-plain
# Wed, 13 May 2020 21:06:36 GMT
ENV MEMCACHED_VERSION=1.6.6
# Wed, 13 May 2020 21:06:36 GMT
ENV MEMCACHED_SHA1=d8895b12dc9fc82b389f1713e2c09cc6ca3d03e4
# Wed, 13 May 2020 21:17:01 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		dpkg-dev dpkg 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		tar 		wget 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& make test 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Wed, 13 May 2020 21:17:02 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 13 May 2020 21:17:05 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 13 May 2020 21:17:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 13 May 2020 21:17:07 GMT
USER memcache
# Wed, 13 May 2020 21:17:08 GMT
EXPOSE 11211
# Wed, 13 May 2020 21:17:10 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:29e5d40040c18c692ed73df24511071725b74956ca1a61fe6056a651d86a13bd`  
		Last Modified: Fri, 24 Apr 2020 00:15:41 GMT  
		Size: 2.7 MB (2724424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fe5c53c35221a3533be681a0b6993aafc24fb08c1669f6e2cc3a14ae53ec625`  
		Last Modified: Fri, 24 Apr 2020 11:14:02 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8563552dafaf43a304948c84a7acc248f525f7112d769119ce9c6a68a5e3691`  
		Last Modified: Fri, 24 Apr 2020 11:14:02 GMT  
		Size: 15.5 KB (15487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e025d7a35db9442b2a837e76a39855504aabc39e7e3f988809d349af719667a`  
		Last Modified: Wed, 13 May 2020 21:17:37 GMT  
		Size: 1.6 MB (1556696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcaab3e6609fb2db6c7f55beb904fead407e5d2b97b6acafb93c96c03e56799e`  
		Last Modified: Wed, 13 May 2020 21:17:36 GMT  
		Size: 283.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6109ee9cf8d24da13ee3db362111fdb6fad712167f7a2df5c40282502c86c9c`  
		Last Modified: Wed, 13 May 2020 21:17:36 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-alpine` - linux; 386

```console
$ docker pull memcached@sha256:9b0c9b3db5efc1811bdade3e907762b3b280a2c0f691e21879042891d354b9ac
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4474699 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:17e684669b8ae068d4803cd8c284ed9dd369fa7f17e389be1aa8e150279e3552`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 23 Apr 2020 21:16:04 GMT
ADD file:63bd8a316cba8c404cc2e32a5120406c24aee8db3224c469a6077b941d900863 in / 
# Thu, 23 Apr 2020 21:16:04 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 05:40:17 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Fri, 24 Apr 2020 05:40:18 GMT
RUN apk add --no-cache cyrus-sasl-plain
# Fri, 24 Apr 2020 05:40:18 GMT
ENV MEMCACHED_VERSION=1.6.5
# Fri, 24 Apr 2020 05:40:18 GMT
ENV MEMCACHED_SHA1=1ddb5f37f69946b63512ad0f89dc448ff7ba5713
# Fri, 24 Apr 2020 05:48:50 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		dpkg-dev dpkg 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		tar 		wget 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& make test 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Fri, 24 Apr 2020 05:48:50 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 24 Apr 2020 05:48:51 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 24 Apr 2020 05:48:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 05:48:51 GMT
USER memcache
# Fri, 24 Apr 2020 05:48:52 GMT
EXPOSE 11211
# Fri, 24 Apr 2020 05:48:52 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:2826c1e79865da7e0da0a993a2a38db61c3911e05b5df617439a86d4deac90fb`  
		Last Modified: Thu, 23 Apr 2020 21:16:32 GMT  
		Size: 2.8 MB (2808418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99c8f50e3ca0c1433cc286bd4e0a3745ecca7885db26d6589ed10f87bbaab945`  
		Last Modified: Fri, 24 Apr 2020 05:49:15 GMT  
		Size: 1.2 KB (1230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fc013a10731c30303c911d27a87fd13538c35f156dd04c77830fd6aae807373`  
		Last Modified: Fri, 24 Apr 2020 05:49:16 GMT  
		Size: 16.2 KB (16152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37a786658d91db927acd12a837dc612825e43975a8796487411a1c288e3c653f`  
		Last Modified: Fri, 24 Apr 2020 05:49:16 GMT  
		Size: 1.6 MB (1648494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b19c40ceca97a50d53a37fcda076bdfb9abd55944502678c779cf4ffd3cdfeee`  
		Last Modified: Fri, 24 Apr 2020 05:49:16 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22ddfad80624d91b3218e2b53a566c1ac45e3adf5acef7f1313a0a24c43bcb1b`  
		Last Modified: Fri, 24 Apr 2020 05:49:15 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-alpine` - linux; ppc64le

```console
$ docker pull memcached@sha256:90c4016f3fda33920862008a5278d874f8383633bad2e865fff01ed7d900d1c0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4450322 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2edb83f0573ab043b0d92c05a4c7aeb17036f6bd9fa98c65ed0ce3a53cfd4f1b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 23 Apr 2020 20:39:04 GMT
ADD file:1aaebe252dfb1885e066fcbc84aaa915bae149c3608f19600855ad1d4f7450c1 in / 
# Thu, 23 Apr 2020 20:39:06 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 06:58:53 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Fri, 24 Apr 2020 06:59:15 GMT
RUN apk add --no-cache cyrus-sasl-plain
# Fri, 24 Apr 2020 06:59:21 GMT
ENV MEMCACHED_VERSION=1.6.5
# Fri, 24 Apr 2020 06:59:28 GMT
ENV MEMCACHED_SHA1=1ddb5f37f69946b63512ad0f89dc448ff7ba5713
# Fri, 24 Apr 2020 07:08:21 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		dpkg-dev dpkg 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		tar 		wget 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& make test 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Fri, 24 Apr 2020 07:08:26 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 24 Apr 2020 07:08:44 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 24 Apr 2020 07:08:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 07:08:58 GMT
USER memcache
# Fri, 24 Apr 2020 07:09:04 GMT
EXPOSE 11211
# Fri, 24 Apr 2020 07:09:11 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:9a8fdc5b698322331ee7eba7dd6f66f3a4e956554db22dd1e834d519415b4f8e`  
		Last Modified: Thu, 23 Apr 2020 20:41:33 GMT  
		Size: 2.8 MB (2821843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8003ab8fdd2231d50550cbe8a4e5715a79d4707174e50e5208a3525a93b88d58`  
		Last Modified: Fri, 24 Apr 2020 07:09:36 GMT  
		Size: 1.3 KB (1264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cf79da4de605128ba727e77467d72e9e1045bdd33fef6b7e4be6beb023816b1`  
		Last Modified: Fri, 24 Apr 2020 07:09:36 GMT  
		Size: 16.1 KB (16137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b747ed97ad4df5a4b7c87e75b9df6cbd8e80cca2318b6ba49f6565e0a13abc29`  
		Last Modified: Fri, 24 Apr 2020 07:09:37 GMT  
		Size: 1.6 MB (1610672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eddfdbf0368225d39442c7fd411ae489ac0e211fc2ac682b75d3023084110aca`  
		Last Modified: Fri, 24 Apr 2020 07:09:36 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06a46a063e5e1e9324bacfb85d49c5f48b921b80e935a96ae0283bbd65c21a11`  
		Last Modified: Fri, 24 Apr 2020 07:09:37 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-alpine` - linux; s390x

```console
$ docker pull memcached@sha256:e67fbfdb16b98451a2479f1b8ac1253153c1a0207446cd0b96ac3acbc8388374
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4167257 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:172a7a8f96030a5bb34744dedb5dc60f06194a5967f790a4507f2f6a123a1e52`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 23 Apr 2020 17:50:57 GMT
ADD file:a59a30c2fd43c9f3b820751a6f5a54688c14440a1ddace1ab255475f46e6ba2d in / 
# Thu, 23 Apr 2020 17:50:58 GMT
CMD ["/bin/sh"]
# Thu, 23 Apr 2020 19:00:40 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Thu, 23 Apr 2020 19:00:41 GMT
RUN apk add --no-cache cyrus-sasl-plain
# Wed, 13 May 2020 20:44:10 GMT
ENV MEMCACHED_VERSION=1.6.6
# Wed, 13 May 2020 20:44:10 GMT
ENV MEMCACHED_SHA1=d8895b12dc9fc82b389f1713e2c09cc6ca3d03e4
# Wed, 13 May 2020 20:53:11 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		dpkg-dev dpkg 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		tar 		wget 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& make test 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Wed, 13 May 2020 20:53:11 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 13 May 2020 20:53:12 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 13 May 2020 20:53:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 13 May 2020 20:53:12 GMT
USER memcache
# Wed, 13 May 2020 20:53:13 GMT
EXPOSE 11211
# Wed, 13 May 2020 20:53:13 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:7184c046fdf17da4c16ca482e5ede36e1f2d41ac8cea9c036e488fd149d6e8e7`  
		Last Modified: Thu, 23 Apr 2020 17:51:38 GMT  
		Size: 2.6 MB (2582859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca2971d466d139c0291506e9e9a74874f9720887c9d7589ac53625b827b4ddcb`  
		Last Modified: Wed, 13 May 2020 20:53:44 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dba5e1242654650bd369b46ebc84b7619dad9b2965728812cd6c53fbe412447`  
		Last Modified: Wed, 13 May 2020 20:53:50 GMT  
		Size: 15.4 KB (15364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56c7a93509f92f968102940c5f29e41a5246d13ff2ca46d1b943913e1bdb0156`  
		Last Modified: Wed, 13 May 2020 20:53:45 GMT  
		Size: 1.6 MB (1567372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f782215b5f873e287c10ac50cd1ffafe9a48a11bce170ccb5ff224692251297a`  
		Last Modified: Wed, 13 May 2020 20:53:44 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91c50080fccd2633d9e531227847ff62435c70da07804426afede4469d4c11a2`  
		Last Modified: Wed, 13 May 2020 20:53:44 GMT  
		Size: 120.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:alpine`

```console
$ docker pull memcached@sha256:844545820553dec0bfa5d90f16e723df8533863de045d7d2cae07f892a9708b5
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
$ docker pull memcached@sha256:7aff4ef05d45a680295a97643acd5c8fd1b306697df52b9b99d3c5665cc91520
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.4 MB (4383824 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:35acd9837d07e6369afd8683ae08f7da10de93ea5d50e74050abbdeece1e6754`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:03 GMT
ADD file:b91adb67b670d3a6ff9463e48b7def903ed516be66fc4282d22c53e41512be49 in / 
# Fri, 24 Apr 2020 01:05:03 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 17:02:57 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Fri, 24 Apr 2020 17:02:58 GMT
RUN apk add --no-cache cyrus-sasl-plain
# Wed, 13 May 2020 21:06:46 GMT
ENV MEMCACHED_VERSION=1.6.6
# Wed, 13 May 2020 21:06:46 GMT
ENV MEMCACHED_SHA1=d8895b12dc9fc82b389f1713e2c09cc6ca3d03e4
# Wed, 13 May 2020 21:16:24 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		dpkg-dev dpkg 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		tar 		wget 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& make test 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Wed, 13 May 2020 21:16:24 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 13 May 2020 21:16:25 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 13 May 2020 21:16:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 13 May 2020 21:16:25 GMT
USER memcache
# Wed, 13 May 2020 21:16:25 GMT
EXPOSE 11211
# Wed, 13 May 2020 21:16:25 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:cbdbe7a5bc2a134ca8ec91be58565ec07d037386d1f1d8385412d224deafca08`  
		Last Modified: Thu, 23 Apr 2020 14:07:19 GMT  
		Size: 2.8 MB (2813316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b534c8dcbed02f81e7238c6977e5e3c22aa347c9d8967b7c12c392ee7a9f548b`  
		Last Modified: Fri, 24 Apr 2020 17:11:25 GMT  
		Size: 1.2 KB (1229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f82e93b65d94a9b03ff2f6758b7ad7c93eceeecf3e1310ba5c7160af4fd59962`  
		Last Modified: Fri, 24 Apr 2020 17:11:25 GMT  
		Size: 15.1 KB (15096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea07733e4053c9b83448decf54f501b7f1fc49e3dcd8d3765c66f476df674fab`  
		Last Modified: Wed, 13 May 2020 21:16:49 GMT  
		Size: 1.6 MB (1553777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa95676f933fd0bbc2cc1615e9449e9122b4a5129fbdaff414a28df5cad88222`  
		Last Modified: Wed, 13 May 2020 21:16:49 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2198a28066da8054936ad286e306fb5694ee81c36f612760266d1ca33e9563b`  
		Last Modified: Wed, 13 May 2020 21:16:49 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:alpine` - linux; arm variant v6

```console
$ docker pull memcached@sha256:cdedb0318507c578a21a481fbac96717787aaea12acc53f151332ad36dc72a3e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4153141 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:84637e955a61c7f56159f60a65b17b892fe5ac952e43227f0d2725ae342bbd90`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 23 Apr 2020 15:51:24 GMT
ADD file:cc0770cddff6b50d5e31f39886420eb8a0b4af55664d6f7599207c9aeaf6a501 in / 
# Thu, 23 Apr 2020 15:51:25 GMT
CMD ["/bin/sh"]
# Thu, 23 Apr 2020 18:17:02 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Thu, 23 Apr 2020 18:17:05 GMT
RUN apk add --no-cache cyrus-sasl-plain
# Wed, 13 May 2020 20:48:09 GMT
ENV MEMCACHED_VERSION=1.6.6
# Wed, 13 May 2020 20:48:09 GMT
ENV MEMCACHED_SHA1=d8895b12dc9fc82b389f1713e2c09cc6ca3d03e4
# Wed, 13 May 2020 20:58:49 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		dpkg-dev dpkg 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		tar 		wget 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& make test 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Wed, 13 May 2020 20:58:50 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 13 May 2020 20:58:51 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 13 May 2020 20:58:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 13 May 2020 20:58:53 GMT
USER memcache
# Wed, 13 May 2020 20:58:53 GMT
EXPOSE 11211
# Wed, 13 May 2020 20:58:54 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:b9e3228833e92f0688e0f87234e75965e62e47cfbb9ca8cc5fa19c2e7cd13f80`  
		Last Modified: Thu, 23 Apr 2020 15:52:05 GMT  
		Size: 2.6 MB (2619936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93317744ae21705795946b5f7ccb9e69cd54b0d5b2bdbf48e38bc24ab2037dd4`  
		Last Modified: Thu, 23 Apr 2020 18:26:46 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22d5a6e65917b2d4ecdcd28e7178c79f43bd5cceabca1d40ef2708e66642b656`  
		Last Modified: Thu, 23 Apr 2020 18:26:47 GMT  
		Size: 14.7 KB (14705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55286676201b8c21a4a24628ece19d15221ee259c5df155ebcd0793841211612`  
		Last Modified: Wed, 13 May 2020 20:59:13 GMT  
		Size: 1.5 MB (1516837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c924249be839e9ffa60f403cf731eca93b38caa4e09dc57769e4cc25bcb5ca1`  
		Last Modified: Wed, 13 May 2020 20:59:13 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ded1f200c6c3b6d497cbb1a7fc81bd1ee1dd0cf53a43a8b068ce134ec3c7ab1`  
		Last Modified: Wed, 13 May 2020 20:59:12 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:alpine` - linux; arm variant v7

```console
$ docker pull memcached@sha256:b8d5715c8f0905fd1d24efc8254baa1ccf6933d9942b0b84c66750a5662bb811
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3841215 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:331fbc8dc15f015e7fdd524a348b69696983085d2badb3a9a53cb7424a30567d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 23 Apr 2020 22:04:19 GMT
ADD file:33578d3cacfab86c195d99396dd012ec511796a1d2d8d6f0a02b8a055673c294 in / 
# Thu, 23 Apr 2020 22:04:22 GMT
CMD ["/bin/sh"]
# Mon, 27 Apr 2020 20:41:10 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Mon, 27 Apr 2020 20:41:12 GMT
RUN apk add --no-cache cyrus-sasl-plain
# Wed, 13 May 2020 21:00:46 GMT
ENV MEMCACHED_VERSION=1.6.6
# Wed, 13 May 2020 21:00:47 GMT
ENV MEMCACHED_SHA1=d8895b12dc9fc82b389f1713e2c09cc6ca3d03e4
# Wed, 13 May 2020 21:11:09 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		dpkg-dev dpkg 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		tar 		wget 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& make test 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Wed, 13 May 2020 21:11:10 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 13 May 2020 21:11:12 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 13 May 2020 21:11:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 13 May 2020 21:11:13 GMT
USER memcache
# Wed, 13 May 2020 21:11:13 GMT
EXPOSE 11211
# Wed, 13 May 2020 21:11:14 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:3cfb62949d9d8613854db4d5fe502a9219c2b55a153043500078a64e880ae234`  
		Last Modified: Thu, 23 Apr 2020 22:05:12 GMT  
		Size: 2.4 MB (2422063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea5eed70290b5b33d1d0a27554b33b5998613f63667c5797fee672c96ea93df4`  
		Last Modified: Mon, 27 Apr 2020 20:50:54 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea75d9462432267b72327c7684218d1e4d40ec6d9b6578b0e8b79fdc50e2f99b`  
		Last Modified: Mon, 27 Apr 2020 20:50:54 GMT  
		Size: 13.6 KB (13633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e2c49241690acb15f16b690b318be68612c6665317e6f7f8b4cc57b57df0d59`  
		Last Modified: Wed, 13 May 2020 21:11:45 GMT  
		Size: 1.4 MB (1403856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b9dc2878fb274ac6ea5501d45e6a552af904357136bc2c90cfdd5c0a18e445e`  
		Last Modified: Wed, 13 May 2020 21:11:45 GMT  
		Size: 283.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:684fd6b097cf009d3e00a45e92d47256b86881e70726707607ba29c24ec95f3f`  
		Last Modified: Wed, 13 May 2020 21:11:45 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:alpine` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:84ab0fed3c7720f4b9d131bcbdc1df458b99a5e9950ea32ae9c139e5e874c877
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.3 MB (4298272 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f21d64f8b964ecd80325828de3f81900ab258b90d021c999c8db169e9dc75790`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 24 Apr 2020 00:14:18 GMT
ADD file:85ae77bc1e43353ff14e6fe1658be1ed4ecbf4330212ac3d7ab7462add32dd39 in / 
# Fri, 24 Apr 2020 00:14:21 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 11:04:28 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Fri, 24 Apr 2020 11:04:30 GMT
RUN apk add --no-cache cyrus-sasl-plain
# Wed, 13 May 2020 21:06:36 GMT
ENV MEMCACHED_VERSION=1.6.6
# Wed, 13 May 2020 21:06:36 GMT
ENV MEMCACHED_SHA1=d8895b12dc9fc82b389f1713e2c09cc6ca3d03e4
# Wed, 13 May 2020 21:17:01 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		dpkg-dev dpkg 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		tar 		wget 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& make test 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Wed, 13 May 2020 21:17:02 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 13 May 2020 21:17:05 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 13 May 2020 21:17:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 13 May 2020 21:17:07 GMT
USER memcache
# Wed, 13 May 2020 21:17:08 GMT
EXPOSE 11211
# Wed, 13 May 2020 21:17:10 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:29e5d40040c18c692ed73df24511071725b74956ca1a61fe6056a651d86a13bd`  
		Last Modified: Fri, 24 Apr 2020 00:15:41 GMT  
		Size: 2.7 MB (2724424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fe5c53c35221a3533be681a0b6993aafc24fb08c1669f6e2cc3a14ae53ec625`  
		Last Modified: Fri, 24 Apr 2020 11:14:02 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8563552dafaf43a304948c84a7acc248f525f7112d769119ce9c6a68a5e3691`  
		Last Modified: Fri, 24 Apr 2020 11:14:02 GMT  
		Size: 15.5 KB (15487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e025d7a35db9442b2a837e76a39855504aabc39e7e3f988809d349af719667a`  
		Last Modified: Wed, 13 May 2020 21:17:37 GMT  
		Size: 1.6 MB (1556696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcaab3e6609fb2db6c7f55beb904fead407e5d2b97b6acafb93c96c03e56799e`  
		Last Modified: Wed, 13 May 2020 21:17:36 GMT  
		Size: 283.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6109ee9cf8d24da13ee3db362111fdb6fad712167f7a2df5c40282502c86c9c`  
		Last Modified: Wed, 13 May 2020 21:17:36 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:alpine` - linux; 386

```console
$ docker pull memcached@sha256:9b0c9b3db5efc1811bdade3e907762b3b280a2c0f691e21879042891d354b9ac
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4474699 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:17e684669b8ae068d4803cd8c284ed9dd369fa7f17e389be1aa8e150279e3552`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 23 Apr 2020 21:16:04 GMT
ADD file:63bd8a316cba8c404cc2e32a5120406c24aee8db3224c469a6077b941d900863 in / 
# Thu, 23 Apr 2020 21:16:04 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 05:40:17 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Fri, 24 Apr 2020 05:40:18 GMT
RUN apk add --no-cache cyrus-sasl-plain
# Fri, 24 Apr 2020 05:40:18 GMT
ENV MEMCACHED_VERSION=1.6.5
# Fri, 24 Apr 2020 05:40:18 GMT
ENV MEMCACHED_SHA1=1ddb5f37f69946b63512ad0f89dc448ff7ba5713
# Fri, 24 Apr 2020 05:48:50 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		dpkg-dev dpkg 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		tar 		wget 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& make test 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Fri, 24 Apr 2020 05:48:50 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 24 Apr 2020 05:48:51 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 24 Apr 2020 05:48:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 05:48:51 GMT
USER memcache
# Fri, 24 Apr 2020 05:48:52 GMT
EXPOSE 11211
# Fri, 24 Apr 2020 05:48:52 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:2826c1e79865da7e0da0a993a2a38db61c3911e05b5df617439a86d4deac90fb`  
		Last Modified: Thu, 23 Apr 2020 21:16:32 GMT  
		Size: 2.8 MB (2808418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99c8f50e3ca0c1433cc286bd4e0a3745ecca7885db26d6589ed10f87bbaab945`  
		Last Modified: Fri, 24 Apr 2020 05:49:15 GMT  
		Size: 1.2 KB (1230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fc013a10731c30303c911d27a87fd13538c35f156dd04c77830fd6aae807373`  
		Last Modified: Fri, 24 Apr 2020 05:49:16 GMT  
		Size: 16.2 KB (16152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37a786658d91db927acd12a837dc612825e43975a8796487411a1c288e3c653f`  
		Last Modified: Fri, 24 Apr 2020 05:49:16 GMT  
		Size: 1.6 MB (1648494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b19c40ceca97a50d53a37fcda076bdfb9abd55944502678c779cf4ffd3cdfeee`  
		Last Modified: Fri, 24 Apr 2020 05:49:16 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22ddfad80624d91b3218e2b53a566c1ac45e3adf5acef7f1313a0a24c43bcb1b`  
		Last Modified: Fri, 24 Apr 2020 05:49:15 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:alpine` - linux; ppc64le

```console
$ docker pull memcached@sha256:90c4016f3fda33920862008a5278d874f8383633bad2e865fff01ed7d900d1c0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4450322 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2edb83f0573ab043b0d92c05a4c7aeb17036f6bd9fa98c65ed0ce3a53cfd4f1b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 23 Apr 2020 20:39:04 GMT
ADD file:1aaebe252dfb1885e066fcbc84aaa915bae149c3608f19600855ad1d4f7450c1 in / 
# Thu, 23 Apr 2020 20:39:06 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 06:58:53 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Fri, 24 Apr 2020 06:59:15 GMT
RUN apk add --no-cache cyrus-sasl-plain
# Fri, 24 Apr 2020 06:59:21 GMT
ENV MEMCACHED_VERSION=1.6.5
# Fri, 24 Apr 2020 06:59:28 GMT
ENV MEMCACHED_SHA1=1ddb5f37f69946b63512ad0f89dc448ff7ba5713
# Fri, 24 Apr 2020 07:08:21 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		dpkg-dev dpkg 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		tar 		wget 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& make test 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Fri, 24 Apr 2020 07:08:26 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 24 Apr 2020 07:08:44 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 24 Apr 2020 07:08:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 07:08:58 GMT
USER memcache
# Fri, 24 Apr 2020 07:09:04 GMT
EXPOSE 11211
# Fri, 24 Apr 2020 07:09:11 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:9a8fdc5b698322331ee7eba7dd6f66f3a4e956554db22dd1e834d519415b4f8e`  
		Last Modified: Thu, 23 Apr 2020 20:41:33 GMT  
		Size: 2.8 MB (2821843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8003ab8fdd2231d50550cbe8a4e5715a79d4707174e50e5208a3525a93b88d58`  
		Last Modified: Fri, 24 Apr 2020 07:09:36 GMT  
		Size: 1.3 KB (1264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cf79da4de605128ba727e77467d72e9e1045bdd33fef6b7e4be6beb023816b1`  
		Last Modified: Fri, 24 Apr 2020 07:09:36 GMT  
		Size: 16.1 KB (16137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b747ed97ad4df5a4b7c87e75b9df6cbd8e80cca2318b6ba49f6565e0a13abc29`  
		Last Modified: Fri, 24 Apr 2020 07:09:37 GMT  
		Size: 1.6 MB (1610672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eddfdbf0368225d39442c7fd411ae489ac0e211fc2ac682b75d3023084110aca`  
		Last Modified: Fri, 24 Apr 2020 07:09:36 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06a46a063e5e1e9324bacfb85d49c5f48b921b80e935a96ae0283bbd65c21a11`  
		Last Modified: Fri, 24 Apr 2020 07:09:37 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:alpine` - linux; s390x

```console
$ docker pull memcached@sha256:e67fbfdb16b98451a2479f1b8ac1253153c1a0207446cd0b96ac3acbc8388374
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4167257 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:172a7a8f96030a5bb34744dedb5dc60f06194a5967f790a4507f2f6a123a1e52`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 23 Apr 2020 17:50:57 GMT
ADD file:a59a30c2fd43c9f3b820751a6f5a54688c14440a1ddace1ab255475f46e6ba2d in / 
# Thu, 23 Apr 2020 17:50:58 GMT
CMD ["/bin/sh"]
# Thu, 23 Apr 2020 19:00:40 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Thu, 23 Apr 2020 19:00:41 GMT
RUN apk add --no-cache cyrus-sasl-plain
# Wed, 13 May 2020 20:44:10 GMT
ENV MEMCACHED_VERSION=1.6.6
# Wed, 13 May 2020 20:44:10 GMT
ENV MEMCACHED_SHA1=d8895b12dc9fc82b389f1713e2c09cc6ca3d03e4
# Wed, 13 May 2020 20:53:11 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		dpkg-dev dpkg 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		tar 		wget 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& make test 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Wed, 13 May 2020 20:53:11 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 13 May 2020 20:53:12 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 13 May 2020 20:53:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 13 May 2020 20:53:12 GMT
USER memcache
# Wed, 13 May 2020 20:53:13 GMT
EXPOSE 11211
# Wed, 13 May 2020 20:53:13 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:7184c046fdf17da4c16ca482e5ede36e1f2d41ac8cea9c036e488fd149d6e8e7`  
		Last Modified: Thu, 23 Apr 2020 17:51:38 GMT  
		Size: 2.6 MB (2582859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca2971d466d139c0291506e9e9a74874f9720887c9d7589ac53625b827b4ddcb`  
		Last Modified: Wed, 13 May 2020 20:53:44 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dba5e1242654650bd369b46ebc84b7619dad9b2965728812cd6c53fbe412447`  
		Last Modified: Wed, 13 May 2020 20:53:50 GMT  
		Size: 15.4 KB (15364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56c7a93509f92f968102940c5f29e41a5246d13ff2ca46d1b943913e1bdb0156`  
		Last Modified: Wed, 13 May 2020 20:53:45 GMT  
		Size: 1.6 MB (1567372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f782215b5f873e287c10ac50cd1ffafe9a48a11bce170ccb5ff224692251297a`  
		Last Modified: Wed, 13 May 2020 20:53:44 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91c50080fccd2633d9e531227847ff62435c70da07804426afede4469d4c11a2`  
		Last Modified: Wed, 13 May 2020 20:53:44 GMT  
		Size: 120.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:latest`

```console
$ docker pull memcached@sha256:b0f382f16271ffe9dce89bc4d47b8627ae4b491286bec220dadaee3862cdc1e2
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
$ docker pull memcached@sha256:e8c935cf0dfa9eecf9129d9039cfbe12f55c1cecc86902998d4c7c369f5b5a57
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.5 MB (30493690 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9bb369dc76dc6e22e495a01681b1d1c428701d8a06f7304ef333b36f13469e8a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 23 Apr 2020 00:20:32 GMT
ADD file:9b8be2b52ee0fa31da1b6256099030b73546253a57e94cccb24605cd888bb74d in / 
# Thu, 23 Apr 2020 00:20:32 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 03:48:31 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Thu, 23 Apr 2020 03:48:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 13 May 2020 20:57:07 GMT
ENV MEMCACHED_VERSION=1.6.6
# Wed, 13 May 2020 20:57:07 GMT
ENV MEMCACHED_SHA1=d8895b12dc9fc82b389f1713e2c09cc6ca3d03e4
# Wed, 13 May 2020 21:06:31 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 13 May 2020 21:06:31 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 13 May 2020 21:06:32 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 13 May 2020 21:06:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 13 May 2020 21:06:32 GMT
USER memcache
# Wed, 13 May 2020 21:06:32 GMT
EXPOSE 11211
# Wed, 13 May 2020 21:06:32 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:54fec2fa59d0a0de9cd2dec9850b36c43de451f1fd1c0a5bf8f1cf26a61a5da4`  
		Last Modified: Thu, 23 Apr 2020 00:25:10 GMT  
		Size: 27.1 MB (27098254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73a546564c749aeaf996f91019e9cf37b5e395b661aec0dcf2e2c20c11bbda96`  
		Last Modified: Thu, 23 Apr 2020 03:58:00 GMT  
		Size: 5.0 KB (4979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2b17108b143c42eeda6a8587b36cfd6e30c7783fb09e565feb06d09f4172525`  
		Last Modified: Thu, 23 Apr 2020 03:58:01 GMT  
		Size: 2.2 MB (2196403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a1e9dd08a002476ba6cade3017e17f464968c8e94877292d07c5b899a9e8d3a`  
		Last Modified: Wed, 13 May 2020 21:16:44 GMT  
		Size: 1.2 MB (1193645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09cafd6239484b297ad595f395a878b6ce07eefcca9de92a17910aa735abe6d5`  
		Last Modified: Wed, 13 May 2020 21:16:44 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48b6890ea4c000ff4ec7834a60a4422aaa4e75ac040f107523b1a2c653b6a4b4`  
		Last Modified: Wed, 13 May 2020 21:16:43 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:latest` - linux; arm variant v5

```console
$ docker pull memcached@sha256:d430d81aec7724f5662cd0dad2554d354921139f129ec60d96fcd97d835a68e5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.9 MB (27901495 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d38f156a5705d867b8698bf28f60397b2ccaa27ebd90a3a370e641ea8836fea3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 23 Apr 2020 00:52:22 GMT
ADD file:62a9732be4e3237ccc896f724a34606e01f351c4877e52c9a9cd85029c06b956 in / 
# Thu, 23 Apr 2020 00:52:23 GMT
CMD ["bash"]
# Mon, 27 Apr 2020 20:31:39 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Mon, 27 Apr 2020 20:31:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 13 May 2020 20:49:55 GMT
ENV MEMCACHED_VERSION=1.6.6
# Wed, 13 May 2020 20:49:56 GMT
ENV MEMCACHED_SHA1=d8895b12dc9fc82b389f1713e2c09cc6ca3d03e4
# Wed, 13 May 2020 21:01:00 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 13 May 2020 21:01:01 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 13 May 2020 21:01:03 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 13 May 2020 21:01:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 13 May 2020 21:01:05 GMT
USER memcache
# Wed, 13 May 2020 21:01:06 GMT
EXPOSE 11211
# Wed, 13 May 2020 21:01:07 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:a8c46e5952878f9f324df86c5a2b45b2e0020f6721e820981e74461d77a100dd`  
		Last Modified: Thu, 23 Apr 2020 00:59:50 GMT  
		Size: 24.8 MB (24836319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0e09e82475aef1e3124cd928ab36f48dd86a0421490ff8d8eab1ae848dbf6e6`  
		Last Modified: Mon, 27 Apr 2020 20:41:52 GMT  
		Size: 4.9 KB (4901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ed2c941c8d2e3eb09c1ec4cf66006155ff9774d385e99a0fe1de44269bfcb8a`  
		Last Modified: Mon, 27 Apr 2020 20:41:53 GMT  
		Size: 1.9 MB (1896804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:114ca507809768dd949fd745f46978c84751747b86a1b70e2d2e8681f85bb5c7`  
		Last Modified: Wed, 13 May 2020 21:01:32 GMT  
		Size: 1.2 MB (1163062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8325227257270f7e70028b55a4b9824a561441cc464ec94298af0caeb3ae7c7`  
		Last Modified: Wed, 13 May 2020 21:01:32 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65eb2dfc473e854cbe271a2fa75b0ee74363953ba9d80a4dfefc1954d1430c0f`  
		Last Modified: Wed, 13 May 2020 21:01:31 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:latest` - linux; arm variant v7

```console
$ docker pull memcached@sha256:8c0e9908733d5c2401b24e506567ca9ad0b6756c2c92d04b46e2d58eeff0b944
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.7 MB (25656893 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c9b4186eea9043000afc5ff47c169dae434c62ad0d68ef804b36ec022967aeec`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 23 Apr 2020 01:03:26 GMT
ADD file:db6122b36f3e70c5f490b50afba99d49fa345f11d0f5c77bb3c6749f8e2a4f81 in / 
# Thu, 23 Apr 2020 01:03:28 GMT
CMD ["bash"]
# Mon, 27 Apr 2020 20:31:45 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Mon, 27 Apr 2020 20:31:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 13 May 2020 20:49:59 GMT
ENV MEMCACHED_VERSION=1.6.6
# Wed, 13 May 2020 20:49:59 GMT
ENV MEMCACHED_SHA1=d8895b12dc9fc82b389f1713e2c09cc6ca3d03e4
# Wed, 13 May 2020 21:00:32 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 13 May 2020 21:00:33 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 13 May 2020 21:00:35 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 13 May 2020 21:00:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 13 May 2020 21:00:36 GMT
USER memcache
# Wed, 13 May 2020 21:00:37 GMT
EXPOSE 11211
# Wed, 13 May 2020 21:00:38 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:50fb0052086928803f00724ca465c89c45dde5b082b1e59dadb8101286dd5ab6`  
		Last Modified: Thu, 23 Apr 2020 01:11:08 GMT  
		Size: 22.7 MB (22705377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ae844ffae38c0aae3794728fe7c89bff09b70d2226e7b0775beab756cc93856`  
		Last Modified: Mon, 27 Apr 2020 20:50:45 GMT  
		Size: 4.9 KB (4898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6003a4985eba124dc101599be1daf743ce2f44e09d30ea54bf909540aa150a8`  
		Last Modified: Mon, 27 Apr 2020 20:50:45 GMT  
		Size: 1.8 MB (1811519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23bc49c42147e3c6c4bae63d2570761c08ef7aaefc2c07b43258c53f9e8865c9`  
		Last Modified: Wed, 13 May 2020 21:11:35 GMT  
		Size: 1.1 MB (1134692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea93b4316081dba615b7e4d490934ed3ec3cf7979bf5200d7455309149f554c2`  
		Last Modified: Wed, 13 May 2020 21:11:35 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c26e78f516132b9ab5e5b47948d2171d973044571df9d3fcfef732b08086425`  
		Last Modified: Wed, 13 May 2020 21:11:34 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:latest` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:d423b2ef6d053c533639c07693e0cfca1ccb8715b1825c9dd09a5e8754ab1af7
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.1 MB (29102138 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d2b62ffbdd70a7d226f91ebe12b68d7ad5b580ea2fdb690621b441e7a64b2ab`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 23 Apr 2020 00:54:55 GMT
ADD file:581ee9c3c19f0d971aeda008fd399f59171cae75e8936b967dbf3888db4fc0d0 in / 
# Thu, 23 Apr 2020 00:54:58 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 03:03:20 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Thu, 23 Apr 2020 03:03:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 13 May 2020 20:56:07 GMT
ENV MEMCACHED_VERSION=1.6.6
# Wed, 13 May 2020 20:56:08 GMT
ENV MEMCACHED_SHA1=d8895b12dc9fc82b389f1713e2c09cc6ca3d03e4
# Wed, 13 May 2020 21:06:19 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 13 May 2020 21:06:20 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 13 May 2020 21:06:22 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 13 May 2020 21:06:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 13 May 2020 21:06:23 GMT
USER memcache
# Wed, 13 May 2020 21:06:24 GMT
EXPOSE 11211
# Wed, 13 May 2020 21:06:24 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:bdc84a41f2513e28e99efeff9fcbb196b7df9883fb30532184bd67ca415b4673`  
		Last Modified: Thu, 23 Apr 2020 01:03:27 GMT  
		Size: 25.9 MB (25857800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b8ed987f36e3ad8893c5c7ce9e42aeb35d67e90daf262dde60d86dfa94814f5`  
		Last Modified: Thu, 23 Apr 2020 03:32:22 GMT  
		Size: 5.0 KB (5028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:360e6a91a753e3a018e26a9d22b25766c2ebd2231cbc3e245648aead98ddde08`  
		Last Modified: Thu, 23 Apr 2020 03:32:23 GMT  
		Size: 2.1 MB (2074961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9beea1961eacb995614a88fb9793f9a187c12a86f94a6be75130effc76976768`  
		Last Modified: Wed, 13 May 2020 21:17:27 GMT  
		Size: 1.2 MB (1163938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b48ab287b49fd3b8a7f96050d1d72454c2581bae20dbdd2d52ec0d9766d2d56`  
		Last Modified: Wed, 13 May 2020 21:17:26 GMT  
		Size: 290.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dce9e28ac95b05cd478c90cb28edf8e74c70f8fc79bd3acde6d5104bd563f32b`  
		Last Modified: Wed, 13 May 2020 21:17:25 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:latest` - linux; 386

```console
$ docker pull memcached@sha256:4cd7c8a145c4b502f84c55f41e0ae4971614a237b96076093edb951df16af86f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.2 MB (31163013 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66532fde035d2034732c7b657027f1f342acdb811b1d859d9f6ed3bc370262e2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 23 Apr 2020 00:39:36 GMT
ADD file:ca6a74f6b738c738c033152fab2a9aacf22bec5f19a994e6a02b5f919ee33ee9 in / 
# Thu, 23 Apr 2020 00:39:36 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 01:29:35 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Thu, 23 Apr 2020 01:29:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 01:29:42 GMT
ENV MEMCACHED_VERSION=1.6.5
# Thu, 23 Apr 2020 01:29:42 GMT
ENV MEMCACHED_SHA1=1ddb5f37f69946b63512ad0f89dc448ff7ba5713
# Thu, 23 Apr 2020 01:38:20 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 23 Apr 2020 01:38:20 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 23 Apr 2020 01:38:21 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 23 Apr 2020 01:38:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Apr 2020 01:38:21 GMT
USER memcache
# Thu, 23 Apr 2020 01:38:21 GMT
EXPOSE 11211
# Thu, 23 Apr 2020 01:38:21 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:5d3da8f33b97fc107a05b3255a55836b76df9f817de632b1fb63c6e9c024f0df`  
		Last Modified: Thu, 23 Apr 2020 00:44:35 GMT  
		Size: 27.8 MB (27753972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c3cb2639d5e9c8ab44fd2bbe5bedbb5c4d33378f9781d558d2ac27611ecd673`  
		Last Modified: Thu, 23 Apr 2020 01:38:35 GMT  
		Size: 4.9 KB (4898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6f2f84fd6631cbca67ed46fd3b380a42475afb287d8e990ded3d3a91fded71a`  
		Last Modified: Thu, 23 Apr 2020 01:38:35 GMT  
		Size: 2.2 MB (2208055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae882751a1fc445bebd4d4f545c0c69529396863b7ac0b3fc3137b2c3cecbfaa`  
		Last Modified: Thu, 23 Apr 2020 01:38:35 GMT  
		Size: 1.2 MB (1195679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d53c7886eeb4da4192fe5caceac337d1fa31afc20be46a9476fd10e35bd4d81e`  
		Last Modified: Thu, 23 Apr 2020 01:38:35 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43f9bc6252b62803993a04eff4ad6e08d728474f2c446e92d32b5ab3ac38ab08`  
		Last Modified: Thu, 23 Apr 2020 01:38:35 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:latest` - linux; mips64le

```console
$ docker pull memcached@sha256:2b4b9c9aba5b7a352d4f631bfdf5b38489d2e2ea2bb40ce5c0d592d2f3beb517
```

-	Docker Version: 19.03.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.7 MB (28725203 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:53b77428fcdf16a094d4463e769da9547573740a8f4723c8951289da773cd5a4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 23 Apr 2020 00:09:47 GMT
ADD file:7509945bd8a224048260e88b466aa3b156615e16b64e0a6702da277052fcb98b in / 
# Thu, 23 Apr 2020 00:09:48 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 01:41:19 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Thu, 23 Apr 2020 01:41:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 01:41:33 GMT
ENV MEMCACHED_VERSION=1.6.5
# Thu, 23 Apr 2020 01:41:33 GMT
ENV MEMCACHED_SHA1=1ddb5f37f69946b63512ad0f89dc448ff7ba5713
# Sun, 26 Apr 2020 13:18:16 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Sun, 26 Apr 2020 13:18:17 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Sun, 26 Apr 2020 13:18:19 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Sun, 26 Apr 2020 13:18:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sun, 26 Apr 2020 13:18:20 GMT
USER memcache
# Sun, 26 Apr 2020 13:18:20 GMT
EXPOSE 11211
# Sun, 26 Apr 2020 13:18:20 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:ae8f0fa6cb0d971b4b8fedf7fc9b00f61f780b383fe7d64e6c2e4be8d20c3987`  
		Last Modified: Thu, 23 Apr 2020 00:17:46 GMT  
		Size: 25.8 MB (25762125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af60fd257f6555ca6e3d16a15d8ffa2104ab04985a4ed8086673ea9a801fd4e3`  
		Last Modified: Sun, 26 Apr 2020 13:18:38 GMT  
		Size: 5.0 KB (4983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f1056e8039be8264aef0eb2e4da6fc056a4ca433ef9c12b2249c56daa5c80d1`  
		Last Modified: Sun, 26 Apr 2020 13:18:40 GMT  
		Size: 1.8 MB (1775978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11395212b0482ecc9c692dec8ec4b925f6a00bf9e1221b5346ee0e0adaf15bcf`  
		Last Modified: Sun, 26 Apr 2020 13:18:39 GMT  
		Size: 1.2 MB (1181708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b73dfa2d44a3c35a22d2140a094f6791462908f7643607468b7ab494ba8466e`  
		Last Modified: Sun, 26 Apr 2020 13:18:38 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a944298863ce1f89b5fd93b096bb2353280d7b5cd6f08d6e370b80a8624ebe8a`  
		Last Modified: Sun, 26 Apr 2020 13:18:38 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:latest` - linux; ppc64le

```console
$ docker pull memcached@sha256:72020baf7b956f0e50b60da653793669acfe24dab1c0e03c92e4101756c69870
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.1 MB (34070273 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:13679844e3928d60db09df9f08012634fe562bf0bbe2755d7e8bdfc5a8843dee`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 23 Apr 2020 00:36:00 GMT
ADD file:5b3c3d2945800e1743dc02a4f68bd830fe2f67ca437223692eb460147c158c2b in / 
# Thu, 23 Apr 2020 00:36:04 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 05:29:22 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Thu, 23 Apr 2020 05:29:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 05:29:41 GMT
ENV MEMCACHED_VERSION=1.6.5
# Thu, 23 Apr 2020 05:29:43 GMT
ENV MEMCACHED_SHA1=1ddb5f37f69946b63512ad0f89dc448ff7ba5713
# Thu, 23 Apr 2020 05:39:43 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 23 Apr 2020 05:39:44 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 23 Apr 2020 05:39:48 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 23 Apr 2020 05:39:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Apr 2020 05:39:51 GMT
USER memcache
# Thu, 23 Apr 2020 05:39:53 GMT
EXPOSE 11211
# Thu, 23 Apr 2020 05:39:55 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:012c6cdbd1af202bbfbea5945fafbb9aca9097f1fa3cb493a29155fdc02cc43c`  
		Last Modified: Thu, 23 Apr 2020 00:50:14 GMT  
		Size: 30.5 MB (30524638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca611c057695089b7850ed3bf7f38c5979756d58e7de7d6c7307568e0ac9000d`  
		Last Modified: Thu, 23 Apr 2020 05:40:21 GMT  
		Size: 5.0 KB (4988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e22a29cab6d03b4f3f09bf64881923227d5fc4d38aa6a1c8367751663ed3694a`  
		Last Modified: Thu, 23 Apr 2020 05:40:21 GMT  
		Size: 2.3 MB (2322671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b265c0fd772a3a696cd9c7860788c4e3b7287f882955c5e459a6c41b64a7e531`  
		Last Modified: Thu, 23 Apr 2020 05:40:22 GMT  
		Size: 1.2 MB (1217568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a05552e552ebc4b7164ee3b7161d37f2672294b65d98445aa530535ec57dd7f5`  
		Last Modified: Thu, 23 Apr 2020 05:40:21 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce1f225499a970ebb67b042406d96bb81fe400cc061e7e275de90e73499ca5db`  
		Last Modified: Thu, 23 Apr 2020 05:40:21 GMT  
		Size: 120.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:latest` - linux; s390x

```console
$ docker pull memcached@sha256:267df373701f14c0f868a2a95f6690723010071a8982a2b6a87f9e4afafb89dc
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.8 MB (28788396 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:be9e90914277188f44c6a29fec5f783023e7665d98f610dc36b3087ae622a8ac`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 23 Apr 2020 00:51:48 GMT
ADD file:f6c2560f9185c1bcaff95e576e57449f606d51b85fad02646c1b0962bc9353c9 in / 
# Thu, 23 Apr 2020 00:51:50 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 00:58:53 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Thu, 23 Apr 2020 00:58:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 13 May 2020 20:34:57 GMT
ENV MEMCACHED_VERSION=1.6.6
# Wed, 13 May 2020 20:34:57 GMT
ENV MEMCACHED_SHA1=d8895b12dc9fc82b389f1713e2c09cc6ca3d03e4
# Wed, 13 May 2020 20:43:55 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 13 May 2020 20:43:55 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 13 May 2020 20:43:56 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 13 May 2020 20:43:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 13 May 2020 20:43:56 GMT
USER memcache
# Wed, 13 May 2020 20:43:56 GMT
EXPOSE 11211
# Wed, 13 May 2020 20:43:57 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:d89dc3741ad42b79c3d8545495c429f3100d3f22234ff993bd04017b0675e868`  
		Last Modified: Thu, 23 Apr 2020 00:56:00 GMT  
		Size: 25.7 MB (25712105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed7b337870b6c06d26297cc61114e98f8d23b6cfd7ceda5779286b09d85058e8`  
		Last Modified: Wed, 13 May 2020 20:53:33 GMT  
		Size: 5.0 KB (5028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c35c02588420fb9764d4f49d302f8e0d38aa8665a3f567a238a90c3be58b6b46`  
		Last Modified: Wed, 13 May 2020 20:53:33 GMT  
		Size: 1.9 MB (1886010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8781268196c7fca5682511a33b8fa3847b89e8a56b81d4a95e45c914b19dbb74`  
		Last Modified: Wed, 13 May 2020 20:53:32 GMT  
		Size: 1.2 MB (1184846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:926216811f65028b36b78fac4d9bd85fa41c2b6b8f07b8bd466207403e99cb38`  
		Last Modified: Wed, 13 May 2020 20:53:38 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6de9b312d644cc1f4014c4aceb68cdca1cc2a710fadeaf50d94511ba356784e`  
		Last Modified: Wed, 13 May 2020 20:53:38 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
