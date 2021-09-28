<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `memcached`

-	[`memcached:1`](#memcached1)
-	[`memcached:1-alpine`](#memcached1-alpine)
-	[`memcached:1-alpine3.14`](#memcached1-alpine314)
-	[`memcached:1-buster`](#memcached1-buster)
-	[`memcached:1.6`](#memcached16)
-	[`memcached:1.6-alpine`](#memcached16-alpine)
-	[`memcached:1.6-alpine3.14`](#memcached16-alpine314)
-	[`memcached:1.6-buster`](#memcached16-buster)
-	[`memcached:1.6.10`](#memcached1610)
-	[`memcached:1.6.10-alpine`](#memcached1610-alpine)
-	[`memcached:1.6.10-alpine3.14`](#memcached1610-alpine314)
-	[`memcached:1.6.10-buster`](#memcached1610-buster)
-	[`memcached:alpine`](#memcachedalpine)
-	[`memcached:alpine3.14`](#memcachedalpine314)
-	[`memcached:buster`](#memcachedbuster)
-	[`memcached:latest`](#memcachedlatest)

## `memcached:1`

```console
$ docker pull memcached@sha256:0507080446e022bbcb398fef743f5479d61569f2992beccd200033e037968511
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
$ docker pull memcached@sha256:b93ad58a06f215580205490133ce2165fa69f1930b964e890981f629df497e84
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.6 MB (30631755 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:444d9869f3507356b3fb6ffb7ed74ffc3be04be873a6876423c24d17acbf1128`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 03 Sep 2021 01:21:46 GMT
ADD file:4ff85d9f6aa246746912db62dea02eb71750474bb29611e770516a1fcd217add in / 
# Fri, 03 Sep 2021 01:21:46 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 07:33:54 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Fri, 03 Sep 2021 07:34:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 07:34:01 GMT
ENV MEMCACHED_VERSION=1.6.10
# Fri, 03 Sep 2021 07:34:01 GMT
ENV MEMCACHED_SHA1=cb5b9fe77a2a59cc6cc7103a415bc07df9ddc6ec
# Fri, 03 Sep 2021 07:38:24 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Fri, 03 Sep 2021 07:38:24 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 03 Sep 2021 07:38:25 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 03 Sep 2021 07:38:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 03 Sep 2021 07:38:25 GMT
USER memcache
# Fri, 03 Sep 2021 07:38:26 GMT
EXPOSE 11211
# Fri, 03 Sep 2021 07:38:26 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:a330b6cecb98cd2425fd25fce36669073f593b3176b4ee14731e48c05d678cdd`  
		Last Modified: Fri, 03 Sep 2021 01:28:19 GMT  
		Size: 27.1 MB (27145844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7dcde8d481fe08e2bab1fc8a1dc0e30c1d8cc9647d2867a6bc06942de810d56`  
		Last Modified: Fri, 03 Sep 2021 07:38:54 GMT  
		Size: 5.0 KB (4981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c3e0b65008f095303aa1ff733845d2eed7b3836fad196bc16533b3420711745`  
		Last Modified: Fri, 03 Sep 2021 07:38:54 GMT  
		Size: 2.2 MB (2197580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ad3eb30b171e7b0c33373bdeb39dfc36b63b8ec501af75bae3d4a964872f042`  
		Last Modified: Fri, 03 Sep 2021 07:38:54 GMT  
		Size: 1.3 MB (1282944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e6e03de9a5467b70b4d10bf021740a05eea1aeebfd87864b4a9289df9cb64c0`  
		Last Modified: Fri, 03 Sep 2021 07:38:54 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe0025a339764c7acc0034c701ca2b443e0b1803745c41094ea54289f754a81c`  
		Last Modified: Fri, 03 Sep 2021 07:38:54 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1` - linux; arm variant v5

```console
$ docker pull memcached@sha256:5e1d0b6ce4b1b257e47c484709733908552416681c8f054bc97735e5ec114fa2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.0 MB (28036699 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd9fb75ae310df2e536d3a10e6dd9222317f89456fe6082c139b112849e5081b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 03 Sep 2021 00:51:26 GMT
ADD file:350748a564076da397b991745cd42e0688d15c72b9fd5c81f8ea0bb8938a2b3d in / 
# Fri, 03 Sep 2021 00:51:27 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 02:24:47 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Fri, 03 Sep 2021 02:24:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 02:24:58 GMT
ENV MEMCACHED_VERSION=1.6.10
# Fri, 03 Sep 2021 02:24:59 GMT
ENV MEMCACHED_SHA1=cb5b9fe77a2a59cc6cc7103a415bc07df9ddc6ec
# Fri, 03 Sep 2021 02:29:11 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Fri, 03 Sep 2021 02:29:12 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 03 Sep 2021 02:29:13 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 03 Sep 2021 02:29:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 03 Sep 2021 02:29:14 GMT
USER memcache
# Fri, 03 Sep 2021 02:29:14 GMT
EXPOSE 11211
# Fri, 03 Sep 2021 02:29:15 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:b019db4b5197128481d48d92ecacd6bb356c027a3d08393f6567a6fa183ba769`  
		Last Modified: Fri, 03 Sep 2021 01:07:12 GMT  
		Size: 24.9 MB (24879114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4faeba39e66674ac57454c2edb8018a9a29475db4893acb59bf00e84e5c4e88a`  
		Last Modified: Fri, 03 Sep 2021 02:30:10 GMT  
		Size: 4.9 KB (4895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b39e5da0381154e8db96921f6038b79a61f458bf76f9fdaae0d3f44b2d81f184`  
		Last Modified: Fri, 03 Sep 2021 02:30:11 GMT  
		Size: 1.9 MB (1897972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb47be4e43a9bfad0082a507b5885f22b4104821defe786af5237a6b48211a71`  
		Last Modified: Fri, 03 Sep 2021 02:30:11 GMT  
		Size: 1.3 MB (1254312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee01c0ace3ff5a5a86664234d47a50480b12f50f1390f5b78ab2b76a73e3346f`  
		Last Modified: Fri, 03 Sep 2021 02:30:10 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:240af99f2a1c8953e4436d48b387f4aa33defc9e83416c71f2d67d05c2a8cb48`  
		Last Modified: Fri, 03 Sep 2021 02:30:10 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1` - linux; arm variant v7

```console
$ docker pull memcached@sha256:ee3f4a07ff534651238a464f5b0a3b582facdc9784f9e0f9a5bcd0128762da4f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.8 MB (25788867 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6222a822647e49fef3f296a084e4504bd705efe8e0649bc91541e03b8a5d7b8a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 03 Sep 2021 01:00:40 GMT
ADD file:4754bbccf4c59f77dd54f3888871f0635a2f9655cda53f50e63237f1580286e0 in / 
# Fri, 03 Sep 2021 01:00:41 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 06:44:19 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Fri, 03 Sep 2021 06:44:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 06:44:29 GMT
ENV MEMCACHED_VERSION=1.6.10
# Fri, 03 Sep 2021 06:44:30 GMT
ENV MEMCACHED_SHA1=cb5b9fe77a2a59cc6cc7103a415bc07df9ddc6ec
# Fri, 03 Sep 2021 06:48:21 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Fri, 03 Sep 2021 06:48:22 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 03 Sep 2021 06:48:23 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 03 Sep 2021 06:48:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 03 Sep 2021 06:48:24 GMT
USER memcache
# Fri, 03 Sep 2021 06:48:25 GMT
EXPOSE 11211
# Fri, 03 Sep 2021 06:48:25 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:2215ad7863d95c38f1f794f1d5b4d6c5ca4ca7e921e4bb7218b803f7ed270675`  
		Last Modified: Fri, 03 Sep 2021 01:16:23 GMT  
		Size: 22.7 MB (22746151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d554d32fa680ffcf04f8b509fa6a16e796fadc0ecf8db8c48bcc2a911f9f4591`  
		Last Modified: Fri, 03 Sep 2021 07:00:56 GMT  
		Size: 4.9 KB (4895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a550041e12d651682f2b70b45620898d8cebd97f4b4b3469aaeac8d452a76ef`  
		Last Modified: Fri, 03 Sep 2021 07:00:56 GMT  
		Size: 1.8 MB (1812490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ae1581582d0b08a4635fe57247a454da856fea52ec988126ee4f2f1781b7acd`  
		Last Modified: Fri, 03 Sep 2021 07:00:56 GMT  
		Size: 1.2 MB (1224925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:678c3e64de445bdc9a420655f01c8abab5f2e7ef4f41d441e6d2310ea2c36de5`  
		Last Modified: Fri, 03 Sep 2021 07:00:55 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a21b13a7b8549e46debb4d9b1117211df9edcc02f822ec99d1fe1b4278f1e56`  
		Last Modified: Fri, 03 Sep 2021 07:00:55 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:57e906b2282c3e67137cc8c2ab5148c8e748256b2e3934c5b7ecd77a6a186de5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.3 MB (29250783 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:932f1c94fc6e8e017820dcb97fe4b624efacba7409cb99c99a369c649b03829d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 03 Sep 2021 00:40:58 GMT
ADD file:4a1d7f2d989aee6bd83da076b6e9dd3da2da97cf5654bd37568e9baec30ac4b1 in / 
# Fri, 03 Sep 2021 00:40:58 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 02:46:23 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Fri, 03 Sep 2021 02:46:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 02:46:27 GMT
ENV MEMCACHED_VERSION=1.6.10
# Fri, 03 Sep 2021 02:46:28 GMT
ENV MEMCACHED_SHA1=cb5b9fe77a2a59cc6cc7103a415bc07df9ddc6ec
# Fri, 03 Sep 2021 02:50:03 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Fri, 03 Sep 2021 02:50:03 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 03 Sep 2021 02:50:04 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 03 Sep 2021 02:50:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 03 Sep 2021 02:50:04 GMT
USER memcache
# Fri, 03 Sep 2021 02:50:05 GMT
EXPOSE 11211
# Fri, 03 Sep 2021 02:50:05 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:d10c227306ce3db344a8399cbc02bbf0dcb36519318efbde3c6027c00be8b40e`  
		Last Modified: Fri, 03 Sep 2021 00:49:47 GMT  
		Size: 25.9 MB (25914860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee708d85ae4c6929688ee243da330a395c81a5da3913f7aaaeea88283b5752b1`  
		Last Modified: Fri, 03 Sep 2021 02:51:01 GMT  
		Size: 5.0 KB (5024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41eee23f132aa5ef6810f141bd4852d174eb68bd5e9f8fc4e278e2fc55f7cea8`  
		Last Modified: Fri, 03 Sep 2021 02:51:02 GMT  
		Size: 2.1 MB (2075717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d9a7819a72ed1b598aabafd5ac9be7be62ac6b085cc30dbda97ef193641fc05`  
		Last Modified: Fri, 03 Sep 2021 02:51:01 GMT  
		Size: 1.3 MB (1254776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ae146d1bf5917e1fb0f4aa46a655feefc0ec5e00ef4e775beed00fa6a1d0aa1`  
		Last Modified: Fri, 03 Sep 2021 02:51:01 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3cae1f92b0ec75c4c83b4b5a4ce47b455952d638c215f1588a20af7261fba5b`  
		Last Modified: Fri, 03 Sep 2021 02:51:01 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1` - linux; 386

```console
$ docker pull memcached@sha256:221d230cb426e233ce34c9669663db5628d85a6ffe1d98292cfb54d66a7e1f8a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.3 MB (31292631 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7283abe72dd41573bd7262a0ba163f6ef7ddf757bc5178c95eea585f8335e784`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 03 Sep 2021 00:40:24 GMT
ADD file:6bf4b6f4aa28306610ef10c68f422a7210ff2fbd5345cec07bc5f76d54a4c8bc in / 
# Fri, 03 Sep 2021 00:40:24 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 06:44:15 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Fri, 03 Sep 2021 06:44:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 06:44:21 GMT
ENV MEMCACHED_VERSION=1.6.10
# Fri, 03 Sep 2021 06:44:21 GMT
ENV MEMCACHED_SHA1=cb5b9fe77a2a59cc6cc7103a415bc07df9ddc6ec
# Fri, 03 Sep 2021 06:48:23 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Fri, 03 Sep 2021 06:48:24 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 03 Sep 2021 06:48:25 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 03 Sep 2021 06:48:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 03 Sep 2021 06:48:26 GMT
USER memcache
# Fri, 03 Sep 2021 06:48:26 GMT
EXPOSE 11211
# Fri, 03 Sep 2021 06:48:26 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:7e87f600658a0c0d3bd8b82b9c645b5ec2763492ec627c1c1c1183c2ad3c45d5`  
		Last Modified: Fri, 03 Sep 2021 00:49:06 GMT  
		Size: 27.8 MB (27797513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9454a8c8c54135f6e7f591277550407671a2a183d0ea7a1b04e0b7bf1ecfeb39`  
		Last Modified: Fri, 03 Sep 2021 06:49:32 GMT  
		Size: 4.9 KB (4895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4900dba329569a63986180bc83b94449c1dffc3a804c2910a2a3f288509964d3`  
		Last Modified: Fri, 03 Sep 2021 06:49:32 GMT  
		Size: 2.2 MB (2209620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb8624563e6585b031c874cc180ee08148f5773238b0bc1571feb1b64b198ee5`  
		Last Modified: Fri, 03 Sep 2021 06:49:32 GMT  
		Size: 1.3 MB (1280199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86f15c6c59e3205f04fba85035da98cd62d3f67bca6baa035b56db7f4f5dfb5c`  
		Last Modified: Fri, 03 Sep 2021 06:49:32 GMT  
		Size: 283.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f1b51c6ca8d549a8b18622d1c15504b94257295420bc332544f8d9026fff6f3`  
		Last Modified: Fri, 03 Sep 2021 06:49:32 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1` - linux; mips64le

```console
$ docker pull memcached@sha256:33ce4398cd07967870c76b95ec5314cbe8280d564309b25d0640e8dd94cb7198
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.9 MB (28866865 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cc3e459293995ad1867b805e319ebb5b3942502abbad00cf3f9b3a4ccc26c740`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 28 Sep 2021 02:11:41 GMT
ADD file:df525c65bc60141f19ab937525d724c6d29cac53beb30f92d79ea4b2edf5a13e in / 
# Tue, 28 Sep 2021 02:11:41 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 02:51:00 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 28 Sep 2021 02:51:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:51:13 GMT
ENV MEMCACHED_VERSION=1.6.10
# Tue, 28 Sep 2021 02:51:13 GMT
ENV MEMCACHED_SHA1=cb5b9fe77a2a59cc6cc7103a415bc07df9ddc6ec
# Tue, 28 Sep 2021 02:56:56 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 28 Sep 2021 02:56:56 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 28 Sep 2021 02:56:58 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 28 Sep 2021 02:56:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 28 Sep 2021 02:56:59 GMT
USER memcache
# Tue, 28 Sep 2021 02:56:59 GMT
EXPOSE 11211
# Tue, 28 Sep 2021 02:56:59 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:f1b3d9dde862ddf88a05cec47ce54e641c4057c7bfb377e2a065c72a42a76321`  
		Last Modified: Tue, 28 Sep 2021 02:22:07 GMT  
		Size: 25.8 MB (25813001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e684588e988c227c0fedbcfeb8361e35b75eaa06e38cf8207979b491712d3dc`  
		Last Modified: Tue, 28 Sep 2021 02:57:18 GMT  
		Size: 5.0 KB (4981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35a3bc6181fe53d4bf46e98ebace046f2014668d601c2c3975c3dc6fc655acbc`  
		Last Modified: Tue, 28 Sep 2021 02:57:19 GMT  
		Size: 1.8 MB (1777273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f49b3d8a270ebba87297e2461fe81567f28a880e22d7ef977a60930ad82d6aa6`  
		Last Modified: Tue, 28 Sep 2021 02:57:19 GMT  
		Size: 1.3 MB (1271204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:119de6bb61edbff9dc8919b6bbb0f35c144a065c899d3fe20127480e2985c0d8`  
		Last Modified: Tue, 28 Sep 2021 02:57:18 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ecffae4c1838eb68ee866feaae4a6357c6198f1e86b5a1719bd7646795396d6`  
		Last Modified: Tue, 28 Sep 2021 02:57:18 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1` - linux; ppc64le

```console
$ docker pull memcached@sha256:49728dba09507cb74bbfae419b5b8051106768fd3b53aa7964da2b4a7cf0d44f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.2 MB (34190787 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4563ba0117902a70591f2170ab90e34de0431ae24402ee05aa741d4eafbd036f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 03 Sep 2021 01:24:33 GMT
ADD file:6c1662ddb92232ae8969a86a18dacab97b3b5792a1ecda49e6ac741a1a5c878c in / 
# Fri, 03 Sep 2021 01:24:41 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 08:06:59 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Fri, 03 Sep 2021 08:07:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 08:07:23 GMT
ENV MEMCACHED_VERSION=1.6.10
# Fri, 03 Sep 2021 08:07:26 GMT
ENV MEMCACHED_SHA1=cb5b9fe77a2a59cc6cc7103a415bc07df9ddc6ec
# Fri, 03 Sep 2021 08:13:31 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Fri, 03 Sep 2021 08:13:32 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 03 Sep 2021 08:13:43 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 03 Sep 2021 08:13:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 03 Sep 2021 08:13:57 GMT
USER memcache
# Fri, 03 Sep 2021 08:14:01 GMT
EXPOSE 11211
# Fri, 03 Sep 2021 08:14:05 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:8258146296247df1f308a336d4abf286afae14e3375edefb87a091e80745e29f`  
		Last Modified: Fri, 03 Sep 2021 01:39:45 GMT  
		Size: 30.6 MB (30553675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2f96132a11c70c50168ade17294cf7e8c919db231f87a28818170d9917a3268`  
		Last Modified: Fri, 03 Sep 2021 08:14:54 GMT  
		Size: 5.0 KB (4988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:973046a9e11e4bf003ce0e9688dc396e6e0ded760e9914a57132e130fa64289a`  
		Last Modified: Fri, 03 Sep 2021 08:14:55 GMT  
		Size: 2.3 MB (2323873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e5495ff67177662caa9f0459d68cb0641f32eddb666f4238634e357e58bdad1`  
		Last Modified: Fri, 03 Sep 2021 08:14:55 GMT  
		Size: 1.3 MB (1307845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b406b4303f1d8fe163586ca2e7abe3639c752a524f2c44e46677c01e36f937c`  
		Last Modified: Fri, 03 Sep 2021 08:14:54 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ff817a29aac3d654f6e919cbea3ea8125cce972e357c595217ec95807e07c3d`  
		Last Modified: Fri, 03 Sep 2021 08:14:54 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1` - linux; s390x

```console
$ docker pull memcached@sha256:53459c6f3d42b7b718e1ccbb3090ff35e649d8d005fa1917cee1ee1fbfea608a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.9 MB (28925755 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8831bffed7f4d435dd3c714d24529fea34f84468cbc5abec57feeb4728059de`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 28 Sep 2021 01:43:29 GMT
ADD file:118e7a596407435b5e2ff0aae6bb9bff3b66000c91ca37bfe1eeb98c23d99d49 in / 
# Tue, 28 Sep 2021 01:43:30 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 02:31:35 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 28 Sep 2021 02:31:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:31:39 GMT
ENV MEMCACHED_VERSION=1.6.10
# Tue, 28 Sep 2021 02:31:39 GMT
ENV MEMCACHED_SHA1=cb5b9fe77a2a59cc6cc7103a415bc07df9ddc6ec
# Tue, 28 Sep 2021 02:34:53 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 28 Sep 2021 02:34:54 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 28 Sep 2021 02:34:54 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 28 Sep 2021 02:34:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 28 Sep 2021 02:34:54 GMT
USER memcache
# Tue, 28 Sep 2021 02:34:54 GMT
EXPOSE 11211
# Tue, 28 Sep 2021 02:34:55 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:7cfe208f95c1b63305981b069795676fa149e7115b9044c241ee45ef4aaf0bb3`  
		Last Modified: Tue, 28 Sep 2021 01:49:36 GMT  
		Size: 25.8 MB (25760871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff755a70833a769c5a32cb251e86ac9aa6ae1dce7f547dc1bef874a22855b63d`  
		Last Modified: Tue, 28 Sep 2021 02:35:52 GMT  
		Size: 5.0 KB (5022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d08a7a4b96e17b9ef0eb0b8dd97ad0dc3d75227841b6374b7071e7989d9fed3c`  
		Last Modified: Tue, 28 Sep 2021 02:35:52 GMT  
		Size: 1.9 MB (1887230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4b9662cd31c943100c81ad7c951195bf462ad510ed53de50144b8617d870a84`  
		Last Modified: Tue, 28 Sep 2021 02:35:52 GMT  
		Size: 1.3 MB (1272226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fc50167475bec35471f2d4f925c2d427f3757ac01cd3f8f82cc5685771c2744`  
		Last Modified: Tue, 28 Sep 2021 02:35:52 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c69d6c53bee775bfd205e1d0426724cebf2eddd3034e82681311e18028641c25`  
		Last Modified: Tue, 28 Sep 2021 02:35:52 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:1-alpine`

```console
$ docker pull memcached@sha256:99e30a033ef422d6ad3ebe18c6c1009f20bee2d025fc00569be5dcd81aadc7be
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 7
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `memcached:1-alpine` - linux; amd64

```console
$ docker pull memcached@sha256:67d93d2efc4859c0b2e5a24bc13e759788c1f28d97a4d68b58a3de323e8ccb38
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3904613 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec200929117689b8cbba5a24fe5e892d7e4bfec5b654cef54958801a6ab9e92b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Fri, 27 Aug 2021 20:39:15 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Fri, 27 Aug 2021 20:39:16 GMT
RUN apk add --no-cache libsasl
# Fri, 27 Aug 2021 20:39:16 GMT
ENV MEMCACHED_VERSION=1.6.10
# Fri, 27 Aug 2021 20:39:17 GMT
ENV MEMCACHED_SHA1=cb5b9fe77a2a59cc6cc7103a415bc07df9ddc6ec
# Fri, 27 Aug 2021 20:43:47 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Fri, 27 Aug 2021 20:43:47 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 27 Aug 2021 20:43:49 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 27 Aug 2021 20:43:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 Aug 2021 20:43:50 GMT
USER memcache
# Fri, 27 Aug 2021 20:43:50 GMT
EXPOSE 11211
# Fri, 27 Aug 2021 20:43:50 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:a0d0a0d46f8b52473982a3c466318f479767577551a53ffc9074c9fa7035982e`  
		Last Modified: Fri, 27 Aug 2021 17:20:13 GMT  
		Size: 2.8 MB (2814446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84db6e403c6f8cdc8217536fa7d8bb9bbee66a7a49106104b3ceeace758e887b`  
		Last Modified: Fri, 27 Aug 2021 20:44:26 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7430c0d88cc6cc6389bb62e421f43031b009d21243f7362290bcf11b82e9e967`  
		Last Modified: Fri, 27 Aug 2021 20:44:26 GMT  
		Size: 155.5 KB (155516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3919afa4c767ba881b469a2798f6ad270dc23bbd9174d2994a0208bf508febba`  
		Last Modified: Fri, 27 Aug 2021 20:44:26 GMT  
		Size: 933.0 KB (932979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e81a6f988f7ee7ae5df06403e582d0edb09dcd73e81bacdaa17d1e0da71e13b`  
		Last Modified: Fri, 27 Aug 2021 20:44:26 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d5ed3d833f3ab3255decd4fc642f2368e6791acc470e40c2f3eb7463b7351dc`  
		Last Modified: Fri, 27 Aug 2021 20:44:26 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-alpine` - linux; arm variant v6

```console
$ docker pull memcached@sha256:4d05de82436bd51ed609a745b8ddd01e296692beb5a372dcbdcf0b1f54818d03
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.3 MB (4270486 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:56e8bda6e6346ca01fa3a313ef7bcfcc696040d48be803f6c16922dedc8deae1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 16 Dec 2020 23:49:43 GMT
ADD file:0a16715e2d0e5811c3c578945d618db0e269847a799340248f9ba8d393c9eec2 in / 
# Wed, 16 Dec 2020 23:49:45 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 01:44:25 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Thu, 17 Dec 2020 01:44:29 GMT
RUN apk add --no-cache cyrus-sasl-plain
# Thu, 17 Dec 2020 01:44:30 GMT
ENV MEMCACHED_VERSION=1.6.9
# Thu, 17 Dec 2020 01:44:31 GMT
ENV MEMCACHED_SHA1=42ae062094fdf083cfe7b21ff377c781011c2be1
# Thu, 17 Dec 2020 01:47:40 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		dpkg-dev dpkg 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		tar 		wget 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Thu, 17 Dec 2020 01:47:41 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 17 Dec 2020 01:47:43 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 17 Dec 2020 01:47:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Dec 2020 01:47:44 GMT
USER memcache
# Thu, 17 Dec 2020 01:47:45 GMT
EXPOSE 11211
# Thu, 17 Dec 2020 01:47:46 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:93247449aef3c56eb4f7ab7b3fed95743c974b823def6dd86ec84008126e7903`  
		Last Modified: Wed, 16 Dec 2020 23:50:24 GMT  
		Size: 2.6 MB (2604163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cc04af65958529b14246e2401008ef0186d74a33d2aa1b64d5f49633a1ff8f1`  
		Last Modified: Thu, 17 Dec 2020 01:48:06 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08bb28157acd02855bdf031eb7158f2cbb9849a6a9e6b45b4b82b507df6d83e9`  
		Last Modified: Thu, 17 Dec 2020 01:48:06 GMT  
		Size: 14.9 KB (14904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b32778d38f805e0e2a84689dba047adda457098c6f4a0b3aeb51a9e9d3e7f2b`  
		Last Modified: Thu, 17 Dec 2020 01:48:06 GMT  
		Size: 1.6 MB (1649753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:506d15aa86681d1812c5696615302d2a50938410c852b6aa0d0680c7baa4589f`  
		Last Modified: Thu, 17 Dec 2020 01:48:06 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f55730e61cf75cdadfaf0682212c74d7a2355e652e0655cc74ba35a4b7cfb4c1`  
		Last Modified: Thu, 17 Dec 2020 01:48:06 GMT  
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
$ docker pull memcached@sha256:8ed70173927cd66ad4e1bac9803ba7114502646685f70abb395ef668a46db5fb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3793233 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c5c3d9ec3f6b46ae9e7305a3958b059ffc7d935b5f2094e78973054a0394060e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 27 Aug 2021 17:39:33 GMT
ADD file:dc8af9c7bfe9f9541e1db38dea01c4201609f3075b31e108f2073ffed8c5e4b9 in / 
# Fri, 27 Aug 2021 17:39:33 GMT
CMD ["/bin/sh"]
# Fri, 27 Aug 2021 20:15:01 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Fri, 27 Aug 2021 20:15:02 GMT
RUN apk add --no-cache libsasl
# Fri, 27 Aug 2021 20:15:02 GMT
ENV MEMCACHED_VERSION=1.6.10
# Fri, 27 Aug 2021 20:15:02 GMT
ENV MEMCACHED_SHA1=cb5b9fe77a2a59cc6cc7103a415bc07df9ddc6ec
# Fri, 27 Aug 2021 20:18:55 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Fri, 27 Aug 2021 20:18:55 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 27 Aug 2021 20:18:56 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 27 Aug 2021 20:18:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 Aug 2021 20:18:56 GMT
USER memcache
# Fri, 27 Aug 2021 20:18:56 GMT
EXPOSE 11211
# Fri, 27 Aug 2021 20:18:56 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:552d1f2373af9bfe12033568ebbfb0ccbb0de11279f9a415a29207e264d7f4d9`  
		Last Modified: Fri, 27 Aug 2021 17:40:18 GMT  
		Size: 2.7 MB (2711827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ab312377ca26aa6df3e0bb8b11a63d6964544ffd2552b8e7cebb0acbbc3036d`  
		Last Modified: Fri, 27 Aug 2021 20:19:53 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a538168cab1a5c606dfa94dd8b09de5598c9071505476146fa99500011f8e7f5`  
		Last Modified: Fri, 27 Aug 2021 20:19:53 GMT  
		Size: 157.2 KB (157194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae4e52b47025818dc222e8dcd9310ab3f3c757a434fb786d7100cfaef304d4ed`  
		Last Modified: Fri, 27 Aug 2021 20:19:53 GMT  
		Size: 922.5 KB (922539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bedcb7a468e2a54e811d3ab62759e10500ea8b580eb12a600991eb1a3eed136`  
		Last Modified: Fri, 27 Aug 2021 20:19:53 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50b5ad9ab615a8b63e96efab0f2b3b2ff0a60abcb13a2529437f46368a641c6e`  
		Last Modified: Fri, 27 Aug 2021 20:19:53 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-alpine` - linux; 386

```console
$ docker pull memcached@sha256:82a99c470435ce9fd7cebf6565305c9f9a20eb2142839f8a7eaf42fc04b1e64a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3937988 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:503d28ddbe03b1e33458c354e3e0cef3142579c20bdf6e8c1f4b447257a2de01`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 27 Aug 2021 17:38:29 GMT
ADD file:42a7bc5a08b546b47049dd0f89ae4e7a8c86342f87000f39ade3ff52916a6c2e in / 
# Fri, 27 Aug 2021 17:38:30 GMT
CMD ["/bin/sh"]
# Fri, 27 Aug 2021 19:48:52 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Fri, 27 Aug 2021 19:48:54 GMT
RUN apk add --no-cache libsasl
# Fri, 27 Aug 2021 19:48:54 GMT
ENV MEMCACHED_VERSION=1.6.10
# Fri, 27 Aug 2021 19:48:55 GMT
ENV MEMCACHED_SHA1=cb5b9fe77a2a59cc6cc7103a415bc07df9ddc6ec
# Fri, 27 Aug 2021 19:53:36 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Fri, 27 Aug 2021 19:53:36 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 27 Aug 2021 19:53:37 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 27 Aug 2021 19:53:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 Aug 2021 19:53:38 GMT
USER memcache
# Fri, 27 Aug 2021 19:53:38 GMT
EXPOSE 11211
# Fri, 27 Aug 2021 19:53:38 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:b11ae9fc5d8a106cfed3a6f6c75e5b5b5797c566fac4411622b4055df6541286`  
		Last Modified: Fri, 27 Aug 2021 17:39:18 GMT  
		Size: 2.8 MB (2822857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a776c6c02658f2d17623bce57a634d82f2dc8c8bee59f4d90fc786c3e69e31ff`  
		Last Modified: Fri, 27 Aug 2021 19:54:35 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fab8279289e8b7a476ce09017d9bcdb33bccbe04750f2ccba41c0a43f828b16`  
		Last Modified: Fri, 27 Aug 2021 19:54:35 GMT  
		Size: 169.0 KB (169012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24c50e3cfd5d1f42d6dd2505b7b02ca2ed14cb53d2199df2bed319e84146d13b`  
		Last Modified: Fri, 27 Aug 2021 19:54:36 GMT  
		Size: 944.4 KB (944446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3856e8e8dfa799b89d86a7552466e0b451bc8b8b140b56d53056ea942b82b102`  
		Last Modified: Fri, 27 Aug 2021 19:54:35 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bd1d4e4fe24a075a95e91ec623e250fb1071d34af2ec3a777ceecca3d62ea9f`  
		Last Modified: Fri, 27 Aug 2021 19:54:35 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-alpine` - linux; ppc64le

```console
$ docker pull memcached@sha256:5ea0c2672938efeae9c4cf8a45bdb1a06eaacb2f1014ed8fef3d3c6339b3fac5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.0 MB (3954868 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e20a2c1b753cc0bb4b19ca80b7d333dcbb37ce0a77e99c1b96ef27b09b680fa7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 27 Aug 2021 19:39:54 GMT
ADD file:d213c56ffc24a5051e8060fd0fec1a0520367c10d88ab16321c36336b6c66098 in / 
# Fri, 27 Aug 2021 19:39:59 GMT
CMD ["/bin/sh"]
# Sat, 28 Aug 2021 02:52:59 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Sat, 28 Aug 2021 02:53:08 GMT
RUN apk add --no-cache libsasl
# Sat, 28 Aug 2021 02:53:10 GMT
ENV MEMCACHED_VERSION=1.6.10
# Sat, 28 Aug 2021 02:53:12 GMT
ENV MEMCACHED_SHA1=cb5b9fe77a2a59cc6cc7103a415bc07df9ddc6ec
# Sat, 28 Aug 2021 02:56:38 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Sat, 28 Aug 2021 02:56:40 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Sat, 28 Aug 2021 02:56:47 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Sat, 28 Aug 2021 02:56:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 28 Aug 2021 02:56:57 GMT
USER memcache
# Sat, 28 Aug 2021 02:57:02 GMT
EXPOSE 11211
# Sat, 28 Aug 2021 02:57:09 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:63da8ca98f7b4b94381aed56862a60aecf355d9428b9aeb7c61d5bd017100c18`  
		Last Modified: Fri, 27 Aug 2021 19:41:06 GMT  
		Size: 2.8 MB (2812284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a54fbc6ddd30fadabd2cf34600dd72918de6e611345c8202b6cd56a411467659`  
		Last Modified: Sat, 28 Aug 2021 02:58:02 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdd08b1afa1a2e02df391d85b3cfccf552f50b91046d9eafbe19feffb2f58910`  
		Last Modified: Sat, 28 Aug 2021 02:58:02 GMT  
		Size: 179.7 KB (179652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d214dccc5e7f55ecf8e9ec4471487fa0f6ba5ba2e84a3c746ff458410a29c755`  
		Last Modified: Sat, 28 Aug 2021 02:58:02 GMT  
		Size: 961.3 KB (961258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a6ae8b6fa12461573aab65c6be736cd4668463495c569d1113861ff729fb89f`  
		Last Modified: Sat, 28 Aug 2021 02:58:02 GMT  
		Size: 283.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fef62e61ad65fab7f854dd8a0a437b4ed6853b4186a9639a41ac47dae3f7d9e`  
		Last Modified: Sat, 28 Aug 2021 02:58:02 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-alpine` - linux; s390x

```console
$ docker pull memcached@sha256:cebdf9f1ff4ffe7551d4917b4a53e78ac48da41a694a8301fbd92459ebd9f45f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.7 MB (3695912 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:047503017563255821d3a05e00a220624c8698ef1a285eb6a05023ef0c1335e4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 27 Aug 2021 17:41:29 GMT
ADD file:9b40ee281e8797067fb2ae207c406084cb81593090338a8b7cb09ade52168daa in / 
# Fri, 27 Aug 2021 17:41:30 GMT
CMD ["/bin/sh"]
# Fri, 27 Aug 2021 19:13:56 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Fri, 27 Aug 2021 19:13:58 GMT
RUN apk add --no-cache libsasl
# Fri, 27 Aug 2021 19:13:59 GMT
ENV MEMCACHED_VERSION=1.6.10
# Fri, 27 Aug 2021 19:13:59 GMT
ENV MEMCACHED_SHA1=cb5b9fe77a2a59cc6cc7103a415bc07df9ddc6ec
# Fri, 27 Aug 2021 19:22:03 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Fri, 27 Aug 2021 19:22:04 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 27 Aug 2021 19:22:05 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 27 Aug 2021 19:22:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 Aug 2021 19:22:06 GMT
USER memcache
# Fri, 27 Aug 2021 19:22:06 GMT
EXPOSE 11211
# Fri, 27 Aug 2021 19:22:07 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:da14cb6b6dc946dbb2d84386bcaca84e2d46f650767cd11bdb3331ec9d623988`  
		Last Modified: Fri, 27 Aug 2021 17:42:25 GMT  
		Size: 2.6 MB (2603464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5c3123815589d4cfc45a071f344bd0f3ca08ee63a471c2c114af2dece4699a0`  
		Last Modified: Fri, 27 Aug 2021 19:23:06 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d25c400e2d4eb8dee97bc754e9e52585af4304ec8cf3121b619bd5756796fb52`  
		Last Modified: Fri, 27 Aug 2021 19:23:06 GMT  
		Size: 161.5 KB (161520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:611fd541e530a5444852c1a56f01565817097a4b2abec64399dcf4fdd84dfe88`  
		Last Modified: Fri, 27 Aug 2021 19:23:06 GMT  
		Size: 929.3 KB (929257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cb82aed96a5a46fb2399db9bf85a3ff9a7ce3de3468fe74285ad84fd557a1ca`  
		Last Modified: Fri, 27 Aug 2021 19:23:06 GMT  
		Size: 283.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c18159f487fe568305c6aaeb29b07af5f859402bb29566a404f9fccbd86bafbf`  
		Last Modified: Fri, 27 Aug 2021 19:23:06 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:1-alpine3.14`

```console
$ docker pull memcached@sha256:d57531b1d9bfffc9ada8c669fe761da3c7f9a15b9ac27d0f383e318d40f90e0d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `memcached:1-alpine3.14` - linux; amd64

```console
$ docker pull memcached@sha256:67d93d2efc4859c0b2e5a24bc13e759788c1f28d97a4d68b58a3de323e8ccb38
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3904613 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec200929117689b8cbba5a24fe5e892d7e4bfec5b654cef54958801a6ab9e92b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Fri, 27 Aug 2021 20:39:15 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Fri, 27 Aug 2021 20:39:16 GMT
RUN apk add --no-cache libsasl
# Fri, 27 Aug 2021 20:39:16 GMT
ENV MEMCACHED_VERSION=1.6.10
# Fri, 27 Aug 2021 20:39:17 GMT
ENV MEMCACHED_SHA1=cb5b9fe77a2a59cc6cc7103a415bc07df9ddc6ec
# Fri, 27 Aug 2021 20:43:47 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Fri, 27 Aug 2021 20:43:47 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 27 Aug 2021 20:43:49 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 27 Aug 2021 20:43:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 Aug 2021 20:43:50 GMT
USER memcache
# Fri, 27 Aug 2021 20:43:50 GMT
EXPOSE 11211
# Fri, 27 Aug 2021 20:43:50 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:a0d0a0d46f8b52473982a3c466318f479767577551a53ffc9074c9fa7035982e`  
		Last Modified: Fri, 27 Aug 2021 17:20:13 GMT  
		Size: 2.8 MB (2814446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84db6e403c6f8cdc8217536fa7d8bb9bbee66a7a49106104b3ceeace758e887b`  
		Last Modified: Fri, 27 Aug 2021 20:44:26 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7430c0d88cc6cc6389bb62e421f43031b009d21243f7362290bcf11b82e9e967`  
		Last Modified: Fri, 27 Aug 2021 20:44:26 GMT  
		Size: 155.5 KB (155516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3919afa4c767ba881b469a2798f6ad270dc23bbd9174d2994a0208bf508febba`  
		Last Modified: Fri, 27 Aug 2021 20:44:26 GMT  
		Size: 933.0 KB (932979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e81a6f988f7ee7ae5df06403e582d0edb09dcd73e81bacdaa17d1e0da71e13b`  
		Last Modified: Fri, 27 Aug 2021 20:44:26 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d5ed3d833f3ab3255decd4fc642f2368e6791acc470e40c2f3eb7463b7351dc`  
		Last Modified: Fri, 27 Aug 2021 20:44:26 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-alpine3.14` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:8ed70173927cd66ad4e1bac9803ba7114502646685f70abb395ef668a46db5fb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3793233 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c5c3d9ec3f6b46ae9e7305a3958b059ffc7d935b5f2094e78973054a0394060e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 27 Aug 2021 17:39:33 GMT
ADD file:dc8af9c7bfe9f9541e1db38dea01c4201609f3075b31e108f2073ffed8c5e4b9 in / 
# Fri, 27 Aug 2021 17:39:33 GMT
CMD ["/bin/sh"]
# Fri, 27 Aug 2021 20:15:01 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Fri, 27 Aug 2021 20:15:02 GMT
RUN apk add --no-cache libsasl
# Fri, 27 Aug 2021 20:15:02 GMT
ENV MEMCACHED_VERSION=1.6.10
# Fri, 27 Aug 2021 20:15:02 GMT
ENV MEMCACHED_SHA1=cb5b9fe77a2a59cc6cc7103a415bc07df9ddc6ec
# Fri, 27 Aug 2021 20:18:55 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Fri, 27 Aug 2021 20:18:55 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 27 Aug 2021 20:18:56 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 27 Aug 2021 20:18:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 Aug 2021 20:18:56 GMT
USER memcache
# Fri, 27 Aug 2021 20:18:56 GMT
EXPOSE 11211
# Fri, 27 Aug 2021 20:18:56 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:552d1f2373af9bfe12033568ebbfb0ccbb0de11279f9a415a29207e264d7f4d9`  
		Last Modified: Fri, 27 Aug 2021 17:40:18 GMT  
		Size: 2.7 MB (2711827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ab312377ca26aa6df3e0bb8b11a63d6964544ffd2552b8e7cebb0acbbc3036d`  
		Last Modified: Fri, 27 Aug 2021 20:19:53 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a538168cab1a5c606dfa94dd8b09de5598c9071505476146fa99500011f8e7f5`  
		Last Modified: Fri, 27 Aug 2021 20:19:53 GMT  
		Size: 157.2 KB (157194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae4e52b47025818dc222e8dcd9310ab3f3c757a434fb786d7100cfaef304d4ed`  
		Last Modified: Fri, 27 Aug 2021 20:19:53 GMT  
		Size: 922.5 KB (922539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bedcb7a468e2a54e811d3ab62759e10500ea8b580eb12a600991eb1a3eed136`  
		Last Modified: Fri, 27 Aug 2021 20:19:53 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50b5ad9ab615a8b63e96efab0f2b3b2ff0a60abcb13a2529437f46368a641c6e`  
		Last Modified: Fri, 27 Aug 2021 20:19:53 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-alpine3.14` - linux; 386

```console
$ docker pull memcached@sha256:82a99c470435ce9fd7cebf6565305c9f9a20eb2142839f8a7eaf42fc04b1e64a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3937988 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:503d28ddbe03b1e33458c354e3e0cef3142579c20bdf6e8c1f4b447257a2de01`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 27 Aug 2021 17:38:29 GMT
ADD file:42a7bc5a08b546b47049dd0f89ae4e7a8c86342f87000f39ade3ff52916a6c2e in / 
# Fri, 27 Aug 2021 17:38:30 GMT
CMD ["/bin/sh"]
# Fri, 27 Aug 2021 19:48:52 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Fri, 27 Aug 2021 19:48:54 GMT
RUN apk add --no-cache libsasl
# Fri, 27 Aug 2021 19:48:54 GMT
ENV MEMCACHED_VERSION=1.6.10
# Fri, 27 Aug 2021 19:48:55 GMT
ENV MEMCACHED_SHA1=cb5b9fe77a2a59cc6cc7103a415bc07df9ddc6ec
# Fri, 27 Aug 2021 19:53:36 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Fri, 27 Aug 2021 19:53:36 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 27 Aug 2021 19:53:37 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 27 Aug 2021 19:53:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 Aug 2021 19:53:38 GMT
USER memcache
# Fri, 27 Aug 2021 19:53:38 GMT
EXPOSE 11211
# Fri, 27 Aug 2021 19:53:38 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:b11ae9fc5d8a106cfed3a6f6c75e5b5b5797c566fac4411622b4055df6541286`  
		Last Modified: Fri, 27 Aug 2021 17:39:18 GMT  
		Size: 2.8 MB (2822857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a776c6c02658f2d17623bce57a634d82f2dc8c8bee59f4d90fc786c3e69e31ff`  
		Last Modified: Fri, 27 Aug 2021 19:54:35 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fab8279289e8b7a476ce09017d9bcdb33bccbe04750f2ccba41c0a43f828b16`  
		Last Modified: Fri, 27 Aug 2021 19:54:35 GMT  
		Size: 169.0 KB (169012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24c50e3cfd5d1f42d6dd2505b7b02ca2ed14cb53d2199df2bed319e84146d13b`  
		Last Modified: Fri, 27 Aug 2021 19:54:36 GMT  
		Size: 944.4 KB (944446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3856e8e8dfa799b89d86a7552466e0b451bc8b8b140b56d53056ea942b82b102`  
		Last Modified: Fri, 27 Aug 2021 19:54:35 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bd1d4e4fe24a075a95e91ec623e250fb1071d34af2ec3a777ceecca3d62ea9f`  
		Last Modified: Fri, 27 Aug 2021 19:54:35 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-alpine3.14` - linux; ppc64le

```console
$ docker pull memcached@sha256:5ea0c2672938efeae9c4cf8a45bdb1a06eaacb2f1014ed8fef3d3c6339b3fac5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.0 MB (3954868 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e20a2c1b753cc0bb4b19ca80b7d333dcbb37ce0a77e99c1b96ef27b09b680fa7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 27 Aug 2021 19:39:54 GMT
ADD file:d213c56ffc24a5051e8060fd0fec1a0520367c10d88ab16321c36336b6c66098 in / 
# Fri, 27 Aug 2021 19:39:59 GMT
CMD ["/bin/sh"]
# Sat, 28 Aug 2021 02:52:59 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Sat, 28 Aug 2021 02:53:08 GMT
RUN apk add --no-cache libsasl
# Sat, 28 Aug 2021 02:53:10 GMT
ENV MEMCACHED_VERSION=1.6.10
# Sat, 28 Aug 2021 02:53:12 GMT
ENV MEMCACHED_SHA1=cb5b9fe77a2a59cc6cc7103a415bc07df9ddc6ec
# Sat, 28 Aug 2021 02:56:38 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Sat, 28 Aug 2021 02:56:40 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Sat, 28 Aug 2021 02:56:47 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Sat, 28 Aug 2021 02:56:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 28 Aug 2021 02:56:57 GMT
USER memcache
# Sat, 28 Aug 2021 02:57:02 GMT
EXPOSE 11211
# Sat, 28 Aug 2021 02:57:09 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:63da8ca98f7b4b94381aed56862a60aecf355d9428b9aeb7c61d5bd017100c18`  
		Last Modified: Fri, 27 Aug 2021 19:41:06 GMT  
		Size: 2.8 MB (2812284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a54fbc6ddd30fadabd2cf34600dd72918de6e611345c8202b6cd56a411467659`  
		Last Modified: Sat, 28 Aug 2021 02:58:02 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdd08b1afa1a2e02df391d85b3cfccf552f50b91046d9eafbe19feffb2f58910`  
		Last Modified: Sat, 28 Aug 2021 02:58:02 GMT  
		Size: 179.7 KB (179652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d214dccc5e7f55ecf8e9ec4471487fa0f6ba5ba2e84a3c746ff458410a29c755`  
		Last Modified: Sat, 28 Aug 2021 02:58:02 GMT  
		Size: 961.3 KB (961258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a6ae8b6fa12461573aab65c6be736cd4668463495c569d1113861ff729fb89f`  
		Last Modified: Sat, 28 Aug 2021 02:58:02 GMT  
		Size: 283.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fef62e61ad65fab7f854dd8a0a437b4ed6853b4186a9639a41ac47dae3f7d9e`  
		Last Modified: Sat, 28 Aug 2021 02:58:02 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-alpine3.14` - linux; s390x

```console
$ docker pull memcached@sha256:cebdf9f1ff4ffe7551d4917b4a53e78ac48da41a694a8301fbd92459ebd9f45f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.7 MB (3695912 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:047503017563255821d3a05e00a220624c8698ef1a285eb6a05023ef0c1335e4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 27 Aug 2021 17:41:29 GMT
ADD file:9b40ee281e8797067fb2ae207c406084cb81593090338a8b7cb09ade52168daa in / 
# Fri, 27 Aug 2021 17:41:30 GMT
CMD ["/bin/sh"]
# Fri, 27 Aug 2021 19:13:56 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Fri, 27 Aug 2021 19:13:58 GMT
RUN apk add --no-cache libsasl
# Fri, 27 Aug 2021 19:13:59 GMT
ENV MEMCACHED_VERSION=1.6.10
# Fri, 27 Aug 2021 19:13:59 GMT
ENV MEMCACHED_SHA1=cb5b9fe77a2a59cc6cc7103a415bc07df9ddc6ec
# Fri, 27 Aug 2021 19:22:03 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Fri, 27 Aug 2021 19:22:04 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 27 Aug 2021 19:22:05 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 27 Aug 2021 19:22:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 Aug 2021 19:22:06 GMT
USER memcache
# Fri, 27 Aug 2021 19:22:06 GMT
EXPOSE 11211
# Fri, 27 Aug 2021 19:22:07 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:da14cb6b6dc946dbb2d84386bcaca84e2d46f650767cd11bdb3331ec9d623988`  
		Last Modified: Fri, 27 Aug 2021 17:42:25 GMT  
		Size: 2.6 MB (2603464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5c3123815589d4cfc45a071f344bd0f3ca08ee63a471c2c114af2dece4699a0`  
		Last Modified: Fri, 27 Aug 2021 19:23:06 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d25c400e2d4eb8dee97bc754e9e52585af4304ec8cf3121b619bd5756796fb52`  
		Last Modified: Fri, 27 Aug 2021 19:23:06 GMT  
		Size: 161.5 KB (161520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:611fd541e530a5444852c1a56f01565817097a4b2abec64399dcf4fdd84dfe88`  
		Last Modified: Fri, 27 Aug 2021 19:23:06 GMT  
		Size: 929.3 KB (929257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cb82aed96a5a46fb2399db9bf85a3ff9a7ce3de3468fe74285ad84fd557a1ca`  
		Last Modified: Fri, 27 Aug 2021 19:23:06 GMT  
		Size: 283.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c18159f487fe568305c6aaeb29b07af5f859402bb29566a404f9fccbd86bafbf`  
		Last Modified: Fri, 27 Aug 2021 19:23:06 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:1-buster`

```console
$ docker pull memcached@sha256:0507080446e022bbcb398fef743f5479d61569f2992beccd200033e037968511
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

### `memcached:1-buster` - linux; amd64

```console
$ docker pull memcached@sha256:b93ad58a06f215580205490133ce2165fa69f1930b964e890981f629df497e84
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.6 MB (30631755 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:444d9869f3507356b3fb6ffb7ed74ffc3be04be873a6876423c24d17acbf1128`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 03 Sep 2021 01:21:46 GMT
ADD file:4ff85d9f6aa246746912db62dea02eb71750474bb29611e770516a1fcd217add in / 
# Fri, 03 Sep 2021 01:21:46 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 07:33:54 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Fri, 03 Sep 2021 07:34:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 07:34:01 GMT
ENV MEMCACHED_VERSION=1.6.10
# Fri, 03 Sep 2021 07:34:01 GMT
ENV MEMCACHED_SHA1=cb5b9fe77a2a59cc6cc7103a415bc07df9ddc6ec
# Fri, 03 Sep 2021 07:38:24 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Fri, 03 Sep 2021 07:38:24 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 03 Sep 2021 07:38:25 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 03 Sep 2021 07:38:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 03 Sep 2021 07:38:25 GMT
USER memcache
# Fri, 03 Sep 2021 07:38:26 GMT
EXPOSE 11211
# Fri, 03 Sep 2021 07:38:26 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:a330b6cecb98cd2425fd25fce36669073f593b3176b4ee14731e48c05d678cdd`  
		Last Modified: Fri, 03 Sep 2021 01:28:19 GMT  
		Size: 27.1 MB (27145844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7dcde8d481fe08e2bab1fc8a1dc0e30c1d8cc9647d2867a6bc06942de810d56`  
		Last Modified: Fri, 03 Sep 2021 07:38:54 GMT  
		Size: 5.0 KB (4981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c3e0b65008f095303aa1ff733845d2eed7b3836fad196bc16533b3420711745`  
		Last Modified: Fri, 03 Sep 2021 07:38:54 GMT  
		Size: 2.2 MB (2197580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ad3eb30b171e7b0c33373bdeb39dfc36b63b8ec501af75bae3d4a964872f042`  
		Last Modified: Fri, 03 Sep 2021 07:38:54 GMT  
		Size: 1.3 MB (1282944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e6e03de9a5467b70b4d10bf021740a05eea1aeebfd87864b4a9289df9cb64c0`  
		Last Modified: Fri, 03 Sep 2021 07:38:54 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe0025a339764c7acc0034c701ca2b443e0b1803745c41094ea54289f754a81c`  
		Last Modified: Fri, 03 Sep 2021 07:38:54 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-buster` - linux; arm variant v5

```console
$ docker pull memcached@sha256:5e1d0b6ce4b1b257e47c484709733908552416681c8f054bc97735e5ec114fa2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.0 MB (28036699 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd9fb75ae310df2e536d3a10e6dd9222317f89456fe6082c139b112849e5081b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 03 Sep 2021 00:51:26 GMT
ADD file:350748a564076da397b991745cd42e0688d15c72b9fd5c81f8ea0bb8938a2b3d in / 
# Fri, 03 Sep 2021 00:51:27 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 02:24:47 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Fri, 03 Sep 2021 02:24:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 02:24:58 GMT
ENV MEMCACHED_VERSION=1.6.10
# Fri, 03 Sep 2021 02:24:59 GMT
ENV MEMCACHED_SHA1=cb5b9fe77a2a59cc6cc7103a415bc07df9ddc6ec
# Fri, 03 Sep 2021 02:29:11 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Fri, 03 Sep 2021 02:29:12 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 03 Sep 2021 02:29:13 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 03 Sep 2021 02:29:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 03 Sep 2021 02:29:14 GMT
USER memcache
# Fri, 03 Sep 2021 02:29:14 GMT
EXPOSE 11211
# Fri, 03 Sep 2021 02:29:15 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:b019db4b5197128481d48d92ecacd6bb356c027a3d08393f6567a6fa183ba769`  
		Last Modified: Fri, 03 Sep 2021 01:07:12 GMT  
		Size: 24.9 MB (24879114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4faeba39e66674ac57454c2edb8018a9a29475db4893acb59bf00e84e5c4e88a`  
		Last Modified: Fri, 03 Sep 2021 02:30:10 GMT  
		Size: 4.9 KB (4895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b39e5da0381154e8db96921f6038b79a61f458bf76f9fdaae0d3f44b2d81f184`  
		Last Modified: Fri, 03 Sep 2021 02:30:11 GMT  
		Size: 1.9 MB (1897972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb47be4e43a9bfad0082a507b5885f22b4104821defe786af5237a6b48211a71`  
		Last Modified: Fri, 03 Sep 2021 02:30:11 GMT  
		Size: 1.3 MB (1254312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee01c0ace3ff5a5a86664234d47a50480b12f50f1390f5b78ab2b76a73e3346f`  
		Last Modified: Fri, 03 Sep 2021 02:30:10 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:240af99f2a1c8953e4436d48b387f4aa33defc9e83416c71f2d67d05c2a8cb48`  
		Last Modified: Fri, 03 Sep 2021 02:30:10 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-buster` - linux; arm variant v7

```console
$ docker pull memcached@sha256:ee3f4a07ff534651238a464f5b0a3b582facdc9784f9e0f9a5bcd0128762da4f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.8 MB (25788867 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6222a822647e49fef3f296a084e4504bd705efe8e0649bc91541e03b8a5d7b8a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 03 Sep 2021 01:00:40 GMT
ADD file:4754bbccf4c59f77dd54f3888871f0635a2f9655cda53f50e63237f1580286e0 in / 
# Fri, 03 Sep 2021 01:00:41 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 06:44:19 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Fri, 03 Sep 2021 06:44:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 06:44:29 GMT
ENV MEMCACHED_VERSION=1.6.10
# Fri, 03 Sep 2021 06:44:30 GMT
ENV MEMCACHED_SHA1=cb5b9fe77a2a59cc6cc7103a415bc07df9ddc6ec
# Fri, 03 Sep 2021 06:48:21 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Fri, 03 Sep 2021 06:48:22 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 03 Sep 2021 06:48:23 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 03 Sep 2021 06:48:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 03 Sep 2021 06:48:24 GMT
USER memcache
# Fri, 03 Sep 2021 06:48:25 GMT
EXPOSE 11211
# Fri, 03 Sep 2021 06:48:25 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:2215ad7863d95c38f1f794f1d5b4d6c5ca4ca7e921e4bb7218b803f7ed270675`  
		Last Modified: Fri, 03 Sep 2021 01:16:23 GMT  
		Size: 22.7 MB (22746151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d554d32fa680ffcf04f8b509fa6a16e796fadc0ecf8db8c48bcc2a911f9f4591`  
		Last Modified: Fri, 03 Sep 2021 07:00:56 GMT  
		Size: 4.9 KB (4895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a550041e12d651682f2b70b45620898d8cebd97f4b4b3469aaeac8d452a76ef`  
		Last Modified: Fri, 03 Sep 2021 07:00:56 GMT  
		Size: 1.8 MB (1812490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ae1581582d0b08a4635fe57247a454da856fea52ec988126ee4f2f1781b7acd`  
		Last Modified: Fri, 03 Sep 2021 07:00:56 GMT  
		Size: 1.2 MB (1224925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:678c3e64de445bdc9a420655f01c8abab5f2e7ef4f41d441e6d2310ea2c36de5`  
		Last Modified: Fri, 03 Sep 2021 07:00:55 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a21b13a7b8549e46debb4d9b1117211df9edcc02f822ec99d1fe1b4278f1e56`  
		Last Modified: Fri, 03 Sep 2021 07:00:55 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-buster` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:57e906b2282c3e67137cc8c2ab5148c8e748256b2e3934c5b7ecd77a6a186de5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.3 MB (29250783 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:932f1c94fc6e8e017820dcb97fe4b624efacba7409cb99c99a369c649b03829d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 03 Sep 2021 00:40:58 GMT
ADD file:4a1d7f2d989aee6bd83da076b6e9dd3da2da97cf5654bd37568e9baec30ac4b1 in / 
# Fri, 03 Sep 2021 00:40:58 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 02:46:23 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Fri, 03 Sep 2021 02:46:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 02:46:27 GMT
ENV MEMCACHED_VERSION=1.6.10
# Fri, 03 Sep 2021 02:46:28 GMT
ENV MEMCACHED_SHA1=cb5b9fe77a2a59cc6cc7103a415bc07df9ddc6ec
# Fri, 03 Sep 2021 02:50:03 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Fri, 03 Sep 2021 02:50:03 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 03 Sep 2021 02:50:04 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 03 Sep 2021 02:50:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 03 Sep 2021 02:50:04 GMT
USER memcache
# Fri, 03 Sep 2021 02:50:05 GMT
EXPOSE 11211
# Fri, 03 Sep 2021 02:50:05 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:d10c227306ce3db344a8399cbc02bbf0dcb36519318efbde3c6027c00be8b40e`  
		Last Modified: Fri, 03 Sep 2021 00:49:47 GMT  
		Size: 25.9 MB (25914860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee708d85ae4c6929688ee243da330a395c81a5da3913f7aaaeea88283b5752b1`  
		Last Modified: Fri, 03 Sep 2021 02:51:01 GMT  
		Size: 5.0 KB (5024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41eee23f132aa5ef6810f141bd4852d174eb68bd5e9f8fc4e278e2fc55f7cea8`  
		Last Modified: Fri, 03 Sep 2021 02:51:02 GMT  
		Size: 2.1 MB (2075717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d9a7819a72ed1b598aabafd5ac9be7be62ac6b085cc30dbda97ef193641fc05`  
		Last Modified: Fri, 03 Sep 2021 02:51:01 GMT  
		Size: 1.3 MB (1254776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ae146d1bf5917e1fb0f4aa46a655feefc0ec5e00ef4e775beed00fa6a1d0aa1`  
		Last Modified: Fri, 03 Sep 2021 02:51:01 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3cae1f92b0ec75c4c83b4b5a4ce47b455952d638c215f1588a20af7261fba5b`  
		Last Modified: Fri, 03 Sep 2021 02:51:01 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-buster` - linux; 386

```console
$ docker pull memcached@sha256:221d230cb426e233ce34c9669663db5628d85a6ffe1d98292cfb54d66a7e1f8a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.3 MB (31292631 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7283abe72dd41573bd7262a0ba163f6ef7ddf757bc5178c95eea585f8335e784`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 03 Sep 2021 00:40:24 GMT
ADD file:6bf4b6f4aa28306610ef10c68f422a7210ff2fbd5345cec07bc5f76d54a4c8bc in / 
# Fri, 03 Sep 2021 00:40:24 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 06:44:15 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Fri, 03 Sep 2021 06:44:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 06:44:21 GMT
ENV MEMCACHED_VERSION=1.6.10
# Fri, 03 Sep 2021 06:44:21 GMT
ENV MEMCACHED_SHA1=cb5b9fe77a2a59cc6cc7103a415bc07df9ddc6ec
# Fri, 03 Sep 2021 06:48:23 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Fri, 03 Sep 2021 06:48:24 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 03 Sep 2021 06:48:25 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 03 Sep 2021 06:48:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 03 Sep 2021 06:48:26 GMT
USER memcache
# Fri, 03 Sep 2021 06:48:26 GMT
EXPOSE 11211
# Fri, 03 Sep 2021 06:48:26 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:7e87f600658a0c0d3bd8b82b9c645b5ec2763492ec627c1c1c1183c2ad3c45d5`  
		Last Modified: Fri, 03 Sep 2021 00:49:06 GMT  
		Size: 27.8 MB (27797513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9454a8c8c54135f6e7f591277550407671a2a183d0ea7a1b04e0b7bf1ecfeb39`  
		Last Modified: Fri, 03 Sep 2021 06:49:32 GMT  
		Size: 4.9 KB (4895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4900dba329569a63986180bc83b94449c1dffc3a804c2910a2a3f288509964d3`  
		Last Modified: Fri, 03 Sep 2021 06:49:32 GMT  
		Size: 2.2 MB (2209620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb8624563e6585b031c874cc180ee08148f5773238b0bc1571feb1b64b198ee5`  
		Last Modified: Fri, 03 Sep 2021 06:49:32 GMT  
		Size: 1.3 MB (1280199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86f15c6c59e3205f04fba85035da98cd62d3f67bca6baa035b56db7f4f5dfb5c`  
		Last Modified: Fri, 03 Sep 2021 06:49:32 GMT  
		Size: 283.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f1b51c6ca8d549a8b18622d1c15504b94257295420bc332544f8d9026fff6f3`  
		Last Modified: Fri, 03 Sep 2021 06:49:32 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-buster` - linux; mips64le

```console
$ docker pull memcached@sha256:33ce4398cd07967870c76b95ec5314cbe8280d564309b25d0640e8dd94cb7198
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.9 MB (28866865 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cc3e459293995ad1867b805e319ebb5b3942502abbad00cf3f9b3a4ccc26c740`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 28 Sep 2021 02:11:41 GMT
ADD file:df525c65bc60141f19ab937525d724c6d29cac53beb30f92d79ea4b2edf5a13e in / 
# Tue, 28 Sep 2021 02:11:41 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 02:51:00 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 28 Sep 2021 02:51:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:51:13 GMT
ENV MEMCACHED_VERSION=1.6.10
# Tue, 28 Sep 2021 02:51:13 GMT
ENV MEMCACHED_SHA1=cb5b9fe77a2a59cc6cc7103a415bc07df9ddc6ec
# Tue, 28 Sep 2021 02:56:56 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 28 Sep 2021 02:56:56 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 28 Sep 2021 02:56:58 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 28 Sep 2021 02:56:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 28 Sep 2021 02:56:59 GMT
USER memcache
# Tue, 28 Sep 2021 02:56:59 GMT
EXPOSE 11211
# Tue, 28 Sep 2021 02:56:59 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:f1b3d9dde862ddf88a05cec47ce54e641c4057c7bfb377e2a065c72a42a76321`  
		Last Modified: Tue, 28 Sep 2021 02:22:07 GMT  
		Size: 25.8 MB (25813001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e684588e988c227c0fedbcfeb8361e35b75eaa06e38cf8207979b491712d3dc`  
		Last Modified: Tue, 28 Sep 2021 02:57:18 GMT  
		Size: 5.0 KB (4981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35a3bc6181fe53d4bf46e98ebace046f2014668d601c2c3975c3dc6fc655acbc`  
		Last Modified: Tue, 28 Sep 2021 02:57:19 GMT  
		Size: 1.8 MB (1777273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f49b3d8a270ebba87297e2461fe81567f28a880e22d7ef977a60930ad82d6aa6`  
		Last Modified: Tue, 28 Sep 2021 02:57:19 GMT  
		Size: 1.3 MB (1271204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:119de6bb61edbff9dc8919b6bbb0f35c144a065c899d3fe20127480e2985c0d8`  
		Last Modified: Tue, 28 Sep 2021 02:57:18 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ecffae4c1838eb68ee866feaae4a6357c6198f1e86b5a1719bd7646795396d6`  
		Last Modified: Tue, 28 Sep 2021 02:57:18 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-buster` - linux; ppc64le

```console
$ docker pull memcached@sha256:49728dba09507cb74bbfae419b5b8051106768fd3b53aa7964da2b4a7cf0d44f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.2 MB (34190787 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4563ba0117902a70591f2170ab90e34de0431ae24402ee05aa741d4eafbd036f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 03 Sep 2021 01:24:33 GMT
ADD file:6c1662ddb92232ae8969a86a18dacab97b3b5792a1ecda49e6ac741a1a5c878c in / 
# Fri, 03 Sep 2021 01:24:41 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 08:06:59 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Fri, 03 Sep 2021 08:07:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 08:07:23 GMT
ENV MEMCACHED_VERSION=1.6.10
# Fri, 03 Sep 2021 08:07:26 GMT
ENV MEMCACHED_SHA1=cb5b9fe77a2a59cc6cc7103a415bc07df9ddc6ec
# Fri, 03 Sep 2021 08:13:31 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Fri, 03 Sep 2021 08:13:32 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 03 Sep 2021 08:13:43 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 03 Sep 2021 08:13:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 03 Sep 2021 08:13:57 GMT
USER memcache
# Fri, 03 Sep 2021 08:14:01 GMT
EXPOSE 11211
# Fri, 03 Sep 2021 08:14:05 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:8258146296247df1f308a336d4abf286afae14e3375edefb87a091e80745e29f`  
		Last Modified: Fri, 03 Sep 2021 01:39:45 GMT  
		Size: 30.6 MB (30553675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2f96132a11c70c50168ade17294cf7e8c919db231f87a28818170d9917a3268`  
		Last Modified: Fri, 03 Sep 2021 08:14:54 GMT  
		Size: 5.0 KB (4988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:973046a9e11e4bf003ce0e9688dc396e6e0ded760e9914a57132e130fa64289a`  
		Last Modified: Fri, 03 Sep 2021 08:14:55 GMT  
		Size: 2.3 MB (2323873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e5495ff67177662caa9f0459d68cb0641f32eddb666f4238634e357e58bdad1`  
		Last Modified: Fri, 03 Sep 2021 08:14:55 GMT  
		Size: 1.3 MB (1307845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b406b4303f1d8fe163586ca2e7abe3639c752a524f2c44e46677c01e36f937c`  
		Last Modified: Fri, 03 Sep 2021 08:14:54 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ff817a29aac3d654f6e919cbea3ea8125cce972e357c595217ec95807e07c3d`  
		Last Modified: Fri, 03 Sep 2021 08:14:54 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-buster` - linux; s390x

```console
$ docker pull memcached@sha256:53459c6f3d42b7b718e1ccbb3090ff35e649d8d005fa1917cee1ee1fbfea608a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.9 MB (28925755 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8831bffed7f4d435dd3c714d24529fea34f84468cbc5abec57feeb4728059de`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 28 Sep 2021 01:43:29 GMT
ADD file:118e7a596407435b5e2ff0aae6bb9bff3b66000c91ca37bfe1eeb98c23d99d49 in / 
# Tue, 28 Sep 2021 01:43:30 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 02:31:35 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 28 Sep 2021 02:31:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:31:39 GMT
ENV MEMCACHED_VERSION=1.6.10
# Tue, 28 Sep 2021 02:31:39 GMT
ENV MEMCACHED_SHA1=cb5b9fe77a2a59cc6cc7103a415bc07df9ddc6ec
# Tue, 28 Sep 2021 02:34:53 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 28 Sep 2021 02:34:54 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 28 Sep 2021 02:34:54 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 28 Sep 2021 02:34:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 28 Sep 2021 02:34:54 GMT
USER memcache
# Tue, 28 Sep 2021 02:34:54 GMT
EXPOSE 11211
# Tue, 28 Sep 2021 02:34:55 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:7cfe208f95c1b63305981b069795676fa149e7115b9044c241ee45ef4aaf0bb3`  
		Last Modified: Tue, 28 Sep 2021 01:49:36 GMT  
		Size: 25.8 MB (25760871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff755a70833a769c5a32cb251e86ac9aa6ae1dce7f547dc1bef874a22855b63d`  
		Last Modified: Tue, 28 Sep 2021 02:35:52 GMT  
		Size: 5.0 KB (5022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d08a7a4b96e17b9ef0eb0b8dd97ad0dc3d75227841b6374b7071e7989d9fed3c`  
		Last Modified: Tue, 28 Sep 2021 02:35:52 GMT  
		Size: 1.9 MB (1887230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4b9662cd31c943100c81ad7c951195bf462ad510ed53de50144b8617d870a84`  
		Last Modified: Tue, 28 Sep 2021 02:35:52 GMT  
		Size: 1.3 MB (1272226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fc50167475bec35471f2d4f925c2d427f3757ac01cd3f8f82cc5685771c2744`  
		Last Modified: Tue, 28 Sep 2021 02:35:52 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c69d6c53bee775bfd205e1d0426724cebf2eddd3034e82681311e18028641c25`  
		Last Modified: Tue, 28 Sep 2021 02:35:52 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:1.6`

```console
$ docker pull memcached@sha256:0507080446e022bbcb398fef743f5479d61569f2992beccd200033e037968511
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
$ docker pull memcached@sha256:b93ad58a06f215580205490133ce2165fa69f1930b964e890981f629df497e84
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.6 MB (30631755 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:444d9869f3507356b3fb6ffb7ed74ffc3be04be873a6876423c24d17acbf1128`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 03 Sep 2021 01:21:46 GMT
ADD file:4ff85d9f6aa246746912db62dea02eb71750474bb29611e770516a1fcd217add in / 
# Fri, 03 Sep 2021 01:21:46 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 07:33:54 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Fri, 03 Sep 2021 07:34:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 07:34:01 GMT
ENV MEMCACHED_VERSION=1.6.10
# Fri, 03 Sep 2021 07:34:01 GMT
ENV MEMCACHED_SHA1=cb5b9fe77a2a59cc6cc7103a415bc07df9ddc6ec
# Fri, 03 Sep 2021 07:38:24 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Fri, 03 Sep 2021 07:38:24 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 03 Sep 2021 07:38:25 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 03 Sep 2021 07:38:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 03 Sep 2021 07:38:25 GMT
USER memcache
# Fri, 03 Sep 2021 07:38:26 GMT
EXPOSE 11211
# Fri, 03 Sep 2021 07:38:26 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:a330b6cecb98cd2425fd25fce36669073f593b3176b4ee14731e48c05d678cdd`  
		Last Modified: Fri, 03 Sep 2021 01:28:19 GMT  
		Size: 27.1 MB (27145844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7dcde8d481fe08e2bab1fc8a1dc0e30c1d8cc9647d2867a6bc06942de810d56`  
		Last Modified: Fri, 03 Sep 2021 07:38:54 GMT  
		Size: 5.0 KB (4981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c3e0b65008f095303aa1ff733845d2eed7b3836fad196bc16533b3420711745`  
		Last Modified: Fri, 03 Sep 2021 07:38:54 GMT  
		Size: 2.2 MB (2197580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ad3eb30b171e7b0c33373bdeb39dfc36b63b8ec501af75bae3d4a964872f042`  
		Last Modified: Fri, 03 Sep 2021 07:38:54 GMT  
		Size: 1.3 MB (1282944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e6e03de9a5467b70b4d10bf021740a05eea1aeebfd87864b4a9289df9cb64c0`  
		Last Modified: Fri, 03 Sep 2021 07:38:54 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe0025a339764c7acc0034c701ca2b443e0b1803745c41094ea54289f754a81c`  
		Last Modified: Fri, 03 Sep 2021 07:38:54 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6` - linux; arm variant v5

```console
$ docker pull memcached@sha256:5e1d0b6ce4b1b257e47c484709733908552416681c8f054bc97735e5ec114fa2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.0 MB (28036699 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd9fb75ae310df2e536d3a10e6dd9222317f89456fe6082c139b112849e5081b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 03 Sep 2021 00:51:26 GMT
ADD file:350748a564076da397b991745cd42e0688d15c72b9fd5c81f8ea0bb8938a2b3d in / 
# Fri, 03 Sep 2021 00:51:27 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 02:24:47 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Fri, 03 Sep 2021 02:24:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 02:24:58 GMT
ENV MEMCACHED_VERSION=1.6.10
# Fri, 03 Sep 2021 02:24:59 GMT
ENV MEMCACHED_SHA1=cb5b9fe77a2a59cc6cc7103a415bc07df9ddc6ec
# Fri, 03 Sep 2021 02:29:11 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Fri, 03 Sep 2021 02:29:12 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 03 Sep 2021 02:29:13 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 03 Sep 2021 02:29:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 03 Sep 2021 02:29:14 GMT
USER memcache
# Fri, 03 Sep 2021 02:29:14 GMT
EXPOSE 11211
# Fri, 03 Sep 2021 02:29:15 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:b019db4b5197128481d48d92ecacd6bb356c027a3d08393f6567a6fa183ba769`  
		Last Modified: Fri, 03 Sep 2021 01:07:12 GMT  
		Size: 24.9 MB (24879114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4faeba39e66674ac57454c2edb8018a9a29475db4893acb59bf00e84e5c4e88a`  
		Last Modified: Fri, 03 Sep 2021 02:30:10 GMT  
		Size: 4.9 KB (4895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b39e5da0381154e8db96921f6038b79a61f458bf76f9fdaae0d3f44b2d81f184`  
		Last Modified: Fri, 03 Sep 2021 02:30:11 GMT  
		Size: 1.9 MB (1897972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb47be4e43a9bfad0082a507b5885f22b4104821defe786af5237a6b48211a71`  
		Last Modified: Fri, 03 Sep 2021 02:30:11 GMT  
		Size: 1.3 MB (1254312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee01c0ace3ff5a5a86664234d47a50480b12f50f1390f5b78ab2b76a73e3346f`  
		Last Modified: Fri, 03 Sep 2021 02:30:10 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:240af99f2a1c8953e4436d48b387f4aa33defc9e83416c71f2d67d05c2a8cb48`  
		Last Modified: Fri, 03 Sep 2021 02:30:10 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6` - linux; arm variant v7

```console
$ docker pull memcached@sha256:ee3f4a07ff534651238a464f5b0a3b582facdc9784f9e0f9a5bcd0128762da4f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.8 MB (25788867 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6222a822647e49fef3f296a084e4504bd705efe8e0649bc91541e03b8a5d7b8a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 03 Sep 2021 01:00:40 GMT
ADD file:4754bbccf4c59f77dd54f3888871f0635a2f9655cda53f50e63237f1580286e0 in / 
# Fri, 03 Sep 2021 01:00:41 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 06:44:19 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Fri, 03 Sep 2021 06:44:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 06:44:29 GMT
ENV MEMCACHED_VERSION=1.6.10
# Fri, 03 Sep 2021 06:44:30 GMT
ENV MEMCACHED_SHA1=cb5b9fe77a2a59cc6cc7103a415bc07df9ddc6ec
# Fri, 03 Sep 2021 06:48:21 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Fri, 03 Sep 2021 06:48:22 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 03 Sep 2021 06:48:23 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 03 Sep 2021 06:48:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 03 Sep 2021 06:48:24 GMT
USER memcache
# Fri, 03 Sep 2021 06:48:25 GMT
EXPOSE 11211
# Fri, 03 Sep 2021 06:48:25 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:2215ad7863d95c38f1f794f1d5b4d6c5ca4ca7e921e4bb7218b803f7ed270675`  
		Last Modified: Fri, 03 Sep 2021 01:16:23 GMT  
		Size: 22.7 MB (22746151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d554d32fa680ffcf04f8b509fa6a16e796fadc0ecf8db8c48bcc2a911f9f4591`  
		Last Modified: Fri, 03 Sep 2021 07:00:56 GMT  
		Size: 4.9 KB (4895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a550041e12d651682f2b70b45620898d8cebd97f4b4b3469aaeac8d452a76ef`  
		Last Modified: Fri, 03 Sep 2021 07:00:56 GMT  
		Size: 1.8 MB (1812490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ae1581582d0b08a4635fe57247a454da856fea52ec988126ee4f2f1781b7acd`  
		Last Modified: Fri, 03 Sep 2021 07:00:56 GMT  
		Size: 1.2 MB (1224925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:678c3e64de445bdc9a420655f01c8abab5f2e7ef4f41d441e6d2310ea2c36de5`  
		Last Modified: Fri, 03 Sep 2021 07:00:55 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a21b13a7b8549e46debb4d9b1117211df9edcc02f822ec99d1fe1b4278f1e56`  
		Last Modified: Fri, 03 Sep 2021 07:00:55 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:57e906b2282c3e67137cc8c2ab5148c8e748256b2e3934c5b7ecd77a6a186de5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.3 MB (29250783 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:932f1c94fc6e8e017820dcb97fe4b624efacba7409cb99c99a369c649b03829d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 03 Sep 2021 00:40:58 GMT
ADD file:4a1d7f2d989aee6bd83da076b6e9dd3da2da97cf5654bd37568e9baec30ac4b1 in / 
# Fri, 03 Sep 2021 00:40:58 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 02:46:23 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Fri, 03 Sep 2021 02:46:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 02:46:27 GMT
ENV MEMCACHED_VERSION=1.6.10
# Fri, 03 Sep 2021 02:46:28 GMT
ENV MEMCACHED_SHA1=cb5b9fe77a2a59cc6cc7103a415bc07df9ddc6ec
# Fri, 03 Sep 2021 02:50:03 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Fri, 03 Sep 2021 02:50:03 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 03 Sep 2021 02:50:04 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 03 Sep 2021 02:50:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 03 Sep 2021 02:50:04 GMT
USER memcache
# Fri, 03 Sep 2021 02:50:05 GMT
EXPOSE 11211
# Fri, 03 Sep 2021 02:50:05 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:d10c227306ce3db344a8399cbc02bbf0dcb36519318efbde3c6027c00be8b40e`  
		Last Modified: Fri, 03 Sep 2021 00:49:47 GMT  
		Size: 25.9 MB (25914860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee708d85ae4c6929688ee243da330a395c81a5da3913f7aaaeea88283b5752b1`  
		Last Modified: Fri, 03 Sep 2021 02:51:01 GMT  
		Size: 5.0 KB (5024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41eee23f132aa5ef6810f141bd4852d174eb68bd5e9f8fc4e278e2fc55f7cea8`  
		Last Modified: Fri, 03 Sep 2021 02:51:02 GMT  
		Size: 2.1 MB (2075717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d9a7819a72ed1b598aabafd5ac9be7be62ac6b085cc30dbda97ef193641fc05`  
		Last Modified: Fri, 03 Sep 2021 02:51:01 GMT  
		Size: 1.3 MB (1254776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ae146d1bf5917e1fb0f4aa46a655feefc0ec5e00ef4e775beed00fa6a1d0aa1`  
		Last Modified: Fri, 03 Sep 2021 02:51:01 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3cae1f92b0ec75c4c83b4b5a4ce47b455952d638c215f1588a20af7261fba5b`  
		Last Modified: Fri, 03 Sep 2021 02:51:01 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6` - linux; 386

```console
$ docker pull memcached@sha256:221d230cb426e233ce34c9669663db5628d85a6ffe1d98292cfb54d66a7e1f8a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.3 MB (31292631 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7283abe72dd41573bd7262a0ba163f6ef7ddf757bc5178c95eea585f8335e784`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 03 Sep 2021 00:40:24 GMT
ADD file:6bf4b6f4aa28306610ef10c68f422a7210ff2fbd5345cec07bc5f76d54a4c8bc in / 
# Fri, 03 Sep 2021 00:40:24 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 06:44:15 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Fri, 03 Sep 2021 06:44:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 06:44:21 GMT
ENV MEMCACHED_VERSION=1.6.10
# Fri, 03 Sep 2021 06:44:21 GMT
ENV MEMCACHED_SHA1=cb5b9fe77a2a59cc6cc7103a415bc07df9ddc6ec
# Fri, 03 Sep 2021 06:48:23 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Fri, 03 Sep 2021 06:48:24 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 03 Sep 2021 06:48:25 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 03 Sep 2021 06:48:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 03 Sep 2021 06:48:26 GMT
USER memcache
# Fri, 03 Sep 2021 06:48:26 GMT
EXPOSE 11211
# Fri, 03 Sep 2021 06:48:26 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:7e87f600658a0c0d3bd8b82b9c645b5ec2763492ec627c1c1c1183c2ad3c45d5`  
		Last Modified: Fri, 03 Sep 2021 00:49:06 GMT  
		Size: 27.8 MB (27797513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9454a8c8c54135f6e7f591277550407671a2a183d0ea7a1b04e0b7bf1ecfeb39`  
		Last Modified: Fri, 03 Sep 2021 06:49:32 GMT  
		Size: 4.9 KB (4895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4900dba329569a63986180bc83b94449c1dffc3a804c2910a2a3f288509964d3`  
		Last Modified: Fri, 03 Sep 2021 06:49:32 GMT  
		Size: 2.2 MB (2209620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb8624563e6585b031c874cc180ee08148f5773238b0bc1571feb1b64b198ee5`  
		Last Modified: Fri, 03 Sep 2021 06:49:32 GMT  
		Size: 1.3 MB (1280199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86f15c6c59e3205f04fba85035da98cd62d3f67bca6baa035b56db7f4f5dfb5c`  
		Last Modified: Fri, 03 Sep 2021 06:49:32 GMT  
		Size: 283.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f1b51c6ca8d549a8b18622d1c15504b94257295420bc332544f8d9026fff6f3`  
		Last Modified: Fri, 03 Sep 2021 06:49:32 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6` - linux; mips64le

```console
$ docker pull memcached@sha256:33ce4398cd07967870c76b95ec5314cbe8280d564309b25d0640e8dd94cb7198
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.9 MB (28866865 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cc3e459293995ad1867b805e319ebb5b3942502abbad00cf3f9b3a4ccc26c740`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 28 Sep 2021 02:11:41 GMT
ADD file:df525c65bc60141f19ab937525d724c6d29cac53beb30f92d79ea4b2edf5a13e in / 
# Tue, 28 Sep 2021 02:11:41 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 02:51:00 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 28 Sep 2021 02:51:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:51:13 GMT
ENV MEMCACHED_VERSION=1.6.10
# Tue, 28 Sep 2021 02:51:13 GMT
ENV MEMCACHED_SHA1=cb5b9fe77a2a59cc6cc7103a415bc07df9ddc6ec
# Tue, 28 Sep 2021 02:56:56 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 28 Sep 2021 02:56:56 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 28 Sep 2021 02:56:58 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 28 Sep 2021 02:56:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 28 Sep 2021 02:56:59 GMT
USER memcache
# Tue, 28 Sep 2021 02:56:59 GMT
EXPOSE 11211
# Tue, 28 Sep 2021 02:56:59 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:f1b3d9dde862ddf88a05cec47ce54e641c4057c7bfb377e2a065c72a42a76321`  
		Last Modified: Tue, 28 Sep 2021 02:22:07 GMT  
		Size: 25.8 MB (25813001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e684588e988c227c0fedbcfeb8361e35b75eaa06e38cf8207979b491712d3dc`  
		Last Modified: Tue, 28 Sep 2021 02:57:18 GMT  
		Size: 5.0 KB (4981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35a3bc6181fe53d4bf46e98ebace046f2014668d601c2c3975c3dc6fc655acbc`  
		Last Modified: Tue, 28 Sep 2021 02:57:19 GMT  
		Size: 1.8 MB (1777273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f49b3d8a270ebba87297e2461fe81567f28a880e22d7ef977a60930ad82d6aa6`  
		Last Modified: Tue, 28 Sep 2021 02:57:19 GMT  
		Size: 1.3 MB (1271204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:119de6bb61edbff9dc8919b6bbb0f35c144a065c899d3fe20127480e2985c0d8`  
		Last Modified: Tue, 28 Sep 2021 02:57:18 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ecffae4c1838eb68ee866feaae4a6357c6198f1e86b5a1719bd7646795396d6`  
		Last Modified: Tue, 28 Sep 2021 02:57:18 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6` - linux; ppc64le

```console
$ docker pull memcached@sha256:49728dba09507cb74bbfae419b5b8051106768fd3b53aa7964da2b4a7cf0d44f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.2 MB (34190787 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4563ba0117902a70591f2170ab90e34de0431ae24402ee05aa741d4eafbd036f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 03 Sep 2021 01:24:33 GMT
ADD file:6c1662ddb92232ae8969a86a18dacab97b3b5792a1ecda49e6ac741a1a5c878c in / 
# Fri, 03 Sep 2021 01:24:41 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 08:06:59 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Fri, 03 Sep 2021 08:07:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 08:07:23 GMT
ENV MEMCACHED_VERSION=1.6.10
# Fri, 03 Sep 2021 08:07:26 GMT
ENV MEMCACHED_SHA1=cb5b9fe77a2a59cc6cc7103a415bc07df9ddc6ec
# Fri, 03 Sep 2021 08:13:31 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Fri, 03 Sep 2021 08:13:32 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 03 Sep 2021 08:13:43 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 03 Sep 2021 08:13:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 03 Sep 2021 08:13:57 GMT
USER memcache
# Fri, 03 Sep 2021 08:14:01 GMT
EXPOSE 11211
# Fri, 03 Sep 2021 08:14:05 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:8258146296247df1f308a336d4abf286afae14e3375edefb87a091e80745e29f`  
		Last Modified: Fri, 03 Sep 2021 01:39:45 GMT  
		Size: 30.6 MB (30553675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2f96132a11c70c50168ade17294cf7e8c919db231f87a28818170d9917a3268`  
		Last Modified: Fri, 03 Sep 2021 08:14:54 GMT  
		Size: 5.0 KB (4988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:973046a9e11e4bf003ce0e9688dc396e6e0ded760e9914a57132e130fa64289a`  
		Last Modified: Fri, 03 Sep 2021 08:14:55 GMT  
		Size: 2.3 MB (2323873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e5495ff67177662caa9f0459d68cb0641f32eddb666f4238634e357e58bdad1`  
		Last Modified: Fri, 03 Sep 2021 08:14:55 GMT  
		Size: 1.3 MB (1307845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b406b4303f1d8fe163586ca2e7abe3639c752a524f2c44e46677c01e36f937c`  
		Last Modified: Fri, 03 Sep 2021 08:14:54 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ff817a29aac3d654f6e919cbea3ea8125cce972e357c595217ec95807e07c3d`  
		Last Modified: Fri, 03 Sep 2021 08:14:54 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6` - linux; s390x

```console
$ docker pull memcached@sha256:53459c6f3d42b7b718e1ccbb3090ff35e649d8d005fa1917cee1ee1fbfea608a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.9 MB (28925755 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8831bffed7f4d435dd3c714d24529fea34f84468cbc5abec57feeb4728059de`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 28 Sep 2021 01:43:29 GMT
ADD file:118e7a596407435b5e2ff0aae6bb9bff3b66000c91ca37bfe1eeb98c23d99d49 in / 
# Tue, 28 Sep 2021 01:43:30 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 02:31:35 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 28 Sep 2021 02:31:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:31:39 GMT
ENV MEMCACHED_VERSION=1.6.10
# Tue, 28 Sep 2021 02:31:39 GMT
ENV MEMCACHED_SHA1=cb5b9fe77a2a59cc6cc7103a415bc07df9ddc6ec
# Tue, 28 Sep 2021 02:34:53 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 28 Sep 2021 02:34:54 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 28 Sep 2021 02:34:54 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 28 Sep 2021 02:34:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 28 Sep 2021 02:34:54 GMT
USER memcache
# Tue, 28 Sep 2021 02:34:54 GMT
EXPOSE 11211
# Tue, 28 Sep 2021 02:34:55 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:7cfe208f95c1b63305981b069795676fa149e7115b9044c241ee45ef4aaf0bb3`  
		Last Modified: Tue, 28 Sep 2021 01:49:36 GMT  
		Size: 25.8 MB (25760871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff755a70833a769c5a32cb251e86ac9aa6ae1dce7f547dc1bef874a22855b63d`  
		Last Modified: Tue, 28 Sep 2021 02:35:52 GMT  
		Size: 5.0 KB (5022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d08a7a4b96e17b9ef0eb0b8dd97ad0dc3d75227841b6374b7071e7989d9fed3c`  
		Last Modified: Tue, 28 Sep 2021 02:35:52 GMT  
		Size: 1.9 MB (1887230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4b9662cd31c943100c81ad7c951195bf462ad510ed53de50144b8617d870a84`  
		Last Modified: Tue, 28 Sep 2021 02:35:52 GMT  
		Size: 1.3 MB (1272226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fc50167475bec35471f2d4f925c2d427f3757ac01cd3f8f82cc5685771c2744`  
		Last Modified: Tue, 28 Sep 2021 02:35:52 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c69d6c53bee775bfd205e1d0426724cebf2eddd3034e82681311e18028641c25`  
		Last Modified: Tue, 28 Sep 2021 02:35:52 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:1.6-alpine`

```console
$ docker pull memcached@sha256:99e30a033ef422d6ad3ebe18c6c1009f20bee2d025fc00569be5dcd81aadc7be
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 7
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `memcached:1.6-alpine` - linux; amd64

```console
$ docker pull memcached@sha256:67d93d2efc4859c0b2e5a24bc13e759788c1f28d97a4d68b58a3de323e8ccb38
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3904613 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec200929117689b8cbba5a24fe5e892d7e4bfec5b654cef54958801a6ab9e92b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Fri, 27 Aug 2021 20:39:15 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Fri, 27 Aug 2021 20:39:16 GMT
RUN apk add --no-cache libsasl
# Fri, 27 Aug 2021 20:39:16 GMT
ENV MEMCACHED_VERSION=1.6.10
# Fri, 27 Aug 2021 20:39:17 GMT
ENV MEMCACHED_SHA1=cb5b9fe77a2a59cc6cc7103a415bc07df9ddc6ec
# Fri, 27 Aug 2021 20:43:47 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Fri, 27 Aug 2021 20:43:47 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 27 Aug 2021 20:43:49 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 27 Aug 2021 20:43:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 Aug 2021 20:43:50 GMT
USER memcache
# Fri, 27 Aug 2021 20:43:50 GMT
EXPOSE 11211
# Fri, 27 Aug 2021 20:43:50 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:a0d0a0d46f8b52473982a3c466318f479767577551a53ffc9074c9fa7035982e`  
		Last Modified: Fri, 27 Aug 2021 17:20:13 GMT  
		Size: 2.8 MB (2814446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84db6e403c6f8cdc8217536fa7d8bb9bbee66a7a49106104b3ceeace758e887b`  
		Last Modified: Fri, 27 Aug 2021 20:44:26 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7430c0d88cc6cc6389bb62e421f43031b009d21243f7362290bcf11b82e9e967`  
		Last Modified: Fri, 27 Aug 2021 20:44:26 GMT  
		Size: 155.5 KB (155516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3919afa4c767ba881b469a2798f6ad270dc23bbd9174d2994a0208bf508febba`  
		Last Modified: Fri, 27 Aug 2021 20:44:26 GMT  
		Size: 933.0 KB (932979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e81a6f988f7ee7ae5df06403e582d0edb09dcd73e81bacdaa17d1e0da71e13b`  
		Last Modified: Fri, 27 Aug 2021 20:44:26 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d5ed3d833f3ab3255decd4fc642f2368e6791acc470e40c2f3eb7463b7351dc`  
		Last Modified: Fri, 27 Aug 2021 20:44:26 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-alpine` - linux; arm variant v6

```console
$ docker pull memcached@sha256:4d05de82436bd51ed609a745b8ddd01e296692beb5a372dcbdcf0b1f54818d03
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.3 MB (4270486 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:56e8bda6e6346ca01fa3a313ef7bcfcc696040d48be803f6c16922dedc8deae1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 16 Dec 2020 23:49:43 GMT
ADD file:0a16715e2d0e5811c3c578945d618db0e269847a799340248f9ba8d393c9eec2 in / 
# Wed, 16 Dec 2020 23:49:45 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 01:44:25 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Thu, 17 Dec 2020 01:44:29 GMT
RUN apk add --no-cache cyrus-sasl-plain
# Thu, 17 Dec 2020 01:44:30 GMT
ENV MEMCACHED_VERSION=1.6.9
# Thu, 17 Dec 2020 01:44:31 GMT
ENV MEMCACHED_SHA1=42ae062094fdf083cfe7b21ff377c781011c2be1
# Thu, 17 Dec 2020 01:47:40 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		dpkg-dev dpkg 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		tar 		wget 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Thu, 17 Dec 2020 01:47:41 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 17 Dec 2020 01:47:43 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 17 Dec 2020 01:47:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Dec 2020 01:47:44 GMT
USER memcache
# Thu, 17 Dec 2020 01:47:45 GMT
EXPOSE 11211
# Thu, 17 Dec 2020 01:47:46 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:93247449aef3c56eb4f7ab7b3fed95743c974b823def6dd86ec84008126e7903`  
		Last Modified: Wed, 16 Dec 2020 23:50:24 GMT  
		Size: 2.6 MB (2604163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cc04af65958529b14246e2401008ef0186d74a33d2aa1b64d5f49633a1ff8f1`  
		Last Modified: Thu, 17 Dec 2020 01:48:06 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08bb28157acd02855bdf031eb7158f2cbb9849a6a9e6b45b4b82b507df6d83e9`  
		Last Modified: Thu, 17 Dec 2020 01:48:06 GMT  
		Size: 14.9 KB (14904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b32778d38f805e0e2a84689dba047adda457098c6f4a0b3aeb51a9e9d3e7f2b`  
		Last Modified: Thu, 17 Dec 2020 01:48:06 GMT  
		Size: 1.6 MB (1649753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:506d15aa86681d1812c5696615302d2a50938410c852b6aa0d0680c7baa4589f`  
		Last Modified: Thu, 17 Dec 2020 01:48:06 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f55730e61cf75cdadfaf0682212c74d7a2355e652e0655cc74ba35a4b7cfb4c1`  
		Last Modified: Thu, 17 Dec 2020 01:48:06 GMT  
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
$ docker pull memcached@sha256:8ed70173927cd66ad4e1bac9803ba7114502646685f70abb395ef668a46db5fb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3793233 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c5c3d9ec3f6b46ae9e7305a3958b059ffc7d935b5f2094e78973054a0394060e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 27 Aug 2021 17:39:33 GMT
ADD file:dc8af9c7bfe9f9541e1db38dea01c4201609f3075b31e108f2073ffed8c5e4b9 in / 
# Fri, 27 Aug 2021 17:39:33 GMT
CMD ["/bin/sh"]
# Fri, 27 Aug 2021 20:15:01 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Fri, 27 Aug 2021 20:15:02 GMT
RUN apk add --no-cache libsasl
# Fri, 27 Aug 2021 20:15:02 GMT
ENV MEMCACHED_VERSION=1.6.10
# Fri, 27 Aug 2021 20:15:02 GMT
ENV MEMCACHED_SHA1=cb5b9fe77a2a59cc6cc7103a415bc07df9ddc6ec
# Fri, 27 Aug 2021 20:18:55 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Fri, 27 Aug 2021 20:18:55 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 27 Aug 2021 20:18:56 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 27 Aug 2021 20:18:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 Aug 2021 20:18:56 GMT
USER memcache
# Fri, 27 Aug 2021 20:18:56 GMT
EXPOSE 11211
# Fri, 27 Aug 2021 20:18:56 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:552d1f2373af9bfe12033568ebbfb0ccbb0de11279f9a415a29207e264d7f4d9`  
		Last Modified: Fri, 27 Aug 2021 17:40:18 GMT  
		Size: 2.7 MB (2711827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ab312377ca26aa6df3e0bb8b11a63d6964544ffd2552b8e7cebb0acbbc3036d`  
		Last Modified: Fri, 27 Aug 2021 20:19:53 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a538168cab1a5c606dfa94dd8b09de5598c9071505476146fa99500011f8e7f5`  
		Last Modified: Fri, 27 Aug 2021 20:19:53 GMT  
		Size: 157.2 KB (157194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae4e52b47025818dc222e8dcd9310ab3f3c757a434fb786d7100cfaef304d4ed`  
		Last Modified: Fri, 27 Aug 2021 20:19:53 GMT  
		Size: 922.5 KB (922539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bedcb7a468e2a54e811d3ab62759e10500ea8b580eb12a600991eb1a3eed136`  
		Last Modified: Fri, 27 Aug 2021 20:19:53 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50b5ad9ab615a8b63e96efab0f2b3b2ff0a60abcb13a2529437f46368a641c6e`  
		Last Modified: Fri, 27 Aug 2021 20:19:53 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-alpine` - linux; 386

```console
$ docker pull memcached@sha256:82a99c470435ce9fd7cebf6565305c9f9a20eb2142839f8a7eaf42fc04b1e64a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3937988 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:503d28ddbe03b1e33458c354e3e0cef3142579c20bdf6e8c1f4b447257a2de01`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 27 Aug 2021 17:38:29 GMT
ADD file:42a7bc5a08b546b47049dd0f89ae4e7a8c86342f87000f39ade3ff52916a6c2e in / 
# Fri, 27 Aug 2021 17:38:30 GMT
CMD ["/bin/sh"]
# Fri, 27 Aug 2021 19:48:52 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Fri, 27 Aug 2021 19:48:54 GMT
RUN apk add --no-cache libsasl
# Fri, 27 Aug 2021 19:48:54 GMT
ENV MEMCACHED_VERSION=1.6.10
# Fri, 27 Aug 2021 19:48:55 GMT
ENV MEMCACHED_SHA1=cb5b9fe77a2a59cc6cc7103a415bc07df9ddc6ec
# Fri, 27 Aug 2021 19:53:36 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Fri, 27 Aug 2021 19:53:36 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 27 Aug 2021 19:53:37 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 27 Aug 2021 19:53:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 Aug 2021 19:53:38 GMT
USER memcache
# Fri, 27 Aug 2021 19:53:38 GMT
EXPOSE 11211
# Fri, 27 Aug 2021 19:53:38 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:b11ae9fc5d8a106cfed3a6f6c75e5b5b5797c566fac4411622b4055df6541286`  
		Last Modified: Fri, 27 Aug 2021 17:39:18 GMT  
		Size: 2.8 MB (2822857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a776c6c02658f2d17623bce57a634d82f2dc8c8bee59f4d90fc786c3e69e31ff`  
		Last Modified: Fri, 27 Aug 2021 19:54:35 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fab8279289e8b7a476ce09017d9bcdb33bccbe04750f2ccba41c0a43f828b16`  
		Last Modified: Fri, 27 Aug 2021 19:54:35 GMT  
		Size: 169.0 KB (169012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24c50e3cfd5d1f42d6dd2505b7b02ca2ed14cb53d2199df2bed319e84146d13b`  
		Last Modified: Fri, 27 Aug 2021 19:54:36 GMT  
		Size: 944.4 KB (944446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3856e8e8dfa799b89d86a7552466e0b451bc8b8b140b56d53056ea942b82b102`  
		Last Modified: Fri, 27 Aug 2021 19:54:35 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bd1d4e4fe24a075a95e91ec623e250fb1071d34af2ec3a777ceecca3d62ea9f`  
		Last Modified: Fri, 27 Aug 2021 19:54:35 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-alpine` - linux; ppc64le

```console
$ docker pull memcached@sha256:5ea0c2672938efeae9c4cf8a45bdb1a06eaacb2f1014ed8fef3d3c6339b3fac5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.0 MB (3954868 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e20a2c1b753cc0bb4b19ca80b7d333dcbb37ce0a77e99c1b96ef27b09b680fa7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 27 Aug 2021 19:39:54 GMT
ADD file:d213c56ffc24a5051e8060fd0fec1a0520367c10d88ab16321c36336b6c66098 in / 
# Fri, 27 Aug 2021 19:39:59 GMT
CMD ["/bin/sh"]
# Sat, 28 Aug 2021 02:52:59 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Sat, 28 Aug 2021 02:53:08 GMT
RUN apk add --no-cache libsasl
# Sat, 28 Aug 2021 02:53:10 GMT
ENV MEMCACHED_VERSION=1.6.10
# Sat, 28 Aug 2021 02:53:12 GMT
ENV MEMCACHED_SHA1=cb5b9fe77a2a59cc6cc7103a415bc07df9ddc6ec
# Sat, 28 Aug 2021 02:56:38 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Sat, 28 Aug 2021 02:56:40 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Sat, 28 Aug 2021 02:56:47 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Sat, 28 Aug 2021 02:56:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 28 Aug 2021 02:56:57 GMT
USER memcache
# Sat, 28 Aug 2021 02:57:02 GMT
EXPOSE 11211
# Sat, 28 Aug 2021 02:57:09 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:63da8ca98f7b4b94381aed56862a60aecf355d9428b9aeb7c61d5bd017100c18`  
		Last Modified: Fri, 27 Aug 2021 19:41:06 GMT  
		Size: 2.8 MB (2812284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a54fbc6ddd30fadabd2cf34600dd72918de6e611345c8202b6cd56a411467659`  
		Last Modified: Sat, 28 Aug 2021 02:58:02 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdd08b1afa1a2e02df391d85b3cfccf552f50b91046d9eafbe19feffb2f58910`  
		Last Modified: Sat, 28 Aug 2021 02:58:02 GMT  
		Size: 179.7 KB (179652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d214dccc5e7f55ecf8e9ec4471487fa0f6ba5ba2e84a3c746ff458410a29c755`  
		Last Modified: Sat, 28 Aug 2021 02:58:02 GMT  
		Size: 961.3 KB (961258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a6ae8b6fa12461573aab65c6be736cd4668463495c569d1113861ff729fb89f`  
		Last Modified: Sat, 28 Aug 2021 02:58:02 GMT  
		Size: 283.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fef62e61ad65fab7f854dd8a0a437b4ed6853b4186a9639a41ac47dae3f7d9e`  
		Last Modified: Sat, 28 Aug 2021 02:58:02 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-alpine` - linux; s390x

```console
$ docker pull memcached@sha256:cebdf9f1ff4ffe7551d4917b4a53e78ac48da41a694a8301fbd92459ebd9f45f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.7 MB (3695912 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:047503017563255821d3a05e00a220624c8698ef1a285eb6a05023ef0c1335e4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 27 Aug 2021 17:41:29 GMT
ADD file:9b40ee281e8797067fb2ae207c406084cb81593090338a8b7cb09ade52168daa in / 
# Fri, 27 Aug 2021 17:41:30 GMT
CMD ["/bin/sh"]
# Fri, 27 Aug 2021 19:13:56 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Fri, 27 Aug 2021 19:13:58 GMT
RUN apk add --no-cache libsasl
# Fri, 27 Aug 2021 19:13:59 GMT
ENV MEMCACHED_VERSION=1.6.10
# Fri, 27 Aug 2021 19:13:59 GMT
ENV MEMCACHED_SHA1=cb5b9fe77a2a59cc6cc7103a415bc07df9ddc6ec
# Fri, 27 Aug 2021 19:22:03 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Fri, 27 Aug 2021 19:22:04 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 27 Aug 2021 19:22:05 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 27 Aug 2021 19:22:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 Aug 2021 19:22:06 GMT
USER memcache
# Fri, 27 Aug 2021 19:22:06 GMT
EXPOSE 11211
# Fri, 27 Aug 2021 19:22:07 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:da14cb6b6dc946dbb2d84386bcaca84e2d46f650767cd11bdb3331ec9d623988`  
		Last Modified: Fri, 27 Aug 2021 17:42:25 GMT  
		Size: 2.6 MB (2603464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5c3123815589d4cfc45a071f344bd0f3ca08ee63a471c2c114af2dece4699a0`  
		Last Modified: Fri, 27 Aug 2021 19:23:06 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d25c400e2d4eb8dee97bc754e9e52585af4304ec8cf3121b619bd5756796fb52`  
		Last Modified: Fri, 27 Aug 2021 19:23:06 GMT  
		Size: 161.5 KB (161520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:611fd541e530a5444852c1a56f01565817097a4b2abec64399dcf4fdd84dfe88`  
		Last Modified: Fri, 27 Aug 2021 19:23:06 GMT  
		Size: 929.3 KB (929257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cb82aed96a5a46fb2399db9bf85a3ff9a7ce3de3468fe74285ad84fd557a1ca`  
		Last Modified: Fri, 27 Aug 2021 19:23:06 GMT  
		Size: 283.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c18159f487fe568305c6aaeb29b07af5f859402bb29566a404f9fccbd86bafbf`  
		Last Modified: Fri, 27 Aug 2021 19:23:06 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:1.6-alpine3.14`

```console
$ docker pull memcached@sha256:d57531b1d9bfffc9ada8c669fe761da3c7f9a15b9ac27d0f383e318d40f90e0d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `memcached:1.6-alpine3.14` - linux; amd64

```console
$ docker pull memcached@sha256:67d93d2efc4859c0b2e5a24bc13e759788c1f28d97a4d68b58a3de323e8ccb38
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3904613 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec200929117689b8cbba5a24fe5e892d7e4bfec5b654cef54958801a6ab9e92b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Fri, 27 Aug 2021 20:39:15 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Fri, 27 Aug 2021 20:39:16 GMT
RUN apk add --no-cache libsasl
# Fri, 27 Aug 2021 20:39:16 GMT
ENV MEMCACHED_VERSION=1.6.10
# Fri, 27 Aug 2021 20:39:17 GMT
ENV MEMCACHED_SHA1=cb5b9fe77a2a59cc6cc7103a415bc07df9ddc6ec
# Fri, 27 Aug 2021 20:43:47 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Fri, 27 Aug 2021 20:43:47 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 27 Aug 2021 20:43:49 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 27 Aug 2021 20:43:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 Aug 2021 20:43:50 GMT
USER memcache
# Fri, 27 Aug 2021 20:43:50 GMT
EXPOSE 11211
# Fri, 27 Aug 2021 20:43:50 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:a0d0a0d46f8b52473982a3c466318f479767577551a53ffc9074c9fa7035982e`  
		Last Modified: Fri, 27 Aug 2021 17:20:13 GMT  
		Size: 2.8 MB (2814446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84db6e403c6f8cdc8217536fa7d8bb9bbee66a7a49106104b3ceeace758e887b`  
		Last Modified: Fri, 27 Aug 2021 20:44:26 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7430c0d88cc6cc6389bb62e421f43031b009d21243f7362290bcf11b82e9e967`  
		Last Modified: Fri, 27 Aug 2021 20:44:26 GMT  
		Size: 155.5 KB (155516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3919afa4c767ba881b469a2798f6ad270dc23bbd9174d2994a0208bf508febba`  
		Last Modified: Fri, 27 Aug 2021 20:44:26 GMT  
		Size: 933.0 KB (932979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e81a6f988f7ee7ae5df06403e582d0edb09dcd73e81bacdaa17d1e0da71e13b`  
		Last Modified: Fri, 27 Aug 2021 20:44:26 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d5ed3d833f3ab3255decd4fc642f2368e6791acc470e40c2f3eb7463b7351dc`  
		Last Modified: Fri, 27 Aug 2021 20:44:26 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-alpine3.14` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:8ed70173927cd66ad4e1bac9803ba7114502646685f70abb395ef668a46db5fb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3793233 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c5c3d9ec3f6b46ae9e7305a3958b059ffc7d935b5f2094e78973054a0394060e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 27 Aug 2021 17:39:33 GMT
ADD file:dc8af9c7bfe9f9541e1db38dea01c4201609f3075b31e108f2073ffed8c5e4b9 in / 
# Fri, 27 Aug 2021 17:39:33 GMT
CMD ["/bin/sh"]
# Fri, 27 Aug 2021 20:15:01 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Fri, 27 Aug 2021 20:15:02 GMT
RUN apk add --no-cache libsasl
# Fri, 27 Aug 2021 20:15:02 GMT
ENV MEMCACHED_VERSION=1.6.10
# Fri, 27 Aug 2021 20:15:02 GMT
ENV MEMCACHED_SHA1=cb5b9fe77a2a59cc6cc7103a415bc07df9ddc6ec
# Fri, 27 Aug 2021 20:18:55 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Fri, 27 Aug 2021 20:18:55 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 27 Aug 2021 20:18:56 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 27 Aug 2021 20:18:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 Aug 2021 20:18:56 GMT
USER memcache
# Fri, 27 Aug 2021 20:18:56 GMT
EXPOSE 11211
# Fri, 27 Aug 2021 20:18:56 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:552d1f2373af9bfe12033568ebbfb0ccbb0de11279f9a415a29207e264d7f4d9`  
		Last Modified: Fri, 27 Aug 2021 17:40:18 GMT  
		Size: 2.7 MB (2711827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ab312377ca26aa6df3e0bb8b11a63d6964544ffd2552b8e7cebb0acbbc3036d`  
		Last Modified: Fri, 27 Aug 2021 20:19:53 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a538168cab1a5c606dfa94dd8b09de5598c9071505476146fa99500011f8e7f5`  
		Last Modified: Fri, 27 Aug 2021 20:19:53 GMT  
		Size: 157.2 KB (157194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae4e52b47025818dc222e8dcd9310ab3f3c757a434fb786d7100cfaef304d4ed`  
		Last Modified: Fri, 27 Aug 2021 20:19:53 GMT  
		Size: 922.5 KB (922539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bedcb7a468e2a54e811d3ab62759e10500ea8b580eb12a600991eb1a3eed136`  
		Last Modified: Fri, 27 Aug 2021 20:19:53 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50b5ad9ab615a8b63e96efab0f2b3b2ff0a60abcb13a2529437f46368a641c6e`  
		Last Modified: Fri, 27 Aug 2021 20:19:53 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-alpine3.14` - linux; 386

```console
$ docker pull memcached@sha256:82a99c470435ce9fd7cebf6565305c9f9a20eb2142839f8a7eaf42fc04b1e64a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3937988 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:503d28ddbe03b1e33458c354e3e0cef3142579c20bdf6e8c1f4b447257a2de01`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 27 Aug 2021 17:38:29 GMT
ADD file:42a7bc5a08b546b47049dd0f89ae4e7a8c86342f87000f39ade3ff52916a6c2e in / 
# Fri, 27 Aug 2021 17:38:30 GMT
CMD ["/bin/sh"]
# Fri, 27 Aug 2021 19:48:52 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Fri, 27 Aug 2021 19:48:54 GMT
RUN apk add --no-cache libsasl
# Fri, 27 Aug 2021 19:48:54 GMT
ENV MEMCACHED_VERSION=1.6.10
# Fri, 27 Aug 2021 19:48:55 GMT
ENV MEMCACHED_SHA1=cb5b9fe77a2a59cc6cc7103a415bc07df9ddc6ec
# Fri, 27 Aug 2021 19:53:36 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Fri, 27 Aug 2021 19:53:36 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 27 Aug 2021 19:53:37 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 27 Aug 2021 19:53:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 Aug 2021 19:53:38 GMT
USER memcache
# Fri, 27 Aug 2021 19:53:38 GMT
EXPOSE 11211
# Fri, 27 Aug 2021 19:53:38 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:b11ae9fc5d8a106cfed3a6f6c75e5b5b5797c566fac4411622b4055df6541286`  
		Last Modified: Fri, 27 Aug 2021 17:39:18 GMT  
		Size: 2.8 MB (2822857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a776c6c02658f2d17623bce57a634d82f2dc8c8bee59f4d90fc786c3e69e31ff`  
		Last Modified: Fri, 27 Aug 2021 19:54:35 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fab8279289e8b7a476ce09017d9bcdb33bccbe04750f2ccba41c0a43f828b16`  
		Last Modified: Fri, 27 Aug 2021 19:54:35 GMT  
		Size: 169.0 KB (169012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24c50e3cfd5d1f42d6dd2505b7b02ca2ed14cb53d2199df2bed319e84146d13b`  
		Last Modified: Fri, 27 Aug 2021 19:54:36 GMT  
		Size: 944.4 KB (944446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3856e8e8dfa799b89d86a7552466e0b451bc8b8b140b56d53056ea942b82b102`  
		Last Modified: Fri, 27 Aug 2021 19:54:35 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bd1d4e4fe24a075a95e91ec623e250fb1071d34af2ec3a777ceecca3d62ea9f`  
		Last Modified: Fri, 27 Aug 2021 19:54:35 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-alpine3.14` - linux; ppc64le

```console
$ docker pull memcached@sha256:5ea0c2672938efeae9c4cf8a45bdb1a06eaacb2f1014ed8fef3d3c6339b3fac5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.0 MB (3954868 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e20a2c1b753cc0bb4b19ca80b7d333dcbb37ce0a77e99c1b96ef27b09b680fa7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 27 Aug 2021 19:39:54 GMT
ADD file:d213c56ffc24a5051e8060fd0fec1a0520367c10d88ab16321c36336b6c66098 in / 
# Fri, 27 Aug 2021 19:39:59 GMT
CMD ["/bin/sh"]
# Sat, 28 Aug 2021 02:52:59 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Sat, 28 Aug 2021 02:53:08 GMT
RUN apk add --no-cache libsasl
# Sat, 28 Aug 2021 02:53:10 GMT
ENV MEMCACHED_VERSION=1.6.10
# Sat, 28 Aug 2021 02:53:12 GMT
ENV MEMCACHED_SHA1=cb5b9fe77a2a59cc6cc7103a415bc07df9ddc6ec
# Sat, 28 Aug 2021 02:56:38 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Sat, 28 Aug 2021 02:56:40 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Sat, 28 Aug 2021 02:56:47 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Sat, 28 Aug 2021 02:56:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 28 Aug 2021 02:56:57 GMT
USER memcache
# Sat, 28 Aug 2021 02:57:02 GMT
EXPOSE 11211
# Sat, 28 Aug 2021 02:57:09 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:63da8ca98f7b4b94381aed56862a60aecf355d9428b9aeb7c61d5bd017100c18`  
		Last Modified: Fri, 27 Aug 2021 19:41:06 GMT  
		Size: 2.8 MB (2812284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a54fbc6ddd30fadabd2cf34600dd72918de6e611345c8202b6cd56a411467659`  
		Last Modified: Sat, 28 Aug 2021 02:58:02 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdd08b1afa1a2e02df391d85b3cfccf552f50b91046d9eafbe19feffb2f58910`  
		Last Modified: Sat, 28 Aug 2021 02:58:02 GMT  
		Size: 179.7 KB (179652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d214dccc5e7f55ecf8e9ec4471487fa0f6ba5ba2e84a3c746ff458410a29c755`  
		Last Modified: Sat, 28 Aug 2021 02:58:02 GMT  
		Size: 961.3 KB (961258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a6ae8b6fa12461573aab65c6be736cd4668463495c569d1113861ff729fb89f`  
		Last Modified: Sat, 28 Aug 2021 02:58:02 GMT  
		Size: 283.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fef62e61ad65fab7f854dd8a0a437b4ed6853b4186a9639a41ac47dae3f7d9e`  
		Last Modified: Sat, 28 Aug 2021 02:58:02 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-alpine3.14` - linux; s390x

```console
$ docker pull memcached@sha256:cebdf9f1ff4ffe7551d4917b4a53e78ac48da41a694a8301fbd92459ebd9f45f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.7 MB (3695912 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:047503017563255821d3a05e00a220624c8698ef1a285eb6a05023ef0c1335e4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 27 Aug 2021 17:41:29 GMT
ADD file:9b40ee281e8797067fb2ae207c406084cb81593090338a8b7cb09ade52168daa in / 
# Fri, 27 Aug 2021 17:41:30 GMT
CMD ["/bin/sh"]
# Fri, 27 Aug 2021 19:13:56 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Fri, 27 Aug 2021 19:13:58 GMT
RUN apk add --no-cache libsasl
# Fri, 27 Aug 2021 19:13:59 GMT
ENV MEMCACHED_VERSION=1.6.10
# Fri, 27 Aug 2021 19:13:59 GMT
ENV MEMCACHED_SHA1=cb5b9fe77a2a59cc6cc7103a415bc07df9ddc6ec
# Fri, 27 Aug 2021 19:22:03 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Fri, 27 Aug 2021 19:22:04 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 27 Aug 2021 19:22:05 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 27 Aug 2021 19:22:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 Aug 2021 19:22:06 GMT
USER memcache
# Fri, 27 Aug 2021 19:22:06 GMT
EXPOSE 11211
# Fri, 27 Aug 2021 19:22:07 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:da14cb6b6dc946dbb2d84386bcaca84e2d46f650767cd11bdb3331ec9d623988`  
		Last Modified: Fri, 27 Aug 2021 17:42:25 GMT  
		Size: 2.6 MB (2603464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5c3123815589d4cfc45a071f344bd0f3ca08ee63a471c2c114af2dece4699a0`  
		Last Modified: Fri, 27 Aug 2021 19:23:06 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d25c400e2d4eb8dee97bc754e9e52585af4304ec8cf3121b619bd5756796fb52`  
		Last Modified: Fri, 27 Aug 2021 19:23:06 GMT  
		Size: 161.5 KB (161520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:611fd541e530a5444852c1a56f01565817097a4b2abec64399dcf4fdd84dfe88`  
		Last Modified: Fri, 27 Aug 2021 19:23:06 GMT  
		Size: 929.3 KB (929257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cb82aed96a5a46fb2399db9bf85a3ff9a7ce3de3468fe74285ad84fd557a1ca`  
		Last Modified: Fri, 27 Aug 2021 19:23:06 GMT  
		Size: 283.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c18159f487fe568305c6aaeb29b07af5f859402bb29566a404f9fccbd86bafbf`  
		Last Modified: Fri, 27 Aug 2021 19:23:06 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:1.6-buster`

```console
$ docker pull memcached@sha256:0507080446e022bbcb398fef743f5479d61569f2992beccd200033e037968511
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

### `memcached:1.6-buster` - linux; amd64

```console
$ docker pull memcached@sha256:b93ad58a06f215580205490133ce2165fa69f1930b964e890981f629df497e84
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.6 MB (30631755 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:444d9869f3507356b3fb6ffb7ed74ffc3be04be873a6876423c24d17acbf1128`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 03 Sep 2021 01:21:46 GMT
ADD file:4ff85d9f6aa246746912db62dea02eb71750474bb29611e770516a1fcd217add in / 
# Fri, 03 Sep 2021 01:21:46 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 07:33:54 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Fri, 03 Sep 2021 07:34:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 07:34:01 GMT
ENV MEMCACHED_VERSION=1.6.10
# Fri, 03 Sep 2021 07:34:01 GMT
ENV MEMCACHED_SHA1=cb5b9fe77a2a59cc6cc7103a415bc07df9ddc6ec
# Fri, 03 Sep 2021 07:38:24 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Fri, 03 Sep 2021 07:38:24 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 03 Sep 2021 07:38:25 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 03 Sep 2021 07:38:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 03 Sep 2021 07:38:25 GMT
USER memcache
# Fri, 03 Sep 2021 07:38:26 GMT
EXPOSE 11211
# Fri, 03 Sep 2021 07:38:26 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:a330b6cecb98cd2425fd25fce36669073f593b3176b4ee14731e48c05d678cdd`  
		Last Modified: Fri, 03 Sep 2021 01:28:19 GMT  
		Size: 27.1 MB (27145844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7dcde8d481fe08e2bab1fc8a1dc0e30c1d8cc9647d2867a6bc06942de810d56`  
		Last Modified: Fri, 03 Sep 2021 07:38:54 GMT  
		Size: 5.0 KB (4981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c3e0b65008f095303aa1ff733845d2eed7b3836fad196bc16533b3420711745`  
		Last Modified: Fri, 03 Sep 2021 07:38:54 GMT  
		Size: 2.2 MB (2197580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ad3eb30b171e7b0c33373bdeb39dfc36b63b8ec501af75bae3d4a964872f042`  
		Last Modified: Fri, 03 Sep 2021 07:38:54 GMT  
		Size: 1.3 MB (1282944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e6e03de9a5467b70b4d10bf021740a05eea1aeebfd87864b4a9289df9cb64c0`  
		Last Modified: Fri, 03 Sep 2021 07:38:54 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe0025a339764c7acc0034c701ca2b443e0b1803745c41094ea54289f754a81c`  
		Last Modified: Fri, 03 Sep 2021 07:38:54 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-buster` - linux; arm variant v5

```console
$ docker pull memcached@sha256:5e1d0b6ce4b1b257e47c484709733908552416681c8f054bc97735e5ec114fa2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.0 MB (28036699 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd9fb75ae310df2e536d3a10e6dd9222317f89456fe6082c139b112849e5081b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 03 Sep 2021 00:51:26 GMT
ADD file:350748a564076da397b991745cd42e0688d15c72b9fd5c81f8ea0bb8938a2b3d in / 
# Fri, 03 Sep 2021 00:51:27 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 02:24:47 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Fri, 03 Sep 2021 02:24:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 02:24:58 GMT
ENV MEMCACHED_VERSION=1.6.10
# Fri, 03 Sep 2021 02:24:59 GMT
ENV MEMCACHED_SHA1=cb5b9fe77a2a59cc6cc7103a415bc07df9ddc6ec
# Fri, 03 Sep 2021 02:29:11 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Fri, 03 Sep 2021 02:29:12 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 03 Sep 2021 02:29:13 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 03 Sep 2021 02:29:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 03 Sep 2021 02:29:14 GMT
USER memcache
# Fri, 03 Sep 2021 02:29:14 GMT
EXPOSE 11211
# Fri, 03 Sep 2021 02:29:15 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:b019db4b5197128481d48d92ecacd6bb356c027a3d08393f6567a6fa183ba769`  
		Last Modified: Fri, 03 Sep 2021 01:07:12 GMT  
		Size: 24.9 MB (24879114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4faeba39e66674ac57454c2edb8018a9a29475db4893acb59bf00e84e5c4e88a`  
		Last Modified: Fri, 03 Sep 2021 02:30:10 GMT  
		Size: 4.9 KB (4895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b39e5da0381154e8db96921f6038b79a61f458bf76f9fdaae0d3f44b2d81f184`  
		Last Modified: Fri, 03 Sep 2021 02:30:11 GMT  
		Size: 1.9 MB (1897972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb47be4e43a9bfad0082a507b5885f22b4104821defe786af5237a6b48211a71`  
		Last Modified: Fri, 03 Sep 2021 02:30:11 GMT  
		Size: 1.3 MB (1254312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee01c0ace3ff5a5a86664234d47a50480b12f50f1390f5b78ab2b76a73e3346f`  
		Last Modified: Fri, 03 Sep 2021 02:30:10 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:240af99f2a1c8953e4436d48b387f4aa33defc9e83416c71f2d67d05c2a8cb48`  
		Last Modified: Fri, 03 Sep 2021 02:30:10 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-buster` - linux; arm variant v7

```console
$ docker pull memcached@sha256:ee3f4a07ff534651238a464f5b0a3b582facdc9784f9e0f9a5bcd0128762da4f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.8 MB (25788867 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6222a822647e49fef3f296a084e4504bd705efe8e0649bc91541e03b8a5d7b8a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 03 Sep 2021 01:00:40 GMT
ADD file:4754bbccf4c59f77dd54f3888871f0635a2f9655cda53f50e63237f1580286e0 in / 
# Fri, 03 Sep 2021 01:00:41 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 06:44:19 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Fri, 03 Sep 2021 06:44:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 06:44:29 GMT
ENV MEMCACHED_VERSION=1.6.10
# Fri, 03 Sep 2021 06:44:30 GMT
ENV MEMCACHED_SHA1=cb5b9fe77a2a59cc6cc7103a415bc07df9ddc6ec
# Fri, 03 Sep 2021 06:48:21 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Fri, 03 Sep 2021 06:48:22 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 03 Sep 2021 06:48:23 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 03 Sep 2021 06:48:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 03 Sep 2021 06:48:24 GMT
USER memcache
# Fri, 03 Sep 2021 06:48:25 GMT
EXPOSE 11211
# Fri, 03 Sep 2021 06:48:25 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:2215ad7863d95c38f1f794f1d5b4d6c5ca4ca7e921e4bb7218b803f7ed270675`  
		Last Modified: Fri, 03 Sep 2021 01:16:23 GMT  
		Size: 22.7 MB (22746151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d554d32fa680ffcf04f8b509fa6a16e796fadc0ecf8db8c48bcc2a911f9f4591`  
		Last Modified: Fri, 03 Sep 2021 07:00:56 GMT  
		Size: 4.9 KB (4895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a550041e12d651682f2b70b45620898d8cebd97f4b4b3469aaeac8d452a76ef`  
		Last Modified: Fri, 03 Sep 2021 07:00:56 GMT  
		Size: 1.8 MB (1812490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ae1581582d0b08a4635fe57247a454da856fea52ec988126ee4f2f1781b7acd`  
		Last Modified: Fri, 03 Sep 2021 07:00:56 GMT  
		Size: 1.2 MB (1224925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:678c3e64de445bdc9a420655f01c8abab5f2e7ef4f41d441e6d2310ea2c36de5`  
		Last Modified: Fri, 03 Sep 2021 07:00:55 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a21b13a7b8549e46debb4d9b1117211df9edcc02f822ec99d1fe1b4278f1e56`  
		Last Modified: Fri, 03 Sep 2021 07:00:55 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-buster` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:57e906b2282c3e67137cc8c2ab5148c8e748256b2e3934c5b7ecd77a6a186de5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.3 MB (29250783 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:932f1c94fc6e8e017820dcb97fe4b624efacba7409cb99c99a369c649b03829d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 03 Sep 2021 00:40:58 GMT
ADD file:4a1d7f2d989aee6bd83da076b6e9dd3da2da97cf5654bd37568e9baec30ac4b1 in / 
# Fri, 03 Sep 2021 00:40:58 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 02:46:23 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Fri, 03 Sep 2021 02:46:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 02:46:27 GMT
ENV MEMCACHED_VERSION=1.6.10
# Fri, 03 Sep 2021 02:46:28 GMT
ENV MEMCACHED_SHA1=cb5b9fe77a2a59cc6cc7103a415bc07df9ddc6ec
# Fri, 03 Sep 2021 02:50:03 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Fri, 03 Sep 2021 02:50:03 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 03 Sep 2021 02:50:04 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 03 Sep 2021 02:50:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 03 Sep 2021 02:50:04 GMT
USER memcache
# Fri, 03 Sep 2021 02:50:05 GMT
EXPOSE 11211
# Fri, 03 Sep 2021 02:50:05 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:d10c227306ce3db344a8399cbc02bbf0dcb36519318efbde3c6027c00be8b40e`  
		Last Modified: Fri, 03 Sep 2021 00:49:47 GMT  
		Size: 25.9 MB (25914860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee708d85ae4c6929688ee243da330a395c81a5da3913f7aaaeea88283b5752b1`  
		Last Modified: Fri, 03 Sep 2021 02:51:01 GMT  
		Size: 5.0 KB (5024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41eee23f132aa5ef6810f141bd4852d174eb68bd5e9f8fc4e278e2fc55f7cea8`  
		Last Modified: Fri, 03 Sep 2021 02:51:02 GMT  
		Size: 2.1 MB (2075717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d9a7819a72ed1b598aabafd5ac9be7be62ac6b085cc30dbda97ef193641fc05`  
		Last Modified: Fri, 03 Sep 2021 02:51:01 GMT  
		Size: 1.3 MB (1254776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ae146d1bf5917e1fb0f4aa46a655feefc0ec5e00ef4e775beed00fa6a1d0aa1`  
		Last Modified: Fri, 03 Sep 2021 02:51:01 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3cae1f92b0ec75c4c83b4b5a4ce47b455952d638c215f1588a20af7261fba5b`  
		Last Modified: Fri, 03 Sep 2021 02:51:01 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-buster` - linux; 386

```console
$ docker pull memcached@sha256:221d230cb426e233ce34c9669663db5628d85a6ffe1d98292cfb54d66a7e1f8a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.3 MB (31292631 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7283abe72dd41573bd7262a0ba163f6ef7ddf757bc5178c95eea585f8335e784`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 03 Sep 2021 00:40:24 GMT
ADD file:6bf4b6f4aa28306610ef10c68f422a7210ff2fbd5345cec07bc5f76d54a4c8bc in / 
# Fri, 03 Sep 2021 00:40:24 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 06:44:15 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Fri, 03 Sep 2021 06:44:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 06:44:21 GMT
ENV MEMCACHED_VERSION=1.6.10
# Fri, 03 Sep 2021 06:44:21 GMT
ENV MEMCACHED_SHA1=cb5b9fe77a2a59cc6cc7103a415bc07df9ddc6ec
# Fri, 03 Sep 2021 06:48:23 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Fri, 03 Sep 2021 06:48:24 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 03 Sep 2021 06:48:25 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 03 Sep 2021 06:48:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 03 Sep 2021 06:48:26 GMT
USER memcache
# Fri, 03 Sep 2021 06:48:26 GMT
EXPOSE 11211
# Fri, 03 Sep 2021 06:48:26 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:7e87f600658a0c0d3bd8b82b9c645b5ec2763492ec627c1c1c1183c2ad3c45d5`  
		Last Modified: Fri, 03 Sep 2021 00:49:06 GMT  
		Size: 27.8 MB (27797513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9454a8c8c54135f6e7f591277550407671a2a183d0ea7a1b04e0b7bf1ecfeb39`  
		Last Modified: Fri, 03 Sep 2021 06:49:32 GMT  
		Size: 4.9 KB (4895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4900dba329569a63986180bc83b94449c1dffc3a804c2910a2a3f288509964d3`  
		Last Modified: Fri, 03 Sep 2021 06:49:32 GMT  
		Size: 2.2 MB (2209620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb8624563e6585b031c874cc180ee08148f5773238b0bc1571feb1b64b198ee5`  
		Last Modified: Fri, 03 Sep 2021 06:49:32 GMT  
		Size: 1.3 MB (1280199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86f15c6c59e3205f04fba85035da98cd62d3f67bca6baa035b56db7f4f5dfb5c`  
		Last Modified: Fri, 03 Sep 2021 06:49:32 GMT  
		Size: 283.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f1b51c6ca8d549a8b18622d1c15504b94257295420bc332544f8d9026fff6f3`  
		Last Modified: Fri, 03 Sep 2021 06:49:32 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-buster` - linux; mips64le

```console
$ docker pull memcached@sha256:33ce4398cd07967870c76b95ec5314cbe8280d564309b25d0640e8dd94cb7198
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.9 MB (28866865 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cc3e459293995ad1867b805e319ebb5b3942502abbad00cf3f9b3a4ccc26c740`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 28 Sep 2021 02:11:41 GMT
ADD file:df525c65bc60141f19ab937525d724c6d29cac53beb30f92d79ea4b2edf5a13e in / 
# Tue, 28 Sep 2021 02:11:41 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 02:51:00 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 28 Sep 2021 02:51:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:51:13 GMT
ENV MEMCACHED_VERSION=1.6.10
# Tue, 28 Sep 2021 02:51:13 GMT
ENV MEMCACHED_SHA1=cb5b9fe77a2a59cc6cc7103a415bc07df9ddc6ec
# Tue, 28 Sep 2021 02:56:56 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 28 Sep 2021 02:56:56 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 28 Sep 2021 02:56:58 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 28 Sep 2021 02:56:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 28 Sep 2021 02:56:59 GMT
USER memcache
# Tue, 28 Sep 2021 02:56:59 GMT
EXPOSE 11211
# Tue, 28 Sep 2021 02:56:59 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:f1b3d9dde862ddf88a05cec47ce54e641c4057c7bfb377e2a065c72a42a76321`  
		Last Modified: Tue, 28 Sep 2021 02:22:07 GMT  
		Size: 25.8 MB (25813001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e684588e988c227c0fedbcfeb8361e35b75eaa06e38cf8207979b491712d3dc`  
		Last Modified: Tue, 28 Sep 2021 02:57:18 GMT  
		Size: 5.0 KB (4981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35a3bc6181fe53d4bf46e98ebace046f2014668d601c2c3975c3dc6fc655acbc`  
		Last Modified: Tue, 28 Sep 2021 02:57:19 GMT  
		Size: 1.8 MB (1777273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f49b3d8a270ebba87297e2461fe81567f28a880e22d7ef977a60930ad82d6aa6`  
		Last Modified: Tue, 28 Sep 2021 02:57:19 GMT  
		Size: 1.3 MB (1271204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:119de6bb61edbff9dc8919b6bbb0f35c144a065c899d3fe20127480e2985c0d8`  
		Last Modified: Tue, 28 Sep 2021 02:57:18 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ecffae4c1838eb68ee866feaae4a6357c6198f1e86b5a1719bd7646795396d6`  
		Last Modified: Tue, 28 Sep 2021 02:57:18 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-buster` - linux; ppc64le

```console
$ docker pull memcached@sha256:49728dba09507cb74bbfae419b5b8051106768fd3b53aa7964da2b4a7cf0d44f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.2 MB (34190787 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4563ba0117902a70591f2170ab90e34de0431ae24402ee05aa741d4eafbd036f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 03 Sep 2021 01:24:33 GMT
ADD file:6c1662ddb92232ae8969a86a18dacab97b3b5792a1ecda49e6ac741a1a5c878c in / 
# Fri, 03 Sep 2021 01:24:41 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 08:06:59 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Fri, 03 Sep 2021 08:07:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 08:07:23 GMT
ENV MEMCACHED_VERSION=1.6.10
# Fri, 03 Sep 2021 08:07:26 GMT
ENV MEMCACHED_SHA1=cb5b9fe77a2a59cc6cc7103a415bc07df9ddc6ec
# Fri, 03 Sep 2021 08:13:31 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Fri, 03 Sep 2021 08:13:32 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 03 Sep 2021 08:13:43 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 03 Sep 2021 08:13:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 03 Sep 2021 08:13:57 GMT
USER memcache
# Fri, 03 Sep 2021 08:14:01 GMT
EXPOSE 11211
# Fri, 03 Sep 2021 08:14:05 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:8258146296247df1f308a336d4abf286afae14e3375edefb87a091e80745e29f`  
		Last Modified: Fri, 03 Sep 2021 01:39:45 GMT  
		Size: 30.6 MB (30553675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2f96132a11c70c50168ade17294cf7e8c919db231f87a28818170d9917a3268`  
		Last Modified: Fri, 03 Sep 2021 08:14:54 GMT  
		Size: 5.0 KB (4988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:973046a9e11e4bf003ce0e9688dc396e6e0ded760e9914a57132e130fa64289a`  
		Last Modified: Fri, 03 Sep 2021 08:14:55 GMT  
		Size: 2.3 MB (2323873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e5495ff67177662caa9f0459d68cb0641f32eddb666f4238634e357e58bdad1`  
		Last Modified: Fri, 03 Sep 2021 08:14:55 GMT  
		Size: 1.3 MB (1307845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b406b4303f1d8fe163586ca2e7abe3639c752a524f2c44e46677c01e36f937c`  
		Last Modified: Fri, 03 Sep 2021 08:14:54 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ff817a29aac3d654f6e919cbea3ea8125cce972e357c595217ec95807e07c3d`  
		Last Modified: Fri, 03 Sep 2021 08:14:54 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-buster` - linux; s390x

```console
$ docker pull memcached@sha256:53459c6f3d42b7b718e1ccbb3090ff35e649d8d005fa1917cee1ee1fbfea608a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.9 MB (28925755 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8831bffed7f4d435dd3c714d24529fea34f84468cbc5abec57feeb4728059de`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 28 Sep 2021 01:43:29 GMT
ADD file:118e7a596407435b5e2ff0aae6bb9bff3b66000c91ca37bfe1eeb98c23d99d49 in / 
# Tue, 28 Sep 2021 01:43:30 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 02:31:35 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 28 Sep 2021 02:31:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:31:39 GMT
ENV MEMCACHED_VERSION=1.6.10
# Tue, 28 Sep 2021 02:31:39 GMT
ENV MEMCACHED_SHA1=cb5b9fe77a2a59cc6cc7103a415bc07df9ddc6ec
# Tue, 28 Sep 2021 02:34:53 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 28 Sep 2021 02:34:54 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 28 Sep 2021 02:34:54 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 28 Sep 2021 02:34:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 28 Sep 2021 02:34:54 GMT
USER memcache
# Tue, 28 Sep 2021 02:34:54 GMT
EXPOSE 11211
# Tue, 28 Sep 2021 02:34:55 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:7cfe208f95c1b63305981b069795676fa149e7115b9044c241ee45ef4aaf0bb3`  
		Last Modified: Tue, 28 Sep 2021 01:49:36 GMT  
		Size: 25.8 MB (25760871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff755a70833a769c5a32cb251e86ac9aa6ae1dce7f547dc1bef874a22855b63d`  
		Last Modified: Tue, 28 Sep 2021 02:35:52 GMT  
		Size: 5.0 KB (5022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d08a7a4b96e17b9ef0eb0b8dd97ad0dc3d75227841b6374b7071e7989d9fed3c`  
		Last Modified: Tue, 28 Sep 2021 02:35:52 GMT  
		Size: 1.9 MB (1887230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4b9662cd31c943100c81ad7c951195bf462ad510ed53de50144b8617d870a84`  
		Last Modified: Tue, 28 Sep 2021 02:35:52 GMT  
		Size: 1.3 MB (1272226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fc50167475bec35471f2d4f925c2d427f3757ac01cd3f8f82cc5685771c2744`  
		Last Modified: Tue, 28 Sep 2021 02:35:52 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c69d6c53bee775bfd205e1d0426724cebf2eddd3034e82681311e18028641c25`  
		Last Modified: Tue, 28 Sep 2021 02:35:52 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:1.6.10`

```console
$ docker pull memcached@sha256:0507080446e022bbcb398fef743f5479d61569f2992beccd200033e037968511
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

### `memcached:1.6.10` - linux; amd64

```console
$ docker pull memcached@sha256:b93ad58a06f215580205490133ce2165fa69f1930b964e890981f629df497e84
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.6 MB (30631755 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:444d9869f3507356b3fb6ffb7ed74ffc3be04be873a6876423c24d17acbf1128`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 03 Sep 2021 01:21:46 GMT
ADD file:4ff85d9f6aa246746912db62dea02eb71750474bb29611e770516a1fcd217add in / 
# Fri, 03 Sep 2021 01:21:46 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 07:33:54 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Fri, 03 Sep 2021 07:34:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 07:34:01 GMT
ENV MEMCACHED_VERSION=1.6.10
# Fri, 03 Sep 2021 07:34:01 GMT
ENV MEMCACHED_SHA1=cb5b9fe77a2a59cc6cc7103a415bc07df9ddc6ec
# Fri, 03 Sep 2021 07:38:24 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Fri, 03 Sep 2021 07:38:24 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 03 Sep 2021 07:38:25 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 03 Sep 2021 07:38:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 03 Sep 2021 07:38:25 GMT
USER memcache
# Fri, 03 Sep 2021 07:38:26 GMT
EXPOSE 11211
# Fri, 03 Sep 2021 07:38:26 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:a330b6cecb98cd2425fd25fce36669073f593b3176b4ee14731e48c05d678cdd`  
		Last Modified: Fri, 03 Sep 2021 01:28:19 GMT  
		Size: 27.1 MB (27145844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7dcde8d481fe08e2bab1fc8a1dc0e30c1d8cc9647d2867a6bc06942de810d56`  
		Last Modified: Fri, 03 Sep 2021 07:38:54 GMT  
		Size: 5.0 KB (4981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c3e0b65008f095303aa1ff733845d2eed7b3836fad196bc16533b3420711745`  
		Last Modified: Fri, 03 Sep 2021 07:38:54 GMT  
		Size: 2.2 MB (2197580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ad3eb30b171e7b0c33373bdeb39dfc36b63b8ec501af75bae3d4a964872f042`  
		Last Modified: Fri, 03 Sep 2021 07:38:54 GMT  
		Size: 1.3 MB (1282944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e6e03de9a5467b70b4d10bf021740a05eea1aeebfd87864b4a9289df9cb64c0`  
		Last Modified: Fri, 03 Sep 2021 07:38:54 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe0025a339764c7acc0034c701ca2b443e0b1803745c41094ea54289f754a81c`  
		Last Modified: Fri, 03 Sep 2021 07:38:54 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.10` - linux; arm variant v5

```console
$ docker pull memcached@sha256:5e1d0b6ce4b1b257e47c484709733908552416681c8f054bc97735e5ec114fa2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.0 MB (28036699 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd9fb75ae310df2e536d3a10e6dd9222317f89456fe6082c139b112849e5081b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 03 Sep 2021 00:51:26 GMT
ADD file:350748a564076da397b991745cd42e0688d15c72b9fd5c81f8ea0bb8938a2b3d in / 
# Fri, 03 Sep 2021 00:51:27 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 02:24:47 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Fri, 03 Sep 2021 02:24:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 02:24:58 GMT
ENV MEMCACHED_VERSION=1.6.10
# Fri, 03 Sep 2021 02:24:59 GMT
ENV MEMCACHED_SHA1=cb5b9fe77a2a59cc6cc7103a415bc07df9ddc6ec
# Fri, 03 Sep 2021 02:29:11 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Fri, 03 Sep 2021 02:29:12 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 03 Sep 2021 02:29:13 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 03 Sep 2021 02:29:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 03 Sep 2021 02:29:14 GMT
USER memcache
# Fri, 03 Sep 2021 02:29:14 GMT
EXPOSE 11211
# Fri, 03 Sep 2021 02:29:15 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:b019db4b5197128481d48d92ecacd6bb356c027a3d08393f6567a6fa183ba769`  
		Last Modified: Fri, 03 Sep 2021 01:07:12 GMT  
		Size: 24.9 MB (24879114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4faeba39e66674ac57454c2edb8018a9a29475db4893acb59bf00e84e5c4e88a`  
		Last Modified: Fri, 03 Sep 2021 02:30:10 GMT  
		Size: 4.9 KB (4895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b39e5da0381154e8db96921f6038b79a61f458bf76f9fdaae0d3f44b2d81f184`  
		Last Modified: Fri, 03 Sep 2021 02:30:11 GMT  
		Size: 1.9 MB (1897972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb47be4e43a9bfad0082a507b5885f22b4104821defe786af5237a6b48211a71`  
		Last Modified: Fri, 03 Sep 2021 02:30:11 GMT  
		Size: 1.3 MB (1254312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee01c0ace3ff5a5a86664234d47a50480b12f50f1390f5b78ab2b76a73e3346f`  
		Last Modified: Fri, 03 Sep 2021 02:30:10 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:240af99f2a1c8953e4436d48b387f4aa33defc9e83416c71f2d67d05c2a8cb48`  
		Last Modified: Fri, 03 Sep 2021 02:30:10 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.10` - linux; arm variant v7

```console
$ docker pull memcached@sha256:ee3f4a07ff534651238a464f5b0a3b582facdc9784f9e0f9a5bcd0128762da4f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.8 MB (25788867 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6222a822647e49fef3f296a084e4504bd705efe8e0649bc91541e03b8a5d7b8a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 03 Sep 2021 01:00:40 GMT
ADD file:4754bbccf4c59f77dd54f3888871f0635a2f9655cda53f50e63237f1580286e0 in / 
# Fri, 03 Sep 2021 01:00:41 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 06:44:19 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Fri, 03 Sep 2021 06:44:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 06:44:29 GMT
ENV MEMCACHED_VERSION=1.6.10
# Fri, 03 Sep 2021 06:44:30 GMT
ENV MEMCACHED_SHA1=cb5b9fe77a2a59cc6cc7103a415bc07df9ddc6ec
# Fri, 03 Sep 2021 06:48:21 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Fri, 03 Sep 2021 06:48:22 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 03 Sep 2021 06:48:23 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 03 Sep 2021 06:48:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 03 Sep 2021 06:48:24 GMT
USER memcache
# Fri, 03 Sep 2021 06:48:25 GMT
EXPOSE 11211
# Fri, 03 Sep 2021 06:48:25 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:2215ad7863d95c38f1f794f1d5b4d6c5ca4ca7e921e4bb7218b803f7ed270675`  
		Last Modified: Fri, 03 Sep 2021 01:16:23 GMT  
		Size: 22.7 MB (22746151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d554d32fa680ffcf04f8b509fa6a16e796fadc0ecf8db8c48bcc2a911f9f4591`  
		Last Modified: Fri, 03 Sep 2021 07:00:56 GMT  
		Size: 4.9 KB (4895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a550041e12d651682f2b70b45620898d8cebd97f4b4b3469aaeac8d452a76ef`  
		Last Modified: Fri, 03 Sep 2021 07:00:56 GMT  
		Size: 1.8 MB (1812490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ae1581582d0b08a4635fe57247a454da856fea52ec988126ee4f2f1781b7acd`  
		Last Modified: Fri, 03 Sep 2021 07:00:56 GMT  
		Size: 1.2 MB (1224925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:678c3e64de445bdc9a420655f01c8abab5f2e7ef4f41d441e6d2310ea2c36de5`  
		Last Modified: Fri, 03 Sep 2021 07:00:55 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a21b13a7b8549e46debb4d9b1117211df9edcc02f822ec99d1fe1b4278f1e56`  
		Last Modified: Fri, 03 Sep 2021 07:00:55 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.10` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:57e906b2282c3e67137cc8c2ab5148c8e748256b2e3934c5b7ecd77a6a186de5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.3 MB (29250783 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:932f1c94fc6e8e017820dcb97fe4b624efacba7409cb99c99a369c649b03829d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 03 Sep 2021 00:40:58 GMT
ADD file:4a1d7f2d989aee6bd83da076b6e9dd3da2da97cf5654bd37568e9baec30ac4b1 in / 
# Fri, 03 Sep 2021 00:40:58 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 02:46:23 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Fri, 03 Sep 2021 02:46:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 02:46:27 GMT
ENV MEMCACHED_VERSION=1.6.10
# Fri, 03 Sep 2021 02:46:28 GMT
ENV MEMCACHED_SHA1=cb5b9fe77a2a59cc6cc7103a415bc07df9ddc6ec
# Fri, 03 Sep 2021 02:50:03 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Fri, 03 Sep 2021 02:50:03 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 03 Sep 2021 02:50:04 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 03 Sep 2021 02:50:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 03 Sep 2021 02:50:04 GMT
USER memcache
# Fri, 03 Sep 2021 02:50:05 GMT
EXPOSE 11211
# Fri, 03 Sep 2021 02:50:05 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:d10c227306ce3db344a8399cbc02bbf0dcb36519318efbde3c6027c00be8b40e`  
		Last Modified: Fri, 03 Sep 2021 00:49:47 GMT  
		Size: 25.9 MB (25914860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee708d85ae4c6929688ee243da330a395c81a5da3913f7aaaeea88283b5752b1`  
		Last Modified: Fri, 03 Sep 2021 02:51:01 GMT  
		Size: 5.0 KB (5024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41eee23f132aa5ef6810f141bd4852d174eb68bd5e9f8fc4e278e2fc55f7cea8`  
		Last Modified: Fri, 03 Sep 2021 02:51:02 GMT  
		Size: 2.1 MB (2075717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d9a7819a72ed1b598aabafd5ac9be7be62ac6b085cc30dbda97ef193641fc05`  
		Last Modified: Fri, 03 Sep 2021 02:51:01 GMT  
		Size: 1.3 MB (1254776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ae146d1bf5917e1fb0f4aa46a655feefc0ec5e00ef4e775beed00fa6a1d0aa1`  
		Last Modified: Fri, 03 Sep 2021 02:51:01 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3cae1f92b0ec75c4c83b4b5a4ce47b455952d638c215f1588a20af7261fba5b`  
		Last Modified: Fri, 03 Sep 2021 02:51:01 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.10` - linux; 386

```console
$ docker pull memcached@sha256:221d230cb426e233ce34c9669663db5628d85a6ffe1d98292cfb54d66a7e1f8a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.3 MB (31292631 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7283abe72dd41573bd7262a0ba163f6ef7ddf757bc5178c95eea585f8335e784`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 03 Sep 2021 00:40:24 GMT
ADD file:6bf4b6f4aa28306610ef10c68f422a7210ff2fbd5345cec07bc5f76d54a4c8bc in / 
# Fri, 03 Sep 2021 00:40:24 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 06:44:15 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Fri, 03 Sep 2021 06:44:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 06:44:21 GMT
ENV MEMCACHED_VERSION=1.6.10
# Fri, 03 Sep 2021 06:44:21 GMT
ENV MEMCACHED_SHA1=cb5b9fe77a2a59cc6cc7103a415bc07df9ddc6ec
# Fri, 03 Sep 2021 06:48:23 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Fri, 03 Sep 2021 06:48:24 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 03 Sep 2021 06:48:25 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 03 Sep 2021 06:48:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 03 Sep 2021 06:48:26 GMT
USER memcache
# Fri, 03 Sep 2021 06:48:26 GMT
EXPOSE 11211
# Fri, 03 Sep 2021 06:48:26 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:7e87f600658a0c0d3bd8b82b9c645b5ec2763492ec627c1c1c1183c2ad3c45d5`  
		Last Modified: Fri, 03 Sep 2021 00:49:06 GMT  
		Size: 27.8 MB (27797513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9454a8c8c54135f6e7f591277550407671a2a183d0ea7a1b04e0b7bf1ecfeb39`  
		Last Modified: Fri, 03 Sep 2021 06:49:32 GMT  
		Size: 4.9 KB (4895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4900dba329569a63986180bc83b94449c1dffc3a804c2910a2a3f288509964d3`  
		Last Modified: Fri, 03 Sep 2021 06:49:32 GMT  
		Size: 2.2 MB (2209620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb8624563e6585b031c874cc180ee08148f5773238b0bc1571feb1b64b198ee5`  
		Last Modified: Fri, 03 Sep 2021 06:49:32 GMT  
		Size: 1.3 MB (1280199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86f15c6c59e3205f04fba85035da98cd62d3f67bca6baa035b56db7f4f5dfb5c`  
		Last Modified: Fri, 03 Sep 2021 06:49:32 GMT  
		Size: 283.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f1b51c6ca8d549a8b18622d1c15504b94257295420bc332544f8d9026fff6f3`  
		Last Modified: Fri, 03 Sep 2021 06:49:32 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.10` - linux; mips64le

```console
$ docker pull memcached@sha256:33ce4398cd07967870c76b95ec5314cbe8280d564309b25d0640e8dd94cb7198
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.9 MB (28866865 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cc3e459293995ad1867b805e319ebb5b3942502abbad00cf3f9b3a4ccc26c740`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 28 Sep 2021 02:11:41 GMT
ADD file:df525c65bc60141f19ab937525d724c6d29cac53beb30f92d79ea4b2edf5a13e in / 
# Tue, 28 Sep 2021 02:11:41 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 02:51:00 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 28 Sep 2021 02:51:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:51:13 GMT
ENV MEMCACHED_VERSION=1.6.10
# Tue, 28 Sep 2021 02:51:13 GMT
ENV MEMCACHED_SHA1=cb5b9fe77a2a59cc6cc7103a415bc07df9ddc6ec
# Tue, 28 Sep 2021 02:56:56 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 28 Sep 2021 02:56:56 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 28 Sep 2021 02:56:58 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 28 Sep 2021 02:56:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 28 Sep 2021 02:56:59 GMT
USER memcache
# Tue, 28 Sep 2021 02:56:59 GMT
EXPOSE 11211
# Tue, 28 Sep 2021 02:56:59 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:f1b3d9dde862ddf88a05cec47ce54e641c4057c7bfb377e2a065c72a42a76321`  
		Last Modified: Tue, 28 Sep 2021 02:22:07 GMT  
		Size: 25.8 MB (25813001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e684588e988c227c0fedbcfeb8361e35b75eaa06e38cf8207979b491712d3dc`  
		Last Modified: Tue, 28 Sep 2021 02:57:18 GMT  
		Size: 5.0 KB (4981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35a3bc6181fe53d4bf46e98ebace046f2014668d601c2c3975c3dc6fc655acbc`  
		Last Modified: Tue, 28 Sep 2021 02:57:19 GMT  
		Size: 1.8 MB (1777273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f49b3d8a270ebba87297e2461fe81567f28a880e22d7ef977a60930ad82d6aa6`  
		Last Modified: Tue, 28 Sep 2021 02:57:19 GMT  
		Size: 1.3 MB (1271204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:119de6bb61edbff9dc8919b6bbb0f35c144a065c899d3fe20127480e2985c0d8`  
		Last Modified: Tue, 28 Sep 2021 02:57:18 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ecffae4c1838eb68ee866feaae4a6357c6198f1e86b5a1719bd7646795396d6`  
		Last Modified: Tue, 28 Sep 2021 02:57:18 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.10` - linux; ppc64le

```console
$ docker pull memcached@sha256:49728dba09507cb74bbfae419b5b8051106768fd3b53aa7964da2b4a7cf0d44f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.2 MB (34190787 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4563ba0117902a70591f2170ab90e34de0431ae24402ee05aa741d4eafbd036f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 03 Sep 2021 01:24:33 GMT
ADD file:6c1662ddb92232ae8969a86a18dacab97b3b5792a1ecda49e6ac741a1a5c878c in / 
# Fri, 03 Sep 2021 01:24:41 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 08:06:59 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Fri, 03 Sep 2021 08:07:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 08:07:23 GMT
ENV MEMCACHED_VERSION=1.6.10
# Fri, 03 Sep 2021 08:07:26 GMT
ENV MEMCACHED_SHA1=cb5b9fe77a2a59cc6cc7103a415bc07df9ddc6ec
# Fri, 03 Sep 2021 08:13:31 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Fri, 03 Sep 2021 08:13:32 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 03 Sep 2021 08:13:43 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 03 Sep 2021 08:13:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 03 Sep 2021 08:13:57 GMT
USER memcache
# Fri, 03 Sep 2021 08:14:01 GMT
EXPOSE 11211
# Fri, 03 Sep 2021 08:14:05 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:8258146296247df1f308a336d4abf286afae14e3375edefb87a091e80745e29f`  
		Last Modified: Fri, 03 Sep 2021 01:39:45 GMT  
		Size: 30.6 MB (30553675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2f96132a11c70c50168ade17294cf7e8c919db231f87a28818170d9917a3268`  
		Last Modified: Fri, 03 Sep 2021 08:14:54 GMT  
		Size: 5.0 KB (4988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:973046a9e11e4bf003ce0e9688dc396e6e0ded760e9914a57132e130fa64289a`  
		Last Modified: Fri, 03 Sep 2021 08:14:55 GMT  
		Size: 2.3 MB (2323873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e5495ff67177662caa9f0459d68cb0641f32eddb666f4238634e357e58bdad1`  
		Last Modified: Fri, 03 Sep 2021 08:14:55 GMT  
		Size: 1.3 MB (1307845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b406b4303f1d8fe163586ca2e7abe3639c752a524f2c44e46677c01e36f937c`  
		Last Modified: Fri, 03 Sep 2021 08:14:54 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ff817a29aac3d654f6e919cbea3ea8125cce972e357c595217ec95807e07c3d`  
		Last Modified: Fri, 03 Sep 2021 08:14:54 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.10` - linux; s390x

```console
$ docker pull memcached@sha256:53459c6f3d42b7b718e1ccbb3090ff35e649d8d005fa1917cee1ee1fbfea608a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.9 MB (28925755 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8831bffed7f4d435dd3c714d24529fea34f84468cbc5abec57feeb4728059de`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 28 Sep 2021 01:43:29 GMT
ADD file:118e7a596407435b5e2ff0aae6bb9bff3b66000c91ca37bfe1eeb98c23d99d49 in / 
# Tue, 28 Sep 2021 01:43:30 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 02:31:35 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 28 Sep 2021 02:31:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:31:39 GMT
ENV MEMCACHED_VERSION=1.6.10
# Tue, 28 Sep 2021 02:31:39 GMT
ENV MEMCACHED_SHA1=cb5b9fe77a2a59cc6cc7103a415bc07df9ddc6ec
# Tue, 28 Sep 2021 02:34:53 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 28 Sep 2021 02:34:54 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 28 Sep 2021 02:34:54 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 28 Sep 2021 02:34:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 28 Sep 2021 02:34:54 GMT
USER memcache
# Tue, 28 Sep 2021 02:34:54 GMT
EXPOSE 11211
# Tue, 28 Sep 2021 02:34:55 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:7cfe208f95c1b63305981b069795676fa149e7115b9044c241ee45ef4aaf0bb3`  
		Last Modified: Tue, 28 Sep 2021 01:49:36 GMT  
		Size: 25.8 MB (25760871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff755a70833a769c5a32cb251e86ac9aa6ae1dce7f547dc1bef874a22855b63d`  
		Last Modified: Tue, 28 Sep 2021 02:35:52 GMT  
		Size: 5.0 KB (5022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d08a7a4b96e17b9ef0eb0b8dd97ad0dc3d75227841b6374b7071e7989d9fed3c`  
		Last Modified: Tue, 28 Sep 2021 02:35:52 GMT  
		Size: 1.9 MB (1887230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4b9662cd31c943100c81ad7c951195bf462ad510ed53de50144b8617d870a84`  
		Last Modified: Tue, 28 Sep 2021 02:35:52 GMT  
		Size: 1.3 MB (1272226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fc50167475bec35471f2d4f925c2d427f3757ac01cd3f8f82cc5685771c2744`  
		Last Modified: Tue, 28 Sep 2021 02:35:52 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c69d6c53bee775bfd205e1d0426724cebf2eddd3034e82681311e18028641c25`  
		Last Modified: Tue, 28 Sep 2021 02:35:52 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:1.6.10-alpine`

```console
$ docker pull memcached@sha256:d57531b1d9bfffc9ada8c669fe761da3c7f9a15b9ac27d0f383e318d40f90e0d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `memcached:1.6.10-alpine` - linux; amd64

```console
$ docker pull memcached@sha256:67d93d2efc4859c0b2e5a24bc13e759788c1f28d97a4d68b58a3de323e8ccb38
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3904613 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec200929117689b8cbba5a24fe5e892d7e4bfec5b654cef54958801a6ab9e92b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Fri, 27 Aug 2021 20:39:15 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Fri, 27 Aug 2021 20:39:16 GMT
RUN apk add --no-cache libsasl
# Fri, 27 Aug 2021 20:39:16 GMT
ENV MEMCACHED_VERSION=1.6.10
# Fri, 27 Aug 2021 20:39:17 GMT
ENV MEMCACHED_SHA1=cb5b9fe77a2a59cc6cc7103a415bc07df9ddc6ec
# Fri, 27 Aug 2021 20:43:47 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Fri, 27 Aug 2021 20:43:47 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 27 Aug 2021 20:43:49 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 27 Aug 2021 20:43:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 Aug 2021 20:43:50 GMT
USER memcache
# Fri, 27 Aug 2021 20:43:50 GMT
EXPOSE 11211
# Fri, 27 Aug 2021 20:43:50 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:a0d0a0d46f8b52473982a3c466318f479767577551a53ffc9074c9fa7035982e`  
		Last Modified: Fri, 27 Aug 2021 17:20:13 GMT  
		Size: 2.8 MB (2814446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84db6e403c6f8cdc8217536fa7d8bb9bbee66a7a49106104b3ceeace758e887b`  
		Last Modified: Fri, 27 Aug 2021 20:44:26 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7430c0d88cc6cc6389bb62e421f43031b009d21243f7362290bcf11b82e9e967`  
		Last Modified: Fri, 27 Aug 2021 20:44:26 GMT  
		Size: 155.5 KB (155516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3919afa4c767ba881b469a2798f6ad270dc23bbd9174d2994a0208bf508febba`  
		Last Modified: Fri, 27 Aug 2021 20:44:26 GMT  
		Size: 933.0 KB (932979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e81a6f988f7ee7ae5df06403e582d0edb09dcd73e81bacdaa17d1e0da71e13b`  
		Last Modified: Fri, 27 Aug 2021 20:44:26 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d5ed3d833f3ab3255decd4fc642f2368e6791acc470e40c2f3eb7463b7351dc`  
		Last Modified: Fri, 27 Aug 2021 20:44:26 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.10-alpine` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:8ed70173927cd66ad4e1bac9803ba7114502646685f70abb395ef668a46db5fb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3793233 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c5c3d9ec3f6b46ae9e7305a3958b059ffc7d935b5f2094e78973054a0394060e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 27 Aug 2021 17:39:33 GMT
ADD file:dc8af9c7bfe9f9541e1db38dea01c4201609f3075b31e108f2073ffed8c5e4b9 in / 
# Fri, 27 Aug 2021 17:39:33 GMT
CMD ["/bin/sh"]
# Fri, 27 Aug 2021 20:15:01 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Fri, 27 Aug 2021 20:15:02 GMT
RUN apk add --no-cache libsasl
# Fri, 27 Aug 2021 20:15:02 GMT
ENV MEMCACHED_VERSION=1.6.10
# Fri, 27 Aug 2021 20:15:02 GMT
ENV MEMCACHED_SHA1=cb5b9fe77a2a59cc6cc7103a415bc07df9ddc6ec
# Fri, 27 Aug 2021 20:18:55 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Fri, 27 Aug 2021 20:18:55 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 27 Aug 2021 20:18:56 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 27 Aug 2021 20:18:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 Aug 2021 20:18:56 GMT
USER memcache
# Fri, 27 Aug 2021 20:18:56 GMT
EXPOSE 11211
# Fri, 27 Aug 2021 20:18:56 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:552d1f2373af9bfe12033568ebbfb0ccbb0de11279f9a415a29207e264d7f4d9`  
		Last Modified: Fri, 27 Aug 2021 17:40:18 GMT  
		Size: 2.7 MB (2711827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ab312377ca26aa6df3e0bb8b11a63d6964544ffd2552b8e7cebb0acbbc3036d`  
		Last Modified: Fri, 27 Aug 2021 20:19:53 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a538168cab1a5c606dfa94dd8b09de5598c9071505476146fa99500011f8e7f5`  
		Last Modified: Fri, 27 Aug 2021 20:19:53 GMT  
		Size: 157.2 KB (157194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae4e52b47025818dc222e8dcd9310ab3f3c757a434fb786d7100cfaef304d4ed`  
		Last Modified: Fri, 27 Aug 2021 20:19:53 GMT  
		Size: 922.5 KB (922539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bedcb7a468e2a54e811d3ab62759e10500ea8b580eb12a600991eb1a3eed136`  
		Last Modified: Fri, 27 Aug 2021 20:19:53 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50b5ad9ab615a8b63e96efab0f2b3b2ff0a60abcb13a2529437f46368a641c6e`  
		Last Modified: Fri, 27 Aug 2021 20:19:53 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.10-alpine` - linux; 386

```console
$ docker pull memcached@sha256:82a99c470435ce9fd7cebf6565305c9f9a20eb2142839f8a7eaf42fc04b1e64a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3937988 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:503d28ddbe03b1e33458c354e3e0cef3142579c20bdf6e8c1f4b447257a2de01`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 27 Aug 2021 17:38:29 GMT
ADD file:42a7bc5a08b546b47049dd0f89ae4e7a8c86342f87000f39ade3ff52916a6c2e in / 
# Fri, 27 Aug 2021 17:38:30 GMT
CMD ["/bin/sh"]
# Fri, 27 Aug 2021 19:48:52 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Fri, 27 Aug 2021 19:48:54 GMT
RUN apk add --no-cache libsasl
# Fri, 27 Aug 2021 19:48:54 GMT
ENV MEMCACHED_VERSION=1.6.10
# Fri, 27 Aug 2021 19:48:55 GMT
ENV MEMCACHED_SHA1=cb5b9fe77a2a59cc6cc7103a415bc07df9ddc6ec
# Fri, 27 Aug 2021 19:53:36 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Fri, 27 Aug 2021 19:53:36 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 27 Aug 2021 19:53:37 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 27 Aug 2021 19:53:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 Aug 2021 19:53:38 GMT
USER memcache
# Fri, 27 Aug 2021 19:53:38 GMT
EXPOSE 11211
# Fri, 27 Aug 2021 19:53:38 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:b11ae9fc5d8a106cfed3a6f6c75e5b5b5797c566fac4411622b4055df6541286`  
		Last Modified: Fri, 27 Aug 2021 17:39:18 GMT  
		Size: 2.8 MB (2822857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a776c6c02658f2d17623bce57a634d82f2dc8c8bee59f4d90fc786c3e69e31ff`  
		Last Modified: Fri, 27 Aug 2021 19:54:35 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fab8279289e8b7a476ce09017d9bcdb33bccbe04750f2ccba41c0a43f828b16`  
		Last Modified: Fri, 27 Aug 2021 19:54:35 GMT  
		Size: 169.0 KB (169012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24c50e3cfd5d1f42d6dd2505b7b02ca2ed14cb53d2199df2bed319e84146d13b`  
		Last Modified: Fri, 27 Aug 2021 19:54:36 GMT  
		Size: 944.4 KB (944446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3856e8e8dfa799b89d86a7552466e0b451bc8b8b140b56d53056ea942b82b102`  
		Last Modified: Fri, 27 Aug 2021 19:54:35 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bd1d4e4fe24a075a95e91ec623e250fb1071d34af2ec3a777ceecca3d62ea9f`  
		Last Modified: Fri, 27 Aug 2021 19:54:35 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.10-alpine` - linux; ppc64le

```console
$ docker pull memcached@sha256:5ea0c2672938efeae9c4cf8a45bdb1a06eaacb2f1014ed8fef3d3c6339b3fac5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.0 MB (3954868 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e20a2c1b753cc0bb4b19ca80b7d333dcbb37ce0a77e99c1b96ef27b09b680fa7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 27 Aug 2021 19:39:54 GMT
ADD file:d213c56ffc24a5051e8060fd0fec1a0520367c10d88ab16321c36336b6c66098 in / 
# Fri, 27 Aug 2021 19:39:59 GMT
CMD ["/bin/sh"]
# Sat, 28 Aug 2021 02:52:59 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Sat, 28 Aug 2021 02:53:08 GMT
RUN apk add --no-cache libsasl
# Sat, 28 Aug 2021 02:53:10 GMT
ENV MEMCACHED_VERSION=1.6.10
# Sat, 28 Aug 2021 02:53:12 GMT
ENV MEMCACHED_SHA1=cb5b9fe77a2a59cc6cc7103a415bc07df9ddc6ec
# Sat, 28 Aug 2021 02:56:38 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Sat, 28 Aug 2021 02:56:40 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Sat, 28 Aug 2021 02:56:47 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Sat, 28 Aug 2021 02:56:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 28 Aug 2021 02:56:57 GMT
USER memcache
# Sat, 28 Aug 2021 02:57:02 GMT
EXPOSE 11211
# Sat, 28 Aug 2021 02:57:09 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:63da8ca98f7b4b94381aed56862a60aecf355d9428b9aeb7c61d5bd017100c18`  
		Last Modified: Fri, 27 Aug 2021 19:41:06 GMT  
		Size: 2.8 MB (2812284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a54fbc6ddd30fadabd2cf34600dd72918de6e611345c8202b6cd56a411467659`  
		Last Modified: Sat, 28 Aug 2021 02:58:02 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdd08b1afa1a2e02df391d85b3cfccf552f50b91046d9eafbe19feffb2f58910`  
		Last Modified: Sat, 28 Aug 2021 02:58:02 GMT  
		Size: 179.7 KB (179652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d214dccc5e7f55ecf8e9ec4471487fa0f6ba5ba2e84a3c746ff458410a29c755`  
		Last Modified: Sat, 28 Aug 2021 02:58:02 GMT  
		Size: 961.3 KB (961258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a6ae8b6fa12461573aab65c6be736cd4668463495c569d1113861ff729fb89f`  
		Last Modified: Sat, 28 Aug 2021 02:58:02 GMT  
		Size: 283.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fef62e61ad65fab7f854dd8a0a437b4ed6853b4186a9639a41ac47dae3f7d9e`  
		Last Modified: Sat, 28 Aug 2021 02:58:02 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.10-alpine` - linux; s390x

```console
$ docker pull memcached@sha256:cebdf9f1ff4ffe7551d4917b4a53e78ac48da41a694a8301fbd92459ebd9f45f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.7 MB (3695912 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:047503017563255821d3a05e00a220624c8698ef1a285eb6a05023ef0c1335e4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 27 Aug 2021 17:41:29 GMT
ADD file:9b40ee281e8797067fb2ae207c406084cb81593090338a8b7cb09ade52168daa in / 
# Fri, 27 Aug 2021 17:41:30 GMT
CMD ["/bin/sh"]
# Fri, 27 Aug 2021 19:13:56 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Fri, 27 Aug 2021 19:13:58 GMT
RUN apk add --no-cache libsasl
# Fri, 27 Aug 2021 19:13:59 GMT
ENV MEMCACHED_VERSION=1.6.10
# Fri, 27 Aug 2021 19:13:59 GMT
ENV MEMCACHED_SHA1=cb5b9fe77a2a59cc6cc7103a415bc07df9ddc6ec
# Fri, 27 Aug 2021 19:22:03 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Fri, 27 Aug 2021 19:22:04 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 27 Aug 2021 19:22:05 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 27 Aug 2021 19:22:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 Aug 2021 19:22:06 GMT
USER memcache
# Fri, 27 Aug 2021 19:22:06 GMT
EXPOSE 11211
# Fri, 27 Aug 2021 19:22:07 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:da14cb6b6dc946dbb2d84386bcaca84e2d46f650767cd11bdb3331ec9d623988`  
		Last Modified: Fri, 27 Aug 2021 17:42:25 GMT  
		Size: 2.6 MB (2603464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5c3123815589d4cfc45a071f344bd0f3ca08ee63a471c2c114af2dece4699a0`  
		Last Modified: Fri, 27 Aug 2021 19:23:06 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d25c400e2d4eb8dee97bc754e9e52585af4304ec8cf3121b619bd5756796fb52`  
		Last Modified: Fri, 27 Aug 2021 19:23:06 GMT  
		Size: 161.5 KB (161520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:611fd541e530a5444852c1a56f01565817097a4b2abec64399dcf4fdd84dfe88`  
		Last Modified: Fri, 27 Aug 2021 19:23:06 GMT  
		Size: 929.3 KB (929257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cb82aed96a5a46fb2399db9bf85a3ff9a7ce3de3468fe74285ad84fd557a1ca`  
		Last Modified: Fri, 27 Aug 2021 19:23:06 GMT  
		Size: 283.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c18159f487fe568305c6aaeb29b07af5f859402bb29566a404f9fccbd86bafbf`  
		Last Modified: Fri, 27 Aug 2021 19:23:06 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:1.6.10-alpine3.14`

```console
$ docker pull memcached@sha256:d57531b1d9bfffc9ada8c669fe761da3c7f9a15b9ac27d0f383e318d40f90e0d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `memcached:1.6.10-alpine3.14` - linux; amd64

```console
$ docker pull memcached@sha256:67d93d2efc4859c0b2e5a24bc13e759788c1f28d97a4d68b58a3de323e8ccb38
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3904613 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec200929117689b8cbba5a24fe5e892d7e4bfec5b654cef54958801a6ab9e92b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Fri, 27 Aug 2021 20:39:15 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Fri, 27 Aug 2021 20:39:16 GMT
RUN apk add --no-cache libsasl
# Fri, 27 Aug 2021 20:39:16 GMT
ENV MEMCACHED_VERSION=1.6.10
# Fri, 27 Aug 2021 20:39:17 GMT
ENV MEMCACHED_SHA1=cb5b9fe77a2a59cc6cc7103a415bc07df9ddc6ec
# Fri, 27 Aug 2021 20:43:47 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Fri, 27 Aug 2021 20:43:47 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 27 Aug 2021 20:43:49 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 27 Aug 2021 20:43:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 Aug 2021 20:43:50 GMT
USER memcache
# Fri, 27 Aug 2021 20:43:50 GMT
EXPOSE 11211
# Fri, 27 Aug 2021 20:43:50 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:a0d0a0d46f8b52473982a3c466318f479767577551a53ffc9074c9fa7035982e`  
		Last Modified: Fri, 27 Aug 2021 17:20:13 GMT  
		Size: 2.8 MB (2814446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84db6e403c6f8cdc8217536fa7d8bb9bbee66a7a49106104b3ceeace758e887b`  
		Last Modified: Fri, 27 Aug 2021 20:44:26 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7430c0d88cc6cc6389bb62e421f43031b009d21243f7362290bcf11b82e9e967`  
		Last Modified: Fri, 27 Aug 2021 20:44:26 GMT  
		Size: 155.5 KB (155516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3919afa4c767ba881b469a2798f6ad270dc23bbd9174d2994a0208bf508febba`  
		Last Modified: Fri, 27 Aug 2021 20:44:26 GMT  
		Size: 933.0 KB (932979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e81a6f988f7ee7ae5df06403e582d0edb09dcd73e81bacdaa17d1e0da71e13b`  
		Last Modified: Fri, 27 Aug 2021 20:44:26 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d5ed3d833f3ab3255decd4fc642f2368e6791acc470e40c2f3eb7463b7351dc`  
		Last Modified: Fri, 27 Aug 2021 20:44:26 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.10-alpine3.14` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:8ed70173927cd66ad4e1bac9803ba7114502646685f70abb395ef668a46db5fb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3793233 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c5c3d9ec3f6b46ae9e7305a3958b059ffc7d935b5f2094e78973054a0394060e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 27 Aug 2021 17:39:33 GMT
ADD file:dc8af9c7bfe9f9541e1db38dea01c4201609f3075b31e108f2073ffed8c5e4b9 in / 
# Fri, 27 Aug 2021 17:39:33 GMT
CMD ["/bin/sh"]
# Fri, 27 Aug 2021 20:15:01 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Fri, 27 Aug 2021 20:15:02 GMT
RUN apk add --no-cache libsasl
# Fri, 27 Aug 2021 20:15:02 GMT
ENV MEMCACHED_VERSION=1.6.10
# Fri, 27 Aug 2021 20:15:02 GMT
ENV MEMCACHED_SHA1=cb5b9fe77a2a59cc6cc7103a415bc07df9ddc6ec
# Fri, 27 Aug 2021 20:18:55 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Fri, 27 Aug 2021 20:18:55 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 27 Aug 2021 20:18:56 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 27 Aug 2021 20:18:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 Aug 2021 20:18:56 GMT
USER memcache
# Fri, 27 Aug 2021 20:18:56 GMT
EXPOSE 11211
# Fri, 27 Aug 2021 20:18:56 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:552d1f2373af9bfe12033568ebbfb0ccbb0de11279f9a415a29207e264d7f4d9`  
		Last Modified: Fri, 27 Aug 2021 17:40:18 GMT  
		Size: 2.7 MB (2711827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ab312377ca26aa6df3e0bb8b11a63d6964544ffd2552b8e7cebb0acbbc3036d`  
		Last Modified: Fri, 27 Aug 2021 20:19:53 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a538168cab1a5c606dfa94dd8b09de5598c9071505476146fa99500011f8e7f5`  
		Last Modified: Fri, 27 Aug 2021 20:19:53 GMT  
		Size: 157.2 KB (157194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae4e52b47025818dc222e8dcd9310ab3f3c757a434fb786d7100cfaef304d4ed`  
		Last Modified: Fri, 27 Aug 2021 20:19:53 GMT  
		Size: 922.5 KB (922539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bedcb7a468e2a54e811d3ab62759e10500ea8b580eb12a600991eb1a3eed136`  
		Last Modified: Fri, 27 Aug 2021 20:19:53 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50b5ad9ab615a8b63e96efab0f2b3b2ff0a60abcb13a2529437f46368a641c6e`  
		Last Modified: Fri, 27 Aug 2021 20:19:53 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.10-alpine3.14` - linux; 386

```console
$ docker pull memcached@sha256:82a99c470435ce9fd7cebf6565305c9f9a20eb2142839f8a7eaf42fc04b1e64a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3937988 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:503d28ddbe03b1e33458c354e3e0cef3142579c20bdf6e8c1f4b447257a2de01`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 27 Aug 2021 17:38:29 GMT
ADD file:42a7bc5a08b546b47049dd0f89ae4e7a8c86342f87000f39ade3ff52916a6c2e in / 
# Fri, 27 Aug 2021 17:38:30 GMT
CMD ["/bin/sh"]
# Fri, 27 Aug 2021 19:48:52 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Fri, 27 Aug 2021 19:48:54 GMT
RUN apk add --no-cache libsasl
# Fri, 27 Aug 2021 19:48:54 GMT
ENV MEMCACHED_VERSION=1.6.10
# Fri, 27 Aug 2021 19:48:55 GMT
ENV MEMCACHED_SHA1=cb5b9fe77a2a59cc6cc7103a415bc07df9ddc6ec
# Fri, 27 Aug 2021 19:53:36 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Fri, 27 Aug 2021 19:53:36 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 27 Aug 2021 19:53:37 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 27 Aug 2021 19:53:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 Aug 2021 19:53:38 GMT
USER memcache
# Fri, 27 Aug 2021 19:53:38 GMT
EXPOSE 11211
# Fri, 27 Aug 2021 19:53:38 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:b11ae9fc5d8a106cfed3a6f6c75e5b5b5797c566fac4411622b4055df6541286`  
		Last Modified: Fri, 27 Aug 2021 17:39:18 GMT  
		Size: 2.8 MB (2822857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a776c6c02658f2d17623bce57a634d82f2dc8c8bee59f4d90fc786c3e69e31ff`  
		Last Modified: Fri, 27 Aug 2021 19:54:35 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fab8279289e8b7a476ce09017d9bcdb33bccbe04750f2ccba41c0a43f828b16`  
		Last Modified: Fri, 27 Aug 2021 19:54:35 GMT  
		Size: 169.0 KB (169012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24c50e3cfd5d1f42d6dd2505b7b02ca2ed14cb53d2199df2bed319e84146d13b`  
		Last Modified: Fri, 27 Aug 2021 19:54:36 GMT  
		Size: 944.4 KB (944446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3856e8e8dfa799b89d86a7552466e0b451bc8b8b140b56d53056ea942b82b102`  
		Last Modified: Fri, 27 Aug 2021 19:54:35 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bd1d4e4fe24a075a95e91ec623e250fb1071d34af2ec3a777ceecca3d62ea9f`  
		Last Modified: Fri, 27 Aug 2021 19:54:35 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.10-alpine3.14` - linux; ppc64le

```console
$ docker pull memcached@sha256:5ea0c2672938efeae9c4cf8a45bdb1a06eaacb2f1014ed8fef3d3c6339b3fac5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.0 MB (3954868 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e20a2c1b753cc0bb4b19ca80b7d333dcbb37ce0a77e99c1b96ef27b09b680fa7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 27 Aug 2021 19:39:54 GMT
ADD file:d213c56ffc24a5051e8060fd0fec1a0520367c10d88ab16321c36336b6c66098 in / 
# Fri, 27 Aug 2021 19:39:59 GMT
CMD ["/bin/sh"]
# Sat, 28 Aug 2021 02:52:59 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Sat, 28 Aug 2021 02:53:08 GMT
RUN apk add --no-cache libsasl
# Sat, 28 Aug 2021 02:53:10 GMT
ENV MEMCACHED_VERSION=1.6.10
# Sat, 28 Aug 2021 02:53:12 GMT
ENV MEMCACHED_SHA1=cb5b9fe77a2a59cc6cc7103a415bc07df9ddc6ec
# Sat, 28 Aug 2021 02:56:38 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Sat, 28 Aug 2021 02:56:40 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Sat, 28 Aug 2021 02:56:47 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Sat, 28 Aug 2021 02:56:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 28 Aug 2021 02:56:57 GMT
USER memcache
# Sat, 28 Aug 2021 02:57:02 GMT
EXPOSE 11211
# Sat, 28 Aug 2021 02:57:09 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:63da8ca98f7b4b94381aed56862a60aecf355d9428b9aeb7c61d5bd017100c18`  
		Last Modified: Fri, 27 Aug 2021 19:41:06 GMT  
		Size: 2.8 MB (2812284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a54fbc6ddd30fadabd2cf34600dd72918de6e611345c8202b6cd56a411467659`  
		Last Modified: Sat, 28 Aug 2021 02:58:02 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdd08b1afa1a2e02df391d85b3cfccf552f50b91046d9eafbe19feffb2f58910`  
		Last Modified: Sat, 28 Aug 2021 02:58:02 GMT  
		Size: 179.7 KB (179652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d214dccc5e7f55ecf8e9ec4471487fa0f6ba5ba2e84a3c746ff458410a29c755`  
		Last Modified: Sat, 28 Aug 2021 02:58:02 GMT  
		Size: 961.3 KB (961258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a6ae8b6fa12461573aab65c6be736cd4668463495c569d1113861ff729fb89f`  
		Last Modified: Sat, 28 Aug 2021 02:58:02 GMT  
		Size: 283.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fef62e61ad65fab7f854dd8a0a437b4ed6853b4186a9639a41ac47dae3f7d9e`  
		Last Modified: Sat, 28 Aug 2021 02:58:02 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.10-alpine3.14` - linux; s390x

```console
$ docker pull memcached@sha256:cebdf9f1ff4ffe7551d4917b4a53e78ac48da41a694a8301fbd92459ebd9f45f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.7 MB (3695912 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:047503017563255821d3a05e00a220624c8698ef1a285eb6a05023ef0c1335e4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 27 Aug 2021 17:41:29 GMT
ADD file:9b40ee281e8797067fb2ae207c406084cb81593090338a8b7cb09ade52168daa in / 
# Fri, 27 Aug 2021 17:41:30 GMT
CMD ["/bin/sh"]
# Fri, 27 Aug 2021 19:13:56 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Fri, 27 Aug 2021 19:13:58 GMT
RUN apk add --no-cache libsasl
# Fri, 27 Aug 2021 19:13:59 GMT
ENV MEMCACHED_VERSION=1.6.10
# Fri, 27 Aug 2021 19:13:59 GMT
ENV MEMCACHED_SHA1=cb5b9fe77a2a59cc6cc7103a415bc07df9ddc6ec
# Fri, 27 Aug 2021 19:22:03 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Fri, 27 Aug 2021 19:22:04 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 27 Aug 2021 19:22:05 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 27 Aug 2021 19:22:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 Aug 2021 19:22:06 GMT
USER memcache
# Fri, 27 Aug 2021 19:22:06 GMT
EXPOSE 11211
# Fri, 27 Aug 2021 19:22:07 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:da14cb6b6dc946dbb2d84386bcaca84e2d46f650767cd11bdb3331ec9d623988`  
		Last Modified: Fri, 27 Aug 2021 17:42:25 GMT  
		Size: 2.6 MB (2603464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5c3123815589d4cfc45a071f344bd0f3ca08ee63a471c2c114af2dece4699a0`  
		Last Modified: Fri, 27 Aug 2021 19:23:06 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d25c400e2d4eb8dee97bc754e9e52585af4304ec8cf3121b619bd5756796fb52`  
		Last Modified: Fri, 27 Aug 2021 19:23:06 GMT  
		Size: 161.5 KB (161520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:611fd541e530a5444852c1a56f01565817097a4b2abec64399dcf4fdd84dfe88`  
		Last Modified: Fri, 27 Aug 2021 19:23:06 GMT  
		Size: 929.3 KB (929257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cb82aed96a5a46fb2399db9bf85a3ff9a7ce3de3468fe74285ad84fd557a1ca`  
		Last Modified: Fri, 27 Aug 2021 19:23:06 GMT  
		Size: 283.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c18159f487fe568305c6aaeb29b07af5f859402bb29566a404f9fccbd86bafbf`  
		Last Modified: Fri, 27 Aug 2021 19:23:06 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:1.6.10-buster`

```console
$ docker pull memcached@sha256:0507080446e022bbcb398fef743f5479d61569f2992beccd200033e037968511
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

### `memcached:1.6.10-buster` - linux; amd64

```console
$ docker pull memcached@sha256:b93ad58a06f215580205490133ce2165fa69f1930b964e890981f629df497e84
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.6 MB (30631755 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:444d9869f3507356b3fb6ffb7ed74ffc3be04be873a6876423c24d17acbf1128`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 03 Sep 2021 01:21:46 GMT
ADD file:4ff85d9f6aa246746912db62dea02eb71750474bb29611e770516a1fcd217add in / 
# Fri, 03 Sep 2021 01:21:46 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 07:33:54 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Fri, 03 Sep 2021 07:34:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 07:34:01 GMT
ENV MEMCACHED_VERSION=1.6.10
# Fri, 03 Sep 2021 07:34:01 GMT
ENV MEMCACHED_SHA1=cb5b9fe77a2a59cc6cc7103a415bc07df9ddc6ec
# Fri, 03 Sep 2021 07:38:24 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Fri, 03 Sep 2021 07:38:24 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 03 Sep 2021 07:38:25 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 03 Sep 2021 07:38:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 03 Sep 2021 07:38:25 GMT
USER memcache
# Fri, 03 Sep 2021 07:38:26 GMT
EXPOSE 11211
# Fri, 03 Sep 2021 07:38:26 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:a330b6cecb98cd2425fd25fce36669073f593b3176b4ee14731e48c05d678cdd`  
		Last Modified: Fri, 03 Sep 2021 01:28:19 GMT  
		Size: 27.1 MB (27145844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7dcde8d481fe08e2bab1fc8a1dc0e30c1d8cc9647d2867a6bc06942de810d56`  
		Last Modified: Fri, 03 Sep 2021 07:38:54 GMT  
		Size: 5.0 KB (4981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c3e0b65008f095303aa1ff733845d2eed7b3836fad196bc16533b3420711745`  
		Last Modified: Fri, 03 Sep 2021 07:38:54 GMT  
		Size: 2.2 MB (2197580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ad3eb30b171e7b0c33373bdeb39dfc36b63b8ec501af75bae3d4a964872f042`  
		Last Modified: Fri, 03 Sep 2021 07:38:54 GMT  
		Size: 1.3 MB (1282944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e6e03de9a5467b70b4d10bf021740a05eea1aeebfd87864b4a9289df9cb64c0`  
		Last Modified: Fri, 03 Sep 2021 07:38:54 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe0025a339764c7acc0034c701ca2b443e0b1803745c41094ea54289f754a81c`  
		Last Modified: Fri, 03 Sep 2021 07:38:54 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.10-buster` - linux; arm variant v5

```console
$ docker pull memcached@sha256:5e1d0b6ce4b1b257e47c484709733908552416681c8f054bc97735e5ec114fa2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.0 MB (28036699 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd9fb75ae310df2e536d3a10e6dd9222317f89456fe6082c139b112849e5081b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 03 Sep 2021 00:51:26 GMT
ADD file:350748a564076da397b991745cd42e0688d15c72b9fd5c81f8ea0bb8938a2b3d in / 
# Fri, 03 Sep 2021 00:51:27 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 02:24:47 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Fri, 03 Sep 2021 02:24:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 02:24:58 GMT
ENV MEMCACHED_VERSION=1.6.10
# Fri, 03 Sep 2021 02:24:59 GMT
ENV MEMCACHED_SHA1=cb5b9fe77a2a59cc6cc7103a415bc07df9ddc6ec
# Fri, 03 Sep 2021 02:29:11 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Fri, 03 Sep 2021 02:29:12 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 03 Sep 2021 02:29:13 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 03 Sep 2021 02:29:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 03 Sep 2021 02:29:14 GMT
USER memcache
# Fri, 03 Sep 2021 02:29:14 GMT
EXPOSE 11211
# Fri, 03 Sep 2021 02:29:15 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:b019db4b5197128481d48d92ecacd6bb356c027a3d08393f6567a6fa183ba769`  
		Last Modified: Fri, 03 Sep 2021 01:07:12 GMT  
		Size: 24.9 MB (24879114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4faeba39e66674ac57454c2edb8018a9a29475db4893acb59bf00e84e5c4e88a`  
		Last Modified: Fri, 03 Sep 2021 02:30:10 GMT  
		Size: 4.9 KB (4895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b39e5da0381154e8db96921f6038b79a61f458bf76f9fdaae0d3f44b2d81f184`  
		Last Modified: Fri, 03 Sep 2021 02:30:11 GMT  
		Size: 1.9 MB (1897972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb47be4e43a9bfad0082a507b5885f22b4104821defe786af5237a6b48211a71`  
		Last Modified: Fri, 03 Sep 2021 02:30:11 GMT  
		Size: 1.3 MB (1254312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee01c0ace3ff5a5a86664234d47a50480b12f50f1390f5b78ab2b76a73e3346f`  
		Last Modified: Fri, 03 Sep 2021 02:30:10 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:240af99f2a1c8953e4436d48b387f4aa33defc9e83416c71f2d67d05c2a8cb48`  
		Last Modified: Fri, 03 Sep 2021 02:30:10 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.10-buster` - linux; arm variant v7

```console
$ docker pull memcached@sha256:ee3f4a07ff534651238a464f5b0a3b582facdc9784f9e0f9a5bcd0128762da4f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.8 MB (25788867 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6222a822647e49fef3f296a084e4504bd705efe8e0649bc91541e03b8a5d7b8a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 03 Sep 2021 01:00:40 GMT
ADD file:4754bbccf4c59f77dd54f3888871f0635a2f9655cda53f50e63237f1580286e0 in / 
# Fri, 03 Sep 2021 01:00:41 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 06:44:19 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Fri, 03 Sep 2021 06:44:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 06:44:29 GMT
ENV MEMCACHED_VERSION=1.6.10
# Fri, 03 Sep 2021 06:44:30 GMT
ENV MEMCACHED_SHA1=cb5b9fe77a2a59cc6cc7103a415bc07df9ddc6ec
# Fri, 03 Sep 2021 06:48:21 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Fri, 03 Sep 2021 06:48:22 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 03 Sep 2021 06:48:23 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 03 Sep 2021 06:48:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 03 Sep 2021 06:48:24 GMT
USER memcache
# Fri, 03 Sep 2021 06:48:25 GMT
EXPOSE 11211
# Fri, 03 Sep 2021 06:48:25 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:2215ad7863d95c38f1f794f1d5b4d6c5ca4ca7e921e4bb7218b803f7ed270675`  
		Last Modified: Fri, 03 Sep 2021 01:16:23 GMT  
		Size: 22.7 MB (22746151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d554d32fa680ffcf04f8b509fa6a16e796fadc0ecf8db8c48bcc2a911f9f4591`  
		Last Modified: Fri, 03 Sep 2021 07:00:56 GMT  
		Size: 4.9 KB (4895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a550041e12d651682f2b70b45620898d8cebd97f4b4b3469aaeac8d452a76ef`  
		Last Modified: Fri, 03 Sep 2021 07:00:56 GMT  
		Size: 1.8 MB (1812490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ae1581582d0b08a4635fe57247a454da856fea52ec988126ee4f2f1781b7acd`  
		Last Modified: Fri, 03 Sep 2021 07:00:56 GMT  
		Size: 1.2 MB (1224925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:678c3e64de445bdc9a420655f01c8abab5f2e7ef4f41d441e6d2310ea2c36de5`  
		Last Modified: Fri, 03 Sep 2021 07:00:55 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a21b13a7b8549e46debb4d9b1117211df9edcc02f822ec99d1fe1b4278f1e56`  
		Last Modified: Fri, 03 Sep 2021 07:00:55 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.10-buster` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:57e906b2282c3e67137cc8c2ab5148c8e748256b2e3934c5b7ecd77a6a186de5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.3 MB (29250783 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:932f1c94fc6e8e017820dcb97fe4b624efacba7409cb99c99a369c649b03829d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 03 Sep 2021 00:40:58 GMT
ADD file:4a1d7f2d989aee6bd83da076b6e9dd3da2da97cf5654bd37568e9baec30ac4b1 in / 
# Fri, 03 Sep 2021 00:40:58 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 02:46:23 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Fri, 03 Sep 2021 02:46:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 02:46:27 GMT
ENV MEMCACHED_VERSION=1.6.10
# Fri, 03 Sep 2021 02:46:28 GMT
ENV MEMCACHED_SHA1=cb5b9fe77a2a59cc6cc7103a415bc07df9ddc6ec
# Fri, 03 Sep 2021 02:50:03 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Fri, 03 Sep 2021 02:50:03 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 03 Sep 2021 02:50:04 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 03 Sep 2021 02:50:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 03 Sep 2021 02:50:04 GMT
USER memcache
# Fri, 03 Sep 2021 02:50:05 GMT
EXPOSE 11211
# Fri, 03 Sep 2021 02:50:05 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:d10c227306ce3db344a8399cbc02bbf0dcb36519318efbde3c6027c00be8b40e`  
		Last Modified: Fri, 03 Sep 2021 00:49:47 GMT  
		Size: 25.9 MB (25914860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee708d85ae4c6929688ee243da330a395c81a5da3913f7aaaeea88283b5752b1`  
		Last Modified: Fri, 03 Sep 2021 02:51:01 GMT  
		Size: 5.0 KB (5024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41eee23f132aa5ef6810f141bd4852d174eb68bd5e9f8fc4e278e2fc55f7cea8`  
		Last Modified: Fri, 03 Sep 2021 02:51:02 GMT  
		Size: 2.1 MB (2075717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d9a7819a72ed1b598aabafd5ac9be7be62ac6b085cc30dbda97ef193641fc05`  
		Last Modified: Fri, 03 Sep 2021 02:51:01 GMT  
		Size: 1.3 MB (1254776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ae146d1bf5917e1fb0f4aa46a655feefc0ec5e00ef4e775beed00fa6a1d0aa1`  
		Last Modified: Fri, 03 Sep 2021 02:51:01 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3cae1f92b0ec75c4c83b4b5a4ce47b455952d638c215f1588a20af7261fba5b`  
		Last Modified: Fri, 03 Sep 2021 02:51:01 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.10-buster` - linux; 386

```console
$ docker pull memcached@sha256:221d230cb426e233ce34c9669663db5628d85a6ffe1d98292cfb54d66a7e1f8a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.3 MB (31292631 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7283abe72dd41573bd7262a0ba163f6ef7ddf757bc5178c95eea585f8335e784`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 03 Sep 2021 00:40:24 GMT
ADD file:6bf4b6f4aa28306610ef10c68f422a7210ff2fbd5345cec07bc5f76d54a4c8bc in / 
# Fri, 03 Sep 2021 00:40:24 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 06:44:15 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Fri, 03 Sep 2021 06:44:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 06:44:21 GMT
ENV MEMCACHED_VERSION=1.6.10
# Fri, 03 Sep 2021 06:44:21 GMT
ENV MEMCACHED_SHA1=cb5b9fe77a2a59cc6cc7103a415bc07df9ddc6ec
# Fri, 03 Sep 2021 06:48:23 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Fri, 03 Sep 2021 06:48:24 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 03 Sep 2021 06:48:25 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 03 Sep 2021 06:48:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 03 Sep 2021 06:48:26 GMT
USER memcache
# Fri, 03 Sep 2021 06:48:26 GMT
EXPOSE 11211
# Fri, 03 Sep 2021 06:48:26 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:7e87f600658a0c0d3bd8b82b9c645b5ec2763492ec627c1c1c1183c2ad3c45d5`  
		Last Modified: Fri, 03 Sep 2021 00:49:06 GMT  
		Size: 27.8 MB (27797513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9454a8c8c54135f6e7f591277550407671a2a183d0ea7a1b04e0b7bf1ecfeb39`  
		Last Modified: Fri, 03 Sep 2021 06:49:32 GMT  
		Size: 4.9 KB (4895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4900dba329569a63986180bc83b94449c1dffc3a804c2910a2a3f288509964d3`  
		Last Modified: Fri, 03 Sep 2021 06:49:32 GMT  
		Size: 2.2 MB (2209620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb8624563e6585b031c874cc180ee08148f5773238b0bc1571feb1b64b198ee5`  
		Last Modified: Fri, 03 Sep 2021 06:49:32 GMT  
		Size: 1.3 MB (1280199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86f15c6c59e3205f04fba85035da98cd62d3f67bca6baa035b56db7f4f5dfb5c`  
		Last Modified: Fri, 03 Sep 2021 06:49:32 GMT  
		Size: 283.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f1b51c6ca8d549a8b18622d1c15504b94257295420bc332544f8d9026fff6f3`  
		Last Modified: Fri, 03 Sep 2021 06:49:32 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.10-buster` - linux; mips64le

```console
$ docker pull memcached@sha256:33ce4398cd07967870c76b95ec5314cbe8280d564309b25d0640e8dd94cb7198
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.9 MB (28866865 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cc3e459293995ad1867b805e319ebb5b3942502abbad00cf3f9b3a4ccc26c740`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 28 Sep 2021 02:11:41 GMT
ADD file:df525c65bc60141f19ab937525d724c6d29cac53beb30f92d79ea4b2edf5a13e in / 
# Tue, 28 Sep 2021 02:11:41 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 02:51:00 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 28 Sep 2021 02:51:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:51:13 GMT
ENV MEMCACHED_VERSION=1.6.10
# Tue, 28 Sep 2021 02:51:13 GMT
ENV MEMCACHED_SHA1=cb5b9fe77a2a59cc6cc7103a415bc07df9ddc6ec
# Tue, 28 Sep 2021 02:56:56 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 28 Sep 2021 02:56:56 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 28 Sep 2021 02:56:58 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 28 Sep 2021 02:56:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 28 Sep 2021 02:56:59 GMT
USER memcache
# Tue, 28 Sep 2021 02:56:59 GMT
EXPOSE 11211
# Tue, 28 Sep 2021 02:56:59 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:f1b3d9dde862ddf88a05cec47ce54e641c4057c7bfb377e2a065c72a42a76321`  
		Last Modified: Tue, 28 Sep 2021 02:22:07 GMT  
		Size: 25.8 MB (25813001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e684588e988c227c0fedbcfeb8361e35b75eaa06e38cf8207979b491712d3dc`  
		Last Modified: Tue, 28 Sep 2021 02:57:18 GMT  
		Size: 5.0 KB (4981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35a3bc6181fe53d4bf46e98ebace046f2014668d601c2c3975c3dc6fc655acbc`  
		Last Modified: Tue, 28 Sep 2021 02:57:19 GMT  
		Size: 1.8 MB (1777273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f49b3d8a270ebba87297e2461fe81567f28a880e22d7ef977a60930ad82d6aa6`  
		Last Modified: Tue, 28 Sep 2021 02:57:19 GMT  
		Size: 1.3 MB (1271204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:119de6bb61edbff9dc8919b6bbb0f35c144a065c899d3fe20127480e2985c0d8`  
		Last Modified: Tue, 28 Sep 2021 02:57:18 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ecffae4c1838eb68ee866feaae4a6357c6198f1e86b5a1719bd7646795396d6`  
		Last Modified: Tue, 28 Sep 2021 02:57:18 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.10-buster` - linux; ppc64le

```console
$ docker pull memcached@sha256:49728dba09507cb74bbfae419b5b8051106768fd3b53aa7964da2b4a7cf0d44f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.2 MB (34190787 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4563ba0117902a70591f2170ab90e34de0431ae24402ee05aa741d4eafbd036f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 03 Sep 2021 01:24:33 GMT
ADD file:6c1662ddb92232ae8969a86a18dacab97b3b5792a1ecda49e6ac741a1a5c878c in / 
# Fri, 03 Sep 2021 01:24:41 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 08:06:59 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Fri, 03 Sep 2021 08:07:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 08:07:23 GMT
ENV MEMCACHED_VERSION=1.6.10
# Fri, 03 Sep 2021 08:07:26 GMT
ENV MEMCACHED_SHA1=cb5b9fe77a2a59cc6cc7103a415bc07df9ddc6ec
# Fri, 03 Sep 2021 08:13:31 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Fri, 03 Sep 2021 08:13:32 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 03 Sep 2021 08:13:43 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 03 Sep 2021 08:13:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 03 Sep 2021 08:13:57 GMT
USER memcache
# Fri, 03 Sep 2021 08:14:01 GMT
EXPOSE 11211
# Fri, 03 Sep 2021 08:14:05 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:8258146296247df1f308a336d4abf286afae14e3375edefb87a091e80745e29f`  
		Last Modified: Fri, 03 Sep 2021 01:39:45 GMT  
		Size: 30.6 MB (30553675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2f96132a11c70c50168ade17294cf7e8c919db231f87a28818170d9917a3268`  
		Last Modified: Fri, 03 Sep 2021 08:14:54 GMT  
		Size: 5.0 KB (4988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:973046a9e11e4bf003ce0e9688dc396e6e0ded760e9914a57132e130fa64289a`  
		Last Modified: Fri, 03 Sep 2021 08:14:55 GMT  
		Size: 2.3 MB (2323873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e5495ff67177662caa9f0459d68cb0641f32eddb666f4238634e357e58bdad1`  
		Last Modified: Fri, 03 Sep 2021 08:14:55 GMT  
		Size: 1.3 MB (1307845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b406b4303f1d8fe163586ca2e7abe3639c752a524f2c44e46677c01e36f937c`  
		Last Modified: Fri, 03 Sep 2021 08:14:54 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ff817a29aac3d654f6e919cbea3ea8125cce972e357c595217ec95807e07c3d`  
		Last Modified: Fri, 03 Sep 2021 08:14:54 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.10-buster` - linux; s390x

```console
$ docker pull memcached@sha256:53459c6f3d42b7b718e1ccbb3090ff35e649d8d005fa1917cee1ee1fbfea608a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.9 MB (28925755 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8831bffed7f4d435dd3c714d24529fea34f84468cbc5abec57feeb4728059de`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 28 Sep 2021 01:43:29 GMT
ADD file:118e7a596407435b5e2ff0aae6bb9bff3b66000c91ca37bfe1eeb98c23d99d49 in / 
# Tue, 28 Sep 2021 01:43:30 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 02:31:35 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 28 Sep 2021 02:31:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:31:39 GMT
ENV MEMCACHED_VERSION=1.6.10
# Tue, 28 Sep 2021 02:31:39 GMT
ENV MEMCACHED_SHA1=cb5b9fe77a2a59cc6cc7103a415bc07df9ddc6ec
# Tue, 28 Sep 2021 02:34:53 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 28 Sep 2021 02:34:54 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 28 Sep 2021 02:34:54 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 28 Sep 2021 02:34:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 28 Sep 2021 02:34:54 GMT
USER memcache
# Tue, 28 Sep 2021 02:34:54 GMT
EXPOSE 11211
# Tue, 28 Sep 2021 02:34:55 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:7cfe208f95c1b63305981b069795676fa149e7115b9044c241ee45ef4aaf0bb3`  
		Last Modified: Tue, 28 Sep 2021 01:49:36 GMT  
		Size: 25.8 MB (25760871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff755a70833a769c5a32cb251e86ac9aa6ae1dce7f547dc1bef874a22855b63d`  
		Last Modified: Tue, 28 Sep 2021 02:35:52 GMT  
		Size: 5.0 KB (5022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d08a7a4b96e17b9ef0eb0b8dd97ad0dc3d75227841b6374b7071e7989d9fed3c`  
		Last Modified: Tue, 28 Sep 2021 02:35:52 GMT  
		Size: 1.9 MB (1887230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4b9662cd31c943100c81ad7c951195bf462ad510ed53de50144b8617d870a84`  
		Last Modified: Tue, 28 Sep 2021 02:35:52 GMT  
		Size: 1.3 MB (1272226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fc50167475bec35471f2d4f925c2d427f3757ac01cd3f8f82cc5685771c2744`  
		Last Modified: Tue, 28 Sep 2021 02:35:52 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c69d6c53bee775bfd205e1d0426724cebf2eddd3034e82681311e18028641c25`  
		Last Modified: Tue, 28 Sep 2021 02:35:52 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:alpine`

```console
$ docker pull memcached@sha256:99e30a033ef422d6ad3ebe18c6c1009f20bee2d025fc00569be5dcd81aadc7be
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 7
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `memcached:alpine` - linux; amd64

```console
$ docker pull memcached@sha256:67d93d2efc4859c0b2e5a24bc13e759788c1f28d97a4d68b58a3de323e8ccb38
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3904613 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec200929117689b8cbba5a24fe5e892d7e4bfec5b654cef54958801a6ab9e92b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Fri, 27 Aug 2021 20:39:15 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Fri, 27 Aug 2021 20:39:16 GMT
RUN apk add --no-cache libsasl
# Fri, 27 Aug 2021 20:39:16 GMT
ENV MEMCACHED_VERSION=1.6.10
# Fri, 27 Aug 2021 20:39:17 GMT
ENV MEMCACHED_SHA1=cb5b9fe77a2a59cc6cc7103a415bc07df9ddc6ec
# Fri, 27 Aug 2021 20:43:47 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Fri, 27 Aug 2021 20:43:47 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 27 Aug 2021 20:43:49 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 27 Aug 2021 20:43:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 Aug 2021 20:43:50 GMT
USER memcache
# Fri, 27 Aug 2021 20:43:50 GMT
EXPOSE 11211
# Fri, 27 Aug 2021 20:43:50 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:a0d0a0d46f8b52473982a3c466318f479767577551a53ffc9074c9fa7035982e`  
		Last Modified: Fri, 27 Aug 2021 17:20:13 GMT  
		Size: 2.8 MB (2814446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84db6e403c6f8cdc8217536fa7d8bb9bbee66a7a49106104b3ceeace758e887b`  
		Last Modified: Fri, 27 Aug 2021 20:44:26 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7430c0d88cc6cc6389bb62e421f43031b009d21243f7362290bcf11b82e9e967`  
		Last Modified: Fri, 27 Aug 2021 20:44:26 GMT  
		Size: 155.5 KB (155516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3919afa4c767ba881b469a2798f6ad270dc23bbd9174d2994a0208bf508febba`  
		Last Modified: Fri, 27 Aug 2021 20:44:26 GMT  
		Size: 933.0 KB (932979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e81a6f988f7ee7ae5df06403e582d0edb09dcd73e81bacdaa17d1e0da71e13b`  
		Last Modified: Fri, 27 Aug 2021 20:44:26 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d5ed3d833f3ab3255decd4fc642f2368e6791acc470e40c2f3eb7463b7351dc`  
		Last Modified: Fri, 27 Aug 2021 20:44:26 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:alpine` - linux; arm variant v6

```console
$ docker pull memcached@sha256:4d05de82436bd51ed609a745b8ddd01e296692beb5a372dcbdcf0b1f54818d03
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.3 MB (4270486 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:56e8bda6e6346ca01fa3a313ef7bcfcc696040d48be803f6c16922dedc8deae1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 16 Dec 2020 23:49:43 GMT
ADD file:0a16715e2d0e5811c3c578945d618db0e269847a799340248f9ba8d393c9eec2 in / 
# Wed, 16 Dec 2020 23:49:45 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 01:44:25 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Thu, 17 Dec 2020 01:44:29 GMT
RUN apk add --no-cache cyrus-sasl-plain
# Thu, 17 Dec 2020 01:44:30 GMT
ENV MEMCACHED_VERSION=1.6.9
# Thu, 17 Dec 2020 01:44:31 GMT
ENV MEMCACHED_SHA1=42ae062094fdf083cfe7b21ff377c781011c2be1
# Thu, 17 Dec 2020 01:47:40 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		dpkg-dev dpkg 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		tar 		wget 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Thu, 17 Dec 2020 01:47:41 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 17 Dec 2020 01:47:43 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 17 Dec 2020 01:47:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Dec 2020 01:47:44 GMT
USER memcache
# Thu, 17 Dec 2020 01:47:45 GMT
EXPOSE 11211
# Thu, 17 Dec 2020 01:47:46 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:93247449aef3c56eb4f7ab7b3fed95743c974b823def6dd86ec84008126e7903`  
		Last Modified: Wed, 16 Dec 2020 23:50:24 GMT  
		Size: 2.6 MB (2604163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cc04af65958529b14246e2401008ef0186d74a33d2aa1b64d5f49633a1ff8f1`  
		Last Modified: Thu, 17 Dec 2020 01:48:06 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08bb28157acd02855bdf031eb7158f2cbb9849a6a9e6b45b4b82b507df6d83e9`  
		Last Modified: Thu, 17 Dec 2020 01:48:06 GMT  
		Size: 14.9 KB (14904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b32778d38f805e0e2a84689dba047adda457098c6f4a0b3aeb51a9e9d3e7f2b`  
		Last Modified: Thu, 17 Dec 2020 01:48:06 GMT  
		Size: 1.6 MB (1649753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:506d15aa86681d1812c5696615302d2a50938410c852b6aa0d0680c7baa4589f`  
		Last Modified: Thu, 17 Dec 2020 01:48:06 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f55730e61cf75cdadfaf0682212c74d7a2355e652e0655cc74ba35a4b7cfb4c1`  
		Last Modified: Thu, 17 Dec 2020 01:48:06 GMT  
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
$ docker pull memcached@sha256:8ed70173927cd66ad4e1bac9803ba7114502646685f70abb395ef668a46db5fb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3793233 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c5c3d9ec3f6b46ae9e7305a3958b059ffc7d935b5f2094e78973054a0394060e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 27 Aug 2021 17:39:33 GMT
ADD file:dc8af9c7bfe9f9541e1db38dea01c4201609f3075b31e108f2073ffed8c5e4b9 in / 
# Fri, 27 Aug 2021 17:39:33 GMT
CMD ["/bin/sh"]
# Fri, 27 Aug 2021 20:15:01 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Fri, 27 Aug 2021 20:15:02 GMT
RUN apk add --no-cache libsasl
# Fri, 27 Aug 2021 20:15:02 GMT
ENV MEMCACHED_VERSION=1.6.10
# Fri, 27 Aug 2021 20:15:02 GMT
ENV MEMCACHED_SHA1=cb5b9fe77a2a59cc6cc7103a415bc07df9ddc6ec
# Fri, 27 Aug 2021 20:18:55 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Fri, 27 Aug 2021 20:18:55 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 27 Aug 2021 20:18:56 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 27 Aug 2021 20:18:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 Aug 2021 20:18:56 GMT
USER memcache
# Fri, 27 Aug 2021 20:18:56 GMT
EXPOSE 11211
# Fri, 27 Aug 2021 20:18:56 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:552d1f2373af9bfe12033568ebbfb0ccbb0de11279f9a415a29207e264d7f4d9`  
		Last Modified: Fri, 27 Aug 2021 17:40:18 GMT  
		Size: 2.7 MB (2711827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ab312377ca26aa6df3e0bb8b11a63d6964544ffd2552b8e7cebb0acbbc3036d`  
		Last Modified: Fri, 27 Aug 2021 20:19:53 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a538168cab1a5c606dfa94dd8b09de5598c9071505476146fa99500011f8e7f5`  
		Last Modified: Fri, 27 Aug 2021 20:19:53 GMT  
		Size: 157.2 KB (157194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae4e52b47025818dc222e8dcd9310ab3f3c757a434fb786d7100cfaef304d4ed`  
		Last Modified: Fri, 27 Aug 2021 20:19:53 GMT  
		Size: 922.5 KB (922539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bedcb7a468e2a54e811d3ab62759e10500ea8b580eb12a600991eb1a3eed136`  
		Last Modified: Fri, 27 Aug 2021 20:19:53 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50b5ad9ab615a8b63e96efab0f2b3b2ff0a60abcb13a2529437f46368a641c6e`  
		Last Modified: Fri, 27 Aug 2021 20:19:53 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:alpine` - linux; 386

```console
$ docker pull memcached@sha256:82a99c470435ce9fd7cebf6565305c9f9a20eb2142839f8a7eaf42fc04b1e64a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3937988 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:503d28ddbe03b1e33458c354e3e0cef3142579c20bdf6e8c1f4b447257a2de01`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 27 Aug 2021 17:38:29 GMT
ADD file:42a7bc5a08b546b47049dd0f89ae4e7a8c86342f87000f39ade3ff52916a6c2e in / 
# Fri, 27 Aug 2021 17:38:30 GMT
CMD ["/bin/sh"]
# Fri, 27 Aug 2021 19:48:52 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Fri, 27 Aug 2021 19:48:54 GMT
RUN apk add --no-cache libsasl
# Fri, 27 Aug 2021 19:48:54 GMT
ENV MEMCACHED_VERSION=1.6.10
# Fri, 27 Aug 2021 19:48:55 GMT
ENV MEMCACHED_SHA1=cb5b9fe77a2a59cc6cc7103a415bc07df9ddc6ec
# Fri, 27 Aug 2021 19:53:36 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Fri, 27 Aug 2021 19:53:36 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 27 Aug 2021 19:53:37 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 27 Aug 2021 19:53:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 Aug 2021 19:53:38 GMT
USER memcache
# Fri, 27 Aug 2021 19:53:38 GMT
EXPOSE 11211
# Fri, 27 Aug 2021 19:53:38 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:b11ae9fc5d8a106cfed3a6f6c75e5b5b5797c566fac4411622b4055df6541286`  
		Last Modified: Fri, 27 Aug 2021 17:39:18 GMT  
		Size: 2.8 MB (2822857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a776c6c02658f2d17623bce57a634d82f2dc8c8bee59f4d90fc786c3e69e31ff`  
		Last Modified: Fri, 27 Aug 2021 19:54:35 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fab8279289e8b7a476ce09017d9bcdb33bccbe04750f2ccba41c0a43f828b16`  
		Last Modified: Fri, 27 Aug 2021 19:54:35 GMT  
		Size: 169.0 KB (169012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24c50e3cfd5d1f42d6dd2505b7b02ca2ed14cb53d2199df2bed319e84146d13b`  
		Last Modified: Fri, 27 Aug 2021 19:54:36 GMT  
		Size: 944.4 KB (944446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3856e8e8dfa799b89d86a7552466e0b451bc8b8b140b56d53056ea942b82b102`  
		Last Modified: Fri, 27 Aug 2021 19:54:35 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bd1d4e4fe24a075a95e91ec623e250fb1071d34af2ec3a777ceecca3d62ea9f`  
		Last Modified: Fri, 27 Aug 2021 19:54:35 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:alpine` - linux; ppc64le

```console
$ docker pull memcached@sha256:5ea0c2672938efeae9c4cf8a45bdb1a06eaacb2f1014ed8fef3d3c6339b3fac5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.0 MB (3954868 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e20a2c1b753cc0bb4b19ca80b7d333dcbb37ce0a77e99c1b96ef27b09b680fa7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 27 Aug 2021 19:39:54 GMT
ADD file:d213c56ffc24a5051e8060fd0fec1a0520367c10d88ab16321c36336b6c66098 in / 
# Fri, 27 Aug 2021 19:39:59 GMT
CMD ["/bin/sh"]
# Sat, 28 Aug 2021 02:52:59 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Sat, 28 Aug 2021 02:53:08 GMT
RUN apk add --no-cache libsasl
# Sat, 28 Aug 2021 02:53:10 GMT
ENV MEMCACHED_VERSION=1.6.10
# Sat, 28 Aug 2021 02:53:12 GMT
ENV MEMCACHED_SHA1=cb5b9fe77a2a59cc6cc7103a415bc07df9ddc6ec
# Sat, 28 Aug 2021 02:56:38 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Sat, 28 Aug 2021 02:56:40 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Sat, 28 Aug 2021 02:56:47 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Sat, 28 Aug 2021 02:56:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 28 Aug 2021 02:56:57 GMT
USER memcache
# Sat, 28 Aug 2021 02:57:02 GMT
EXPOSE 11211
# Sat, 28 Aug 2021 02:57:09 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:63da8ca98f7b4b94381aed56862a60aecf355d9428b9aeb7c61d5bd017100c18`  
		Last Modified: Fri, 27 Aug 2021 19:41:06 GMT  
		Size: 2.8 MB (2812284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a54fbc6ddd30fadabd2cf34600dd72918de6e611345c8202b6cd56a411467659`  
		Last Modified: Sat, 28 Aug 2021 02:58:02 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdd08b1afa1a2e02df391d85b3cfccf552f50b91046d9eafbe19feffb2f58910`  
		Last Modified: Sat, 28 Aug 2021 02:58:02 GMT  
		Size: 179.7 KB (179652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d214dccc5e7f55ecf8e9ec4471487fa0f6ba5ba2e84a3c746ff458410a29c755`  
		Last Modified: Sat, 28 Aug 2021 02:58:02 GMT  
		Size: 961.3 KB (961258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a6ae8b6fa12461573aab65c6be736cd4668463495c569d1113861ff729fb89f`  
		Last Modified: Sat, 28 Aug 2021 02:58:02 GMT  
		Size: 283.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fef62e61ad65fab7f854dd8a0a437b4ed6853b4186a9639a41ac47dae3f7d9e`  
		Last Modified: Sat, 28 Aug 2021 02:58:02 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:alpine` - linux; s390x

```console
$ docker pull memcached@sha256:cebdf9f1ff4ffe7551d4917b4a53e78ac48da41a694a8301fbd92459ebd9f45f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.7 MB (3695912 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:047503017563255821d3a05e00a220624c8698ef1a285eb6a05023ef0c1335e4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 27 Aug 2021 17:41:29 GMT
ADD file:9b40ee281e8797067fb2ae207c406084cb81593090338a8b7cb09ade52168daa in / 
# Fri, 27 Aug 2021 17:41:30 GMT
CMD ["/bin/sh"]
# Fri, 27 Aug 2021 19:13:56 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Fri, 27 Aug 2021 19:13:58 GMT
RUN apk add --no-cache libsasl
# Fri, 27 Aug 2021 19:13:59 GMT
ENV MEMCACHED_VERSION=1.6.10
# Fri, 27 Aug 2021 19:13:59 GMT
ENV MEMCACHED_SHA1=cb5b9fe77a2a59cc6cc7103a415bc07df9ddc6ec
# Fri, 27 Aug 2021 19:22:03 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Fri, 27 Aug 2021 19:22:04 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 27 Aug 2021 19:22:05 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 27 Aug 2021 19:22:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 Aug 2021 19:22:06 GMT
USER memcache
# Fri, 27 Aug 2021 19:22:06 GMT
EXPOSE 11211
# Fri, 27 Aug 2021 19:22:07 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:da14cb6b6dc946dbb2d84386bcaca84e2d46f650767cd11bdb3331ec9d623988`  
		Last Modified: Fri, 27 Aug 2021 17:42:25 GMT  
		Size: 2.6 MB (2603464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5c3123815589d4cfc45a071f344bd0f3ca08ee63a471c2c114af2dece4699a0`  
		Last Modified: Fri, 27 Aug 2021 19:23:06 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d25c400e2d4eb8dee97bc754e9e52585af4304ec8cf3121b619bd5756796fb52`  
		Last Modified: Fri, 27 Aug 2021 19:23:06 GMT  
		Size: 161.5 KB (161520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:611fd541e530a5444852c1a56f01565817097a4b2abec64399dcf4fdd84dfe88`  
		Last Modified: Fri, 27 Aug 2021 19:23:06 GMT  
		Size: 929.3 KB (929257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cb82aed96a5a46fb2399db9bf85a3ff9a7ce3de3468fe74285ad84fd557a1ca`  
		Last Modified: Fri, 27 Aug 2021 19:23:06 GMT  
		Size: 283.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c18159f487fe568305c6aaeb29b07af5f859402bb29566a404f9fccbd86bafbf`  
		Last Modified: Fri, 27 Aug 2021 19:23:06 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:alpine3.14`

```console
$ docker pull memcached@sha256:d57531b1d9bfffc9ada8c669fe761da3c7f9a15b9ac27d0f383e318d40f90e0d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `memcached:alpine3.14` - linux; amd64

```console
$ docker pull memcached@sha256:67d93d2efc4859c0b2e5a24bc13e759788c1f28d97a4d68b58a3de323e8ccb38
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3904613 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec200929117689b8cbba5a24fe5e892d7e4bfec5b654cef54958801a6ab9e92b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Fri, 27 Aug 2021 20:39:15 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Fri, 27 Aug 2021 20:39:16 GMT
RUN apk add --no-cache libsasl
# Fri, 27 Aug 2021 20:39:16 GMT
ENV MEMCACHED_VERSION=1.6.10
# Fri, 27 Aug 2021 20:39:17 GMT
ENV MEMCACHED_SHA1=cb5b9fe77a2a59cc6cc7103a415bc07df9ddc6ec
# Fri, 27 Aug 2021 20:43:47 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Fri, 27 Aug 2021 20:43:47 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 27 Aug 2021 20:43:49 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 27 Aug 2021 20:43:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 Aug 2021 20:43:50 GMT
USER memcache
# Fri, 27 Aug 2021 20:43:50 GMT
EXPOSE 11211
# Fri, 27 Aug 2021 20:43:50 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:a0d0a0d46f8b52473982a3c466318f479767577551a53ffc9074c9fa7035982e`  
		Last Modified: Fri, 27 Aug 2021 17:20:13 GMT  
		Size: 2.8 MB (2814446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84db6e403c6f8cdc8217536fa7d8bb9bbee66a7a49106104b3ceeace758e887b`  
		Last Modified: Fri, 27 Aug 2021 20:44:26 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7430c0d88cc6cc6389bb62e421f43031b009d21243f7362290bcf11b82e9e967`  
		Last Modified: Fri, 27 Aug 2021 20:44:26 GMT  
		Size: 155.5 KB (155516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3919afa4c767ba881b469a2798f6ad270dc23bbd9174d2994a0208bf508febba`  
		Last Modified: Fri, 27 Aug 2021 20:44:26 GMT  
		Size: 933.0 KB (932979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e81a6f988f7ee7ae5df06403e582d0edb09dcd73e81bacdaa17d1e0da71e13b`  
		Last Modified: Fri, 27 Aug 2021 20:44:26 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d5ed3d833f3ab3255decd4fc642f2368e6791acc470e40c2f3eb7463b7351dc`  
		Last Modified: Fri, 27 Aug 2021 20:44:26 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:alpine3.14` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:8ed70173927cd66ad4e1bac9803ba7114502646685f70abb395ef668a46db5fb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3793233 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c5c3d9ec3f6b46ae9e7305a3958b059ffc7d935b5f2094e78973054a0394060e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 27 Aug 2021 17:39:33 GMT
ADD file:dc8af9c7bfe9f9541e1db38dea01c4201609f3075b31e108f2073ffed8c5e4b9 in / 
# Fri, 27 Aug 2021 17:39:33 GMT
CMD ["/bin/sh"]
# Fri, 27 Aug 2021 20:15:01 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Fri, 27 Aug 2021 20:15:02 GMT
RUN apk add --no-cache libsasl
# Fri, 27 Aug 2021 20:15:02 GMT
ENV MEMCACHED_VERSION=1.6.10
# Fri, 27 Aug 2021 20:15:02 GMT
ENV MEMCACHED_SHA1=cb5b9fe77a2a59cc6cc7103a415bc07df9ddc6ec
# Fri, 27 Aug 2021 20:18:55 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Fri, 27 Aug 2021 20:18:55 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 27 Aug 2021 20:18:56 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 27 Aug 2021 20:18:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 Aug 2021 20:18:56 GMT
USER memcache
# Fri, 27 Aug 2021 20:18:56 GMT
EXPOSE 11211
# Fri, 27 Aug 2021 20:18:56 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:552d1f2373af9bfe12033568ebbfb0ccbb0de11279f9a415a29207e264d7f4d9`  
		Last Modified: Fri, 27 Aug 2021 17:40:18 GMT  
		Size: 2.7 MB (2711827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ab312377ca26aa6df3e0bb8b11a63d6964544ffd2552b8e7cebb0acbbc3036d`  
		Last Modified: Fri, 27 Aug 2021 20:19:53 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a538168cab1a5c606dfa94dd8b09de5598c9071505476146fa99500011f8e7f5`  
		Last Modified: Fri, 27 Aug 2021 20:19:53 GMT  
		Size: 157.2 KB (157194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae4e52b47025818dc222e8dcd9310ab3f3c757a434fb786d7100cfaef304d4ed`  
		Last Modified: Fri, 27 Aug 2021 20:19:53 GMT  
		Size: 922.5 KB (922539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bedcb7a468e2a54e811d3ab62759e10500ea8b580eb12a600991eb1a3eed136`  
		Last Modified: Fri, 27 Aug 2021 20:19:53 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50b5ad9ab615a8b63e96efab0f2b3b2ff0a60abcb13a2529437f46368a641c6e`  
		Last Modified: Fri, 27 Aug 2021 20:19:53 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:alpine3.14` - linux; 386

```console
$ docker pull memcached@sha256:82a99c470435ce9fd7cebf6565305c9f9a20eb2142839f8a7eaf42fc04b1e64a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3937988 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:503d28ddbe03b1e33458c354e3e0cef3142579c20bdf6e8c1f4b447257a2de01`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 27 Aug 2021 17:38:29 GMT
ADD file:42a7bc5a08b546b47049dd0f89ae4e7a8c86342f87000f39ade3ff52916a6c2e in / 
# Fri, 27 Aug 2021 17:38:30 GMT
CMD ["/bin/sh"]
# Fri, 27 Aug 2021 19:48:52 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Fri, 27 Aug 2021 19:48:54 GMT
RUN apk add --no-cache libsasl
# Fri, 27 Aug 2021 19:48:54 GMT
ENV MEMCACHED_VERSION=1.6.10
# Fri, 27 Aug 2021 19:48:55 GMT
ENV MEMCACHED_SHA1=cb5b9fe77a2a59cc6cc7103a415bc07df9ddc6ec
# Fri, 27 Aug 2021 19:53:36 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Fri, 27 Aug 2021 19:53:36 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 27 Aug 2021 19:53:37 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 27 Aug 2021 19:53:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 Aug 2021 19:53:38 GMT
USER memcache
# Fri, 27 Aug 2021 19:53:38 GMT
EXPOSE 11211
# Fri, 27 Aug 2021 19:53:38 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:b11ae9fc5d8a106cfed3a6f6c75e5b5b5797c566fac4411622b4055df6541286`  
		Last Modified: Fri, 27 Aug 2021 17:39:18 GMT  
		Size: 2.8 MB (2822857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a776c6c02658f2d17623bce57a634d82f2dc8c8bee59f4d90fc786c3e69e31ff`  
		Last Modified: Fri, 27 Aug 2021 19:54:35 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fab8279289e8b7a476ce09017d9bcdb33bccbe04750f2ccba41c0a43f828b16`  
		Last Modified: Fri, 27 Aug 2021 19:54:35 GMT  
		Size: 169.0 KB (169012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24c50e3cfd5d1f42d6dd2505b7b02ca2ed14cb53d2199df2bed319e84146d13b`  
		Last Modified: Fri, 27 Aug 2021 19:54:36 GMT  
		Size: 944.4 KB (944446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3856e8e8dfa799b89d86a7552466e0b451bc8b8b140b56d53056ea942b82b102`  
		Last Modified: Fri, 27 Aug 2021 19:54:35 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bd1d4e4fe24a075a95e91ec623e250fb1071d34af2ec3a777ceecca3d62ea9f`  
		Last Modified: Fri, 27 Aug 2021 19:54:35 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:alpine3.14` - linux; ppc64le

```console
$ docker pull memcached@sha256:5ea0c2672938efeae9c4cf8a45bdb1a06eaacb2f1014ed8fef3d3c6339b3fac5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.0 MB (3954868 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e20a2c1b753cc0bb4b19ca80b7d333dcbb37ce0a77e99c1b96ef27b09b680fa7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 27 Aug 2021 19:39:54 GMT
ADD file:d213c56ffc24a5051e8060fd0fec1a0520367c10d88ab16321c36336b6c66098 in / 
# Fri, 27 Aug 2021 19:39:59 GMT
CMD ["/bin/sh"]
# Sat, 28 Aug 2021 02:52:59 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Sat, 28 Aug 2021 02:53:08 GMT
RUN apk add --no-cache libsasl
# Sat, 28 Aug 2021 02:53:10 GMT
ENV MEMCACHED_VERSION=1.6.10
# Sat, 28 Aug 2021 02:53:12 GMT
ENV MEMCACHED_SHA1=cb5b9fe77a2a59cc6cc7103a415bc07df9ddc6ec
# Sat, 28 Aug 2021 02:56:38 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Sat, 28 Aug 2021 02:56:40 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Sat, 28 Aug 2021 02:56:47 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Sat, 28 Aug 2021 02:56:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 28 Aug 2021 02:56:57 GMT
USER memcache
# Sat, 28 Aug 2021 02:57:02 GMT
EXPOSE 11211
# Sat, 28 Aug 2021 02:57:09 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:63da8ca98f7b4b94381aed56862a60aecf355d9428b9aeb7c61d5bd017100c18`  
		Last Modified: Fri, 27 Aug 2021 19:41:06 GMT  
		Size: 2.8 MB (2812284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a54fbc6ddd30fadabd2cf34600dd72918de6e611345c8202b6cd56a411467659`  
		Last Modified: Sat, 28 Aug 2021 02:58:02 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdd08b1afa1a2e02df391d85b3cfccf552f50b91046d9eafbe19feffb2f58910`  
		Last Modified: Sat, 28 Aug 2021 02:58:02 GMT  
		Size: 179.7 KB (179652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d214dccc5e7f55ecf8e9ec4471487fa0f6ba5ba2e84a3c746ff458410a29c755`  
		Last Modified: Sat, 28 Aug 2021 02:58:02 GMT  
		Size: 961.3 KB (961258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a6ae8b6fa12461573aab65c6be736cd4668463495c569d1113861ff729fb89f`  
		Last Modified: Sat, 28 Aug 2021 02:58:02 GMT  
		Size: 283.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fef62e61ad65fab7f854dd8a0a437b4ed6853b4186a9639a41ac47dae3f7d9e`  
		Last Modified: Sat, 28 Aug 2021 02:58:02 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:alpine3.14` - linux; s390x

```console
$ docker pull memcached@sha256:cebdf9f1ff4ffe7551d4917b4a53e78ac48da41a694a8301fbd92459ebd9f45f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.7 MB (3695912 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:047503017563255821d3a05e00a220624c8698ef1a285eb6a05023ef0c1335e4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 27 Aug 2021 17:41:29 GMT
ADD file:9b40ee281e8797067fb2ae207c406084cb81593090338a8b7cb09ade52168daa in / 
# Fri, 27 Aug 2021 17:41:30 GMT
CMD ["/bin/sh"]
# Fri, 27 Aug 2021 19:13:56 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Fri, 27 Aug 2021 19:13:58 GMT
RUN apk add --no-cache libsasl
# Fri, 27 Aug 2021 19:13:59 GMT
ENV MEMCACHED_VERSION=1.6.10
# Fri, 27 Aug 2021 19:13:59 GMT
ENV MEMCACHED_SHA1=cb5b9fe77a2a59cc6cc7103a415bc07df9ddc6ec
# Fri, 27 Aug 2021 19:22:03 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Fri, 27 Aug 2021 19:22:04 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 27 Aug 2021 19:22:05 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 27 Aug 2021 19:22:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 Aug 2021 19:22:06 GMT
USER memcache
# Fri, 27 Aug 2021 19:22:06 GMT
EXPOSE 11211
# Fri, 27 Aug 2021 19:22:07 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:da14cb6b6dc946dbb2d84386bcaca84e2d46f650767cd11bdb3331ec9d623988`  
		Last Modified: Fri, 27 Aug 2021 17:42:25 GMT  
		Size: 2.6 MB (2603464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5c3123815589d4cfc45a071f344bd0f3ca08ee63a471c2c114af2dece4699a0`  
		Last Modified: Fri, 27 Aug 2021 19:23:06 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d25c400e2d4eb8dee97bc754e9e52585af4304ec8cf3121b619bd5756796fb52`  
		Last Modified: Fri, 27 Aug 2021 19:23:06 GMT  
		Size: 161.5 KB (161520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:611fd541e530a5444852c1a56f01565817097a4b2abec64399dcf4fdd84dfe88`  
		Last Modified: Fri, 27 Aug 2021 19:23:06 GMT  
		Size: 929.3 KB (929257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cb82aed96a5a46fb2399db9bf85a3ff9a7ce3de3468fe74285ad84fd557a1ca`  
		Last Modified: Fri, 27 Aug 2021 19:23:06 GMT  
		Size: 283.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c18159f487fe568305c6aaeb29b07af5f859402bb29566a404f9fccbd86bafbf`  
		Last Modified: Fri, 27 Aug 2021 19:23:06 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:buster`

```console
$ docker pull memcached@sha256:0507080446e022bbcb398fef743f5479d61569f2992beccd200033e037968511
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

### `memcached:buster` - linux; amd64

```console
$ docker pull memcached@sha256:b93ad58a06f215580205490133ce2165fa69f1930b964e890981f629df497e84
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.6 MB (30631755 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:444d9869f3507356b3fb6ffb7ed74ffc3be04be873a6876423c24d17acbf1128`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 03 Sep 2021 01:21:46 GMT
ADD file:4ff85d9f6aa246746912db62dea02eb71750474bb29611e770516a1fcd217add in / 
# Fri, 03 Sep 2021 01:21:46 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 07:33:54 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Fri, 03 Sep 2021 07:34:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 07:34:01 GMT
ENV MEMCACHED_VERSION=1.6.10
# Fri, 03 Sep 2021 07:34:01 GMT
ENV MEMCACHED_SHA1=cb5b9fe77a2a59cc6cc7103a415bc07df9ddc6ec
# Fri, 03 Sep 2021 07:38:24 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Fri, 03 Sep 2021 07:38:24 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 03 Sep 2021 07:38:25 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 03 Sep 2021 07:38:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 03 Sep 2021 07:38:25 GMT
USER memcache
# Fri, 03 Sep 2021 07:38:26 GMT
EXPOSE 11211
# Fri, 03 Sep 2021 07:38:26 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:a330b6cecb98cd2425fd25fce36669073f593b3176b4ee14731e48c05d678cdd`  
		Last Modified: Fri, 03 Sep 2021 01:28:19 GMT  
		Size: 27.1 MB (27145844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7dcde8d481fe08e2bab1fc8a1dc0e30c1d8cc9647d2867a6bc06942de810d56`  
		Last Modified: Fri, 03 Sep 2021 07:38:54 GMT  
		Size: 5.0 KB (4981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c3e0b65008f095303aa1ff733845d2eed7b3836fad196bc16533b3420711745`  
		Last Modified: Fri, 03 Sep 2021 07:38:54 GMT  
		Size: 2.2 MB (2197580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ad3eb30b171e7b0c33373bdeb39dfc36b63b8ec501af75bae3d4a964872f042`  
		Last Modified: Fri, 03 Sep 2021 07:38:54 GMT  
		Size: 1.3 MB (1282944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e6e03de9a5467b70b4d10bf021740a05eea1aeebfd87864b4a9289df9cb64c0`  
		Last Modified: Fri, 03 Sep 2021 07:38:54 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe0025a339764c7acc0034c701ca2b443e0b1803745c41094ea54289f754a81c`  
		Last Modified: Fri, 03 Sep 2021 07:38:54 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:buster` - linux; arm variant v5

```console
$ docker pull memcached@sha256:5e1d0b6ce4b1b257e47c484709733908552416681c8f054bc97735e5ec114fa2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.0 MB (28036699 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd9fb75ae310df2e536d3a10e6dd9222317f89456fe6082c139b112849e5081b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 03 Sep 2021 00:51:26 GMT
ADD file:350748a564076da397b991745cd42e0688d15c72b9fd5c81f8ea0bb8938a2b3d in / 
# Fri, 03 Sep 2021 00:51:27 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 02:24:47 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Fri, 03 Sep 2021 02:24:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 02:24:58 GMT
ENV MEMCACHED_VERSION=1.6.10
# Fri, 03 Sep 2021 02:24:59 GMT
ENV MEMCACHED_SHA1=cb5b9fe77a2a59cc6cc7103a415bc07df9ddc6ec
# Fri, 03 Sep 2021 02:29:11 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Fri, 03 Sep 2021 02:29:12 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 03 Sep 2021 02:29:13 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 03 Sep 2021 02:29:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 03 Sep 2021 02:29:14 GMT
USER memcache
# Fri, 03 Sep 2021 02:29:14 GMT
EXPOSE 11211
# Fri, 03 Sep 2021 02:29:15 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:b019db4b5197128481d48d92ecacd6bb356c027a3d08393f6567a6fa183ba769`  
		Last Modified: Fri, 03 Sep 2021 01:07:12 GMT  
		Size: 24.9 MB (24879114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4faeba39e66674ac57454c2edb8018a9a29475db4893acb59bf00e84e5c4e88a`  
		Last Modified: Fri, 03 Sep 2021 02:30:10 GMT  
		Size: 4.9 KB (4895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b39e5da0381154e8db96921f6038b79a61f458bf76f9fdaae0d3f44b2d81f184`  
		Last Modified: Fri, 03 Sep 2021 02:30:11 GMT  
		Size: 1.9 MB (1897972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb47be4e43a9bfad0082a507b5885f22b4104821defe786af5237a6b48211a71`  
		Last Modified: Fri, 03 Sep 2021 02:30:11 GMT  
		Size: 1.3 MB (1254312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee01c0ace3ff5a5a86664234d47a50480b12f50f1390f5b78ab2b76a73e3346f`  
		Last Modified: Fri, 03 Sep 2021 02:30:10 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:240af99f2a1c8953e4436d48b387f4aa33defc9e83416c71f2d67d05c2a8cb48`  
		Last Modified: Fri, 03 Sep 2021 02:30:10 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:buster` - linux; arm variant v7

```console
$ docker pull memcached@sha256:ee3f4a07ff534651238a464f5b0a3b582facdc9784f9e0f9a5bcd0128762da4f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.8 MB (25788867 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6222a822647e49fef3f296a084e4504bd705efe8e0649bc91541e03b8a5d7b8a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 03 Sep 2021 01:00:40 GMT
ADD file:4754bbccf4c59f77dd54f3888871f0635a2f9655cda53f50e63237f1580286e0 in / 
# Fri, 03 Sep 2021 01:00:41 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 06:44:19 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Fri, 03 Sep 2021 06:44:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 06:44:29 GMT
ENV MEMCACHED_VERSION=1.6.10
# Fri, 03 Sep 2021 06:44:30 GMT
ENV MEMCACHED_SHA1=cb5b9fe77a2a59cc6cc7103a415bc07df9ddc6ec
# Fri, 03 Sep 2021 06:48:21 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Fri, 03 Sep 2021 06:48:22 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 03 Sep 2021 06:48:23 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 03 Sep 2021 06:48:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 03 Sep 2021 06:48:24 GMT
USER memcache
# Fri, 03 Sep 2021 06:48:25 GMT
EXPOSE 11211
# Fri, 03 Sep 2021 06:48:25 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:2215ad7863d95c38f1f794f1d5b4d6c5ca4ca7e921e4bb7218b803f7ed270675`  
		Last Modified: Fri, 03 Sep 2021 01:16:23 GMT  
		Size: 22.7 MB (22746151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d554d32fa680ffcf04f8b509fa6a16e796fadc0ecf8db8c48bcc2a911f9f4591`  
		Last Modified: Fri, 03 Sep 2021 07:00:56 GMT  
		Size: 4.9 KB (4895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a550041e12d651682f2b70b45620898d8cebd97f4b4b3469aaeac8d452a76ef`  
		Last Modified: Fri, 03 Sep 2021 07:00:56 GMT  
		Size: 1.8 MB (1812490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ae1581582d0b08a4635fe57247a454da856fea52ec988126ee4f2f1781b7acd`  
		Last Modified: Fri, 03 Sep 2021 07:00:56 GMT  
		Size: 1.2 MB (1224925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:678c3e64de445bdc9a420655f01c8abab5f2e7ef4f41d441e6d2310ea2c36de5`  
		Last Modified: Fri, 03 Sep 2021 07:00:55 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a21b13a7b8549e46debb4d9b1117211df9edcc02f822ec99d1fe1b4278f1e56`  
		Last Modified: Fri, 03 Sep 2021 07:00:55 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:buster` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:57e906b2282c3e67137cc8c2ab5148c8e748256b2e3934c5b7ecd77a6a186de5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.3 MB (29250783 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:932f1c94fc6e8e017820dcb97fe4b624efacba7409cb99c99a369c649b03829d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 03 Sep 2021 00:40:58 GMT
ADD file:4a1d7f2d989aee6bd83da076b6e9dd3da2da97cf5654bd37568e9baec30ac4b1 in / 
# Fri, 03 Sep 2021 00:40:58 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 02:46:23 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Fri, 03 Sep 2021 02:46:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 02:46:27 GMT
ENV MEMCACHED_VERSION=1.6.10
# Fri, 03 Sep 2021 02:46:28 GMT
ENV MEMCACHED_SHA1=cb5b9fe77a2a59cc6cc7103a415bc07df9ddc6ec
# Fri, 03 Sep 2021 02:50:03 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Fri, 03 Sep 2021 02:50:03 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 03 Sep 2021 02:50:04 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 03 Sep 2021 02:50:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 03 Sep 2021 02:50:04 GMT
USER memcache
# Fri, 03 Sep 2021 02:50:05 GMT
EXPOSE 11211
# Fri, 03 Sep 2021 02:50:05 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:d10c227306ce3db344a8399cbc02bbf0dcb36519318efbde3c6027c00be8b40e`  
		Last Modified: Fri, 03 Sep 2021 00:49:47 GMT  
		Size: 25.9 MB (25914860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee708d85ae4c6929688ee243da330a395c81a5da3913f7aaaeea88283b5752b1`  
		Last Modified: Fri, 03 Sep 2021 02:51:01 GMT  
		Size: 5.0 KB (5024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41eee23f132aa5ef6810f141bd4852d174eb68bd5e9f8fc4e278e2fc55f7cea8`  
		Last Modified: Fri, 03 Sep 2021 02:51:02 GMT  
		Size: 2.1 MB (2075717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d9a7819a72ed1b598aabafd5ac9be7be62ac6b085cc30dbda97ef193641fc05`  
		Last Modified: Fri, 03 Sep 2021 02:51:01 GMT  
		Size: 1.3 MB (1254776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ae146d1bf5917e1fb0f4aa46a655feefc0ec5e00ef4e775beed00fa6a1d0aa1`  
		Last Modified: Fri, 03 Sep 2021 02:51:01 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3cae1f92b0ec75c4c83b4b5a4ce47b455952d638c215f1588a20af7261fba5b`  
		Last Modified: Fri, 03 Sep 2021 02:51:01 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:buster` - linux; 386

```console
$ docker pull memcached@sha256:221d230cb426e233ce34c9669663db5628d85a6ffe1d98292cfb54d66a7e1f8a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.3 MB (31292631 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7283abe72dd41573bd7262a0ba163f6ef7ddf757bc5178c95eea585f8335e784`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 03 Sep 2021 00:40:24 GMT
ADD file:6bf4b6f4aa28306610ef10c68f422a7210ff2fbd5345cec07bc5f76d54a4c8bc in / 
# Fri, 03 Sep 2021 00:40:24 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 06:44:15 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Fri, 03 Sep 2021 06:44:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 06:44:21 GMT
ENV MEMCACHED_VERSION=1.6.10
# Fri, 03 Sep 2021 06:44:21 GMT
ENV MEMCACHED_SHA1=cb5b9fe77a2a59cc6cc7103a415bc07df9ddc6ec
# Fri, 03 Sep 2021 06:48:23 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Fri, 03 Sep 2021 06:48:24 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 03 Sep 2021 06:48:25 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 03 Sep 2021 06:48:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 03 Sep 2021 06:48:26 GMT
USER memcache
# Fri, 03 Sep 2021 06:48:26 GMT
EXPOSE 11211
# Fri, 03 Sep 2021 06:48:26 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:7e87f600658a0c0d3bd8b82b9c645b5ec2763492ec627c1c1c1183c2ad3c45d5`  
		Last Modified: Fri, 03 Sep 2021 00:49:06 GMT  
		Size: 27.8 MB (27797513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9454a8c8c54135f6e7f591277550407671a2a183d0ea7a1b04e0b7bf1ecfeb39`  
		Last Modified: Fri, 03 Sep 2021 06:49:32 GMT  
		Size: 4.9 KB (4895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4900dba329569a63986180bc83b94449c1dffc3a804c2910a2a3f288509964d3`  
		Last Modified: Fri, 03 Sep 2021 06:49:32 GMT  
		Size: 2.2 MB (2209620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb8624563e6585b031c874cc180ee08148f5773238b0bc1571feb1b64b198ee5`  
		Last Modified: Fri, 03 Sep 2021 06:49:32 GMT  
		Size: 1.3 MB (1280199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86f15c6c59e3205f04fba85035da98cd62d3f67bca6baa035b56db7f4f5dfb5c`  
		Last Modified: Fri, 03 Sep 2021 06:49:32 GMT  
		Size: 283.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f1b51c6ca8d549a8b18622d1c15504b94257295420bc332544f8d9026fff6f3`  
		Last Modified: Fri, 03 Sep 2021 06:49:32 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:buster` - linux; mips64le

```console
$ docker pull memcached@sha256:33ce4398cd07967870c76b95ec5314cbe8280d564309b25d0640e8dd94cb7198
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.9 MB (28866865 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cc3e459293995ad1867b805e319ebb5b3942502abbad00cf3f9b3a4ccc26c740`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 28 Sep 2021 02:11:41 GMT
ADD file:df525c65bc60141f19ab937525d724c6d29cac53beb30f92d79ea4b2edf5a13e in / 
# Tue, 28 Sep 2021 02:11:41 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 02:51:00 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 28 Sep 2021 02:51:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:51:13 GMT
ENV MEMCACHED_VERSION=1.6.10
# Tue, 28 Sep 2021 02:51:13 GMT
ENV MEMCACHED_SHA1=cb5b9fe77a2a59cc6cc7103a415bc07df9ddc6ec
# Tue, 28 Sep 2021 02:56:56 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 28 Sep 2021 02:56:56 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 28 Sep 2021 02:56:58 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 28 Sep 2021 02:56:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 28 Sep 2021 02:56:59 GMT
USER memcache
# Tue, 28 Sep 2021 02:56:59 GMT
EXPOSE 11211
# Tue, 28 Sep 2021 02:56:59 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:f1b3d9dde862ddf88a05cec47ce54e641c4057c7bfb377e2a065c72a42a76321`  
		Last Modified: Tue, 28 Sep 2021 02:22:07 GMT  
		Size: 25.8 MB (25813001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e684588e988c227c0fedbcfeb8361e35b75eaa06e38cf8207979b491712d3dc`  
		Last Modified: Tue, 28 Sep 2021 02:57:18 GMT  
		Size: 5.0 KB (4981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35a3bc6181fe53d4bf46e98ebace046f2014668d601c2c3975c3dc6fc655acbc`  
		Last Modified: Tue, 28 Sep 2021 02:57:19 GMT  
		Size: 1.8 MB (1777273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f49b3d8a270ebba87297e2461fe81567f28a880e22d7ef977a60930ad82d6aa6`  
		Last Modified: Tue, 28 Sep 2021 02:57:19 GMT  
		Size: 1.3 MB (1271204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:119de6bb61edbff9dc8919b6bbb0f35c144a065c899d3fe20127480e2985c0d8`  
		Last Modified: Tue, 28 Sep 2021 02:57:18 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ecffae4c1838eb68ee866feaae4a6357c6198f1e86b5a1719bd7646795396d6`  
		Last Modified: Tue, 28 Sep 2021 02:57:18 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:buster` - linux; ppc64le

```console
$ docker pull memcached@sha256:49728dba09507cb74bbfae419b5b8051106768fd3b53aa7964da2b4a7cf0d44f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.2 MB (34190787 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4563ba0117902a70591f2170ab90e34de0431ae24402ee05aa741d4eafbd036f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 03 Sep 2021 01:24:33 GMT
ADD file:6c1662ddb92232ae8969a86a18dacab97b3b5792a1ecda49e6ac741a1a5c878c in / 
# Fri, 03 Sep 2021 01:24:41 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 08:06:59 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Fri, 03 Sep 2021 08:07:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 08:07:23 GMT
ENV MEMCACHED_VERSION=1.6.10
# Fri, 03 Sep 2021 08:07:26 GMT
ENV MEMCACHED_SHA1=cb5b9fe77a2a59cc6cc7103a415bc07df9ddc6ec
# Fri, 03 Sep 2021 08:13:31 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Fri, 03 Sep 2021 08:13:32 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 03 Sep 2021 08:13:43 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 03 Sep 2021 08:13:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 03 Sep 2021 08:13:57 GMT
USER memcache
# Fri, 03 Sep 2021 08:14:01 GMT
EXPOSE 11211
# Fri, 03 Sep 2021 08:14:05 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:8258146296247df1f308a336d4abf286afae14e3375edefb87a091e80745e29f`  
		Last Modified: Fri, 03 Sep 2021 01:39:45 GMT  
		Size: 30.6 MB (30553675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2f96132a11c70c50168ade17294cf7e8c919db231f87a28818170d9917a3268`  
		Last Modified: Fri, 03 Sep 2021 08:14:54 GMT  
		Size: 5.0 KB (4988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:973046a9e11e4bf003ce0e9688dc396e6e0ded760e9914a57132e130fa64289a`  
		Last Modified: Fri, 03 Sep 2021 08:14:55 GMT  
		Size: 2.3 MB (2323873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e5495ff67177662caa9f0459d68cb0641f32eddb666f4238634e357e58bdad1`  
		Last Modified: Fri, 03 Sep 2021 08:14:55 GMT  
		Size: 1.3 MB (1307845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b406b4303f1d8fe163586ca2e7abe3639c752a524f2c44e46677c01e36f937c`  
		Last Modified: Fri, 03 Sep 2021 08:14:54 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ff817a29aac3d654f6e919cbea3ea8125cce972e357c595217ec95807e07c3d`  
		Last Modified: Fri, 03 Sep 2021 08:14:54 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:buster` - linux; s390x

```console
$ docker pull memcached@sha256:53459c6f3d42b7b718e1ccbb3090ff35e649d8d005fa1917cee1ee1fbfea608a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.9 MB (28925755 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8831bffed7f4d435dd3c714d24529fea34f84468cbc5abec57feeb4728059de`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 28 Sep 2021 01:43:29 GMT
ADD file:118e7a596407435b5e2ff0aae6bb9bff3b66000c91ca37bfe1eeb98c23d99d49 in / 
# Tue, 28 Sep 2021 01:43:30 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 02:31:35 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 28 Sep 2021 02:31:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:31:39 GMT
ENV MEMCACHED_VERSION=1.6.10
# Tue, 28 Sep 2021 02:31:39 GMT
ENV MEMCACHED_SHA1=cb5b9fe77a2a59cc6cc7103a415bc07df9ddc6ec
# Tue, 28 Sep 2021 02:34:53 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 28 Sep 2021 02:34:54 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 28 Sep 2021 02:34:54 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 28 Sep 2021 02:34:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 28 Sep 2021 02:34:54 GMT
USER memcache
# Tue, 28 Sep 2021 02:34:54 GMT
EXPOSE 11211
# Tue, 28 Sep 2021 02:34:55 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:7cfe208f95c1b63305981b069795676fa149e7115b9044c241ee45ef4aaf0bb3`  
		Last Modified: Tue, 28 Sep 2021 01:49:36 GMT  
		Size: 25.8 MB (25760871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff755a70833a769c5a32cb251e86ac9aa6ae1dce7f547dc1bef874a22855b63d`  
		Last Modified: Tue, 28 Sep 2021 02:35:52 GMT  
		Size: 5.0 KB (5022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d08a7a4b96e17b9ef0eb0b8dd97ad0dc3d75227841b6374b7071e7989d9fed3c`  
		Last Modified: Tue, 28 Sep 2021 02:35:52 GMT  
		Size: 1.9 MB (1887230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4b9662cd31c943100c81ad7c951195bf462ad510ed53de50144b8617d870a84`  
		Last Modified: Tue, 28 Sep 2021 02:35:52 GMT  
		Size: 1.3 MB (1272226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fc50167475bec35471f2d4f925c2d427f3757ac01cd3f8f82cc5685771c2744`  
		Last Modified: Tue, 28 Sep 2021 02:35:52 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c69d6c53bee775bfd205e1d0426724cebf2eddd3034e82681311e18028641c25`  
		Last Modified: Tue, 28 Sep 2021 02:35:52 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:latest`

```console
$ docker pull memcached@sha256:0507080446e022bbcb398fef743f5479d61569f2992beccd200033e037968511
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
$ docker pull memcached@sha256:b93ad58a06f215580205490133ce2165fa69f1930b964e890981f629df497e84
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.6 MB (30631755 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:444d9869f3507356b3fb6ffb7ed74ffc3be04be873a6876423c24d17acbf1128`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 03 Sep 2021 01:21:46 GMT
ADD file:4ff85d9f6aa246746912db62dea02eb71750474bb29611e770516a1fcd217add in / 
# Fri, 03 Sep 2021 01:21:46 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 07:33:54 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Fri, 03 Sep 2021 07:34:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 07:34:01 GMT
ENV MEMCACHED_VERSION=1.6.10
# Fri, 03 Sep 2021 07:34:01 GMT
ENV MEMCACHED_SHA1=cb5b9fe77a2a59cc6cc7103a415bc07df9ddc6ec
# Fri, 03 Sep 2021 07:38:24 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Fri, 03 Sep 2021 07:38:24 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 03 Sep 2021 07:38:25 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 03 Sep 2021 07:38:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 03 Sep 2021 07:38:25 GMT
USER memcache
# Fri, 03 Sep 2021 07:38:26 GMT
EXPOSE 11211
# Fri, 03 Sep 2021 07:38:26 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:a330b6cecb98cd2425fd25fce36669073f593b3176b4ee14731e48c05d678cdd`  
		Last Modified: Fri, 03 Sep 2021 01:28:19 GMT  
		Size: 27.1 MB (27145844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7dcde8d481fe08e2bab1fc8a1dc0e30c1d8cc9647d2867a6bc06942de810d56`  
		Last Modified: Fri, 03 Sep 2021 07:38:54 GMT  
		Size: 5.0 KB (4981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c3e0b65008f095303aa1ff733845d2eed7b3836fad196bc16533b3420711745`  
		Last Modified: Fri, 03 Sep 2021 07:38:54 GMT  
		Size: 2.2 MB (2197580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ad3eb30b171e7b0c33373bdeb39dfc36b63b8ec501af75bae3d4a964872f042`  
		Last Modified: Fri, 03 Sep 2021 07:38:54 GMT  
		Size: 1.3 MB (1282944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e6e03de9a5467b70b4d10bf021740a05eea1aeebfd87864b4a9289df9cb64c0`  
		Last Modified: Fri, 03 Sep 2021 07:38:54 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe0025a339764c7acc0034c701ca2b443e0b1803745c41094ea54289f754a81c`  
		Last Modified: Fri, 03 Sep 2021 07:38:54 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:latest` - linux; arm variant v5

```console
$ docker pull memcached@sha256:5e1d0b6ce4b1b257e47c484709733908552416681c8f054bc97735e5ec114fa2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.0 MB (28036699 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd9fb75ae310df2e536d3a10e6dd9222317f89456fe6082c139b112849e5081b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 03 Sep 2021 00:51:26 GMT
ADD file:350748a564076da397b991745cd42e0688d15c72b9fd5c81f8ea0bb8938a2b3d in / 
# Fri, 03 Sep 2021 00:51:27 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 02:24:47 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Fri, 03 Sep 2021 02:24:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 02:24:58 GMT
ENV MEMCACHED_VERSION=1.6.10
# Fri, 03 Sep 2021 02:24:59 GMT
ENV MEMCACHED_SHA1=cb5b9fe77a2a59cc6cc7103a415bc07df9ddc6ec
# Fri, 03 Sep 2021 02:29:11 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Fri, 03 Sep 2021 02:29:12 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 03 Sep 2021 02:29:13 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 03 Sep 2021 02:29:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 03 Sep 2021 02:29:14 GMT
USER memcache
# Fri, 03 Sep 2021 02:29:14 GMT
EXPOSE 11211
# Fri, 03 Sep 2021 02:29:15 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:b019db4b5197128481d48d92ecacd6bb356c027a3d08393f6567a6fa183ba769`  
		Last Modified: Fri, 03 Sep 2021 01:07:12 GMT  
		Size: 24.9 MB (24879114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4faeba39e66674ac57454c2edb8018a9a29475db4893acb59bf00e84e5c4e88a`  
		Last Modified: Fri, 03 Sep 2021 02:30:10 GMT  
		Size: 4.9 KB (4895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b39e5da0381154e8db96921f6038b79a61f458bf76f9fdaae0d3f44b2d81f184`  
		Last Modified: Fri, 03 Sep 2021 02:30:11 GMT  
		Size: 1.9 MB (1897972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb47be4e43a9bfad0082a507b5885f22b4104821defe786af5237a6b48211a71`  
		Last Modified: Fri, 03 Sep 2021 02:30:11 GMT  
		Size: 1.3 MB (1254312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee01c0ace3ff5a5a86664234d47a50480b12f50f1390f5b78ab2b76a73e3346f`  
		Last Modified: Fri, 03 Sep 2021 02:30:10 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:240af99f2a1c8953e4436d48b387f4aa33defc9e83416c71f2d67d05c2a8cb48`  
		Last Modified: Fri, 03 Sep 2021 02:30:10 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:latest` - linux; arm variant v7

```console
$ docker pull memcached@sha256:ee3f4a07ff534651238a464f5b0a3b582facdc9784f9e0f9a5bcd0128762da4f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.8 MB (25788867 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6222a822647e49fef3f296a084e4504bd705efe8e0649bc91541e03b8a5d7b8a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 03 Sep 2021 01:00:40 GMT
ADD file:4754bbccf4c59f77dd54f3888871f0635a2f9655cda53f50e63237f1580286e0 in / 
# Fri, 03 Sep 2021 01:00:41 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 06:44:19 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Fri, 03 Sep 2021 06:44:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 06:44:29 GMT
ENV MEMCACHED_VERSION=1.6.10
# Fri, 03 Sep 2021 06:44:30 GMT
ENV MEMCACHED_SHA1=cb5b9fe77a2a59cc6cc7103a415bc07df9ddc6ec
# Fri, 03 Sep 2021 06:48:21 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Fri, 03 Sep 2021 06:48:22 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 03 Sep 2021 06:48:23 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 03 Sep 2021 06:48:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 03 Sep 2021 06:48:24 GMT
USER memcache
# Fri, 03 Sep 2021 06:48:25 GMT
EXPOSE 11211
# Fri, 03 Sep 2021 06:48:25 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:2215ad7863d95c38f1f794f1d5b4d6c5ca4ca7e921e4bb7218b803f7ed270675`  
		Last Modified: Fri, 03 Sep 2021 01:16:23 GMT  
		Size: 22.7 MB (22746151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d554d32fa680ffcf04f8b509fa6a16e796fadc0ecf8db8c48bcc2a911f9f4591`  
		Last Modified: Fri, 03 Sep 2021 07:00:56 GMT  
		Size: 4.9 KB (4895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a550041e12d651682f2b70b45620898d8cebd97f4b4b3469aaeac8d452a76ef`  
		Last Modified: Fri, 03 Sep 2021 07:00:56 GMT  
		Size: 1.8 MB (1812490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ae1581582d0b08a4635fe57247a454da856fea52ec988126ee4f2f1781b7acd`  
		Last Modified: Fri, 03 Sep 2021 07:00:56 GMT  
		Size: 1.2 MB (1224925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:678c3e64de445bdc9a420655f01c8abab5f2e7ef4f41d441e6d2310ea2c36de5`  
		Last Modified: Fri, 03 Sep 2021 07:00:55 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a21b13a7b8549e46debb4d9b1117211df9edcc02f822ec99d1fe1b4278f1e56`  
		Last Modified: Fri, 03 Sep 2021 07:00:55 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:latest` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:57e906b2282c3e67137cc8c2ab5148c8e748256b2e3934c5b7ecd77a6a186de5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.3 MB (29250783 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:932f1c94fc6e8e017820dcb97fe4b624efacba7409cb99c99a369c649b03829d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 03 Sep 2021 00:40:58 GMT
ADD file:4a1d7f2d989aee6bd83da076b6e9dd3da2da97cf5654bd37568e9baec30ac4b1 in / 
# Fri, 03 Sep 2021 00:40:58 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 02:46:23 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Fri, 03 Sep 2021 02:46:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 02:46:27 GMT
ENV MEMCACHED_VERSION=1.6.10
# Fri, 03 Sep 2021 02:46:28 GMT
ENV MEMCACHED_SHA1=cb5b9fe77a2a59cc6cc7103a415bc07df9ddc6ec
# Fri, 03 Sep 2021 02:50:03 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Fri, 03 Sep 2021 02:50:03 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 03 Sep 2021 02:50:04 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 03 Sep 2021 02:50:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 03 Sep 2021 02:50:04 GMT
USER memcache
# Fri, 03 Sep 2021 02:50:05 GMT
EXPOSE 11211
# Fri, 03 Sep 2021 02:50:05 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:d10c227306ce3db344a8399cbc02bbf0dcb36519318efbde3c6027c00be8b40e`  
		Last Modified: Fri, 03 Sep 2021 00:49:47 GMT  
		Size: 25.9 MB (25914860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee708d85ae4c6929688ee243da330a395c81a5da3913f7aaaeea88283b5752b1`  
		Last Modified: Fri, 03 Sep 2021 02:51:01 GMT  
		Size: 5.0 KB (5024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41eee23f132aa5ef6810f141bd4852d174eb68bd5e9f8fc4e278e2fc55f7cea8`  
		Last Modified: Fri, 03 Sep 2021 02:51:02 GMT  
		Size: 2.1 MB (2075717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d9a7819a72ed1b598aabafd5ac9be7be62ac6b085cc30dbda97ef193641fc05`  
		Last Modified: Fri, 03 Sep 2021 02:51:01 GMT  
		Size: 1.3 MB (1254776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ae146d1bf5917e1fb0f4aa46a655feefc0ec5e00ef4e775beed00fa6a1d0aa1`  
		Last Modified: Fri, 03 Sep 2021 02:51:01 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3cae1f92b0ec75c4c83b4b5a4ce47b455952d638c215f1588a20af7261fba5b`  
		Last Modified: Fri, 03 Sep 2021 02:51:01 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:latest` - linux; 386

```console
$ docker pull memcached@sha256:221d230cb426e233ce34c9669663db5628d85a6ffe1d98292cfb54d66a7e1f8a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.3 MB (31292631 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7283abe72dd41573bd7262a0ba163f6ef7ddf757bc5178c95eea585f8335e784`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 03 Sep 2021 00:40:24 GMT
ADD file:6bf4b6f4aa28306610ef10c68f422a7210ff2fbd5345cec07bc5f76d54a4c8bc in / 
# Fri, 03 Sep 2021 00:40:24 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 06:44:15 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Fri, 03 Sep 2021 06:44:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 06:44:21 GMT
ENV MEMCACHED_VERSION=1.6.10
# Fri, 03 Sep 2021 06:44:21 GMT
ENV MEMCACHED_SHA1=cb5b9fe77a2a59cc6cc7103a415bc07df9ddc6ec
# Fri, 03 Sep 2021 06:48:23 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Fri, 03 Sep 2021 06:48:24 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 03 Sep 2021 06:48:25 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 03 Sep 2021 06:48:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 03 Sep 2021 06:48:26 GMT
USER memcache
# Fri, 03 Sep 2021 06:48:26 GMT
EXPOSE 11211
# Fri, 03 Sep 2021 06:48:26 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:7e87f600658a0c0d3bd8b82b9c645b5ec2763492ec627c1c1c1183c2ad3c45d5`  
		Last Modified: Fri, 03 Sep 2021 00:49:06 GMT  
		Size: 27.8 MB (27797513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9454a8c8c54135f6e7f591277550407671a2a183d0ea7a1b04e0b7bf1ecfeb39`  
		Last Modified: Fri, 03 Sep 2021 06:49:32 GMT  
		Size: 4.9 KB (4895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4900dba329569a63986180bc83b94449c1dffc3a804c2910a2a3f288509964d3`  
		Last Modified: Fri, 03 Sep 2021 06:49:32 GMT  
		Size: 2.2 MB (2209620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb8624563e6585b031c874cc180ee08148f5773238b0bc1571feb1b64b198ee5`  
		Last Modified: Fri, 03 Sep 2021 06:49:32 GMT  
		Size: 1.3 MB (1280199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86f15c6c59e3205f04fba85035da98cd62d3f67bca6baa035b56db7f4f5dfb5c`  
		Last Modified: Fri, 03 Sep 2021 06:49:32 GMT  
		Size: 283.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f1b51c6ca8d549a8b18622d1c15504b94257295420bc332544f8d9026fff6f3`  
		Last Modified: Fri, 03 Sep 2021 06:49:32 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:latest` - linux; mips64le

```console
$ docker pull memcached@sha256:33ce4398cd07967870c76b95ec5314cbe8280d564309b25d0640e8dd94cb7198
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.9 MB (28866865 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cc3e459293995ad1867b805e319ebb5b3942502abbad00cf3f9b3a4ccc26c740`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 28 Sep 2021 02:11:41 GMT
ADD file:df525c65bc60141f19ab937525d724c6d29cac53beb30f92d79ea4b2edf5a13e in / 
# Tue, 28 Sep 2021 02:11:41 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 02:51:00 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 28 Sep 2021 02:51:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:51:13 GMT
ENV MEMCACHED_VERSION=1.6.10
# Tue, 28 Sep 2021 02:51:13 GMT
ENV MEMCACHED_SHA1=cb5b9fe77a2a59cc6cc7103a415bc07df9ddc6ec
# Tue, 28 Sep 2021 02:56:56 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 28 Sep 2021 02:56:56 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 28 Sep 2021 02:56:58 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 28 Sep 2021 02:56:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 28 Sep 2021 02:56:59 GMT
USER memcache
# Tue, 28 Sep 2021 02:56:59 GMT
EXPOSE 11211
# Tue, 28 Sep 2021 02:56:59 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:f1b3d9dde862ddf88a05cec47ce54e641c4057c7bfb377e2a065c72a42a76321`  
		Last Modified: Tue, 28 Sep 2021 02:22:07 GMT  
		Size: 25.8 MB (25813001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e684588e988c227c0fedbcfeb8361e35b75eaa06e38cf8207979b491712d3dc`  
		Last Modified: Tue, 28 Sep 2021 02:57:18 GMT  
		Size: 5.0 KB (4981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35a3bc6181fe53d4bf46e98ebace046f2014668d601c2c3975c3dc6fc655acbc`  
		Last Modified: Tue, 28 Sep 2021 02:57:19 GMT  
		Size: 1.8 MB (1777273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f49b3d8a270ebba87297e2461fe81567f28a880e22d7ef977a60930ad82d6aa6`  
		Last Modified: Tue, 28 Sep 2021 02:57:19 GMT  
		Size: 1.3 MB (1271204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:119de6bb61edbff9dc8919b6bbb0f35c144a065c899d3fe20127480e2985c0d8`  
		Last Modified: Tue, 28 Sep 2021 02:57:18 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ecffae4c1838eb68ee866feaae4a6357c6198f1e86b5a1719bd7646795396d6`  
		Last Modified: Tue, 28 Sep 2021 02:57:18 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:latest` - linux; ppc64le

```console
$ docker pull memcached@sha256:49728dba09507cb74bbfae419b5b8051106768fd3b53aa7964da2b4a7cf0d44f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.2 MB (34190787 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4563ba0117902a70591f2170ab90e34de0431ae24402ee05aa741d4eafbd036f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 03 Sep 2021 01:24:33 GMT
ADD file:6c1662ddb92232ae8969a86a18dacab97b3b5792a1ecda49e6ac741a1a5c878c in / 
# Fri, 03 Sep 2021 01:24:41 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 08:06:59 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Fri, 03 Sep 2021 08:07:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 08:07:23 GMT
ENV MEMCACHED_VERSION=1.6.10
# Fri, 03 Sep 2021 08:07:26 GMT
ENV MEMCACHED_SHA1=cb5b9fe77a2a59cc6cc7103a415bc07df9ddc6ec
# Fri, 03 Sep 2021 08:13:31 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Fri, 03 Sep 2021 08:13:32 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 03 Sep 2021 08:13:43 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 03 Sep 2021 08:13:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 03 Sep 2021 08:13:57 GMT
USER memcache
# Fri, 03 Sep 2021 08:14:01 GMT
EXPOSE 11211
# Fri, 03 Sep 2021 08:14:05 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:8258146296247df1f308a336d4abf286afae14e3375edefb87a091e80745e29f`  
		Last Modified: Fri, 03 Sep 2021 01:39:45 GMT  
		Size: 30.6 MB (30553675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2f96132a11c70c50168ade17294cf7e8c919db231f87a28818170d9917a3268`  
		Last Modified: Fri, 03 Sep 2021 08:14:54 GMT  
		Size: 5.0 KB (4988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:973046a9e11e4bf003ce0e9688dc396e6e0ded760e9914a57132e130fa64289a`  
		Last Modified: Fri, 03 Sep 2021 08:14:55 GMT  
		Size: 2.3 MB (2323873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e5495ff67177662caa9f0459d68cb0641f32eddb666f4238634e357e58bdad1`  
		Last Modified: Fri, 03 Sep 2021 08:14:55 GMT  
		Size: 1.3 MB (1307845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b406b4303f1d8fe163586ca2e7abe3639c752a524f2c44e46677c01e36f937c`  
		Last Modified: Fri, 03 Sep 2021 08:14:54 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ff817a29aac3d654f6e919cbea3ea8125cce972e357c595217ec95807e07c3d`  
		Last Modified: Fri, 03 Sep 2021 08:14:54 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:latest` - linux; s390x

```console
$ docker pull memcached@sha256:53459c6f3d42b7b718e1ccbb3090ff35e649d8d005fa1917cee1ee1fbfea608a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.9 MB (28925755 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8831bffed7f4d435dd3c714d24529fea34f84468cbc5abec57feeb4728059de`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 28 Sep 2021 01:43:29 GMT
ADD file:118e7a596407435b5e2ff0aae6bb9bff3b66000c91ca37bfe1eeb98c23d99d49 in / 
# Tue, 28 Sep 2021 01:43:30 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 02:31:35 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 28 Sep 2021 02:31:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:31:39 GMT
ENV MEMCACHED_VERSION=1.6.10
# Tue, 28 Sep 2021 02:31:39 GMT
ENV MEMCACHED_SHA1=cb5b9fe77a2a59cc6cc7103a415bc07df9ddc6ec
# Tue, 28 Sep 2021 02:34:53 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 28 Sep 2021 02:34:54 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 28 Sep 2021 02:34:54 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 28 Sep 2021 02:34:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 28 Sep 2021 02:34:54 GMT
USER memcache
# Tue, 28 Sep 2021 02:34:54 GMT
EXPOSE 11211
# Tue, 28 Sep 2021 02:34:55 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:7cfe208f95c1b63305981b069795676fa149e7115b9044c241ee45ef4aaf0bb3`  
		Last Modified: Tue, 28 Sep 2021 01:49:36 GMT  
		Size: 25.8 MB (25760871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff755a70833a769c5a32cb251e86ac9aa6ae1dce7f547dc1bef874a22855b63d`  
		Last Modified: Tue, 28 Sep 2021 02:35:52 GMT  
		Size: 5.0 KB (5022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d08a7a4b96e17b9ef0eb0b8dd97ad0dc3d75227841b6374b7071e7989d9fed3c`  
		Last Modified: Tue, 28 Sep 2021 02:35:52 GMT  
		Size: 1.9 MB (1887230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4b9662cd31c943100c81ad7c951195bf462ad510ed53de50144b8617d870a84`  
		Last Modified: Tue, 28 Sep 2021 02:35:52 GMT  
		Size: 1.3 MB (1272226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fc50167475bec35471f2d4f925c2d427f3757ac01cd3f8f82cc5685771c2744`  
		Last Modified: Tue, 28 Sep 2021 02:35:52 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c69d6c53bee775bfd205e1d0426724cebf2eddd3034e82681311e18028641c25`  
		Last Modified: Tue, 28 Sep 2021 02:35:52 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
