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
-	[`memcached:1.6.16`](#memcached1616)
-	[`memcached:1.6.16-alpine`](#memcached1616-alpine)
-	[`memcached:1.6.16-alpine3.16`](#memcached1616-alpine316)
-	[`memcached:1.6.16-bullseye`](#memcached1616-bullseye)
-	[`memcached:alpine`](#memcachedalpine)
-	[`memcached:alpine3.16`](#memcachedalpine316)
-	[`memcached:bullseye`](#memcachedbullseye)
-	[`memcached:latest`](#memcachedlatest)

## `memcached:1`

```console
$ docker pull memcached@sha256:0afaa8e890393e089efc991b62ec98d3dd53e5da995abfa548e5df9c70722015
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
$ docker pull memcached@sha256:d6479777ae4663bb6752d9e779a2180adeae2e6f91da834a6c042665ef961b19
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.0 MB (32956000 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:36a225838cd6927616fc3c9afc4fc26e1fbe4097250b113b6b8508e02ae6a589`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 02 Aug 2022 01:20:04 GMT
ADD file:0eae0dca665c7044bf242cb1fc92cb8ea744f5af2dd376a558c90bc47349aefe in / 
# Tue, 02 Aug 2022 01:20:05 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 04:45:12 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 02 Aug 2022 04:45:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 04 Aug 2022 19:59:25 GMT
ENV MEMCACHED_VERSION=1.6.16
# Thu, 04 Aug 2022 19:59:25 GMT
ENV MEMCACHED_SHA1=724f31c3462fb6b07264d72d0043fd65545fd84a
# Thu, 04 Aug 2022 20:02:08 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 04 Aug 2022 20:02:08 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 04 Aug 2022 20:02:08 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 04 Aug 2022 20:02:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 04 Aug 2022 20:02:09 GMT
USER memcache
# Thu, 04 Aug 2022 20:02:09 GMT
EXPOSE 11211
# Thu, 04 Aug 2022 20:02:09 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:1efc276f4ff952c055dea726cfc96ec6a4fdb8b62d9eed816bd2b788f2860ad7`  
		Last Modified: Tue, 02 Aug 2022 01:24:13 GMT  
		Size: 31.4 MB (31366757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60bd6790acf68c1ccc4757e879b51b4dbc273681e1f30606a2ccd4b55623d288`  
		Last Modified: Tue, 02 Aug 2022 04:48:24 GMT  
		Size: 5.0 KB (4980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e72821989d416909e21411733d7d034cfa908016dceb0b6e2717a5fb9faa617`  
		Last Modified: Tue, 02 Aug 2022 04:48:24 GMT  
		Size: 328.1 KB (328097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a972a764145eff4153208b9f8bed20e2179ececcec6e6d462d74400d526ccb4c`  
		Last Modified: Thu, 04 Aug 2022 20:05:45 GMT  
		Size: 1.3 MB (1255762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc9c8a212883923ae20b3e2d671f8dcc32307603465cf915c7e83bd5ac522c69`  
		Last Modified: Thu, 04 Aug 2022 20:05:45 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:157eedd0af5feece73dbebf45897c44894a10678feca71d5d57ac4904492badc`  
		Last Modified: Thu, 04 Aug 2022 20:05:46 GMT  
		Size: 118.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1` - linux; arm variant v5

```console
$ docker pull memcached@sha256:39515e68cebee2b2b88891c2b46b1c517587063301f77bbf7c312f6f9b372d65
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.5 MB (30454297 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8bf4bc30f264f1f9a0ede671e3a081ea54d1b6c3127ad5d9d4df3de21a985f5a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 02 Aug 2022 00:49:10 GMT
ADD file:4cd2f95737fd3007912428eeac56036c9e67e989e66cec08a8be99da47f88494 in / 
# Tue, 02 Aug 2022 00:49:10 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 01:58:42 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 02 Aug 2022 01:58:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 04 Aug 2022 19:50:51 GMT
ENV MEMCACHED_VERSION=1.6.16
# Thu, 04 Aug 2022 19:50:51 GMT
ENV MEMCACHED_SHA1=724f31c3462fb6b07264d72d0043fd65545fd84a
# Thu, 04 Aug 2022 19:56:43 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 04 Aug 2022 19:56:44 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 04 Aug 2022 19:56:44 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 04 Aug 2022 19:56:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 04 Aug 2022 19:56:44 GMT
USER memcache
# Thu, 04 Aug 2022 19:56:44 GMT
EXPOSE 11211
# Thu, 04 Aug 2022 19:56:45 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:5890b0ca6af5e8467a488e68716691950496a8f247d0495c2d595ddcb1893aff`  
		Last Modified: Tue, 02 Aug 2022 00:56:06 GMT  
		Size: 28.9 MB (28905515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e34350eb48491f2ab07c0f07724d37412df97ee9093c7c2458c9917afe37a42d`  
		Last Modified: Tue, 02 Aug 2022 02:04:59 GMT  
		Size: 4.9 KB (4894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36ecb6d2f4e3224a48197a5aa9d40970083bf4a92f41fbb493ac5adf9441a4ad`  
		Last Modified: Tue, 02 Aug 2022 02:04:59 GMT  
		Size: 316.6 KB (316628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e691cd60b95cdbb7fe7d3d74b1af54a56f440ac30d1dee94df4c4c370610b68d`  
		Last Modified: Thu, 04 Aug 2022 19:57:24 GMT  
		Size: 1.2 MB (1226852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8da76a828532ea569bd0e56b5a07a5e8bff4fe6efe22a5940260a261d113dc05`  
		Last Modified: Thu, 04 Aug 2022 19:57:23 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1705baeac52cb73666f9792b18547ce08509addd9ff3f19f6b91d21d5d10c8aa`  
		Last Modified: Thu, 04 Aug 2022 19:57:23 GMT  
		Size: 120.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1` - linux; arm variant v7

```console
$ docker pull memcached@sha256:25e768546f1e321b2a9031611f8ecd4081990c82f8774f7e051a5480cf18445d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.1 MB (28076294 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5959e4e12e1b75611311d3866bc95f9fe30048418f972e70fa2c671a66149fdd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 02 Aug 2022 00:58:59 GMT
ADD file:1575b776a15adacebc0875642e97a80807d42dcfc8917e1406d47af7ac244c97 in / 
# Tue, 02 Aug 2022 00:58:59 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 06:28:56 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 02 Aug 2022 06:29:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 04 Aug 2022 21:30:08 GMT
ENV MEMCACHED_VERSION=1.6.16
# Thu, 04 Aug 2022 21:30:08 GMT
ENV MEMCACHED_SHA1=724f31c3462fb6b07264d72d0043fd65545fd84a
# Thu, 04 Aug 2022 21:36:35 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 04 Aug 2022 21:36:35 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 04 Aug 2022 21:36:36 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 04 Aug 2022 21:36:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 04 Aug 2022 21:36:37 GMT
USER memcache
# Thu, 04 Aug 2022 21:36:37 GMT
EXPOSE 11211
# Thu, 04 Aug 2022 21:36:37 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:1dd75a3a9c893a7dc313f683dd62464b7eab6c6d522ee62c8a17022631830f32`  
		Last Modified: Tue, 02 Aug 2022 01:06:45 GMT  
		Size: 26.6 MB (26560586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44a675a8ce135f198539dc76b078733393238f7c7b899c8635980eed8f35f1cc`  
		Last Modified: Tue, 02 Aug 2022 09:35:13 GMT  
		Size: 4.9 KB (4890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:497b0afd04c92a1e5d41f58dbc0d5d544b8880d000c0ffbd03adb48c32c0116b`  
		Last Modified: Tue, 02 Aug 2022 09:35:13 GMT  
		Size: 312.1 KB (312067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8874fe992be272d0e0780725714c2439507699c15bfad1a073df948a34eb668d`  
		Last Modified: Fri, 05 Aug 2022 00:37:30 GMT  
		Size: 1.2 MB (1198344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cd5e042b98c640c152a56816e122c5e7b0abe91535d5d891dceed9748e42129`  
		Last Modified: Fri, 05 Aug 2022 00:37:29 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e871a0f93bdc7cb723e47f45514f914186b73d1890a53cdfe8525dd034926d59`  
		Last Modified: Fri, 05 Aug 2022 00:37:29 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:759082b00d406f92781542ce86756eb73c5efe20acc7df6c25ac86be320a3ef5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.4 MB (31433439 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e91fe6663d9d90deed07c1d003a80fa6698137267c83310828f24a7ef63f6ef`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 02 Aug 2022 00:40:38 GMT
ADD file:6039adfbca55ed34a719c37672c664e3524130a0e2a3b8663629b8120b81b790 in / 
# Tue, 02 Aug 2022 00:40:39 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 03:56:15 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 02 Aug 2022 03:56:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 04 Aug 2022 20:33:46 GMT
ENV MEMCACHED_VERSION=1.6.16
# Thu, 04 Aug 2022 20:33:47 GMT
ENV MEMCACHED_SHA1=724f31c3462fb6b07264d72d0043fd65545fd84a
# Thu, 04 Aug 2022 20:36:17 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 04 Aug 2022 20:36:19 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 04 Aug 2022 20:36:19 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 04 Aug 2022 20:36:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 04 Aug 2022 20:36:21 GMT
USER memcache
# Thu, 04 Aug 2022 20:36:22 GMT
EXPOSE 11211
# Thu, 04 Aug 2022 20:36:23 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:a9fe95647e78b5516c7e2327355b6996e2ea295cd76ae242cbfe87f016b4e760`  
		Last Modified: Tue, 02 Aug 2022 00:46:05 GMT  
		Size: 30.1 MB (30054304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b983df009e7dc88033f53f015c09c56fd4db032d1abcade3333d8d4b515ff4af`  
		Last Modified: Tue, 02 Aug 2022 03:59:48 GMT  
		Size: 4.9 KB (4902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60720019405b50af041f391ec7dad90893ee95fc63fd6b3fb9da04850936f5db`  
		Last Modified: Tue, 02 Aug 2022 03:59:48 GMT  
		Size: 119.2 KB (119225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70569bedb4ee539337d6d3fd88e4076a1464b3a77bcfcca6604e18b815dbc402`  
		Last Modified: Thu, 04 Aug 2022 20:40:00 GMT  
		Size: 1.3 MB (1254600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:565112c01ad7b82688180f4fe70f5433126d79cc4b74e3d7f308601e2d34d9fe`  
		Last Modified: Thu, 04 Aug 2022 20:39:59 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce11290eb88924797c1fa048bd052c1243e4cb47e3469b26f3f1a3bc26472d19`  
		Last Modified: Thu, 04 Aug 2022 20:39:59 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1` - linux; 386

```console
$ docker pull memcached@sha256:deec44ba81c574f36b5b53185684413e4e97c3374d256e762ccf0e50fa1ff0f0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.8 MB (33762417 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9640d046f98daa1268a24f35ea7de08f83c728d88f2483d734101b09bad34768`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 02 Aug 2022 00:39:20 GMT
ADD file:f771e2286465694126158821089d801c7296376be2a56189e6041a15d2fe79f5 in / 
# Tue, 02 Aug 2022 00:39:21 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 03:12:03 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 02 Aug 2022 03:12:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 04 Aug 2022 20:28:41 GMT
ENV MEMCACHED_VERSION=1.6.16
# Thu, 04 Aug 2022 20:28:42 GMT
ENV MEMCACHED_SHA1=724f31c3462fb6b07264d72d0043fd65545fd84a
# Thu, 04 Aug 2022 20:31:30 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 04 Aug 2022 20:31:32 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 04 Aug 2022 20:31:32 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 04 Aug 2022 20:31:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 04 Aug 2022 20:31:34 GMT
USER memcache
# Thu, 04 Aug 2022 20:31:35 GMT
EXPOSE 11211
# Thu, 04 Aug 2022 20:31:36 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:90eb7f0ce9f33cf5dcd67d54c2fa606186dbaa5f95b6046f36145097267f9e53`  
		Last Modified: Tue, 02 Aug 2022 00:45:14 GMT  
		Size: 32.4 MB (32374054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:107cdc14debc414f1e6554b58402d2be697942f8f22b45d5c9b6bff8be3f332a`  
		Last Modified: Tue, 02 Aug 2022 03:15:55 GMT  
		Size: 4.8 KB (4771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b33bafb66f7f078457cf82ba6cfcbab5feae0e38bc0d959a5b50fa98fbcbf4ac`  
		Last Modified: Tue, 02 Aug 2022 03:15:55 GMT  
		Size: 130.1 KB (130114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c122afb77220a37620d69b968b43d326ed98ef7d9ed80ea06c3a7fa1c54dc73f`  
		Last Modified: Thu, 04 Aug 2022 20:35:38 GMT  
		Size: 1.3 MB (1253069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2426ab0684229e93e257d5c6357fbad018ee92d3cdcf5a7812171aa06bf82ca9`  
		Last Modified: Thu, 04 Aug 2022 20:35:38 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:240ed953e9e062d3ea6893fe34ecd1e5e060a240ae2a66092c6970c0be0eeed5`  
		Last Modified: Thu, 04 Aug 2022 20:35:38 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1` - linux; mips64le

```console
$ docker pull memcached@sha256:0d6798ccd4a9ac44c6ca7c358b2de6bdedbfe104de7d9987eedc68864ab8acc0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.0 MB (31002934 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aca3e1ecca25fb97ad1d376d73b212cad11874d1f051c4c4bac1b2d27abc15fd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 02 Aug 2022 01:10:34 GMT
ADD file:6dc22a1e5b5fcf23f2549406ddcc45c4e244f46e21eafa881de81fa87438e5d8 in / 
# Tue, 02 Aug 2022 01:10:38 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 03:22:53 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 02 Aug 2022 03:23:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 04 Aug 2022 20:07:25 GMT
ENV MEMCACHED_VERSION=1.6.16
# Thu, 04 Aug 2022 20:07:28 GMT
ENV MEMCACHED_SHA1=724f31c3462fb6b07264d72d0043fd65545fd84a
# Thu, 04 Aug 2022 20:14:28 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 04 Aug 2022 20:14:30 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 04 Aug 2022 20:14:35 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 04 Aug 2022 20:14:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 04 Aug 2022 20:14:40 GMT
USER memcache
# Thu, 04 Aug 2022 20:14:42 GMT
EXPOSE 11211
# Thu, 04 Aug 2022 20:14:45 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:88350749a27614c791450c256b051f023d81cdd256211274b1efac493779d2be`  
		Last Modified: Tue, 02 Aug 2022 01:21:02 GMT  
		Size: 29.6 MB (29628964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:117af7bbaadea9c81bbaa3a8a77b1ab5cd05bcac856c462cda2e81c9a40596ab`  
		Last Modified: Tue, 02 Aug 2022 03:30:45 GMT  
		Size: 4.9 KB (4863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53a16d313748bd6b2dade87de73d79edd8a08e4cb662769a717f8587abc8d5e0`  
		Last Modified: Tue, 02 Aug 2022 03:30:46 GMT  
		Size: 117.1 KB (117127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d524786af3243ee367d118f6d5260cffa06d800f492f9b4bb36c910958186933`  
		Last Modified: Thu, 04 Aug 2022 20:15:05 GMT  
		Size: 1.3 MB (1251571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4badb1f1970762d08dbd43d7e101081a5fabd3c45e18afd70636397e83102d2f`  
		Last Modified: Thu, 04 Aug 2022 20:15:04 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3102636392803c3bbff48f39e7f143e3bf9a0528365d63b90dc31cd32060d3e0`  
		Last Modified: Thu, 04 Aug 2022 20:15:04 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1` - linux; ppc64le

```console
$ docker pull memcached@sha256:fef67c5248379f0c7154c6298ae0236afa239c6a2e7677ff26cf67e2e902873c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.0 MB (36957550 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19ebbfa2abfbf5d8014f1a3d04cab132b47836a64e68160efb3b8c752addaedd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 02 Aug 2022 01:17:30 GMT
ADD file:3a95a896d463569ce82199957052b3467123a4bd3385a0a4e397cf08402a99c3 in / 
# Tue, 02 Aug 2022 01:17:32 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 03:45:30 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 02 Aug 2022 03:45:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 04 Aug 2022 20:31:03 GMT
ENV MEMCACHED_VERSION=1.6.16
# Thu, 04 Aug 2022 20:31:04 GMT
ENV MEMCACHED_SHA1=724f31c3462fb6b07264d72d0043fd65545fd84a
# Thu, 04 Aug 2022 20:34:08 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 04 Aug 2022 20:34:09 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 04 Aug 2022 20:34:10 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 04 Aug 2022 20:34:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 04 Aug 2022 20:34:10 GMT
USER memcache
# Thu, 04 Aug 2022 20:34:11 GMT
EXPOSE 11211
# Thu, 04 Aug 2022 20:34:11 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:5241cd116d6e6e2d62f3d8c2245b74daca9f6cc154eaccd738feb41984c74714`  
		Last Modified: Tue, 02 Aug 2022 01:24:39 GMT  
		Size: 35.3 MB (35272771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58860b5324185f5059438d063f2a2b9c8ec05e058d0c1467db47a258a089c691`  
		Last Modified: Tue, 02 Aug 2022 03:53:12 GMT  
		Size: 5.0 KB (4978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82fb13381eff7e0b9526ba592f13e09cea5295914fde283ea341e5b71cb31493`  
		Last Modified: Tue, 02 Aug 2022 03:53:13 GMT  
		Size: 356.9 KB (356918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b33f6ac4fcd819056777e9462124dfc34dca6f35e1cae56a64d12bd150e4dfc9`  
		Last Modified: Thu, 04 Aug 2022 20:38:29 GMT  
		Size: 1.3 MB (1322475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:893b74576495c7a62c5d4447a7453f60f228fbb0e6d2dc4edf7e67661c455f57`  
		Last Modified: Thu, 04 Aug 2022 20:38:28 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7855d0c39dc9730d8ec3369fa86f770bd433a903eb346e9115b7442574441f24`  
		Last Modified: Thu, 04 Aug 2022 20:38:28 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1` - linux; s390x

```console
$ docker pull memcached@sha256:4f7e9706bfd16d98bfb48a6435c8359a167ab733777f16f24996cad3f431bdc5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.2 MB (31211398 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6739ca31062c74398fdfec102afbacead1c25fa0decf2fa14bdecdcb6b160543`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 02 Aug 2022 00:42:27 GMT
ADD file:c2afc8990930846fbe7c99bfdfe9ea562c75feb6e3c9122431f7c9f8b5e51a7f in / 
# Tue, 02 Aug 2022 00:42:29 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 02:37:02 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 02 Aug 2022 02:37:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 04 Aug 2022 20:28:18 GMT
ENV MEMCACHED_VERSION=1.6.16
# Thu, 04 Aug 2022 20:28:18 GMT
ENV MEMCACHED_SHA1=724f31c3462fb6b07264d72d0043fd65545fd84a
# Thu, 04 Aug 2022 20:31:37 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 04 Aug 2022 20:31:37 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 04 Aug 2022 20:31:37 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 04 Aug 2022 20:31:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 04 Aug 2022 20:31:38 GMT
USER memcache
# Thu, 04 Aug 2022 20:31:38 GMT
EXPOSE 11211
# Thu, 04 Aug 2022 20:31:38 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:026d311d0716db60eba0572ea784c21031f420960510cebcc383dc53949b4db8`  
		Last Modified: Tue, 02 Aug 2022 00:48:01 GMT  
		Size: 29.6 MB (29640259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0ffdb328e548bd6b6311c78665ac8cd3be8f0b2e09691701d9b0bae0924f8f5`  
		Last Modified: Tue, 02 Aug 2022 02:41:16 GMT  
		Size: 5.0 KB (5025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fbb9677007b0ebab2fe6feab520da1962d3fcffb3490aa844681a46fcb35749`  
		Last Modified: Tue, 02 Aug 2022 02:41:16 GMT  
		Size: 324.2 KB (324183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9c93abfa1f832f2e1f02fbe7b9a489735142c2051dafa7af20d985ff2e2106b`  
		Last Modified: Thu, 04 Aug 2022 20:36:17 GMT  
		Size: 1.2 MB (1241523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f78bf4cf172bedc6ad3c92b859859b10c0394104262328d5664ddc0b1488b29`  
		Last Modified: Thu, 04 Aug 2022 20:36:17 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6a26d2d4c34166613098e1380842f1355b534e2335a1dea2128c193b7f19bec`  
		Last Modified: Thu, 04 Aug 2022 20:36:16 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:1-alpine`

```console
$ docker pull memcached@sha256:69942a0c1666bd15245d423a255a64f4b8543546b7c0f40a1b421f64bc40fcb8
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
$ docker pull memcached@sha256:9b2ecb3fb8713d7c971eaf6e97150fcf34735d105bab81dd53e45d18da6c6b90
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3860216 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:22e40b7fd940b01ddffc7c8fddff80d89c6572d89d7c9664343a2c1e3efe389b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 18 Jul 2022 21:00:15 GMT
ADD file:a2648378045615c3785c752423b1afc8dc1c2b213393344f4d0ca17e7255c1cb in / 
# Mon, 18 Jul 2022 21:00:15 GMT
CMD ["/bin/sh"]
# Tue, 19 Jul 2022 01:33:13 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 19 Jul 2022 01:33:14 GMT
RUN apk add --no-cache libsasl
# Thu, 04 Aug 2022 20:02:18 GMT
ENV MEMCACHED_VERSION=1.6.16
# Thu, 04 Aug 2022 20:02:18 GMT
ENV MEMCACHED_SHA1=724f31c3462fb6b07264d72d0043fd65545fd84a
# Thu, 04 Aug 2022 20:05:09 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Thu, 04 Aug 2022 20:05:09 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 04 Aug 2022 20:05:09 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 04 Aug 2022 20:05:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 04 Aug 2022 20:05:10 GMT
USER memcache
# Thu, 04 Aug 2022 20:05:10 GMT
EXPOSE 11211
# Thu, 04 Aug 2022 20:05:10 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:530afca65e2ea04227630ae746e0c85b2bd1a179379cbf2b6501b49c4cab2ccc`  
		Last Modified: Mon, 18 Jul 2022 19:09:35 GMT  
		Size: 2.8 MB (2798806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3e13ff258fbd16cc42fcdb1bd800f73f4b380857d2a6096906444ec790c6542`  
		Last Modified: Tue, 19 Jul 2022 01:36:41 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90922b6720c8f20007711c5660b8269518b50979be1cef2cb4c0b12a7ac78ff7`  
		Last Modified: Tue, 19 Jul 2022 01:36:41 GMT  
		Size: 108.3 KB (108315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51aa27d6f4905ed1e531c58fa8d22676bfac86a2ba49c01894f95245d65329f7`  
		Last Modified: Thu, 04 Aug 2022 20:06:10 GMT  
		Size: 951.4 KB (951422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35e3d85200a71563435aa4bb45d98232f964b19c4facc2bc63d6ae3db816cbb4`  
		Last Modified: Thu, 04 Aug 2022 20:06:10 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74ba9b8d8a47b35ef57b45387b27d98410a32a2814a83a6cc686136b48fbb420`  
		Last Modified: Thu, 04 Aug 2022 20:06:10 GMT  
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
$ docker pull memcached@sha256:ad6951d968e4efe51c8da00a45147c17103c337177ececea11271806da36563d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.7 MB (3744755 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c64051372a720608fa1f9fed496d62daf26dd098c6ecf5189d59c3c4aede3d8f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 18 Jul 2022 21:57:05 GMT
ADD file:9ccb70abba88b6de789b29f17770246f765ffbb072fe598580bfc29ce3213f1c in / 
# Mon, 18 Jul 2022 21:57:05 GMT
CMD ["/bin/sh"]
# Mon, 18 Jul 2022 23:40:46 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Mon, 18 Jul 2022 23:40:48 GMT
RUN apk add --no-cache libsasl
# Thu, 04 Aug 2022 20:36:31 GMT
ENV MEMCACHED_VERSION=1.6.16
# Thu, 04 Aug 2022 20:36:32 GMT
ENV MEMCACHED_SHA1=724f31c3462fb6b07264d72d0043fd65545fd84a
# Thu, 04 Aug 2022 20:39:14 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Thu, 04 Aug 2022 20:39:16 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 04 Aug 2022 20:39:16 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 04 Aug 2022 20:39:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 04 Aug 2022 20:39:18 GMT
USER memcache
# Thu, 04 Aug 2022 20:39:19 GMT
EXPOSE 11211
# Thu, 04 Aug 2022 20:39:20 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:f97344484467e4c4ebb85aae724170073799295a3442c50ab532e249bd27b412`  
		Last Modified: Mon, 18 Jul 2022 19:08:29 GMT  
		Size: 2.7 MB (2694720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7da60570c25aa47c5a2b9fcd4be47a0a93240f9f4f2ab5a4d0b52c2646f40a28`  
		Last Modified: Mon, 18 Jul 2022 23:44:19 GMT  
		Size: 1.2 KB (1240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66a722c1c0875bed8b5bc87f4e2844ed10d7d9c12755721cd2164aa8b1c690d3`  
		Last Modified: Mon, 18 Jul 2022 23:44:20 GMT  
		Size: 109.6 KB (109554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19d417474c6b68c4c39d74d0adc463d1b8efd38f3c8f97b0a06230a45762e419`  
		Last Modified: Thu, 04 Aug 2022 20:40:30 GMT  
		Size: 938.8 KB (938833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9ffa798617a9bfdd85f3d0e02e2e00587f4a41d08fdf2f2cb2e1545b83c9090`  
		Last Modified: Thu, 04 Aug 2022 20:40:30 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:953ea2e6fdf83d907c05809ff46325d9d363d4cea34f88de5c84c87be30aa90d`  
		Last Modified: Thu, 04 Aug 2022 20:40:30 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-alpine` - linux; 386

```console
$ docker pull memcached@sha256:ee1fc765b96e3511c6b013639aec361b29013747c099430e8d347cf3692fac6e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3886569 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d6788e9d28dbe037c2a56c89130413dd2dcf2e394c99b8cfe32d79eecdaa1783`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 18 Jul 2022 20:38:19 GMT
ADD file:be69b7550bf861d8fb12bdbe1edf3a0d2519a6a4da61bd04858b6258ffbf48a7 in / 
# Mon, 18 Jul 2022 20:38:19 GMT
CMD ["/bin/sh"]
# Tue, 19 Jul 2022 01:27:41 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 19 Jul 2022 01:27:42 GMT
RUN apk add --no-cache libsasl
# Thu, 04 Aug 2022 20:31:52 GMT
ENV MEMCACHED_VERSION=1.6.16
# Thu, 04 Aug 2022 20:31:53 GMT
ENV MEMCACHED_SHA1=724f31c3462fb6b07264d72d0043fd65545fd84a
# Thu, 04 Aug 2022 20:34:46 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Thu, 04 Aug 2022 20:34:48 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 04 Aug 2022 20:34:48 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 04 Aug 2022 20:34:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 04 Aug 2022 20:34:50 GMT
USER memcache
# Thu, 04 Aug 2022 20:34:51 GMT
EXPOSE 11211
# Thu, 04 Aug 2022 20:34:52 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:5d7f927419794ebb7496ac38b0659686317b2d2fac7252a4a0d40d43d5fdd662`  
		Last Modified: Mon, 18 Jul 2022 19:09:22 GMT  
		Size: 2.8 MB (2802334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bd21aea877c073ddb40c30afa2f3e8f58c6fef7737835158747cf175df4ef4e`  
		Last Modified: Tue, 19 Jul 2022 01:31:30 GMT  
		Size: 1.2 KB (1241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fba37b4bd3e4b8bdb4184c8f065ce7b15f3fadd48bbb46f43623a90737e59911`  
		Last Modified: Tue, 19 Jul 2022 01:31:31 GMT  
		Size: 119.8 KB (119833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bf6c5b49cad3fa44a9ca5f146e497c4fb38ee5f14d27a2164224225a90e55aa`  
		Last Modified: Thu, 04 Aug 2022 20:36:09 GMT  
		Size: 962.8 KB (962757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cff8368515defad6347e63b43774e1ab0921279b4081ee4d8d36d28079e6c5d`  
		Last Modified: Thu, 04 Aug 2022 20:36:09 GMT  
		Size: 283.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e402b0471e504b912c3be68ebc0b6934213ca421d3b90ab8eb15f698c24157a`  
		Last Modified: Thu, 04 Aug 2022 20:36:09 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-alpine` - linux; ppc64le

```console
$ docker pull memcached@sha256:b9d56b200da6dd58c0da595669a18edfb7c77db42a4305b20a9a72c43b1bb034
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3898842 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4292cb4f0bd2997ab218f436690f4d170d349cead12c74fbc6c9acc4489ee307`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 18 Jul 2022 21:29:30 GMT
ADD file:69e4080f15f54e2d8f8aa25fdcba9c01dde149d43592edd5023106675e54a769 in / 
# Mon, 18 Jul 2022 21:29:31 GMT
CMD ["/bin/sh"]
# Tue, 02 Aug 2022 03:48:55 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 02 Aug 2022 03:48:57 GMT
RUN apk add --no-cache libsasl
# Thu, 04 Aug 2022 20:34:28 GMT
ENV MEMCACHED_VERSION=1.6.16
# Thu, 04 Aug 2022 20:34:29 GMT
ENV MEMCACHED_SHA1=724f31c3462fb6b07264d72d0043fd65545fd84a
# Thu, 04 Aug 2022 20:37:42 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Thu, 04 Aug 2022 20:37:42 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 04 Aug 2022 20:37:43 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 04 Aug 2022 20:37:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 04 Aug 2022 20:37:44 GMT
USER memcache
# Thu, 04 Aug 2022 20:37:44 GMT
EXPOSE 11211
# Thu, 04 Aug 2022 20:37:44 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:602896d442490cd3fbb6599f0f862d3673b7cd58eca3ac842b8e09bf8d012443`  
		Last Modified: Mon, 18 Jul 2022 19:09:09 GMT  
		Size: 2.8 MB (2789923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e6cec9872fd3c66c2b19cff2dd853136a16b03e523f70d0cd8875dff75abdf6`  
		Last Modified: Tue, 02 Aug 2022 03:53:48 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2420696d84e23c3f6e09fb61166d22a8b83d011559aa421d5d5e9f4ccf2f06a`  
		Last Modified: Tue, 02 Aug 2022 03:53:48 GMT  
		Size: 126.1 KB (126059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c706cce31e40f8bd79f2caa6ecef5e085849307288d79ebffc91b574118f04ba`  
		Last Modified: Thu, 04 Aug 2022 20:39:03 GMT  
		Size: 981.2 KB (981184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e86b61d9d1ecc2880ffc457445a2f5dcfaa3317fa84796de7bb78f30b5c31e15`  
		Last Modified: Thu, 04 Aug 2022 20:39:03 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74db60069b975f4fa4efaf1fe6ee2af6977e661683c83a54c141faff25255f11`  
		Last Modified: Thu, 04 Aug 2022 20:39:03 GMT  
		Size: 120.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-alpine` - linux; s390x

```console
$ docker pull memcached@sha256:62da518bff73ec0e140de7ecadbc4c0bbeaec3886cf144ac9deea64a95905fa7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.6 MB (3636817 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:057cc21d3a6bf40d3f50d6b8ce6d9004c65a7fb5a448f98761e044c79691adf5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 18 Jul 2022 20:41:35 GMT
ADD file:deaa573cd61e07709846a5300fb627a8610e9754129c085ed483ff8897d0c002 in / 
# Mon, 18 Jul 2022 20:41:36 GMT
CMD ["/bin/sh"]
# Mon, 18 Jul 2022 22:46:43 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Mon, 18 Jul 2022 22:46:46 GMT
RUN apk add --no-cache libsasl
# Thu, 04 Aug 2022 20:31:55 GMT
ENV MEMCACHED_VERSION=1.6.16
# Thu, 04 Aug 2022 20:31:55 GMT
ENV MEMCACHED_SHA1=724f31c3462fb6b07264d72d0043fd65545fd84a
# Thu, 04 Aug 2022 20:35:27 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Thu, 04 Aug 2022 20:35:27 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 04 Aug 2022 20:35:27 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 04 Aug 2022 20:35:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 04 Aug 2022 20:35:28 GMT
USER memcache
# Thu, 04 Aug 2022 20:35:28 GMT
EXPOSE 11211
# Thu, 04 Aug 2022 20:35:28 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:5f1840d5bacf4162a87f497e22d94bce946e660bdfce8eeefcbf7bd0beb193f3`  
		Last Modified: Mon, 18 Jul 2022 20:42:36 GMT  
		Size: 2.6 MB (2580798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2b6f46f9ccd4c19bfc103544d0d83ceef7feae4d70d25397d620ca381065659`  
		Last Modified: Mon, 18 Jul 2022 22:52:40 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f491a581763941ae0ec0ec035bdfb8073504d7fdc2eec6eb1e70878f26c16351`  
		Last Modified: Mon, 18 Jul 2022 22:52:40 GMT  
		Size: 112.5 KB (112503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:978f61b805ce2eb5610c877e3b8dc826f82016a7cf4af02737c7e2c44a1ede3f`  
		Last Modified: Thu, 04 Aug 2022 20:36:36 GMT  
		Size: 941.8 KB (941845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0a55bbbae5442cc2430fd5859fdd4c002e763bfe72f074645ea038f97652422`  
		Last Modified: Thu, 04 Aug 2022 20:36:36 GMT  
		Size: 283.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16ad3c74a3fe0b757743e632dbef104cea78e39b57e4155dab2020488d5b4546`  
		Last Modified: Thu, 04 Aug 2022 20:36:36 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:1-alpine3.16`

```console
$ docker pull memcached@sha256:6f612899171e3ec7380f48ca3bc4043482423db2462846c9a55124b44e3dee5d
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
$ docker pull memcached@sha256:9b2ecb3fb8713d7c971eaf6e97150fcf34735d105bab81dd53e45d18da6c6b90
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3860216 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:22e40b7fd940b01ddffc7c8fddff80d89c6572d89d7c9664343a2c1e3efe389b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 18 Jul 2022 21:00:15 GMT
ADD file:a2648378045615c3785c752423b1afc8dc1c2b213393344f4d0ca17e7255c1cb in / 
# Mon, 18 Jul 2022 21:00:15 GMT
CMD ["/bin/sh"]
# Tue, 19 Jul 2022 01:33:13 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 19 Jul 2022 01:33:14 GMT
RUN apk add --no-cache libsasl
# Thu, 04 Aug 2022 20:02:18 GMT
ENV MEMCACHED_VERSION=1.6.16
# Thu, 04 Aug 2022 20:02:18 GMT
ENV MEMCACHED_SHA1=724f31c3462fb6b07264d72d0043fd65545fd84a
# Thu, 04 Aug 2022 20:05:09 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Thu, 04 Aug 2022 20:05:09 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 04 Aug 2022 20:05:09 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 04 Aug 2022 20:05:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 04 Aug 2022 20:05:10 GMT
USER memcache
# Thu, 04 Aug 2022 20:05:10 GMT
EXPOSE 11211
# Thu, 04 Aug 2022 20:05:10 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:530afca65e2ea04227630ae746e0c85b2bd1a179379cbf2b6501b49c4cab2ccc`  
		Last Modified: Mon, 18 Jul 2022 19:09:35 GMT  
		Size: 2.8 MB (2798806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3e13ff258fbd16cc42fcdb1bd800f73f4b380857d2a6096906444ec790c6542`  
		Last Modified: Tue, 19 Jul 2022 01:36:41 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90922b6720c8f20007711c5660b8269518b50979be1cef2cb4c0b12a7ac78ff7`  
		Last Modified: Tue, 19 Jul 2022 01:36:41 GMT  
		Size: 108.3 KB (108315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51aa27d6f4905ed1e531c58fa8d22676bfac86a2ba49c01894f95245d65329f7`  
		Last Modified: Thu, 04 Aug 2022 20:06:10 GMT  
		Size: 951.4 KB (951422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35e3d85200a71563435aa4bb45d98232f964b19c4facc2bc63d6ae3db816cbb4`  
		Last Modified: Thu, 04 Aug 2022 20:06:10 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74ba9b8d8a47b35ef57b45387b27d98410a32a2814a83a6cc686136b48fbb420`  
		Last Modified: Thu, 04 Aug 2022 20:06:10 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-alpine3.16` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:ad6951d968e4efe51c8da00a45147c17103c337177ececea11271806da36563d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.7 MB (3744755 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c64051372a720608fa1f9fed496d62daf26dd098c6ecf5189d59c3c4aede3d8f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 18 Jul 2022 21:57:05 GMT
ADD file:9ccb70abba88b6de789b29f17770246f765ffbb072fe598580bfc29ce3213f1c in / 
# Mon, 18 Jul 2022 21:57:05 GMT
CMD ["/bin/sh"]
# Mon, 18 Jul 2022 23:40:46 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Mon, 18 Jul 2022 23:40:48 GMT
RUN apk add --no-cache libsasl
# Thu, 04 Aug 2022 20:36:31 GMT
ENV MEMCACHED_VERSION=1.6.16
# Thu, 04 Aug 2022 20:36:32 GMT
ENV MEMCACHED_SHA1=724f31c3462fb6b07264d72d0043fd65545fd84a
# Thu, 04 Aug 2022 20:39:14 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Thu, 04 Aug 2022 20:39:16 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 04 Aug 2022 20:39:16 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 04 Aug 2022 20:39:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 04 Aug 2022 20:39:18 GMT
USER memcache
# Thu, 04 Aug 2022 20:39:19 GMT
EXPOSE 11211
# Thu, 04 Aug 2022 20:39:20 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:f97344484467e4c4ebb85aae724170073799295a3442c50ab532e249bd27b412`  
		Last Modified: Mon, 18 Jul 2022 19:08:29 GMT  
		Size: 2.7 MB (2694720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7da60570c25aa47c5a2b9fcd4be47a0a93240f9f4f2ab5a4d0b52c2646f40a28`  
		Last Modified: Mon, 18 Jul 2022 23:44:19 GMT  
		Size: 1.2 KB (1240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66a722c1c0875bed8b5bc87f4e2844ed10d7d9c12755721cd2164aa8b1c690d3`  
		Last Modified: Mon, 18 Jul 2022 23:44:20 GMT  
		Size: 109.6 KB (109554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19d417474c6b68c4c39d74d0adc463d1b8efd38f3c8f97b0a06230a45762e419`  
		Last Modified: Thu, 04 Aug 2022 20:40:30 GMT  
		Size: 938.8 KB (938833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9ffa798617a9bfdd85f3d0e02e2e00587f4a41d08fdf2f2cb2e1545b83c9090`  
		Last Modified: Thu, 04 Aug 2022 20:40:30 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:953ea2e6fdf83d907c05809ff46325d9d363d4cea34f88de5c84c87be30aa90d`  
		Last Modified: Thu, 04 Aug 2022 20:40:30 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-alpine3.16` - linux; 386

```console
$ docker pull memcached@sha256:ee1fc765b96e3511c6b013639aec361b29013747c099430e8d347cf3692fac6e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3886569 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d6788e9d28dbe037c2a56c89130413dd2dcf2e394c99b8cfe32d79eecdaa1783`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 18 Jul 2022 20:38:19 GMT
ADD file:be69b7550bf861d8fb12bdbe1edf3a0d2519a6a4da61bd04858b6258ffbf48a7 in / 
# Mon, 18 Jul 2022 20:38:19 GMT
CMD ["/bin/sh"]
# Tue, 19 Jul 2022 01:27:41 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 19 Jul 2022 01:27:42 GMT
RUN apk add --no-cache libsasl
# Thu, 04 Aug 2022 20:31:52 GMT
ENV MEMCACHED_VERSION=1.6.16
# Thu, 04 Aug 2022 20:31:53 GMT
ENV MEMCACHED_SHA1=724f31c3462fb6b07264d72d0043fd65545fd84a
# Thu, 04 Aug 2022 20:34:46 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Thu, 04 Aug 2022 20:34:48 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 04 Aug 2022 20:34:48 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 04 Aug 2022 20:34:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 04 Aug 2022 20:34:50 GMT
USER memcache
# Thu, 04 Aug 2022 20:34:51 GMT
EXPOSE 11211
# Thu, 04 Aug 2022 20:34:52 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:5d7f927419794ebb7496ac38b0659686317b2d2fac7252a4a0d40d43d5fdd662`  
		Last Modified: Mon, 18 Jul 2022 19:09:22 GMT  
		Size: 2.8 MB (2802334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bd21aea877c073ddb40c30afa2f3e8f58c6fef7737835158747cf175df4ef4e`  
		Last Modified: Tue, 19 Jul 2022 01:31:30 GMT  
		Size: 1.2 KB (1241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fba37b4bd3e4b8bdb4184c8f065ce7b15f3fadd48bbb46f43623a90737e59911`  
		Last Modified: Tue, 19 Jul 2022 01:31:31 GMT  
		Size: 119.8 KB (119833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bf6c5b49cad3fa44a9ca5f146e497c4fb38ee5f14d27a2164224225a90e55aa`  
		Last Modified: Thu, 04 Aug 2022 20:36:09 GMT  
		Size: 962.8 KB (962757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cff8368515defad6347e63b43774e1ab0921279b4081ee4d8d36d28079e6c5d`  
		Last Modified: Thu, 04 Aug 2022 20:36:09 GMT  
		Size: 283.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e402b0471e504b912c3be68ebc0b6934213ca421d3b90ab8eb15f698c24157a`  
		Last Modified: Thu, 04 Aug 2022 20:36:09 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-alpine3.16` - linux; ppc64le

```console
$ docker pull memcached@sha256:b9d56b200da6dd58c0da595669a18edfb7c77db42a4305b20a9a72c43b1bb034
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3898842 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4292cb4f0bd2997ab218f436690f4d170d349cead12c74fbc6c9acc4489ee307`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 18 Jul 2022 21:29:30 GMT
ADD file:69e4080f15f54e2d8f8aa25fdcba9c01dde149d43592edd5023106675e54a769 in / 
# Mon, 18 Jul 2022 21:29:31 GMT
CMD ["/bin/sh"]
# Tue, 02 Aug 2022 03:48:55 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 02 Aug 2022 03:48:57 GMT
RUN apk add --no-cache libsasl
# Thu, 04 Aug 2022 20:34:28 GMT
ENV MEMCACHED_VERSION=1.6.16
# Thu, 04 Aug 2022 20:34:29 GMT
ENV MEMCACHED_SHA1=724f31c3462fb6b07264d72d0043fd65545fd84a
# Thu, 04 Aug 2022 20:37:42 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Thu, 04 Aug 2022 20:37:42 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 04 Aug 2022 20:37:43 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 04 Aug 2022 20:37:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 04 Aug 2022 20:37:44 GMT
USER memcache
# Thu, 04 Aug 2022 20:37:44 GMT
EXPOSE 11211
# Thu, 04 Aug 2022 20:37:44 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:602896d442490cd3fbb6599f0f862d3673b7cd58eca3ac842b8e09bf8d012443`  
		Last Modified: Mon, 18 Jul 2022 19:09:09 GMT  
		Size: 2.8 MB (2789923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e6cec9872fd3c66c2b19cff2dd853136a16b03e523f70d0cd8875dff75abdf6`  
		Last Modified: Tue, 02 Aug 2022 03:53:48 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2420696d84e23c3f6e09fb61166d22a8b83d011559aa421d5d5e9f4ccf2f06a`  
		Last Modified: Tue, 02 Aug 2022 03:53:48 GMT  
		Size: 126.1 KB (126059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c706cce31e40f8bd79f2caa6ecef5e085849307288d79ebffc91b574118f04ba`  
		Last Modified: Thu, 04 Aug 2022 20:39:03 GMT  
		Size: 981.2 KB (981184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e86b61d9d1ecc2880ffc457445a2f5dcfaa3317fa84796de7bb78f30b5c31e15`  
		Last Modified: Thu, 04 Aug 2022 20:39:03 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74db60069b975f4fa4efaf1fe6ee2af6977e661683c83a54c141faff25255f11`  
		Last Modified: Thu, 04 Aug 2022 20:39:03 GMT  
		Size: 120.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-alpine3.16` - linux; s390x

```console
$ docker pull memcached@sha256:62da518bff73ec0e140de7ecadbc4c0bbeaec3886cf144ac9deea64a95905fa7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.6 MB (3636817 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:057cc21d3a6bf40d3f50d6b8ce6d9004c65a7fb5a448f98761e044c79691adf5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 18 Jul 2022 20:41:35 GMT
ADD file:deaa573cd61e07709846a5300fb627a8610e9754129c085ed483ff8897d0c002 in / 
# Mon, 18 Jul 2022 20:41:36 GMT
CMD ["/bin/sh"]
# Mon, 18 Jul 2022 22:46:43 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Mon, 18 Jul 2022 22:46:46 GMT
RUN apk add --no-cache libsasl
# Thu, 04 Aug 2022 20:31:55 GMT
ENV MEMCACHED_VERSION=1.6.16
# Thu, 04 Aug 2022 20:31:55 GMT
ENV MEMCACHED_SHA1=724f31c3462fb6b07264d72d0043fd65545fd84a
# Thu, 04 Aug 2022 20:35:27 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Thu, 04 Aug 2022 20:35:27 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 04 Aug 2022 20:35:27 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 04 Aug 2022 20:35:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 04 Aug 2022 20:35:28 GMT
USER memcache
# Thu, 04 Aug 2022 20:35:28 GMT
EXPOSE 11211
# Thu, 04 Aug 2022 20:35:28 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:5f1840d5bacf4162a87f497e22d94bce946e660bdfce8eeefcbf7bd0beb193f3`  
		Last Modified: Mon, 18 Jul 2022 20:42:36 GMT  
		Size: 2.6 MB (2580798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2b6f46f9ccd4c19bfc103544d0d83ceef7feae4d70d25397d620ca381065659`  
		Last Modified: Mon, 18 Jul 2022 22:52:40 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f491a581763941ae0ec0ec035bdfb8073504d7fdc2eec6eb1e70878f26c16351`  
		Last Modified: Mon, 18 Jul 2022 22:52:40 GMT  
		Size: 112.5 KB (112503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:978f61b805ce2eb5610c877e3b8dc826f82016a7cf4af02737c7e2c44a1ede3f`  
		Last Modified: Thu, 04 Aug 2022 20:36:36 GMT  
		Size: 941.8 KB (941845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0a55bbbae5442cc2430fd5859fdd4c002e763bfe72f074645ea038f97652422`  
		Last Modified: Thu, 04 Aug 2022 20:36:36 GMT  
		Size: 283.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16ad3c74a3fe0b757743e632dbef104cea78e39b57e4155dab2020488d5b4546`  
		Last Modified: Thu, 04 Aug 2022 20:36:36 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:1-bullseye`

```console
$ docker pull memcached@sha256:0afaa8e890393e089efc991b62ec98d3dd53e5da995abfa548e5df9c70722015
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
$ docker pull memcached@sha256:d6479777ae4663bb6752d9e779a2180adeae2e6f91da834a6c042665ef961b19
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.0 MB (32956000 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:36a225838cd6927616fc3c9afc4fc26e1fbe4097250b113b6b8508e02ae6a589`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 02 Aug 2022 01:20:04 GMT
ADD file:0eae0dca665c7044bf242cb1fc92cb8ea744f5af2dd376a558c90bc47349aefe in / 
# Tue, 02 Aug 2022 01:20:05 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 04:45:12 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 02 Aug 2022 04:45:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 04 Aug 2022 19:59:25 GMT
ENV MEMCACHED_VERSION=1.6.16
# Thu, 04 Aug 2022 19:59:25 GMT
ENV MEMCACHED_SHA1=724f31c3462fb6b07264d72d0043fd65545fd84a
# Thu, 04 Aug 2022 20:02:08 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 04 Aug 2022 20:02:08 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 04 Aug 2022 20:02:08 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 04 Aug 2022 20:02:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 04 Aug 2022 20:02:09 GMT
USER memcache
# Thu, 04 Aug 2022 20:02:09 GMT
EXPOSE 11211
# Thu, 04 Aug 2022 20:02:09 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:1efc276f4ff952c055dea726cfc96ec6a4fdb8b62d9eed816bd2b788f2860ad7`  
		Last Modified: Tue, 02 Aug 2022 01:24:13 GMT  
		Size: 31.4 MB (31366757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60bd6790acf68c1ccc4757e879b51b4dbc273681e1f30606a2ccd4b55623d288`  
		Last Modified: Tue, 02 Aug 2022 04:48:24 GMT  
		Size: 5.0 KB (4980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e72821989d416909e21411733d7d034cfa908016dceb0b6e2717a5fb9faa617`  
		Last Modified: Tue, 02 Aug 2022 04:48:24 GMT  
		Size: 328.1 KB (328097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a972a764145eff4153208b9f8bed20e2179ececcec6e6d462d74400d526ccb4c`  
		Last Modified: Thu, 04 Aug 2022 20:05:45 GMT  
		Size: 1.3 MB (1255762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc9c8a212883923ae20b3e2d671f8dcc32307603465cf915c7e83bd5ac522c69`  
		Last Modified: Thu, 04 Aug 2022 20:05:45 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:157eedd0af5feece73dbebf45897c44894a10678feca71d5d57ac4904492badc`  
		Last Modified: Thu, 04 Aug 2022 20:05:46 GMT  
		Size: 118.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-bullseye` - linux; arm variant v5

```console
$ docker pull memcached@sha256:39515e68cebee2b2b88891c2b46b1c517587063301f77bbf7c312f6f9b372d65
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.5 MB (30454297 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8bf4bc30f264f1f9a0ede671e3a081ea54d1b6c3127ad5d9d4df3de21a985f5a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 02 Aug 2022 00:49:10 GMT
ADD file:4cd2f95737fd3007912428eeac56036c9e67e989e66cec08a8be99da47f88494 in / 
# Tue, 02 Aug 2022 00:49:10 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 01:58:42 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 02 Aug 2022 01:58:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 04 Aug 2022 19:50:51 GMT
ENV MEMCACHED_VERSION=1.6.16
# Thu, 04 Aug 2022 19:50:51 GMT
ENV MEMCACHED_SHA1=724f31c3462fb6b07264d72d0043fd65545fd84a
# Thu, 04 Aug 2022 19:56:43 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 04 Aug 2022 19:56:44 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 04 Aug 2022 19:56:44 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 04 Aug 2022 19:56:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 04 Aug 2022 19:56:44 GMT
USER memcache
# Thu, 04 Aug 2022 19:56:44 GMT
EXPOSE 11211
# Thu, 04 Aug 2022 19:56:45 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:5890b0ca6af5e8467a488e68716691950496a8f247d0495c2d595ddcb1893aff`  
		Last Modified: Tue, 02 Aug 2022 00:56:06 GMT  
		Size: 28.9 MB (28905515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e34350eb48491f2ab07c0f07724d37412df97ee9093c7c2458c9917afe37a42d`  
		Last Modified: Tue, 02 Aug 2022 02:04:59 GMT  
		Size: 4.9 KB (4894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36ecb6d2f4e3224a48197a5aa9d40970083bf4a92f41fbb493ac5adf9441a4ad`  
		Last Modified: Tue, 02 Aug 2022 02:04:59 GMT  
		Size: 316.6 KB (316628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e691cd60b95cdbb7fe7d3d74b1af54a56f440ac30d1dee94df4c4c370610b68d`  
		Last Modified: Thu, 04 Aug 2022 19:57:24 GMT  
		Size: 1.2 MB (1226852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8da76a828532ea569bd0e56b5a07a5e8bff4fe6efe22a5940260a261d113dc05`  
		Last Modified: Thu, 04 Aug 2022 19:57:23 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1705baeac52cb73666f9792b18547ce08509addd9ff3f19f6b91d21d5d10c8aa`  
		Last Modified: Thu, 04 Aug 2022 19:57:23 GMT  
		Size: 120.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-bullseye` - linux; arm variant v7

```console
$ docker pull memcached@sha256:25e768546f1e321b2a9031611f8ecd4081990c82f8774f7e051a5480cf18445d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.1 MB (28076294 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5959e4e12e1b75611311d3866bc95f9fe30048418f972e70fa2c671a66149fdd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 02 Aug 2022 00:58:59 GMT
ADD file:1575b776a15adacebc0875642e97a80807d42dcfc8917e1406d47af7ac244c97 in / 
# Tue, 02 Aug 2022 00:58:59 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 06:28:56 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 02 Aug 2022 06:29:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 04 Aug 2022 21:30:08 GMT
ENV MEMCACHED_VERSION=1.6.16
# Thu, 04 Aug 2022 21:30:08 GMT
ENV MEMCACHED_SHA1=724f31c3462fb6b07264d72d0043fd65545fd84a
# Thu, 04 Aug 2022 21:36:35 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 04 Aug 2022 21:36:35 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 04 Aug 2022 21:36:36 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 04 Aug 2022 21:36:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 04 Aug 2022 21:36:37 GMT
USER memcache
# Thu, 04 Aug 2022 21:36:37 GMT
EXPOSE 11211
# Thu, 04 Aug 2022 21:36:37 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:1dd75a3a9c893a7dc313f683dd62464b7eab6c6d522ee62c8a17022631830f32`  
		Last Modified: Tue, 02 Aug 2022 01:06:45 GMT  
		Size: 26.6 MB (26560586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44a675a8ce135f198539dc76b078733393238f7c7b899c8635980eed8f35f1cc`  
		Last Modified: Tue, 02 Aug 2022 09:35:13 GMT  
		Size: 4.9 KB (4890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:497b0afd04c92a1e5d41f58dbc0d5d544b8880d000c0ffbd03adb48c32c0116b`  
		Last Modified: Tue, 02 Aug 2022 09:35:13 GMT  
		Size: 312.1 KB (312067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8874fe992be272d0e0780725714c2439507699c15bfad1a073df948a34eb668d`  
		Last Modified: Fri, 05 Aug 2022 00:37:30 GMT  
		Size: 1.2 MB (1198344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cd5e042b98c640c152a56816e122c5e7b0abe91535d5d891dceed9748e42129`  
		Last Modified: Fri, 05 Aug 2022 00:37:29 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e871a0f93bdc7cb723e47f45514f914186b73d1890a53cdfe8525dd034926d59`  
		Last Modified: Fri, 05 Aug 2022 00:37:29 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-bullseye` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:759082b00d406f92781542ce86756eb73c5efe20acc7df6c25ac86be320a3ef5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.4 MB (31433439 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e91fe6663d9d90deed07c1d003a80fa6698137267c83310828f24a7ef63f6ef`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 02 Aug 2022 00:40:38 GMT
ADD file:6039adfbca55ed34a719c37672c664e3524130a0e2a3b8663629b8120b81b790 in / 
# Tue, 02 Aug 2022 00:40:39 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 03:56:15 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 02 Aug 2022 03:56:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 04 Aug 2022 20:33:46 GMT
ENV MEMCACHED_VERSION=1.6.16
# Thu, 04 Aug 2022 20:33:47 GMT
ENV MEMCACHED_SHA1=724f31c3462fb6b07264d72d0043fd65545fd84a
# Thu, 04 Aug 2022 20:36:17 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 04 Aug 2022 20:36:19 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 04 Aug 2022 20:36:19 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 04 Aug 2022 20:36:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 04 Aug 2022 20:36:21 GMT
USER memcache
# Thu, 04 Aug 2022 20:36:22 GMT
EXPOSE 11211
# Thu, 04 Aug 2022 20:36:23 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:a9fe95647e78b5516c7e2327355b6996e2ea295cd76ae242cbfe87f016b4e760`  
		Last Modified: Tue, 02 Aug 2022 00:46:05 GMT  
		Size: 30.1 MB (30054304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b983df009e7dc88033f53f015c09c56fd4db032d1abcade3333d8d4b515ff4af`  
		Last Modified: Tue, 02 Aug 2022 03:59:48 GMT  
		Size: 4.9 KB (4902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60720019405b50af041f391ec7dad90893ee95fc63fd6b3fb9da04850936f5db`  
		Last Modified: Tue, 02 Aug 2022 03:59:48 GMT  
		Size: 119.2 KB (119225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70569bedb4ee539337d6d3fd88e4076a1464b3a77bcfcca6604e18b815dbc402`  
		Last Modified: Thu, 04 Aug 2022 20:40:00 GMT  
		Size: 1.3 MB (1254600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:565112c01ad7b82688180f4fe70f5433126d79cc4b74e3d7f308601e2d34d9fe`  
		Last Modified: Thu, 04 Aug 2022 20:39:59 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce11290eb88924797c1fa048bd052c1243e4cb47e3469b26f3f1a3bc26472d19`  
		Last Modified: Thu, 04 Aug 2022 20:39:59 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-bullseye` - linux; 386

```console
$ docker pull memcached@sha256:deec44ba81c574f36b5b53185684413e4e97c3374d256e762ccf0e50fa1ff0f0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.8 MB (33762417 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9640d046f98daa1268a24f35ea7de08f83c728d88f2483d734101b09bad34768`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 02 Aug 2022 00:39:20 GMT
ADD file:f771e2286465694126158821089d801c7296376be2a56189e6041a15d2fe79f5 in / 
# Tue, 02 Aug 2022 00:39:21 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 03:12:03 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 02 Aug 2022 03:12:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 04 Aug 2022 20:28:41 GMT
ENV MEMCACHED_VERSION=1.6.16
# Thu, 04 Aug 2022 20:28:42 GMT
ENV MEMCACHED_SHA1=724f31c3462fb6b07264d72d0043fd65545fd84a
# Thu, 04 Aug 2022 20:31:30 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 04 Aug 2022 20:31:32 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 04 Aug 2022 20:31:32 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 04 Aug 2022 20:31:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 04 Aug 2022 20:31:34 GMT
USER memcache
# Thu, 04 Aug 2022 20:31:35 GMT
EXPOSE 11211
# Thu, 04 Aug 2022 20:31:36 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:90eb7f0ce9f33cf5dcd67d54c2fa606186dbaa5f95b6046f36145097267f9e53`  
		Last Modified: Tue, 02 Aug 2022 00:45:14 GMT  
		Size: 32.4 MB (32374054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:107cdc14debc414f1e6554b58402d2be697942f8f22b45d5c9b6bff8be3f332a`  
		Last Modified: Tue, 02 Aug 2022 03:15:55 GMT  
		Size: 4.8 KB (4771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b33bafb66f7f078457cf82ba6cfcbab5feae0e38bc0d959a5b50fa98fbcbf4ac`  
		Last Modified: Tue, 02 Aug 2022 03:15:55 GMT  
		Size: 130.1 KB (130114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c122afb77220a37620d69b968b43d326ed98ef7d9ed80ea06c3a7fa1c54dc73f`  
		Last Modified: Thu, 04 Aug 2022 20:35:38 GMT  
		Size: 1.3 MB (1253069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2426ab0684229e93e257d5c6357fbad018ee92d3cdcf5a7812171aa06bf82ca9`  
		Last Modified: Thu, 04 Aug 2022 20:35:38 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:240ed953e9e062d3ea6893fe34ecd1e5e060a240ae2a66092c6970c0be0eeed5`  
		Last Modified: Thu, 04 Aug 2022 20:35:38 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-bullseye` - linux; mips64le

```console
$ docker pull memcached@sha256:0d6798ccd4a9ac44c6ca7c358b2de6bdedbfe104de7d9987eedc68864ab8acc0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.0 MB (31002934 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aca3e1ecca25fb97ad1d376d73b212cad11874d1f051c4c4bac1b2d27abc15fd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 02 Aug 2022 01:10:34 GMT
ADD file:6dc22a1e5b5fcf23f2549406ddcc45c4e244f46e21eafa881de81fa87438e5d8 in / 
# Tue, 02 Aug 2022 01:10:38 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 03:22:53 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 02 Aug 2022 03:23:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 04 Aug 2022 20:07:25 GMT
ENV MEMCACHED_VERSION=1.6.16
# Thu, 04 Aug 2022 20:07:28 GMT
ENV MEMCACHED_SHA1=724f31c3462fb6b07264d72d0043fd65545fd84a
# Thu, 04 Aug 2022 20:14:28 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 04 Aug 2022 20:14:30 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 04 Aug 2022 20:14:35 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 04 Aug 2022 20:14:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 04 Aug 2022 20:14:40 GMT
USER memcache
# Thu, 04 Aug 2022 20:14:42 GMT
EXPOSE 11211
# Thu, 04 Aug 2022 20:14:45 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:88350749a27614c791450c256b051f023d81cdd256211274b1efac493779d2be`  
		Last Modified: Tue, 02 Aug 2022 01:21:02 GMT  
		Size: 29.6 MB (29628964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:117af7bbaadea9c81bbaa3a8a77b1ab5cd05bcac856c462cda2e81c9a40596ab`  
		Last Modified: Tue, 02 Aug 2022 03:30:45 GMT  
		Size: 4.9 KB (4863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53a16d313748bd6b2dade87de73d79edd8a08e4cb662769a717f8587abc8d5e0`  
		Last Modified: Tue, 02 Aug 2022 03:30:46 GMT  
		Size: 117.1 KB (117127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d524786af3243ee367d118f6d5260cffa06d800f492f9b4bb36c910958186933`  
		Last Modified: Thu, 04 Aug 2022 20:15:05 GMT  
		Size: 1.3 MB (1251571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4badb1f1970762d08dbd43d7e101081a5fabd3c45e18afd70636397e83102d2f`  
		Last Modified: Thu, 04 Aug 2022 20:15:04 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3102636392803c3bbff48f39e7f143e3bf9a0528365d63b90dc31cd32060d3e0`  
		Last Modified: Thu, 04 Aug 2022 20:15:04 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-bullseye` - linux; ppc64le

```console
$ docker pull memcached@sha256:fef67c5248379f0c7154c6298ae0236afa239c6a2e7677ff26cf67e2e902873c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.0 MB (36957550 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19ebbfa2abfbf5d8014f1a3d04cab132b47836a64e68160efb3b8c752addaedd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 02 Aug 2022 01:17:30 GMT
ADD file:3a95a896d463569ce82199957052b3467123a4bd3385a0a4e397cf08402a99c3 in / 
# Tue, 02 Aug 2022 01:17:32 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 03:45:30 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 02 Aug 2022 03:45:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 04 Aug 2022 20:31:03 GMT
ENV MEMCACHED_VERSION=1.6.16
# Thu, 04 Aug 2022 20:31:04 GMT
ENV MEMCACHED_SHA1=724f31c3462fb6b07264d72d0043fd65545fd84a
# Thu, 04 Aug 2022 20:34:08 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 04 Aug 2022 20:34:09 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 04 Aug 2022 20:34:10 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 04 Aug 2022 20:34:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 04 Aug 2022 20:34:10 GMT
USER memcache
# Thu, 04 Aug 2022 20:34:11 GMT
EXPOSE 11211
# Thu, 04 Aug 2022 20:34:11 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:5241cd116d6e6e2d62f3d8c2245b74daca9f6cc154eaccd738feb41984c74714`  
		Last Modified: Tue, 02 Aug 2022 01:24:39 GMT  
		Size: 35.3 MB (35272771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58860b5324185f5059438d063f2a2b9c8ec05e058d0c1467db47a258a089c691`  
		Last Modified: Tue, 02 Aug 2022 03:53:12 GMT  
		Size: 5.0 KB (4978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82fb13381eff7e0b9526ba592f13e09cea5295914fde283ea341e5b71cb31493`  
		Last Modified: Tue, 02 Aug 2022 03:53:13 GMT  
		Size: 356.9 KB (356918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b33f6ac4fcd819056777e9462124dfc34dca6f35e1cae56a64d12bd150e4dfc9`  
		Last Modified: Thu, 04 Aug 2022 20:38:29 GMT  
		Size: 1.3 MB (1322475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:893b74576495c7a62c5d4447a7453f60f228fbb0e6d2dc4edf7e67661c455f57`  
		Last Modified: Thu, 04 Aug 2022 20:38:28 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7855d0c39dc9730d8ec3369fa86f770bd433a903eb346e9115b7442574441f24`  
		Last Modified: Thu, 04 Aug 2022 20:38:28 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-bullseye` - linux; s390x

```console
$ docker pull memcached@sha256:4f7e9706bfd16d98bfb48a6435c8359a167ab733777f16f24996cad3f431bdc5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.2 MB (31211398 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6739ca31062c74398fdfec102afbacead1c25fa0decf2fa14bdecdcb6b160543`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 02 Aug 2022 00:42:27 GMT
ADD file:c2afc8990930846fbe7c99bfdfe9ea562c75feb6e3c9122431f7c9f8b5e51a7f in / 
# Tue, 02 Aug 2022 00:42:29 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 02:37:02 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 02 Aug 2022 02:37:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 04 Aug 2022 20:28:18 GMT
ENV MEMCACHED_VERSION=1.6.16
# Thu, 04 Aug 2022 20:28:18 GMT
ENV MEMCACHED_SHA1=724f31c3462fb6b07264d72d0043fd65545fd84a
# Thu, 04 Aug 2022 20:31:37 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 04 Aug 2022 20:31:37 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 04 Aug 2022 20:31:37 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 04 Aug 2022 20:31:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 04 Aug 2022 20:31:38 GMT
USER memcache
# Thu, 04 Aug 2022 20:31:38 GMT
EXPOSE 11211
# Thu, 04 Aug 2022 20:31:38 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:026d311d0716db60eba0572ea784c21031f420960510cebcc383dc53949b4db8`  
		Last Modified: Tue, 02 Aug 2022 00:48:01 GMT  
		Size: 29.6 MB (29640259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0ffdb328e548bd6b6311c78665ac8cd3be8f0b2e09691701d9b0bae0924f8f5`  
		Last Modified: Tue, 02 Aug 2022 02:41:16 GMT  
		Size: 5.0 KB (5025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fbb9677007b0ebab2fe6feab520da1962d3fcffb3490aa844681a46fcb35749`  
		Last Modified: Tue, 02 Aug 2022 02:41:16 GMT  
		Size: 324.2 KB (324183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9c93abfa1f832f2e1f02fbe7b9a489735142c2051dafa7af20d985ff2e2106b`  
		Last Modified: Thu, 04 Aug 2022 20:36:17 GMT  
		Size: 1.2 MB (1241523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f78bf4cf172bedc6ad3c92b859859b10c0394104262328d5664ddc0b1488b29`  
		Last Modified: Thu, 04 Aug 2022 20:36:17 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6a26d2d4c34166613098e1380842f1355b534e2335a1dea2128c193b7f19bec`  
		Last Modified: Thu, 04 Aug 2022 20:36:16 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:1.6`

```console
$ docker pull memcached@sha256:0afaa8e890393e089efc991b62ec98d3dd53e5da995abfa548e5df9c70722015
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
$ docker pull memcached@sha256:d6479777ae4663bb6752d9e779a2180adeae2e6f91da834a6c042665ef961b19
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.0 MB (32956000 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:36a225838cd6927616fc3c9afc4fc26e1fbe4097250b113b6b8508e02ae6a589`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 02 Aug 2022 01:20:04 GMT
ADD file:0eae0dca665c7044bf242cb1fc92cb8ea744f5af2dd376a558c90bc47349aefe in / 
# Tue, 02 Aug 2022 01:20:05 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 04:45:12 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 02 Aug 2022 04:45:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 04 Aug 2022 19:59:25 GMT
ENV MEMCACHED_VERSION=1.6.16
# Thu, 04 Aug 2022 19:59:25 GMT
ENV MEMCACHED_SHA1=724f31c3462fb6b07264d72d0043fd65545fd84a
# Thu, 04 Aug 2022 20:02:08 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 04 Aug 2022 20:02:08 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 04 Aug 2022 20:02:08 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 04 Aug 2022 20:02:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 04 Aug 2022 20:02:09 GMT
USER memcache
# Thu, 04 Aug 2022 20:02:09 GMT
EXPOSE 11211
# Thu, 04 Aug 2022 20:02:09 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:1efc276f4ff952c055dea726cfc96ec6a4fdb8b62d9eed816bd2b788f2860ad7`  
		Last Modified: Tue, 02 Aug 2022 01:24:13 GMT  
		Size: 31.4 MB (31366757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60bd6790acf68c1ccc4757e879b51b4dbc273681e1f30606a2ccd4b55623d288`  
		Last Modified: Tue, 02 Aug 2022 04:48:24 GMT  
		Size: 5.0 KB (4980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e72821989d416909e21411733d7d034cfa908016dceb0b6e2717a5fb9faa617`  
		Last Modified: Tue, 02 Aug 2022 04:48:24 GMT  
		Size: 328.1 KB (328097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a972a764145eff4153208b9f8bed20e2179ececcec6e6d462d74400d526ccb4c`  
		Last Modified: Thu, 04 Aug 2022 20:05:45 GMT  
		Size: 1.3 MB (1255762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc9c8a212883923ae20b3e2d671f8dcc32307603465cf915c7e83bd5ac522c69`  
		Last Modified: Thu, 04 Aug 2022 20:05:45 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:157eedd0af5feece73dbebf45897c44894a10678feca71d5d57ac4904492badc`  
		Last Modified: Thu, 04 Aug 2022 20:05:46 GMT  
		Size: 118.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6` - linux; arm variant v5

```console
$ docker pull memcached@sha256:39515e68cebee2b2b88891c2b46b1c517587063301f77bbf7c312f6f9b372d65
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.5 MB (30454297 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8bf4bc30f264f1f9a0ede671e3a081ea54d1b6c3127ad5d9d4df3de21a985f5a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 02 Aug 2022 00:49:10 GMT
ADD file:4cd2f95737fd3007912428eeac56036c9e67e989e66cec08a8be99da47f88494 in / 
# Tue, 02 Aug 2022 00:49:10 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 01:58:42 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 02 Aug 2022 01:58:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 04 Aug 2022 19:50:51 GMT
ENV MEMCACHED_VERSION=1.6.16
# Thu, 04 Aug 2022 19:50:51 GMT
ENV MEMCACHED_SHA1=724f31c3462fb6b07264d72d0043fd65545fd84a
# Thu, 04 Aug 2022 19:56:43 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 04 Aug 2022 19:56:44 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 04 Aug 2022 19:56:44 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 04 Aug 2022 19:56:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 04 Aug 2022 19:56:44 GMT
USER memcache
# Thu, 04 Aug 2022 19:56:44 GMT
EXPOSE 11211
# Thu, 04 Aug 2022 19:56:45 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:5890b0ca6af5e8467a488e68716691950496a8f247d0495c2d595ddcb1893aff`  
		Last Modified: Tue, 02 Aug 2022 00:56:06 GMT  
		Size: 28.9 MB (28905515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e34350eb48491f2ab07c0f07724d37412df97ee9093c7c2458c9917afe37a42d`  
		Last Modified: Tue, 02 Aug 2022 02:04:59 GMT  
		Size: 4.9 KB (4894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36ecb6d2f4e3224a48197a5aa9d40970083bf4a92f41fbb493ac5adf9441a4ad`  
		Last Modified: Tue, 02 Aug 2022 02:04:59 GMT  
		Size: 316.6 KB (316628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e691cd60b95cdbb7fe7d3d74b1af54a56f440ac30d1dee94df4c4c370610b68d`  
		Last Modified: Thu, 04 Aug 2022 19:57:24 GMT  
		Size: 1.2 MB (1226852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8da76a828532ea569bd0e56b5a07a5e8bff4fe6efe22a5940260a261d113dc05`  
		Last Modified: Thu, 04 Aug 2022 19:57:23 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1705baeac52cb73666f9792b18547ce08509addd9ff3f19f6b91d21d5d10c8aa`  
		Last Modified: Thu, 04 Aug 2022 19:57:23 GMT  
		Size: 120.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6` - linux; arm variant v7

```console
$ docker pull memcached@sha256:25e768546f1e321b2a9031611f8ecd4081990c82f8774f7e051a5480cf18445d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.1 MB (28076294 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5959e4e12e1b75611311d3866bc95f9fe30048418f972e70fa2c671a66149fdd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 02 Aug 2022 00:58:59 GMT
ADD file:1575b776a15adacebc0875642e97a80807d42dcfc8917e1406d47af7ac244c97 in / 
# Tue, 02 Aug 2022 00:58:59 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 06:28:56 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 02 Aug 2022 06:29:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 04 Aug 2022 21:30:08 GMT
ENV MEMCACHED_VERSION=1.6.16
# Thu, 04 Aug 2022 21:30:08 GMT
ENV MEMCACHED_SHA1=724f31c3462fb6b07264d72d0043fd65545fd84a
# Thu, 04 Aug 2022 21:36:35 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 04 Aug 2022 21:36:35 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 04 Aug 2022 21:36:36 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 04 Aug 2022 21:36:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 04 Aug 2022 21:36:37 GMT
USER memcache
# Thu, 04 Aug 2022 21:36:37 GMT
EXPOSE 11211
# Thu, 04 Aug 2022 21:36:37 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:1dd75a3a9c893a7dc313f683dd62464b7eab6c6d522ee62c8a17022631830f32`  
		Last Modified: Tue, 02 Aug 2022 01:06:45 GMT  
		Size: 26.6 MB (26560586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44a675a8ce135f198539dc76b078733393238f7c7b899c8635980eed8f35f1cc`  
		Last Modified: Tue, 02 Aug 2022 09:35:13 GMT  
		Size: 4.9 KB (4890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:497b0afd04c92a1e5d41f58dbc0d5d544b8880d000c0ffbd03adb48c32c0116b`  
		Last Modified: Tue, 02 Aug 2022 09:35:13 GMT  
		Size: 312.1 KB (312067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8874fe992be272d0e0780725714c2439507699c15bfad1a073df948a34eb668d`  
		Last Modified: Fri, 05 Aug 2022 00:37:30 GMT  
		Size: 1.2 MB (1198344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cd5e042b98c640c152a56816e122c5e7b0abe91535d5d891dceed9748e42129`  
		Last Modified: Fri, 05 Aug 2022 00:37:29 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e871a0f93bdc7cb723e47f45514f914186b73d1890a53cdfe8525dd034926d59`  
		Last Modified: Fri, 05 Aug 2022 00:37:29 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:759082b00d406f92781542ce86756eb73c5efe20acc7df6c25ac86be320a3ef5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.4 MB (31433439 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e91fe6663d9d90deed07c1d003a80fa6698137267c83310828f24a7ef63f6ef`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 02 Aug 2022 00:40:38 GMT
ADD file:6039adfbca55ed34a719c37672c664e3524130a0e2a3b8663629b8120b81b790 in / 
# Tue, 02 Aug 2022 00:40:39 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 03:56:15 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 02 Aug 2022 03:56:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 04 Aug 2022 20:33:46 GMT
ENV MEMCACHED_VERSION=1.6.16
# Thu, 04 Aug 2022 20:33:47 GMT
ENV MEMCACHED_SHA1=724f31c3462fb6b07264d72d0043fd65545fd84a
# Thu, 04 Aug 2022 20:36:17 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 04 Aug 2022 20:36:19 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 04 Aug 2022 20:36:19 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 04 Aug 2022 20:36:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 04 Aug 2022 20:36:21 GMT
USER memcache
# Thu, 04 Aug 2022 20:36:22 GMT
EXPOSE 11211
# Thu, 04 Aug 2022 20:36:23 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:a9fe95647e78b5516c7e2327355b6996e2ea295cd76ae242cbfe87f016b4e760`  
		Last Modified: Tue, 02 Aug 2022 00:46:05 GMT  
		Size: 30.1 MB (30054304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b983df009e7dc88033f53f015c09c56fd4db032d1abcade3333d8d4b515ff4af`  
		Last Modified: Tue, 02 Aug 2022 03:59:48 GMT  
		Size: 4.9 KB (4902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60720019405b50af041f391ec7dad90893ee95fc63fd6b3fb9da04850936f5db`  
		Last Modified: Tue, 02 Aug 2022 03:59:48 GMT  
		Size: 119.2 KB (119225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70569bedb4ee539337d6d3fd88e4076a1464b3a77bcfcca6604e18b815dbc402`  
		Last Modified: Thu, 04 Aug 2022 20:40:00 GMT  
		Size: 1.3 MB (1254600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:565112c01ad7b82688180f4fe70f5433126d79cc4b74e3d7f308601e2d34d9fe`  
		Last Modified: Thu, 04 Aug 2022 20:39:59 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce11290eb88924797c1fa048bd052c1243e4cb47e3469b26f3f1a3bc26472d19`  
		Last Modified: Thu, 04 Aug 2022 20:39:59 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6` - linux; 386

```console
$ docker pull memcached@sha256:deec44ba81c574f36b5b53185684413e4e97c3374d256e762ccf0e50fa1ff0f0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.8 MB (33762417 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9640d046f98daa1268a24f35ea7de08f83c728d88f2483d734101b09bad34768`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 02 Aug 2022 00:39:20 GMT
ADD file:f771e2286465694126158821089d801c7296376be2a56189e6041a15d2fe79f5 in / 
# Tue, 02 Aug 2022 00:39:21 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 03:12:03 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 02 Aug 2022 03:12:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 04 Aug 2022 20:28:41 GMT
ENV MEMCACHED_VERSION=1.6.16
# Thu, 04 Aug 2022 20:28:42 GMT
ENV MEMCACHED_SHA1=724f31c3462fb6b07264d72d0043fd65545fd84a
# Thu, 04 Aug 2022 20:31:30 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 04 Aug 2022 20:31:32 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 04 Aug 2022 20:31:32 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 04 Aug 2022 20:31:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 04 Aug 2022 20:31:34 GMT
USER memcache
# Thu, 04 Aug 2022 20:31:35 GMT
EXPOSE 11211
# Thu, 04 Aug 2022 20:31:36 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:90eb7f0ce9f33cf5dcd67d54c2fa606186dbaa5f95b6046f36145097267f9e53`  
		Last Modified: Tue, 02 Aug 2022 00:45:14 GMT  
		Size: 32.4 MB (32374054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:107cdc14debc414f1e6554b58402d2be697942f8f22b45d5c9b6bff8be3f332a`  
		Last Modified: Tue, 02 Aug 2022 03:15:55 GMT  
		Size: 4.8 KB (4771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b33bafb66f7f078457cf82ba6cfcbab5feae0e38bc0d959a5b50fa98fbcbf4ac`  
		Last Modified: Tue, 02 Aug 2022 03:15:55 GMT  
		Size: 130.1 KB (130114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c122afb77220a37620d69b968b43d326ed98ef7d9ed80ea06c3a7fa1c54dc73f`  
		Last Modified: Thu, 04 Aug 2022 20:35:38 GMT  
		Size: 1.3 MB (1253069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2426ab0684229e93e257d5c6357fbad018ee92d3cdcf5a7812171aa06bf82ca9`  
		Last Modified: Thu, 04 Aug 2022 20:35:38 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:240ed953e9e062d3ea6893fe34ecd1e5e060a240ae2a66092c6970c0be0eeed5`  
		Last Modified: Thu, 04 Aug 2022 20:35:38 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6` - linux; mips64le

```console
$ docker pull memcached@sha256:0d6798ccd4a9ac44c6ca7c358b2de6bdedbfe104de7d9987eedc68864ab8acc0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.0 MB (31002934 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aca3e1ecca25fb97ad1d376d73b212cad11874d1f051c4c4bac1b2d27abc15fd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 02 Aug 2022 01:10:34 GMT
ADD file:6dc22a1e5b5fcf23f2549406ddcc45c4e244f46e21eafa881de81fa87438e5d8 in / 
# Tue, 02 Aug 2022 01:10:38 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 03:22:53 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 02 Aug 2022 03:23:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 04 Aug 2022 20:07:25 GMT
ENV MEMCACHED_VERSION=1.6.16
# Thu, 04 Aug 2022 20:07:28 GMT
ENV MEMCACHED_SHA1=724f31c3462fb6b07264d72d0043fd65545fd84a
# Thu, 04 Aug 2022 20:14:28 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 04 Aug 2022 20:14:30 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 04 Aug 2022 20:14:35 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 04 Aug 2022 20:14:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 04 Aug 2022 20:14:40 GMT
USER memcache
# Thu, 04 Aug 2022 20:14:42 GMT
EXPOSE 11211
# Thu, 04 Aug 2022 20:14:45 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:88350749a27614c791450c256b051f023d81cdd256211274b1efac493779d2be`  
		Last Modified: Tue, 02 Aug 2022 01:21:02 GMT  
		Size: 29.6 MB (29628964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:117af7bbaadea9c81bbaa3a8a77b1ab5cd05bcac856c462cda2e81c9a40596ab`  
		Last Modified: Tue, 02 Aug 2022 03:30:45 GMT  
		Size: 4.9 KB (4863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53a16d313748bd6b2dade87de73d79edd8a08e4cb662769a717f8587abc8d5e0`  
		Last Modified: Tue, 02 Aug 2022 03:30:46 GMT  
		Size: 117.1 KB (117127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d524786af3243ee367d118f6d5260cffa06d800f492f9b4bb36c910958186933`  
		Last Modified: Thu, 04 Aug 2022 20:15:05 GMT  
		Size: 1.3 MB (1251571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4badb1f1970762d08dbd43d7e101081a5fabd3c45e18afd70636397e83102d2f`  
		Last Modified: Thu, 04 Aug 2022 20:15:04 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3102636392803c3bbff48f39e7f143e3bf9a0528365d63b90dc31cd32060d3e0`  
		Last Modified: Thu, 04 Aug 2022 20:15:04 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6` - linux; ppc64le

```console
$ docker pull memcached@sha256:fef67c5248379f0c7154c6298ae0236afa239c6a2e7677ff26cf67e2e902873c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.0 MB (36957550 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19ebbfa2abfbf5d8014f1a3d04cab132b47836a64e68160efb3b8c752addaedd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 02 Aug 2022 01:17:30 GMT
ADD file:3a95a896d463569ce82199957052b3467123a4bd3385a0a4e397cf08402a99c3 in / 
# Tue, 02 Aug 2022 01:17:32 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 03:45:30 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 02 Aug 2022 03:45:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 04 Aug 2022 20:31:03 GMT
ENV MEMCACHED_VERSION=1.6.16
# Thu, 04 Aug 2022 20:31:04 GMT
ENV MEMCACHED_SHA1=724f31c3462fb6b07264d72d0043fd65545fd84a
# Thu, 04 Aug 2022 20:34:08 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 04 Aug 2022 20:34:09 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 04 Aug 2022 20:34:10 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 04 Aug 2022 20:34:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 04 Aug 2022 20:34:10 GMT
USER memcache
# Thu, 04 Aug 2022 20:34:11 GMT
EXPOSE 11211
# Thu, 04 Aug 2022 20:34:11 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:5241cd116d6e6e2d62f3d8c2245b74daca9f6cc154eaccd738feb41984c74714`  
		Last Modified: Tue, 02 Aug 2022 01:24:39 GMT  
		Size: 35.3 MB (35272771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58860b5324185f5059438d063f2a2b9c8ec05e058d0c1467db47a258a089c691`  
		Last Modified: Tue, 02 Aug 2022 03:53:12 GMT  
		Size: 5.0 KB (4978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82fb13381eff7e0b9526ba592f13e09cea5295914fde283ea341e5b71cb31493`  
		Last Modified: Tue, 02 Aug 2022 03:53:13 GMT  
		Size: 356.9 KB (356918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b33f6ac4fcd819056777e9462124dfc34dca6f35e1cae56a64d12bd150e4dfc9`  
		Last Modified: Thu, 04 Aug 2022 20:38:29 GMT  
		Size: 1.3 MB (1322475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:893b74576495c7a62c5d4447a7453f60f228fbb0e6d2dc4edf7e67661c455f57`  
		Last Modified: Thu, 04 Aug 2022 20:38:28 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7855d0c39dc9730d8ec3369fa86f770bd433a903eb346e9115b7442574441f24`  
		Last Modified: Thu, 04 Aug 2022 20:38:28 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6` - linux; s390x

```console
$ docker pull memcached@sha256:4f7e9706bfd16d98bfb48a6435c8359a167ab733777f16f24996cad3f431bdc5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.2 MB (31211398 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6739ca31062c74398fdfec102afbacead1c25fa0decf2fa14bdecdcb6b160543`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 02 Aug 2022 00:42:27 GMT
ADD file:c2afc8990930846fbe7c99bfdfe9ea562c75feb6e3c9122431f7c9f8b5e51a7f in / 
# Tue, 02 Aug 2022 00:42:29 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 02:37:02 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 02 Aug 2022 02:37:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 04 Aug 2022 20:28:18 GMT
ENV MEMCACHED_VERSION=1.6.16
# Thu, 04 Aug 2022 20:28:18 GMT
ENV MEMCACHED_SHA1=724f31c3462fb6b07264d72d0043fd65545fd84a
# Thu, 04 Aug 2022 20:31:37 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 04 Aug 2022 20:31:37 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 04 Aug 2022 20:31:37 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 04 Aug 2022 20:31:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 04 Aug 2022 20:31:38 GMT
USER memcache
# Thu, 04 Aug 2022 20:31:38 GMT
EXPOSE 11211
# Thu, 04 Aug 2022 20:31:38 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:026d311d0716db60eba0572ea784c21031f420960510cebcc383dc53949b4db8`  
		Last Modified: Tue, 02 Aug 2022 00:48:01 GMT  
		Size: 29.6 MB (29640259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0ffdb328e548bd6b6311c78665ac8cd3be8f0b2e09691701d9b0bae0924f8f5`  
		Last Modified: Tue, 02 Aug 2022 02:41:16 GMT  
		Size: 5.0 KB (5025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fbb9677007b0ebab2fe6feab520da1962d3fcffb3490aa844681a46fcb35749`  
		Last Modified: Tue, 02 Aug 2022 02:41:16 GMT  
		Size: 324.2 KB (324183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9c93abfa1f832f2e1f02fbe7b9a489735142c2051dafa7af20d985ff2e2106b`  
		Last Modified: Thu, 04 Aug 2022 20:36:17 GMT  
		Size: 1.2 MB (1241523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f78bf4cf172bedc6ad3c92b859859b10c0394104262328d5664ddc0b1488b29`  
		Last Modified: Thu, 04 Aug 2022 20:36:17 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6a26d2d4c34166613098e1380842f1355b534e2335a1dea2128c193b7f19bec`  
		Last Modified: Thu, 04 Aug 2022 20:36:16 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:1.6-alpine`

```console
$ docker pull memcached@sha256:69942a0c1666bd15245d423a255a64f4b8543546b7c0f40a1b421f64bc40fcb8
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
$ docker pull memcached@sha256:9b2ecb3fb8713d7c971eaf6e97150fcf34735d105bab81dd53e45d18da6c6b90
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3860216 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:22e40b7fd940b01ddffc7c8fddff80d89c6572d89d7c9664343a2c1e3efe389b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 18 Jul 2022 21:00:15 GMT
ADD file:a2648378045615c3785c752423b1afc8dc1c2b213393344f4d0ca17e7255c1cb in / 
# Mon, 18 Jul 2022 21:00:15 GMT
CMD ["/bin/sh"]
# Tue, 19 Jul 2022 01:33:13 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 19 Jul 2022 01:33:14 GMT
RUN apk add --no-cache libsasl
# Thu, 04 Aug 2022 20:02:18 GMT
ENV MEMCACHED_VERSION=1.6.16
# Thu, 04 Aug 2022 20:02:18 GMT
ENV MEMCACHED_SHA1=724f31c3462fb6b07264d72d0043fd65545fd84a
# Thu, 04 Aug 2022 20:05:09 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Thu, 04 Aug 2022 20:05:09 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 04 Aug 2022 20:05:09 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 04 Aug 2022 20:05:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 04 Aug 2022 20:05:10 GMT
USER memcache
# Thu, 04 Aug 2022 20:05:10 GMT
EXPOSE 11211
# Thu, 04 Aug 2022 20:05:10 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:530afca65e2ea04227630ae746e0c85b2bd1a179379cbf2b6501b49c4cab2ccc`  
		Last Modified: Mon, 18 Jul 2022 19:09:35 GMT  
		Size: 2.8 MB (2798806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3e13ff258fbd16cc42fcdb1bd800f73f4b380857d2a6096906444ec790c6542`  
		Last Modified: Tue, 19 Jul 2022 01:36:41 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90922b6720c8f20007711c5660b8269518b50979be1cef2cb4c0b12a7ac78ff7`  
		Last Modified: Tue, 19 Jul 2022 01:36:41 GMT  
		Size: 108.3 KB (108315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51aa27d6f4905ed1e531c58fa8d22676bfac86a2ba49c01894f95245d65329f7`  
		Last Modified: Thu, 04 Aug 2022 20:06:10 GMT  
		Size: 951.4 KB (951422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35e3d85200a71563435aa4bb45d98232f964b19c4facc2bc63d6ae3db816cbb4`  
		Last Modified: Thu, 04 Aug 2022 20:06:10 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74ba9b8d8a47b35ef57b45387b27d98410a32a2814a83a6cc686136b48fbb420`  
		Last Modified: Thu, 04 Aug 2022 20:06:10 GMT  
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
$ docker pull memcached@sha256:ad6951d968e4efe51c8da00a45147c17103c337177ececea11271806da36563d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.7 MB (3744755 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c64051372a720608fa1f9fed496d62daf26dd098c6ecf5189d59c3c4aede3d8f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 18 Jul 2022 21:57:05 GMT
ADD file:9ccb70abba88b6de789b29f17770246f765ffbb072fe598580bfc29ce3213f1c in / 
# Mon, 18 Jul 2022 21:57:05 GMT
CMD ["/bin/sh"]
# Mon, 18 Jul 2022 23:40:46 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Mon, 18 Jul 2022 23:40:48 GMT
RUN apk add --no-cache libsasl
# Thu, 04 Aug 2022 20:36:31 GMT
ENV MEMCACHED_VERSION=1.6.16
# Thu, 04 Aug 2022 20:36:32 GMT
ENV MEMCACHED_SHA1=724f31c3462fb6b07264d72d0043fd65545fd84a
# Thu, 04 Aug 2022 20:39:14 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Thu, 04 Aug 2022 20:39:16 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 04 Aug 2022 20:39:16 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 04 Aug 2022 20:39:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 04 Aug 2022 20:39:18 GMT
USER memcache
# Thu, 04 Aug 2022 20:39:19 GMT
EXPOSE 11211
# Thu, 04 Aug 2022 20:39:20 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:f97344484467e4c4ebb85aae724170073799295a3442c50ab532e249bd27b412`  
		Last Modified: Mon, 18 Jul 2022 19:08:29 GMT  
		Size: 2.7 MB (2694720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7da60570c25aa47c5a2b9fcd4be47a0a93240f9f4f2ab5a4d0b52c2646f40a28`  
		Last Modified: Mon, 18 Jul 2022 23:44:19 GMT  
		Size: 1.2 KB (1240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66a722c1c0875bed8b5bc87f4e2844ed10d7d9c12755721cd2164aa8b1c690d3`  
		Last Modified: Mon, 18 Jul 2022 23:44:20 GMT  
		Size: 109.6 KB (109554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19d417474c6b68c4c39d74d0adc463d1b8efd38f3c8f97b0a06230a45762e419`  
		Last Modified: Thu, 04 Aug 2022 20:40:30 GMT  
		Size: 938.8 KB (938833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9ffa798617a9bfdd85f3d0e02e2e00587f4a41d08fdf2f2cb2e1545b83c9090`  
		Last Modified: Thu, 04 Aug 2022 20:40:30 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:953ea2e6fdf83d907c05809ff46325d9d363d4cea34f88de5c84c87be30aa90d`  
		Last Modified: Thu, 04 Aug 2022 20:40:30 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-alpine` - linux; 386

```console
$ docker pull memcached@sha256:ee1fc765b96e3511c6b013639aec361b29013747c099430e8d347cf3692fac6e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3886569 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d6788e9d28dbe037c2a56c89130413dd2dcf2e394c99b8cfe32d79eecdaa1783`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 18 Jul 2022 20:38:19 GMT
ADD file:be69b7550bf861d8fb12bdbe1edf3a0d2519a6a4da61bd04858b6258ffbf48a7 in / 
# Mon, 18 Jul 2022 20:38:19 GMT
CMD ["/bin/sh"]
# Tue, 19 Jul 2022 01:27:41 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 19 Jul 2022 01:27:42 GMT
RUN apk add --no-cache libsasl
# Thu, 04 Aug 2022 20:31:52 GMT
ENV MEMCACHED_VERSION=1.6.16
# Thu, 04 Aug 2022 20:31:53 GMT
ENV MEMCACHED_SHA1=724f31c3462fb6b07264d72d0043fd65545fd84a
# Thu, 04 Aug 2022 20:34:46 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Thu, 04 Aug 2022 20:34:48 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 04 Aug 2022 20:34:48 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 04 Aug 2022 20:34:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 04 Aug 2022 20:34:50 GMT
USER memcache
# Thu, 04 Aug 2022 20:34:51 GMT
EXPOSE 11211
# Thu, 04 Aug 2022 20:34:52 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:5d7f927419794ebb7496ac38b0659686317b2d2fac7252a4a0d40d43d5fdd662`  
		Last Modified: Mon, 18 Jul 2022 19:09:22 GMT  
		Size: 2.8 MB (2802334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bd21aea877c073ddb40c30afa2f3e8f58c6fef7737835158747cf175df4ef4e`  
		Last Modified: Tue, 19 Jul 2022 01:31:30 GMT  
		Size: 1.2 KB (1241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fba37b4bd3e4b8bdb4184c8f065ce7b15f3fadd48bbb46f43623a90737e59911`  
		Last Modified: Tue, 19 Jul 2022 01:31:31 GMT  
		Size: 119.8 KB (119833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bf6c5b49cad3fa44a9ca5f146e497c4fb38ee5f14d27a2164224225a90e55aa`  
		Last Modified: Thu, 04 Aug 2022 20:36:09 GMT  
		Size: 962.8 KB (962757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cff8368515defad6347e63b43774e1ab0921279b4081ee4d8d36d28079e6c5d`  
		Last Modified: Thu, 04 Aug 2022 20:36:09 GMT  
		Size: 283.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e402b0471e504b912c3be68ebc0b6934213ca421d3b90ab8eb15f698c24157a`  
		Last Modified: Thu, 04 Aug 2022 20:36:09 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-alpine` - linux; ppc64le

```console
$ docker pull memcached@sha256:b9d56b200da6dd58c0da595669a18edfb7c77db42a4305b20a9a72c43b1bb034
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3898842 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4292cb4f0bd2997ab218f436690f4d170d349cead12c74fbc6c9acc4489ee307`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 18 Jul 2022 21:29:30 GMT
ADD file:69e4080f15f54e2d8f8aa25fdcba9c01dde149d43592edd5023106675e54a769 in / 
# Mon, 18 Jul 2022 21:29:31 GMT
CMD ["/bin/sh"]
# Tue, 02 Aug 2022 03:48:55 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 02 Aug 2022 03:48:57 GMT
RUN apk add --no-cache libsasl
# Thu, 04 Aug 2022 20:34:28 GMT
ENV MEMCACHED_VERSION=1.6.16
# Thu, 04 Aug 2022 20:34:29 GMT
ENV MEMCACHED_SHA1=724f31c3462fb6b07264d72d0043fd65545fd84a
# Thu, 04 Aug 2022 20:37:42 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Thu, 04 Aug 2022 20:37:42 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 04 Aug 2022 20:37:43 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 04 Aug 2022 20:37:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 04 Aug 2022 20:37:44 GMT
USER memcache
# Thu, 04 Aug 2022 20:37:44 GMT
EXPOSE 11211
# Thu, 04 Aug 2022 20:37:44 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:602896d442490cd3fbb6599f0f862d3673b7cd58eca3ac842b8e09bf8d012443`  
		Last Modified: Mon, 18 Jul 2022 19:09:09 GMT  
		Size: 2.8 MB (2789923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e6cec9872fd3c66c2b19cff2dd853136a16b03e523f70d0cd8875dff75abdf6`  
		Last Modified: Tue, 02 Aug 2022 03:53:48 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2420696d84e23c3f6e09fb61166d22a8b83d011559aa421d5d5e9f4ccf2f06a`  
		Last Modified: Tue, 02 Aug 2022 03:53:48 GMT  
		Size: 126.1 KB (126059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c706cce31e40f8bd79f2caa6ecef5e085849307288d79ebffc91b574118f04ba`  
		Last Modified: Thu, 04 Aug 2022 20:39:03 GMT  
		Size: 981.2 KB (981184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e86b61d9d1ecc2880ffc457445a2f5dcfaa3317fa84796de7bb78f30b5c31e15`  
		Last Modified: Thu, 04 Aug 2022 20:39:03 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74db60069b975f4fa4efaf1fe6ee2af6977e661683c83a54c141faff25255f11`  
		Last Modified: Thu, 04 Aug 2022 20:39:03 GMT  
		Size: 120.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-alpine` - linux; s390x

```console
$ docker pull memcached@sha256:62da518bff73ec0e140de7ecadbc4c0bbeaec3886cf144ac9deea64a95905fa7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.6 MB (3636817 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:057cc21d3a6bf40d3f50d6b8ce6d9004c65a7fb5a448f98761e044c79691adf5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 18 Jul 2022 20:41:35 GMT
ADD file:deaa573cd61e07709846a5300fb627a8610e9754129c085ed483ff8897d0c002 in / 
# Mon, 18 Jul 2022 20:41:36 GMT
CMD ["/bin/sh"]
# Mon, 18 Jul 2022 22:46:43 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Mon, 18 Jul 2022 22:46:46 GMT
RUN apk add --no-cache libsasl
# Thu, 04 Aug 2022 20:31:55 GMT
ENV MEMCACHED_VERSION=1.6.16
# Thu, 04 Aug 2022 20:31:55 GMT
ENV MEMCACHED_SHA1=724f31c3462fb6b07264d72d0043fd65545fd84a
# Thu, 04 Aug 2022 20:35:27 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Thu, 04 Aug 2022 20:35:27 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 04 Aug 2022 20:35:27 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 04 Aug 2022 20:35:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 04 Aug 2022 20:35:28 GMT
USER memcache
# Thu, 04 Aug 2022 20:35:28 GMT
EXPOSE 11211
# Thu, 04 Aug 2022 20:35:28 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:5f1840d5bacf4162a87f497e22d94bce946e660bdfce8eeefcbf7bd0beb193f3`  
		Last Modified: Mon, 18 Jul 2022 20:42:36 GMT  
		Size: 2.6 MB (2580798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2b6f46f9ccd4c19bfc103544d0d83ceef7feae4d70d25397d620ca381065659`  
		Last Modified: Mon, 18 Jul 2022 22:52:40 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f491a581763941ae0ec0ec035bdfb8073504d7fdc2eec6eb1e70878f26c16351`  
		Last Modified: Mon, 18 Jul 2022 22:52:40 GMT  
		Size: 112.5 KB (112503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:978f61b805ce2eb5610c877e3b8dc826f82016a7cf4af02737c7e2c44a1ede3f`  
		Last Modified: Thu, 04 Aug 2022 20:36:36 GMT  
		Size: 941.8 KB (941845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0a55bbbae5442cc2430fd5859fdd4c002e763bfe72f074645ea038f97652422`  
		Last Modified: Thu, 04 Aug 2022 20:36:36 GMT  
		Size: 283.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16ad3c74a3fe0b757743e632dbef104cea78e39b57e4155dab2020488d5b4546`  
		Last Modified: Thu, 04 Aug 2022 20:36:36 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:1.6-alpine3.16`

```console
$ docker pull memcached@sha256:6f612899171e3ec7380f48ca3bc4043482423db2462846c9a55124b44e3dee5d
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
$ docker pull memcached@sha256:9b2ecb3fb8713d7c971eaf6e97150fcf34735d105bab81dd53e45d18da6c6b90
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3860216 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:22e40b7fd940b01ddffc7c8fddff80d89c6572d89d7c9664343a2c1e3efe389b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 18 Jul 2022 21:00:15 GMT
ADD file:a2648378045615c3785c752423b1afc8dc1c2b213393344f4d0ca17e7255c1cb in / 
# Mon, 18 Jul 2022 21:00:15 GMT
CMD ["/bin/sh"]
# Tue, 19 Jul 2022 01:33:13 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 19 Jul 2022 01:33:14 GMT
RUN apk add --no-cache libsasl
# Thu, 04 Aug 2022 20:02:18 GMT
ENV MEMCACHED_VERSION=1.6.16
# Thu, 04 Aug 2022 20:02:18 GMT
ENV MEMCACHED_SHA1=724f31c3462fb6b07264d72d0043fd65545fd84a
# Thu, 04 Aug 2022 20:05:09 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Thu, 04 Aug 2022 20:05:09 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 04 Aug 2022 20:05:09 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 04 Aug 2022 20:05:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 04 Aug 2022 20:05:10 GMT
USER memcache
# Thu, 04 Aug 2022 20:05:10 GMT
EXPOSE 11211
# Thu, 04 Aug 2022 20:05:10 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:530afca65e2ea04227630ae746e0c85b2bd1a179379cbf2b6501b49c4cab2ccc`  
		Last Modified: Mon, 18 Jul 2022 19:09:35 GMT  
		Size: 2.8 MB (2798806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3e13ff258fbd16cc42fcdb1bd800f73f4b380857d2a6096906444ec790c6542`  
		Last Modified: Tue, 19 Jul 2022 01:36:41 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90922b6720c8f20007711c5660b8269518b50979be1cef2cb4c0b12a7ac78ff7`  
		Last Modified: Tue, 19 Jul 2022 01:36:41 GMT  
		Size: 108.3 KB (108315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51aa27d6f4905ed1e531c58fa8d22676bfac86a2ba49c01894f95245d65329f7`  
		Last Modified: Thu, 04 Aug 2022 20:06:10 GMT  
		Size: 951.4 KB (951422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35e3d85200a71563435aa4bb45d98232f964b19c4facc2bc63d6ae3db816cbb4`  
		Last Modified: Thu, 04 Aug 2022 20:06:10 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74ba9b8d8a47b35ef57b45387b27d98410a32a2814a83a6cc686136b48fbb420`  
		Last Modified: Thu, 04 Aug 2022 20:06:10 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-alpine3.16` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:ad6951d968e4efe51c8da00a45147c17103c337177ececea11271806da36563d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.7 MB (3744755 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c64051372a720608fa1f9fed496d62daf26dd098c6ecf5189d59c3c4aede3d8f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 18 Jul 2022 21:57:05 GMT
ADD file:9ccb70abba88b6de789b29f17770246f765ffbb072fe598580bfc29ce3213f1c in / 
# Mon, 18 Jul 2022 21:57:05 GMT
CMD ["/bin/sh"]
# Mon, 18 Jul 2022 23:40:46 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Mon, 18 Jul 2022 23:40:48 GMT
RUN apk add --no-cache libsasl
# Thu, 04 Aug 2022 20:36:31 GMT
ENV MEMCACHED_VERSION=1.6.16
# Thu, 04 Aug 2022 20:36:32 GMT
ENV MEMCACHED_SHA1=724f31c3462fb6b07264d72d0043fd65545fd84a
# Thu, 04 Aug 2022 20:39:14 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Thu, 04 Aug 2022 20:39:16 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 04 Aug 2022 20:39:16 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 04 Aug 2022 20:39:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 04 Aug 2022 20:39:18 GMT
USER memcache
# Thu, 04 Aug 2022 20:39:19 GMT
EXPOSE 11211
# Thu, 04 Aug 2022 20:39:20 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:f97344484467e4c4ebb85aae724170073799295a3442c50ab532e249bd27b412`  
		Last Modified: Mon, 18 Jul 2022 19:08:29 GMT  
		Size: 2.7 MB (2694720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7da60570c25aa47c5a2b9fcd4be47a0a93240f9f4f2ab5a4d0b52c2646f40a28`  
		Last Modified: Mon, 18 Jul 2022 23:44:19 GMT  
		Size: 1.2 KB (1240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66a722c1c0875bed8b5bc87f4e2844ed10d7d9c12755721cd2164aa8b1c690d3`  
		Last Modified: Mon, 18 Jul 2022 23:44:20 GMT  
		Size: 109.6 KB (109554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19d417474c6b68c4c39d74d0adc463d1b8efd38f3c8f97b0a06230a45762e419`  
		Last Modified: Thu, 04 Aug 2022 20:40:30 GMT  
		Size: 938.8 KB (938833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9ffa798617a9bfdd85f3d0e02e2e00587f4a41d08fdf2f2cb2e1545b83c9090`  
		Last Modified: Thu, 04 Aug 2022 20:40:30 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:953ea2e6fdf83d907c05809ff46325d9d363d4cea34f88de5c84c87be30aa90d`  
		Last Modified: Thu, 04 Aug 2022 20:40:30 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-alpine3.16` - linux; 386

```console
$ docker pull memcached@sha256:ee1fc765b96e3511c6b013639aec361b29013747c099430e8d347cf3692fac6e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3886569 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d6788e9d28dbe037c2a56c89130413dd2dcf2e394c99b8cfe32d79eecdaa1783`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 18 Jul 2022 20:38:19 GMT
ADD file:be69b7550bf861d8fb12bdbe1edf3a0d2519a6a4da61bd04858b6258ffbf48a7 in / 
# Mon, 18 Jul 2022 20:38:19 GMT
CMD ["/bin/sh"]
# Tue, 19 Jul 2022 01:27:41 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 19 Jul 2022 01:27:42 GMT
RUN apk add --no-cache libsasl
# Thu, 04 Aug 2022 20:31:52 GMT
ENV MEMCACHED_VERSION=1.6.16
# Thu, 04 Aug 2022 20:31:53 GMT
ENV MEMCACHED_SHA1=724f31c3462fb6b07264d72d0043fd65545fd84a
# Thu, 04 Aug 2022 20:34:46 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Thu, 04 Aug 2022 20:34:48 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 04 Aug 2022 20:34:48 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 04 Aug 2022 20:34:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 04 Aug 2022 20:34:50 GMT
USER memcache
# Thu, 04 Aug 2022 20:34:51 GMT
EXPOSE 11211
# Thu, 04 Aug 2022 20:34:52 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:5d7f927419794ebb7496ac38b0659686317b2d2fac7252a4a0d40d43d5fdd662`  
		Last Modified: Mon, 18 Jul 2022 19:09:22 GMT  
		Size: 2.8 MB (2802334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bd21aea877c073ddb40c30afa2f3e8f58c6fef7737835158747cf175df4ef4e`  
		Last Modified: Tue, 19 Jul 2022 01:31:30 GMT  
		Size: 1.2 KB (1241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fba37b4bd3e4b8bdb4184c8f065ce7b15f3fadd48bbb46f43623a90737e59911`  
		Last Modified: Tue, 19 Jul 2022 01:31:31 GMT  
		Size: 119.8 KB (119833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bf6c5b49cad3fa44a9ca5f146e497c4fb38ee5f14d27a2164224225a90e55aa`  
		Last Modified: Thu, 04 Aug 2022 20:36:09 GMT  
		Size: 962.8 KB (962757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cff8368515defad6347e63b43774e1ab0921279b4081ee4d8d36d28079e6c5d`  
		Last Modified: Thu, 04 Aug 2022 20:36:09 GMT  
		Size: 283.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e402b0471e504b912c3be68ebc0b6934213ca421d3b90ab8eb15f698c24157a`  
		Last Modified: Thu, 04 Aug 2022 20:36:09 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-alpine3.16` - linux; ppc64le

```console
$ docker pull memcached@sha256:b9d56b200da6dd58c0da595669a18edfb7c77db42a4305b20a9a72c43b1bb034
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3898842 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4292cb4f0bd2997ab218f436690f4d170d349cead12c74fbc6c9acc4489ee307`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 18 Jul 2022 21:29:30 GMT
ADD file:69e4080f15f54e2d8f8aa25fdcba9c01dde149d43592edd5023106675e54a769 in / 
# Mon, 18 Jul 2022 21:29:31 GMT
CMD ["/bin/sh"]
# Tue, 02 Aug 2022 03:48:55 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 02 Aug 2022 03:48:57 GMT
RUN apk add --no-cache libsasl
# Thu, 04 Aug 2022 20:34:28 GMT
ENV MEMCACHED_VERSION=1.6.16
# Thu, 04 Aug 2022 20:34:29 GMT
ENV MEMCACHED_SHA1=724f31c3462fb6b07264d72d0043fd65545fd84a
# Thu, 04 Aug 2022 20:37:42 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Thu, 04 Aug 2022 20:37:42 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 04 Aug 2022 20:37:43 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 04 Aug 2022 20:37:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 04 Aug 2022 20:37:44 GMT
USER memcache
# Thu, 04 Aug 2022 20:37:44 GMT
EXPOSE 11211
# Thu, 04 Aug 2022 20:37:44 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:602896d442490cd3fbb6599f0f862d3673b7cd58eca3ac842b8e09bf8d012443`  
		Last Modified: Mon, 18 Jul 2022 19:09:09 GMT  
		Size: 2.8 MB (2789923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e6cec9872fd3c66c2b19cff2dd853136a16b03e523f70d0cd8875dff75abdf6`  
		Last Modified: Tue, 02 Aug 2022 03:53:48 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2420696d84e23c3f6e09fb61166d22a8b83d011559aa421d5d5e9f4ccf2f06a`  
		Last Modified: Tue, 02 Aug 2022 03:53:48 GMT  
		Size: 126.1 KB (126059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c706cce31e40f8bd79f2caa6ecef5e085849307288d79ebffc91b574118f04ba`  
		Last Modified: Thu, 04 Aug 2022 20:39:03 GMT  
		Size: 981.2 KB (981184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e86b61d9d1ecc2880ffc457445a2f5dcfaa3317fa84796de7bb78f30b5c31e15`  
		Last Modified: Thu, 04 Aug 2022 20:39:03 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74db60069b975f4fa4efaf1fe6ee2af6977e661683c83a54c141faff25255f11`  
		Last Modified: Thu, 04 Aug 2022 20:39:03 GMT  
		Size: 120.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-alpine3.16` - linux; s390x

```console
$ docker pull memcached@sha256:62da518bff73ec0e140de7ecadbc4c0bbeaec3886cf144ac9deea64a95905fa7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.6 MB (3636817 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:057cc21d3a6bf40d3f50d6b8ce6d9004c65a7fb5a448f98761e044c79691adf5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 18 Jul 2022 20:41:35 GMT
ADD file:deaa573cd61e07709846a5300fb627a8610e9754129c085ed483ff8897d0c002 in / 
# Mon, 18 Jul 2022 20:41:36 GMT
CMD ["/bin/sh"]
# Mon, 18 Jul 2022 22:46:43 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Mon, 18 Jul 2022 22:46:46 GMT
RUN apk add --no-cache libsasl
# Thu, 04 Aug 2022 20:31:55 GMT
ENV MEMCACHED_VERSION=1.6.16
# Thu, 04 Aug 2022 20:31:55 GMT
ENV MEMCACHED_SHA1=724f31c3462fb6b07264d72d0043fd65545fd84a
# Thu, 04 Aug 2022 20:35:27 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Thu, 04 Aug 2022 20:35:27 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 04 Aug 2022 20:35:27 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 04 Aug 2022 20:35:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 04 Aug 2022 20:35:28 GMT
USER memcache
# Thu, 04 Aug 2022 20:35:28 GMT
EXPOSE 11211
# Thu, 04 Aug 2022 20:35:28 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:5f1840d5bacf4162a87f497e22d94bce946e660bdfce8eeefcbf7bd0beb193f3`  
		Last Modified: Mon, 18 Jul 2022 20:42:36 GMT  
		Size: 2.6 MB (2580798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2b6f46f9ccd4c19bfc103544d0d83ceef7feae4d70d25397d620ca381065659`  
		Last Modified: Mon, 18 Jul 2022 22:52:40 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f491a581763941ae0ec0ec035bdfb8073504d7fdc2eec6eb1e70878f26c16351`  
		Last Modified: Mon, 18 Jul 2022 22:52:40 GMT  
		Size: 112.5 KB (112503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:978f61b805ce2eb5610c877e3b8dc826f82016a7cf4af02737c7e2c44a1ede3f`  
		Last Modified: Thu, 04 Aug 2022 20:36:36 GMT  
		Size: 941.8 KB (941845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0a55bbbae5442cc2430fd5859fdd4c002e763bfe72f074645ea038f97652422`  
		Last Modified: Thu, 04 Aug 2022 20:36:36 GMT  
		Size: 283.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16ad3c74a3fe0b757743e632dbef104cea78e39b57e4155dab2020488d5b4546`  
		Last Modified: Thu, 04 Aug 2022 20:36:36 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:1.6-bullseye`

```console
$ docker pull memcached@sha256:0afaa8e890393e089efc991b62ec98d3dd53e5da995abfa548e5df9c70722015
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
$ docker pull memcached@sha256:d6479777ae4663bb6752d9e779a2180adeae2e6f91da834a6c042665ef961b19
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.0 MB (32956000 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:36a225838cd6927616fc3c9afc4fc26e1fbe4097250b113b6b8508e02ae6a589`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 02 Aug 2022 01:20:04 GMT
ADD file:0eae0dca665c7044bf242cb1fc92cb8ea744f5af2dd376a558c90bc47349aefe in / 
# Tue, 02 Aug 2022 01:20:05 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 04:45:12 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 02 Aug 2022 04:45:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 04 Aug 2022 19:59:25 GMT
ENV MEMCACHED_VERSION=1.6.16
# Thu, 04 Aug 2022 19:59:25 GMT
ENV MEMCACHED_SHA1=724f31c3462fb6b07264d72d0043fd65545fd84a
# Thu, 04 Aug 2022 20:02:08 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 04 Aug 2022 20:02:08 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 04 Aug 2022 20:02:08 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 04 Aug 2022 20:02:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 04 Aug 2022 20:02:09 GMT
USER memcache
# Thu, 04 Aug 2022 20:02:09 GMT
EXPOSE 11211
# Thu, 04 Aug 2022 20:02:09 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:1efc276f4ff952c055dea726cfc96ec6a4fdb8b62d9eed816bd2b788f2860ad7`  
		Last Modified: Tue, 02 Aug 2022 01:24:13 GMT  
		Size: 31.4 MB (31366757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60bd6790acf68c1ccc4757e879b51b4dbc273681e1f30606a2ccd4b55623d288`  
		Last Modified: Tue, 02 Aug 2022 04:48:24 GMT  
		Size: 5.0 KB (4980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e72821989d416909e21411733d7d034cfa908016dceb0b6e2717a5fb9faa617`  
		Last Modified: Tue, 02 Aug 2022 04:48:24 GMT  
		Size: 328.1 KB (328097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a972a764145eff4153208b9f8bed20e2179ececcec6e6d462d74400d526ccb4c`  
		Last Modified: Thu, 04 Aug 2022 20:05:45 GMT  
		Size: 1.3 MB (1255762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc9c8a212883923ae20b3e2d671f8dcc32307603465cf915c7e83bd5ac522c69`  
		Last Modified: Thu, 04 Aug 2022 20:05:45 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:157eedd0af5feece73dbebf45897c44894a10678feca71d5d57ac4904492badc`  
		Last Modified: Thu, 04 Aug 2022 20:05:46 GMT  
		Size: 118.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-bullseye` - linux; arm variant v5

```console
$ docker pull memcached@sha256:39515e68cebee2b2b88891c2b46b1c517587063301f77bbf7c312f6f9b372d65
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.5 MB (30454297 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8bf4bc30f264f1f9a0ede671e3a081ea54d1b6c3127ad5d9d4df3de21a985f5a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 02 Aug 2022 00:49:10 GMT
ADD file:4cd2f95737fd3007912428eeac56036c9e67e989e66cec08a8be99da47f88494 in / 
# Tue, 02 Aug 2022 00:49:10 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 01:58:42 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 02 Aug 2022 01:58:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 04 Aug 2022 19:50:51 GMT
ENV MEMCACHED_VERSION=1.6.16
# Thu, 04 Aug 2022 19:50:51 GMT
ENV MEMCACHED_SHA1=724f31c3462fb6b07264d72d0043fd65545fd84a
# Thu, 04 Aug 2022 19:56:43 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 04 Aug 2022 19:56:44 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 04 Aug 2022 19:56:44 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 04 Aug 2022 19:56:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 04 Aug 2022 19:56:44 GMT
USER memcache
# Thu, 04 Aug 2022 19:56:44 GMT
EXPOSE 11211
# Thu, 04 Aug 2022 19:56:45 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:5890b0ca6af5e8467a488e68716691950496a8f247d0495c2d595ddcb1893aff`  
		Last Modified: Tue, 02 Aug 2022 00:56:06 GMT  
		Size: 28.9 MB (28905515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e34350eb48491f2ab07c0f07724d37412df97ee9093c7c2458c9917afe37a42d`  
		Last Modified: Tue, 02 Aug 2022 02:04:59 GMT  
		Size: 4.9 KB (4894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36ecb6d2f4e3224a48197a5aa9d40970083bf4a92f41fbb493ac5adf9441a4ad`  
		Last Modified: Tue, 02 Aug 2022 02:04:59 GMT  
		Size: 316.6 KB (316628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e691cd60b95cdbb7fe7d3d74b1af54a56f440ac30d1dee94df4c4c370610b68d`  
		Last Modified: Thu, 04 Aug 2022 19:57:24 GMT  
		Size: 1.2 MB (1226852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8da76a828532ea569bd0e56b5a07a5e8bff4fe6efe22a5940260a261d113dc05`  
		Last Modified: Thu, 04 Aug 2022 19:57:23 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1705baeac52cb73666f9792b18547ce08509addd9ff3f19f6b91d21d5d10c8aa`  
		Last Modified: Thu, 04 Aug 2022 19:57:23 GMT  
		Size: 120.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-bullseye` - linux; arm variant v7

```console
$ docker pull memcached@sha256:25e768546f1e321b2a9031611f8ecd4081990c82f8774f7e051a5480cf18445d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.1 MB (28076294 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5959e4e12e1b75611311d3866bc95f9fe30048418f972e70fa2c671a66149fdd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 02 Aug 2022 00:58:59 GMT
ADD file:1575b776a15adacebc0875642e97a80807d42dcfc8917e1406d47af7ac244c97 in / 
# Tue, 02 Aug 2022 00:58:59 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 06:28:56 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 02 Aug 2022 06:29:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 04 Aug 2022 21:30:08 GMT
ENV MEMCACHED_VERSION=1.6.16
# Thu, 04 Aug 2022 21:30:08 GMT
ENV MEMCACHED_SHA1=724f31c3462fb6b07264d72d0043fd65545fd84a
# Thu, 04 Aug 2022 21:36:35 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 04 Aug 2022 21:36:35 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 04 Aug 2022 21:36:36 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 04 Aug 2022 21:36:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 04 Aug 2022 21:36:37 GMT
USER memcache
# Thu, 04 Aug 2022 21:36:37 GMT
EXPOSE 11211
# Thu, 04 Aug 2022 21:36:37 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:1dd75a3a9c893a7dc313f683dd62464b7eab6c6d522ee62c8a17022631830f32`  
		Last Modified: Tue, 02 Aug 2022 01:06:45 GMT  
		Size: 26.6 MB (26560586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44a675a8ce135f198539dc76b078733393238f7c7b899c8635980eed8f35f1cc`  
		Last Modified: Tue, 02 Aug 2022 09:35:13 GMT  
		Size: 4.9 KB (4890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:497b0afd04c92a1e5d41f58dbc0d5d544b8880d000c0ffbd03adb48c32c0116b`  
		Last Modified: Tue, 02 Aug 2022 09:35:13 GMT  
		Size: 312.1 KB (312067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8874fe992be272d0e0780725714c2439507699c15bfad1a073df948a34eb668d`  
		Last Modified: Fri, 05 Aug 2022 00:37:30 GMT  
		Size: 1.2 MB (1198344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cd5e042b98c640c152a56816e122c5e7b0abe91535d5d891dceed9748e42129`  
		Last Modified: Fri, 05 Aug 2022 00:37:29 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e871a0f93bdc7cb723e47f45514f914186b73d1890a53cdfe8525dd034926d59`  
		Last Modified: Fri, 05 Aug 2022 00:37:29 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-bullseye` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:759082b00d406f92781542ce86756eb73c5efe20acc7df6c25ac86be320a3ef5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.4 MB (31433439 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e91fe6663d9d90deed07c1d003a80fa6698137267c83310828f24a7ef63f6ef`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 02 Aug 2022 00:40:38 GMT
ADD file:6039adfbca55ed34a719c37672c664e3524130a0e2a3b8663629b8120b81b790 in / 
# Tue, 02 Aug 2022 00:40:39 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 03:56:15 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 02 Aug 2022 03:56:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 04 Aug 2022 20:33:46 GMT
ENV MEMCACHED_VERSION=1.6.16
# Thu, 04 Aug 2022 20:33:47 GMT
ENV MEMCACHED_SHA1=724f31c3462fb6b07264d72d0043fd65545fd84a
# Thu, 04 Aug 2022 20:36:17 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 04 Aug 2022 20:36:19 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 04 Aug 2022 20:36:19 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 04 Aug 2022 20:36:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 04 Aug 2022 20:36:21 GMT
USER memcache
# Thu, 04 Aug 2022 20:36:22 GMT
EXPOSE 11211
# Thu, 04 Aug 2022 20:36:23 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:a9fe95647e78b5516c7e2327355b6996e2ea295cd76ae242cbfe87f016b4e760`  
		Last Modified: Tue, 02 Aug 2022 00:46:05 GMT  
		Size: 30.1 MB (30054304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b983df009e7dc88033f53f015c09c56fd4db032d1abcade3333d8d4b515ff4af`  
		Last Modified: Tue, 02 Aug 2022 03:59:48 GMT  
		Size: 4.9 KB (4902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60720019405b50af041f391ec7dad90893ee95fc63fd6b3fb9da04850936f5db`  
		Last Modified: Tue, 02 Aug 2022 03:59:48 GMT  
		Size: 119.2 KB (119225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70569bedb4ee539337d6d3fd88e4076a1464b3a77bcfcca6604e18b815dbc402`  
		Last Modified: Thu, 04 Aug 2022 20:40:00 GMT  
		Size: 1.3 MB (1254600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:565112c01ad7b82688180f4fe70f5433126d79cc4b74e3d7f308601e2d34d9fe`  
		Last Modified: Thu, 04 Aug 2022 20:39:59 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce11290eb88924797c1fa048bd052c1243e4cb47e3469b26f3f1a3bc26472d19`  
		Last Modified: Thu, 04 Aug 2022 20:39:59 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-bullseye` - linux; 386

```console
$ docker pull memcached@sha256:deec44ba81c574f36b5b53185684413e4e97c3374d256e762ccf0e50fa1ff0f0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.8 MB (33762417 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9640d046f98daa1268a24f35ea7de08f83c728d88f2483d734101b09bad34768`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 02 Aug 2022 00:39:20 GMT
ADD file:f771e2286465694126158821089d801c7296376be2a56189e6041a15d2fe79f5 in / 
# Tue, 02 Aug 2022 00:39:21 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 03:12:03 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 02 Aug 2022 03:12:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 04 Aug 2022 20:28:41 GMT
ENV MEMCACHED_VERSION=1.6.16
# Thu, 04 Aug 2022 20:28:42 GMT
ENV MEMCACHED_SHA1=724f31c3462fb6b07264d72d0043fd65545fd84a
# Thu, 04 Aug 2022 20:31:30 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 04 Aug 2022 20:31:32 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 04 Aug 2022 20:31:32 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 04 Aug 2022 20:31:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 04 Aug 2022 20:31:34 GMT
USER memcache
# Thu, 04 Aug 2022 20:31:35 GMT
EXPOSE 11211
# Thu, 04 Aug 2022 20:31:36 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:90eb7f0ce9f33cf5dcd67d54c2fa606186dbaa5f95b6046f36145097267f9e53`  
		Last Modified: Tue, 02 Aug 2022 00:45:14 GMT  
		Size: 32.4 MB (32374054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:107cdc14debc414f1e6554b58402d2be697942f8f22b45d5c9b6bff8be3f332a`  
		Last Modified: Tue, 02 Aug 2022 03:15:55 GMT  
		Size: 4.8 KB (4771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b33bafb66f7f078457cf82ba6cfcbab5feae0e38bc0d959a5b50fa98fbcbf4ac`  
		Last Modified: Tue, 02 Aug 2022 03:15:55 GMT  
		Size: 130.1 KB (130114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c122afb77220a37620d69b968b43d326ed98ef7d9ed80ea06c3a7fa1c54dc73f`  
		Last Modified: Thu, 04 Aug 2022 20:35:38 GMT  
		Size: 1.3 MB (1253069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2426ab0684229e93e257d5c6357fbad018ee92d3cdcf5a7812171aa06bf82ca9`  
		Last Modified: Thu, 04 Aug 2022 20:35:38 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:240ed953e9e062d3ea6893fe34ecd1e5e060a240ae2a66092c6970c0be0eeed5`  
		Last Modified: Thu, 04 Aug 2022 20:35:38 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-bullseye` - linux; mips64le

```console
$ docker pull memcached@sha256:0d6798ccd4a9ac44c6ca7c358b2de6bdedbfe104de7d9987eedc68864ab8acc0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.0 MB (31002934 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aca3e1ecca25fb97ad1d376d73b212cad11874d1f051c4c4bac1b2d27abc15fd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 02 Aug 2022 01:10:34 GMT
ADD file:6dc22a1e5b5fcf23f2549406ddcc45c4e244f46e21eafa881de81fa87438e5d8 in / 
# Tue, 02 Aug 2022 01:10:38 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 03:22:53 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 02 Aug 2022 03:23:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 04 Aug 2022 20:07:25 GMT
ENV MEMCACHED_VERSION=1.6.16
# Thu, 04 Aug 2022 20:07:28 GMT
ENV MEMCACHED_SHA1=724f31c3462fb6b07264d72d0043fd65545fd84a
# Thu, 04 Aug 2022 20:14:28 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 04 Aug 2022 20:14:30 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 04 Aug 2022 20:14:35 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 04 Aug 2022 20:14:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 04 Aug 2022 20:14:40 GMT
USER memcache
# Thu, 04 Aug 2022 20:14:42 GMT
EXPOSE 11211
# Thu, 04 Aug 2022 20:14:45 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:88350749a27614c791450c256b051f023d81cdd256211274b1efac493779d2be`  
		Last Modified: Tue, 02 Aug 2022 01:21:02 GMT  
		Size: 29.6 MB (29628964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:117af7bbaadea9c81bbaa3a8a77b1ab5cd05bcac856c462cda2e81c9a40596ab`  
		Last Modified: Tue, 02 Aug 2022 03:30:45 GMT  
		Size: 4.9 KB (4863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53a16d313748bd6b2dade87de73d79edd8a08e4cb662769a717f8587abc8d5e0`  
		Last Modified: Tue, 02 Aug 2022 03:30:46 GMT  
		Size: 117.1 KB (117127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d524786af3243ee367d118f6d5260cffa06d800f492f9b4bb36c910958186933`  
		Last Modified: Thu, 04 Aug 2022 20:15:05 GMT  
		Size: 1.3 MB (1251571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4badb1f1970762d08dbd43d7e101081a5fabd3c45e18afd70636397e83102d2f`  
		Last Modified: Thu, 04 Aug 2022 20:15:04 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3102636392803c3bbff48f39e7f143e3bf9a0528365d63b90dc31cd32060d3e0`  
		Last Modified: Thu, 04 Aug 2022 20:15:04 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-bullseye` - linux; ppc64le

```console
$ docker pull memcached@sha256:fef67c5248379f0c7154c6298ae0236afa239c6a2e7677ff26cf67e2e902873c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.0 MB (36957550 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19ebbfa2abfbf5d8014f1a3d04cab132b47836a64e68160efb3b8c752addaedd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 02 Aug 2022 01:17:30 GMT
ADD file:3a95a896d463569ce82199957052b3467123a4bd3385a0a4e397cf08402a99c3 in / 
# Tue, 02 Aug 2022 01:17:32 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 03:45:30 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 02 Aug 2022 03:45:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 04 Aug 2022 20:31:03 GMT
ENV MEMCACHED_VERSION=1.6.16
# Thu, 04 Aug 2022 20:31:04 GMT
ENV MEMCACHED_SHA1=724f31c3462fb6b07264d72d0043fd65545fd84a
# Thu, 04 Aug 2022 20:34:08 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 04 Aug 2022 20:34:09 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 04 Aug 2022 20:34:10 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 04 Aug 2022 20:34:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 04 Aug 2022 20:34:10 GMT
USER memcache
# Thu, 04 Aug 2022 20:34:11 GMT
EXPOSE 11211
# Thu, 04 Aug 2022 20:34:11 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:5241cd116d6e6e2d62f3d8c2245b74daca9f6cc154eaccd738feb41984c74714`  
		Last Modified: Tue, 02 Aug 2022 01:24:39 GMT  
		Size: 35.3 MB (35272771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58860b5324185f5059438d063f2a2b9c8ec05e058d0c1467db47a258a089c691`  
		Last Modified: Tue, 02 Aug 2022 03:53:12 GMT  
		Size: 5.0 KB (4978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82fb13381eff7e0b9526ba592f13e09cea5295914fde283ea341e5b71cb31493`  
		Last Modified: Tue, 02 Aug 2022 03:53:13 GMT  
		Size: 356.9 KB (356918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b33f6ac4fcd819056777e9462124dfc34dca6f35e1cae56a64d12bd150e4dfc9`  
		Last Modified: Thu, 04 Aug 2022 20:38:29 GMT  
		Size: 1.3 MB (1322475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:893b74576495c7a62c5d4447a7453f60f228fbb0e6d2dc4edf7e67661c455f57`  
		Last Modified: Thu, 04 Aug 2022 20:38:28 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7855d0c39dc9730d8ec3369fa86f770bd433a903eb346e9115b7442574441f24`  
		Last Modified: Thu, 04 Aug 2022 20:38:28 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-bullseye` - linux; s390x

```console
$ docker pull memcached@sha256:4f7e9706bfd16d98bfb48a6435c8359a167ab733777f16f24996cad3f431bdc5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.2 MB (31211398 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6739ca31062c74398fdfec102afbacead1c25fa0decf2fa14bdecdcb6b160543`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 02 Aug 2022 00:42:27 GMT
ADD file:c2afc8990930846fbe7c99bfdfe9ea562c75feb6e3c9122431f7c9f8b5e51a7f in / 
# Tue, 02 Aug 2022 00:42:29 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 02:37:02 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 02 Aug 2022 02:37:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 04 Aug 2022 20:28:18 GMT
ENV MEMCACHED_VERSION=1.6.16
# Thu, 04 Aug 2022 20:28:18 GMT
ENV MEMCACHED_SHA1=724f31c3462fb6b07264d72d0043fd65545fd84a
# Thu, 04 Aug 2022 20:31:37 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 04 Aug 2022 20:31:37 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 04 Aug 2022 20:31:37 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 04 Aug 2022 20:31:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 04 Aug 2022 20:31:38 GMT
USER memcache
# Thu, 04 Aug 2022 20:31:38 GMT
EXPOSE 11211
# Thu, 04 Aug 2022 20:31:38 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:026d311d0716db60eba0572ea784c21031f420960510cebcc383dc53949b4db8`  
		Last Modified: Tue, 02 Aug 2022 00:48:01 GMT  
		Size: 29.6 MB (29640259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0ffdb328e548bd6b6311c78665ac8cd3be8f0b2e09691701d9b0bae0924f8f5`  
		Last Modified: Tue, 02 Aug 2022 02:41:16 GMT  
		Size: 5.0 KB (5025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fbb9677007b0ebab2fe6feab520da1962d3fcffb3490aa844681a46fcb35749`  
		Last Modified: Tue, 02 Aug 2022 02:41:16 GMT  
		Size: 324.2 KB (324183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9c93abfa1f832f2e1f02fbe7b9a489735142c2051dafa7af20d985ff2e2106b`  
		Last Modified: Thu, 04 Aug 2022 20:36:17 GMT  
		Size: 1.2 MB (1241523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f78bf4cf172bedc6ad3c92b859859b10c0394104262328d5664ddc0b1488b29`  
		Last Modified: Thu, 04 Aug 2022 20:36:17 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6a26d2d4c34166613098e1380842f1355b534e2335a1dea2128c193b7f19bec`  
		Last Modified: Thu, 04 Aug 2022 20:36:16 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:1.6.16`

```console
$ docker pull memcached@sha256:0afaa8e890393e089efc991b62ec98d3dd53e5da995abfa548e5df9c70722015
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

### `memcached:1.6.16` - linux; amd64

```console
$ docker pull memcached@sha256:d6479777ae4663bb6752d9e779a2180adeae2e6f91da834a6c042665ef961b19
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.0 MB (32956000 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:36a225838cd6927616fc3c9afc4fc26e1fbe4097250b113b6b8508e02ae6a589`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 02 Aug 2022 01:20:04 GMT
ADD file:0eae0dca665c7044bf242cb1fc92cb8ea744f5af2dd376a558c90bc47349aefe in / 
# Tue, 02 Aug 2022 01:20:05 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 04:45:12 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 02 Aug 2022 04:45:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 04 Aug 2022 19:59:25 GMT
ENV MEMCACHED_VERSION=1.6.16
# Thu, 04 Aug 2022 19:59:25 GMT
ENV MEMCACHED_SHA1=724f31c3462fb6b07264d72d0043fd65545fd84a
# Thu, 04 Aug 2022 20:02:08 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 04 Aug 2022 20:02:08 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 04 Aug 2022 20:02:08 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 04 Aug 2022 20:02:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 04 Aug 2022 20:02:09 GMT
USER memcache
# Thu, 04 Aug 2022 20:02:09 GMT
EXPOSE 11211
# Thu, 04 Aug 2022 20:02:09 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:1efc276f4ff952c055dea726cfc96ec6a4fdb8b62d9eed816bd2b788f2860ad7`  
		Last Modified: Tue, 02 Aug 2022 01:24:13 GMT  
		Size: 31.4 MB (31366757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60bd6790acf68c1ccc4757e879b51b4dbc273681e1f30606a2ccd4b55623d288`  
		Last Modified: Tue, 02 Aug 2022 04:48:24 GMT  
		Size: 5.0 KB (4980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e72821989d416909e21411733d7d034cfa908016dceb0b6e2717a5fb9faa617`  
		Last Modified: Tue, 02 Aug 2022 04:48:24 GMT  
		Size: 328.1 KB (328097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a972a764145eff4153208b9f8bed20e2179ececcec6e6d462d74400d526ccb4c`  
		Last Modified: Thu, 04 Aug 2022 20:05:45 GMT  
		Size: 1.3 MB (1255762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc9c8a212883923ae20b3e2d671f8dcc32307603465cf915c7e83bd5ac522c69`  
		Last Modified: Thu, 04 Aug 2022 20:05:45 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:157eedd0af5feece73dbebf45897c44894a10678feca71d5d57ac4904492badc`  
		Last Modified: Thu, 04 Aug 2022 20:05:46 GMT  
		Size: 118.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.16` - linux; arm variant v5

```console
$ docker pull memcached@sha256:39515e68cebee2b2b88891c2b46b1c517587063301f77bbf7c312f6f9b372d65
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.5 MB (30454297 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8bf4bc30f264f1f9a0ede671e3a081ea54d1b6c3127ad5d9d4df3de21a985f5a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 02 Aug 2022 00:49:10 GMT
ADD file:4cd2f95737fd3007912428eeac56036c9e67e989e66cec08a8be99da47f88494 in / 
# Tue, 02 Aug 2022 00:49:10 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 01:58:42 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 02 Aug 2022 01:58:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 04 Aug 2022 19:50:51 GMT
ENV MEMCACHED_VERSION=1.6.16
# Thu, 04 Aug 2022 19:50:51 GMT
ENV MEMCACHED_SHA1=724f31c3462fb6b07264d72d0043fd65545fd84a
# Thu, 04 Aug 2022 19:56:43 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 04 Aug 2022 19:56:44 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 04 Aug 2022 19:56:44 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 04 Aug 2022 19:56:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 04 Aug 2022 19:56:44 GMT
USER memcache
# Thu, 04 Aug 2022 19:56:44 GMT
EXPOSE 11211
# Thu, 04 Aug 2022 19:56:45 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:5890b0ca6af5e8467a488e68716691950496a8f247d0495c2d595ddcb1893aff`  
		Last Modified: Tue, 02 Aug 2022 00:56:06 GMT  
		Size: 28.9 MB (28905515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e34350eb48491f2ab07c0f07724d37412df97ee9093c7c2458c9917afe37a42d`  
		Last Modified: Tue, 02 Aug 2022 02:04:59 GMT  
		Size: 4.9 KB (4894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36ecb6d2f4e3224a48197a5aa9d40970083bf4a92f41fbb493ac5adf9441a4ad`  
		Last Modified: Tue, 02 Aug 2022 02:04:59 GMT  
		Size: 316.6 KB (316628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e691cd60b95cdbb7fe7d3d74b1af54a56f440ac30d1dee94df4c4c370610b68d`  
		Last Modified: Thu, 04 Aug 2022 19:57:24 GMT  
		Size: 1.2 MB (1226852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8da76a828532ea569bd0e56b5a07a5e8bff4fe6efe22a5940260a261d113dc05`  
		Last Modified: Thu, 04 Aug 2022 19:57:23 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1705baeac52cb73666f9792b18547ce08509addd9ff3f19f6b91d21d5d10c8aa`  
		Last Modified: Thu, 04 Aug 2022 19:57:23 GMT  
		Size: 120.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.16` - linux; arm variant v7

```console
$ docker pull memcached@sha256:25e768546f1e321b2a9031611f8ecd4081990c82f8774f7e051a5480cf18445d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.1 MB (28076294 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5959e4e12e1b75611311d3866bc95f9fe30048418f972e70fa2c671a66149fdd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 02 Aug 2022 00:58:59 GMT
ADD file:1575b776a15adacebc0875642e97a80807d42dcfc8917e1406d47af7ac244c97 in / 
# Tue, 02 Aug 2022 00:58:59 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 06:28:56 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 02 Aug 2022 06:29:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 04 Aug 2022 21:30:08 GMT
ENV MEMCACHED_VERSION=1.6.16
# Thu, 04 Aug 2022 21:30:08 GMT
ENV MEMCACHED_SHA1=724f31c3462fb6b07264d72d0043fd65545fd84a
# Thu, 04 Aug 2022 21:36:35 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 04 Aug 2022 21:36:35 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 04 Aug 2022 21:36:36 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 04 Aug 2022 21:36:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 04 Aug 2022 21:36:37 GMT
USER memcache
# Thu, 04 Aug 2022 21:36:37 GMT
EXPOSE 11211
# Thu, 04 Aug 2022 21:36:37 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:1dd75a3a9c893a7dc313f683dd62464b7eab6c6d522ee62c8a17022631830f32`  
		Last Modified: Tue, 02 Aug 2022 01:06:45 GMT  
		Size: 26.6 MB (26560586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44a675a8ce135f198539dc76b078733393238f7c7b899c8635980eed8f35f1cc`  
		Last Modified: Tue, 02 Aug 2022 09:35:13 GMT  
		Size: 4.9 KB (4890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:497b0afd04c92a1e5d41f58dbc0d5d544b8880d000c0ffbd03adb48c32c0116b`  
		Last Modified: Tue, 02 Aug 2022 09:35:13 GMT  
		Size: 312.1 KB (312067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8874fe992be272d0e0780725714c2439507699c15bfad1a073df948a34eb668d`  
		Last Modified: Fri, 05 Aug 2022 00:37:30 GMT  
		Size: 1.2 MB (1198344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cd5e042b98c640c152a56816e122c5e7b0abe91535d5d891dceed9748e42129`  
		Last Modified: Fri, 05 Aug 2022 00:37:29 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e871a0f93bdc7cb723e47f45514f914186b73d1890a53cdfe8525dd034926d59`  
		Last Modified: Fri, 05 Aug 2022 00:37:29 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.16` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:759082b00d406f92781542ce86756eb73c5efe20acc7df6c25ac86be320a3ef5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.4 MB (31433439 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e91fe6663d9d90deed07c1d003a80fa6698137267c83310828f24a7ef63f6ef`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 02 Aug 2022 00:40:38 GMT
ADD file:6039adfbca55ed34a719c37672c664e3524130a0e2a3b8663629b8120b81b790 in / 
# Tue, 02 Aug 2022 00:40:39 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 03:56:15 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 02 Aug 2022 03:56:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 04 Aug 2022 20:33:46 GMT
ENV MEMCACHED_VERSION=1.6.16
# Thu, 04 Aug 2022 20:33:47 GMT
ENV MEMCACHED_SHA1=724f31c3462fb6b07264d72d0043fd65545fd84a
# Thu, 04 Aug 2022 20:36:17 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 04 Aug 2022 20:36:19 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 04 Aug 2022 20:36:19 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 04 Aug 2022 20:36:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 04 Aug 2022 20:36:21 GMT
USER memcache
# Thu, 04 Aug 2022 20:36:22 GMT
EXPOSE 11211
# Thu, 04 Aug 2022 20:36:23 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:a9fe95647e78b5516c7e2327355b6996e2ea295cd76ae242cbfe87f016b4e760`  
		Last Modified: Tue, 02 Aug 2022 00:46:05 GMT  
		Size: 30.1 MB (30054304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b983df009e7dc88033f53f015c09c56fd4db032d1abcade3333d8d4b515ff4af`  
		Last Modified: Tue, 02 Aug 2022 03:59:48 GMT  
		Size: 4.9 KB (4902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60720019405b50af041f391ec7dad90893ee95fc63fd6b3fb9da04850936f5db`  
		Last Modified: Tue, 02 Aug 2022 03:59:48 GMT  
		Size: 119.2 KB (119225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70569bedb4ee539337d6d3fd88e4076a1464b3a77bcfcca6604e18b815dbc402`  
		Last Modified: Thu, 04 Aug 2022 20:40:00 GMT  
		Size: 1.3 MB (1254600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:565112c01ad7b82688180f4fe70f5433126d79cc4b74e3d7f308601e2d34d9fe`  
		Last Modified: Thu, 04 Aug 2022 20:39:59 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce11290eb88924797c1fa048bd052c1243e4cb47e3469b26f3f1a3bc26472d19`  
		Last Modified: Thu, 04 Aug 2022 20:39:59 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.16` - linux; 386

```console
$ docker pull memcached@sha256:deec44ba81c574f36b5b53185684413e4e97c3374d256e762ccf0e50fa1ff0f0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.8 MB (33762417 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9640d046f98daa1268a24f35ea7de08f83c728d88f2483d734101b09bad34768`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 02 Aug 2022 00:39:20 GMT
ADD file:f771e2286465694126158821089d801c7296376be2a56189e6041a15d2fe79f5 in / 
# Tue, 02 Aug 2022 00:39:21 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 03:12:03 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 02 Aug 2022 03:12:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 04 Aug 2022 20:28:41 GMT
ENV MEMCACHED_VERSION=1.6.16
# Thu, 04 Aug 2022 20:28:42 GMT
ENV MEMCACHED_SHA1=724f31c3462fb6b07264d72d0043fd65545fd84a
# Thu, 04 Aug 2022 20:31:30 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 04 Aug 2022 20:31:32 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 04 Aug 2022 20:31:32 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 04 Aug 2022 20:31:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 04 Aug 2022 20:31:34 GMT
USER memcache
# Thu, 04 Aug 2022 20:31:35 GMT
EXPOSE 11211
# Thu, 04 Aug 2022 20:31:36 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:90eb7f0ce9f33cf5dcd67d54c2fa606186dbaa5f95b6046f36145097267f9e53`  
		Last Modified: Tue, 02 Aug 2022 00:45:14 GMT  
		Size: 32.4 MB (32374054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:107cdc14debc414f1e6554b58402d2be697942f8f22b45d5c9b6bff8be3f332a`  
		Last Modified: Tue, 02 Aug 2022 03:15:55 GMT  
		Size: 4.8 KB (4771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b33bafb66f7f078457cf82ba6cfcbab5feae0e38bc0d959a5b50fa98fbcbf4ac`  
		Last Modified: Tue, 02 Aug 2022 03:15:55 GMT  
		Size: 130.1 KB (130114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c122afb77220a37620d69b968b43d326ed98ef7d9ed80ea06c3a7fa1c54dc73f`  
		Last Modified: Thu, 04 Aug 2022 20:35:38 GMT  
		Size: 1.3 MB (1253069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2426ab0684229e93e257d5c6357fbad018ee92d3cdcf5a7812171aa06bf82ca9`  
		Last Modified: Thu, 04 Aug 2022 20:35:38 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:240ed953e9e062d3ea6893fe34ecd1e5e060a240ae2a66092c6970c0be0eeed5`  
		Last Modified: Thu, 04 Aug 2022 20:35:38 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.16` - linux; mips64le

```console
$ docker pull memcached@sha256:0d6798ccd4a9ac44c6ca7c358b2de6bdedbfe104de7d9987eedc68864ab8acc0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.0 MB (31002934 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aca3e1ecca25fb97ad1d376d73b212cad11874d1f051c4c4bac1b2d27abc15fd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 02 Aug 2022 01:10:34 GMT
ADD file:6dc22a1e5b5fcf23f2549406ddcc45c4e244f46e21eafa881de81fa87438e5d8 in / 
# Tue, 02 Aug 2022 01:10:38 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 03:22:53 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 02 Aug 2022 03:23:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 04 Aug 2022 20:07:25 GMT
ENV MEMCACHED_VERSION=1.6.16
# Thu, 04 Aug 2022 20:07:28 GMT
ENV MEMCACHED_SHA1=724f31c3462fb6b07264d72d0043fd65545fd84a
# Thu, 04 Aug 2022 20:14:28 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 04 Aug 2022 20:14:30 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 04 Aug 2022 20:14:35 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 04 Aug 2022 20:14:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 04 Aug 2022 20:14:40 GMT
USER memcache
# Thu, 04 Aug 2022 20:14:42 GMT
EXPOSE 11211
# Thu, 04 Aug 2022 20:14:45 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:88350749a27614c791450c256b051f023d81cdd256211274b1efac493779d2be`  
		Last Modified: Tue, 02 Aug 2022 01:21:02 GMT  
		Size: 29.6 MB (29628964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:117af7bbaadea9c81bbaa3a8a77b1ab5cd05bcac856c462cda2e81c9a40596ab`  
		Last Modified: Tue, 02 Aug 2022 03:30:45 GMT  
		Size: 4.9 KB (4863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53a16d313748bd6b2dade87de73d79edd8a08e4cb662769a717f8587abc8d5e0`  
		Last Modified: Tue, 02 Aug 2022 03:30:46 GMT  
		Size: 117.1 KB (117127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d524786af3243ee367d118f6d5260cffa06d800f492f9b4bb36c910958186933`  
		Last Modified: Thu, 04 Aug 2022 20:15:05 GMT  
		Size: 1.3 MB (1251571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4badb1f1970762d08dbd43d7e101081a5fabd3c45e18afd70636397e83102d2f`  
		Last Modified: Thu, 04 Aug 2022 20:15:04 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3102636392803c3bbff48f39e7f143e3bf9a0528365d63b90dc31cd32060d3e0`  
		Last Modified: Thu, 04 Aug 2022 20:15:04 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.16` - linux; ppc64le

```console
$ docker pull memcached@sha256:fef67c5248379f0c7154c6298ae0236afa239c6a2e7677ff26cf67e2e902873c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.0 MB (36957550 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19ebbfa2abfbf5d8014f1a3d04cab132b47836a64e68160efb3b8c752addaedd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 02 Aug 2022 01:17:30 GMT
ADD file:3a95a896d463569ce82199957052b3467123a4bd3385a0a4e397cf08402a99c3 in / 
# Tue, 02 Aug 2022 01:17:32 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 03:45:30 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 02 Aug 2022 03:45:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 04 Aug 2022 20:31:03 GMT
ENV MEMCACHED_VERSION=1.6.16
# Thu, 04 Aug 2022 20:31:04 GMT
ENV MEMCACHED_SHA1=724f31c3462fb6b07264d72d0043fd65545fd84a
# Thu, 04 Aug 2022 20:34:08 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 04 Aug 2022 20:34:09 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 04 Aug 2022 20:34:10 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 04 Aug 2022 20:34:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 04 Aug 2022 20:34:10 GMT
USER memcache
# Thu, 04 Aug 2022 20:34:11 GMT
EXPOSE 11211
# Thu, 04 Aug 2022 20:34:11 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:5241cd116d6e6e2d62f3d8c2245b74daca9f6cc154eaccd738feb41984c74714`  
		Last Modified: Tue, 02 Aug 2022 01:24:39 GMT  
		Size: 35.3 MB (35272771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58860b5324185f5059438d063f2a2b9c8ec05e058d0c1467db47a258a089c691`  
		Last Modified: Tue, 02 Aug 2022 03:53:12 GMT  
		Size: 5.0 KB (4978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82fb13381eff7e0b9526ba592f13e09cea5295914fde283ea341e5b71cb31493`  
		Last Modified: Tue, 02 Aug 2022 03:53:13 GMT  
		Size: 356.9 KB (356918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b33f6ac4fcd819056777e9462124dfc34dca6f35e1cae56a64d12bd150e4dfc9`  
		Last Modified: Thu, 04 Aug 2022 20:38:29 GMT  
		Size: 1.3 MB (1322475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:893b74576495c7a62c5d4447a7453f60f228fbb0e6d2dc4edf7e67661c455f57`  
		Last Modified: Thu, 04 Aug 2022 20:38:28 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7855d0c39dc9730d8ec3369fa86f770bd433a903eb346e9115b7442574441f24`  
		Last Modified: Thu, 04 Aug 2022 20:38:28 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.16` - linux; s390x

```console
$ docker pull memcached@sha256:4f7e9706bfd16d98bfb48a6435c8359a167ab733777f16f24996cad3f431bdc5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.2 MB (31211398 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6739ca31062c74398fdfec102afbacead1c25fa0decf2fa14bdecdcb6b160543`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 02 Aug 2022 00:42:27 GMT
ADD file:c2afc8990930846fbe7c99bfdfe9ea562c75feb6e3c9122431f7c9f8b5e51a7f in / 
# Tue, 02 Aug 2022 00:42:29 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 02:37:02 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 02 Aug 2022 02:37:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 04 Aug 2022 20:28:18 GMT
ENV MEMCACHED_VERSION=1.6.16
# Thu, 04 Aug 2022 20:28:18 GMT
ENV MEMCACHED_SHA1=724f31c3462fb6b07264d72d0043fd65545fd84a
# Thu, 04 Aug 2022 20:31:37 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 04 Aug 2022 20:31:37 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 04 Aug 2022 20:31:37 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 04 Aug 2022 20:31:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 04 Aug 2022 20:31:38 GMT
USER memcache
# Thu, 04 Aug 2022 20:31:38 GMT
EXPOSE 11211
# Thu, 04 Aug 2022 20:31:38 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:026d311d0716db60eba0572ea784c21031f420960510cebcc383dc53949b4db8`  
		Last Modified: Tue, 02 Aug 2022 00:48:01 GMT  
		Size: 29.6 MB (29640259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0ffdb328e548bd6b6311c78665ac8cd3be8f0b2e09691701d9b0bae0924f8f5`  
		Last Modified: Tue, 02 Aug 2022 02:41:16 GMT  
		Size: 5.0 KB (5025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fbb9677007b0ebab2fe6feab520da1962d3fcffb3490aa844681a46fcb35749`  
		Last Modified: Tue, 02 Aug 2022 02:41:16 GMT  
		Size: 324.2 KB (324183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9c93abfa1f832f2e1f02fbe7b9a489735142c2051dafa7af20d985ff2e2106b`  
		Last Modified: Thu, 04 Aug 2022 20:36:17 GMT  
		Size: 1.2 MB (1241523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f78bf4cf172bedc6ad3c92b859859b10c0394104262328d5664ddc0b1488b29`  
		Last Modified: Thu, 04 Aug 2022 20:36:17 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6a26d2d4c34166613098e1380842f1355b534e2335a1dea2128c193b7f19bec`  
		Last Modified: Thu, 04 Aug 2022 20:36:16 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:1.6.16-alpine`

```console
$ docker pull memcached@sha256:6f612899171e3ec7380f48ca3bc4043482423db2462846c9a55124b44e3dee5d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `memcached:1.6.16-alpine` - linux; amd64

```console
$ docker pull memcached@sha256:9b2ecb3fb8713d7c971eaf6e97150fcf34735d105bab81dd53e45d18da6c6b90
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3860216 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:22e40b7fd940b01ddffc7c8fddff80d89c6572d89d7c9664343a2c1e3efe389b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 18 Jul 2022 21:00:15 GMT
ADD file:a2648378045615c3785c752423b1afc8dc1c2b213393344f4d0ca17e7255c1cb in / 
# Mon, 18 Jul 2022 21:00:15 GMT
CMD ["/bin/sh"]
# Tue, 19 Jul 2022 01:33:13 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 19 Jul 2022 01:33:14 GMT
RUN apk add --no-cache libsasl
# Thu, 04 Aug 2022 20:02:18 GMT
ENV MEMCACHED_VERSION=1.6.16
# Thu, 04 Aug 2022 20:02:18 GMT
ENV MEMCACHED_SHA1=724f31c3462fb6b07264d72d0043fd65545fd84a
# Thu, 04 Aug 2022 20:05:09 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Thu, 04 Aug 2022 20:05:09 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 04 Aug 2022 20:05:09 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 04 Aug 2022 20:05:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 04 Aug 2022 20:05:10 GMT
USER memcache
# Thu, 04 Aug 2022 20:05:10 GMT
EXPOSE 11211
# Thu, 04 Aug 2022 20:05:10 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:530afca65e2ea04227630ae746e0c85b2bd1a179379cbf2b6501b49c4cab2ccc`  
		Last Modified: Mon, 18 Jul 2022 19:09:35 GMT  
		Size: 2.8 MB (2798806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3e13ff258fbd16cc42fcdb1bd800f73f4b380857d2a6096906444ec790c6542`  
		Last Modified: Tue, 19 Jul 2022 01:36:41 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90922b6720c8f20007711c5660b8269518b50979be1cef2cb4c0b12a7ac78ff7`  
		Last Modified: Tue, 19 Jul 2022 01:36:41 GMT  
		Size: 108.3 KB (108315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51aa27d6f4905ed1e531c58fa8d22676bfac86a2ba49c01894f95245d65329f7`  
		Last Modified: Thu, 04 Aug 2022 20:06:10 GMT  
		Size: 951.4 KB (951422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35e3d85200a71563435aa4bb45d98232f964b19c4facc2bc63d6ae3db816cbb4`  
		Last Modified: Thu, 04 Aug 2022 20:06:10 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74ba9b8d8a47b35ef57b45387b27d98410a32a2814a83a6cc686136b48fbb420`  
		Last Modified: Thu, 04 Aug 2022 20:06:10 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.16-alpine` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:ad6951d968e4efe51c8da00a45147c17103c337177ececea11271806da36563d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.7 MB (3744755 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c64051372a720608fa1f9fed496d62daf26dd098c6ecf5189d59c3c4aede3d8f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 18 Jul 2022 21:57:05 GMT
ADD file:9ccb70abba88b6de789b29f17770246f765ffbb072fe598580bfc29ce3213f1c in / 
# Mon, 18 Jul 2022 21:57:05 GMT
CMD ["/bin/sh"]
# Mon, 18 Jul 2022 23:40:46 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Mon, 18 Jul 2022 23:40:48 GMT
RUN apk add --no-cache libsasl
# Thu, 04 Aug 2022 20:36:31 GMT
ENV MEMCACHED_VERSION=1.6.16
# Thu, 04 Aug 2022 20:36:32 GMT
ENV MEMCACHED_SHA1=724f31c3462fb6b07264d72d0043fd65545fd84a
# Thu, 04 Aug 2022 20:39:14 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Thu, 04 Aug 2022 20:39:16 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 04 Aug 2022 20:39:16 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 04 Aug 2022 20:39:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 04 Aug 2022 20:39:18 GMT
USER memcache
# Thu, 04 Aug 2022 20:39:19 GMT
EXPOSE 11211
# Thu, 04 Aug 2022 20:39:20 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:f97344484467e4c4ebb85aae724170073799295a3442c50ab532e249bd27b412`  
		Last Modified: Mon, 18 Jul 2022 19:08:29 GMT  
		Size: 2.7 MB (2694720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7da60570c25aa47c5a2b9fcd4be47a0a93240f9f4f2ab5a4d0b52c2646f40a28`  
		Last Modified: Mon, 18 Jul 2022 23:44:19 GMT  
		Size: 1.2 KB (1240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66a722c1c0875bed8b5bc87f4e2844ed10d7d9c12755721cd2164aa8b1c690d3`  
		Last Modified: Mon, 18 Jul 2022 23:44:20 GMT  
		Size: 109.6 KB (109554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19d417474c6b68c4c39d74d0adc463d1b8efd38f3c8f97b0a06230a45762e419`  
		Last Modified: Thu, 04 Aug 2022 20:40:30 GMT  
		Size: 938.8 KB (938833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9ffa798617a9bfdd85f3d0e02e2e00587f4a41d08fdf2f2cb2e1545b83c9090`  
		Last Modified: Thu, 04 Aug 2022 20:40:30 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:953ea2e6fdf83d907c05809ff46325d9d363d4cea34f88de5c84c87be30aa90d`  
		Last Modified: Thu, 04 Aug 2022 20:40:30 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.16-alpine` - linux; 386

```console
$ docker pull memcached@sha256:ee1fc765b96e3511c6b013639aec361b29013747c099430e8d347cf3692fac6e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3886569 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d6788e9d28dbe037c2a56c89130413dd2dcf2e394c99b8cfe32d79eecdaa1783`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 18 Jul 2022 20:38:19 GMT
ADD file:be69b7550bf861d8fb12bdbe1edf3a0d2519a6a4da61bd04858b6258ffbf48a7 in / 
# Mon, 18 Jul 2022 20:38:19 GMT
CMD ["/bin/sh"]
# Tue, 19 Jul 2022 01:27:41 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 19 Jul 2022 01:27:42 GMT
RUN apk add --no-cache libsasl
# Thu, 04 Aug 2022 20:31:52 GMT
ENV MEMCACHED_VERSION=1.6.16
# Thu, 04 Aug 2022 20:31:53 GMT
ENV MEMCACHED_SHA1=724f31c3462fb6b07264d72d0043fd65545fd84a
# Thu, 04 Aug 2022 20:34:46 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Thu, 04 Aug 2022 20:34:48 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 04 Aug 2022 20:34:48 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 04 Aug 2022 20:34:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 04 Aug 2022 20:34:50 GMT
USER memcache
# Thu, 04 Aug 2022 20:34:51 GMT
EXPOSE 11211
# Thu, 04 Aug 2022 20:34:52 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:5d7f927419794ebb7496ac38b0659686317b2d2fac7252a4a0d40d43d5fdd662`  
		Last Modified: Mon, 18 Jul 2022 19:09:22 GMT  
		Size: 2.8 MB (2802334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bd21aea877c073ddb40c30afa2f3e8f58c6fef7737835158747cf175df4ef4e`  
		Last Modified: Tue, 19 Jul 2022 01:31:30 GMT  
		Size: 1.2 KB (1241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fba37b4bd3e4b8bdb4184c8f065ce7b15f3fadd48bbb46f43623a90737e59911`  
		Last Modified: Tue, 19 Jul 2022 01:31:31 GMT  
		Size: 119.8 KB (119833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bf6c5b49cad3fa44a9ca5f146e497c4fb38ee5f14d27a2164224225a90e55aa`  
		Last Modified: Thu, 04 Aug 2022 20:36:09 GMT  
		Size: 962.8 KB (962757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cff8368515defad6347e63b43774e1ab0921279b4081ee4d8d36d28079e6c5d`  
		Last Modified: Thu, 04 Aug 2022 20:36:09 GMT  
		Size: 283.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e402b0471e504b912c3be68ebc0b6934213ca421d3b90ab8eb15f698c24157a`  
		Last Modified: Thu, 04 Aug 2022 20:36:09 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.16-alpine` - linux; ppc64le

```console
$ docker pull memcached@sha256:b9d56b200da6dd58c0da595669a18edfb7c77db42a4305b20a9a72c43b1bb034
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3898842 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4292cb4f0bd2997ab218f436690f4d170d349cead12c74fbc6c9acc4489ee307`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 18 Jul 2022 21:29:30 GMT
ADD file:69e4080f15f54e2d8f8aa25fdcba9c01dde149d43592edd5023106675e54a769 in / 
# Mon, 18 Jul 2022 21:29:31 GMT
CMD ["/bin/sh"]
# Tue, 02 Aug 2022 03:48:55 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 02 Aug 2022 03:48:57 GMT
RUN apk add --no-cache libsasl
# Thu, 04 Aug 2022 20:34:28 GMT
ENV MEMCACHED_VERSION=1.6.16
# Thu, 04 Aug 2022 20:34:29 GMT
ENV MEMCACHED_SHA1=724f31c3462fb6b07264d72d0043fd65545fd84a
# Thu, 04 Aug 2022 20:37:42 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Thu, 04 Aug 2022 20:37:42 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 04 Aug 2022 20:37:43 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 04 Aug 2022 20:37:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 04 Aug 2022 20:37:44 GMT
USER memcache
# Thu, 04 Aug 2022 20:37:44 GMT
EXPOSE 11211
# Thu, 04 Aug 2022 20:37:44 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:602896d442490cd3fbb6599f0f862d3673b7cd58eca3ac842b8e09bf8d012443`  
		Last Modified: Mon, 18 Jul 2022 19:09:09 GMT  
		Size: 2.8 MB (2789923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e6cec9872fd3c66c2b19cff2dd853136a16b03e523f70d0cd8875dff75abdf6`  
		Last Modified: Tue, 02 Aug 2022 03:53:48 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2420696d84e23c3f6e09fb61166d22a8b83d011559aa421d5d5e9f4ccf2f06a`  
		Last Modified: Tue, 02 Aug 2022 03:53:48 GMT  
		Size: 126.1 KB (126059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c706cce31e40f8bd79f2caa6ecef5e085849307288d79ebffc91b574118f04ba`  
		Last Modified: Thu, 04 Aug 2022 20:39:03 GMT  
		Size: 981.2 KB (981184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e86b61d9d1ecc2880ffc457445a2f5dcfaa3317fa84796de7bb78f30b5c31e15`  
		Last Modified: Thu, 04 Aug 2022 20:39:03 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74db60069b975f4fa4efaf1fe6ee2af6977e661683c83a54c141faff25255f11`  
		Last Modified: Thu, 04 Aug 2022 20:39:03 GMT  
		Size: 120.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.16-alpine` - linux; s390x

```console
$ docker pull memcached@sha256:62da518bff73ec0e140de7ecadbc4c0bbeaec3886cf144ac9deea64a95905fa7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.6 MB (3636817 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:057cc21d3a6bf40d3f50d6b8ce6d9004c65a7fb5a448f98761e044c79691adf5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 18 Jul 2022 20:41:35 GMT
ADD file:deaa573cd61e07709846a5300fb627a8610e9754129c085ed483ff8897d0c002 in / 
# Mon, 18 Jul 2022 20:41:36 GMT
CMD ["/bin/sh"]
# Mon, 18 Jul 2022 22:46:43 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Mon, 18 Jul 2022 22:46:46 GMT
RUN apk add --no-cache libsasl
# Thu, 04 Aug 2022 20:31:55 GMT
ENV MEMCACHED_VERSION=1.6.16
# Thu, 04 Aug 2022 20:31:55 GMT
ENV MEMCACHED_SHA1=724f31c3462fb6b07264d72d0043fd65545fd84a
# Thu, 04 Aug 2022 20:35:27 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Thu, 04 Aug 2022 20:35:27 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 04 Aug 2022 20:35:27 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 04 Aug 2022 20:35:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 04 Aug 2022 20:35:28 GMT
USER memcache
# Thu, 04 Aug 2022 20:35:28 GMT
EXPOSE 11211
# Thu, 04 Aug 2022 20:35:28 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:5f1840d5bacf4162a87f497e22d94bce946e660bdfce8eeefcbf7bd0beb193f3`  
		Last Modified: Mon, 18 Jul 2022 20:42:36 GMT  
		Size: 2.6 MB (2580798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2b6f46f9ccd4c19bfc103544d0d83ceef7feae4d70d25397d620ca381065659`  
		Last Modified: Mon, 18 Jul 2022 22:52:40 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f491a581763941ae0ec0ec035bdfb8073504d7fdc2eec6eb1e70878f26c16351`  
		Last Modified: Mon, 18 Jul 2022 22:52:40 GMT  
		Size: 112.5 KB (112503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:978f61b805ce2eb5610c877e3b8dc826f82016a7cf4af02737c7e2c44a1ede3f`  
		Last Modified: Thu, 04 Aug 2022 20:36:36 GMT  
		Size: 941.8 KB (941845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0a55bbbae5442cc2430fd5859fdd4c002e763bfe72f074645ea038f97652422`  
		Last Modified: Thu, 04 Aug 2022 20:36:36 GMT  
		Size: 283.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16ad3c74a3fe0b757743e632dbef104cea78e39b57e4155dab2020488d5b4546`  
		Last Modified: Thu, 04 Aug 2022 20:36:36 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:1.6.16-alpine3.16`

```console
$ docker pull memcached@sha256:6f612899171e3ec7380f48ca3bc4043482423db2462846c9a55124b44e3dee5d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `memcached:1.6.16-alpine3.16` - linux; amd64

```console
$ docker pull memcached@sha256:9b2ecb3fb8713d7c971eaf6e97150fcf34735d105bab81dd53e45d18da6c6b90
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3860216 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:22e40b7fd940b01ddffc7c8fddff80d89c6572d89d7c9664343a2c1e3efe389b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 18 Jul 2022 21:00:15 GMT
ADD file:a2648378045615c3785c752423b1afc8dc1c2b213393344f4d0ca17e7255c1cb in / 
# Mon, 18 Jul 2022 21:00:15 GMT
CMD ["/bin/sh"]
# Tue, 19 Jul 2022 01:33:13 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 19 Jul 2022 01:33:14 GMT
RUN apk add --no-cache libsasl
# Thu, 04 Aug 2022 20:02:18 GMT
ENV MEMCACHED_VERSION=1.6.16
# Thu, 04 Aug 2022 20:02:18 GMT
ENV MEMCACHED_SHA1=724f31c3462fb6b07264d72d0043fd65545fd84a
# Thu, 04 Aug 2022 20:05:09 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Thu, 04 Aug 2022 20:05:09 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 04 Aug 2022 20:05:09 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 04 Aug 2022 20:05:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 04 Aug 2022 20:05:10 GMT
USER memcache
# Thu, 04 Aug 2022 20:05:10 GMT
EXPOSE 11211
# Thu, 04 Aug 2022 20:05:10 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:530afca65e2ea04227630ae746e0c85b2bd1a179379cbf2b6501b49c4cab2ccc`  
		Last Modified: Mon, 18 Jul 2022 19:09:35 GMT  
		Size: 2.8 MB (2798806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3e13ff258fbd16cc42fcdb1bd800f73f4b380857d2a6096906444ec790c6542`  
		Last Modified: Tue, 19 Jul 2022 01:36:41 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90922b6720c8f20007711c5660b8269518b50979be1cef2cb4c0b12a7ac78ff7`  
		Last Modified: Tue, 19 Jul 2022 01:36:41 GMT  
		Size: 108.3 KB (108315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51aa27d6f4905ed1e531c58fa8d22676bfac86a2ba49c01894f95245d65329f7`  
		Last Modified: Thu, 04 Aug 2022 20:06:10 GMT  
		Size: 951.4 KB (951422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35e3d85200a71563435aa4bb45d98232f964b19c4facc2bc63d6ae3db816cbb4`  
		Last Modified: Thu, 04 Aug 2022 20:06:10 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74ba9b8d8a47b35ef57b45387b27d98410a32a2814a83a6cc686136b48fbb420`  
		Last Modified: Thu, 04 Aug 2022 20:06:10 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.16-alpine3.16` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:ad6951d968e4efe51c8da00a45147c17103c337177ececea11271806da36563d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.7 MB (3744755 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c64051372a720608fa1f9fed496d62daf26dd098c6ecf5189d59c3c4aede3d8f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 18 Jul 2022 21:57:05 GMT
ADD file:9ccb70abba88b6de789b29f17770246f765ffbb072fe598580bfc29ce3213f1c in / 
# Mon, 18 Jul 2022 21:57:05 GMT
CMD ["/bin/sh"]
# Mon, 18 Jul 2022 23:40:46 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Mon, 18 Jul 2022 23:40:48 GMT
RUN apk add --no-cache libsasl
# Thu, 04 Aug 2022 20:36:31 GMT
ENV MEMCACHED_VERSION=1.6.16
# Thu, 04 Aug 2022 20:36:32 GMT
ENV MEMCACHED_SHA1=724f31c3462fb6b07264d72d0043fd65545fd84a
# Thu, 04 Aug 2022 20:39:14 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Thu, 04 Aug 2022 20:39:16 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 04 Aug 2022 20:39:16 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 04 Aug 2022 20:39:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 04 Aug 2022 20:39:18 GMT
USER memcache
# Thu, 04 Aug 2022 20:39:19 GMT
EXPOSE 11211
# Thu, 04 Aug 2022 20:39:20 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:f97344484467e4c4ebb85aae724170073799295a3442c50ab532e249bd27b412`  
		Last Modified: Mon, 18 Jul 2022 19:08:29 GMT  
		Size: 2.7 MB (2694720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7da60570c25aa47c5a2b9fcd4be47a0a93240f9f4f2ab5a4d0b52c2646f40a28`  
		Last Modified: Mon, 18 Jul 2022 23:44:19 GMT  
		Size: 1.2 KB (1240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66a722c1c0875bed8b5bc87f4e2844ed10d7d9c12755721cd2164aa8b1c690d3`  
		Last Modified: Mon, 18 Jul 2022 23:44:20 GMT  
		Size: 109.6 KB (109554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19d417474c6b68c4c39d74d0adc463d1b8efd38f3c8f97b0a06230a45762e419`  
		Last Modified: Thu, 04 Aug 2022 20:40:30 GMT  
		Size: 938.8 KB (938833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9ffa798617a9bfdd85f3d0e02e2e00587f4a41d08fdf2f2cb2e1545b83c9090`  
		Last Modified: Thu, 04 Aug 2022 20:40:30 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:953ea2e6fdf83d907c05809ff46325d9d363d4cea34f88de5c84c87be30aa90d`  
		Last Modified: Thu, 04 Aug 2022 20:40:30 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.16-alpine3.16` - linux; 386

```console
$ docker pull memcached@sha256:ee1fc765b96e3511c6b013639aec361b29013747c099430e8d347cf3692fac6e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3886569 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d6788e9d28dbe037c2a56c89130413dd2dcf2e394c99b8cfe32d79eecdaa1783`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 18 Jul 2022 20:38:19 GMT
ADD file:be69b7550bf861d8fb12bdbe1edf3a0d2519a6a4da61bd04858b6258ffbf48a7 in / 
# Mon, 18 Jul 2022 20:38:19 GMT
CMD ["/bin/sh"]
# Tue, 19 Jul 2022 01:27:41 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 19 Jul 2022 01:27:42 GMT
RUN apk add --no-cache libsasl
# Thu, 04 Aug 2022 20:31:52 GMT
ENV MEMCACHED_VERSION=1.6.16
# Thu, 04 Aug 2022 20:31:53 GMT
ENV MEMCACHED_SHA1=724f31c3462fb6b07264d72d0043fd65545fd84a
# Thu, 04 Aug 2022 20:34:46 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Thu, 04 Aug 2022 20:34:48 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 04 Aug 2022 20:34:48 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 04 Aug 2022 20:34:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 04 Aug 2022 20:34:50 GMT
USER memcache
# Thu, 04 Aug 2022 20:34:51 GMT
EXPOSE 11211
# Thu, 04 Aug 2022 20:34:52 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:5d7f927419794ebb7496ac38b0659686317b2d2fac7252a4a0d40d43d5fdd662`  
		Last Modified: Mon, 18 Jul 2022 19:09:22 GMT  
		Size: 2.8 MB (2802334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bd21aea877c073ddb40c30afa2f3e8f58c6fef7737835158747cf175df4ef4e`  
		Last Modified: Tue, 19 Jul 2022 01:31:30 GMT  
		Size: 1.2 KB (1241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fba37b4bd3e4b8bdb4184c8f065ce7b15f3fadd48bbb46f43623a90737e59911`  
		Last Modified: Tue, 19 Jul 2022 01:31:31 GMT  
		Size: 119.8 KB (119833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bf6c5b49cad3fa44a9ca5f146e497c4fb38ee5f14d27a2164224225a90e55aa`  
		Last Modified: Thu, 04 Aug 2022 20:36:09 GMT  
		Size: 962.8 KB (962757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cff8368515defad6347e63b43774e1ab0921279b4081ee4d8d36d28079e6c5d`  
		Last Modified: Thu, 04 Aug 2022 20:36:09 GMT  
		Size: 283.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e402b0471e504b912c3be68ebc0b6934213ca421d3b90ab8eb15f698c24157a`  
		Last Modified: Thu, 04 Aug 2022 20:36:09 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.16-alpine3.16` - linux; ppc64le

```console
$ docker pull memcached@sha256:b9d56b200da6dd58c0da595669a18edfb7c77db42a4305b20a9a72c43b1bb034
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3898842 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4292cb4f0bd2997ab218f436690f4d170d349cead12c74fbc6c9acc4489ee307`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 18 Jul 2022 21:29:30 GMT
ADD file:69e4080f15f54e2d8f8aa25fdcba9c01dde149d43592edd5023106675e54a769 in / 
# Mon, 18 Jul 2022 21:29:31 GMT
CMD ["/bin/sh"]
# Tue, 02 Aug 2022 03:48:55 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 02 Aug 2022 03:48:57 GMT
RUN apk add --no-cache libsasl
# Thu, 04 Aug 2022 20:34:28 GMT
ENV MEMCACHED_VERSION=1.6.16
# Thu, 04 Aug 2022 20:34:29 GMT
ENV MEMCACHED_SHA1=724f31c3462fb6b07264d72d0043fd65545fd84a
# Thu, 04 Aug 2022 20:37:42 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Thu, 04 Aug 2022 20:37:42 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 04 Aug 2022 20:37:43 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 04 Aug 2022 20:37:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 04 Aug 2022 20:37:44 GMT
USER memcache
# Thu, 04 Aug 2022 20:37:44 GMT
EXPOSE 11211
# Thu, 04 Aug 2022 20:37:44 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:602896d442490cd3fbb6599f0f862d3673b7cd58eca3ac842b8e09bf8d012443`  
		Last Modified: Mon, 18 Jul 2022 19:09:09 GMT  
		Size: 2.8 MB (2789923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e6cec9872fd3c66c2b19cff2dd853136a16b03e523f70d0cd8875dff75abdf6`  
		Last Modified: Tue, 02 Aug 2022 03:53:48 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2420696d84e23c3f6e09fb61166d22a8b83d011559aa421d5d5e9f4ccf2f06a`  
		Last Modified: Tue, 02 Aug 2022 03:53:48 GMT  
		Size: 126.1 KB (126059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c706cce31e40f8bd79f2caa6ecef5e085849307288d79ebffc91b574118f04ba`  
		Last Modified: Thu, 04 Aug 2022 20:39:03 GMT  
		Size: 981.2 KB (981184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e86b61d9d1ecc2880ffc457445a2f5dcfaa3317fa84796de7bb78f30b5c31e15`  
		Last Modified: Thu, 04 Aug 2022 20:39:03 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74db60069b975f4fa4efaf1fe6ee2af6977e661683c83a54c141faff25255f11`  
		Last Modified: Thu, 04 Aug 2022 20:39:03 GMT  
		Size: 120.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.16-alpine3.16` - linux; s390x

```console
$ docker pull memcached@sha256:62da518bff73ec0e140de7ecadbc4c0bbeaec3886cf144ac9deea64a95905fa7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.6 MB (3636817 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:057cc21d3a6bf40d3f50d6b8ce6d9004c65a7fb5a448f98761e044c79691adf5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 18 Jul 2022 20:41:35 GMT
ADD file:deaa573cd61e07709846a5300fb627a8610e9754129c085ed483ff8897d0c002 in / 
# Mon, 18 Jul 2022 20:41:36 GMT
CMD ["/bin/sh"]
# Mon, 18 Jul 2022 22:46:43 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Mon, 18 Jul 2022 22:46:46 GMT
RUN apk add --no-cache libsasl
# Thu, 04 Aug 2022 20:31:55 GMT
ENV MEMCACHED_VERSION=1.6.16
# Thu, 04 Aug 2022 20:31:55 GMT
ENV MEMCACHED_SHA1=724f31c3462fb6b07264d72d0043fd65545fd84a
# Thu, 04 Aug 2022 20:35:27 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Thu, 04 Aug 2022 20:35:27 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 04 Aug 2022 20:35:27 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 04 Aug 2022 20:35:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 04 Aug 2022 20:35:28 GMT
USER memcache
# Thu, 04 Aug 2022 20:35:28 GMT
EXPOSE 11211
# Thu, 04 Aug 2022 20:35:28 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:5f1840d5bacf4162a87f497e22d94bce946e660bdfce8eeefcbf7bd0beb193f3`  
		Last Modified: Mon, 18 Jul 2022 20:42:36 GMT  
		Size: 2.6 MB (2580798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2b6f46f9ccd4c19bfc103544d0d83ceef7feae4d70d25397d620ca381065659`  
		Last Modified: Mon, 18 Jul 2022 22:52:40 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f491a581763941ae0ec0ec035bdfb8073504d7fdc2eec6eb1e70878f26c16351`  
		Last Modified: Mon, 18 Jul 2022 22:52:40 GMT  
		Size: 112.5 KB (112503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:978f61b805ce2eb5610c877e3b8dc826f82016a7cf4af02737c7e2c44a1ede3f`  
		Last Modified: Thu, 04 Aug 2022 20:36:36 GMT  
		Size: 941.8 KB (941845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0a55bbbae5442cc2430fd5859fdd4c002e763bfe72f074645ea038f97652422`  
		Last Modified: Thu, 04 Aug 2022 20:36:36 GMT  
		Size: 283.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16ad3c74a3fe0b757743e632dbef104cea78e39b57e4155dab2020488d5b4546`  
		Last Modified: Thu, 04 Aug 2022 20:36:36 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:1.6.16-bullseye`

```console
$ docker pull memcached@sha256:0afaa8e890393e089efc991b62ec98d3dd53e5da995abfa548e5df9c70722015
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

### `memcached:1.6.16-bullseye` - linux; amd64

```console
$ docker pull memcached@sha256:d6479777ae4663bb6752d9e779a2180adeae2e6f91da834a6c042665ef961b19
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.0 MB (32956000 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:36a225838cd6927616fc3c9afc4fc26e1fbe4097250b113b6b8508e02ae6a589`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 02 Aug 2022 01:20:04 GMT
ADD file:0eae0dca665c7044bf242cb1fc92cb8ea744f5af2dd376a558c90bc47349aefe in / 
# Tue, 02 Aug 2022 01:20:05 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 04:45:12 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 02 Aug 2022 04:45:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 04 Aug 2022 19:59:25 GMT
ENV MEMCACHED_VERSION=1.6.16
# Thu, 04 Aug 2022 19:59:25 GMT
ENV MEMCACHED_SHA1=724f31c3462fb6b07264d72d0043fd65545fd84a
# Thu, 04 Aug 2022 20:02:08 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 04 Aug 2022 20:02:08 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 04 Aug 2022 20:02:08 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 04 Aug 2022 20:02:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 04 Aug 2022 20:02:09 GMT
USER memcache
# Thu, 04 Aug 2022 20:02:09 GMT
EXPOSE 11211
# Thu, 04 Aug 2022 20:02:09 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:1efc276f4ff952c055dea726cfc96ec6a4fdb8b62d9eed816bd2b788f2860ad7`  
		Last Modified: Tue, 02 Aug 2022 01:24:13 GMT  
		Size: 31.4 MB (31366757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60bd6790acf68c1ccc4757e879b51b4dbc273681e1f30606a2ccd4b55623d288`  
		Last Modified: Tue, 02 Aug 2022 04:48:24 GMT  
		Size: 5.0 KB (4980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e72821989d416909e21411733d7d034cfa908016dceb0b6e2717a5fb9faa617`  
		Last Modified: Tue, 02 Aug 2022 04:48:24 GMT  
		Size: 328.1 KB (328097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a972a764145eff4153208b9f8bed20e2179ececcec6e6d462d74400d526ccb4c`  
		Last Modified: Thu, 04 Aug 2022 20:05:45 GMT  
		Size: 1.3 MB (1255762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc9c8a212883923ae20b3e2d671f8dcc32307603465cf915c7e83bd5ac522c69`  
		Last Modified: Thu, 04 Aug 2022 20:05:45 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:157eedd0af5feece73dbebf45897c44894a10678feca71d5d57ac4904492badc`  
		Last Modified: Thu, 04 Aug 2022 20:05:46 GMT  
		Size: 118.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.16-bullseye` - linux; arm variant v5

```console
$ docker pull memcached@sha256:39515e68cebee2b2b88891c2b46b1c517587063301f77bbf7c312f6f9b372d65
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.5 MB (30454297 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8bf4bc30f264f1f9a0ede671e3a081ea54d1b6c3127ad5d9d4df3de21a985f5a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 02 Aug 2022 00:49:10 GMT
ADD file:4cd2f95737fd3007912428eeac56036c9e67e989e66cec08a8be99da47f88494 in / 
# Tue, 02 Aug 2022 00:49:10 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 01:58:42 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 02 Aug 2022 01:58:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 04 Aug 2022 19:50:51 GMT
ENV MEMCACHED_VERSION=1.6.16
# Thu, 04 Aug 2022 19:50:51 GMT
ENV MEMCACHED_SHA1=724f31c3462fb6b07264d72d0043fd65545fd84a
# Thu, 04 Aug 2022 19:56:43 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 04 Aug 2022 19:56:44 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 04 Aug 2022 19:56:44 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 04 Aug 2022 19:56:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 04 Aug 2022 19:56:44 GMT
USER memcache
# Thu, 04 Aug 2022 19:56:44 GMT
EXPOSE 11211
# Thu, 04 Aug 2022 19:56:45 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:5890b0ca6af5e8467a488e68716691950496a8f247d0495c2d595ddcb1893aff`  
		Last Modified: Tue, 02 Aug 2022 00:56:06 GMT  
		Size: 28.9 MB (28905515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e34350eb48491f2ab07c0f07724d37412df97ee9093c7c2458c9917afe37a42d`  
		Last Modified: Tue, 02 Aug 2022 02:04:59 GMT  
		Size: 4.9 KB (4894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36ecb6d2f4e3224a48197a5aa9d40970083bf4a92f41fbb493ac5adf9441a4ad`  
		Last Modified: Tue, 02 Aug 2022 02:04:59 GMT  
		Size: 316.6 KB (316628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e691cd60b95cdbb7fe7d3d74b1af54a56f440ac30d1dee94df4c4c370610b68d`  
		Last Modified: Thu, 04 Aug 2022 19:57:24 GMT  
		Size: 1.2 MB (1226852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8da76a828532ea569bd0e56b5a07a5e8bff4fe6efe22a5940260a261d113dc05`  
		Last Modified: Thu, 04 Aug 2022 19:57:23 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1705baeac52cb73666f9792b18547ce08509addd9ff3f19f6b91d21d5d10c8aa`  
		Last Modified: Thu, 04 Aug 2022 19:57:23 GMT  
		Size: 120.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.16-bullseye` - linux; arm variant v7

```console
$ docker pull memcached@sha256:25e768546f1e321b2a9031611f8ecd4081990c82f8774f7e051a5480cf18445d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.1 MB (28076294 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5959e4e12e1b75611311d3866bc95f9fe30048418f972e70fa2c671a66149fdd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 02 Aug 2022 00:58:59 GMT
ADD file:1575b776a15adacebc0875642e97a80807d42dcfc8917e1406d47af7ac244c97 in / 
# Tue, 02 Aug 2022 00:58:59 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 06:28:56 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 02 Aug 2022 06:29:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 04 Aug 2022 21:30:08 GMT
ENV MEMCACHED_VERSION=1.6.16
# Thu, 04 Aug 2022 21:30:08 GMT
ENV MEMCACHED_SHA1=724f31c3462fb6b07264d72d0043fd65545fd84a
# Thu, 04 Aug 2022 21:36:35 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 04 Aug 2022 21:36:35 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 04 Aug 2022 21:36:36 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 04 Aug 2022 21:36:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 04 Aug 2022 21:36:37 GMT
USER memcache
# Thu, 04 Aug 2022 21:36:37 GMT
EXPOSE 11211
# Thu, 04 Aug 2022 21:36:37 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:1dd75a3a9c893a7dc313f683dd62464b7eab6c6d522ee62c8a17022631830f32`  
		Last Modified: Tue, 02 Aug 2022 01:06:45 GMT  
		Size: 26.6 MB (26560586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44a675a8ce135f198539dc76b078733393238f7c7b899c8635980eed8f35f1cc`  
		Last Modified: Tue, 02 Aug 2022 09:35:13 GMT  
		Size: 4.9 KB (4890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:497b0afd04c92a1e5d41f58dbc0d5d544b8880d000c0ffbd03adb48c32c0116b`  
		Last Modified: Tue, 02 Aug 2022 09:35:13 GMT  
		Size: 312.1 KB (312067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8874fe992be272d0e0780725714c2439507699c15bfad1a073df948a34eb668d`  
		Last Modified: Fri, 05 Aug 2022 00:37:30 GMT  
		Size: 1.2 MB (1198344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cd5e042b98c640c152a56816e122c5e7b0abe91535d5d891dceed9748e42129`  
		Last Modified: Fri, 05 Aug 2022 00:37:29 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e871a0f93bdc7cb723e47f45514f914186b73d1890a53cdfe8525dd034926d59`  
		Last Modified: Fri, 05 Aug 2022 00:37:29 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.16-bullseye` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:759082b00d406f92781542ce86756eb73c5efe20acc7df6c25ac86be320a3ef5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.4 MB (31433439 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e91fe6663d9d90deed07c1d003a80fa6698137267c83310828f24a7ef63f6ef`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 02 Aug 2022 00:40:38 GMT
ADD file:6039adfbca55ed34a719c37672c664e3524130a0e2a3b8663629b8120b81b790 in / 
# Tue, 02 Aug 2022 00:40:39 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 03:56:15 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 02 Aug 2022 03:56:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 04 Aug 2022 20:33:46 GMT
ENV MEMCACHED_VERSION=1.6.16
# Thu, 04 Aug 2022 20:33:47 GMT
ENV MEMCACHED_SHA1=724f31c3462fb6b07264d72d0043fd65545fd84a
# Thu, 04 Aug 2022 20:36:17 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 04 Aug 2022 20:36:19 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 04 Aug 2022 20:36:19 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 04 Aug 2022 20:36:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 04 Aug 2022 20:36:21 GMT
USER memcache
# Thu, 04 Aug 2022 20:36:22 GMT
EXPOSE 11211
# Thu, 04 Aug 2022 20:36:23 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:a9fe95647e78b5516c7e2327355b6996e2ea295cd76ae242cbfe87f016b4e760`  
		Last Modified: Tue, 02 Aug 2022 00:46:05 GMT  
		Size: 30.1 MB (30054304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b983df009e7dc88033f53f015c09c56fd4db032d1abcade3333d8d4b515ff4af`  
		Last Modified: Tue, 02 Aug 2022 03:59:48 GMT  
		Size: 4.9 KB (4902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60720019405b50af041f391ec7dad90893ee95fc63fd6b3fb9da04850936f5db`  
		Last Modified: Tue, 02 Aug 2022 03:59:48 GMT  
		Size: 119.2 KB (119225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70569bedb4ee539337d6d3fd88e4076a1464b3a77bcfcca6604e18b815dbc402`  
		Last Modified: Thu, 04 Aug 2022 20:40:00 GMT  
		Size: 1.3 MB (1254600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:565112c01ad7b82688180f4fe70f5433126d79cc4b74e3d7f308601e2d34d9fe`  
		Last Modified: Thu, 04 Aug 2022 20:39:59 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce11290eb88924797c1fa048bd052c1243e4cb47e3469b26f3f1a3bc26472d19`  
		Last Modified: Thu, 04 Aug 2022 20:39:59 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.16-bullseye` - linux; 386

```console
$ docker pull memcached@sha256:deec44ba81c574f36b5b53185684413e4e97c3374d256e762ccf0e50fa1ff0f0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.8 MB (33762417 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9640d046f98daa1268a24f35ea7de08f83c728d88f2483d734101b09bad34768`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 02 Aug 2022 00:39:20 GMT
ADD file:f771e2286465694126158821089d801c7296376be2a56189e6041a15d2fe79f5 in / 
# Tue, 02 Aug 2022 00:39:21 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 03:12:03 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 02 Aug 2022 03:12:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 04 Aug 2022 20:28:41 GMT
ENV MEMCACHED_VERSION=1.6.16
# Thu, 04 Aug 2022 20:28:42 GMT
ENV MEMCACHED_SHA1=724f31c3462fb6b07264d72d0043fd65545fd84a
# Thu, 04 Aug 2022 20:31:30 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 04 Aug 2022 20:31:32 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 04 Aug 2022 20:31:32 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 04 Aug 2022 20:31:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 04 Aug 2022 20:31:34 GMT
USER memcache
# Thu, 04 Aug 2022 20:31:35 GMT
EXPOSE 11211
# Thu, 04 Aug 2022 20:31:36 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:90eb7f0ce9f33cf5dcd67d54c2fa606186dbaa5f95b6046f36145097267f9e53`  
		Last Modified: Tue, 02 Aug 2022 00:45:14 GMT  
		Size: 32.4 MB (32374054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:107cdc14debc414f1e6554b58402d2be697942f8f22b45d5c9b6bff8be3f332a`  
		Last Modified: Tue, 02 Aug 2022 03:15:55 GMT  
		Size: 4.8 KB (4771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b33bafb66f7f078457cf82ba6cfcbab5feae0e38bc0d959a5b50fa98fbcbf4ac`  
		Last Modified: Tue, 02 Aug 2022 03:15:55 GMT  
		Size: 130.1 KB (130114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c122afb77220a37620d69b968b43d326ed98ef7d9ed80ea06c3a7fa1c54dc73f`  
		Last Modified: Thu, 04 Aug 2022 20:35:38 GMT  
		Size: 1.3 MB (1253069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2426ab0684229e93e257d5c6357fbad018ee92d3cdcf5a7812171aa06bf82ca9`  
		Last Modified: Thu, 04 Aug 2022 20:35:38 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:240ed953e9e062d3ea6893fe34ecd1e5e060a240ae2a66092c6970c0be0eeed5`  
		Last Modified: Thu, 04 Aug 2022 20:35:38 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.16-bullseye` - linux; mips64le

```console
$ docker pull memcached@sha256:0d6798ccd4a9ac44c6ca7c358b2de6bdedbfe104de7d9987eedc68864ab8acc0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.0 MB (31002934 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aca3e1ecca25fb97ad1d376d73b212cad11874d1f051c4c4bac1b2d27abc15fd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 02 Aug 2022 01:10:34 GMT
ADD file:6dc22a1e5b5fcf23f2549406ddcc45c4e244f46e21eafa881de81fa87438e5d8 in / 
# Tue, 02 Aug 2022 01:10:38 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 03:22:53 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 02 Aug 2022 03:23:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 04 Aug 2022 20:07:25 GMT
ENV MEMCACHED_VERSION=1.6.16
# Thu, 04 Aug 2022 20:07:28 GMT
ENV MEMCACHED_SHA1=724f31c3462fb6b07264d72d0043fd65545fd84a
# Thu, 04 Aug 2022 20:14:28 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 04 Aug 2022 20:14:30 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 04 Aug 2022 20:14:35 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 04 Aug 2022 20:14:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 04 Aug 2022 20:14:40 GMT
USER memcache
# Thu, 04 Aug 2022 20:14:42 GMT
EXPOSE 11211
# Thu, 04 Aug 2022 20:14:45 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:88350749a27614c791450c256b051f023d81cdd256211274b1efac493779d2be`  
		Last Modified: Tue, 02 Aug 2022 01:21:02 GMT  
		Size: 29.6 MB (29628964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:117af7bbaadea9c81bbaa3a8a77b1ab5cd05bcac856c462cda2e81c9a40596ab`  
		Last Modified: Tue, 02 Aug 2022 03:30:45 GMT  
		Size: 4.9 KB (4863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53a16d313748bd6b2dade87de73d79edd8a08e4cb662769a717f8587abc8d5e0`  
		Last Modified: Tue, 02 Aug 2022 03:30:46 GMT  
		Size: 117.1 KB (117127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d524786af3243ee367d118f6d5260cffa06d800f492f9b4bb36c910958186933`  
		Last Modified: Thu, 04 Aug 2022 20:15:05 GMT  
		Size: 1.3 MB (1251571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4badb1f1970762d08dbd43d7e101081a5fabd3c45e18afd70636397e83102d2f`  
		Last Modified: Thu, 04 Aug 2022 20:15:04 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3102636392803c3bbff48f39e7f143e3bf9a0528365d63b90dc31cd32060d3e0`  
		Last Modified: Thu, 04 Aug 2022 20:15:04 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.16-bullseye` - linux; ppc64le

```console
$ docker pull memcached@sha256:fef67c5248379f0c7154c6298ae0236afa239c6a2e7677ff26cf67e2e902873c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.0 MB (36957550 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19ebbfa2abfbf5d8014f1a3d04cab132b47836a64e68160efb3b8c752addaedd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 02 Aug 2022 01:17:30 GMT
ADD file:3a95a896d463569ce82199957052b3467123a4bd3385a0a4e397cf08402a99c3 in / 
# Tue, 02 Aug 2022 01:17:32 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 03:45:30 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 02 Aug 2022 03:45:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 04 Aug 2022 20:31:03 GMT
ENV MEMCACHED_VERSION=1.6.16
# Thu, 04 Aug 2022 20:31:04 GMT
ENV MEMCACHED_SHA1=724f31c3462fb6b07264d72d0043fd65545fd84a
# Thu, 04 Aug 2022 20:34:08 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 04 Aug 2022 20:34:09 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 04 Aug 2022 20:34:10 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 04 Aug 2022 20:34:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 04 Aug 2022 20:34:10 GMT
USER memcache
# Thu, 04 Aug 2022 20:34:11 GMT
EXPOSE 11211
# Thu, 04 Aug 2022 20:34:11 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:5241cd116d6e6e2d62f3d8c2245b74daca9f6cc154eaccd738feb41984c74714`  
		Last Modified: Tue, 02 Aug 2022 01:24:39 GMT  
		Size: 35.3 MB (35272771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58860b5324185f5059438d063f2a2b9c8ec05e058d0c1467db47a258a089c691`  
		Last Modified: Tue, 02 Aug 2022 03:53:12 GMT  
		Size: 5.0 KB (4978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82fb13381eff7e0b9526ba592f13e09cea5295914fde283ea341e5b71cb31493`  
		Last Modified: Tue, 02 Aug 2022 03:53:13 GMT  
		Size: 356.9 KB (356918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b33f6ac4fcd819056777e9462124dfc34dca6f35e1cae56a64d12bd150e4dfc9`  
		Last Modified: Thu, 04 Aug 2022 20:38:29 GMT  
		Size: 1.3 MB (1322475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:893b74576495c7a62c5d4447a7453f60f228fbb0e6d2dc4edf7e67661c455f57`  
		Last Modified: Thu, 04 Aug 2022 20:38:28 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7855d0c39dc9730d8ec3369fa86f770bd433a903eb346e9115b7442574441f24`  
		Last Modified: Thu, 04 Aug 2022 20:38:28 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.16-bullseye` - linux; s390x

```console
$ docker pull memcached@sha256:4f7e9706bfd16d98bfb48a6435c8359a167ab733777f16f24996cad3f431bdc5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.2 MB (31211398 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6739ca31062c74398fdfec102afbacead1c25fa0decf2fa14bdecdcb6b160543`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 02 Aug 2022 00:42:27 GMT
ADD file:c2afc8990930846fbe7c99bfdfe9ea562c75feb6e3c9122431f7c9f8b5e51a7f in / 
# Tue, 02 Aug 2022 00:42:29 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 02:37:02 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 02 Aug 2022 02:37:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 04 Aug 2022 20:28:18 GMT
ENV MEMCACHED_VERSION=1.6.16
# Thu, 04 Aug 2022 20:28:18 GMT
ENV MEMCACHED_SHA1=724f31c3462fb6b07264d72d0043fd65545fd84a
# Thu, 04 Aug 2022 20:31:37 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 04 Aug 2022 20:31:37 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 04 Aug 2022 20:31:37 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 04 Aug 2022 20:31:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 04 Aug 2022 20:31:38 GMT
USER memcache
# Thu, 04 Aug 2022 20:31:38 GMT
EXPOSE 11211
# Thu, 04 Aug 2022 20:31:38 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:026d311d0716db60eba0572ea784c21031f420960510cebcc383dc53949b4db8`  
		Last Modified: Tue, 02 Aug 2022 00:48:01 GMT  
		Size: 29.6 MB (29640259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0ffdb328e548bd6b6311c78665ac8cd3be8f0b2e09691701d9b0bae0924f8f5`  
		Last Modified: Tue, 02 Aug 2022 02:41:16 GMT  
		Size: 5.0 KB (5025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fbb9677007b0ebab2fe6feab520da1962d3fcffb3490aa844681a46fcb35749`  
		Last Modified: Tue, 02 Aug 2022 02:41:16 GMT  
		Size: 324.2 KB (324183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9c93abfa1f832f2e1f02fbe7b9a489735142c2051dafa7af20d985ff2e2106b`  
		Last Modified: Thu, 04 Aug 2022 20:36:17 GMT  
		Size: 1.2 MB (1241523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f78bf4cf172bedc6ad3c92b859859b10c0394104262328d5664ddc0b1488b29`  
		Last Modified: Thu, 04 Aug 2022 20:36:17 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6a26d2d4c34166613098e1380842f1355b534e2335a1dea2128c193b7f19bec`  
		Last Modified: Thu, 04 Aug 2022 20:36:16 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:alpine`

```console
$ docker pull memcached@sha256:69942a0c1666bd15245d423a255a64f4b8543546b7c0f40a1b421f64bc40fcb8
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
$ docker pull memcached@sha256:9b2ecb3fb8713d7c971eaf6e97150fcf34735d105bab81dd53e45d18da6c6b90
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3860216 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:22e40b7fd940b01ddffc7c8fddff80d89c6572d89d7c9664343a2c1e3efe389b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 18 Jul 2022 21:00:15 GMT
ADD file:a2648378045615c3785c752423b1afc8dc1c2b213393344f4d0ca17e7255c1cb in / 
# Mon, 18 Jul 2022 21:00:15 GMT
CMD ["/bin/sh"]
# Tue, 19 Jul 2022 01:33:13 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 19 Jul 2022 01:33:14 GMT
RUN apk add --no-cache libsasl
# Thu, 04 Aug 2022 20:02:18 GMT
ENV MEMCACHED_VERSION=1.6.16
# Thu, 04 Aug 2022 20:02:18 GMT
ENV MEMCACHED_SHA1=724f31c3462fb6b07264d72d0043fd65545fd84a
# Thu, 04 Aug 2022 20:05:09 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Thu, 04 Aug 2022 20:05:09 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 04 Aug 2022 20:05:09 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 04 Aug 2022 20:05:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 04 Aug 2022 20:05:10 GMT
USER memcache
# Thu, 04 Aug 2022 20:05:10 GMT
EXPOSE 11211
# Thu, 04 Aug 2022 20:05:10 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:530afca65e2ea04227630ae746e0c85b2bd1a179379cbf2b6501b49c4cab2ccc`  
		Last Modified: Mon, 18 Jul 2022 19:09:35 GMT  
		Size: 2.8 MB (2798806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3e13ff258fbd16cc42fcdb1bd800f73f4b380857d2a6096906444ec790c6542`  
		Last Modified: Tue, 19 Jul 2022 01:36:41 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90922b6720c8f20007711c5660b8269518b50979be1cef2cb4c0b12a7ac78ff7`  
		Last Modified: Tue, 19 Jul 2022 01:36:41 GMT  
		Size: 108.3 KB (108315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51aa27d6f4905ed1e531c58fa8d22676bfac86a2ba49c01894f95245d65329f7`  
		Last Modified: Thu, 04 Aug 2022 20:06:10 GMT  
		Size: 951.4 KB (951422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35e3d85200a71563435aa4bb45d98232f964b19c4facc2bc63d6ae3db816cbb4`  
		Last Modified: Thu, 04 Aug 2022 20:06:10 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74ba9b8d8a47b35ef57b45387b27d98410a32a2814a83a6cc686136b48fbb420`  
		Last Modified: Thu, 04 Aug 2022 20:06:10 GMT  
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
$ docker pull memcached@sha256:ad6951d968e4efe51c8da00a45147c17103c337177ececea11271806da36563d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.7 MB (3744755 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c64051372a720608fa1f9fed496d62daf26dd098c6ecf5189d59c3c4aede3d8f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 18 Jul 2022 21:57:05 GMT
ADD file:9ccb70abba88b6de789b29f17770246f765ffbb072fe598580bfc29ce3213f1c in / 
# Mon, 18 Jul 2022 21:57:05 GMT
CMD ["/bin/sh"]
# Mon, 18 Jul 2022 23:40:46 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Mon, 18 Jul 2022 23:40:48 GMT
RUN apk add --no-cache libsasl
# Thu, 04 Aug 2022 20:36:31 GMT
ENV MEMCACHED_VERSION=1.6.16
# Thu, 04 Aug 2022 20:36:32 GMT
ENV MEMCACHED_SHA1=724f31c3462fb6b07264d72d0043fd65545fd84a
# Thu, 04 Aug 2022 20:39:14 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Thu, 04 Aug 2022 20:39:16 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 04 Aug 2022 20:39:16 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 04 Aug 2022 20:39:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 04 Aug 2022 20:39:18 GMT
USER memcache
# Thu, 04 Aug 2022 20:39:19 GMT
EXPOSE 11211
# Thu, 04 Aug 2022 20:39:20 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:f97344484467e4c4ebb85aae724170073799295a3442c50ab532e249bd27b412`  
		Last Modified: Mon, 18 Jul 2022 19:08:29 GMT  
		Size: 2.7 MB (2694720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7da60570c25aa47c5a2b9fcd4be47a0a93240f9f4f2ab5a4d0b52c2646f40a28`  
		Last Modified: Mon, 18 Jul 2022 23:44:19 GMT  
		Size: 1.2 KB (1240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66a722c1c0875bed8b5bc87f4e2844ed10d7d9c12755721cd2164aa8b1c690d3`  
		Last Modified: Mon, 18 Jul 2022 23:44:20 GMT  
		Size: 109.6 KB (109554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19d417474c6b68c4c39d74d0adc463d1b8efd38f3c8f97b0a06230a45762e419`  
		Last Modified: Thu, 04 Aug 2022 20:40:30 GMT  
		Size: 938.8 KB (938833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9ffa798617a9bfdd85f3d0e02e2e00587f4a41d08fdf2f2cb2e1545b83c9090`  
		Last Modified: Thu, 04 Aug 2022 20:40:30 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:953ea2e6fdf83d907c05809ff46325d9d363d4cea34f88de5c84c87be30aa90d`  
		Last Modified: Thu, 04 Aug 2022 20:40:30 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:alpine` - linux; 386

```console
$ docker pull memcached@sha256:ee1fc765b96e3511c6b013639aec361b29013747c099430e8d347cf3692fac6e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3886569 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d6788e9d28dbe037c2a56c89130413dd2dcf2e394c99b8cfe32d79eecdaa1783`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 18 Jul 2022 20:38:19 GMT
ADD file:be69b7550bf861d8fb12bdbe1edf3a0d2519a6a4da61bd04858b6258ffbf48a7 in / 
# Mon, 18 Jul 2022 20:38:19 GMT
CMD ["/bin/sh"]
# Tue, 19 Jul 2022 01:27:41 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 19 Jul 2022 01:27:42 GMT
RUN apk add --no-cache libsasl
# Thu, 04 Aug 2022 20:31:52 GMT
ENV MEMCACHED_VERSION=1.6.16
# Thu, 04 Aug 2022 20:31:53 GMT
ENV MEMCACHED_SHA1=724f31c3462fb6b07264d72d0043fd65545fd84a
# Thu, 04 Aug 2022 20:34:46 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Thu, 04 Aug 2022 20:34:48 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 04 Aug 2022 20:34:48 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 04 Aug 2022 20:34:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 04 Aug 2022 20:34:50 GMT
USER memcache
# Thu, 04 Aug 2022 20:34:51 GMT
EXPOSE 11211
# Thu, 04 Aug 2022 20:34:52 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:5d7f927419794ebb7496ac38b0659686317b2d2fac7252a4a0d40d43d5fdd662`  
		Last Modified: Mon, 18 Jul 2022 19:09:22 GMT  
		Size: 2.8 MB (2802334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bd21aea877c073ddb40c30afa2f3e8f58c6fef7737835158747cf175df4ef4e`  
		Last Modified: Tue, 19 Jul 2022 01:31:30 GMT  
		Size: 1.2 KB (1241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fba37b4bd3e4b8bdb4184c8f065ce7b15f3fadd48bbb46f43623a90737e59911`  
		Last Modified: Tue, 19 Jul 2022 01:31:31 GMT  
		Size: 119.8 KB (119833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bf6c5b49cad3fa44a9ca5f146e497c4fb38ee5f14d27a2164224225a90e55aa`  
		Last Modified: Thu, 04 Aug 2022 20:36:09 GMT  
		Size: 962.8 KB (962757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cff8368515defad6347e63b43774e1ab0921279b4081ee4d8d36d28079e6c5d`  
		Last Modified: Thu, 04 Aug 2022 20:36:09 GMT  
		Size: 283.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e402b0471e504b912c3be68ebc0b6934213ca421d3b90ab8eb15f698c24157a`  
		Last Modified: Thu, 04 Aug 2022 20:36:09 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:alpine` - linux; ppc64le

```console
$ docker pull memcached@sha256:b9d56b200da6dd58c0da595669a18edfb7c77db42a4305b20a9a72c43b1bb034
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3898842 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4292cb4f0bd2997ab218f436690f4d170d349cead12c74fbc6c9acc4489ee307`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 18 Jul 2022 21:29:30 GMT
ADD file:69e4080f15f54e2d8f8aa25fdcba9c01dde149d43592edd5023106675e54a769 in / 
# Mon, 18 Jul 2022 21:29:31 GMT
CMD ["/bin/sh"]
# Tue, 02 Aug 2022 03:48:55 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 02 Aug 2022 03:48:57 GMT
RUN apk add --no-cache libsasl
# Thu, 04 Aug 2022 20:34:28 GMT
ENV MEMCACHED_VERSION=1.6.16
# Thu, 04 Aug 2022 20:34:29 GMT
ENV MEMCACHED_SHA1=724f31c3462fb6b07264d72d0043fd65545fd84a
# Thu, 04 Aug 2022 20:37:42 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Thu, 04 Aug 2022 20:37:42 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 04 Aug 2022 20:37:43 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 04 Aug 2022 20:37:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 04 Aug 2022 20:37:44 GMT
USER memcache
# Thu, 04 Aug 2022 20:37:44 GMT
EXPOSE 11211
# Thu, 04 Aug 2022 20:37:44 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:602896d442490cd3fbb6599f0f862d3673b7cd58eca3ac842b8e09bf8d012443`  
		Last Modified: Mon, 18 Jul 2022 19:09:09 GMT  
		Size: 2.8 MB (2789923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e6cec9872fd3c66c2b19cff2dd853136a16b03e523f70d0cd8875dff75abdf6`  
		Last Modified: Tue, 02 Aug 2022 03:53:48 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2420696d84e23c3f6e09fb61166d22a8b83d011559aa421d5d5e9f4ccf2f06a`  
		Last Modified: Tue, 02 Aug 2022 03:53:48 GMT  
		Size: 126.1 KB (126059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c706cce31e40f8bd79f2caa6ecef5e085849307288d79ebffc91b574118f04ba`  
		Last Modified: Thu, 04 Aug 2022 20:39:03 GMT  
		Size: 981.2 KB (981184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e86b61d9d1ecc2880ffc457445a2f5dcfaa3317fa84796de7bb78f30b5c31e15`  
		Last Modified: Thu, 04 Aug 2022 20:39:03 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74db60069b975f4fa4efaf1fe6ee2af6977e661683c83a54c141faff25255f11`  
		Last Modified: Thu, 04 Aug 2022 20:39:03 GMT  
		Size: 120.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:alpine` - linux; s390x

```console
$ docker pull memcached@sha256:62da518bff73ec0e140de7ecadbc4c0bbeaec3886cf144ac9deea64a95905fa7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.6 MB (3636817 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:057cc21d3a6bf40d3f50d6b8ce6d9004c65a7fb5a448f98761e044c79691adf5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 18 Jul 2022 20:41:35 GMT
ADD file:deaa573cd61e07709846a5300fb627a8610e9754129c085ed483ff8897d0c002 in / 
# Mon, 18 Jul 2022 20:41:36 GMT
CMD ["/bin/sh"]
# Mon, 18 Jul 2022 22:46:43 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Mon, 18 Jul 2022 22:46:46 GMT
RUN apk add --no-cache libsasl
# Thu, 04 Aug 2022 20:31:55 GMT
ENV MEMCACHED_VERSION=1.6.16
# Thu, 04 Aug 2022 20:31:55 GMT
ENV MEMCACHED_SHA1=724f31c3462fb6b07264d72d0043fd65545fd84a
# Thu, 04 Aug 2022 20:35:27 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Thu, 04 Aug 2022 20:35:27 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 04 Aug 2022 20:35:27 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 04 Aug 2022 20:35:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 04 Aug 2022 20:35:28 GMT
USER memcache
# Thu, 04 Aug 2022 20:35:28 GMT
EXPOSE 11211
# Thu, 04 Aug 2022 20:35:28 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:5f1840d5bacf4162a87f497e22d94bce946e660bdfce8eeefcbf7bd0beb193f3`  
		Last Modified: Mon, 18 Jul 2022 20:42:36 GMT  
		Size: 2.6 MB (2580798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2b6f46f9ccd4c19bfc103544d0d83ceef7feae4d70d25397d620ca381065659`  
		Last Modified: Mon, 18 Jul 2022 22:52:40 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f491a581763941ae0ec0ec035bdfb8073504d7fdc2eec6eb1e70878f26c16351`  
		Last Modified: Mon, 18 Jul 2022 22:52:40 GMT  
		Size: 112.5 KB (112503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:978f61b805ce2eb5610c877e3b8dc826f82016a7cf4af02737c7e2c44a1ede3f`  
		Last Modified: Thu, 04 Aug 2022 20:36:36 GMT  
		Size: 941.8 KB (941845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0a55bbbae5442cc2430fd5859fdd4c002e763bfe72f074645ea038f97652422`  
		Last Modified: Thu, 04 Aug 2022 20:36:36 GMT  
		Size: 283.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16ad3c74a3fe0b757743e632dbef104cea78e39b57e4155dab2020488d5b4546`  
		Last Modified: Thu, 04 Aug 2022 20:36:36 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:alpine3.16`

```console
$ docker pull memcached@sha256:6f612899171e3ec7380f48ca3bc4043482423db2462846c9a55124b44e3dee5d
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
$ docker pull memcached@sha256:9b2ecb3fb8713d7c971eaf6e97150fcf34735d105bab81dd53e45d18da6c6b90
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3860216 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:22e40b7fd940b01ddffc7c8fddff80d89c6572d89d7c9664343a2c1e3efe389b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 18 Jul 2022 21:00:15 GMT
ADD file:a2648378045615c3785c752423b1afc8dc1c2b213393344f4d0ca17e7255c1cb in / 
# Mon, 18 Jul 2022 21:00:15 GMT
CMD ["/bin/sh"]
# Tue, 19 Jul 2022 01:33:13 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 19 Jul 2022 01:33:14 GMT
RUN apk add --no-cache libsasl
# Thu, 04 Aug 2022 20:02:18 GMT
ENV MEMCACHED_VERSION=1.6.16
# Thu, 04 Aug 2022 20:02:18 GMT
ENV MEMCACHED_SHA1=724f31c3462fb6b07264d72d0043fd65545fd84a
# Thu, 04 Aug 2022 20:05:09 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Thu, 04 Aug 2022 20:05:09 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 04 Aug 2022 20:05:09 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 04 Aug 2022 20:05:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 04 Aug 2022 20:05:10 GMT
USER memcache
# Thu, 04 Aug 2022 20:05:10 GMT
EXPOSE 11211
# Thu, 04 Aug 2022 20:05:10 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:530afca65e2ea04227630ae746e0c85b2bd1a179379cbf2b6501b49c4cab2ccc`  
		Last Modified: Mon, 18 Jul 2022 19:09:35 GMT  
		Size: 2.8 MB (2798806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3e13ff258fbd16cc42fcdb1bd800f73f4b380857d2a6096906444ec790c6542`  
		Last Modified: Tue, 19 Jul 2022 01:36:41 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90922b6720c8f20007711c5660b8269518b50979be1cef2cb4c0b12a7ac78ff7`  
		Last Modified: Tue, 19 Jul 2022 01:36:41 GMT  
		Size: 108.3 KB (108315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51aa27d6f4905ed1e531c58fa8d22676bfac86a2ba49c01894f95245d65329f7`  
		Last Modified: Thu, 04 Aug 2022 20:06:10 GMT  
		Size: 951.4 KB (951422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35e3d85200a71563435aa4bb45d98232f964b19c4facc2bc63d6ae3db816cbb4`  
		Last Modified: Thu, 04 Aug 2022 20:06:10 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74ba9b8d8a47b35ef57b45387b27d98410a32a2814a83a6cc686136b48fbb420`  
		Last Modified: Thu, 04 Aug 2022 20:06:10 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:alpine3.16` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:ad6951d968e4efe51c8da00a45147c17103c337177ececea11271806da36563d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.7 MB (3744755 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c64051372a720608fa1f9fed496d62daf26dd098c6ecf5189d59c3c4aede3d8f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 18 Jul 2022 21:57:05 GMT
ADD file:9ccb70abba88b6de789b29f17770246f765ffbb072fe598580bfc29ce3213f1c in / 
# Mon, 18 Jul 2022 21:57:05 GMT
CMD ["/bin/sh"]
# Mon, 18 Jul 2022 23:40:46 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Mon, 18 Jul 2022 23:40:48 GMT
RUN apk add --no-cache libsasl
# Thu, 04 Aug 2022 20:36:31 GMT
ENV MEMCACHED_VERSION=1.6.16
# Thu, 04 Aug 2022 20:36:32 GMT
ENV MEMCACHED_SHA1=724f31c3462fb6b07264d72d0043fd65545fd84a
# Thu, 04 Aug 2022 20:39:14 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Thu, 04 Aug 2022 20:39:16 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 04 Aug 2022 20:39:16 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 04 Aug 2022 20:39:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 04 Aug 2022 20:39:18 GMT
USER memcache
# Thu, 04 Aug 2022 20:39:19 GMT
EXPOSE 11211
# Thu, 04 Aug 2022 20:39:20 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:f97344484467e4c4ebb85aae724170073799295a3442c50ab532e249bd27b412`  
		Last Modified: Mon, 18 Jul 2022 19:08:29 GMT  
		Size: 2.7 MB (2694720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7da60570c25aa47c5a2b9fcd4be47a0a93240f9f4f2ab5a4d0b52c2646f40a28`  
		Last Modified: Mon, 18 Jul 2022 23:44:19 GMT  
		Size: 1.2 KB (1240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66a722c1c0875bed8b5bc87f4e2844ed10d7d9c12755721cd2164aa8b1c690d3`  
		Last Modified: Mon, 18 Jul 2022 23:44:20 GMT  
		Size: 109.6 KB (109554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19d417474c6b68c4c39d74d0adc463d1b8efd38f3c8f97b0a06230a45762e419`  
		Last Modified: Thu, 04 Aug 2022 20:40:30 GMT  
		Size: 938.8 KB (938833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9ffa798617a9bfdd85f3d0e02e2e00587f4a41d08fdf2f2cb2e1545b83c9090`  
		Last Modified: Thu, 04 Aug 2022 20:40:30 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:953ea2e6fdf83d907c05809ff46325d9d363d4cea34f88de5c84c87be30aa90d`  
		Last Modified: Thu, 04 Aug 2022 20:40:30 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:alpine3.16` - linux; 386

```console
$ docker pull memcached@sha256:ee1fc765b96e3511c6b013639aec361b29013747c099430e8d347cf3692fac6e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3886569 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d6788e9d28dbe037c2a56c89130413dd2dcf2e394c99b8cfe32d79eecdaa1783`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 18 Jul 2022 20:38:19 GMT
ADD file:be69b7550bf861d8fb12bdbe1edf3a0d2519a6a4da61bd04858b6258ffbf48a7 in / 
# Mon, 18 Jul 2022 20:38:19 GMT
CMD ["/bin/sh"]
# Tue, 19 Jul 2022 01:27:41 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 19 Jul 2022 01:27:42 GMT
RUN apk add --no-cache libsasl
# Thu, 04 Aug 2022 20:31:52 GMT
ENV MEMCACHED_VERSION=1.6.16
# Thu, 04 Aug 2022 20:31:53 GMT
ENV MEMCACHED_SHA1=724f31c3462fb6b07264d72d0043fd65545fd84a
# Thu, 04 Aug 2022 20:34:46 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Thu, 04 Aug 2022 20:34:48 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 04 Aug 2022 20:34:48 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 04 Aug 2022 20:34:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 04 Aug 2022 20:34:50 GMT
USER memcache
# Thu, 04 Aug 2022 20:34:51 GMT
EXPOSE 11211
# Thu, 04 Aug 2022 20:34:52 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:5d7f927419794ebb7496ac38b0659686317b2d2fac7252a4a0d40d43d5fdd662`  
		Last Modified: Mon, 18 Jul 2022 19:09:22 GMT  
		Size: 2.8 MB (2802334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bd21aea877c073ddb40c30afa2f3e8f58c6fef7737835158747cf175df4ef4e`  
		Last Modified: Tue, 19 Jul 2022 01:31:30 GMT  
		Size: 1.2 KB (1241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fba37b4bd3e4b8bdb4184c8f065ce7b15f3fadd48bbb46f43623a90737e59911`  
		Last Modified: Tue, 19 Jul 2022 01:31:31 GMT  
		Size: 119.8 KB (119833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bf6c5b49cad3fa44a9ca5f146e497c4fb38ee5f14d27a2164224225a90e55aa`  
		Last Modified: Thu, 04 Aug 2022 20:36:09 GMT  
		Size: 962.8 KB (962757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cff8368515defad6347e63b43774e1ab0921279b4081ee4d8d36d28079e6c5d`  
		Last Modified: Thu, 04 Aug 2022 20:36:09 GMT  
		Size: 283.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e402b0471e504b912c3be68ebc0b6934213ca421d3b90ab8eb15f698c24157a`  
		Last Modified: Thu, 04 Aug 2022 20:36:09 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:alpine3.16` - linux; ppc64le

```console
$ docker pull memcached@sha256:b9d56b200da6dd58c0da595669a18edfb7c77db42a4305b20a9a72c43b1bb034
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3898842 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4292cb4f0bd2997ab218f436690f4d170d349cead12c74fbc6c9acc4489ee307`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 18 Jul 2022 21:29:30 GMT
ADD file:69e4080f15f54e2d8f8aa25fdcba9c01dde149d43592edd5023106675e54a769 in / 
# Mon, 18 Jul 2022 21:29:31 GMT
CMD ["/bin/sh"]
# Tue, 02 Aug 2022 03:48:55 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 02 Aug 2022 03:48:57 GMT
RUN apk add --no-cache libsasl
# Thu, 04 Aug 2022 20:34:28 GMT
ENV MEMCACHED_VERSION=1.6.16
# Thu, 04 Aug 2022 20:34:29 GMT
ENV MEMCACHED_SHA1=724f31c3462fb6b07264d72d0043fd65545fd84a
# Thu, 04 Aug 2022 20:37:42 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Thu, 04 Aug 2022 20:37:42 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 04 Aug 2022 20:37:43 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 04 Aug 2022 20:37:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 04 Aug 2022 20:37:44 GMT
USER memcache
# Thu, 04 Aug 2022 20:37:44 GMT
EXPOSE 11211
# Thu, 04 Aug 2022 20:37:44 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:602896d442490cd3fbb6599f0f862d3673b7cd58eca3ac842b8e09bf8d012443`  
		Last Modified: Mon, 18 Jul 2022 19:09:09 GMT  
		Size: 2.8 MB (2789923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e6cec9872fd3c66c2b19cff2dd853136a16b03e523f70d0cd8875dff75abdf6`  
		Last Modified: Tue, 02 Aug 2022 03:53:48 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2420696d84e23c3f6e09fb61166d22a8b83d011559aa421d5d5e9f4ccf2f06a`  
		Last Modified: Tue, 02 Aug 2022 03:53:48 GMT  
		Size: 126.1 KB (126059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c706cce31e40f8bd79f2caa6ecef5e085849307288d79ebffc91b574118f04ba`  
		Last Modified: Thu, 04 Aug 2022 20:39:03 GMT  
		Size: 981.2 KB (981184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e86b61d9d1ecc2880ffc457445a2f5dcfaa3317fa84796de7bb78f30b5c31e15`  
		Last Modified: Thu, 04 Aug 2022 20:39:03 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74db60069b975f4fa4efaf1fe6ee2af6977e661683c83a54c141faff25255f11`  
		Last Modified: Thu, 04 Aug 2022 20:39:03 GMT  
		Size: 120.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:alpine3.16` - linux; s390x

```console
$ docker pull memcached@sha256:62da518bff73ec0e140de7ecadbc4c0bbeaec3886cf144ac9deea64a95905fa7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.6 MB (3636817 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:057cc21d3a6bf40d3f50d6b8ce6d9004c65a7fb5a448f98761e044c79691adf5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 18 Jul 2022 20:41:35 GMT
ADD file:deaa573cd61e07709846a5300fb627a8610e9754129c085ed483ff8897d0c002 in / 
# Mon, 18 Jul 2022 20:41:36 GMT
CMD ["/bin/sh"]
# Mon, 18 Jul 2022 22:46:43 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Mon, 18 Jul 2022 22:46:46 GMT
RUN apk add --no-cache libsasl
# Thu, 04 Aug 2022 20:31:55 GMT
ENV MEMCACHED_VERSION=1.6.16
# Thu, 04 Aug 2022 20:31:55 GMT
ENV MEMCACHED_SHA1=724f31c3462fb6b07264d72d0043fd65545fd84a
# Thu, 04 Aug 2022 20:35:27 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Thu, 04 Aug 2022 20:35:27 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 04 Aug 2022 20:35:27 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 04 Aug 2022 20:35:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 04 Aug 2022 20:35:28 GMT
USER memcache
# Thu, 04 Aug 2022 20:35:28 GMT
EXPOSE 11211
# Thu, 04 Aug 2022 20:35:28 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:5f1840d5bacf4162a87f497e22d94bce946e660bdfce8eeefcbf7bd0beb193f3`  
		Last Modified: Mon, 18 Jul 2022 20:42:36 GMT  
		Size: 2.6 MB (2580798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2b6f46f9ccd4c19bfc103544d0d83ceef7feae4d70d25397d620ca381065659`  
		Last Modified: Mon, 18 Jul 2022 22:52:40 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f491a581763941ae0ec0ec035bdfb8073504d7fdc2eec6eb1e70878f26c16351`  
		Last Modified: Mon, 18 Jul 2022 22:52:40 GMT  
		Size: 112.5 KB (112503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:978f61b805ce2eb5610c877e3b8dc826f82016a7cf4af02737c7e2c44a1ede3f`  
		Last Modified: Thu, 04 Aug 2022 20:36:36 GMT  
		Size: 941.8 KB (941845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0a55bbbae5442cc2430fd5859fdd4c002e763bfe72f074645ea038f97652422`  
		Last Modified: Thu, 04 Aug 2022 20:36:36 GMT  
		Size: 283.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16ad3c74a3fe0b757743e632dbef104cea78e39b57e4155dab2020488d5b4546`  
		Last Modified: Thu, 04 Aug 2022 20:36:36 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:bullseye`

```console
$ docker pull memcached@sha256:0afaa8e890393e089efc991b62ec98d3dd53e5da995abfa548e5df9c70722015
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
$ docker pull memcached@sha256:d6479777ae4663bb6752d9e779a2180adeae2e6f91da834a6c042665ef961b19
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.0 MB (32956000 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:36a225838cd6927616fc3c9afc4fc26e1fbe4097250b113b6b8508e02ae6a589`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 02 Aug 2022 01:20:04 GMT
ADD file:0eae0dca665c7044bf242cb1fc92cb8ea744f5af2dd376a558c90bc47349aefe in / 
# Tue, 02 Aug 2022 01:20:05 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 04:45:12 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 02 Aug 2022 04:45:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 04 Aug 2022 19:59:25 GMT
ENV MEMCACHED_VERSION=1.6.16
# Thu, 04 Aug 2022 19:59:25 GMT
ENV MEMCACHED_SHA1=724f31c3462fb6b07264d72d0043fd65545fd84a
# Thu, 04 Aug 2022 20:02:08 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 04 Aug 2022 20:02:08 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 04 Aug 2022 20:02:08 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 04 Aug 2022 20:02:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 04 Aug 2022 20:02:09 GMT
USER memcache
# Thu, 04 Aug 2022 20:02:09 GMT
EXPOSE 11211
# Thu, 04 Aug 2022 20:02:09 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:1efc276f4ff952c055dea726cfc96ec6a4fdb8b62d9eed816bd2b788f2860ad7`  
		Last Modified: Tue, 02 Aug 2022 01:24:13 GMT  
		Size: 31.4 MB (31366757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60bd6790acf68c1ccc4757e879b51b4dbc273681e1f30606a2ccd4b55623d288`  
		Last Modified: Tue, 02 Aug 2022 04:48:24 GMT  
		Size: 5.0 KB (4980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e72821989d416909e21411733d7d034cfa908016dceb0b6e2717a5fb9faa617`  
		Last Modified: Tue, 02 Aug 2022 04:48:24 GMT  
		Size: 328.1 KB (328097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a972a764145eff4153208b9f8bed20e2179ececcec6e6d462d74400d526ccb4c`  
		Last Modified: Thu, 04 Aug 2022 20:05:45 GMT  
		Size: 1.3 MB (1255762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc9c8a212883923ae20b3e2d671f8dcc32307603465cf915c7e83bd5ac522c69`  
		Last Modified: Thu, 04 Aug 2022 20:05:45 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:157eedd0af5feece73dbebf45897c44894a10678feca71d5d57ac4904492badc`  
		Last Modified: Thu, 04 Aug 2022 20:05:46 GMT  
		Size: 118.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:bullseye` - linux; arm variant v5

```console
$ docker pull memcached@sha256:39515e68cebee2b2b88891c2b46b1c517587063301f77bbf7c312f6f9b372d65
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.5 MB (30454297 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8bf4bc30f264f1f9a0ede671e3a081ea54d1b6c3127ad5d9d4df3de21a985f5a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 02 Aug 2022 00:49:10 GMT
ADD file:4cd2f95737fd3007912428eeac56036c9e67e989e66cec08a8be99da47f88494 in / 
# Tue, 02 Aug 2022 00:49:10 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 01:58:42 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 02 Aug 2022 01:58:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 04 Aug 2022 19:50:51 GMT
ENV MEMCACHED_VERSION=1.6.16
# Thu, 04 Aug 2022 19:50:51 GMT
ENV MEMCACHED_SHA1=724f31c3462fb6b07264d72d0043fd65545fd84a
# Thu, 04 Aug 2022 19:56:43 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 04 Aug 2022 19:56:44 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 04 Aug 2022 19:56:44 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 04 Aug 2022 19:56:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 04 Aug 2022 19:56:44 GMT
USER memcache
# Thu, 04 Aug 2022 19:56:44 GMT
EXPOSE 11211
# Thu, 04 Aug 2022 19:56:45 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:5890b0ca6af5e8467a488e68716691950496a8f247d0495c2d595ddcb1893aff`  
		Last Modified: Tue, 02 Aug 2022 00:56:06 GMT  
		Size: 28.9 MB (28905515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e34350eb48491f2ab07c0f07724d37412df97ee9093c7c2458c9917afe37a42d`  
		Last Modified: Tue, 02 Aug 2022 02:04:59 GMT  
		Size: 4.9 KB (4894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36ecb6d2f4e3224a48197a5aa9d40970083bf4a92f41fbb493ac5adf9441a4ad`  
		Last Modified: Tue, 02 Aug 2022 02:04:59 GMT  
		Size: 316.6 KB (316628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e691cd60b95cdbb7fe7d3d74b1af54a56f440ac30d1dee94df4c4c370610b68d`  
		Last Modified: Thu, 04 Aug 2022 19:57:24 GMT  
		Size: 1.2 MB (1226852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8da76a828532ea569bd0e56b5a07a5e8bff4fe6efe22a5940260a261d113dc05`  
		Last Modified: Thu, 04 Aug 2022 19:57:23 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1705baeac52cb73666f9792b18547ce08509addd9ff3f19f6b91d21d5d10c8aa`  
		Last Modified: Thu, 04 Aug 2022 19:57:23 GMT  
		Size: 120.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:bullseye` - linux; arm variant v7

```console
$ docker pull memcached@sha256:25e768546f1e321b2a9031611f8ecd4081990c82f8774f7e051a5480cf18445d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.1 MB (28076294 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5959e4e12e1b75611311d3866bc95f9fe30048418f972e70fa2c671a66149fdd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 02 Aug 2022 00:58:59 GMT
ADD file:1575b776a15adacebc0875642e97a80807d42dcfc8917e1406d47af7ac244c97 in / 
# Tue, 02 Aug 2022 00:58:59 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 06:28:56 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 02 Aug 2022 06:29:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 04 Aug 2022 21:30:08 GMT
ENV MEMCACHED_VERSION=1.6.16
# Thu, 04 Aug 2022 21:30:08 GMT
ENV MEMCACHED_SHA1=724f31c3462fb6b07264d72d0043fd65545fd84a
# Thu, 04 Aug 2022 21:36:35 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 04 Aug 2022 21:36:35 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 04 Aug 2022 21:36:36 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 04 Aug 2022 21:36:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 04 Aug 2022 21:36:37 GMT
USER memcache
# Thu, 04 Aug 2022 21:36:37 GMT
EXPOSE 11211
# Thu, 04 Aug 2022 21:36:37 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:1dd75a3a9c893a7dc313f683dd62464b7eab6c6d522ee62c8a17022631830f32`  
		Last Modified: Tue, 02 Aug 2022 01:06:45 GMT  
		Size: 26.6 MB (26560586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44a675a8ce135f198539dc76b078733393238f7c7b899c8635980eed8f35f1cc`  
		Last Modified: Tue, 02 Aug 2022 09:35:13 GMT  
		Size: 4.9 KB (4890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:497b0afd04c92a1e5d41f58dbc0d5d544b8880d000c0ffbd03adb48c32c0116b`  
		Last Modified: Tue, 02 Aug 2022 09:35:13 GMT  
		Size: 312.1 KB (312067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8874fe992be272d0e0780725714c2439507699c15bfad1a073df948a34eb668d`  
		Last Modified: Fri, 05 Aug 2022 00:37:30 GMT  
		Size: 1.2 MB (1198344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cd5e042b98c640c152a56816e122c5e7b0abe91535d5d891dceed9748e42129`  
		Last Modified: Fri, 05 Aug 2022 00:37:29 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e871a0f93bdc7cb723e47f45514f914186b73d1890a53cdfe8525dd034926d59`  
		Last Modified: Fri, 05 Aug 2022 00:37:29 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:bullseye` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:759082b00d406f92781542ce86756eb73c5efe20acc7df6c25ac86be320a3ef5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.4 MB (31433439 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e91fe6663d9d90deed07c1d003a80fa6698137267c83310828f24a7ef63f6ef`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 02 Aug 2022 00:40:38 GMT
ADD file:6039adfbca55ed34a719c37672c664e3524130a0e2a3b8663629b8120b81b790 in / 
# Tue, 02 Aug 2022 00:40:39 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 03:56:15 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 02 Aug 2022 03:56:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 04 Aug 2022 20:33:46 GMT
ENV MEMCACHED_VERSION=1.6.16
# Thu, 04 Aug 2022 20:33:47 GMT
ENV MEMCACHED_SHA1=724f31c3462fb6b07264d72d0043fd65545fd84a
# Thu, 04 Aug 2022 20:36:17 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 04 Aug 2022 20:36:19 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 04 Aug 2022 20:36:19 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 04 Aug 2022 20:36:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 04 Aug 2022 20:36:21 GMT
USER memcache
# Thu, 04 Aug 2022 20:36:22 GMT
EXPOSE 11211
# Thu, 04 Aug 2022 20:36:23 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:a9fe95647e78b5516c7e2327355b6996e2ea295cd76ae242cbfe87f016b4e760`  
		Last Modified: Tue, 02 Aug 2022 00:46:05 GMT  
		Size: 30.1 MB (30054304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b983df009e7dc88033f53f015c09c56fd4db032d1abcade3333d8d4b515ff4af`  
		Last Modified: Tue, 02 Aug 2022 03:59:48 GMT  
		Size: 4.9 KB (4902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60720019405b50af041f391ec7dad90893ee95fc63fd6b3fb9da04850936f5db`  
		Last Modified: Tue, 02 Aug 2022 03:59:48 GMT  
		Size: 119.2 KB (119225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70569bedb4ee539337d6d3fd88e4076a1464b3a77bcfcca6604e18b815dbc402`  
		Last Modified: Thu, 04 Aug 2022 20:40:00 GMT  
		Size: 1.3 MB (1254600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:565112c01ad7b82688180f4fe70f5433126d79cc4b74e3d7f308601e2d34d9fe`  
		Last Modified: Thu, 04 Aug 2022 20:39:59 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce11290eb88924797c1fa048bd052c1243e4cb47e3469b26f3f1a3bc26472d19`  
		Last Modified: Thu, 04 Aug 2022 20:39:59 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:bullseye` - linux; 386

```console
$ docker pull memcached@sha256:deec44ba81c574f36b5b53185684413e4e97c3374d256e762ccf0e50fa1ff0f0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.8 MB (33762417 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9640d046f98daa1268a24f35ea7de08f83c728d88f2483d734101b09bad34768`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 02 Aug 2022 00:39:20 GMT
ADD file:f771e2286465694126158821089d801c7296376be2a56189e6041a15d2fe79f5 in / 
# Tue, 02 Aug 2022 00:39:21 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 03:12:03 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 02 Aug 2022 03:12:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 04 Aug 2022 20:28:41 GMT
ENV MEMCACHED_VERSION=1.6.16
# Thu, 04 Aug 2022 20:28:42 GMT
ENV MEMCACHED_SHA1=724f31c3462fb6b07264d72d0043fd65545fd84a
# Thu, 04 Aug 2022 20:31:30 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 04 Aug 2022 20:31:32 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 04 Aug 2022 20:31:32 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 04 Aug 2022 20:31:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 04 Aug 2022 20:31:34 GMT
USER memcache
# Thu, 04 Aug 2022 20:31:35 GMT
EXPOSE 11211
# Thu, 04 Aug 2022 20:31:36 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:90eb7f0ce9f33cf5dcd67d54c2fa606186dbaa5f95b6046f36145097267f9e53`  
		Last Modified: Tue, 02 Aug 2022 00:45:14 GMT  
		Size: 32.4 MB (32374054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:107cdc14debc414f1e6554b58402d2be697942f8f22b45d5c9b6bff8be3f332a`  
		Last Modified: Tue, 02 Aug 2022 03:15:55 GMT  
		Size: 4.8 KB (4771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b33bafb66f7f078457cf82ba6cfcbab5feae0e38bc0d959a5b50fa98fbcbf4ac`  
		Last Modified: Tue, 02 Aug 2022 03:15:55 GMT  
		Size: 130.1 KB (130114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c122afb77220a37620d69b968b43d326ed98ef7d9ed80ea06c3a7fa1c54dc73f`  
		Last Modified: Thu, 04 Aug 2022 20:35:38 GMT  
		Size: 1.3 MB (1253069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2426ab0684229e93e257d5c6357fbad018ee92d3cdcf5a7812171aa06bf82ca9`  
		Last Modified: Thu, 04 Aug 2022 20:35:38 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:240ed953e9e062d3ea6893fe34ecd1e5e060a240ae2a66092c6970c0be0eeed5`  
		Last Modified: Thu, 04 Aug 2022 20:35:38 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:bullseye` - linux; mips64le

```console
$ docker pull memcached@sha256:0d6798ccd4a9ac44c6ca7c358b2de6bdedbfe104de7d9987eedc68864ab8acc0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.0 MB (31002934 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aca3e1ecca25fb97ad1d376d73b212cad11874d1f051c4c4bac1b2d27abc15fd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 02 Aug 2022 01:10:34 GMT
ADD file:6dc22a1e5b5fcf23f2549406ddcc45c4e244f46e21eafa881de81fa87438e5d8 in / 
# Tue, 02 Aug 2022 01:10:38 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 03:22:53 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 02 Aug 2022 03:23:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 04 Aug 2022 20:07:25 GMT
ENV MEMCACHED_VERSION=1.6.16
# Thu, 04 Aug 2022 20:07:28 GMT
ENV MEMCACHED_SHA1=724f31c3462fb6b07264d72d0043fd65545fd84a
# Thu, 04 Aug 2022 20:14:28 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 04 Aug 2022 20:14:30 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 04 Aug 2022 20:14:35 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 04 Aug 2022 20:14:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 04 Aug 2022 20:14:40 GMT
USER memcache
# Thu, 04 Aug 2022 20:14:42 GMT
EXPOSE 11211
# Thu, 04 Aug 2022 20:14:45 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:88350749a27614c791450c256b051f023d81cdd256211274b1efac493779d2be`  
		Last Modified: Tue, 02 Aug 2022 01:21:02 GMT  
		Size: 29.6 MB (29628964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:117af7bbaadea9c81bbaa3a8a77b1ab5cd05bcac856c462cda2e81c9a40596ab`  
		Last Modified: Tue, 02 Aug 2022 03:30:45 GMT  
		Size: 4.9 KB (4863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53a16d313748bd6b2dade87de73d79edd8a08e4cb662769a717f8587abc8d5e0`  
		Last Modified: Tue, 02 Aug 2022 03:30:46 GMT  
		Size: 117.1 KB (117127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d524786af3243ee367d118f6d5260cffa06d800f492f9b4bb36c910958186933`  
		Last Modified: Thu, 04 Aug 2022 20:15:05 GMT  
		Size: 1.3 MB (1251571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4badb1f1970762d08dbd43d7e101081a5fabd3c45e18afd70636397e83102d2f`  
		Last Modified: Thu, 04 Aug 2022 20:15:04 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3102636392803c3bbff48f39e7f143e3bf9a0528365d63b90dc31cd32060d3e0`  
		Last Modified: Thu, 04 Aug 2022 20:15:04 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:bullseye` - linux; ppc64le

```console
$ docker pull memcached@sha256:fef67c5248379f0c7154c6298ae0236afa239c6a2e7677ff26cf67e2e902873c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.0 MB (36957550 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19ebbfa2abfbf5d8014f1a3d04cab132b47836a64e68160efb3b8c752addaedd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 02 Aug 2022 01:17:30 GMT
ADD file:3a95a896d463569ce82199957052b3467123a4bd3385a0a4e397cf08402a99c3 in / 
# Tue, 02 Aug 2022 01:17:32 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 03:45:30 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 02 Aug 2022 03:45:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 04 Aug 2022 20:31:03 GMT
ENV MEMCACHED_VERSION=1.6.16
# Thu, 04 Aug 2022 20:31:04 GMT
ENV MEMCACHED_SHA1=724f31c3462fb6b07264d72d0043fd65545fd84a
# Thu, 04 Aug 2022 20:34:08 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 04 Aug 2022 20:34:09 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 04 Aug 2022 20:34:10 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 04 Aug 2022 20:34:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 04 Aug 2022 20:34:10 GMT
USER memcache
# Thu, 04 Aug 2022 20:34:11 GMT
EXPOSE 11211
# Thu, 04 Aug 2022 20:34:11 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:5241cd116d6e6e2d62f3d8c2245b74daca9f6cc154eaccd738feb41984c74714`  
		Last Modified: Tue, 02 Aug 2022 01:24:39 GMT  
		Size: 35.3 MB (35272771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58860b5324185f5059438d063f2a2b9c8ec05e058d0c1467db47a258a089c691`  
		Last Modified: Tue, 02 Aug 2022 03:53:12 GMT  
		Size: 5.0 KB (4978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82fb13381eff7e0b9526ba592f13e09cea5295914fde283ea341e5b71cb31493`  
		Last Modified: Tue, 02 Aug 2022 03:53:13 GMT  
		Size: 356.9 KB (356918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b33f6ac4fcd819056777e9462124dfc34dca6f35e1cae56a64d12bd150e4dfc9`  
		Last Modified: Thu, 04 Aug 2022 20:38:29 GMT  
		Size: 1.3 MB (1322475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:893b74576495c7a62c5d4447a7453f60f228fbb0e6d2dc4edf7e67661c455f57`  
		Last Modified: Thu, 04 Aug 2022 20:38:28 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7855d0c39dc9730d8ec3369fa86f770bd433a903eb346e9115b7442574441f24`  
		Last Modified: Thu, 04 Aug 2022 20:38:28 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:bullseye` - linux; s390x

```console
$ docker pull memcached@sha256:4f7e9706bfd16d98bfb48a6435c8359a167ab733777f16f24996cad3f431bdc5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.2 MB (31211398 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6739ca31062c74398fdfec102afbacead1c25fa0decf2fa14bdecdcb6b160543`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 02 Aug 2022 00:42:27 GMT
ADD file:c2afc8990930846fbe7c99bfdfe9ea562c75feb6e3c9122431f7c9f8b5e51a7f in / 
# Tue, 02 Aug 2022 00:42:29 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 02:37:02 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 02 Aug 2022 02:37:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 04 Aug 2022 20:28:18 GMT
ENV MEMCACHED_VERSION=1.6.16
# Thu, 04 Aug 2022 20:28:18 GMT
ENV MEMCACHED_SHA1=724f31c3462fb6b07264d72d0043fd65545fd84a
# Thu, 04 Aug 2022 20:31:37 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 04 Aug 2022 20:31:37 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 04 Aug 2022 20:31:37 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 04 Aug 2022 20:31:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 04 Aug 2022 20:31:38 GMT
USER memcache
# Thu, 04 Aug 2022 20:31:38 GMT
EXPOSE 11211
# Thu, 04 Aug 2022 20:31:38 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:026d311d0716db60eba0572ea784c21031f420960510cebcc383dc53949b4db8`  
		Last Modified: Tue, 02 Aug 2022 00:48:01 GMT  
		Size: 29.6 MB (29640259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0ffdb328e548bd6b6311c78665ac8cd3be8f0b2e09691701d9b0bae0924f8f5`  
		Last Modified: Tue, 02 Aug 2022 02:41:16 GMT  
		Size: 5.0 KB (5025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fbb9677007b0ebab2fe6feab520da1962d3fcffb3490aa844681a46fcb35749`  
		Last Modified: Tue, 02 Aug 2022 02:41:16 GMT  
		Size: 324.2 KB (324183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9c93abfa1f832f2e1f02fbe7b9a489735142c2051dafa7af20d985ff2e2106b`  
		Last Modified: Thu, 04 Aug 2022 20:36:17 GMT  
		Size: 1.2 MB (1241523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f78bf4cf172bedc6ad3c92b859859b10c0394104262328d5664ddc0b1488b29`  
		Last Modified: Thu, 04 Aug 2022 20:36:17 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6a26d2d4c34166613098e1380842f1355b534e2335a1dea2128c193b7f19bec`  
		Last Modified: Thu, 04 Aug 2022 20:36:16 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:latest`

```console
$ docker pull memcached@sha256:0afaa8e890393e089efc991b62ec98d3dd53e5da995abfa548e5df9c70722015
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
$ docker pull memcached@sha256:d6479777ae4663bb6752d9e779a2180adeae2e6f91da834a6c042665ef961b19
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.0 MB (32956000 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:36a225838cd6927616fc3c9afc4fc26e1fbe4097250b113b6b8508e02ae6a589`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 02 Aug 2022 01:20:04 GMT
ADD file:0eae0dca665c7044bf242cb1fc92cb8ea744f5af2dd376a558c90bc47349aefe in / 
# Tue, 02 Aug 2022 01:20:05 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 04:45:12 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 02 Aug 2022 04:45:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 04 Aug 2022 19:59:25 GMT
ENV MEMCACHED_VERSION=1.6.16
# Thu, 04 Aug 2022 19:59:25 GMT
ENV MEMCACHED_SHA1=724f31c3462fb6b07264d72d0043fd65545fd84a
# Thu, 04 Aug 2022 20:02:08 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 04 Aug 2022 20:02:08 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 04 Aug 2022 20:02:08 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 04 Aug 2022 20:02:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 04 Aug 2022 20:02:09 GMT
USER memcache
# Thu, 04 Aug 2022 20:02:09 GMT
EXPOSE 11211
# Thu, 04 Aug 2022 20:02:09 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:1efc276f4ff952c055dea726cfc96ec6a4fdb8b62d9eed816bd2b788f2860ad7`  
		Last Modified: Tue, 02 Aug 2022 01:24:13 GMT  
		Size: 31.4 MB (31366757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60bd6790acf68c1ccc4757e879b51b4dbc273681e1f30606a2ccd4b55623d288`  
		Last Modified: Tue, 02 Aug 2022 04:48:24 GMT  
		Size: 5.0 KB (4980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e72821989d416909e21411733d7d034cfa908016dceb0b6e2717a5fb9faa617`  
		Last Modified: Tue, 02 Aug 2022 04:48:24 GMT  
		Size: 328.1 KB (328097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a972a764145eff4153208b9f8bed20e2179ececcec6e6d462d74400d526ccb4c`  
		Last Modified: Thu, 04 Aug 2022 20:05:45 GMT  
		Size: 1.3 MB (1255762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc9c8a212883923ae20b3e2d671f8dcc32307603465cf915c7e83bd5ac522c69`  
		Last Modified: Thu, 04 Aug 2022 20:05:45 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:157eedd0af5feece73dbebf45897c44894a10678feca71d5d57ac4904492badc`  
		Last Modified: Thu, 04 Aug 2022 20:05:46 GMT  
		Size: 118.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:latest` - linux; arm variant v5

```console
$ docker pull memcached@sha256:39515e68cebee2b2b88891c2b46b1c517587063301f77bbf7c312f6f9b372d65
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.5 MB (30454297 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8bf4bc30f264f1f9a0ede671e3a081ea54d1b6c3127ad5d9d4df3de21a985f5a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 02 Aug 2022 00:49:10 GMT
ADD file:4cd2f95737fd3007912428eeac56036c9e67e989e66cec08a8be99da47f88494 in / 
# Tue, 02 Aug 2022 00:49:10 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 01:58:42 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 02 Aug 2022 01:58:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 04 Aug 2022 19:50:51 GMT
ENV MEMCACHED_VERSION=1.6.16
# Thu, 04 Aug 2022 19:50:51 GMT
ENV MEMCACHED_SHA1=724f31c3462fb6b07264d72d0043fd65545fd84a
# Thu, 04 Aug 2022 19:56:43 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 04 Aug 2022 19:56:44 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 04 Aug 2022 19:56:44 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 04 Aug 2022 19:56:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 04 Aug 2022 19:56:44 GMT
USER memcache
# Thu, 04 Aug 2022 19:56:44 GMT
EXPOSE 11211
# Thu, 04 Aug 2022 19:56:45 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:5890b0ca6af5e8467a488e68716691950496a8f247d0495c2d595ddcb1893aff`  
		Last Modified: Tue, 02 Aug 2022 00:56:06 GMT  
		Size: 28.9 MB (28905515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e34350eb48491f2ab07c0f07724d37412df97ee9093c7c2458c9917afe37a42d`  
		Last Modified: Tue, 02 Aug 2022 02:04:59 GMT  
		Size: 4.9 KB (4894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36ecb6d2f4e3224a48197a5aa9d40970083bf4a92f41fbb493ac5adf9441a4ad`  
		Last Modified: Tue, 02 Aug 2022 02:04:59 GMT  
		Size: 316.6 KB (316628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e691cd60b95cdbb7fe7d3d74b1af54a56f440ac30d1dee94df4c4c370610b68d`  
		Last Modified: Thu, 04 Aug 2022 19:57:24 GMT  
		Size: 1.2 MB (1226852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8da76a828532ea569bd0e56b5a07a5e8bff4fe6efe22a5940260a261d113dc05`  
		Last Modified: Thu, 04 Aug 2022 19:57:23 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1705baeac52cb73666f9792b18547ce08509addd9ff3f19f6b91d21d5d10c8aa`  
		Last Modified: Thu, 04 Aug 2022 19:57:23 GMT  
		Size: 120.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:latest` - linux; arm variant v7

```console
$ docker pull memcached@sha256:25e768546f1e321b2a9031611f8ecd4081990c82f8774f7e051a5480cf18445d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.1 MB (28076294 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5959e4e12e1b75611311d3866bc95f9fe30048418f972e70fa2c671a66149fdd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 02 Aug 2022 00:58:59 GMT
ADD file:1575b776a15adacebc0875642e97a80807d42dcfc8917e1406d47af7ac244c97 in / 
# Tue, 02 Aug 2022 00:58:59 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 06:28:56 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 02 Aug 2022 06:29:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 04 Aug 2022 21:30:08 GMT
ENV MEMCACHED_VERSION=1.6.16
# Thu, 04 Aug 2022 21:30:08 GMT
ENV MEMCACHED_SHA1=724f31c3462fb6b07264d72d0043fd65545fd84a
# Thu, 04 Aug 2022 21:36:35 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 04 Aug 2022 21:36:35 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 04 Aug 2022 21:36:36 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 04 Aug 2022 21:36:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 04 Aug 2022 21:36:37 GMT
USER memcache
# Thu, 04 Aug 2022 21:36:37 GMT
EXPOSE 11211
# Thu, 04 Aug 2022 21:36:37 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:1dd75a3a9c893a7dc313f683dd62464b7eab6c6d522ee62c8a17022631830f32`  
		Last Modified: Tue, 02 Aug 2022 01:06:45 GMT  
		Size: 26.6 MB (26560586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44a675a8ce135f198539dc76b078733393238f7c7b899c8635980eed8f35f1cc`  
		Last Modified: Tue, 02 Aug 2022 09:35:13 GMT  
		Size: 4.9 KB (4890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:497b0afd04c92a1e5d41f58dbc0d5d544b8880d000c0ffbd03adb48c32c0116b`  
		Last Modified: Tue, 02 Aug 2022 09:35:13 GMT  
		Size: 312.1 KB (312067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8874fe992be272d0e0780725714c2439507699c15bfad1a073df948a34eb668d`  
		Last Modified: Fri, 05 Aug 2022 00:37:30 GMT  
		Size: 1.2 MB (1198344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cd5e042b98c640c152a56816e122c5e7b0abe91535d5d891dceed9748e42129`  
		Last Modified: Fri, 05 Aug 2022 00:37:29 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e871a0f93bdc7cb723e47f45514f914186b73d1890a53cdfe8525dd034926d59`  
		Last Modified: Fri, 05 Aug 2022 00:37:29 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:latest` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:759082b00d406f92781542ce86756eb73c5efe20acc7df6c25ac86be320a3ef5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.4 MB (31433439 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e91fe6663d9d90deed07c1d003a80fa6698137267c83310828f24a7ef63f6ef`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 02 Aug 2022 00:40:38 GMT
ADD file:6039adfbca55ed34a719c37672c664e3524130a0e2a3b8663629b8120b81b790 in / 
# Tue, 02 Aug 2022 00:40:39 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 03:56:15 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 02 Aug 2022 03:56:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 04 Aug 2022 20:33:46 GMT
ENV MEMCACHED_VERSION=1.6.16
# Thu, 04 Aug 2022 20:33:47 GMT
ENV MEMCACHED_SHA1=724f31c3462fb6b07264d72d0043fd65545fd84a
# Thu, 04 Aug 2022 20:36:17 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 04 Aug 2022 20:36:19 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 04 Aug 2022 20:36:19 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 04 Aug 2022 20:36:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 04 Aug 2022 20:36:21 GMT
USER memcache
# Thu, 04 Aug 2022 20:36:22 GMT
EXPOSE 11211
# Thu, 04 Aug 2022 20:36:23 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:a9fe95647e78b5516c7e2327355b6996e2ea295cd76ae242cbfe87f016b4e760`  
		Last Modified: Tue, 02 Aug 2022 00:46:05 GMT  
		Size: 30.1 MB (30054304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b983df009e7dc88033f53f015c09c56fd4db032d1abcade3333d8d4b515ff4af`  
		Last Modified: Tue, 02 Aug 2022 03:59:48 GMT  
		Size: 4.9 KB (4902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60720019405b50af041f391ec7dad90893ee95fc63fd6b3fb9da04850936f5db`  
		Last Modified: Tue, 02 Aug 2022 03:59:48 GMT  
		Size: 119.2 KB (119225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70569bedb4ee539337d6d3fd88e4076a1464b3a77bcfcca6604e18b815dbc402`  
		Last Modified: Thu, 04 Aug 2022 20:40:00 GMT  
		Size: 1.3 MB (1254600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:565112c01ad7b82688180f4fe70f5433126d79cc4b74e3d7f308601e2d34d9fe`  
		Last Modified: Thu, 04 Aug 2022 20:39:59 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce11290eb88924797c1fa048bd052c1243e4cb47e3469b26f3f1a3bc26472d19`  
		Last Modified: Thu, 04 Aug 2022 20:39:59 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:latest` - linux; 386

```console
$ docker pull memcached@sha256:deec44ba81c574f36b5b53185684413e4e97c3374d256e762ccf0e50fa1ff0f0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.8 MB (33762417 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9640d046f98daa1268a24f35ea7de08f83c728d88f2483d734101b09bad34768`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 02 Aug 2022 00:39:20 GMT
ADD file:f771e2286465694126158821089d801c7296376be2a56189e6041a15d2fe79f5 in / 
# Tue, 02 Aug 2022 00:39:21 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 03:12:03 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 02 Aug 2022 03:12:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 04 Aug 2022 20:28:41 GMT
ENV MEMCACHED_VERSION=1.6.16
# Thu, 04 Aug 2022 20:28:42 GMT
ENV MEMCACHED_SHA1=724f31c3462fb6b07264d72d0043fd65545fd84a
# Thu, 04 Aug 2022 20:31:30 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 04 Aug 2022 20:31:32 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 04 Aug 2022 20:31:32 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 04 Aug 2022 20:31:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 04 Aug 2022 20:31:34 GMT
USER memcache
# Thu, 04 Aug 2022 20:31:35 GMT
EXPOSE 11211
# Thu, 04 Aug 2022 20:31:36 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:90eb7f0ce9f33cf5dcd67d54c2fa606186dbaa5f95b6046f36145097267f9e53`  
		Last Modified: Tue, 02 Aug 2022 00:45:14 GMT  
		Size: 32.4 MB (32374054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:107cdc14debc414f1e6554b58402d2be697942f8f22b45d5c9b6bff8be3f332a`  
		Last Modified: Tue, 02 Aug 2022 03:15:55 GMT  
		Size: 4.8 KB (4771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b33bafb66f7f078457cf82ba6cfcbab5feae0e38bc0d959a5b50fa98fbcbf4ac`  
		Last Modified: Tue, 02 Aug 2022 03:15:55 GMT  
		Size: 130.1 KB (130114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c122afb77220a37620d69b968b43d326ed98ef7d9ed80ea06c3a7fa1c54dc73f`  
		Last Modified: Thu, 04 Aug 2022 20:35:38 GMT  
		Size: 1.3 MB (1253069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2426ab0684229e93e257d5c6357fbad018ee92d3cdcf5a7812171aa06bf82ca9`  
		Last Modified: Thu, 04 Aug 2022 20:35:38 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:240ed953e9e062d3ea6893fe34ecd1e5e060a240ae2a66092c6970c0be0eeed5`  
		Last Modified: Thu, 04 Aug 2022 20:35:38 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:latest` - linux; mips64le

```console
$ docker pull memcached@sha256:0d6798ccd4a9ac44c6ca7c358b2de6bdedbfe104de7d9987eedc68864ab8acc0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.0 MB (31002934 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aca3e1ecca25fb97ad1d376d73b212cad11874d1f051c4c4bac1b2d27abc15fd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 02 Aug 2022 01:10:34 GMT
ADD file:6dc22a1e5b5fcf23f2549406ddcc45c4e244f46e21eafa881de81fa87438e5d8 in / 
# Tue, 02 Aug 2022 01:10:38 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 03:22:53 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 02 Aug 2022 03:23:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 04 Aug 2022 20:07:25 GMT
ENV MEMCACHED_VERSION=1.6.16
# Thu, 04 Aug 2022 20:07:28 GMT
ENV MEMCACHED_SHA1=724f31c3462fb6b07264d72d0043fd65545fd84a
# Thu, 04 Aug 2022 20:14:28 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 04 Aug 2022 20:14:30 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 04 Aug 2022 20:14:35 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 04 Aug 2022 20:14:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 04 Aug 2022 20:14:40 GMT
USER memcache
# Thu, 04 Aug 2022 20:14:42 GMT
EXPOSE 11211
# Thu, 04 Aug 2022 20:14:45 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:88350749a27614c791450c256b051f023d81cdd256211274b1efac493779d2be`  
		Last Modified: Tue, 02 Aug 2022 01:21:02 GMT  
		Size: 29.6 MB (29628964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:117af7bbaadea9c81bbaa3a8a77b1ab5cd05bcac856c462cda2e81c9a40596ab`  
		Last Modified: Tue, 02 Aug 2022 03:30:45 GMT  
		Size: 4.9 KB (4863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53a16d313748bd6b2dade87de73d79edd8a08e4cb662769a717f8587abc8d5e0`  
		Last Modified: Tue, 02 Aug 2022 03:30:46 GMT  
		Size: 117.1 KB (117127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d524786af3243ee367d118f6d5260cffa06d800f492f9b4bb36c910958186933`  
		Last Modified: Thu, 04 Aug 2022 20:15:05 GMT  
		Size: 1.3 MB (1251571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4badb1f1970762d08dbd43d7e101081a5fabd3c45e18afd70636397e83102d2f`  
		Last Modified: Thu, 04 Aug 2022 20:15:04 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3102636392803c3bbff48f39e7f143e3bf9a0528365d63b90dc31cd32060d3e0`  
		Last Modified: Thu, 04 Aug 2022 20:15:04 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:latest` - linux; ppc64le

```console
$ docker pull memcached@sha256:fef67c5248379f0c7154c6298ae0236afa239c6a2e7677ff26cf67e2e902873c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.0 MB (36957550 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19ebbfa2abfbf5d8014f1a3d04cab132b47836a64e68160efb3b8c752addaedd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 02 Aug 2022 01:17:30 GMT
ADD file:3a95a896d463569ce82199957052b3467123a4bd3385a0a4e397cf08402a99c3 in / 
# Tue, 02 Aug 2022 01:17:32 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 03:45:30 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 02 Aug 2022 03:45:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 04 Aug 2022 20:31:03 GMT
ENV MEMCACHED_VERSION=1.6.16
# Thu, 04 Aug 2022 20:31:04 GMT
ENV MEMCACHED_SHA1=724f31c3462fb6b07264d72d0043fd65545fd84a
# Thu, 04 Aug 2022 20:34:08 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 04 Aug 2022 20:34:09 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 04 Aug 2022 20:34:10 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 04 Aug 2022 20:34:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 04 Aug 2022 20:34:10 GMT
USER memcache
# Thu, 04 Aug 2022 20:34:11 GMT
EXPOSE 11211
# Thu, 04 Aug 2022 20:34:11 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:5241cd116d6e6e2d62f3d8c2245b74daca9f6cc154eaccd738feb41984c74714`  
		Last Modified: Tue, 02 Aug 2022 01:24:39 GMT  
		Size: 35.3 MB (35272771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58860b5324185f5059438d063f2a2b9c8ec05e058d0c1467db47a258a089c691`  
		Last Modified: Tue, 02 Aug 2022 03:53:12 GMT  
		Size: 5.0 KB (4978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82fb13381eff7e0b9526ba592f13e09cea5295914fde283ea341e5b71cb31493`  
		Last Modified: Tue, 02 Aug 2022 03:53:13 GMT  
		Size: 356.9 KB (356918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b33f6ac4fcd819056777e9462124dfc34dca6f35e1cae56a64d12bd150e4dfc9`  
		Last Modified: Thu, 04 Aug 2022 20:38:29 GMT  
		Size: 1.3 MB (1322475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:893b74576495c7a62c5d4447a7453f60f228fbb0e6d2dc4edf7e67661c455f57`  
		Last Modified: Thu, 04 Aug 2022 20:38:28 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7855d0c39dc9730d8ec3369fa86f770bd433a903eb346e9115b7442574441f24`  
		Last Modified: Thu, 04 Aug 2022 20:38:28 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:latest` - linux; s390x

```console
$ docker pull memcached@sha256:4f7e9706bfd16d98bfb48a6435c8359a167ab733777f16f24996cad3f431bdc5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.2 MB (31211398 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6739ca31062c74398fdfec102afbacead1c25fa0decf2fa14bdecdcb6b160543`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 02 Aug 2022 00:42:27 GMT
ADD file:c2afc8990930846fbe7c99bfdfe9ea562c75feb6e3c9122431f7c9f8b5e51a7f in / 
# Tue, 02 Aug 2022 00:42:29 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 02:37:02 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 02 Aug 2022 02:37:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 04 Aug 2022 20:28:18 GMT
ENV MEMCACHED_VERSION=1.6.16
# Thu, 04 Aug 2022 20:28:18 GMT
ENV MEMCACHED_SHA1=724f31c3462fb6b07264d72d0043fd65545fd84a
# Thu, 04 Aug 2022 20:31:37 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 04 Aug 2022 20:31:37 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 04 Aug 2022 20:31:37 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 04 Aug 2022 20:31:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 04 Aug 2022 20:31:38 GMT
USER memcache
# Thu, 04 Aug 2022 20:31:38 GMT
EXPOSE 11211
# Thu, 04 Aug 2022 20:31:38 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:026d311d0716db60eba0572ea784c21031f420960510cebcc383dc53949b4db8`  
		Last Modified: Tue, 02 Aug 2022 00:48:01 GMT  
		Size: 29.6 MB (29640259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0ffdb328e548bd6b6311c78665ac8cd3be8f0b2e09691701d9b0bae0924f8f5`  
		Last Modified: Tue, 02 Aug 2022 02:41:16 GMT  
		Size: 5.0 KB (5025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fbb9677007b0ebab2fe6feab520da1962d3fcffb3490aa844681a46fcb35749`  
		Last Modified: Tue, 02 Aug 2022 02:41:16 GMT  
		Size: 324.2 KB (324183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9c93abfa1f832f2e1f02fbe7b9a489735142c2051dafa7af20d985ff2e2106b`  
		Last Modified: Thu, 04 Aug 2022 20:36:17 GMT  
		Size: 1.2 MB (1241523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f78bf4cf172bedc6ad3c92b859859b10c0394104262328d5664ddc0b1488b29`  
		Last Modified: Thu, 04 Aug 2022 20:36:17 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6a26d2d4c34166613098e1380842f1355b534e2335a1dea2128c193b7f19bec`  
		Last Modified: Thu, 04 Aug 2022 20:36:16 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
