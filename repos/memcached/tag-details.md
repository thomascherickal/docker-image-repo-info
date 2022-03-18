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
-	[`memcached:1.6.14`](#memcached1614)
-	[`memcached:1.6.14-alpine`](#memcached1614-alpine)
-	[`memcached:1.6.14-alpine3.15`](#memcached1614-alpine315)
-	[`memcached:1.6.14-bullseye`](#memcached1614-bullseye)
-	[`memcached:alpine`](#memcachedalpine)
-	[`memcached:alpine3.15`](#memcachedalpine315)
-	[`memcached:bullseye`](#memcachedbullseye)
-	[`memcached:latest`](#memcachedlatest)

## `memcached:1`

```console
$ docker pull memcached@sha256:67ceec1841427583fd33842be1a41243351997c4803d05c14f95f0c8c6826f93
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
$ docker pull memcached@sha256:6a51dd2e23a3ead43158d3255ab8c2d9b0b2f0432becf5814c267273c84e8b6a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.0 MB (32965129 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e897df046b27f4dbfae44d31346ef91c2160a46c1b8d5bf652a40e3d76d3914f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 17 Mar 2022 04:03:59 GMT
ADD file:36919ae6bb25e3269eff949443129a01a8a43fb967fe6563939ebe1e1e9b8228 in / 
# Thu, 17 Mar 2022 04:03:59 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 12:47:26 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Thu, 17 Mar 2022 12:47:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Mar 2022 12:47:29 GMT
ENV MEMCACHED_VERSION=1.6.14
# Thu, 17 Mar 2022 12:47:29 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Thu, 17 Mar 2022 12:51:18 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 17 Mar 2022 12:51:18 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 17 Mar 2022 12:51:18 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 17 Mar 2022 12:51:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Mar 2022 12:51:18 GMT
USER memcache
# Thu, 17 Mar 2022 12:51:19 GMT
EXPOSE 11211
# Thu, 17 Mar 2022 12:51:19 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:ae13dd57832654086618a81dbc128846aa092489260c326ee95429b63c3cf213`  
		Last Modified: Thu, 17 Mar 2022 04:10:05 GMT  
		Size: 31.4 MB (31376572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c39e8a8db385456589d2009379dedc9787a9297b0ea679ff564500de9894d325`  
		Last Modified: Thu, 17 Mar 2022 12:55:59 GMT  
		Size: 5.0 KB (4982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fa3e9def276e8e73128ec9d08c6f139621666d0724b33d882ca0943a1a6825b`  
		Last Modified: Thu, 17 Mar 2022 12:55:59 GMT  
		Size: 328.0 KB (328046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9835681ca994d84f0de3da2d9ed0cdb5882c06b58bccdc406102bf4bf8a55700`  
		Last Modified: Thu, 17 Mar 2022 12:55:59 GMT  
		Size: 1.3 MB (1255121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d362d7003189fa875ec372df3c4c9622f2688adb7ed5c9cb2bec35c31b9d523`  
		Last Modified: Thu, 17 Mar 2022 12:55:59 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bd4550226c671e2d98eac87073171c925eebaa0e039ed5e2610d516980dd220`  
		Last Modified: Thu, 17 Mar 2022 12:55:59 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1` - linux; arm variant v5

```console
$ docker pull memcached@sha256:084a4198172362acf346afa27655123636800a135bdaaa857d8d57e7e402c4fa
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.5 MB (30467908 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b9e543544c3f8ef04ec918e92a8e98602cbdc37970011b5960685ffd0103780`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 17 Mar 2022 05:19:45 GMT
ADD file:1eb4f937d40230354e20e28ed781234acd4be2b0dab72f87131a3eac66349719 in / 
# Thu, 17 Mar 2022 05:19:46 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 10:06:48 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Thu, 17 Mar 2022 10:06:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Mar 2022 10:07:00 GMT
ENV MEMCACHED_VERSION=1.6.14
# Thu, 17 Mar 2022 10:07:00 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Thu, 17 Mar 2022 10:11:18 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 17 Mar 2022 10:11:18 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 17 Mar 2022 10:11:20 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 17 Mar 2022 10:11:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Mar 2022 10:11:21 GMT
USER memcache
# Thu, 17 Mar 2022 10:11:21 GMT
EXPOSE 11211
# Thu, 17 Mar 2022 10:11:21 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:4da455e7774c0e977d862a56ab6d85f33ce5dd5a77d45a0a74a272e9eae6bea0`  
		Last Modified: Thu, 17 Mar 2022 05:35:01 GMT  
		Size: 28.9 MB (28919702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39450ea3e36758cb1aaf29a3e4a3694a4f1e5d208ece3da6479b6dcd47705309`  
		Last Modified: Thu, 17 Mar 2022 10:12:14 GMT  
		Size: 4.9 KB (4890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b674f1fc0977777c240d7af9fa6d57e8b24d5332791547c80820aa9d1956d037`  
		Last Modified: Thu, 17 Mar 2022 10:12:14 GMT  
		Size: 316.6 KB (316575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de44c6f01b62d4d56baa2601e6706305eaf35c2da9541623a8c94c7fe1e4b8b2`  
		Last Modified: Thu, 17 Mar 2022 10:12:14 GMT  
		Size: 1.2 MB (1226335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18229473d3cfa938b3ba5d7f36b228bc60b7641660ae3242b56e210a50892b0f`  
		Last Modified: Thu, 17 Mar 2022 10:12:14 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e231e6a0756abb2590d1ef0507c610f0aa1b4f42e40a895d310b330662a98a2`  
		Last Modified: Thu, 17 Mar 2022 10:12:14 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1` - linux; arm variant v7

```console
$ docker pull memcached@sha256:9fe6c86dfef8c0cf535d443045364d887fd0bc8b44f550a8cbb0dca64e33e732
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.1 MB (28090226 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14dc9d69afed7832780e59eca9bf08aecbca59e357a3c301648a665b42b6659a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 17 Mar 2022 09:31:03 GMT
ADD file:e52f9ee2dc3144d7b9eb3ec90c106aa2a094eb4c5c2aa8cbff5c520a5faaef43 in / 
# Thu, 17 Mar 2022 09:31:04 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 21:53:04 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Thu, 17 Mar 2022 21:53:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Mar 2022 21:53:14 GMT
ENV MEMCACHED_VERSION=1.6.14
# Thu, 17 Mar 2022 21:53:14 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Thu, 17 Mar 2022 21:57:21 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 17 Mar 2022 21:57:22 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 17 Mar 2022 21:57:23 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 17 Mar 2022 21:57:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Mar 2022 21:57:24 GMT
USER memcache
# Thu, 17 Mar 2022 21:57:25 GMT
EXPOSE 11211
# Thu, 17 Mar 2022 21:57:25 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:5e5e708ee1f9fdbc69324391f7d1f816c657e6116eff09e7d2247fa9de3a076a`  
		Last Modified: Thu, 17 Mar 2022 09:46:33 GMT  
		Size: 26.6 MB (26575097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f652a8bcf3f50c242f3e27b3792cd55f9c0436702fe2bcdd4ae3df203aa84100`  
		Last Modified: Thu, 17 Mar 2022 22:10:19 GMT  
		Size: 4.9 KB (4896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c1be80f12d4f19157864e18689a8dd9c0f84c3a6c929949b066e7c29f30c5d7`  
		Last Modified: Thu, 17 Mar 2022 22:10:19 GMT  
		Size: 312.0 KB (311999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37ab28ddd02c6ca7832dec8a6b6508e8e4d95b34c8f4fe17457a1844c4442a7a`  
		Last Modified: Thu, 17 Mar 2022 22:10:19 GMT  
		Size: 1.2 MB (1197826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6d7e30c2d27f64a3117e85e87c00c1d4e79aa91e0bf4e4552c68d4710592d64`  
		Last Modified: Thu, 17 Mar 2022 22:10:19 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7f72f97159e0cf88a536b1a268d9bfa7af992046ce641dddb6710eabf7d08e4`  
		Last Modified: Thu, 17 Mar 2022 22:10:19 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:773c0f8c11aa82d0bf14e751ab65784b8993bd7477026d660eb8e970b160aad8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.4 MB (31441503 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1cc644adcd708fa1761227654eacbdd25163b6a5a399599e20c7eabdc2a24a8f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 17 Mar 2022 03:21:57 GMT
ADD file:e52e032f1ace6abd44b3647d43c1b8ae30bac6de804eef09c6ccd793057996fd in / 
# Thu, 17 Mar 2022 03:21:58 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 11:35:48 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Thu, 17 Mar 2022 11:35:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Mar 2022 11:35:52 GMT
ENV MEMCACHED_VERSION=1.6.14
# Thu, 17 Mar 2022 11:35:53 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Thu, 17 Mar 2022 11:38:38 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 17 Mar 2022 11:38:40 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 17 Mar 2022 11:38:40 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 17 Mar 2022 11:38:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Mar 2022 11:38:42 GMT
USER memcache
# Thu, 17 Mar 2022 11:38:43 GMT
EXPOSE 11211
# Thu, 17 Mar 2022 11:38:44 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:32252aec0777ac025a158bc2a8317650a4f2a0a875387011b1165013874f8723`  
		Last Modified: Thu, 17 Mar 2022 03:28:36 GMT  
		Size: 30.1 MB (30063013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:966f1b38b9d3f62f875f8dbd868ecc80c2037b45aadbec50fc16d292be747303`  
		Last Modified: Thu, 17 Mar 2022 11:42:26 GMT  
		Size: 4.9 KB (4903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2898c9abf66c159176811eff24e689c0989d4e7c025c9a7eb0f933d356aec11`  
		Last Modified: Thu, 17 Mar 2022 11:42:26 GMT  
		Size: 119.2 KB (119181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d331819fcfc0b6541dc90aafde95bc8b8a88e453cb3800c977716cff65961a77`  
		Last Modified: Thu, 17 Mar 2022 11:42:26 GMT  
		Size: 1.3 MB (1254002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25a25819b974fbc38bad380c4df00bf1f032cf4eb0112a109c78f9858d9a0a55`  
		Last Modified: Thu, 17 Mar 2022 11:42:26 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7c790b93b28eb9ed542eac0eaf8c5fe2d4c5daa368b0f27bac067fd01bee280`  
		Last Modified: Thu, 17 Mar 2022 11:42:26 GMT  
		Size: 118.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1` - linux; 386

```console
$ docker pull memcached@sha256:3d0458851092782bb1cfb8fdb3edb27fe63775c3fb68f1879137e691de184e82
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.0 MB (33981668 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b7d3a232500fae88433d6e4117fa6e45b0ed4c529c925734eb2982bf3a3ee54`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 17 Mar 2022 08:15:53 GMT
ADD file:2d6be3846f0e5fabd85bc9409b1e2223cad4c57c76f96e9f81489ba78a72a1f5 in / 
# Thu, 17 Mar 2022 08:15:54 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 17:31:22 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Thu, 17 Mar 2022 17:31:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Mar 2022 17:31:26 GMT
ENV MEMCACHED_VERSION=1.6.14
# Thu, 17 Mar 2022 17:31:26 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Thu, 17 Mar 2022 17:35:17 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 17 Mar 2022 17:35:17 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 17 Mar 2022 17:35:18 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 17 Mar 2022 17:35:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Mar 2022 17:35:18 GMT
USER memcache
# Thu, 17 Mar 2022 17:35:18 GMT
EXPOSE 11211
# Thu, 17 Mar 2022 17:35:18 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:176085117cac9b2cf2cf57b3a10c9811dbd2773497fbac3086b5024070447e97`  
		Last Modified: Thu, 17 Mar 2022 08:24:00 GMT  
		Size: 32.4 MB (32386475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe18ed3f6ff50e5b12a7db917c34de3104619ae31e84d9d83ad2d94a3b8c5822`  
		Last Modified: Thu, 17 Mar 2022 17:40:19 GMT  
		Size: 4.9 KB (4896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc15fd9e0c057bb0a0d077f6c21d0b980b6ec5f9e5292c19d6fd790731f7bfc6`  
		Last Modified: Thu, 17 Mar 2022 17:40:19 GMT  
		Size: 336.6 KB (336638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1f8475d0ca14b4624de06fbe3207cdf07b5c31573192d0acc9b1e600b90c430`  
		Last Modified: Thu, 17 Mar 2022 17:40:20 GMT  
		Size: 1.3 MB (1253253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61e85d2ca17a8c6eb12e9cdc031a20d5c2357cf22bc4ad5353d520e13f60b73a`  
		Last Modified: Thu, 17 Mar 2022 17:40:19 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3194d39d810076bc29397aa1a117ac51d7bc610ffb9b7c90613fdf21203b05a3`  
		Last Modified: Thu, 17 Mar 2022 17:40:19 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1` - linux; mips64le

```console
$ docker pull memcached@sha256:9148cd77f369a80c3b52dd4f79ddd8073c192da135e99a311f54641a851b4b60
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.0 MB (31012937 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:16b4bbcf6270bfbe61ccbb8083bf46151a57eb6a74f044b2004509978709ee0d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 17 Mar 2022 08:53:04 GMT
ADD file:795ac4eba576bc4c995df2a18b10ce802ee8a05417cdc53f5aa09452ecf2e832 in / 
# Thu, 17 Mar 2022 08:53:08 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 20:37:19 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Thu, 17 Mar 2022 20:37:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Mar 2022 20:37:40 GMT
ENV MEMCACHED_VERSION=1.6.14
# Thu, 17 Mar 2022 20:37:43 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Thu, 17 Mar 2022 20:44:58 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 17 Mar 2022 20:45:00 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 17 Mar 2022 20:45:05 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 17 Mar 2022 20:45:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Mar 2022 20:45:10 GMT
USER memcache
# Thu, 17 Mar 2022 20:45:13 GMT
EXPOSE 11211
# Thu, 17 Mar 2022 20:45:15 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:4799d88734ae94287a665c0e14621a744706cfbe17a0cf27ae9b0cc630927b11`  
		Last Modified: Thu, 17 Mar 2022 10:43:20 GMT  
		Size: 29.6 MB (29639810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a091b8fd61b3c0cafad5676908a202cec423a829bd2fb2bb79011b3ad5fd0845`  
		Last Modified: Thu, 17 Mar 2022 20:45:41 GMT  
		Size: 4.9 KB (4859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7644e6d2f727759be27279ab11b8f3e186b6918c1b3847badb0d04ae020286b`  
		Last Modified: Thu, 17 Mar 2022 20:45:41 GMT  
		Size: 117.1 KB (117098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47e8f3183abaf23ec67f322bc78981d3c838ad27bba488ec924c07d5b1a053a4`  
		Last Modified: Thu, 17 Mar 2022 20:45:41 GMT  
		Size: 1.3 MB (1250762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f0ac34ae7971e4442dd9abb2bbfa522fc4e65445f1ed51d33795cea9b37830e`  
		Last Modified: Thu, 17 Mar 2022 20:45:40 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0564ebbfe5b917d8a4818a435ddb35d5e4bbb4b4d7187189578f1c224d10ce2b`  
		Last Modified: Thu, 17 Mar 2022 20:45:40 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1` - linux; ppc64le

```console
$ docker pull memcached@sha256:4893f4daa742b31f414b08f98f8e7d0cbedaf63b8d88062bcf3c91a9522a2aab
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.0 MB (36957544 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8db953cc998ed06712eca57fe4ae2b8bb342ce991683fd7592495a21557d0940`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 26 Jan 2022 01:46:51 GMT
ADD file:c03f34c221e57fa5cb625c166d1db9f72d6ba2fa17a3c41a5d04d6875d098949 in / 
# Wed, 26 Jan 2022 01:46:57 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 05:38:39 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 26 Jan 2022 05:38:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 11 Feb 2022 23:47:36 GMT
ENV MEMCACHED_VERSION=1.6.14
# Fri, 11 Feb 2022 23:47:38 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Fri, 11 Feb 2022 23:53:07 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Fri, 11 Feb 2022 23:53:13 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 11 Feb 2022 23:53:34 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 11 Feb 2022 23:53:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Feb 2022 23:53:39 GMT
USER memcache
# Fri, 11 Feb 2022 23:53:41 GMT
EXPOSE 11211
# Fri, 11 Feb 2022 23:53:46 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:3149ee4a73508a4c39107d64a3fdc1b021626a22a0ac95e62fa0cea49ab77fba`  
		Last Modified: Wed, 26 Jan 2022 01:57:01 GMT  
		Size: 35.3 MB (35273030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07bcb451658eb6d9eace467c2e989d96e53c409eb48347a369e9ad80aadcfe96`  
		Last Modified: Wed, 26 Jan 2022 05:45:22 GMT  
		Size: 5.0 KB (4980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8807782e060aa90873de57b2d3ec277632145f166e9c1e3801c57eea7e595cc`  
		Last Modified: Wed, 26 Jan 2022 05:45:22 GMT  
		Size: 356.9 KB (356905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5f2e5d5bb1609e336a37e97218d618550ec5ce28384c32b1141393ef6f04a03`  
		Last Modified: Fri, 11 Feb 2022 23:58:44 GMT  
		Size: 1.3 MB (1322220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76e6da4f290b1cff2fa5b1ad17d42333c67179332511db4da3bd2c5ce12bbdfa`  
		Last Modified: Fri, 11 Feb 2022 23:58:44 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fb140c5468aa121999bc169d30e4ce6b73795cdf67aa21c1dfd3d1194dd0b82`  
		Last Modified: Fri, 11 Feb 2022 23:58:44 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1` - linux; s390x

```console
$ docker pull memcached@sha256:3e4437e519528ef8d3274dfc333f59f7c8c90099329a1e041fb6a71d5be8a1c5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.2 MB (31225911 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6fbcefffe918634bf299753ebcfe4a7284155e249686c5b5db9ffa92a5c0fc87`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 17 Mar 2022 03:06:58 GMT
ADD file:52f9267b4c57ac585a0d3d47a6f2ae1a71398264173ad4f190332957fa629c67 in / 
# Thu, 17 Mar 2022 03:07:01 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 08:47:34 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Thu, 17 Mar 2022 08:47:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Mar 2022 08:47:37 GMT
ENV MEMCACHED_VERSION=1.6.14
# Thu, 17 Mar 2022 08:47:37 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Thu, 17 Mar 2022 08:50:57 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 17 Mar 2022 08:50:57 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 17 Mar 2022 08:50:58 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 17 Mar 2022 08:50:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Mar 2022 08:50:58 GMT
USER memcache
# Thu, 17 Mar 2022 08:50:58 GMT
EXPOSE 11211
# Thu, 17 Mar 2022 08:50:59 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:d101968410e5005df630b0572aec03c88de55b8de81f3cf7e6a57e1ce2e5a8e5`  
		Last Modified: Thu, 17 Mar 2022 03:12:46 GMT  
		Size: 29.7 MB (29655795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1cad003ec39dc6e2e144c0953bad3bce3807fd1679d2c9e27e510724476e1e6`  
		Last Modified: Thu, 17 Mar 2022 08:55:34 GMT  
		Size: 5.0 KB (5022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13e61c306aebe51ff20adaf4ac683a69d93022d34ed4d09bc2ae7bde9d92ba52`  
		Last Modified: Thu, 17 Mar 2022 08:55:34 GMT  
		Size: 324.1 KB (324147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b5e88f796665ba79a22e6a541cbc3f30242e708c56d6b9af4fd0a7cd23abea6`  
		Last Modified: Thu, 17 Mar 2022 08:55:34 GMT  
		Size: 1.2 MB (1240539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77d35a1cb446cb01584cfbb3a61c40aaa1f358f37c8d723fe2437e6d070dbce3`  
		Last Modified: Thu, 17 Mar 2022 08:55:34 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b237b13dadf10fc593967f3714eaab56b7b00b89d435eb7e01be3f172b5b9b69`  
		Last Modified: Thu, 17 Mar 2022 08:55:33 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:1-alpine`

```console
$ docker pull memcached@sha256:f29cd53458fed5079ec81d66878db3f5ef40001b371b0437af6d5a660008f779
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
$ docker pull memcached@sha256:fd1bb2a04baff1bc63d2323d91a4f7135b9f06f1d0294fbe13b8660db7b6dd78
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3862528 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e9d7d65a6545e2698d88de0e6c6eeb620a5bdf19e35635a36ac252bb7dce9d55`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 17 Mar 2022 04:01:58 GMT
ADD file:cf4b631a115c2bbfbd81cad2d3041bceb64a8136aac92ba8a63b6c51d60af764 in / 
# Thu, 17 Mar 2022 04:01:59 GMT
CMD ["/bin/sh"]
# Thu, 17 Mar 2022 12:51:33 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Thu, 17 Mar 2022 12:51:34 GMT
RUN apk add --no-cache libsasl
# Thu, 17 Mar 2022 12:51:34 GMT
ENV MEMCACHED_VERSION=1.6.14
# Thu, 17 Mar 2022 12:51:35 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Thu, 17 Mar 2022 12:55:35 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Thu, 17 Mar 2022 12:55:35 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 17 Mar 2022 12:55:36 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 17 Mar 2022 12:55:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Mar 2022 12:55:36 GMT
USER memcache
# Thu, 17 Mar 2022 12:55:36 GMT
EXPOSE 11211
# Thu, 17 Mar 2022 12:55:36 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:3d243047344378e9b7136d552d48feb7ea8b6fe14ce0990e0cc011d5e369626a`  
		Last Modified: Thu, 17 Mar 2022 04:02:41 GMT  
		Size: 2.8 MB (2812636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e26b137db66bd985a8103e3e70f8985eafa9a9ca3dc6aa33344245535f6a6b0`  
		Last Modified: Thu, 17 Mar 2022 12:56:25 GMT  
		Size: 1.3 KB (1263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5231e0cae31bc5e59bdcb40f696ceaa6b5cad70b9500bc5bfd459174ac1f78dd`  
		Last Modified: Thu, 17 Mar 2022 12:56:25 GMT  
		Size: 109.3 KB (109285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d9fab8e58febfe6f0bfb8d5bdc098221b6348a6128014c4c2b4d4086284696d`  
		Last Modified: Thu, 17 Mar 2022 12:56:25 GMT  
		Size: 938.9 KB (938943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9ca16ee180425777e36c6f23ab6755a192eedf107400360aac9332686f1212b`  
		Last Modified: Thu, 17 Mar 2022 12:56:25 GMT  
		Size: 280.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f81d444d82a8e26057630fab59b6bdb890fe42afa50edabbba60d8685e88d639`  
		Last Modified: Thu, 17 Mar 2022 12:56:24 GMT  
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
$ docker pull memcached@sha256:095e0c44c122b636ae053f2971bb454b3edfe210195707983a9e0a38d22f4411
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3754561 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d01922b70bc4d8d1d2be9eabafa82a0f0152a88e5871b7e9b6949cf1327c9c4f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 17 Mar 2022 03:19:52 GMT
ADD file:cd7d91362950471ca4678cf3833dc47119ab519dea51424c847bbbb21e1649d4 in / 
# Thu, 17 Mar 2022 03:19:52 GMT
CMD ["/bin/sh"]
# Thu, 17 Mar 2022 11:39:00 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Thu, 17 Mar 2022 11:39:02 GMT
RUN apk add --no-cache libsasl
# Thu, 17 Mar 2022 11:39:03 GMT
ENV MEMCACHED_VERSION=1.6.14
# Thu, 17 Mar 2022 11:39:04 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Thu, 17 Mar 2022 11:41:43 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Thu, 17 Mar 2022 11:41:45 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 17 Mar 2022 11:41:45 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 17 Mar 2022 11:41:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Mar 2022 11:41:47 GMT
USER memcache
# Thu, 17 Mar 2022 11:41:48 GMT
EXPOSE 11211
# Thu, 17 Mar 2022 11:41:49 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:148d739a8e6b9342daa1f5b428d3a3c6118f340f21df28c16e06f918ef150147`  
		Last Modified: Thu, 17 Mar 2022 03:20:45 GMT  
		Size: 2.7 MB (2714807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33dde588ab12fbb6aa46070a960ac850c8347e86f29744b40a123a466d4885ab`  
		Last Modified: Thu, 17 Mar 2022 11:42:57 GMT  
		Size: 1.2 KB (1240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bdeb7ac9fd9c67010a55bf3fe0e13866bb31d847353f455c95220027e2bc48c`  
		Last Modified: Thu, 17 Mar 2022 11:42:58 GMT  
		Size: 110.6 KB (110556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6bf3828467e4d3c16fcdc94bf5987db023e892ef9594c9c5dc2c3ccf07bc4bc`  
		Last Modified: Thu, 17 Mar 2022 11:42:58 GMT  
		Size: 927.5 KB (927550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d39e5be11e10e43e4991c6d85f4bdce89416e75c908d33656e4dcb79c26a51bc`  
		Last Modified: Thu, 17 Mar 2022 11:42:57 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9404edf07c113d954a0a5c34650b52d9a1f8e57d166b3e1b022a82c3e27e724`  
		Last Modified: Thu, 17 Mar 2022 11:42:57 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-alpine` - linux; 386

```console
$ docker pull memcached@sha256:8a6352e717a8080f0c0888560cf7ae52c77ee2cbd10ed46c68822370b5188d0f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3891706 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4db903b8d549ba5f131fc35c81b69bdf1822950956033492f126e16dd95b5750`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 17 Mar 2022 08:13:03 GMT
ADD file:22216bc654d9177244235f242fa83cae3b283b3c145cad7ccf11c0d29f5f0ff2 in / 
# Thu, 17 Mar 2022 08:13:03 GMT
CMD ["/bin/sh"]
# Thu, 17 Mar 2022 17:35:31 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Thu, 17 Mar 2022 17:35:32 GMT
RUN apk add --no-cache libsasl
# Thu, 17 Mar 2022 17:35:32 GMT
ENV MEMCACHED_VERSION=1.6.14
# Thu, 17 Mar 2022 17:35:33 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Thu, 17 Mar 2022 17:39:25 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Thu, 17 Mar 2022 17:39:25 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 17 Mar 2022 17:39:26 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 17 Mar 2022 17:39:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Mar 2022 17:39:26 GMT
USER memcache
# Thu, 17 Mar 2022 17:39:26 GMT
EXPOSE 11211
# Thu, 17 Mar 2022 17:39:26 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:93317a1f65ec94b67aefe728a598022610246404e3a68d391c76cd0e5244a2a0`  
		Last Modified: Thu, 17 Mar 2022 08:13:56 GMT  
		Size: 2.8 MB (2821789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae4d8e906564040308eb9f4b96b3808d37aa02b7fffa8e8d5c80126d5e50b1cf`  
		Last Modified: Thu, 17 Mar 2022 17:40:52 GMT  
		Size: 1.3 KB (1263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16143ebb273f49cf3884d5a063dfac8b30d9527c5018e90fac51ac381b5a5f8b`  
		Last Modified: Thu, 17 Mar 2022 17:40:52 GMT  
		Size: 121.2 KB (121183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:107340d48cdbc30d4b57291ca0d28997feed13517f3a508b3b398620dbc97099`  
		Last Modified: Thu, 17 Mar 2022 17:40:52 GMT  
		Size: 947.1 KB (947068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a791ada3ee704cad0a4dba90d29f533e6fcadb132c2522c38b4f0680201a86a9`  
		Last Modified: Thu, 17 Mar 2022 17:40:52 GMT  
		Size: 282.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fc23e842aa74aed8a4ea48cf2b6f027f9592e43e117c394bc70b3d2dcf0627c`  
		Last Modified: Thu, 17 Mar 2022 17:40:53 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-alpine` - linux; ppc64le

```console
$ docker pull memcached@sha256:75cb5141098fb02bb0c554c31c00d28802b414593a6b41d430c10505ee943fe0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.3 MB (5315837 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4be74852968716dd05ad711f1cda531afac5b782fe0dd6692e5aed7d91d54466`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 24 Nov 2021 20:20:16 GMT
ADD file:57115dca2eb707f46b6301e75174e6aa316fb02ac28643b91429b75be51bd8c8 in / 
# Wed, 24 Nov 2021 20:20:20 GMT
CMD ["/bin/sh"]
# Tue, 30 Nov 2021 00:52:13 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 30 Nov 2021 00:52:18 GMT
RUN apk add --no-cache libsasl
# Fri, 11 Feb 2022 23:54:02 GMT
ENV MEMCACHED_VERSION=1.6.14
# Fri, 11 Feb 2022 23:54:06 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Fri, 11 Feb 2022 23:57:48 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Fri, 11 Feb 2022 23:57:50 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 11 Feb 2022 23:57:55 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 11 Feb 2022 23:57:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Feb 2022 23:57:59 GMT
USER memcache
# Fri, 11 Feb 2022 23:58:01 GMT
EXPOSE 11211
# Fri, 11 Feb 2022 23:58:02 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:159b5dcb1717c815c76ff5ea1db730e18e8609c9090238e43282856db9e71f47`  
		Last Modified: Wed, 24 Nov 2021 20:21:14 GMT  
		Size: 2.8 MB (2814780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f44bb0dc5dc6d3634512266fffaecf643a467ef890e0a60fa7daed8a8f379335`  
		Last Modified: Tue, 30 Nov 2021 00:57:03 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:242bba95e896195e2c48210499ed8dad5c07a25a93e0d6304a787f4d5f05bb79`  
		Last Modified: Tue, 30 Nov 2021 00:57:03 GMT  
		Size: 126.2 KB (126210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9d933f0d59015113f25123de9b3460a03fdf091181f4c9330b1bb42c27a8cce`  
		Last Modified: Fri, 11 Feb 2022 23:59:16 GMT  
		Size: 2.4 MB (2373175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:659fd1f60c2bc05966f606e677370eeee3176f7d6dbd530b3f271ba313f8b0fe`  
		Last Modified: Fri, 11 Feb 2022 23:59:15 GMT  
		Size: 282.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8d9d86e7310ff252ce602224ce1643c6b8d50713444e43804cdb93912f89087`  
		Last Modified: Fri, 11 Feb 2022 23:59:15 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-alpine` - linux; s390x

```console
$ docker pull memcached@sha256:5a931719c887b04ccf389c14867075cca4a76c774ecceb8231f801d876c94be9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.7 MB (3651372 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8aed3255f32676856491e1f6e999893205a57c1d26f36d52518c7d72433bcd9c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 17 Mar 2022 03:04:28 GMT
ADD file:f623c69acb1859b41ef29e8f20f4e6c7072d9c6d7210d745afc615251bfe418f in / 
# Thu, 17 Mar 2022 03:04:28 GMT
CMD ["/bin/sh"]
# Thu, 17 Mar 2022 08:51:10 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Thu, 17 Mar 2022 08:51:11 GMT
RUN apk add --no-cache libsasl
# Thu, 17 Mar 2022 08:51:12 GMT
ENV MEMCACHED_VERSION=1.6.14
# Thu, 17 Mar 2022 08:51:12 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Thu, 17 Mar 2022 08:54:42 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Thu, 17 Mar 2022 08:54:42 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 17 Mar 2022 08:54:43 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 17 Mar 2022 08:54:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Mar 2022 08:54:43 GMT
USER memcache
# Thu, 17 Mar 2022 08:54:44 GMT
EXPOSE 11211
# Thu, 17 Mar 2022 08:54:44 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:d51040c5bfbf434887bfed2557335a411e6ef760d04cc178d455d1c3ec1b721c`  
		Last Modified: Thu, 17 Mar 2022 03:05:26 GMT  
		Size: 2.6 MB (2601715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bafa61f6f0948b111a53b71e2c8c1312981357779ca88eaf5e60d4163dc7d03b`  
		Last Modified: Thu, 17 Mar 2022 08:55:51 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6282933aed68188fd9995db64b18a466643f4879e98a97392e6df0309f825ab`  
		Last Modified: Thu, 17 Mar 2022 08:55:51 GMT  
		Size: 113.8 KB (113794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d266558ba8144540d874cf2a04b80cdad0b98138893dbd2bf8dfc0a82587d0fc`  
		Last Modified: Thu, 17 Mar 2022 08:55:51 GMT  
		Size: 934.2 KB (934189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e97cc0f7d043b7a30a2ecd4a02847ed3d1227cdec67c577b9486ae3a40bb7f55`  
		Last Modified: Thu, 17 Mar 2022 08:55:51 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:973434578ea89c81d5ee8f8c926d6efab348a190b4d1f8c59c32b595e5e3ff14`  
		Last Modified: Thu, 17 Mar 2022 08:55:51 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:1-alpine3.15`

```console
$ docker pull memcached@sha256:614ca36d9fbc4953da3276766de5e77bdac23c04ffcde331032be6d854006131
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
$ docker pull memcached@sha256:fd1bb2a04baff1bc63d2323d91a4f7135b9f06f1d0294fbe13b8660db7b6dd78
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3862528 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e9d7d65a6545e2698d88de0e6c6eeb620a5bdf19e35635a36ac252bb7dce9d55`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 17 Mar 2022 04:01:58 GMT
ADD file:cf4b631a115c2bbfbd81cad2d3041bceb64a8136aac92ba8a63b6c51d60af764 in / 
# Thu, 17 Mar 2022 04:01:59 GMT
CMD ["/bin/sh"]
# Thu, 17 Mar 2022 12:51:33 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Thu, 17 Mar 2022 12:51:34 GMT
RUN apk add --no-cache libsasl
# Thu, 17 Mar 2022 12:51:34 GMT
ENV MEMCACHED_VERSION=1.6.14
# Thu, 17 Mar 2022 12:51:35 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Thu, 17 Mar 2022 12:55:35 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Thu, 17 Mar 2022 12:55:35 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 17 Mar 2022 12:55:36 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 17 Mar 2022 12:55:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Mar 2022 12:55:36 GMT
USER memcache
# Thu, 17 Mar 2022 12:55:36 GMT
EXPOSE 11211
# Thu, 17 Mar 2022 12:55:36 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:3d243047344378e9b7136d552d48feb7ea8b6fe14ce0990e0cc011d5e369626a`  
		Last Modified: Thu, 17 Mar 2022 04:02:41 GMT  
		Size: 2.8 MB (2812636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e26b137db66bd985a8103e3e70f8985eafa9a9ca3dc6aa33344245535f6a6b0`  
		Last Modified: Thu, 17 Mar 2022 12:56:25 GMT  
		Size: 1.3 KB (1263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5231e0cae31bc5e59bdcb40f696ceaa6b5cad70b9500bc5bfd459174ac1f78dd`  
		Last Modified: Thu, 17 Mar 2022 12:56:25 GMT  
		Size: 109.3 KB (109285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d9fab8e58febfe6f0bfb8d5bdc098221b6348a6128014c4c2b4d4086284696d`  
		Last Modified: Thu, 17 Mar 2022 12:56:25 GMT  
		Size: 938.9 KB (938943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9ca16ee180425777e36c6f23ab6755a192eedf107400360aac9332686f1212b`  
		Last Modified: Thu, 17 Mar 2022 12:56:25 GMT  
		Size: 280.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f81d444d82a8e26057630fab59b6bdb890fe42afa50edabbba60d8685e88d639`  
		Last Modified: Thu, 17 Mar 2022 12:56:24 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-alpine3.15` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:095e0c44c122b636ae053f2971bb454b3edfe210195707983a9e0a38d22f4411
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3754561 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d01922b70bc4d8d1d2be9eabafa82a0f0152a88e5871b7e9b6949cf1327c9c4f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 17 Mar 2022 03:19:52 GMT
ADD file:cd7d91362950471ca4678cf3833dc47119ab519dea51424c847bbbb21e1649d4 in / 
# Thu, 17 Mar 2022 03:19:52 GMT
CMD ["/bin/sh"]
# Thu, 17 Mar 2022 11:39:00 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Thu, 17 Mar 2022 11:39:02 GMT
RUN apk add --no-cache libsasl
# Thu, 17 Mar 2022 11:39:03 GMT
ENV MEMCACHED_VERSION=1.6.14
# Thu, 17 Mar 2022 11:39:04 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Thu, 17 Mar 2022 11:41:43 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Thu, 17 Mar 2022 11:41:45 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 17 Mar 2022 11:41:45 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 17 Mar 2022 11:41:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Mar 2022 11:41:47 GMT
USER memcache
# Thu, 17 Mar 2022 11:41:48 GMT
EXPOSE 11211
# Thu, 17 Mar 2022 11:41:49 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:148d739a8e6b9342daa1f5b428d3a3c6118f340f21df28c16e06f918ef150147`  
		Last Modified: Thu, 17 Mar 2022 03:20:45 GMT  
		Size: 2.7 MB (2714807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33dde588ab12fbb6aa46070a960ac850c8347e86f29744b40a123a466d4885ab`  
		Last Modified: Thu, 17 Mar 2022 11:42:57 GMT  
		Size: 1.2 KB (1240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bdeb7ac9fd9c67010a55bf3fe0e13866bb31d847353f455c95220027e2bc48c`  
		Last Modified: Thu, 17 Mar 2022 11:42:58 GMT  
		Size: 110.6 KB (110556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6bf3828467e4d3c16fcdc94bf5987db023e892ef9594c9c5dc2c3ccf07bc4bc`  
		Last Modified: Thu, 17 Mar 2022 11:42:58 GMT  
		Size: 927.5 KB (927550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d39e5be11e10e43e4991c6d85f4bdce89416e75c908d33656e4dcb79c26a51bc`  
		Last Modified: Thu, 17 Mar 2022 11:42:57 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9404edf07c113d954a0a5c34650b52d9a1f8e57d166b3e1b022a82c3e27e724`  
		Last Modified: Thu, 17 Mar 2022 11:42:57 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-alpine3.15` - linux; 386

```console
$ docker pull memcached@sha256:8a6352e717a8080f0c0888560cf7ae52c77ee2cbd10ed46c68822370b5188d0f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3891706 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4db903b8d549ba5f131fc35c81b69bdf1822950956033492f126e16dd95b5750`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 17 Mar 2022 08:13:03 GMT
ADD file:22216bc654d9177244235f242fa83cae3b283b3c145cad7ccf11c0d29f5f0ff2 in / 
# Thu, 17 Mar 2022 08:13:03 GMT
CMD ["/bin/sh"]
# Thu, 17 Mar 2022 17:35:31 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Thu, 17 Mar 2022 17:35:32 GMT
RUN apk add --no-cache libsasl
# Thu, 17 Mar 2022 17:35:32 GMT
ENV MEMCACHED_VERSION=1.6.14
# Thu, 17 Mar 2022 17:35:33 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Thu, 17 Mar 2022 17:39:25 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Thu, 17 Mar 2022 17:39:25 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 17 Mar 2022 17:39:26 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 17 Mar 2022 17:39:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Mar 2022 17:39:26 GMT
USER memcache
# Thu, 17 Mar 2022 17:39:26 GMT
EXPOSE 11211
# Thu, 17 Mar 2022 17:39:26 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:93317a1f65ec94b67aefe728a598022610246404e3a68d391c76cd0e5244a2a0`  
		Last Modified: Thu, 17 Mar 2022 08:13:56 GMT  
		Size: 2.8 MB (2821789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae4d8e906564040308eb9f4b96b3808d37aa02b7fffa8e8d5c80126d5e50b1cf`  
		Last Modified: Thu, 17 Mar 2022 17:40:52 GMT  
		Size: 1.3 KB (1263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16143ebb273f49cf3884d5a063dfac8b30d9527c5018e90fac51ac381b5a5f8b`  
		Last Modified: Thu, 17 Mar 2022 17:40:52 GMT  
		Size: 121.2 KB (121183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:107340d48cdbc30d4b57291ca0d28997feed13517f3a508b3b398620dbc97099`  
		Last Modified: Thu, 17 Mar 2022 17:40:52 GMT  
		Size: 947.1 KB (947068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a791ada3ee704cad0a4dba90d29f533e6fcadb132c2522c38b4f0680201a86a9`  
		Last Modified: Thu, 17 Mar 2022 17:40:52 GMT  
		Size: 282.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fc23e842aa74aed8a4ea48cf2b6f027f9592e43e117c394bc70b3d2dcf0627c`  
		Last Modified: Thu, 17 Mar 2022 17:40:53 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-alpine3.15` - linux; ppc64le

```console
$ docker pull memcached@sha256:75cb5141098fb02bb0c554c31c00d28802b414593a6b41d430c10505ee943fe0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.3 MB (5315837 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4be74852968716dd05ad711f1cda531afac5b782fe0dd6692e5aed7d91d54466`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 24 Nov 2021 20:20:16 GMT
ADD file:57115dca2eb707f46b6301e75174e6aa316fb02ac28643b91429b75be51bd8c8 in / 
# Wed, 24 Nov 2021 20:20:20 GMT
CMD ["/bin/sh"]
# Tue, 30 Nov 2021 00:52:13 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 30 Nov 2021 00:52:18 GMT
RUN apk add --no-cache libsasl
# Fri, 11 Feb 2022 23:54:02 GMT
ENV MEMCACHED_VERSION=1.6.14
# Fri, 11 Feb 2022 23:54:06 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Fri, 11 Feb 2022 23:57:48 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Fri, 11 Feb 2022 23:57:50 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 11 Feb 2022 23:57:55 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 11 Feb 2022 23:57:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Feb 2022 23:57:59 GMT
USER memcache
# Fri, 11 Feb 2022 23:58:01 GMT
EXPOSE 11211
# Fri, 11 Feb 2022 23:58:02 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:159b5dcb1717c815c76ff5ea1db730e18e8609c9090238e43282856db9e71f47`  
		Last Modified: Wed, 24 Nov 2021 20:21:14 GMT  
		Size: 2.8 MB (2814780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f44bb0dc5dc6d3634512266fffaecf643a467ef890e0a60fa7daed8a8f379335`  
		Last Modified: Tue, 30 Nov 2021 00:57:03 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:242bba95e896195e2c48210499ed8dad5c07a25a93e0d6304a787f4d5f05bb79`  
		Last Modified: Tue, 30 Nov 2021 00:57:03 GMT  
		Size: 126.2 KB (126210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9d933f0d59015113f25123de9b3460a03fdf091181f4c9330b1bb42c27a8cce`  
		Last Modified: Fri, 11 Feb 2022 23:59:16 GMT  
		Size: 2.4 MB (2373175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:659fd1f60c2bc05966f606e677370eeee3176f7d6dbd530b3f271ba313f8b0fe`  
		Last Modified: Fri, 11 Feb 2022 23:59:15 GMT  
		Size: 282.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8d9d86e7310ff252ce602224ce1643c6b8d50713444e43804cdb93912f89087`  
		Last Modified: Fri, 11 Feb 2022 23:59:15 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-alpine3.15` - linux; s390x

```console
$ docker pull memcached@sha256:5a931719c887b04ccf389c14867075cca4a76c774ecceb8231f801d876c94be9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.7 MB (3651372 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8aed3255f32676856491e1f6e999893205a57c1d26f36d52518c7d72433bcd9c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 17 Mar 2022 03:04:28 GMT
ADD file:f623c69acb1859b41ef29e8f20f4e6c7072d9c6d7210d745afc615251bfe418f in / 
# Thu, 17 Mar 2022 03:04:28 GMT
CMD ["/bin/sh"]
# Thu, 17 Mar 2022 08:51:10 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Thu, 17 Mar 2022 08:51:11 GMT
RUN apk add --no-cache libsasl
# Thu, 17 Mar 2022 08:51:12 GMT
ENV MEMCACHED_VERSION=1.6.14
# Thu, 17 Mar 2022 08:51:12 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Thu, 17 Mar 2022 08:54:42 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Thu, 17 Mar 2022 08:54:42 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 17 Mar 2022 08:54:43 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 17 Mar 2022 08:54:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Mar 2022 08:54:43 GMT
USER memcache
# Thu, 17 Mar 2022 08:54:44 GMT
EXPOSE 11211
# Thu, 17 Mar 2022 08:54:44 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:d51040c5bfbf434887bfed2557335a411e6ef760d04cc178d455d1c3ec1b721c`  
		Last Modified: Thu, 17 Mar 2022 03:05:26 GMT  
		Size: 2.6 MB (2601715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bafa61f6f0948b111a53b71e2c8c1312981357779ca88eaf5e60d4163dc7d03b`  
		Last Modified: Thu, 17 Mar 2022 08:55:51 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6282933aed68188fd9995db64b18a466643f4879e98a97392e6df0309f825ab`  
		Last Modified: Thu, 17 Mar 2022 08:55:51 GMT  
		Size: 113.8 KB (113794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d266558ba8144540d874cf2a04b80cdad0b98138893dbd2bf8dfc0a82587d0fc`  
		Last Modified: Thu, 17 Mar 2022 08:55:51 GMT  
		Size: 934.2 KB (934189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e97cc0f7d043b7a30a2ecd4a02847ed3d1227cdec67c577b9486ae3a40bb7f55`  
		Last Modified: Thu, 17 Mar 2022 08:55:51 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:973434578ea89c81d5ee8f8c926d6efab348a190b4d1f8c59c32b595e5e3ff14`  
		Last Modified: Thu, 17 Mar 2022 08:55:51 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:1-bullseye`

```console
$ docker pull memcached@sha256:67ceec1841427583fd33842be1a41243351997c4803d05c14f95f0c8c6826f93
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
$ docker pull memcached@sha256:6a51dd2e23a3ead43158d3255ab8c2d9b0b2f0432becf5814c267273c84e8b6a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.0 MB (32965129 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e897df046b27f4dbfae44d31346ef91c2160a46c1b8d5bf652a40e3d76d3914f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 17 Mar 2022 04:03:59 GMT
ADD file:36919ae6bb25e3269eff949443129a01a8a43fb967fe6563939ebe1e1e9b8228 in / 
# Thu, 17 Mar 2022 04:03:59 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 12:47:26 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Thu, 17 Mar 2022 12:47:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Mar 2022 12:47:29 GMT
ENV MEMCACHED_VERSION=1.6.14
# Thu, 17 Mar 2022 12:47:29 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Thu, 17 Mar 2022 12:51:18 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 17 Mar 2022 12:51:18 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 17 Mar 2022 12:51:18 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 17 Mar 2022 12:51:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Mar 2022 12:51:18 GMT
USER memcache
# Thu, 17 Mar 2022 12:51:19 GMT
EXPOSE 11211
# Thu, 17 Mar 2022 12:51:19 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:ae13dd57832654086618a81dbc128846aa092489260c326ee95429b63c3cf213`  
		Last Modified: Thu, 17 Mar 2022 04:10:05 GMT  
		Size: 31.4 MB (31376572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c39e8a8db385456589d2009379dedc9787a9297b0ea679ff564500de9894d325`  
		Last Modified: Thu, 17 Mar 2022 12:55:59 GMT  
		Size: 5.0 KB (4982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fa3e9def276e8e73128ec9d08c6f139621666d0724b33d882ca0943a1a6825b`  
		Last Modified: Thu, 17 Mar 2022 12:55:59 GMT  
		Size: 328.0 KB (328046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9835681ca994d84f0de3da2d9ed0cdb5882c06b58bccdc406102bf4bf8a55700`  
		Last Modified: Thu, 17 Mar 2022 12:55:59 GMT  
		Size: 1.3 MB (1255121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d362d7003189fa875ec372df3c4c9622f2688adb7ed5c9cb2bec35c31b9d523`  
		Last Modified: Thu, 17 Mar 2022 12:55:59 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bd4550226c671e2d98eac87073171c925eebaa0e039ed5e2610d516980dd220`  
		Last Modified: Thu, 17 Mar 2022 12:55:59 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-bullseye` - linux; arm variant v5

```console
$ docker pull memcached@sha256:084a4198172362acf346afa27655123636800a135bdaaa857d8d57e7e402c4fa
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.5 MB (30467908 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b9e543544c3f8ef04ec918e92a8e98602cbdc37970011b5960685ffd0103780`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 17 Mar 2022 05:19:45 GMT
ADD file:1eb4f937d40230354e20e28ed781234acd4be2b0dab72f87131a3eac66349719 in / 
# Thu, 17 Mar 2022 05:19:46 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 10:06:48 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Thu, 17 Mar 2022 10:06:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Mar 2022 10:07:00 GMT
ENV MEMCACHED_VERSION=1.6.14
# Thu, 17 Mar 2022 10:07:00 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Thu, 17 Mar 2022 10:11:18 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 17 Mar 2022 10:11:18 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 17 Mar 2022 10:11:20 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 17 Mar 2022 10:11:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Mar 2022 10:11:21 GMT
USER memcache
# Thu, 17 Mar 2022 10:11:21 GMT
EXPOSE 11211
# Thu, 17 Mar 2022 10:11:21 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:4da455e7774c0e977d862a56ab6d85f33ce5dd5a77d45a0a74a272e9eae6bea0`  
		Last Modified: Thu, 17 Mar 2022 05:35:01 GMT  
		Size: 28.9 MB (28919702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39450ea3e36758cb1aaf29a3e4a3694a4f1e5d208ece3da6479b6dcd47705309`  
		Last Modified: Thu, 17 Mar 2022 10:12:14 GMT  
		Size: 4.9 KB (4890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b674f1fc0977777c240d7af9fa6d57e8b24d5332791547c80820aa9d1956d037`  
		Last Modified: Thu, 17 Mar 2022 10:12:14 GMT  
		Size: 316.6 KB (316575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de44c6f01b62d4d56baa2601e6706305eaf35c2da9541623a8c94c7fe1e4b8b2`  
		Last Modified: Thu, 17 Mar 2022 10:12:14 GMT  
		Size: 1.2 MB (1226335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18229473d3cfa938b3ba5d7f36b228bc60b7641660ae3242b56e210a50892b0f`  
		Last Modified: Thu, 17 Mar 2022 10:12:14 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e231e6a0756abb2590d1ef0507c610f0aa1b4f42e40a895d310b330662a98a2`  
		Last Modified: Thu, 17 Mar 2022 10:12:14 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-bullseye` - linux; arm variant v7

```console
$ docker pull memcached@sha256:9fe6c86dfef8c0cf535d443045364d887fd0bc8b44f550a8cbb0dca64e33e732
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.1 MB (28090226 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14dc9d69afed7832780e59eca9bf08aecbca59e357a3c301648a665b42b6659a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 17 Mar 2022 09:31:03 GMT
ADD file:e52f9ee2dc3144d7b9eb3ec90c106aa2a094eb4c5c2aa8cbff5c520a5faaef43 in / 
# Thu, 17 Mar 2022 09:31:04 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 21:53:04 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Thu, 17 Mar 2022 21:53:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Mar 2022 21:53:14 GMT
ENV MEMCACHED_VERSION=1.6.14
# Thu, 17 Mar 2022 21:53:14 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Thu, 17 Mar 2022 21:57:21 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 17 Mar 2022 21:57:22 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 17 Mar 2022 21:57:23 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 17 Mar 2022 21:57:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Mar 2022 21:57:24 GMT
USER memcache
# Thu, 17 Mar 2022 21:57:25 GMT
EXPOSE 11211
# Thu, 17 Mar 2022 21:57:25 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:5e5e708ee1f9fdbc69324391f7d1f816c657e6116eff09e7d2247fa9de3a076a`  
		Last Modified: Thu, 17 Mar 2022 09:46:33 GMT  
		Size: 26.6 MB (26575097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f652a8bcf3f50c242f3e27b3792cd55f9c0436702fe2bcdd4ae3df203aa84100`  
		Last Modified: Thu, 17 Mar 2022 22:10:19 GMT  
		Size: 4.9 KB (4896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c1be80f12d4f19157864e18689a8dd9c0f84c3a6c929949b066e7c29f30c5d7`  
		Last Modified: Thu, 17 Mar 2022 22:10:19 GMT  
		Size: 312.0 KB (311999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37ab28ddd02c6ca7832dec8a6b6508e8e4d95b34c8f4fe17457a1844c4442a7a`  
		Last Modified: Thu, 17 Mar 2022 22:10:19 GMT  
		Size: 1.2 MB (1197826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6d7e30c2d27f64a3117e85e87c00c1d4e79aa91e0bf4e4552c68d4710592d64`  
		Last Modified: Thu, 17 Mar 2022 22:10:19 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7f72f97159e0cf88a536b1a268d9bfa7af992046ce641dddb6710eabf7d08e4`  
		Last Modified: Thu, 17 Mar 2022 22:10:19 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-bullseye` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:773c0f8c11aa82d0bf14e751ab65784b8993bd7477026d660eb8e970b160aad8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.4 MB (31441503 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1cc644adcd708fa1761227654eacbdd25163b6a5a399599e20c7eabdc2a24a8f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 17 Mar 2022 03:21:57 GMT
ADD file:e52e032f1ace6abd44b3647d43c1b8ae30bac6de804eef09c6ccd793057996fd in / 
# Thu, 17 Mar 2022 03:21:58 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 11:35:48 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Thu, 17 Mar 2022 11:35:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Mar 2022 11:35:52 GMT
ENV MEMCACHED_VERSION=1.6.14
# Thu, 17 Mar 2022 11:35:53 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Thu, 17 Mar 2022 11:38:38 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 17 Mar 2022 11:38:40 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 17 Mar 2022 11:38:40 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 17 Mar 2022 11:38:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Mar 2022 11:38:42 GMT
USER memcache
# Thu, 17 Mar 2022 11:38:43 GMT
EXPOSE 11211
# Thu, 17 Mar 2022 11:38:44 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:32252aec0777ac025a158bc2a8317650a4f2a0a875387011b1165013874f8723`  
		Last Modified: Thu, 17 Mar 2022 03:28:36 GMT  
		Size: 30.1 MB (30063013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:966f1b38b9d3f62f875f8dbd868ecc80c2037b45aadbec50fc16d292be747303`  
		Last Modified: Thu, 17 Mar 2022 11:42:26 GMT  
		Size: 4.9 KB (4903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2898c9abf66c159176811eff24e689c0989d4e7c025c9a7eb0f933d356aec11`  
		Last Modified: Thu, 17 Mar 2022 11:42:26 GMT  
		Size: 119.2 KB (119181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d331819fcfc0b6541dc90aafde95bc8b8a88e453cb3800c977716cff65961a77`  
		Last Modified: Thu, 17 Mar 2022 11:42:26 GMT  
		Size: 1.3 MB (1254002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25a25819b974fbc38bad380c4df00bf1f032cf4eb0112a109c78f9858d9a0a55`  
		Last Modified: Thu, 17 Mar 2022 11:42:26 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7c790b93b28eb9ed542eac0eaf8c5fe2d4c5daa368b0f27bac067fd01bee280`  
		Last Modified: Thu, 17 Mar 2022 11:42:26 GMT  
		Size: 118.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-bullseye` - linux; 386

```console
$ docker pull memcached@sha256:3d0458851092782bb1cfb8fdb3edb27fe63775c3fb68f1879137e691de184e82
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.0 MB (33981668 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b7d3a232500fae88433d6e4117fa6e45b0ed4c529c925734eb2982bf3a3ee54`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 17 Mar 2022 08:15:53 GMT
ADD file:2d6be3846f0e5fabd85bc9409b1e2223cad4c57c76f96e9f81489ba78a72a1f5 in / 
# Thu, 17 Mar 2022 08:15:54 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 17:31:22 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Thu, 17 Mar 2022 17:31:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Mar 2022 17:31:26 GMT
ENV MEMCACHED_VERSION=1.6.14
# Thu, 17 Mar 2022 17:31:26 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Thu, 17 Mar 2022 17:35:17 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 17 Mar 2022 17:35:17 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 17 Mar 2022 17:35:18 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 17 Mar 2022 17:35:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Mar 2022 17:35:18 GMT
USER memcache
# Thu, 17 Mar 2022 17:35:18 GMT
EXPOSE 11211
# Thu, 17 Mar 2022 17:35:18 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:176085117cac9b2cf2cf57b3a10c9811dbd2773497fbac3086b5024070447e97`  
		Last Modified: Thu, 17 Mar 2022 08:24:00 GMT  
		Size: 32.4 MB (32386475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe18ed3f6ff50e5b12a7db917c34de3104619ae31e84d9d83ad2d94a3b8c5822`  
		Last Modified: Thu, 17 Mar 2022 17:40:19 GMT  
		Size: 4.9 KB (4896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc15fd9e0c057bb0a0d077f6c21d0b980b6ec5f9e5292c19d6fd790731f7bfc6`  
		Last Modified: Thu, 17 Mar 2022 17:40:19 GMT  
		Size: 336.6 KB (336638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1f8475d0ca14b4624de06fbe3207cdf07b5c31573192d0acc9b1e600b90c430`  
		Last Modified: Thu, 17 Mar 2022 17:40:20 GMT  
		Size: 1.3 MB (1253253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61e85d2ca17a8c6eb12e9cdc031a20d5c2357cf22bc4ad5353d520e13f60b73a`  
		Last Modified: Thu, 17 Mar 2022 17:40:19 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3194d39d810076bc29397aa1a117ac51d7bc610ffb9b7c90613fdf21203b05a3`  
		Last Modified: Thu, 17 Mar 2022 17:40:19 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-bullseye` - linux; mips64le

```console
$ docker pull memcached@sha256:9148cd77f369a80c3b52dd4f79ddd8073c192da135e99a311f54641a851b4b60
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.0 MB (31012937 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:16b4bbcf6270bfbe61ccbb8083bf46151a57eb6a74f044b2004509978709ee0d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 17 Mar 2022 08:53:04 GMT
ADD file:795ac4eba576bc4c995df2a18b10ce802ee8a05417cdc53f5aa09452ecf2e832 in / 
# Thu, 17 Mar 2022 08:53:08 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 20:37:19 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Thu, 17 Mar 2022 20:37:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Mar 2022 20:37:40 GMT
ENV MEMCACHED_VERSION=1.6.14
# Thu, 17 Mar 2022 20:37:43 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Thu, 17 Mar 2022 20:44:58 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 17 Mar 2022 20:45:00 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 17 Mar 2022 20:45:05 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 17 Mar 2022 20:45:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Mar 2022 20:45:10 GMT
USER memcache
# Thu, 17 Mar 2022 20:45:13 GMT
EXPOSE 11211
# Thu, 17 Mar 2022 20:45:15 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:4799d88734ae94287a665c0e14621a744706cfbe17a0cf27ae9b0cc630927b11`  
		Last Modified: Thu, 17 Mar 2022 10:43:20 GMT  
		Size: 29.6 MB (29639810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a091b8fd61b3c0cafad5676908a202cec423a829bd2fb2bb79011b3ad5fd0845`  
		Last Modified: Thu, 17 Mar 2022 20:45:41 GMT  
		Size: 4.9 KB (4859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7644e6d2f727759be27279ab11b8f3e186b6918c1b3847badb0d04ae020286b`  
		Last Modified: Thu, 17 Mar 2022 20:45:41 GMT  
		Size: 117.1 KB (117098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47e8f3183abaf23ec67f322bc78981d3c838ad27bba488ec924c07d5b1a053a4`  
		Last Modified: Thu, 17 Mar 2022 20:45:41 GMT  
		Size: 1.3 MB (1250762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f0ac34ae7971e4442dd9abb2bbfa522fc4e65445f1ed51d33795cea9b37830e`  
		Last Modified: Thu, 17 Mar 2022 20:45:40 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0564ebbfe5b917d8a4818a435ddb35d5e4bbb4b4d7187189578f1c224d10ce2b`  
		Last Modified: Thu, 17 Mar 2022 20:45:40 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-bullseye` - linux; ppc64le

```console
$ docker pull memcached@sha256:4893f4daa742b31f414b08f98f8e7d0cbedaf63b8d88062bcf3c91a9522a2aab
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.0 MB (36957544 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8db953cc998ed06712eca57fe4ae2b8bb342ce991683fd7592495a21557d0940`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 26 Jan 2022 01:46:51 GMT
ADD file:c03f34c221e57fa5cb625c166d1db9f72d6ba2fa17a3c41a5d04d6875d098949 in / 
# Wed, 26 Jan 2022 01:46:57 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 05:38:39 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 26 Jan 2022 05:38:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 11 Feb 2022 23:47:36 GMT
ENV MEMCACHED_VERSION=1.6.14
# Fri, 11 Feb 2022 23:47:38 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Fri, 11 Feb 2022 23:53:07 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Fri, 11 Feb 2022 23:53:13 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 11 Feb 2022 23:53:34 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 11 Feb 2022 23:53:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Feb 2022 23:53:39 GMT
USER memcache
# Fri, 11 Feb 2022 23:53:41 GMT
EXPOSE 11211
# Fri, 11 Feb 2022 23:53:46 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:3149ee4a73508a4c39107d64a3fdc1b021626a22a0ac95e62fa0cea49ab77fba`  
		Last Modified: Wed, 26 Jan 2022 01:57:01 GMT  
		Size: 35.3 MB (35273030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07bcb451658eb6d9eace467c2e989d96e53c409eb48347a369e9ad80aadcfe96`  
		Last Modified: Wed, 26 Jan 2022 05:45:22 GMT  
		Size: 5.0 KB (4980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8807782e060aa90873de57b2d3ec277632145f166e9c1e3801c57eea7e595cc`  
		Last Modified: Wed, 26 Jan 2022 05:45:22 GMT  
		Size: 356.9 KB (356905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5f2e5d5bb1609e336a37e97218d618550ec5ce28384c32b1141393ef6f04a03`  
		Last Modified: Fri, 11 Feb 2022 23:58:44 GMT  
		Size: 1.3 MB (1322220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76e6da4f290b1cff2fa5b1ad17d42333c67179332511db4da3bd2c5ce12bbdfa`  
		Last Modified: Fri, 11 Feb 2022 23:58:44 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fb140c5468aa121999bc169d30e4ce6b73795cdf67aa21c1dfd3d1194dd0b82`  
		Last Modified: Fri, 11 Feb 2022 23:58:44 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-bullseye` - linux; s390x

```console
$ docker pull memcached@sha256:3e4437e519528ef8d3274dfc333f59f7c8c90099329a1e041fb6a71d5be8a1c5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.2 MB (31225911 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6fbcefffe918634bf299753ebcfe4a7284155e249686c5b5db9ffa92a5c0fc87`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 17 Mar 2022 03:06:58 GMT
ADD file:52f9267b4c57ac585a0d3d47a6f2ae1a71398264173ad4f190332957fa629c67 in / 
# Thu, 17 Mar 2022 03:07:01 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 08:47:34 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Thu, 17 Mar 2022 08:47:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Mar 2022 08:47:37 GMT
ENV MEMCACHED_VERSION=1.6.14
# Thu, 17 Mar 2022 08:47:37 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Thu, 17 Mar 2022 08:50:57 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 17 Mar 2022 08:50:57 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 17 Mar 2022 08:50:58 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 17 Mar 2022 08:50:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Mar 2022 08:50:58 GMT
USER memcache
# Thu, 17 Mar 2022 08:50:58 GMT
EXPOSE 11211
# Thu, 17 Mar 2022 08:50:59 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:d101968410e5005df630b0572aec03c88de55b8de81f3cf7e6a57e1ce2e5a8e5`  
		Last Modified: Thu, 17 Mar 2022 03:12:46 GMT  
		Size: 29.7 MB (29655795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1cad003ec39dc6e2e144c0953bad3bce3807fd1679d2c9e27e510724476e1e6`  
		Last Modified: Thu, 17 Mar 2022 08:55:34 GMT  
		Size: 5.0 KB (5022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13e61c306aebe51ff20adaf4ac683a69d93022d34ed4d09bc2ae7bde9d92ba52`  
		Last Modified: Thu, 17 Mar 2022 08:55:34 GMT  
		Size: 324.1 KB (324147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b5e88f796665ba79a22e6a541cbc3f30242e708c56d6b9af4fd0a7cd23abea6`  
		Last Modified: Thu, 17 Mar 2022 08:55:34 GMT  
		Size: 1.2 MB (1240539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77d35a1cb446cb01584cfbb3a61c40aaa1f358f37c8d723fe2437e6d070dbce3`  
		Last Modified: Thu, 17 Mar 2022 08:55:34 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b237b13dadf10fc593967f3714eaab56b7b00b89d435eb7e01be3f172b5b9b69`  
		Last Modified: Thu, 17 Mar 2022 08:55:33 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:1.6`

```console
$ docker pull memcached@sha256:67ceec1841427583fd33842be1a41243351997c4803d05c14f95f0c8c6826f93
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
$ docker pull memcached@sha256:6a51dd2e23a3ead43158d3255ab8c2d9b0b2f0432becf5814c267273c84e8b6a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.0 MB (32965129 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e897df046b27f4dbfae44d31346ef91c2160a46c1b8d5bf652a40e3d76d3914f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 17 Mar 2022 04:03:59 GMT
ADD file:36919ae6bb25e3269eff949443129a01a8a43fb967fe6563939ebe1e1e9b8228 in / 
# Thu, 17 Mar 2022 04:03:59 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 12:47:26 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Thu, 17 Mar 2022 12:47:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Mar 2022 12:47:29 GMT
ENV MEMCACHED_VERSION=1.6.14
# Thu, 17 Mar 2022 12:47:29 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Thu, 17 Mar 2022 12:51:18 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 17 Mar 2022 12:51:18 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 17 Mar 2022 12:51:18 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 17 Mar 2022 12:51:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Mar 2022 12:51:18 GMT
USER memcache
# Thu, 17 Mar 2022 12:51:19 GMT
EXPOSE 11211
# Thu, 17 Mar 2022 12:51:19 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:ae13dd57832654086618a81dbc128846aa092489260c326ee95429b63c3cf213`  
		Last Modified: Thu, 17 Mar 2022 04:10:05 GMT  
		Size: 31.4 MB (31376572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c39e8a8db385456589d2009379dedc9787a9297b0ea679ff564500de9894d325`  
		Last Modified: Thu, 17 Mar 2022 12:55:59 GMT  
		Size: 5.0 KB (4982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fa3e9def276e8e73128ec9d08c6f139621666d0724b33d882ca0943a1a6825b`  
		Last Modified: Thu, 17 Mar 2022 12:55:59 GMT  
		Size: 328.0 KB (328046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9835681ca994d84f0de3da2d9ed0cdb5882c06b58bccdc406102bf4bf8a55700`  
		Last Modified: Thu, 17 Mar 2022 12:55:59 GMT  
		Size: 1.3 MB (1255121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d362d7003189fa875ec372df3c4c9622f2688adb7ed5c9cb2bec35c31b9d523`  
		Last Modified: Thu, 17 Mar 2022 12:55:59 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bd4550226c671e2d98eac87073171c925eebaa0e039ed5e2610d516980dd220`  
		Last Modified: Thu, 17 Mar 2022 12:55:59 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6` - linux; arm variant v5

```console
$ docker pull memcached@sha256:084a4198172362acf346afa27655123636800a135bdaaa857d8d57e7e402c4fa
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.5 MB (30467908 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b9e543544c3f8ef04ec918e92a8e98602cbdc37970011b5960685ffd0103780`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 17 Mar 2022 05:19:45 GMT
ADD file:1eb4f937d40230354e20e28ed781234acd4be2b0dab72f87131a3eac66349719 in / 
# Thu, 17 Mar 2022 05:19:46 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 10:06:48 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Thu, 17 Mar 2022 10:06:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Mar 2022 10:07:00 GMT
ENV MEMCACHED_VERSION=1.6.14
# Thu, 17 Mar 2022 10:07:00 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Thu, 17 Mar 2022 10:11:18 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 17 Mar 2022 10:11:18 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 17 Mar 2022 10:11:20 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 17 Mar 2022 10:11:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Mar 2022 10:11:21 GMT
USER memcache
# Thu, 17 Mar 2022 10:11:21 GMT
EXPOSE 11211
# Thu, 17 Mar 2022 10:11:21 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:4da455e7774c0e977d862a56ab6d85f33ce5dd5a77d45a0a74a272e9eae6bea0`  
		Last Modified: Thu, 17 Mar 2022 05:35:01 GMT  
		Size: 28.9 MB (28919702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39450ea3e36758cb1aaf29a3e4a3694a4f1e5d208ece3da6479b6dcd47705309`  
		Last Modified: Thu, 17 Mar 2022 10:12:14 GMT  
		Size: 4.9 KB (4890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b674f1fc0977777c240d7af9fa6d57e8b24d5332791547c80820aa9d1956d037`  
		Last Modified: Thu, 17 Mar 2022 10:12:14 GMT  
		Size: 316.6 KB (316575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de44c6f01b62d4d56baa2601e6706305eaf35c2da9541623a8c94c7fe1e4b8b2`  
		Last Modified: Thu, 17 Mar 2022 10:12:14 GMT  
		Size: 1.2 MB (1226335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18229473d3cfa938b3ba5d7f36b228bc60b7641660ae3242b56e210a50892b0f`  
		Last Modified: Thu, 17 Mar 2022 10:12:14 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e231e6a0756abb2590d1ef0507c610f0aa1b4f42e40a895d310b330662a98a2`  
		Last Modified: Thu, 17 Mar 2022 10:12:14 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6` - linux; arm variant v7

```console
$ docker pull memcached@sha256:9fe6c86dfef8c0cf535d443045364d887fd0bc8b44f550a8cbb0dca64e33e732
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.1 MB (28090226 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14dc9d69afed7832780e59eca9bf08aecbca59e357a3c301648a665b42b6659a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 17 Mar 2022 09:31:03 GMT
ADD file:e52f9ee2dc3144d7b9eb3ec90c106aa2a094eb4c5c2aa8cbff5c520a5faaef43 in / 
# Thu, 17 Mar 2022 09:31:04 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 21:53:04 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Thu, 17 Mar 2022 21:53:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Mar 2022 21:53:14 GMT
ENV MEMCACHED_VERSION=1.6.14
# Thu, 17 Mar 2022 21:53:14 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Thu, 17 Mar 2022 21:57:21 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 17 Mar 2022 21:57:22 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 17 Mar 2022 21:57:23 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 17 Mar 2022 21:57:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Mar 2022 21:57:24 GMT
USER memcache
# Thu, 17 Mar 2022 21:57:25 GMT
EXPOSE 11211
# Thu, 17 Mar 2022 21:57:25 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:5e5e708ee1f9fdbc69324391f7d1f816c657e6116eff09e7d2247fa9de3a076a`  
		Last Modified: Thu, 17 Mar 2022 09:46:33 GMT  
		Size: 26.6 MB (26575097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f652a8bcf3f50c242f3e27b3792cd55f9c0436702fe2bcdd4ae3df203aa84100`  
		Last Modified: Thu, 17 Mar 2022 22:10:19 GMT  
		Size: 4.9 KB (4896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c1be80f12d4f19157864e18689a8dd9c0f84c3a6c929949b066e7c29f30c5d7`  
		Last Modified: Thu, 17 Mar 2022 22:10:19 GMT  
		Size: 312.0 KB (311999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37ab28ddd02c6ca7832dec8a6b6508e8e4d95b34c8f4fe17457a1844c4442a7a`  
		Last Modified: Thu, 17 Mar 2022 22:10:19 GMT  
		Size: 1.2 MB (1197826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6d7e30c2d27f64a3117e85e87c00c1d4e79aa91e0bf4e4552c68d4710592d64`  
		Last Modified: Thu, 17 Mar 2022 22:10:19 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7f72f97159e0cf88a536b1a268d9bfa7af992046ce641dddb6710eabf7d08e4`  
		Last Modified: Thu, 17 Mar 2022 22:10:19 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:773c0f8c11aa82d0bf14e751ab65784b8993bd7477026d660eb8e970b160aad8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.4 MB (31441503 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1cc644adcd708fa1761227654eacbdd25163b6a5a399599e20c7eabdc2a24a8f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 17 Mar 2022 03:21:57 GMT
ADD file:e52e032f1ace6abd44b3647d43c1b8ae30bac6de804eef09c6ccd793057996fd in / 
# Thu, 17 Mar 2022 03:21:58 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 11:35:48 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Thu, 17 Mar 2022 11:35:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Mar 2022 11:35:52 GMT
ENV MEMCACHED_VERSION=1.6.14
# Thu, 17 Mar 2022 11:35:53 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Thu, 17 Mar 2022 11:38:38 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 17 Mar 2022 11:38:40 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 17 Mar 2022 11:38:40 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 17 Mar 2022 11:38:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Mar 2022 11:38:42 GMT
USER memcache
# Thu, 17 Mar 2022 11:38:43 GMT
EXPOSE 11211
# Thu, 17 Mar 2022 11:38:44 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:32252aec0777ac025a158bc2a8317650a4f2a0a875387011b1165013874f8723`  
		Last Modified: Thu, 17 Mar 2022 03:28:36 GMT  
		Size: 30.1 MB (30063013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:966f1b38b9d3f62f875f8dbd868ecc80c2037b45aadbec50fc16d292be747303`  
		Last Modified: Thu, 17 Mar 2022 11:42:26 GMT  
		Size: 4.9 KB (4903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2898c9abf66c159176811eff24e689c0989d4e7c025c9a7eb0f933d356aec11`  
		Last Modified: Thu, 17 Mar 2022 11:42:26 GMT  
		Size: 119.2 KB (119181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d331819fcfc0b6541dc90aafde95bc8b8a88e453cb3800c977716cff65961a77`  
		Last Modified: Thu, 17 Mar 2022 11:42:26 GMT  
		Size: 1.3 MB (1254002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25a25819b974fbc38bad380c4df00bf1f032cf4eb0112a109c78f9858d9a0a55`  
		Last Modified: Thu, 17 Mar 2022 11:42:26 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7c790b93b28eb9ed542eac0eaf8c5fe2d4c5daa368b0f27bac067fd01bee280`  
		Last Modified: Thu, 17 Mar 2022 11:42:26 GMT  
		Size: 118.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6` - linux; 386

```console
$ docker pull memcached@sha256:3d0458851092782bb1cfb8fdb3edb27fe63775c3fb68f1879137e691de184e82
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.0 MB (33981668 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b7d3a232500fae88433d6e4117fa6e45b0ed4c529c925734eb2982bf3a3ee54`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 17 Mar 2022 08:15:53 GMT
ADD file:2d6be3846f0e5fabd85bc9409b1e2223cad4c57c76f96e9f81489ba78a72a1f5 in / 
# Thu, 17 Mar 2022 08:15:54 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 17:31:22 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Thu, 17 Mar 2022 17:31:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Mar 2022 17:31:26 GMT
ENV MEMCACHED_VERSION=1.6.14
# Thu, 17 Mar 2022 17:31:26 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Thu, 17 Mar 2022 17:35:17 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 17 Mar 2022 17:35:17 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 17 Mar 2022 17:35:18 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 17 Mar 2022 17:35:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Mar 2022 17:35:18 GMT
USER memcache
# Thu, 17 Mar 2022 17:35:18 GMT
EXPOSE 11211
# Thu, 17 Mar 2022 17:35:18 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:176085117cac9b2cf2cf57b3a10c9811dbd2773497fbac3086b5024070447e97`  
		Last Modified: Thu, 17 Mar 2022 08:24:00 GMT  
		Size: 32.4 MB (32386475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe18ed3f6ff50e5b12a7db917c34de3104619ae31e84d9d83ad2d94a3b8c5822`  
		Last Modified: Thu, 17 Mar 2022 17:40:19 GMT  
		Size: 4.9 KB (4896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc15fd9e0c057bb0a0d077f6c21d0b980b6ec5f9e5292c19d6fd790731f7bfc6`  
		Last Modified: Thu, 17 Mar 2022 17:40:19 GMT  
		Size: 336.6 KB (336638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1f8475d0ca14b4624de06fbe3207cdf07b5c31573192d0acc9b1e600b90c430`  
		Last Modified: Thu, 17 Mar 2022 17:40:20 GMT  
		Size: 1.3 MB (1253253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61e85d2ca17a8c6eb12e9cdc031a20d5c2357cf22bc4ad5353d520e13f60b73a`  
		Last Modified: Thu, 17 Mar 2022 17:40:19 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3194d39d810076bc29397aa1a117ac51d7bc610ffb9b7c90613fdf21203b05a3`  
		Last Modified: Thu, 17 Mar 2022 17:40:19 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6` - linux; mips64le

```console
$ docker pull memcached@sha256:9148cd77f369a80c3b52dd4f79ddd8073c192da135e99a311f54641a851b4b60
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.0 MB (31012937 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:16b4bbcf6270bfbe61ccbb8083bf46151a57eb6a74f044b2004509978709ee0d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 17 Mar 2022 08:53:04 GMT
ADD file:795ac4eba576bc4c995df2a18b10ce802ee8a05417cdc53f5aa09452ecf2e832 in / 
# Thu, 17 Mar 2022 08:53:08 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 20:37:19 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Thu, 17 Mar 2022 20:37:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Mar 2022 20:37:40 GMT
ENV MEMCACHED_VERSION=1.6.14
# Thu, 17 Mar 2022 20:37:43 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Thu, 17 Mar 2022 20:44:58 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 17 Mar 2022 20:45:00 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 17 Mar 2022 20:45:05 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 17 Mar 2022 20:45:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Mar 2022 20:45:10 GMT
USER memcache
# Thu, 17 Mar 2022 20:45:13 GMT
EXPOSE 11211
# Thu, 17 Mar 2022 20:45:15 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:4799d88734ae94287a665c0e14621a744706cfbe17a0cf27ae9b0cc630927b11`  
		Last Modified: Thu, 17 Mar 2022 10:43:20 GMT  
		Size: 29.6 MB (29639810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a091b8fd61b3c0cafad5676908a202cec423a829bd2fb2bb79011b3ad5fd0845`  
		Last Modified: Thu, 17 Mar 2022 20:45:41 GMT  
		Size: 4.9 KB (4859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7644e6d2f727759be27279ab11b8f3e186b6918c1b3847badb0d04ae020286b`  
		Last Modified: Thu, 17 Mar 2022 20:45:41 GMT  
		Size: 117.1 KB (117098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47e8f3183abaf23ec67f322bc78981d3c838ad27bba488ec924c07d5b1a053a4`  
		Last Modified: Thu, 17 Mar 2022 20:45:41 GMT  
		Size: 1.3 MB (1250762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f0ac34ae7971e4442dd9abb2bbfa522fc4e65445f1ed51d33795cea9b37830e`  
		Last Modified: Thu, 17 Mar 2022 20:45:40 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0564ebbfe5b917d8a4818a435ddb35d5e4bbb4b4d7187189578f1c224d10ce2b`  
		Last Modified: Thu, 17 Mar 2022 20:45:40 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6` - linux; ppc64le

```console
$ docker pull memcached@sha256:4893f4daa742b31f414b08f98f8e7d0cbedaf63b8d88062bcf3c91a9522a2aab
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.0 MB (36957544 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8db953cc998ed06712eca57fe4ae2b8bb342ce991683fd7592495a21557d0940`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 26 Jan 2022 01:46:51 GMT
ADD file:c03f34c221e57fa5cb625c166d1db9f72d6ba2fa17a3c41a5d04d6875d098949 in / 
# Wed, 26 Jan 2022 01:46:57 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 05:38:39 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 26 Jan 2022 05:38:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 11 Feb 2022 23:47:36 GMT
ENV MEMCACHED_VERSION=1.6.14
# Fri, 11 Feb 2022 23:47:38 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Fri, 11 Feb 2022 23:53:07 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Fri, 11 Feb 2022 23:53:13 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 11 Feb 2022 23:53:34 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 11 Feb 2022 23:53:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Feb 2022 23:53:39 GMT
USER memcache
# Fri, 11 Feb 2022 23:53:41 GMT
EXPOSE 11211
# Fri, 11 Feb 2022 23:53:46 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:3149ee4a73508a4c39107d64a3fdc1b021626a22a0ac95e62fa0cea49ab77fba`  
		Last Modified: Wed, 26 Jan 2022 01:57:01 GMT  
		Size: 35.3 MB (35273030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07bcb451658eb6d9eace467c2e989d96e53c409eb48347a369e9ad80aadcfe96`  
		Last Modified: Wed, 26 Jan 2022 05:45:22 GMT  
		Size: 5.0 KB (4980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8807782e060aa90873de57b2d3ec277632145f166e9c1e3801c57eea7e595cc`  
		Last Modified: Wed, 26 Jan 2022 05:45:22 GMT  
		Size: 356.9 KB (356905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5f2e5d5bb1609e336a37e97218d618550ec5ce28384c32b1141393ef6f04a03`  
		Last Modified: Fri, 11 Feb 2022 23:58:44 GMT  
		Size: 1.3 MB (1322220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76e6da4f290b1cff2fa5b1ad17d42333c67179332511db4da3bd2c5ce12bbdfa`  
		Last Modified: Fri, 11 Feb 2022 23:58:44 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fb140c5468aa121999bc169d30e4ce6b73795cdf67aa21c1dfd3d1194dd0b82`  
		Last Modified: Fri, 11 Feb 2022 23:58:44 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6` - linux; s390x

```console
$ docker pull memcached@sha256:3e4437e519528ef8d3274dfc333f59f7c8c90099329a1e041fb6a71d5be8a1c5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.2 MB (31225911 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6fbcefffe918634bf299753ebcfe4a7284155e249686c5b5db9ffa92a5c0fc87`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 17 Mar 2022 03:06:58 GMT
ADD file:52f9267b4c57ac585a0d3d47a6f2ae1a71398264173ad4f190332957fa629c67 in / 
# Thu, 17 Mar 2022 03:07:01 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 08:47:34 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Thu, 17 Mar 2022 08:47:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Mar 2022 08:47:37 GMT
ENV MEMCACHED_VERSION=1.6.14
# Thu, 17 Mar 2022 08:47:37 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Thu, 17 Mar 2022 08:50:57 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 17 Mar 2022 08:50:57 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 17 Mar 2022 08:50:58 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 17 Mar 2022 08:50:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Mar 2022 08:50:58 GMT
USER memcache
# Thu, 17 Mar 2022 08:50:58 GMT
EXPOSE 11211
# Thu, 17 Mar 2022 08:50:59 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:d101968410e5005df630b0572aec03c88de55b8de81f3cf7e6a57e1ce2e5a8e5`  
		Last Modified: Thu, 17 Mar 2022 03:12:46 GMT  
		Size: 29.7 MB (29655795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1cad003ec39dc6e2e144c0953bad3bce3807fd1679d2c9e27e510724476e1e6`  
		Last Modified: Thu, 17 Mar 2022 08:55:34 GMT  
		Size: 5.0 KB (5022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13e61c306aebe51ff20adaf4ac683a69d93022d34ed4d09bc2ae7bde9d92ba52`  
		Last Modified: Thu, 17 Mar 2022 08:55:34 GMT  
		Size: 324.1 KB (324147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b5e88f796665ba79a22e6a541cbc3f30242e708c56d6b9af4fd0a7cd23abea6`  
		Last Modified: Thu, 17 Mar 2022 08:55:34 GMT  
		Size: 1.2 MB (1240539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77d35a1cb446cb01584cfbb3a61c40aaa1f358f37c8d723fe2437e6d070dbce3`  
		Last Modified: Thu, 17 Mar 2022 08:55:34 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b237b13dadf10fc593967f3714eaab56b7b00b89d435eb7e01be3f172b5b9b69`  
		Last Modified: Thu, 17 Mar 2022 08:55:33 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:1.6-alpine`

```console
$ docker pull memcached@sha256:f29cd53458fed5079ec81d66878db3f5ef40001b371b0437af6d5a660008f779
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
$ docker pull memcached@sha256:fd1bb2a04baff1bc63d2323d91a4f7135b9f06f1d0294fbe13b8660db7b6dd78
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3862528 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e9d7d65a6545e2698d88de0e6c6eeb620a5bdf19e35635a36ac252bb7dce9d55`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 17 Mar 2022 04:01:58 GMT
ADD file:cf4b631a115c2bbfbd81cad2d3041bceb64a8136aac92ba8a63b6c51d60af764 in / 
# Thu, 17 Mar 2022 04:01:59 GMT
CMD ["/bin/sh"]
# Thu, 17 Mar 2022 12:51:33 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Thu, 17 Mar 2022 12:51:34 GMT
RUN apk add --no-cache libsasl
# Thu, 17 Mar 2022 12:51:34 GMT
ENV MEMCACHED_VERSION=1.6.14
# Thu, 17 Mar 2022 12:51:35 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Thu, 17 Mar 2022 12:55:35 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Thu, 17 Mar 2022 12:55:35 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 17 Mar 2022 12:55:36 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 17 Mar 2022 12:55:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Mar 2022 12:55:36 GMT
USER memcache
# Thu, 17 Mar 2022 12:55:36 GMT
EXPOSE 11211
# Thu, 17 Mar 2022 12:55:36 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:3d243047344378e9b7136d552d48feb7ea8b6fe14ce0990e0cc011d5e369626a`  
		Last Modified: Thu, 17 Mar 2022 04:02:41 GMT  
		Size: 2.8 MB (2812636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e26b137db66bd985a8103e3e70f8985eafa9a9ca3dc6aa33344245535f6a6b0`  
		Last Modified: Thu, 17 Mar 2022 12:56:25 GMT  
		Size: 1.3 KB (1263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5231e0cae31bc5e59bdcb40f696ceaa6b5cad70b9500bc5bfd459174ac1f78dd`  
		Last Modified: Thu, 17 Mar 2022 12:56:25 GMT  
		Size: 109.3 KB (109285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d9fab8e58febfe6f0bfb8d5bdc098221b6348a6128014c4c2b4d4086284696d`  
		Last Modified: Thu, 17 Mar 2022 12:56:25 GMT  
		Size: 938.9 KB (938943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9ca16ee180425777e36c6f23ab6755a192eedf107400360aac9332686f1212b`  
		Last Modified: Thu, 17 Mar 2022 12:56:25 GMT  
		Size: 280.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f81d444d82a8e26057630fab59b6bdb890fe42afa50edabbba60d8685e88d639`  
		Last Modified: Thu, 17 Mar 2022 12:56:24 GMT  
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
$ docker pull memcached@sha256:095e0c44c122b636ae053f2971bb454b3edfe210195707983a9e0a38d22f4411
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3754561 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d01922b70bc4d8d1d2be9eabafa82a0f0152a88e5871b7e9b6949cf1327c9c4f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 17 Mar 2022 03:19:52 GMT
ADD file:cd7d91362950471ca4678cf3833dc47119ab519dea51424c847bbbb21e1649d4 in / 
# Thu, 17 Mar 2022 03:19:52 GMT
CMD ["/bin/sh"]
# Thu, 17 Mar 2022 11:39:00 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Thu, 17 Mar 2022 11:39:02 GMT
RUN apk add --no-cache libsasl
# Thu, 17 Mar 2022 11:39:03 GMT
ENV MEMCACHED_VERSION=1.6.14
# Thu, 17 Mar 2022 11:39:04 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Thu, 17 Mar 2022 11:41:43 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Thu, 17 Mar 2022 11:41:45 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 17 Mar 2022 11:41:45 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 17 Mar 2022 11:41:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Mar 2022 11:41:47 GMT
USER memcache
# Thu, 17 Mar 2022 11:41:48 GMT
EXPOSE 11211
# Thu, 17 Mar 2022 11:41:49 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:148d739a8e6b9342daa1f5b428d3a3c6118f340f21df28c16e06f918ef150147`  
		Last Modified: Thu, 17 Mar 2022 03:20:45 GMT  
		Size: 2.7 MB (2714807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33dde588ab12fbb6aa46070a960ac850c8347e86f29744b40a123a466d4885ab`  
		Last Modified: Thu, 17 Mar 2022 11:42:57 GMT  
		Size: 1.2 KB (1240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bdeb7ac9fd9c67010a55bf3fe0e13866bb31d847353f455c95220027e2bc48c`  
		Last Modified: Thu, 17 Mar 2022 11:42:58 GMT  
		Size: 110.6 KB (110556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6bf3828467e4d3c16fcdc94bf5987db023e892ef9594c9c5dc2c3ccf07bc4bc`  
		Last Modified: Thu, 17 Mar 2022 11:42:58 GMT  
		Size: 927.5 KB (927550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d39e5be11e10e43e4991c6d85f4bdce89416e75c908d33656e4dcb79c26a51bc`  
		Last Modified: Thu, 17 Mar 2022 11:42:57 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9404edf07c113d954a0a5c34650b52d9a1f8e57d166b3e1b022a82c3e27e724`  
		Last Modified: Thu, 17 Mar 2022 11:42:57 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-alpine` - linux; 386

```console
$ docker pull memcached@sha256:8a6352e717a8080f0c0888560cf7ae52c77ee2cbd10ed46c68822370b5188d0f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3891706 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4db903b8d549ba5f131fc35c81b69bdf1822950956033492f126e16dd95b5750`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 17 Mar 2022 08:13:03 GMT
ADD file:22216bc654d9177244235f242fa83cae3b283b3c145cad7ccf11c0d29f5f0ff2 in / 
# Thu, 17 Mar 2022 08:13:03 GMT
CMD ["/bin/sh"]
# Thu, 17 Mar 2022 17:35:31 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Thu, 17 Mar 2022 17:35:32 GMT
RUN apk add --no-cache libsasl
# Thu, 17 Mar 2022 17:35:32 GMT
ENV MEMCACHED_VERSION=1.6.14
# Thu, 17 Mar 2022 17:35:33 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Thu, 17 Mar 2022 17:39:25 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Thu, 17 Mar 2022 17:39:25 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 17 Mar 2022 17:39:26 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 17 Mar 2022 17:39:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Mar 2022 17:39:26 GMT
USER memcache
# Thu, 17 Mar 2022 17:39:26 GMT
EXPOSE 11211
# Thu, 17 Mar 2022 17:39:26 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:93317a1f65ec94b67aefe728a598022610246404e3a68d391c76cd0e5244a2a0`  
		Last Modified: Thu, 17 Mar 2022 08:13:56 GMT  
		Size: 2.8 MB (2821789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae4d8e906564040308eb9f4b96b3808d37aa02b7fffa8e8d5c80126d5e50b1cf`  
		Last Modified: Thu, 17 Mar 2022 17:40:52 GMT  
		Size: 1.3 KB (1263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16143ebb273f49cf3884d5a063dfac8b30d9527c5018e90fac51ac381b5a5f8b`  
		Last Modified: Thu, 17 Mar 2022 17:40:52 GMT  
		Size: 121.2 KB (121183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:107340d48cdbc30d4b57291ca0d28997feed13517f3a508b3b398620dbc97099`  
		Last Modified: Thu, 17 Mar 2022 17:40:52 GMT  
		Size: 947.1 KB (947068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a791ada3ee704cad0a4dba90d29f533e6fcadb132c2522c38b4f0680201a86a9`  
		Last Modified: Thu, 17 Mar 2022 17:40:52 GMT  
		Size: 282.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fc23e842aa74aed8a4ea48cf2b6f027f9592e43e117c394bc70b3d2dcf0627c`  
		Last Modified: Thu, 17 Mar 2022 17:40:53 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-alpine` - linux; ppc64le

```console
$ docker pull memcached@sha256:75cb5141098fb02bb0c554c31c00d28802b414593a6b41d430c10505ee943fe0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.3 MB (5315837 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4be74852968716dd05ad711f1cda531afac5b782fe0dd6692e5aed7d91d54466`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 24 Nov 2021 20:20:16 GMT
ADD file:57115dca2eb707f46b6301e75174e6aa316fb02ac28643b91429b75be51bd8c8 in / 
# Wed, 24 Nov 2021 20:20:20 GMT
CMD ["/bin/sh"]
# Tue, 30 Nov 2021 00:52:13 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 30 Nov 2021 00:52:18 GMT
RUN apk add --no-cache libsasl
# Fri, 11 Feb 2022 23:54:02 GMT
ENV MEMCACHED_VERSION=1.6.14
# Fri, 11 Feb 2022 23:54:06 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Fri, 11 Feb 2022 23:57:48 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Fri, 11 Feb 2022 23:57:50 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 11 Feb 2022 23:57:55 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 11 Feb 2022 23:57:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Feb 2022 23:57:59 GMT
USER memcache
# Fri, 11 Feb 2022 23:58:01 GMT
EXPOSE 11211
# Fri, 11 Feb 2022 23:58:02 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:159b5dcb1717c815c76ff5ea1db730e18e8609c9090238e43282856db9e71f47`  
		Last Modified: Wed, 24 Nov 2021 20:21:14 GMT  
		Size: 2.8 MB (2814780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f44bb0dc5dc6d3634512266fffaecf643a467ef890e0a60fa7daed8a8f379335`  
		Last Modified: Tue, 30 Nov 2021 00:57:03 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:242bba95e896195e2c48210499ed8dad5c07a25a93e0d6304a787f4d5f05bb79`  
		Last Modified: Tue, 30 Nov 2021 00:57:03 GMT  
		Size: 126.2 KB (126210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9d933f0d59015113f25123de9b3460a03fdf091181f4c9330b1bb42c27a8cce`  
		Last Modified: Fri, 11 Feb 2022 23:59:16 GMT  
		Size: 2.4 MB (2373175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:659fd1f60c2bc05966f606e677370eeee3176f7d6dbd530b3f271ba313f8b0fe`  
		Last Modified: Fri, 11 Feb 2022 23:59:15 GMT  
		Size: 282.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8d9d86e7310ff252ce602224ce1643c6b8d50713444e43804cdb93912f89087`  
		Last Modified: Fri, 11 Feb 2022 23:59:15 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-alpine` - linux; s390x

```console
$ docker pull memcached@sha256:5a931719c887b04ccf389c14867075cca4a76c774ecceb8231f801d876c94be9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.7 MB (3651372 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8aed3255f32676856491e1f6e999893205a57c1d26f36d52518c7d72433bcd9c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 17 Mar 2022 03:04:28 GMT
ADD file:f623c69acb1859b41ef29e8f20f4e6c7072d9c6d7210d745afc615251bfe418f in / 
# Thu, 17 Mar 2022 03:04:28 GMT
CMD ["/bin/sh"]
# Thu, 17 Mar 2022 08:51:10 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Thu, 17 Mar 2022 08:51:11 GMT
RUN apk add --no-cache libsasl
# Thu, 17 Mar 2022 08:51:12 GMT
ENV MEMCACHED_VERSION=1.6.14
# Thu, 17 Mar 2022 08:51:12 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Thu, 17 Mar 2022 08:54:42 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Thu, 17 Mar 2022 08:54:42 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 17 Mar 2022 08:54:43 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 17 Mar 2022 08:54:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Mar 2022 08:54:43 GMT
USER memcache
# Thu, 17 Mar 2022 08:54:44 GMT
EXPOSE 11211
# Thu, 17 Mar 2022 08:54:44 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:d51040c5bfbf434887bfed2557335a411e6ef760d04cc178d455d1c3ec1b721c`  
		Last Modified: Thu, 17 Mar 2022 03:05:26 GMT  
		Size: 2.6 MB (2601715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bafa61f6f0948b111a53b71e2c8c1312981357779ca88eaf5e60d4163dc7d03b`  
		Last Modified: Thu, 17 Mar 2022 08:55:51 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6282933aed68188fd9995db64b18a466643f4879e98a97392e6df0309f825ab`  
		Last Modified: Thu, 17 Mar 2022 08:55:51 GMT  
		Size: 113.8 KB (113794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d266558ba8144540d874cf2a04b80cdad0b98138893dbd2bf8dfc0a82587d0fc`  
		Last Modified: Thu, 17 Mar 2022 08:55:51 GMT  
		Size: 934.2 KB (934189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e97cc0f7d043b7a30a2ecd4a02847ed3d1227cdec67c577b9486ae3a40bb7f55`  
		Last Modified: Thu, 17 Mar 2022 08:55:51 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:973434578ea89c81d5ee8f8c926d6efab348a190b4d1f8c59c32b595e5e3ff14`  
		Last Modified: Thu, 17 Mar 2022 08:55:51 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:1.6-alpine3.15`

```console
$ docker pull memcached@sha256:614ca36d9fbc4953da3276766de5e77bdac23c04ffcde331032be6d854006131
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
$ docker pull memcached@sha256:fd1bb2a04baff1bc63d2323d91a4f7135b9f06f1d0294fbe13b8660db7b6dd78
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3862528 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e9d7d65a6545e2698d88de0e6c6eeb620a5bdf19e35635a36ac252bb7dce9d55`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 17 Mar 2022 04:01:58 GMT
ADD file:cf4b631a115c2bbfbd81cad2d3041bceb64a8136aac92ba8a63b6c51d60af764 in / 
# Thu, 17 Mar 2022 04:01:59 GMT
CMD ["/bin/sh"]
# Thu, 17 Mar 2022 12:51:33 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Thu, 17 Mar 2022 12:51:34 GMT
RUN apk add --no-cache libsasl
# Thu, 17 Mar 2022 12:51:34 GMT
ENV MEMCACHED_VERSION=1.6.14
# Thu, 17 Mar 2022 12:51:35 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Thu, 17 Mar 2022 12:55:35 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Thu, 17 Mar 2022 12:55:35 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 17 Mar 2022 12:55:36 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 17 Mar 2022 12:55:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Mar 2022 12:55:36 GMT
USER memcache
# Thu, 17 Mar 2022 12:55:36 GMT
EXPOSE 11211
# Thu, 17 Mar 2022 12:55:36 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:3d243047344378e9b7136d552d48feb7ea8b6fe14ce0990e0cc011d5e369626a`  
		Last Modified: Thu, 17 Mar 2022 04:02:41 GMT  
		Size: 2.8 MB (2812636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e26b137db66bd985a8103e3e70f8985eafa9a9ca3dc6aa33344245535f6a6b0`  
		Last Modified: Thu, 17 Mar 2022 12:56:25 GMT  
		Size: 1.3 KB (1263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5231e0cae31bc5e59bdcb40f696ceaa6b5cad70b9500bc5bfd459174ac1f78dd`  
		Last Modified: Thu, 17 Mar 2022 12:56:25 GMT  
		Size: 109.3 KB (109285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d9fab8e58febfe6f0bfb8d5bdc098221b6348a6128014c4c2b4d4086284696d`  
		Last Modified: Thu, 17 Mar 2022 12:56:25 GMT  
		Size: 938.9 KB (938943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9ca16ee180425777e36c6f23ab6755a192eedf107400360aac9332686f1212b`  
		Last Modified: Thu, 17 Mar 2022 12:56:25 GMT  
		Size: 280.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f81d444d82a8e26057630fab59b6bdb890fe42afa50edabbba60d8685e88d639`  
		Last Modified: Thu, 17 Mar 2022 12:56:24 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-alpine3.15` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:095e0c44c122b636ae053f2971bb454b3edfe210195707983a9e0a38d22f4411
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3754561 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d01922b70bc4d8d1d2be9eabafa82a0f0152a88e5871b7e9b6949cf1327c9c4f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 17 Mar 2022 03:19:52 GMT
ADD file:cd7d91362950471ca4678cf3833dc47119ab519dea51424c847bbbb21e1649d4 in / 
# Thu, 17 Mar 2022 03:19:52 GMT
CMD ["/bin/sh"]
# Thu, 17 Mar 2022 11:39:00 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Thu, 17 Mar 2022 11:39:02 GMT
RUN apk add --no-cache libsasl
# Thu, 17 Mar 2022 11:39:03 GMT
ENV MEMCACHED_VERSION=1.6.14
# Thu, 17 Mar 2022 11:39:04 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Thu, 17 Mar 2022 11:41:43 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Thu, 17 Mar 2022 11:41:45 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 17 Mar 2022 11:41:45 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 17 Mar 2022 11:41:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Mar 2022 11:41:47 GMT
USER memcache
# Thu, 17 Mar 2022 11:41:48 GMT
EXPOSE 11211
# Thu, 17 Mar 2022 11:41:49 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:148d739a8e6b9342daa1f5b428d3a3c6118f340f21df28c16e06f918ef150147`  
		Last Modified: Thu, 17 Mar 2022 03:20:45 GMT  
		Size: 2.7 MB (2714807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33dde588ab12fbb6aa46070a960ac850c8347e86f29744b40a123a466d4885ab`  
		Last Modified: Thu, 17 Mar 2022 11:42:57 GMT  
		Size: 1.2 KB (1240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bdeb7ac9fd9c67010a55bf3fe0e13866bb31d847353f455c95220027e2bc48c`  
		Last Modified: Thu, 17 Mar 2022 11:42:58 GMT  
		Size: 110.6 KB (110556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6bf3828467e4d3c16fcdc94bf5987db023e892ef9594c9c5dc2c3ccf07bc4bc`  
		Last Modified: Thu, 17 Mar 2022 11:42:58 GMT  
		Size: 927.5 KB (927550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d39e5be11e10e43e4991c6d85f4bdce89416e75c908d33656e4dcb79c26a51bc`  
		Last Modified: Thu, 17 Mar 2022 11:42:57 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9404edf07c113d954a0a5c34650b52d9a1f8e57d166b3e1b022a82c3e27e724`  
		Last Modified: Thu, 17 Mar 2022 11:42:57 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-alpine3.15` - linux; 386

```console
$ docker pull memcached@sha256:8a6352e717a8080f0c0888560cf7ae52c77ee2cbd10ed46c68822370b5188d0f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3891706 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4db903b8d549ba5f131fc35c81b69bdf1822950956033492f126e16dd95b5750`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 17 Mar 2022 08:13:03 GMT
ADD file:22216bc654d9177244235f242fa83cae3b283b3c145cad7ccf11c0d29f5f0ff2 in / 
# Thu, 17 Mar 2022 08:13:03 GMT
CMD ["/bin/sh"]
# Thu, 17 Mar 2022 17:35:31 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Thu, 17 Mar 2022 17:35:32 GMT
RUN apk add --no-cache libsasl
# Thu, 17 Mar 2022 17:35:32 GMT
ENV MEMCACHED_VERSION=1.6.14
# Thu, 17 Mar 2022 17:35:33 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Thu, 17 Mar 2022 17:39:25 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Thu, 17 Mar 2022 17:39:25 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 17 Mar 2022 17:39:26 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 17 Mar 2022 17:39:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Mar 2022 17:39:26 GMT
USER memcache
# Thu, 17 Mar 2022 17:39:26 GMT
EXPOSE 11211
# Thu, 17 Mar 2022 17:39:26 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:93317a1f65ec94b67aefe728a598022610246404e3a68d391c76cd0e5244a2a0`  
		Last Modified: Thu, 17 Mar 2022 08:13:56 GMT  
		Size: 2.8 MB (2821789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae4d8e906564040308eb9f4b96b3808d37aa02b7fffa8e8d5c80126d5e50b1cf`  
		Last Modified: Thu, 17 Mar 2022 17:40:52 GMT  
		Size: 1.3 KB (1263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16143ebb273f49cf3884d5a063dfac8b30d9527c5018e90fac51ac381b5a5f8b`  
		Last Modified: Thu, 17 Mar 2022 17:40:52 GMT  
		Size: 121.2 KB (121183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:107340d48cdbc30d4b57291ca0d28997feed13517f3a508b3b398620dbc97099`  
		Last Modified: Thu, 17 Mar 2022 17:40:52 GMT  
		Size: 947.1 KB (947068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a791ada3ee704cad0a4dba90d29f533e6fcadb132c2522c38b4f0680201a86a9`  
		Last Modified: Thu, 17 Mar 2022 17:40:52 GMT  
		Size: 282.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fc23e842aa74aed8a4ea48cf2b6f027f9592e43e117c394bc70b3d2dcf0627c`  
		Last Modified: Thu, 17 Mar 2022 17:40:53 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-alpine3.15` - linux; ppc64le

```console
$ docker pull memcached@sha256:75cb5141098fb02bb0c554c31c00d28802b414593a6b41d430c10505ee943fe0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.3 MB (5315837 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4be74852968716dd05ad711f1cda531afac5b782fe0dd6692e5aed7d91d54466`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 24 Nov 2021 20:20:16 GMT
ADD file:57115dca2eb707f46b6301e75174e6aa316fb02ac28643b91429b75be51bd8c8 in / 
# Wed, 24 Nov 2021 20:20:20 GMT
CMD ["/bin/sh"]
# Tue, 30 Nov 2021 00:52:13 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 30 Nov 2021 00:52:18 GMT
RUN apk add --no-cache libsasl
# Fri, 11 Feb 2022 23:54:02 GMT
ENV MEMCACHED_VERSION=1.6.14
# Fri, 11 Feb 2022 23:54:06 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Fri, 11 Feb 2022 23:57:48 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Fri, 11 Feb 2022 23:57:50 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 11 Feb 2022 23:57:55 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 11 Feb 2022 23:57:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Feb 2022 23:57:59 GMT
USER memcache
# Fri, 11 Feb 2022 23:58:01 GMT
EXPOSE 11211
# Fri, 11 Feb 2022 23:58:02 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:159b5dcb1717c815c76ff5ea1db730e18e8609c9090238e43282856db9e71f47`  
		Last Modified: Wed, 24 Nov 2021 20:21:14 GMT  
		Size: 2.8 MB (2814780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f44bb0dc5dc6d3634512266fffaecf643a467ef890e0a60fa7daed8a8f379335`  
		Last Modified: Tue, 30 Nov 2021 00:57:03 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:242bba95e896195e2c48210499ed8dad5c07a25a93e0d6304a787f4d5f05bb79`  
		Last Modified: Tue, 30 Nov 2021 00:57:03 GMT  
		Size: 126.2 KB (126210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9d933f0d59015113f25123de9b3460a03fdf091181f4c9330b1bb42c27a8cce`  
		Last Modified: Fri, 11 Feb 2022 23:59:16 GMT  
		Size: 2.4 MB (2373175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:659fd1f60c2bc05966f606e677370eeee3176f7d6dbd530b3f271ba313f8b0fe`  
		Last Modified: Fri, 11 Feb 2022 23:59:15 GMT  
		Size: 282.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8d9d86e7310ff252ce602224ce1643c6b8d50713444e43804cdb93912f89087`  
		Last Modified: Fri, 11 Feb 2022 23:59:15 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-alpine3.15` - linux; s390x

```console
$ docker pull memcached@sha256:5a931719c887b04ccf389c14867075cca4a76c774ecceb8231f801d876c94be9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.7 MB (3651372 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8aed3255f32676856491e1f6e999893205a57c1d26f36d52518c7d72433bcd9c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 17 Mar 2022 03:04:28 GMT
ADD file:f623c69acb1859b41ef29e8f20f4e6c7072d9c6d7210d745afc615251bfe418f in / 
# Thu, 17 Mar 2022 03:04:28 GMT
CMD ["/bin/sh"]
# Thu, 17 Mar 2022 08:51:10 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Thu, 17 Mar 2022 08:51:11 GMT
RUN apk add --no-cache libsasl
# Thu, 17 Mar 2022 08:51:12 GMT
ENV MEMCACHED_VERSION=1.6.14
# Thu, 17 Mar 2022 08:51:12 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Thu, 17 Mar 2022 08:54:42 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Thu, 17 Mar 2022 08:54:42 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 17 Mar 2022 08:54:43 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 17 Mar 2022 08:54:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Mar 2022 08:54:43 GMT
USER memcache
# Thu, 17 Mar 2022 08:54:44 GMT
EXPOSE 11211
# Thu, 17 Mar 2022 08:54:44 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:d51040c5bfbf434887bfed2557335a411e6ef760d04cc178d455d1c3ec1b721c`  
		Last Modified: Thu, 17 Mar 2022 03:05:26 GMT  
		Size: 2.6 MB (2601715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bafa61f6f0948b111a53b71e2c8c1312981357779ca88eaf5e60d4163dc7d03b`  
		Last Modified: Thu, 17 Mar 2022 08:55:51 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6282933aed68188fd9995db64b18a466643f4879e98a97392e6df0309f825ab`  
		Last Modified: Thu, 17 Mar 2022 08:55:51 GMT  
		Size: 113.8 KB (113794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d266558ba8144540d874cf2a04b80cdad0b98138893dbd2bf8dfc0a82587d0fc`  
		Last Modified: Thu, 17 Mar 2022 08:55:51 GMT  
		Size: 934.2 KB (934189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e97cc0f7d043b7a30a2ecd4a02847ed3d1227cdec67c577b9486ae3a40bb7f55`  
		Last Modified: Thu, 17 Mar 2022 08:55:51 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:973434578ea89c81d5ee8f8c926d6efab348a190b4d1f8c59c32b595e5e3ff14`  
		Last Modified: Thu, 17 Mar 2022 08:55:51 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:1.6-bullseye`

```console
$ docker pull memcached@sha256:67ceec1841427583fd33842be1a41243351997c4803d05c14f95f0c8c6826f93
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
$ docker pull memcached@sha256:6a51dd2e23a3ead43158d3255ab8c2d9b0b2f0432becf5814c267273c84e8b6a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.0 MB (32965129 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e897df046b27f4dbfae44d31346ef91c2160a46c1b8d5bf652a40e3d76d3914f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 17 Mar 2022 04:03:59 GMT
ADD file:36919ae6bb25e3269eff949443129a01a8a43fb967fe6563939ebe1e1e9b8228 in / 
# Thu, 17 Mar 2022 04:03:59 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 12:47:26 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Thu, 17 Mar 2022 12:47:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Mar 2022 12:47:29 GMT
ENV MEMCACHED_VERSION=1.6.14
# Thu, 17 Mar 2022 12:47:29 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Thu, 17 Mar 2022 12:51:18 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 17 Mar 2022 12:51:18 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 17 Mar 2022 12:51:18 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 17 Mar 2022 12:51:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Mar 2022 12:51:18 GMT
USER memcache
# Thu, 17 Mar 2022 12:51:19 GMT
EXPOSE 11211
# Thu, 17 Mar 2022 12:51:19 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:ae13dd57832654086618a81dbc128846aa092489260c326ee95429b63c3cf213`  
		Last Modified: Thu, 17 Mar 2022 04:10:05 GMT  
		Size: 31.4 MB (31376572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c39e8a8db385456589d2009379dedc9787a9297b0ea679ff564500de9894d325`  
		Last Modified: Thu, 17 Mar 2022 12:55:59 GMT  
		Size: 5.0 KB (4982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fa3e9def276e8e73128ec9d08c6f139621666d0724b33d882ca0943a1a6825b`  
		Last Modified: Thu, 17 Mar 2022 12:55:59 GMT  
		Size: 328.0 KB (328046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9835681ca994d84f0de3da2d9ed0cdb5882c06b58bccdc406102bf4bf8a55700`  
		Last Modified: Thu, 17 Mar 2022 12:55:59 GMT  
		Size: 1.3 MB (1255121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d362d7003189fa875ec372df3c4c9622f2688adb7ed5c9cb2bec35c31b9d523`  
		Last Modified: Thu, 17 Mar 2022 12:55:59 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bd4550226c671e2d98eac87073171c925eebaa0e039ed5e2610d516980dd220`  
		Last Modified: Thu, 17 Mar 2022 12:55:59 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-bullseye` - linux; arm variant v5

```console
$ docker pull memcached@sha256:084a4198172362acf346afa27655123636800a135bdaaa857d8d57e7e402c4fa
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.5 MB (30467908 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b9e543544c3f8ef04ec918e92a8e98602cbdc37970011b5960685ffd0103780`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 17 Mar 2022 05:19:45 GMT
ADD file:1eb4f937d40230354e20e28ed781234acd4be2b0dab72f87131a3eac66349719 in / 
# Thu, 17 Mar 2022 05:19:46 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 10:06:48 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Thu, 17 Mar 2022 10:06:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Mar 2022 10:07:00 GMT
ENV MEMCACHED_VERSION=1.6.14
# Thu, 17 Mar 2022 10:07:00 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Thu, 17 Mar 2022 10:11:18 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 17 Mar 2022 10:11:18 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 17 Mar 2022 10:11:20 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 17 Mar 2022 10:11:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Mar 2022 10:11:21 GMT
USER memcache
# Thu, 17 Mar 2022 10:11:21 GMT
EXPOSE 11211
# Thu, 17 Mar 2022 10:11:21 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:4da455e7774c0e977d862a56ab6d85f33ce5dd5a77d45a0a74a272e9eae6bea0`  
		Last Modified: Thu, 17 Mar 2022 05:35:01 GMT  
		Size: 28.9 MB (28919702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39450ea3e36758cb1aaf29a3e4a3694a4f1e5d208ece3da6479b6dcd47705309`  
		Last Modified: Thu, 17 Mar 2022 10:12:14 GMT  
		Size: 4.9 KB (4890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b674f1fc0977777c240d7af9fa6d57e8b24d5332791547c80820aa9d1956d037`  
		Last Modified: Thu, 17 Mar 2022 10:12:14 GMT  
		Size: 316.6 KB (316575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de44c6f01b62d4d56baa2601e6706305eaf35c2da9541623a8c94c7fe1e4b8b2`  
		Last Modified: Thu, 17 Mar 2022 10:12:14 GMT  
		Size: 1.2 MB (1226335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18229473d3cfa938b3ba5d7f36b228bc60b7641660ae3242b56e210a50892b0f`  
		Last Modified: Thu, 17 Mar 2022 10:12:14 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e231e6a0756abb2590d1ef0507c610f0aa1b4f42e40a895d310b330662a98a2`  
		Last Modified: Thu, 17 Mar 2022 10:12:14 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-bullseye` - linux; arm variant v7

```console
$ docker pull memcached@sha256:9fe6c86dfef8c0cf535d443045364d887fd0bc8b44f550a8cbb0dca64e33e732
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.1 MB (28090226 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14dc9d69afed7832780e59eca9bf08aecbca59e357a3c301648a665b42b6659a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 17 Mar 2022 09:31:03 GMT
ADD file:e52f9ee2dc3144d7b9eb3ec90c106aa2a094eb4c5c2aa8cbff5c520a5faaef43 in / 
# Thu, 17 Mar 2022 09:31:04 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 21:53:04 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Thu, 17 Mar 2022 21:53:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Mar 2022 21:53:14 GMT
ENV MEMCACHED_VERSION=1.6.14
# Thu, 17 Mar 2022 21:53:14 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Thu, 17 Mar 2022 21:57:21 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 17 Mar 2022 21:57:22 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 17 Mar 2022 21:57:23 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 17 Mar 2022 21:57:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Mar 2022 21:57:24 GMT
USER memcache
# Thu, 17 Mar 2022 21:57:25 GMT
EXPOSE 11211
# Thu, 17 Mar 2022 21:57:25 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:5e5e708ee1f9fdbc69324391f7d1f816c657e6116eff09e7d2247fa9de3a076a`  
		Last Modified: Thu, 17 Mar 2022 09:46:33 GMT  
		Size: 26.6 MB (26575097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f652a8bcf3f50c242f3e27b3792cd55f9c0436702fe2bcdd4ae3df203aa84100`  
		Last Modified: Thu, 17 Mar 2022 22:10:19 GMT  
		Size: 4.9 KB (4896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c1be80f12d4f19157864e18689a8dd9c0f84c3a6c929949b066e7c29f30c5d7`  
		Last Modified: Thu, 17 Mar 2022 22:10:19 GMT  
		Size: 312.0 KB (311999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37ab28ddd02c6ca7832dec8a6b6508e8e4d95b34c8f4fe17457a1844c4442a7a`  
		Last Modified: Thu, 17 Mar 2022 22:10:19 GMT  
		Size: 1.2 MB (1197826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6d7e30c2d27f64a3117e85e87c00c1d4e79aa91e0bf4e4552c68d4710592d64`  
		Last Modified: Thu, 17 Mar 2022 22:10:19 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7f72f97159e0cf88a536b1a268d9bfa7af992046ce641dddb6710eabf7d08e4`  
		Last Modified: Thu, 17 Mar 2022 22:10:19 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-bullseye` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:773c0f8c11aa82d0bf14e751ab65784b8993bd7477026d660eb8e970b160aad8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.4 MB (31441503 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1cc644adcd708fa1761227654eacbdd25163b6a5a399599e20c7eabdc2a24a8f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 17 Mar 2022 03:21:57 GMT
ADD file:e52e032f1ace6abd44b3647d43c1b8ae30bac6de804eef09c6ccd793057996fd in / 
# Thu, 17 Mar 2022 03:21:58 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 11:35:48 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Thu, 17 Mar 2022 11:35:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Mar 2022 11:35:52 GMT
ENV MEMCACHED_VERSION=1.6.14
# Thu, 17 Mar 2022 11:35:53 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Thu, 17 Mar 2022 11:38:38 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 17 Mar 2022 11:38:40 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 17 Mar 2022 11:38:40 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 17 Mar 2022 11:38:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Mar 2022 11:38:42 GMT
USER memcache
# Thu, 17 Mar 2022 11:38:43 GMT
EXPOSE 11211
# Thu, 17 Mar 2022 11:38:44 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:32252aec0777ac025a158bc2a8317650a4f2a0a875387011b1165013874f8723`  
		Last Modified: Thu, 17 Mar 2022 03:28:36 GMT  
		Size: 30.1 MB (30063013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:966f1b38b9d3f62f875f8dbd868ecc80c2037b45aadbec50fc16d292be747303`  
		Last Modified: Thu, 17 Mar 2022 11:42:26 GMT  
		Size: 4.9 KB (4903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2898c9abf66c159176811eff24e689c0989d4e7c025c9a7eb0f933d356aec11`  
		Last Modified: Thu, 17 Mar 2022 11:42:26 GMT  
		Size: 119.2 KB (119181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d331819fcfc0b6541dc90aafde95bc8b8a88e453cb3800c977716cff65961a77`  
		Last Modified: Thu, 17 Mar 2022 11:42:26 GMT  
		Size: 1.3 MB (1254002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25a25819b974fbc38bad380c4df00bf1f032cf4eb0112a109c78f9858d9a0a55`  
		Last Modified: Thu, 17 Mar 2022 11:42:26 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7c790b93b28eb9ed542eac0eaf8c5fe2d4c5daa368b0f27bac067fd01bee280`  
		Last Modified: Thu, 17 Mar 2022 11:42:26 GMT  
		Size: 118.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-bullseye` - linux; 386

```console
$ docker pull memcached@sha256:3d0458851092782bb1cfb8fdb3edb27fe63775c3fb68f1879137e691de184e82
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.0 MB (33981668 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b7d3a232500fae88433d6e4117fa6e45b0ed4c529c925734eb2982bf3a3ee54`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 17 Mar 2022 08:15:53 GMT
ADD file:2d6be3846f0e5fabd85bc9409b1e2223cad4c57c76f96e9f81489ba78a72a1f5 in / 
# Thu, 17 Mar 2022 08:15:54 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 17:31:22 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Thu, 17 Mar 2022 17:31:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Mar 2022 17:31:26 GMT
ENV MEMCACHED_VERSION=1.6.14
# Thu, 17 Mar 2022 17:31:26 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Thu, 17 Mar 2022 17:35:17 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 17 Mar 2022 17:35:17 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 17 Mar 2022 17:35:18 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 17 Mar 2022 17:35:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Mar 2022 17:35:18 GMT
USER memcache
# Thu, 17 Mar 2022 17:35:18 GMT
EXPOSE 11211
# Thu, 17 Mar 2022 17:35:18 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:176085117cac9b2cf2cf57b3a10c9811dbd2773497fbac3086b5024070447e97`  
		Last Modified: Thu, 17 Mar 2022 08:24:00 GMT  
		Size: 32.4 MB (32386475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe18ed3f6ff50e5b12a7db917c34de3104619ae31e84d9d83ad2d94a3b8c5822`  
		Last Modified: Thu, 17 Mar 2022 17:40:19 GMT  
		Size: 4.9 KB (4896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc15fd9e0c057bb0a0d077f6c21d0b980b6ec5f9e5292c19d6fd790731f7bfc6`  
		Last Modified: Thu, 17 Mar 2022 17:40:19 GMT  
		Size: 336.6 KB (336638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1f8475d0ca14b4624de06fbe3207cdf07b5c31573192d0acc9b1e600b90c430`  
		Last Modified: Thu, 17 Mar 2022 17:40:20 GMT  
		Size: 1.3 MB (1253253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61e85d2ca17a8c6eb12e9cdc031a20d5c2357cf22bc4ad5353d520e13f60b73a`  
		Last Modified: Thu, 17 Mar 2022 17:40:19 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3194d39d810076bc29397aa1a117ac51d7bc610ffb9b7c90613fdf21203b05a3`  
		Last Modified: Thu, 17 Mar 2022 17:40:19 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-bullseye` - linux; mips64le

```console
$ docker pull memcached@sha256:9148cd77f369a80c3b52dd4f79ddd8073c192da135e99a311f54641a851b4b60
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.0 MB (31012937 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:16b4bbcf6270bfbe61ccbb8083bf46151a57eb6a74f044b2004509978709ee0d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 17 Mar 2022 08:53:04 GMT
ADD file:795ac4eba576bc4c995df2a18b10ce802ee8a05417cdc53f5aa09452ecf2e832 in / 
# Thu, 17 Mar 2022 08:53:08 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 20:37:19 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Thu, 17 Mar 2022 20:37:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Mar 2022 20:37:40 GMT
ENV MEMCACHED_VERSION=1.6.14
# Thu, 17 Mar 2022 20:37:43 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Thu, 17 Mar 2022 20:44:58 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 17 Mar 2022 20:45:00 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 17 Mar 2022 20:45:05 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 17 Mar 2022 20:45:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Mar 2022 20:45:10 GMT
USER memcache
# Thu, 17 Mar 2022 20:45:13 GMT
EXPOSE 11211
# Thu, 17 Mar 2022 20:45:15 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:4799d88734ae94287a665c0e14621a744706cfbe17a0cf27ae9b0cc630927b11`  
		Last Modified: Thu, 17 Mar 2022 10:43:20 GMT  
		Size: 29.6 MB (29639810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a091b8fd61b3c0cafad5676908a202cec423a829bd2fb2bb79011b3ad5fd0845`  
		Last Modified: Thu, 17 Mar 2022 20:45:41 GMT  
		Size: 4.9 KB (4859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7644e6d2f727759be27279ab11b8f3e186b6918c1b3847badb0d04ae020286b`  
		Last Modified: Thu, 17 Mar 2022 20:45:41 GMT  
		Size: 117.1 KB (117098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47e8f3183abaf23ec67f322bc78981d3c838ad27bba488ec924c07d5b1a053a4`  
		Last Modified: Thu, 17 Mar 2022 20:45:41 GMT  
		Size: 1.3 MB (1250762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f0ac34ae7971e4442dd9abb2bbfa522fc4e65445f1ed51d33795cea9b37830e`  
		Last Modified: Thu, 17 Mar 2022 20:45:40 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0564ebbfe5b917d8a4818a435ddb35d5e4bbb4b4d7187189578f1c224d10ce2b`  
		Last Modified: Thu, 17 Mar 2022 20:45:40 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-bullseye` - linux; ppc64le

```console
$ docker pull memcached@sha256:4893f4daa742b31f414b08f98f8e7d0cbedaf63b8d88062bcf3c91a9522a2aab
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.0 MB (36957544 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8db953cc998ed06712eca57fe4ae2b8bb342ce991683fd7592495a21557d0940`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 26 Jan 2022 01:46:51 GMT
ADD file:c03f34c221e57fa5cb625c166d1db9f72d6ba2fa17a3c41a5d04d6875d098949 in / 
# Wed, 26 Jan 2022 01:46:57 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 05:38:39 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 26 Jan 2022 05:38:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 11 Feb 2022 23:47:36 GMT
ENV MEMCACHED_VERSION=1.6.14
# Fri, 11 Feb 2022 23:47:38 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Fri, 11 Feb 2022 23:53:07 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Fri, 11 Feb 2022 23:53:13 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 11 Feb 2022 23:53:34 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 11 Feb 2022 23:53:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Feb 2022 23:53:39 GMT
USER memcache
# Fri, 11 Feb 2022 23:53:41 GMT
EXPOSE 11211
# Fri, 11 Feb 2022 23:53:46 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:3149ee4a73508a4c39107d64a3fdc1b021626a22a0ac95e62fa0cea49ab77fba`  
		Last Modified: Wed, 26 Jan 2022 01:57:01 GMT  
		Size: 35.3 MB (35273030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07bcb451658eb6d9eace467c2e989d96e53c409eb48347a369e9ad80aadcfe96`  
		Last Modified: Wed, 26 Jan 2022 05:45:22 GMT  
		Size: 5.0 KB (4980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8807782e060aa90873de57b2d3ec277632145f166e9c1e3801c57eea7e595cc`  
		Last Modified: Wed, 26 Jan 2022 05:45:22 GMT  
		Size: 356.9 KB (356905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5f2e5d5bb1609e336a37e97218d618550ec5ce28384c32b1141393ef6f04a03`  
		Last Modified: Fri, 11 Feb 2022 23:58:44 GMT  
		Size: 1.3 MB (1322220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76e6da4f290b1cff2fa5b1ad17d42333c67179332511db4da3bd2c5ce12bbdfa`  
		Last Modified: Fri, 11 Feb 2022 23:58:44 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fb140c5468aa121999bc169d30e4ce6b73795cdf67aa21c1dfd3d1194dd0b82`  
		Last Modified: Fri, 11 Feb 2022 23:58:44 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-bullseye` - linux; s390x

```console
$ docker pull memcached@sha256:3e4437e519528ef8d3274dfc333f59f7c8c90099329a1e041fb6a71d5be8a1c5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.2 MB (31225911 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6fbcefffe918634bf299753ebcfe4a7284155e249686c5b5db9ffa92a5c0fc87`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 17 Mar 2022 03:06:58 GMT
ADD file:52f9267b4c57ac585a0d3d47a6f2ae1a71398264173ad4f190332957fa629c67 in / 
# Thu, 17 Mar 2022 03:07:01 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 08:47:34 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Thu, 17 Mar 2022 08:47:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Mar 2022 08:47:37 GMT
ENV MEMCACHED_VERSION=1.6.14
# Thu, 17 Mar 2022 08:47:37 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Thu, 17 Mar 2022 08:50:57 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 17 Mar 2022 08:50:57 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 17 Mar 2022 08:50:58 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 17 Mar 2022 08:50:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Mar 2022 08:50:58 GMT
USER memcache
# Thu, 17 Mar 2022 08:50:58 GMT
EXPOSE 11211
# Thu, 17 Mar 2022 08:50:59 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:d101968410e5005df630b0572aec03c88de55b8de81f3cf7e6a57e1ce2e5a8e5`  
		Last Modified: Thu, 17 Mar 2022 03:12:46 GMT  
		Size: 29.7 MB (29655795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1cad003ec39dc6e2e144c0953bad3bce3807fd1679d2c9e27e510724476e1e6`  
		Last Modified: Thu, 17 Mar 2022 08:55:34 GMT  
		Size: 5.0 KB (5022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13e61c306aebe51ff20adaf4ac683a69d93022d34ed4d09bc2ae7bde9d92ba52`  
		Last Modified: Thu, 17 Mar 2022 08:55:34 GMT  
		Size: 324.1 KB (324147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b5e88f796665ba79a22e6a541cbc3f30242e708c56d6b9af4fd0a7cd23abea6`  
		Last Modified: Thu, 17 Mar 2022 08:55:34 GMT  
		Size: 1.2 MB (1240539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77d35a1cb446cb01584cfbb3a61c40aaa1f358f37c8d723fe2437e6d070dbce3`  
		Last Modified: Thu, 17 Mar 2022 08:55:34 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b237b13dadf10fc593967f3714eaab56b7b00b89d435eb7e01be3f172b5b9b69`  
		Last Modified: Thu, 17 Mar 2022 08:55:33 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:1.6.14`

```console
$ docker pull memcached@sha256:67ceec1841427583fd33842be1a41243351997c4803d05c14f95f0c8c6826f93
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

### `memcached:1.6.14` - linux; amd64

```console
$ docker pull memcached@sha256:6a51dd2e23a3ead43158d3255ab8c2d9b0b2f0432becf5814c267273c84e8b6a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.0 MB (32965129 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e897df046b27f4dbfae44d31346ef91c2160a46c1b8d5bf652a40e3d76d3914f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 17 Mar 2022 04:03:59 GMT
ADD file:36919ae6bb25e3269eff949443129a01a8a43fb967fe6563939ebe1e1e9b8228 in / 
# Thu, 17 Mar 2022 04:03:59 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 12:47:26 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Thu, 17 Mar 2022 12:47:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Mar 2022 12:47:29 GMT
ENV MEMCACHED_VERSION=1.6.14
# Thu, 17 Mar 2022 12:47:29 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Thu, 17 Mar 2022 12:51:18 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 17 Mar 2022 12:51:18 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 17 Mar 2022 12:51:18 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 17 Mar 2022 12:51:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Mar 2022 12:51:18 GMT
USER memcache
# Thu, 17 Mar 2022 12:51:19 GMT
EXPOSE 11211
# Thu, 17 Mar 2022 12:51:19 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:ae13dd57832654086618a81dbc128846aa092489260c326ee95429b63c3cf213`  
		Last Modified: Thu, 17 Mar 2022 04:10:05 GMT  
		Size: 31.4 MB (31376572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c39e8a8db385456589d2009379dedc9787a9297b0ea679ff564500de9894d325`  
		Last Modified: Thu, 17 Mar 2022 12:55:59 GMT  
		Size: 5.0 KB (4982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fa3e9def276e8e73128ec9d08c6f139621666d0724b33d882ca0943a1a6825b`  
		Last Modified: Thu, 17 Mar 2022 12:55:59 GMT  
		Size: 328.0 KB (328046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9835681ca994d84f0de3da2d9ed0cdb5882c06b58bccdc406102bf4bf8a55700`  
		Last Modified: Thu, 17 Mar 2022 12:55:59 GMT  
		Size: 1.3 MB (1255121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d362d7003189fa875ec372df3c4c9622f2688adb7ed5c9cb2bec35c31b9d523`  
		Last Modified: Thu, 17 Mar 2022 12:55:59 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bd4550226c671e2d98eac87073171c925eebaa0e039ed5e2610d516980dd220`  
		Last Modified: Thu, 17 Mar 2022 12:55:59 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.14` - linux; arm variant v5

```console
$ docker pull memcached@sha256:084a4198172362acf346afa27655123636800a135bdaaa857d8d57e7e402c4fa
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.5 MB (30467908 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b9e543544c3f8ef04ec918e92a8e98602cbdc37970011b5960685ffd0103780`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 17 Mar 2022 05:19:45 GMT
ADD file:1eb4f937d40230354e20e28ed781234acd4be2b0dab72f87131a3eac66349719 in / 
# Thu, 17 Mar 2022 05:19:46 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 10:06:48 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Thu, 17 Mar 2022 10:06:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Mar 2022 10:07:00 GMT
ENV MEMCACHED_VERSION=1.6.14
# Thu, 17 Mar 2022 10:07:00 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Thu, 17 Mar 2022 10:11:18 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 17 Mar 2022 10:11:18 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 17 Mar 2022 10:11:20 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 17 Mar 2022 10:11:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Mar 2022 10:11:21 GMT
USER memcache
# Thu, 17 Mar 2022 10:11:21 GMT
EXPOSE 11211
# Thu, 17 Mar 2022 10:11:21 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:4da455e7774c0e977d862a56ab6d85f33ce5dd5a77d45a0a74a272e9eae6bea0`  
		Last Modified: Thu, 17 Mar 2022 05:35:01 GMT  
		Size: 28.9 MB (28919702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39450ea3e36758cb1aaf29a3e4a3694a4f1e5d208ece3da6479b6dcd47705309`  
		Last Modified: Thu, 17 Mar 2022 10:12:14 GMT  
		Size: 4.9 KB (4890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b674f1fc0977777c240d7af9fa6d57e8b24d5332791547c80820aa9d1956d037`  
		Last Modified: Thu, 17 Mar 2022 10:12:14 GMT  
		Size: 316.6 KB (316575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de44c6f01b62d4d56baa2601e6706305eaf35c2da9541623a8c94c7fe1e4b8b2`  
		Last Modified: Thu, 17 Mar 2022 10:12:14 GMT  
		Size: 1.2 MB (1226335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18229473d3cfa938b3ba5d7f36b228bc60b7641660ae3242b56e210a50892b0f`  
		Last Modified: Thu, 17 Mar 2022 10:12:14 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e231e6a0756abb2590d1ef0507c610f0aa1b4f42e40a895d310b330662a98a2`  
		Last Modified: Thu, 17 Mar 2022 10:12:14 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.14` - linux; arm variant v7

```console
$ docker pull memcached@sha256:9fe6c86dfef8c0cf535d443045364d887fd0bc8b44f550a8cbb0dca64e33e732
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.1 MB (28090226 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14dc9d69afed7832780e59eca9bf08aecbca59e357a3c301648a665b42b6659a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 17 Mar 2022 09:31:03 GMT
ADD file:e52f9ee2dc3144d7b9eb3ec90c106aa2a094eb4c5c2aa8cbff5c520a5faaef43 in / 
# Thu, 17 Mar 2022 09:31:04 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 21:53:04 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Thu, 17 Mar 2022 21:53:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Mar 2022 21:53:14 GMT
ENV MEMCACHED_VERSION=1.6.14
# Thu, 17 Mar 2022 21:53:14 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Thu, 17 Mar 2022 21:57:21 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 17 Mar 2022 21:57:22 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 17 Mar 2022 21:57:23 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 17 Mar 2022 21:57:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Mar 2022 21:57:24 GMT
USER memcache
# Thu, 17 Mar 2022 21:57:25 GMT
EXPOSE 11211
# Thu, 17 Mar 2022 21:57:25 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:5e5e708ee1f9fdbc69324391f7d1f816c657e6116eff09e7d2247fa9de3a076a`  
		Last Modified: Thu, 17 Mar 2022 09:46:33 GMT  
		Size: 26.6 MB (26575097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f652a8bcf3f50c242f3e27b3792cd55f9c0436702fe2bcdd4ae3df203aa84100`  
		Last Modified: Thu, 17 Mar 2022 22:10:19 GMT  
		Size: 4.9 KB (4896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c1be80f12d4f19157864e18689a8dd9c0f84c3a6c929949b066e7c29f30c5d7`  
		Last Modified: Thu, 17 Mar 2022 22:10:19 GMT  
		Size: 312.0 KB (311999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37ab28ddd02c6ca7832dec8a6b6508e8e4d95b34c8f4fe17457a1844c4442a7a`  
		Last Modified: Thu, 17 Mar 2022 22:10:19 GMT  
		Size: 1.2 MB (1197826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6d7e30c2d27f64a3117e85e87c00c1d4e79aa91e0bf4e4552c68d4710592d64`  
		Last Modified: Thu, 17 Mar 2022 22:10:19 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7f72f97159e0cf88a536b1a268d9bfa7af992046ce641dddb6710eabf7d08e4`  
		Last Modified: Thu, 17 Mar 2022 22:10:19 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.14` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:773c0f8c11aa82d0bf14e751ab65784b8993bd7477026d660eb8e970b160aad8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.4 MB (31441503 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1cc644adcd708fa1761227654eacbdd25163b6a5a399599e20c7eabdc2a24a8f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 17 Mar 2022 03:21:57 GMT
ADD file:e52e032f1ace6abd44b3647d43c1b8ae30bac6de804eef09c6ccd793057996fd in / 
# Thu, 17 Mar 2022 03:21:58 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 11:35:48 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Thu, 17 Mar 2022 11:35:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Mar 2022 11:35:52 GMT
ENV MEMCACHED_VERSION=1.6.14
# Thu, 17 Mar 2022 11:35:53 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Thu, 17 Mar 2022 11:38:38 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 17 Mar 2022 11:38:40 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 17 Mar 2022 11:38:40 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 17 Mar 2022 11:38:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Mar 2022 11:38:42 GMT
USER memcache
# Thu, 17 Mar 2022 11:38:43 GMT
EXPOSE 11211
# Thu, 17 Mar 2022 11:38:44 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:32252aec0777ac025a158bc2a8317650a4f2a0a875387011b1165013874f8723`  
		Last Modified: Thu, 17 Mar 2022 03:28:36 GMT  
		Size: 30.1 MB (30063013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:966f1b38b9d3f62f875f8dbd868ecc80c2037b45aadbec50fc16d292be747303`  
		Last Modified: Thu, 17 Mar 2022 11:42:26 GMT  
		Size: 4.9 KB (4903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2898c9abf66c159176811eff24e689c0989d4e7c025c9a7eb0f933d356aec11`  
		Last Modified: Thu, 17 Mar 2022 11:42:26 GMT  
		Size: 119.2 KB (119181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d331819fcfc0b6541dc90aafde95bc8b8a88e453cb3800c977716cff65961a77`  
		Last Modified: Thu, 17 Mar 2022 11:42:26 GMT  
		Size: 1.3 MB (1254002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25a25819b974fbc38bad380c4df00bf1f032cf4eb0112a109c78f9858d9a0a55`  
		Last Modified: Thu, 17 Mar 2022 11:42:26 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7c790b93b28eb9ed542eac0eaf8c5fe2d4c5daa368b0f27bac067fd01bee280`  
		Last Modified: Thu, 17 Mar 2022 11:42:26 GMT  
		Size: 118.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.14` - linux; 386

```console
$ docker pull memcached@sha256:3d0458851092782bb1cfb8fdb3edb27fe63775c3fb68f1879137e691de184e82
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.0 MB (33981668 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b7d3a232500fae88433d6e4117fa6e45b0ed4c529c925734eb2982bf3a3ee54`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 17 Mar 2022 08:15:53 GMT
ADD file:2d6be3846f0e5fabd85bc9409b1e2223cad4c57c76f96e9f81489ba78a72a1f5 in / 
# Thu, 17 Mar 2022 08:15:54 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 17:31:22 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Thu, 17 Mar 2022 17:31:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Mar 2022 17:31:26 GMT
ENV MEMCACHED_VERSION=1.6.14
# Thu, 17 Mar 2022 17:31:26 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Thu, 17 Mar 2022 17:35:17 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 17 Mar 2022 17:35:17 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 17 Mar 2022 17:35:18 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 17 Mar 2022 17:35:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Mar 2022 17:35:18 GMT
USER memcache
# Thu, 17 Mar 2022 17:35:18 GMT
EXPOSE 11211
# Thu, 17 Mar 2022 17:35:18 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:176085117cac9b2cf2cf57b3a10c9811dbd2773497fbac3086b5024070447e97`  
		Last Modified: Thu, 17 Mar 2022 08:24:00 GMT  
		Size: 32.4 MB (32386475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe18ed3f6ff50e5b12a7db917c34de3104619ae31e84d9d83ad2d94a3b8c5822`  
		Last Modified: Thu, 17 Mar 2022 17:40:19 GMT  
		Size: 4.9 KB (4896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc15fd9e0c057bb0a0d077f6c21d0b980b6ec5f9e5292c19d6fd790731f7bfc6`  
		Last Modified: Thu, 17 Mar 2022 17:40:19 GMT  
		Size: 336.6 KB (336638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1f8475d0ca14b4624de06fbe3207cdf07b5c31573192d0acc9b1e600b90c430`  
		Last Modified: Thu, 17 Mar 2022 17:40:20 GMT  
		Size: 1.3 MB (1253253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61e85d2ca17a8c6eb12e9cdc031a20d5c2357cf22bc4ad5353d520e13f60b73a`  
		Last Modified: Thu, 17 Mar 2022 17:40:19 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3194d39d810076bc29397aa1a117ac51d7bc610ffb9b7c90613fdf21203b05a3`  
		Last Modified: Thu, 17 Mar 2022 17:40:19 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.14` - linux; mips64le

```console
$ docker pull memcached@sha256:9148cd77f369a80c3b52dd4f79ddd8073c192da135e99a311f54641a851b4b60
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.0 MB (31012937 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:16b4bbcf6270bfbe61ccbb8083bf46151a57eb6a74f044b2004509978709ee0d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 17 Mar 2022 08:53:04 GMT
ADD file:795ac4eba576bc4c995df2a18b10ce802ee8a05417cdc53f5aa09452ecf2e832 in / 
# Thu, 17 Mar 2022 08:53:08 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 20:37:19 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Thu, 17 Mar 2022 20:37:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Mar 2022 20:37:40 GMT
ENV MEMCACHED_VERSION=1.6.14
# Thu, 17 Mar 2022 20:37:43 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Thu, 17 Mar 2022 20:44:58 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 17 Mar 2022 20:45:00 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 17 Mar 2022 20:45:05 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 17 Mar 2022 20:45:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Mar 2022 20:45:10 GMT
USER memcache
# Thu, 17 Mar 2022 20:45:13 GMT
EXPOSE 11211
# Thu, 17 Mar 2022 20:45:15 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:4799d88734ae94287a665c0e14621a744706cfbe17a0cf27ae9b0cc630927b11`  
		Last Modified: Thu, 17 Mar 2022 10:43:20 GMT  
		Size: 29.6 MB (29639810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a091b8fd61b3c0cafad5676908a202cec423a829bd2fb2bb79011b3ad5fd0845`  
		Last Modified: Thu, 17 Mar 2022 20:45:41 GMT  
		Size: 4.9 KB (4859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7644e6d2f727759be27279ab11b8f3e186b6918c1b3847badb0d04ae020286b`  
		Last Modified: Thu, 17 Mar 2022 20:45:41 GMT  
		Size: 117.1 KB (117098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47e8f3183abaf23ec67f322bc78981d3c838ad27bba488ec924c07d5b1a053a4`  
		Last Modified: Thu, 17 Mar 2022 20:45:41 GMT  
		Size: 1.3 MB (1250762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f0ac34ae7971e4442dd9abb2bbfa522fc4e65445f1ed51d33795cea9b37830e`  
		Last Modified: Thu, 17 Mar 2022 20:45:40 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0564ebbfe5b917d8a4818a435ddb35d5e4bbb4b4d7187189578f1c224d10ce2b`  
		Last Modified: Thu, 17 Mar 2022 20:45:40 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.14` - linux; ppc64le

```console
$ docker pull memcached@sha256:4893f4daa742b31f414b08f98f8e7d0cbedaf63b8d88062bcf3c91a9522a2aab
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.0 MB (36957544 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8db953cc998ed06712eca57fe4ae2b8bb342ce991683fd7592495a21557d0940`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 26 Jan 2022 01:46:51 GMT
ADD file:c03f34c221e57fa5cb625c166d1db9f72d6ba2fa17a3c41a5d04d6875d098949 in / 
# Wed, 26 Jan 2022 01:46:57 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 05:38:39 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 26 Jan 2022 05:38:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 11 Feb 2022 23:47:36 GMT
ENV MEMCACHED_VERSION=1.6.14
# Fri, 11 Feb 2022 23:47:38 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Fri, 11 Feb 2022 23:53:07 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Fri, 11 Feb 2022 23:53:13 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 11 Feb 2022 23:53:34 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 11 Feb 2022 23:53:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Feb 2022 23:53:39 GMT
USER memcache
# Fri, 11 Feb 2022 23:53:41 GMT
EXPOSE 11211
# Fri, 11 Feb 2022 23:53:46 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:3149ee4a73508a4c39107d64a3fdc1b021626a22a0ac95e62fa0cea49ab77fba`  
		Last Modified: Wed, 26 Jan 2022 01:57:01 GMT  
		Size: 35.3 MB (35273030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07bcb451658eb6d9eace467c2e989d96e53c409eb48347a369e9ad80aadcfe96`  
		Last Modified: Wed, 26 Jan 2022 05:45:22 GMT  
		Size: 5.0 KB (4980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8807782e060aa90873de57b2d3ec277632145f166e9c1e3801c57eea7e595cc`  
		Last Modified: Wed, 26 Jan 2022 05:45:22 GMT  
		Size: 356.9 KB (356905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5f2e5d5bb1609e336a37e97218d618550ec5ce28384c32b1141393ef6f04a03`  
		Last Modified: Fri, 11 Feb 2022 23:58:44 GMT  
		Size: 1.3 MB (1322220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76e6da4f290b1cff2fa5b1ad17d42333c67179332511db4da3bd2c5ce12bbdfa`  
		Last Modified: Fri, 11 Feb 2022 23:58:44 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fb140c5468aa121999bc169d30e4ce6b73795cdf67aa21c1dfd3d1194dd0b82`  
		Last Modified: Fri, 11 Feb 2022 23:58:44 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.14` - linux; s390x

```console
$ docker pull memcached@sha256:3e4437e519528ef8d3274dfc333f59f7c8c90099329a1e041fb6a71d5be8a1c5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.2 MB (31225911 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6fbcefffe918634bf299753ebcfe4a7284155e249686c5b5db9ffa92a5c0fc87`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 17 Mar 2022 03:06:58 GMT
ADD file:52f9267b4c57ac585a0d3d47a6f2ae1a71398264173ad4f190332957fa629c67 in / 
# Thu, 17 Mar 2022 03:07:01 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 08:47:34 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Thu, 17 Mar 2022 08:47:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Mar 2022 08:47:37 GMT
ENV MEMCACHED_VERSION=1.6.14
# Thu, 17 Mar 2022 08:47:37 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Thu, 17 Mar 2022 08:50:57 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 17 Mar 2022 08:50:57 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 17 Mar 2022 08:50:58 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 17 Mar 2022 08:50:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Mar 2022 08:50:58 GMT
USER memcache
# Thu, 17 Mar 2022 08:50:58 GMT
EXPOSE 11211
# Thu, 17 Mar 2022 08:50:59 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:d101968410e5005df630b0572aec03c88de55b8de81f3cf7e6a57e1ce2e5a8e5`  
		Last Modified: Thu, 17 Mar 2022 03:12:46 GMT  
		Size: 29.7 MB (29655795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1cad003ec39dc6e2e144c0953bad3bce3807fd1679d2c9e27e510724476e1e6`  
		Last Modified: Thu, 17 Mar 2022 08:55:34 GMT  
		Size: 5.0 KB (5022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13e61c306aebe51ff20adaf4ac683a69d93022d34ed4d09bc2ae7bde9d92ba52`  
		Last Modified: Thu, 17 Mar 2022 08:55:34 GMT  
		Size: 324.1 KB (324147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b5e88f796665ba79a22e6a541cbc3f30242e708c56d6b9af4fd0a7cd23abea6`  
		Last Modified: Thu, 17 Mar 2022 08:55:34 GMT  
		Size: 1.2 MB (1240539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77d35a1cb446cb01584cfbb3a61c40aaa1f358f37c8d723fe2437e6d070dbce3`  
		Last Modified: Thu, 17 Mar 2022 08:55:34 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b237b13dadf10fc593967f3714eaab56b7b00b89d435eb7e01be3f172b5b9b69`  
		Last Modified: Thu, 17 Mar 2022 08:55:33 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:1.6.14-alpine`

```console
$ docker pull memcached@sha256:614ca36d9fbc4953da3276766de5e77bdac23c04ffcde331032be6d854006131
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `memcached:1.6.14-alpine` - linux; amd64

```console
$ docker pull memcached@sha256:fd1bb2a04baff1bc63d2323d91a4f7135b9f06f1d0294fbe13b8660db7b6dd78
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3862528 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e9d7d65a6545e2698d88de0e6c6eeb620a5bdf19e35635a36ac252bb7dce9d55`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 17 Mar 2022 04:01:58 GMT
ADD file:cf4b631a115c2bbfbd81cad2d3041bceb64a8136aac92ba8a63b6c51d60af764 in / 
# Thu, 17 Mar 2022 04:01:59 GMT
CMD ["/bin/sh"]
# Thu, 17 Mar 2022 12:51:33 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Thu, 17 Mar 2022 12:51:34 GMT
RUN apk add --no-cache libsasl
# Thu, 17 Mar 2022 12:51:34 GMT
ENV MEMCACHED_VERSION=1.6.14
# Thu, 17 Mar 2022 12:51:35 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Thu, 17 Mar 2022 12:55:35 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Thu, 17 Mar 2022 12:55:35 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 17 Mar 2022 12:55:36 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 17 Mar 2022 12:55:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Mar 2022 12:55:36 GMT
USER memcache
# Thu, 17 Mar 2022 12:55:36 GMT
EXPOSE 11211
# Thu, 17 Mar 2022 12:55:36 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:3d243047344378e9b7136d552d48feb7ea8b6fe14ce0990e0cc011d5e369626a`  
		Last Modified: Thu, 17 Mar 2022 04:02:41 GMT  
		Size: 2.8 MB (2812636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e26b137db66bd985a8103e3e70f8985eafa9a9ca3dc6aa33344245535f6a6b0`  
		Last Modified: Thu, 17 Mar 2022 12:56:25 GMT  
		Size: 1.3 KB (1263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5231e0cae31bc5e59bdcb40f696ceaa6b5cad70b9500bc5bfd459174ac1f78dd`  
		Last Modified: Thu, 17 Mar 2022 12:56:25 GMT  
		Size: 109.3 KB (109285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d9fab8e58febfe6f0bfb8d5bdc098221b6348a6128014c4c2b4d4086284696d`  
		Last Modified: Thu, 17 Mar 2022 12:56:25 GMT  
		Size: 938.9 KB (938943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9ca16ee180425777e36c6f23ab6755a192eedf107400360aac9332686f1212b`  
		Last Modified: Thu, 17 Mar 2022 12:56:25 GMT  
		Size: 280.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f81d444d82a8e26057630fab59b6bdb890fe42afa50edabbba60d8685e88d639`  
		Last Modified: Thu, 17 Mar 2022 12:56:24 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.14-alpine` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:095e0c44c122b636ae053f2971bb454b3edfe210195707983a9e0a38d22f4411
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3754561 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d01922b70bc4d8d1d2be9eabafa82a0f0152a88e5871b7e9b6949cf1327c9c4f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 17 Mar 2022 03:19:52 GMT
ADD file:cd7d91362950471ca4678cf3833dc47119ab519dea51424c847bbbb21e1649d4 in / 
# Thu, 17 Mar 2022 03:19:52 GMT
CMD ["/bin/sh"]
# Thu, 17 Mar 2022 11:39:00 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Thu, 17 Mar 2022 11:39:02 GMT
RUN apk add --no-cache libsasl
# Thu, 17 Mar 2022 11:39:03 GMT
ENV MEMCACHED_VERSION=1.6.14
# Thu, 17 Mar 2022 11:39:04 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Thu, 17 Mar 2022 11:41:43 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Thu, 17 Mar 2022 11:41:45 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 17 Mar 2022 11:41:45 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 17 Mar 2022 11:41:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Mar 2022 11:41:47 GMT
USER memcache
# Thu, 17 Mar 2022 11:41:48 GMT
EXPOSE 11211
# Thu, 17 Mar 2022 11:41:49 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:148d739a8e6b9342daa1f5b428d3a3c6118f340f21df28c16e06f918ef150147`  
		Last Modified: Thu, 17 Mar 2022 03:20:45 GMT  
		Size: 2.7 MB (2714807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33dde588ab12fbb6aa46070a960ac850c8347e86f29744b40a123a466d4885ab`  
		Last Modified: Thu, 17 Mar 2022 11:42:57 GMT  
		Size: 1.2 KB (1240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bdeb7ac9fd9c67010a55bf3fe0e13866bb31d847353f455c95220027e2bc48c`  
		Last Modified: Thu, 17 Mar 2022 11:42:58 GMT  
		Size: 110.6 KB (110556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6bf3828467e4d3c16fcdc94bf5987db023e892ef9594c9c5dc2c3ccf07bc4bc`  
		Last Modified: Thu, 17 Mar 2022 11:42:58 GMT  
		Size: 927.5 KB (927550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d39e5be11e10e43e4991c6d85f4bdce89416e75c908d33656e4dcb79c26a51bc`  
		Last Modified: Thu, 17 Mar 2022 11:42:57 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9404edf07c113d954a0a5c34650b52d9a1f8e57d166b3e1b022a82c3e27e724`  
		Last Modified: Thu, 17 Mar 2022 11:42:57 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.14-alpine` - linux; 386

```console
$ docker pull memcached@sha256:8a6352e717a8080f0c0888560cf7ae52c77ee2cbd10ed46c68822370b5188d0f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3891706 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4db903b8d549ba5f131fc35c81b69bdf1822950956033492f126e16dd95b5750`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 17 Mar 2022 08:13:03 GMT
ADD file:22216bc654d9177244235f242fa83cae3b283b3c145cad7ccf11c0d29f5f0ff2 in / 
# Thu, 17 Mar 2022 08:13:03 GMT
CMD ["/bin/sh"]
# Thu, 17 Mar 2022 17:35:31 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Thu, 17 Mar 2022 17:35:32 GMT
RUN apk add --no-cache libsasl
# Thu, 17 Mar 2022 17:35:32 GMT
ENV MEMCACHED_VERSION=1.6.14
# Thu, 17 Mar 2022 17:35:33 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Thu, 17 Mar 2022 17:39:25 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Thu, 17 Mar 2022 17:39:25 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 17 Mar 2022 17:39:26 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 17 Mar 2022 17:39:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Mar 2022 17:39:26 GMT
USER memcache
# Thu, 17 Mar 2022 17:39:26 GMT
EXPOSE 11211
# Thu, 17 Mar 2022 17:39:26 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:93317a1f65ec94b67aefe728a598022610246404e3a68d391c76cd0e5244a2a0`  
		Last Modified: Thu, 17 Mar 2022 08:13:56 GMT  
		Size: 2.8 MB (2821789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae4d8e906564040308eb9f4b96b3808d37aa02b7fffa8e8d5c80126d5e50b1cf`  
		Last Modified: Thu, 17 Mar 2022 17:40:52 GMT  
		Size: 1.3 KB (1263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16143ebb273f49cf3884d5a063dfac8b30d9527c5018e90fac51ac381b5a5f8b`  
		Last Modified: Thu, 17 Mar 2022 17:40:52 GMT  
		Size: 121.2 KB (121183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:107340d48cdbc30d4b57291ca0d28997feed13517f3a508b3b398620dbc97099`  
		Last Modified: Thu, 17 Mar 2022 17:40:52 GMT  
		Size: 947.1 KB (947068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a791ada3ee704cad0a4dba90d29f533e6fcadb132c2522c38b4f0680201a86a9`  
		Last Modified: Thu, 17 Mar 2022 17:40:52 GMT  
		Size: 282.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fc23e842aa74aed8a4ea48cf2b6f027f9592e43e117c394bc70b3d2dcf0627c`  
		Last Modified: Thu, 17 Mar 2022 17:40:53 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.14-alpine` - linux; ppc64le

```console
$ docker pull memcached@sha256:75cb5141098fb02bb0c554c31c00d28802b414593a6b41d430c10505ee943fe0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.3 MB (5315837 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4be74852968716dd05ad711f1cda531afac5b782fe0dd6692e5aed7d91d54466`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 24 Nov 2021 20:20:16 GMT
ADD file:57115dca2eb707f46b6301e75174e6aa316fb02ac28643b91429b75be51bd8c8 in / 
# Wed, 24 Nov 2021 20:20:20 GMT
CMD ["/bin/sh"]
# Tue, 30 Nov 2021 00:52:13 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 30 Nov 2021 00:52:18 GMT
RUN apk add --no-cache libsasl
# Fri, 11 Feb 2022 23:54:02 GMT
ENV MEMCACHED_VERSION=1.6.14
# Fri, 11 Feb 2022 23:54:06 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Fri, 11 Feb 2022 23:57:48 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Fri, 11 Feb 2022 23:57:50 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 11 Feb 2022 23:57:55 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 11 Feb 2022 23:57:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Feb 2022 23:57:59 GMT
USER memcache
# Fri, 11 Feb 2022 23:58:01 GMT
EXPOSE 11211
# Fri, 11 Feb 2022 23:58:02 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:159b5dcb1717c815c76ff5ea1db730e18e8609c9090238e43282856db9e71f47`  
		Last Modified: Wed, 24 Nov 2021 20:21:14 GMT  
		Size: 2.8 MB (2814780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f44bb0dc5dc6d3634512266fffaecf643a467ef890e0a60fa7daed8a8f379335`  
		Last Modified: Tue, 30 Nov 2021 00:57:03 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:242bba95e896195e2c48210499ed8dad5c07a25a93e0d6304a787f4d5f05bb79`  
		Last Modified: Tue, 30 Nov 2021 00:57:03 GMT  
		Size: 126.2 KB (126210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9d933f0d59015113f25123de9b3460a03fdf091181f4c9330b1bb42c27a8cce`  
		Last Modified: Fri, 11 Feb 2022 23:59:16 GMT  
		Size: 2.4 MB (2373175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:659fd1f60c2bc05966f606e677370eeee3176f7d6dbd530b3f271ba313f8b0fe`  
		Last Modified: Fri, 11 Feb 2022 23:59:15 GMT  
		Size: 282.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8d9d86e7310ff252ce602224ce1643c6b8d50713444e43804cdb93912f89087`  
		Last Modified: Fri, 11 Feb 2022 23:59:15 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.14-alpine` - linux; s390x

```console
$ docker pull memcached@sha256:5a931719c887b04ccf389c14867075cca4a76c774ecceb8231f801d876c94be9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.7 MB (3651372 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8aed3255f32676856491e1f6e999893205a57c1d26f36d52518c7d72433bcd9c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 17 Mar 2022 03:04:28 GMT
ADD file:f623c69acb1859b41ef29e8f20f4e6c7072d9c6d7210d745afc615251bfe418f in / 
# Thu, 17 Mar 2022 03:04:28 GMT
CMD ["/bin/sh"]
# Thu, 17 Mar 2022 08:51:10 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Thu, 17 Mar 2022 08:51:11 GMT
RUN apk add --no-cache libsasl
# Thu, 17 Mar 2022 08:51:12 GMT
ENV MEMCACHED_VERSION=1.6.14
# Thu, 17 Mar 2022 08:51:12 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Thu, 17 Mar 2022 08:54:42 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Thu, 17 Mar 2022 08:54:42 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 17 Mar 2022 08:54:43 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 17 Mar 2022 08:54:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Mar 2022 08:54:43 GMT
USER memcache
# Thu, 17 Mar 2022 08:54:44 GMT
EXPOSE 11211
# Thu, 17 Mar 2022 08:54:44 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:d51040c5bfbf434887bfed2557335a411e6ef760d04cc178d455d1c3ec1b721c`  
		Last Modified: Thu, 17 Mar 2022 03:05:26 GMT  
		Size: 2.6 MB (2601715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bafa61f6f0948b111a53b71e2c8c1312981357779ca88eaf5e60d4163dc7d03b`  
		Last Modified: Thu, 17 Mar 2022 08:55:51 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6282933aed68188fd9995db64b18a466643f4879e98a97392e6df0309f825ab`  
		Last Modified: Thu, 17 Mar 2022 08:55:51 GMT  
		Size: 113.8 KB (113794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d266558ba8144540d874cf2a04b80cdad0b98138893dbd2bf8dfc0a82587d0fc`  
		Last Modified: Thu, 17 Mar 2022 08:55:51 GMT  
		Size: 934.2 KB (934189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e97cc0f7d043b7a30a2ecd4a02847ed3d1227cdec67c577b9486ae3a40bb7f55`  
		Last Modified: Thu, 17 Mar 2022 08:55:51 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:973434578ea89c81d5ee8f8c926d6efab348a190b4d1f8c59c32b595e5e3ff14`  
		Last Modified: Thu, 17 Mar 2022 08:55:51 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:1.6.14-alpine3.15`

```console
$ docker pull memcached@sha256:614ca36d9fbc4953da3276766de5e77bdac23c04ffcde331032be6d854006131
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `memcached:1.6.14-alpine3.15` - linux; amd64

```console
$ docker pull memcached@sha256:fd1bb2a04baff1bc63d2323d91a4f7135b9f06f1d0294fbe13b8660db7b6dd78
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3862528 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e9d7d65a6545e2698d88de0e6c6eeb620a5bdf19e35635a36ac252bb7dce9d55`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 17 Mar 2022 04:01:58 GMT
ADD file:cf4b631a115c2bbfbd81cad2d3041bceb64a8136aac92ba8a63b6c51d60af764 in / 
# Thu, 17 Mar 2022 04:01:59 GMT
CMD ["/bin/sh"]
# Thu, 17 Mar 2022 12:51:33 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Thu, 17 Mar 2022 12:51:34 GMT
RUN apk add --no-cache libsasl
# Thu, 17 Mar 2022 12:51:34 GMT
ENV MEMCACHED_VERSION=1.6.14
# Thu, 17 Mar 2022 12:51:35 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Thu, 17 Mar 2022 12:55:35 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Thu, 17 Mar 2022 12:55:35 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 17 Mar 2022 12:55:36 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 17 Mar 2022 12:55:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Mar 2022 12:55:36 GMT
USER memcache
# Thu, 17 Mar 2022 12:55:36 GMT
EXPOSE 11211
# Thu, 17 Mar 2022 12:55:36 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:3d243047344378e9b7136d552d48feb7ea8b6fe14ce0990e0cc011d5e369626a`  
		Last Modified: Thu, 17 Mar 2022 04:02:41 GMT  
		Size: 2.8 MB (2812636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e26b137db66bd985a8103e3e70f8985eafa9a9ca3dc6aa33344245535f6a6b0`  
		Last Modified: Thu, 17 Mar 2022 12:56:25 GMT  
		Size: 1.3 KB (1263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5231e0cae31bc5e59bdcb40f696ceaa6b5cad70b9500bc5bfd459174ac1f78dd`  
		Last Modified: Thu, 17 Mar 2022 12:56:25 GMT  
		Size: 109.3 KB (109285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d9fab8e58febfe6f0bfb8d5bdc098221b6348a6128014c4c2b4d4086284696d`  
		Last Modified: Thu, 17 Mar 2022 12:56:25 GMT  
		Size: 938.9 KB (938943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9ca16ee180425777e36c6f23ab6755a192eedf107400360aac9332686f1212b`  
		Last Modified: Thu, 17 Mar 2022 12:56:25 GMT  
		Size: 280.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f81d444d82a8e26057630fab59b6bdb890fe42afa50edabbba60d8685e88d639`  
		Last Modified: Thu, 17 Mar 2022 12:56:24 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.14-alpine3.15` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:095e0c44c122b636ae053f2971bb454b3edfe210195707983a9e0a38d22f4411
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3754561 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d01922b70bc4d8d1d2be9eabafa82a0f0152a88e5871b7e9b6949cf1327c9c4f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 17 Mar 2022 03:19:52 GMT
ADD file:cd7d91362950471ca4678cf3833dc47119ab519dea51424c847bbbb21e1649d4 in / 
# Thu, 17 Mar 2022 03:19:52 GMT
CMD ["/bin/sh"]
# Thu, 17 Mar 2022 11:39:00 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Thu, 17 Mar 2022 11:39:02 GMT
RUN apk add --no-cache libsasl
# Thu, 17 Mar 2022 11:39:03 GMT
ENV MEMCACHED_VERSION=1.6.14
# Thu, 17 Mar 2022 11:39:04 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Thu, 17 Mar 2022 11:41:43 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Thu, 17 Mar 2022 11:41:45 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 17 Mar 2022 11:41:45 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 17 Mar 2022 11:41:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Mar 2022 11:41:47 GMT
USER memcache
# Thu, 17 Mar 2022 11:41:48 GMT
EXPOSE 11211
# Thu, 17 Mar 2022 11:41:49 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:148d739a8e6b9342daa1f5b428d3a3c6118f340f21df28c16e06f918ef150147`  
		Last Modified: Thu, 17 Mar 2022 03:20:45 GMT  
		Size: 2.7 MB (2714807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33dde588ab12fbb6aa46070a960ac850c8347e86f29744b40a123a466d4885ab`  
		Last Modified: Thu, 17 Mar 2022 11:42:57 GMT  
		Size: 1.2 KB (1240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bdeb7ac9fd9c67010a55bf3fe0e13866bb31d847353f455c95220027e2bc48c`  
		Last Modified: Thu, 17 Mar 2022 11:42:58 GMT  
		Size: 110.6 KB (110556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6bf3828467e4d3c16fcdc94bf5987db023e892ef9594c9c5dc2c3ccf07bc4bc`  
		Last Modified: Thu, 17 Mar 2022 11:42:58 GMT  
		Size: 927.5 KB (927550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d39e5be11e10e43e4991c6d85f4bdce89416e75c908d33656e4dcb79c26a51bc`  
		Last Modified: Thu, 17 Mar 2022 11:42:57 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9404edf07c113d954a0a5c34650b52d9a1f8e57d166b3e1b022a82c3e27e724`  
		Last Modified: Thu, 17 Mar 2022 11:42:57 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.14-alpine3.15` - linux; 386

```console
$ docker pull memcached@sha256:8a6352e717a8080f0c0888560cf7ae52c77ee2cbd10ed46c68822370b5188d0f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3891706 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4db903b8d549ba5f131fc35c81b69bdf1822950956033492f126e16dd95b5750`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 17 Mar 2022 08:13:03 GMT
ADD file:22216bc654d9177244235f242fa83cae3b283b3c145cad7ccf11c0d29f5f0ff2 in / 
# Thu, 17 Mar 2022 08:13:03 GMT
CMD ["/bin/sh"]
# Thu, 17 Mar 2022 17:35:31 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Thu, 17 Mar 2022 17:35:32 GMT
RUN apk add --no-cache libsasl
# Thu, 17 Mar 2022 17:35:32 GMT
ENV MEMCACHED_VERSION=1.6.14
# Thu, 17 Mar 2022 17:35:33 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Thu, 17 Mar 2022 17:39:25 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Thu, 17 Mar 2022 17:39:25 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 17 Mar 2022 17:39:26 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 17 Mar 2022 17:39:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Mar 2022 17:39:26 GMT
USER memcache
# Thu, 17 Mar 2022 17:39:26 GMT
EXPOSE 11211
# Thu, 17 Mar 2022 17:39:26 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:93317a1f65ec94b67aefe728a598022610246404e3a68d391c76cd0e5244a2a0`  
		Last Modified: Thu, 17 Mar 2022 08:13:56 GMT  
		Size: 2.8 MB (2821789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae4d8e906564040308eb9f4b96b3808d37aa02b7fffa8e8d5c80126d5e50b1cf`  
		Last Modified: Thu, 17 Mar 2022 17:40:52 GMT  
		Size: 1.3 KB (1263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16143ebb273f49cf3884d5a063dfac8b30d9527c5018e90fac51ac381b5a5f8b`  
		Last Modified: Thu, 17 Mar 2022 17:40:52 GMT  
		Size: 121.2 KB (121183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:107340d48cdbc30d4b57291ca0d28997feed13517f3a508b3b398620dbc97099`  
		Last Modified: Thu, 17 Mar 2022 17:40:52 GMT  
		Size: 947.1 KB (947068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a791ada3ee704cad0a4dba90d29f533e6fcadb132c2522c38b4f0680201a86a9`  
		Last Modified: Thu, 17 Mar 2022 17:40:52 GMT  
		Size: 282.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fc23e842aa74aed8a4ea48cf2b6f027f9592e43e117c394bc70b3d2dcf0627c`  
		Last Modified: Thu, 17 Mar 2022 17:40:53 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.14-alpine3.15` - linux; ppc64le

```console
$ docker pull memcached@sha256:75cb5141098fb02bb0c554c31c00d28802b414593a6b41d430c10505ee943fe0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.3 MB (5315837 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4be74852968716dd05ad711f1cda531afac5b782fe0dd6692e5aed7d91d54466`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 24 Nov 2021 20:20:16 GMT
ADD file:57115dca2eb707f46b6301e75174e6aa316fb02ac28643b91429b75be51bd8c8 in / 
# Wed, 24 Nov 2021 20:20:20 GMT
CMD ["/bin/sh"]
# Tue, 30 Nov 2021 00:52:13 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 30 Nov 2021 00:52:18 GMT
RUN apk add --no-cache libsasl
# Fri, 11 Feb 2022 23:54:02 GMT
ENV MEMCACHED_VERSION=1.6.14
# Fri, 11 Feb 2022 23:54:06 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Fri, 11 Feb 2022 23:57:48 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Fri, 11 Feb 2022 23:57:50 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 11 Feb 2022 23:57:55 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 11 Feb 2022 23:57:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Feb 2022 23:57:59 GMT
USER memcache
# Fri, 11 Feb 2022 23:58:01 GMT
EXPOSE 11211
# Fri, 11 Feb 2022 23:58:02 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:159b5dcb1717c815c76ff5ea1db730e18e8609c9090238e43282856db9e71f47`  
		Last Modified: Wed, 24 Nov 2021 20:21:14 GMT  
		Size: 2.8 MB (2814780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f44bb0dc5dc6d3634512266fffaecf643a467ef890e0a60fa7daed8a8f379335`  
		Last Modified: Tue, 30 Nov 2021 00:57:03 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:242bba95e896195e2c48210499ed8dad5c07a25a93e0d6304a787f4d5f05bb79`  
		Last Modified: Tue, 30 Nov 2021 00:57:03 GMT  
		Size: 126.2 KB (126210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9d933f0d59015113f25123de9b3460a03fdf091181f4c9330b1bb42c27a8cce`  
		Last Modified: Fri, 11 Feb 2022 23:59:16 GMT  
		Size: 2.4 MB (2373175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:659fd1f60c2bc05966f606e677370eeee3176f7d6dbd530b3f271ba313f8b0fe`  
		Last Modified: Fri, 11 Feb 2022 23:59:15 GMT  
		Size: 282.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8d9d86e7310ff252ce602224ce1643c6b8d50713444e43804cdb93912f89087`  
		Last Modified: Fri, 11 Feb 2022 23:59:15 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.14-alpine3.15` - linux; s390x

```console
$ docker pull memcached@sha256:5a931719c887b04ccf389c14867075cca4a76c774ecceb8231f801d876c94be9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.7 MB (3651372 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8aed3255f32676856491e1f6e999893205a57c1d26f36d52518c7d72433bcd9c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 17 Mar 2022 03:04:28 GMT
ADD file:f623c69acb1859b41ef29e8f20f4e6c7072d9c6d7210d745afc615251bfe418f in / 
# Thu, 17 Mar 2022 03:04:28 GMT
CMD ["/bin/sh"]
# Thu, 17 Mar 2022 08:51:10 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Thu, 17 Mar 2022 08:51:11 GMT
RUN apk add --no-cache libsasl
# Thu, 17 Mar 2022 08:51:12 GMT
ENV MEMCACHED_VERSION=1.6.14
# Thu, 17 Mar 2022 08:51:12 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Thu, 17 Mar 2022 08:54:42 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Thu, 17 Mar 2022 08:54:42 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 17 Mar 2022 08:54:43 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 17 Mar 2022 08:54:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Mar 2022 08:54:43 GMT
USER memcache
# Thu, 17 Mar 2022 08:54:44 GMT
EXPOSE 11211
# Thu, 17 Mar 2022 08:54:44 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:d51040c5bfbf434887bfed2557335a411e6ef760d04cc178d455d1c3ec1b721c`  
		Last Modified: Thu, 17 Mar 2022 03:05:26 GMT  
		Size: 2.6 MB (2601715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bafa61f6f0948b111a53b71e2c8c1312981357779ca88eaf5e60d4163dc7d03b`  
		Last Modified: Thu, 17 Mar 2022 08:55:51 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6282933aed68188fd9995db64b18a466643f4879e98a97392e6df0309f825ab`  
		Last Modified: Thu, 17 Mar 2022 08:55:51 GMT  
		Size: 113.8 KB (113794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d266558ba8144540d874cf2a04b80cdad0b98138893dbd2bf8dfc0a82587d0fc`  
		Last Modified: Thu, 17 Mar 2022 08:55:51 GMT  
		Size: 934.2 KB (934189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e97cc0f7d043b7a30a2ecd4a02847ed3d1227cdec67c577b9486ae3a40bb7f55`  
		Last Modified: Thu, 17 Mar 2022 08:55:51 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:973434578ea89c81d5ee8f8c926d6efab348a190b4d1f8c59c32b595e5e3ff14`  
		Last Modified: Thu, 17 Mar 2022 08:55:51 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:1.6.14-bullseye`

```console
$ docker pull memcached@sha256:67ceec1841427583fd33842be1a41243351997c4803d05c14f95f0c8c6826f93
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

### `memcached:1.6.14-bullseye` - linux; amd64

```console
$ docker pull memcached@sha256:6a51dd2e23a3ead43158d3255ab8c2d9b0b2f0432becf5814c267273c84e8b6a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.0 MB (32965129 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e897df046b27f4dbfae44d31346ef91c2160a46c1b8d5bf652a40e3d76d3914f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 17 Mar 2022 04:03:59 GMT
ADD file:36919ae6bb25e3269eff949443129a01a8a43fb967fe6563939ebe1e1e9b8228 in / 
# Thu, 17 Mar 2022 04:03:59 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 12:47:26 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Thu, 17 Mar 2022 12:47:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Mar 2022 12:47:29 GMT
ENV MEMCACHED_VERSION=1.6.14
# Thu, 17 Mar 2022 12:47:29 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Thu, 17 Mar 2022 12:51:18 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 17 Mar 2022 12:51:18 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 17 Mar 2022 12:51:18 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 17 Mar 2022 12:51:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Mar 2022 12:51:18 GMT
USER memcache
# Thu, 17 Mar 2022 12:51:19 GMT
EXPOSE 11211
# Thu, 17 Mar 2022 12:51:19 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:ae13dd57832654086618a81dbc128846aa092489260c326ee95429b63c3cf213`  
		Last Modified: Thu, 17 Mar 2022 04:10:05 GMT  
		Size: 31.4 MB (31376572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c39e8a8db385456589d2009379dedc9787a9297b0ea679ff564500de9894d325`  
		Last Modified: Thu, 17 Mar 2022 12:55:59 GMT  
		Size: 5.0 KB (4982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fa3e9def276e8e73128ec9d08c6f139621666d0724b33d882ca0943a1a6825b`  
		Last Modified: Thu, 17 Mar 2022 12:55:59 GMT  
		Size: 328.0 KB (328046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9835681ca994d84f0de3da2d9ed0cdb5882c06b58bccdc406102bf4bf8a55700`  
		Last Modified: Thu, 17 Mar 2022 12:55:59 GMT  
		Size: 1.3 MB (1255121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d362d7003189fa875ec372df3c4c9622f2688adb7ed5c9cb2bec35c31b9d523`  
		Last Modified: Thu, 17 Mar 2022 12:55:59 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bd4550226c671e2d98eac87073171c925eebaa0e039ed5e2610d516980dd220`  
		Last Modified: Thu, 17 Mar 2022 12:55:59 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.14-bullseye` - linux; arm variant v5

```console
$ docker pull memcached@sha256:084a4198172362acf346afa27655123636800a135bdaaa857d8d57e7e402c4fa
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.5 MB (30467908 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b9e543544c3f8ef04ec918e92a8e98602cbdc37970011b5960685ffd0103780`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 17 Mar 2022 05:19:45 GMT
ADD file:1eb4f937d40230354e20e28ed781234acd4be2b0dab72f87131a3eac66349719 in / 
# Thu, 17 Mar 2022 05:19:46 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 10:06:48 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Thu, 17 Mar 2022 10:06:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Mar 2022 10:07:00 GMT
ENV MEMCACHED_VERSION=1.6.14
# Thu, 17 Mar 2022 10:07:00 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Thu, 17 Mar 2022 10:11:18 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 17 Mar 2022 10:11:18 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 17 Mar 2022 10:11:20 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 17 Mar 2022 10:11:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Mar 2022 10:11:21 GMT
USER memcache
# Thu, 17 Mar 2022 10:11:21 GMT
EXPOSE 11211
# Thu, 17 Mar 2022 10:11:21 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:4da455e7774c0e977d862a56ab6d85f33ce5dd5a77d45a0a74a272e9eae6bea0`  
		Last Modified: Thu, 17 Mar 2022 05:35:01 GMT  
		Size: 28.9 MB (28919702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39450ea3e36758cb1aaf29a3e4a3694a4f1e5d208ece3da6479b6dcd47705309`  
		Last Modified: Thu, 17 Mar 2022 10:12:14 GMT  
		Size: 4.9 KB (4890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b674f1fc0977777c240d7af9fa6d57e8b24d5332791547c80820aa9d1956d037`  
		Last Modified: Thu, 17 Mar 2022 10:12:14 GMT  
		Size: 316.6 KB (316575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de44c6f01b62d4d56baa2601e6706305eaf35c2da9541623a8c94c7fe1e4b8b2`  
		Last Modified: Thu, 17 Mar 2022 10:12:14 GMT  
		Size: 1.2 MB (1226335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18229473d3cfa938b3ba5d7f36b228bc60b7641660ae3242b56e210a50892b0f`  
		Last Modified: Thu, 17 Mar 2022 10:12:14 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e231e6a0756abb2590d1ef0507c610f0aa1b4f42e40a895d310b330662a98a2`  
		Last Modified: Thu, 17 Mar 2022 10:12:14 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.14-bullseye` - linux; arm variant v7

```console
$ docker pull memcached@sha256:9fe6c86dfef8c0cf535d443045364d887fd0bc8b44f550a8cbb0dca64e33e732
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.1 MB (28090226 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14dc9d69afed7832780e59eca9bf08aecbca59e357a3c301648a665b42b6659a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 17 Mar 2022 09:31:03 GMT
ADD file:e52f9ee2dc3144d7b9eb3ec90c106aa2a094eb4c5c2aa8cbff5c520a5faaef43 in / 
# Thu, 17 Mar 2022 09:31:04 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 21:53:04 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Thu, 17 Mar 2022 21:53:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Mar 2022 21:53:14 GMT
ENV MEMCACHED_VERSION=1.6.14
# Thu, 17 Mar 2022 21:53:14 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Thu, 17 Mar 2022 21:57:21 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 17 Mar 2022 21:57:22 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 17 Mar 2022 21:57:23 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 17 Mar 2022 21:57:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Mar 2022 21:57:24 GMT
USER memcache
# Thu, 17 Mar 2022 21:57:25 GMT
EXPOSE 11211
# Thu, 17 Mar 2022 21:57:25 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:5e5e708ee1f9fdbc69324391f7d1f816c657e6116eff09e7d2247fa9de3a076a`  
		Last Modified: Thu, 17 Mar 2022 09:46:33 GMT  
		Size: 26.6 MB (26575097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f652a8bcf3f50c242f3e27b3792cd55f9c0436702fe2bcdd4ae3df203aa84100`  
		Last Modified: Thu, 17 Mar 2022 22:10:19 GMT  
		Size: 4.9 KB (4896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c1be80f12d4f19157864e18689a8dd9c0f84c3a6c929949b066e7c29f30c5d7`  
		Last Modified: Thu, 17 Mar 2022 22:10:19 GMT  
		Size: 312.0 KB (311999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37ab28ddd02c6ca7832dec8a6b6508e8e4d95b34c8f4fe17457a1844c4442a7a`  
		Last Modified: Thu, 17 Mar 2022 22:10:19 GMT  
		Size: 1.2 MB (1197826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6d7e30c2d27f64a3117e85e87c00c1d4e79aa91e0bf4e4552c68d4710592d64`  
		Last Modified: Thu, 17 Mar 2022 22:10:19 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7f72f97159e0cf88a536b1a268d9bfa7af992046ce641dddb6710eabf7d08e4`  
		Last Modified: Thu, 17 Mar 2022 22:10:19 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.14-bullseye` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:773c0f8c11aa82d0bf14e751ab65784b8993bd7477026d660eb8e970b160aad8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.4 MB (31441503 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1cc644adcd708fa1761227654eacbdd25163b6a5a399599e20c7eabdc2a24a8f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 17 Mar 2022 03:21:57 GMT
ADD file:e52e032f1ace6abd44b3647d43c1b8ae30bac6de804eef09c6ccd793057996fd in / 
# Thu, 17 Mar 2022 03:21:58 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 11:35:48 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Thu, 17 Mar 2022 11:35:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Mar 2022 11:35:52 GMT
ENV MEMCACHED_VERSION=1.6.14
# Thu, 17 Mar 2022 11:35:53 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Thu, 17 Mar 2022 11:38:38 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 17 Mar 2022 11:38:40 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 17 Mar 2022 11:38:40 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 17 Mar 2022 11:38:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Mar 2022 11:38:42 GMT
USER memcache
# Thu, 17 Mar 2022 11:38:43 GMT
EXPOSE 11211
# Thu, 17 Mar 2022 11:38:44 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:32252aec0777ac025a158bc2a8317650a4f2a0a875387011b1165013874f8723`  
		Last Modified: Thu, 17 Mar 2022 03:28:36 GMT  
		Size: 30.1 MB (30063013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:966f1b38b9d3f62f875f8dbd868ecc80c2037b45aadbec50fc16d292be747303`  
		Last Modified: Thu, 17 Mar 2022 11:42:26 GMT  
		Size: 4.9 KB (4903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2898c9abf66c159176811eff24e689c0989d4e7c025c9a7eb0f933d356aec11`  
		Last Modified: Thu, 17 Mar 2022 11:42:26 GMT  
		Size: 119.2 KB (119181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d331819fcfc0b6541dc90aafde95bc8b8a88e453cb3800c977716cff65961a77`  
		Last Modified: Thu, 17 Mar 2022 11:42:26 GMT  
		Size: 1.3 MB (1254002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25a25819b974fbc38bad380c4df00bf1f032cf4eb0112a109c78f9858d9a0a55`  
		Last Modified: Thu, 17 Mar 2022 11:42:26 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7c790b93b28eb9ed542eac0eaf8c5fe2d4c5daa368b0f27bac067fd01bee280`  
		Last Modified: Thu, 17 Mar 2022 11:42:26 GMT  
		Size: 118.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.14-bullseye` - linux; 386

```console
$ docker pull memcached@sha256:3d0458851092782bb1cfb8fdb3edb27fe63775c3fb68f1879137e691de184e82
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.0 MB (33981668 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b7d3a232500fae88433d6e4117fa6e45b0ed4c529c925734eb2982bf3a3ee54`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 17 Mar 2022 08:15:53 GMT
ADD file:2d6be3846f0e5fabd85bc9409b1e2223cad4c57c76f96e9f81489ba78a72a1f5 in / 
# Thu, 17 Mar 2022 08:15:54 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 17:31:22 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Thu, 17 Mar 2022 17:31:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Mar 2022 17:31:26 GMT
ENV MEMCACHED_VERSION=1.6.14
# Thu, 17 Mar 2022 17:31:26 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Thu, 17 Mar 2022 17:35:17 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 17 Mar 2022 17:35:17 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 17 Mar 2022 17:35:18 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 17 Mar 2022 17:35:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Mar 2022 17:35:18 GMT
USER memcache
# Thu, 17 Mar 2022 17:35:18 GMT
EXPOSE 11211
# Thu, 17 Mar 2022 17:35:18 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:176085117cac9b2cf2cf57b3a10c9811dbd2773497fbac3086b5024070447e97`  
		Last Modified: Thu, 17 Mar 2022 08:24:00 GMT  
		Size: 32.4 MB (32386475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe18ed3f6ff50e5b12a7db917c34de3104619ae31e84d9d83ad2d94a3b8c5822`  
		Last Modified: Thu, 17 Mar 2022 17:40:19 GMT  
		Size: 4.9 KB (4896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc15fd9e0c057bb0a0d077f6c21d0b980b6ec5f9e5292c19d6fd790731f7bfc6`  
		Last Modified: Thu, 17 Mar 2022 17:40:19 GMT  
		Size: 336.6 KB (336638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1f8475d0ca14b4624de06fbe3207cdf07b5c31573192d0acc9b1e600b90c430`  
		Last Modified: Thu, 17 Mar 2022 17:40:20 GMT  
		Size: 1.3 MB (1253253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61e85d2ca17a8c6eb12e9cdc031a20d5c2357cf22bc4ad5353d520e13f60b73a`  
		Last Modified: Thu, 17 Mar 2022 17:40:19 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3194d39d810076bc29397aa1a117ac51d7bc610ffb9b7c90613fdf21203b05a3`  
		Last Modified: Thu, 17 Mar 2022 17:40:19 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.14-bullseye` - linux; mips64le

```console
$ docker pull memcached@sha256:9148cd77f369a80c3b52dd4f79ddd8073c192da135e99a311f54641a851b4b60
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.0 MB (31012937 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:16b4bbcf6270bfbe61ccbb8083bf46151a57eb6a74f044b2004509978709ee0d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 17 Mar 2022 08:53:04 GMT
ADD file:795ac4eba576bc4c995df2a18b10ce802ee8a05417cdc53f5aa09452ecf2e832 in / 
# Thu, 17 Mar 2022 08:53:08 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 20:37:19 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Thu, 17 Mar 2022 20:37:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Mar 2022 20:37:40 GMT
ENV MEMCACHED_VERSION=1.6.14
# Thu, 17 Mar 2022 20:37:43 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Thu, 17 Mar 2022 20:44:58 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 17 Mar 2022 20:45:00 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 17 Mar 2022 20:45:05 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 17 Mar 2022 20:45:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Mar 2022 20:45:10 GMT
USER memcache
# Thu, 17 Mar 2022 20:45:13 GMT
EXPOSE 11211
# Thu, 17 Mar 2022 20:45:15 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:4799d88734ae94287a665c0e14621a744706cfbe17a0cf27ae9b0cc630927b11`  
		Last Modified: Thu, 17 Mar 2022 10:43:20 GMT  
		Size: 29.6 MB (29639810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a091b8fd61b3c0cafad5676908a202cec423a829bd2fb2bb79011b3ad5fd0845`  
		Last Modified: Thu, 17 Mar 2022 20:45:41 GMT  
		Size: 4.9 KB (4859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7644e6d2f727759be27279ab11b8f3e186b6918c1b3847badb0d04ae020286b`  
		Last Modified: Thu, 17 Mar 2022 20:45:41 GMT  
		Size: 117.1 KB (117098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47e8f3183abaf23ec67f322bc78981d3c838ad27bba488ec924c07d5b1a053a4`  
		Last Modified: Thu, 17 Mar 2022 20:45:41 GMT  
		Size: 1.3 MB (1250762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f0ac34ae7971e4442dd9abb2bbfa522fc4e65445f1ed51d33795cea9b37830e`  
		Last Modified: Thu, 17 Mar 2022 20:45:40 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0564ebbfe5b917d8a4818a435ddb35d5e4bbb4b4d7187189578f1c224d10ce2b`  
		Last Modified: Thu, 17 Mar 2022 20:45:40 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.14-bullseye` - linux; ppc64le

```console
$ docker pull memcached@sha256:4893f4daa742b31f414b08f98f8e7d0cbedaf63b8d88062bcf3c91a9522a2aab
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.0 MB (36957544 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8db953cc998ed06712eca57fe4ae2b8bb342ce991683fd7592495a21557d0940`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 26 Jan 2022 01:46:51 GMT
ADD file:c03f34c221e57fa5cb625c166d1db9f72d6ba2fa17a3c41a5d04d6875d098949 in / 
# Wed, 26 Jan 2022 01:46:57 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 05:38:39 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 26 Jan 2022 05:38:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 11 Feb 2022 23:47:36 GMT
ENV MEMCACHED_VERSION=1.6.14
# Fri, 11 Feb 2022 23:47:38 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Fri, 11 Feb 2022 23:53:07 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Fri, 11 Feb 2022 23:53:13 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 11 Feb 2022 23:53:34 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 11 Feb 2022 23:53:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Feb 2022 23:53:39 GMT
USER memcache
# Fri, 11 Feb 2022 23:53:41 GMT
EXPOSE 11211
# Fri, 11 Feb 2022 23:53:46 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:3149ee4a73508a4c39107d64a3fdc1b021626a22a0ac95e62fa0cea49ab77fba`  
		Last Modified: Wed, 26 Jan 2022 01:57:01 GMT  
		Size: 35.3 MB (35273030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07bcb451658eb6d9eace467c2e989d96e53c409eb48347a369e9ad80aadcfe96`  
		Last Modified: Wed, 26 Jan 2022 05:45:22 GMT  
		Size: 5.0 KB (4980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8807782e060aa90873de57b2d3ec277632145f166e9c1e3801c57eea7e595cc`  
		Last Modified: Wed, 26 Jan 2022 05:45:22 GMT  
		Size: 356.9 KB (356905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5f2e5d5bb1609e336a37e97218d618550ec5ce28384c32b1141393ef6f04a03`  
		Last Modified: Fri, 11 Feb 2022 23:58:44 GMT  
		Size: 1.3 MB (1322220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76e6da4f290b1cff2fa5b1ad17d42333c67179332511db4da3bd2c5ce12bbdfa`  
		Last Modified: Fri, 11 Feb 2022 23:58:44 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fb140c5468aa121999bc169d30e4ce6b73795cdf67aa21c1dfd3d1194dd0b82`  
		Last Modified: Fri, 11 Feb 2022 23:58:44 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.14-bullseye` - linux; s390x

```console
$ docker pull memcached@sha256:3e4437e519528ef8d3274dfc333f59f7c8c90099329a1e041fb6a71d5be8a1c5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.2 MB (31225911 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6fbcefffe918634bf299753ebcfe4a7284155e249686c5b5db9ffa92a5c0fc87`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 17 Mar 2022 03:06:58 GMT
ADD file:52f9267b4c57ac585a0d3d47a6f2ae1a71398264173ad4f190332957fa629c67 in / 
# Thu, 17 Mar 2022 03:07:01 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 08:47:34 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Thu, 17 Mar 2022 08:47:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Mar 2022 08:47:37 GMT
ENV MEMCACHED_VERSION=1.6.14
# Thu, 17 Mar 2022 08:47:37 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Thu, 17 Mar 2022 08:50:57 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 17 Mar 2022 08:50:57 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 17 Mar 2022 08:50:58 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 17 Mar 2022 08:50:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Mar 2022 08:50:58 GMT
USER memcache
# Thu, 17 Mar 2022 08:50:58 GMT
EXPOSE 11211
# Thu, 17 Mar 2022 08:50:59 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:d101968410e5005df630b0572aec03c88de55b8de81f3cf7e6a57e1ce2e5a8e5`  
		Last Modified: Thu, 17 Mar 2022 03:12:46 GMT  
		Size: 29.7 MB (29655795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1cad003ec39dc6e2e144c0953bad3bce3807fd1679d2c9e27e510724476e1e6`  
		Last Modified: Thu, 17 Mar 2022 08:55:34 GMT  
		Size: 5.0 KB (5022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13e61c306aebe51ff20adaf4ac683a69d93022d34ed4d09bc2ae7bde9d92ba52`  
		Last Modified: Thu, 17 Mar 2022 08:55:34 GMT  
		Size: 324.1 KB (324147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b5e88f796665ba79a22e6a541cbc3f30242e708c56d6b9af4fd0a7cd23abea6`  
		Last Modified: Thu, 17 Mar 2022 08:55:34 GMT  
		Size: 1.2 MB (1240539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77d35a1cb446cb01584cfbb3a61c40aaa1f358f37c8d723fe2437e6d070dbce3`  
		Last Modified: Thu, 17 Mar 2022 08:55:34 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b237b13dadf10fc593967f3714eaab56b7b00b89d435eb7e01be3f172b5b9b69`  
		Last Modified: Thu, 17 Mar 2022 08:55:33 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:alpine`

```console
$ docker pull memcached@sha256:f29cd53458fed5079ec81d66878db3f5ef40001b371b0437af6d5a660008f779
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
$ docker pull memcached@sha256:fd1bb2a04baff1bc63d2323d91a4f7135b9f06f1d0294fbe13b8660db7b6dd78
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3862528 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e9d7d65a6545e2698d88de0e6c6eeb620a5bdf19e35635a36ac252bb7dce9d55`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 17 Mar 2022 04:01:58 GMT
ADD file:cf4b631a115c2bbfbd81cad2d3041bceb64a8136aac92ba8a63b6c51d60af764 in / 
# Thu, 17 Mar 2022 04:01:59 GMT
CMD ["/bin/sh"]
# Thu, 17 Mar 2022 12:51:33 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Thu, 17 Mar 2022 12:51:34 GMT
RUN apk add --no-cache libsasl
# Thu, 17 Mar 2022 12:51:34 GMT
ENV MEMCACHED_VERSION=1.6.14
# Thu, 17 Mar 2022 12:51:35 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Thu, 17 Mar 2022 12:55:35 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Thu, 17 Mar 2022 12:55:35 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 17 Mar 2022 12:55:36 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 17 Mar 2022 12:55:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Mar 2022 12:55:36 GMT
USER memcache
# Thu, 17 Mar 2022 12:55:36 GMT
EXPOSE 11211
# Thu, 17 Mar 2022 12:55:36 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:3d243047344378e9b7136d552d48feb7ea8b6fe14ce0990e0cc011d5e369626a`  
		Last Modified: Thu, 17 Mar 2022 04:02:41 GMT  
		Size: 2.8 MB (2812636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e26b137db66bd985a8103e3e70f8985eafa9a9ca3dc6aa33344245535f6a6b0`  
		Last Modified: Thu, 17 Mar 2022 12:56:25 GMT  
		Size: 1.3 KB (1263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5231e0cae31bc5e59bdcb40f696ceaa6b5cad70b9500bc5bfd459174ac1f78dd`  
		Last Modified: Thu, 17 Mar 2022 12:56:25 GMT  
		Size: 109.3 KB (109285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d9fab8e58febfe6f0bfb8d5bdc098221b6348a6128014c4c2b4d4086284696d`  
		Last Modified: Thu, 17 Mar 2022 12:56:25 GMT  
		Size: 938.9 KB (938943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9ca16ee180425777e36c6f23ab6755a192eedf107400360aac9332686f1212b`  
		Last Modified: Thu, 17 Mar 2022 12:56:25 GMT  
		Size: 280.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f81d444d82a8e26057630fab59b6bdb890fe42afa50edabbba60d8685e88d639`  
		Last Modified: Thu, 17 Mar 2022 12:56:24 GMT  
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
$ docker pull memcached@sha256:095e0c44c122b636ae053f2971bb454b3edfe210195707983a9e0a38d22f4411
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3754561 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d01922b70bc4d8d1d2be9eabafa82a0f0152a88e5871b7e9b6949cf1327c9c4f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 17 Mar 2022 03:19:52 GMT
ADD file:cd7d91362950471ca4678cf3833dc47119ab519dea51424c847bbbb21e1649d4 in / 
# Thu, 17 Mar 2022 03:19:52 GMT
CMD ["/bin/sh"]
# Thu, 17 Mar 2022 11:39:00 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Thu, 17 Mar 2022 11:39:02 GMT
RUN apk add --no-cache libsasl
# Thu, 17 Mar 2022 11:39:03 GMT
ENV MEMCACHED_VERSION=1.6.14
# Thu, 17 Mar 2022 11:39:04 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Thu, 17 Mar 2022 11:41:43 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Thu, 17 Mar 2022 11:41:45 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 17 Mar 2022 11:41:45 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 17 Mar 2022 11:41:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Mar 2022 11:41:47 GMT
USER memcache
# Thu, 17 Mar 2022 11:41:48 GMT
EXPOSE 11211
# Thu, 17 Mar 2022 11:41:49 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:148d739a8e6b9342daa1f5b428d3a3c6118f340f21df28c16e06f918ef150147`  
		Last Modified: Thu, 17 Mar 2022 03:20:45 GMT  
		Size: 2.7 MB (2714807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33dde588ab12fbb6aa46070a960ac850c8347e86f29744b40a123a466d4885ab`  
		Last Modified: Thu, 17 Mar 2022 11:42:57 GMT  
		Size: 1.2 KB (1240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bdeb7ac9fd9c67010a55bf3fe0e13866bb31d847353f455c95220027e2bc48c`  
		Last Modified: Thu, 17 Mar 2022 11:42:58 GMT  
		Size: 110.6 KB (110556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6bf3828467e4d3c16fcdc94bf5987db023e892ef9594c9c5dc2c3ccf07bc4bc`  
		Last Modified: Thu, 17 Mar 2022 11:42:58 GMT  
		Size: 927.5 KB (927550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d39e5be11e10e43e4991c6d85f4bdce89416e75c908d33656e4dcb79c26a51bc`  
		Last Modified: Thu, 17 Mar 2022 11:42:57 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9404edf07c113d954a0a5c34650b52d9a1f8e57d166b3e1b022a82c3e27e724`  
		Last Modified: Thu, 17 Mar 2022 11:42:57 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:alpine` - linux; 386

```console
$ docker pull memcached@sha256:8a6352e717a8080f0c0888560cf7ae52c77ee2cbd10ed46c68822370b5188d0f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3891706 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4db903b8d549ba5f131fc35c81b69bdf1822950956033492f126e16dd95b5750`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 17 Mar 2022 08:13:03 GMT
ADD file:22216bc654d9177244235f242fa83cae3b283b3c145cad7ccf11c0d29f5f0ff2 in / 
# Thu, 17 Mar 2022 08:13:03 GMT
CMD ["/bin/sh"]
# Thu, 17 Mar 2022 17:35:31 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Thu, 17 Mar 2022 17:35:32 GMT
RUN apk add --no-cache libsasl
# Thu, 17 Mar 2022 17:35:32 GMT
ENV MEMCACHED_VERSION=1.6.14
# Thu, 17 Mar 2022 17:35:33 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Thu, 17 Mar 2022 17:39:25 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Thu, 17 Mar 2022 17:39:25 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 17 Mar 2022 17:39:26 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 17 Mar 2022 17:39:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Mar 2022 17:39:26 GMT
USER memcache
# Thu, 17 Mar 2022 17:39:26 GMT
EXPOSE 11211
# Thu, 17 Mar 2022 17:39:26 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:93317a1f65ec94b67aefe728a598022610246404e3a68d391c76cd0e5244a2a0`  
		Last Modified: Thu, 17 Mar 2022 08:13:56 GMT  
		Size: 2.8 MB (2821789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae4d8e906564040308eb9f4b96b3808d37aa02b7fffa8e8d5c80126d5e50b1cf`  
		Last Modified: Thu, 17 Mar 2022 17:40:52 GMT  
		Size: 1.3 KB (1263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16143ebb273f49cf3884d5a063dfac8b30d9527c5018e90fac51ac381b5a5f8b`  
		Last Modified: Thu, 17 Mar 2022 17:40:52 GMT  
		Size: 121.2 KB (121183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:107340d48cdbc30d4b57291ca0d28997feed13517f3a508b3b398620dbc97099`  
		Last Modified: Thu, 17 Mar 2022 17:40:52 GMT  
		Size: 947.1 KB (947068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a791ada3ee704cad0a4dba90d29f533e6fcadb132c2522c38b4f0680201a86a9`  
		Last Modified: Thu, 17 Mar 2022 17:40:52 GMT  
		Size: 282.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fc23e842aa74aed8a4ea48cf2b6f027f9592e43e117c394bc70b3d2dcf0627c`  
		Last Modified: Thu, 17 Mar 2022 17:40:53 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:alpine` - linux; ppc64le

```console
$ docker pull memcached@sha256:75cb5141098fb02bb0c554c31c00d28802b414593a6b41d430c10505ee943fe0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.3 MB (5315837 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4be74852968716dd05ad711f1cda531afac5b782fe0dd6692e5aed7d91d54466`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 24 Nov 2021 20:20:16 GMT
ADD file:57115dca2eb707f46b6301e75174e6aa316fb02ac28643b91429b75be51bd8c8 in / 
# Wed, 24 Nov 2021 20:20:20 GMT
CMD ["/bin/sh"]
# Tue, 30 Nov 2021 00:52:13 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 30 Nov 2021 00:52:18 GMT
RUN apk add --no-cache libsasl
# Fri, 11 Feb 2022 23:54:02 GMT
ENV MEMCACHED_VERSION=1.6.14
# Fri, 11 Feb 2022 23:54:06 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Fri, 11 Feb 2022 23:57:48 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Fri, 11 Feb 2022 23:57:50 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 11 Feb 2022 23:57:55 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 11 Feb 2022 23:57:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Feb 2022 23:57:59 GMT
USER memcache
# Fri, 11 Feb 2022 23:58:01 GMT
EXPOSE 11211
# Fri, 11 Feb 2022 23:58:02 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:159b5dcb1717c815c76ff5ea1db730e18e8609c9090238e43282856db9e71f47`  
		Last Modified: Wed, 24 Nov 2021 20:21:14 GMT  
		Size: 2.8 MB (2814780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f44bb0dc5dc6d3634512266fffaecf643a467ef890e0a60fa7daed8a8f379335`  
		Last Modified: Tue, 30 Nov 2021 00:57:03 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:242bba95e896195e2c48210499ed8dad5c07a25a93e0d6304a787f4d5f05bb79`  
		Last Modified: Tue, 30 Nov 2021 00:57:03 GMT  
		Size: 126.2 KB (126210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9d933f0d59015113f25123de9b3460a03fdf091181f4c9330b1bb42c27a8cce`  
		Last Modified: Fri, 11 Feb 2022 23:59:16 GMT  
		Size: 2.4 MB (2373175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:659fd1f60c2bc05966f606e677370eeee3176f7d6dbd530b3f271ba313f8b0fe`  
		Last Modified: Fri, 11 Feb 2022 23:59:15 GMT  
		Size: 282.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8d9d86e7310ff252ce602224ce1643c6b8d50713444e43804cdb93912f89087`  
		Last Modified: Fri, 11 Feb 2022 23:59:15 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:alpine` - linux; s390x

```console
$ docker pull memcached@sha256:5a931719c887b04ccf389c14867075cca4a76c774ecceb8231f801d876c94be9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.7 MB (3651372 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8aed3255f32676856491e1f6e999893205a57c1d26f36d52518c7d72433bcd9c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 17 Mar 2022 03:04:28 GMT
ADD file:f623c69acb1859b41ef29e8f20f4e6c7072d9c6d7210d745afc615251bfe418f in / 
# Thu, 17 Mar 2022 03:04:28 GMT
CMD ["/bin/sh"]
# Thu, 17 Mar 2022 08:51:10 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Thu, 17 Mar 2022 08:51:11 GMT
RUN apk add --no-cache libsasl
# Thu, 17 Mar 2022 08:51:12 GMT
ENV MEMCACHED_VERSION=1.6.14
# Thu, 17 Mar 2022 08:51:12 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Thu, 17 Mar 2022 08:54:42 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Thu, 17 Mar 2022 08:54:42 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 17 Mar 2022 08:54:43 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 17 Mar 2022 08:54:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Mar 2022 08:54:43 GMT
USER memcache
# Thu, 17 Mar 2022 08:54:44 GMT
EXPOSE 11211
# Thu, 17 Mar 2022 08:54:44 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:d51040c5bfbf434887bfed2557335a411e6ef760d04cc178d455d1c3ec1b721c`  
		Last Modified: Thu, 17 Mar 2022 03:05:26 GMT  
		Size: 2.6 MB (2601715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bafa61f6f0948b111a53b71e2c8c1312981357779ca88eaf5e60d4163dc7d03b`  
		Last Modified: Thu, 17 Mar 2022 08:55:51 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6282933aed68188fd9995db64b18a466643f4879e98a97392e6df0309f825ab`  
		Last Modified: Thu, 17 Mar 2022 08:55:51 GMT  
		Size: 113.8 KB (113794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d266558ba8144540d874cf2a04b80cdad0b98138893dbd2bf8dfc0a82587d0fc`  
		Last Modified: Thu, 17 Mar 2022 08:55:51 GMT  
		Size: 934.2 KB (934189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e97cc0f7d043b7a30a2ecd4a02847ed3d1227cdec67c577b9486ae3a40bb7f55`  
		Last Modified: Thu, 17 Mar 2022 08:55:51 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:973434578ea89c81d5ee8f8c926d6efab348a190b4d1f8c59c32b595e5e3ff14`  
		Last Modified: Thu, 17 Mar 2022 08:55:51 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:alpine3.15`

```console
$ docker pull memcached@sha256:614ca36d9fbc4953da3276766de5e77bdac23c04ffcde331032be6d854006131
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
$ docker pull memcached@sha256:fd1bb2a04baff1bc63d2323d91a4f7135b9f06f1d0294fbe13b8660db7b6dd78
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3862528 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e9d7d65a6545e2698d88de0e6c6eeb620a5bdf19e35635a36ac252bb7dce9d55`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 17 Mar 2022 04:01:58 GMT
ADD file:cf4b631a115c2bbfbd81cad2d3041bceb64a8136aac92ba8a63b6c51d60af764 in / 
# Thu, 17 Mar 2022 04:01:59 GMT
CMD ["/bin/sh"]
# Thu, 17 Mar 2022 12:51:33 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Thu, 17 Mar 2022 12:51:34 GMT
RUN apk add --no-cache libsasl
# Thu, 17 Mar 2022 12:51:34 GMT
ENV MEMCACHED_VERSION=1.6.14
# Thu, 17 Mar 2022 12:51:35 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Thu, 17 Mar 2022 12:55:35 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Thu, 17 Mar 2022 12:55:35 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 17 Mar 2022 12:55:36 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 17 Mar 2022 12:55:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Mar 2022 12:55:36 GMT
USER memcache
# Thu, 17 Mar 2022 12:55:36 GMT
EXPOSE 11211
# Thu, 17 Mar 2022 12:55:36 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:3d243047344378e9b7136d552d48feb7ea8b6fe14ce0990e0cc011d5e369626a`  
		Last Modified: Thu, 17 Mar 2022 04:02:41 GMT  
		Size: 2.8 MB (2812636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e26b137db66bd985a8103e3e70f8985eafa9a9ca3dc6aa33344245535f6a6b0`  
		Last Modified: Thu, 17 Mar 2022 12:56:25 GMT  
		Size: 1.3 KB (1263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5231e0cae31bc5e59bdcb40f696ceaa6b5cad70b9500bc5bfd459174ac1f78dd`  
		Last Modified: Thu, 17 Mar 2022 12:56:25 GMT  
		Size: 109.3 KB (109285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d9fab8e58febfe6f0bfb8d5bdc098221b6348a6128014c4c2b4d4086284696d`  
		Last Modified: Thu, 17 Mar 2022 12:56:25 GMT  
		Size: 938.9 KB (938943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9ca16ee180425777e36c6f23ab6755a192eedf107400360aac9332686f1212b`  
		Last Modified: Thu, 17 Mar 2022 12:56:25 GMT  
		Size: 280.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f81d444d82a8e26057630fab59b6bdb890fe42afa50edabbba60d8685e88d639`  
		Last Modified: Thu, 17 Mar 2022 12:56:24 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:alpine3.15` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:095e0c44c122b636ae053f2971bb454b3edfe210195707983a9e0a38d22f4411
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3754561 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d01922b70bc4d8d1d2be9eabafa82a0f0152a88e5871b7e9b6949cf1327c9c4f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 17 Mar 2022 03:19:52 GMT
ADD file:cd7d91362950471ca4678cf3833dc47119ab519dea51424c847bbbb21e1649d4 in / 
# Thu, 17 Mar 2022 03:19:52 GMT
CMD ["/bin/sh"]
# Thu, 17 Mar 2022 11:39:00 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Thu, 17 Mar 2022 11:39:02 GMT
RUN apk add --no-cache libsasl
# Thu, 17 Mar 2022 11:39:03 GMT
ENV MEMCACHED_VERSION=1.6.14
# Thu, 17 Mar 2022 11:39:04 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Thu, 17 Mar 2022 11:41:43 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Thu, 17 Mar 2022 11:41:45 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 17 Mar 2022 11:41:45 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 17 Mar 2022 11:41:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Mar 2022 11:41:47 GMT
USER memcache
# Thu, 17 Mar 2022 11:41:48 GMT
EXPOSE 11211
# Thu, 17 Mar 2022 11:41:49 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:148d739a8e6b9342daa1f5b428d3a3c6118f340f21df28c16e06f918ef150147`  
		Last Modified: Thu, 17 Mar 2022 03:20:45 GMT  
		Size: 2.7 MB (2714807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33dde588ab12fbb6aa46070a960ac850c8347e86f29744b40a123a466d4885ab`  
		Last Modified: Thu, 17 Mar 2022 11:42:57 GMT  
		Size: 1.2 KB (1240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bdeb7ac9fd9c67010a55bf3fe0e13866bb31d847353f455c95220027e2bc48c`  
		Last Modified: Thu, 17 Mar 2022 11:42:58 GMT  
		Size: 110.6 KB (110556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6bf3828467e4d3c16fcdc94bf5987db023e892ef9594c9c5dc2c3ccf07bc4bc`  
		Last Modified: Thu, 17 Mar 2022 11:42:58 GMT  
		Size: 927.5 KB (927550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d39e5be11e10e43e4991c6d85f4bdce89416e75c908d33656e4dcb79c26a51bc`  
		Last Modified: Thu, 17 Mar 2022 11:42:57 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9404edf07c113d954a0a5c34650b52d9a1f8e57d166b3e1b022a82c3e27e724`  
		Last Modified: Thu, 17 Mar 2022 11:42:57 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:alpine3.15` - linux; 386

```console
$ docker pull memcached@sha256:8a6352e717a8080f0c0888560cf7ae52c77ee2cbd10ed46c68822370b5188d0f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3891706 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4db903b8d549ba5f131fc35c81b69bdf1822950956033492f126e16dd95b5750`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 17 Mar 2022 08:13:03 GMT
ADD file:22216bc654d9177244235f242fa83cae3b283b3c145cad7ccf11c0d29f5f0ff2 in / 
# Thu, 17 Mar 2022 08:13:03 GMT
CMD ["/bin/sh"]
# Thu, 17 Mar 2022 17:35:31 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Thu, 17 Mar 2022 17:35:32 GMT
RUN apk add --no-cache libsasl
# Thu, 17 Mar 2022 17:35:32 GMT
ENV MEMCACHED_VERSION=1.6.14
# Thu, 17 Mar 2022 17:35:33 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Thu, 17 Mar 2022 17:39:25 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Thu, 17 Mar 2022 17:39:25 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 17 Mar 2022 17:39:26 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 17 Mar 2022 17:39:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Mar 2022 17:39:26 GMT
USER memcache
# Thu, 17 Mar 2022 17:39:26 GMT
EXPOSE 11211
# Thu, 17 Mar 2022 17:39:26 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:93317a1f65ec94b67aefe728a598022610246404e3a68d391c76cd0e5244a2a0`  
		Last Modified: Thu, 17 Mar 2022 08:13:56 GMT  
		Size: 2.8 MB (2821789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae4d8e906564040308eb9f4b96b3808d37aa02b7fffa8e8d5c80126d5e50b1cf`  
		Last Modified: Thu, 17 Mar 2022 17:40:52 GMT  
		Size: 1.3 KB (1263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16143ebb273f49cf3884d5a063dfac8b30d9527c5018e90fac51ac381b5a5f8b`  
		Last Modified: Thu, 17 Mar 2022 17:40:52 GMT  
		Size: 121.2 KB (121183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:107340d48cdbc30d4b57291ca0d28997feed13517f3a508b3b398620dbc97099`  
		Last Modified: Thu, 17 Mar 2022 17:40:52 GMT  
		Size: 947.1 KB (947068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a791ada3ee704cad0a4dba90d29f533e6fcadb132c2522c38b4f0680201a86a9`  
		Last Modified: Thu, 17 Mar 2022 17:40:52 GMT  
		Size: 282.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fc23e842aa74aed8a4ea48cf2b6f027f9592e43e117c394bc70b3d2dcf0627c`  
		Last Modified: Thu, 17 Mar 2022 17:40:53 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:alpine3.15` - linux; ppc64le

```console
$ docker pull memcached@sha256:75cb5141098fb02bb0c554c31c00d28802b414593a6b41d430c10505ee943fe0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.3 MB (5315837 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4be74852968716dd05ad711f1cda531afac5b782fe0dd6692e5aed7d91d54466`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 24 Nov 2021 20:20:16 GMT
ADD file:57115dca2eb707f46b6301e75174e6aa316fb02ac28643b91429b75be51bd8c8 in / 
# Wed, 24 Nov 2021 20:20:20 GMT
CMD ["/bin/sh"]
# Tue, 30 Nov 2021 00:52:13 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 30 Nov 2021 00:52:18 GMT
RUN apk add --no-cache libsasl
# Fri, 11 Feb 2022 23:54:02 GMT
ENV MEMCACHED_VERSION=1.6.14
# Fri, 11 Feb 2022 23:54:06 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Fri, 11 Feb 2022 23:57:48 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Fri, 11 Feb 2022 23:57:50 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 11 Feb 2022 23:57:55 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 11 Feb 2022 23:57:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Feb 2022 23:57:59 GMT
USER memcache
# Fri, 11 Feb 2022 23:58:01 GMT
EXPOSE 11211
# Fri, 11 Feb 2022 23:58:02 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:159b5dcb1717c815c76ff5ea1db730e18e8609c9090238e43282856db9e71f47`  
		Last Modified: Wed, 24 Nov 2021 20:21:14 GMT  
		Size: 2.8 MB (2814780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f44bb0dc5dc6d3634512266fffaecf643a467ef890e0a60fa7daed8a8f379335`  
		Last Modified: Tue, 30 Nov 2021 00:57:03 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:242bba95e896195e2c48210499ed8dad5c07a25a93e0d6304a787f4d5f05bb79`  
		Last Modified: Tue, 30 Nov 2021 00:57:03 GMT  
		Size: 126.2 KB (126210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9d933f0d59015113f25123de9b3460a03fdf091181f4c9330b1bb42c27a8cce`  
		Last Modified: Fri, 11 Feb 2022 23:59:16 GMT  
		Size: 2.4 MB (2373175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:659fd1f60c2bc05966f606e677370eeee3176f7d6dbd530b3f271ba313f8b0fe`  
		Last Modified: Fri, 11 Feb 2022 23:59:15 GMT  
		Size: 282.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8d9d86e7310ff252ce602224ce1643c6b8d50713444e43804cdb93912f89087`  
		Last Modified: Fri, 11 Feb 2022 23:59:15 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:alpine3.15` - linux; s390x

```console
$ docker pull memcached@sha256:5a931719c887b04ccf389c14867075cca4a76c774ecceb8231f801d876c94be9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.7 MB (3651372 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8aed3255f32676856491e1f6e999893205a57c1d26f36d52518c7d72433bcd9c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 17 Mar 2022 03:04:28 GMT
ADD file:f623c69acb1859b41ef29e8f20f4e6c7072d9c6d7210d745afc615251bfe418f in / 
# Thu, 17 Mar 2022 03:04:28 GMT
CMD ["/bin/sh"]
# Thu, 17 Mar 2022 08:51:10 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Thu, 17 Mar 2022 08:51:11 GMT
RUN apk add --no-cache libsasl
# Thu, 17 Mar 2022 08:51:12 GMT
ENV MEMCACHED_VERSION=1.6.14
# Thu, 17 Mar 2022 08:51:12 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Thu, 17 Mar 2022 08:54:42 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Thu, 17 Mar 2022 08:54:42 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 17 Mar 2022 08:54:43 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 17 Mar 2022 08:54:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Mar 2022 08:54:43 GMT
USER memcache
# Thu, 17 Mar 2022 08:54:44 GMT
EXPOSE 11211
# Thu, 17 Mar 2022 08:54:44 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:d51040c5bfbf434887bfed2557335a411e6ef760d04cc178d455d1c3ec1b721c`  
		Last Modified: Thu, 17 Mar 2022 03:05:26 GMT  
		Size: 2.6 MB (2601715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bafa61f6f0948b111a53b71e2c8c1312981357779ca88eaf5e60d4163dc7d03b`  
		Last Modified: Thu, 17 Mar 2022 08:55:51 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6282933aed68188fd9995db64b18a466643f4879e98a97392e6df0309f825ab`  
		Last Modified: Thu, 17 Mar 2022 08:55:51 GMT  
		Size: 113.8 KB (113794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d266558ba8144540d874cf2a04b80cdad0b98138893dbd2bf8dfc0a82587d0fc`  
		Last Modified: Thu, 17 Mar 2022 08:55:51 GMT  
		Size: 934.2 KB (934189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e97cc0f7d043b7a30a2ecd4a02847ed3d1227cdec67c577b9486ae3a40bb7f55`  
		Last Modified: Thu, 17 Mar 2022 08:55:51 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:973434578ea89c81d5ee8f8c926d6efab348a190b4d1f8c59c32b595e5e3ff14`  
		Last Modified: Thu, 17 Mar 2022 08:55:51 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:bullseye`

```console
$ docker pull memcached@sha256:67ceec1841427583fd33842be1a41243351997c4803d05c14f95f0c8c6826f93
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
$ docker pull memcached@sha256:6a51dd2e23a3ead43158d3255ab8c2d9b0b2f0432becf5814c267273c84e8b6a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.0 MB (32965129 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e897df046b27f4dbfae44d31346ef91c2160a46c1b8d5bf652a40e3d76d3914f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 17 Mar 2022 04:03:59 GMT
ADD file:36919ae6bb25e3269eff949443129a01a8a43fb967fe6563939ebe1e1e9b8228 in / 
# Thu, 17 Mar 2022 04:03:59 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 12:47:26 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Thu, 17 Mar 2022 12:47:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Mar 2022 12:47:29 GMT
ENV MEMCACHED_VERSION=1.6.14
# Thu, 17 Mar 2022 12:47:29 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Thu, 17 Mar 2022 12:51:18 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 17 Mar 2022 12:51:18 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 17 Mar 2022 12:51:18 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 17 Mar 2022 12:51:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Mar 2022 12:51:18 GMT
USER memcache
# Thu, 17 Mar 2022 12:51:19 GMT
EXPOSE 11211
# Thu, 17 Mar 2022 12:51:19 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:ae13dd57832654086618a81dbc128846aa092489260c326ee95429b63c3cf213`  
		Last Modified: Thu, 17 Mar 2022 04:10:05 GMT  
		Size: 31.4 MB (31376572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c39e8a8db385456589d2009379dedc9787a9297b0ea679ff564500de9894d325`  
		Last Modified: Thu, 17 Mar 2022 12:55:59 GMT  
		Size: 5.0 KB (4982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fa3e9def276e8e73128ec9d08c6f139621666d0724b33d882ca0943a1a6825b`  
		Last Modified: Thu, 17 Mar 2022 12:55:59 GMT  
		Size: 328.0 KB (328046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9835681ca994d84f0de3da2d9ed0cdb5882c06b58bccdc406102bf4bf8a55700`  
		Last Modified: Thu, 17 Mar 2022 12:55:59 GMT  
		Size: 1.3 MB (1255121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d362d7003189fa875ec372df3c4c9622f2688adb7ed5c9cb2bec35c31b9d523`  
		Last Modified: Thu, 17 Mar 2022 12:55:59 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bd4550226c671e2d98eac87073171c925eebaa0e039ed5e2610d516980dd220`  
		Last Modified: Thu, 17 Mar 2022 12:55:59 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:bullseye` - linux; arm variant v5

```console
$ docker pull memcached@sha256:084a4198172362acf346afa27655123636800a135bdaaa857d8d57e7e402c4fa
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.5 MB (30467908 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b9e543544c3f8ef04ec918e92a8e98602cbdc37970011b5960685ffd0103780`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 17 Mar 2022 05:19:45 GMT
ADD file:1eb4f937d40230354e20e28ed781234acd4be2b0dab72f87131a3eac66349719 in / 
# Thu, 17 Mar 2022 05:19:46 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 10:06:48 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Thu, 17 Mar 2022 10:06:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Mar 2022 10:07:00 GMT
ENV MEMCACHED_VERSION=1.6.14
# Thu, 17 Mar 2022 10:07:00 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Thu, 17 Mar 2022 10:11:18 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 17 Mar 2022 10:11:18 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 17 Mar 2022 10:11:20 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 17 Mar 2022 10:11:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Mar 2022 10:11:21 GMT
USER memcache
# Thu, 17 Mar 2022 10:11:21 GMT
EXPOSE 11211
# Thu, 17 Mar 2022 10:11:21 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:4da455e7774c0e977d862a56ab6d85f33ce5dd5a77d45a0a74a272e9eae6bea0`  
		Last Modified: Thu, 17 Mar 2022 05:35:01 GMT  
		Size: 28.9 MB (28919702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39450ea3e36758cb1aaf29a3e4a3694a4f1e5d208ece3da6479b6dcd47705309`  
		Last Modified: Thu, 17 Mar 2022 10:12:14 GMT  
		Size: 4.9 KB (4890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b674f1fc0977777c240d7af9fa6d57e8b24d5332791547c80820aa9d1956d037`  
		Last Modified: Thu, 17 Mar 2022 10:12:14 GMT  
		Size: 316.6 KB (316575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de44c6f01b62d4d56baa2601e6706305eaf35c2da9541623a8c94c7fe1e4b8b2`  
		Last Modified: Thu, 17 Mar 2022 10:12:14 GMT  
		Size: 1.2 MB (1226335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18229473d3cfa938b3ba5d7f36b228bc60b7641660ae3242b56e210a50892b0f`  
		Last Modified: Thu, 17 Mar 2022 10:12:14 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e231e6a0756abb2590d1ef0507c610f0aa1b4f42e40a895d310b330662a98a2`  
		Last Modified: Thu, 17 Mar 2022 10:12:14 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:bullseye` - linux; arm variant v7

```console
$ docker pull memcached@sha256:9fe6c86dfef8c0cf535d443045364d887fd0bc8b44f550a8cbb0dca64e33e732
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.1 MB (28090226 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14dc9d69afed7832780e59eca9bf08aecbca59e357a3c301648a665b42b6659a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 17 Mar 2022 09:31:03 GMT
ADD file:e52f9ee2dc3144d7b9eb3ec90c106aa2a094eb4c5c2aa8cbff5c520a5faaef43 in / 
# Thu, 17 Mar 2022 09:31:04 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 21:53:04 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Thu, 17 Mar 2022 21:53:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Mar 2022 21:53:14 GMT
ENV MEMCACHED_VERSION=1.6.14
# Thu, 17 Mar 2022 21:53:14 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Thu, 17 Mar 2022 21:57:21 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 17 Mar 2022 21:57:22 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 17 Mar 2022 21:57:23 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 17 Mar 2022 21:57:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Mar 2022 21:57:24 GMT
USER memcache
# Thu, 17 Mar 2022 21:57:25 GMT
EXPOSE 11211
# Thu, 17 Mar 2022 21:57:25 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:5e5e708ee1f9fdbc69324391f7d1f816c657e6116eff09e7d2247fa9de3a076a`  
		Last Modified: Thu, 17 Mar 2022 09:46:33 GMT  
		Size: 26.6 MB (26575097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f652a8bcf3f50c242f3e27b3792cd55f9c0436702fe2bcdd4ae3df203aa84100`  
		Last Modified: Thu, 17 Mar 2022 22:10:19 GMT  
		Size: 4.9 KB (4896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c1be80f12d4f19157864e18689a8dd9c0f84c3a6c929949b066e7c29f30c5d7`  
		Last Modified: Thu, 17 Mar 2022 22:10:19 GMT  
		Size: 312.0 KB (311999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37ab28ddd02c6ca7832dec8a6b6508e8e4d95b34c8f4fe17457a1844c4442a7a`  
		Last Modified: Thu, 17 Mar 2022 22:10:19 GMT  
		Size: 1.2 MB (1197826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6d7e30c2d27f64a3117e85e87c00c1d4e79aa91e0bf4e4552c68d4710592d64`  
		Last Modified: Thu, 17 Mar 2022 22:10:19 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7f72f97159e0cf88a536b1a268d9bfa7af992046ce641dddb6710eabf7d08e4`  
		Last Modified: Thu, 17 Mar 2022 22:10:19 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:bullseye` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:773c0f8c11aa82d0bf14e751ab65784b8993bd7477026d660eb8e970b160aad8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.4 MB (31441503 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1cc644adcd708fa1761227654eacbdd25163b6a5a399599e20c7eabdc2a24a8f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 17 Mar 2022 03:21:57 GMT
ADD file:e52e032f1ace6abd44b3647d43c1b8ae30bac6de804eef09c6ccd793057996fd in / 
# Thu, 17 Mar 2022 03:21:58 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 11:35:48 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Thu, 17 Mar 2022 11:35:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Mar 2022 11:35:52 GMT
ENV MEMCACHED_VERSION=1.6.14
# Thu, 17 Mar 2022 11:35:53 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Thu, 17 Mar 2022 11:38:38 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 17 Mar 2022 11:38:40 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 17 Mar 2022 11:38:40 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 17 Mar 2022 11:38:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Mar 2022 11:38:42 GMT
USER memcache
# Thu, 17 Mar 2022 11:38:43 GMT
EXPOSE 11211
# Thu, 17 Mar 2022 11:38:44 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:32252aec0777ac025a158bc2a8317650a4f2a0a875387011b1165013874f8723`  
		Last Modified: Thu, 17 Mar 2022 03:28:36 GMT  
		Size: 30.1 MB (30063013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:966f1b38b9d3f62f875f8dbd868ecc80c2037b45aadbec50fc16d292be747303`  
		Last Modified: Thu, 17 Mar 2022 11:42:26 GMT  
		Size: 4.9 KB (4903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2898c9abf66c159176811eff24e689c0989d4e7c025c9a7eb0f933d356aec11`  
		Last Modified: Thu, 17 Mar 2022 11:42:26 GMT  
		Size: 119.2 KB (119181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d331819fcfc0b6541dc90aafde95bc8b8a88e453cb3800c977716cff65961a77`  
		Last Modified: Thu, 17 Mar 2022 11:42:26 GMT  
		Size: 1.3 MB (1254002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25a25819b974fbc38bad380c4df00bf1f032cf4eb0112a109c78f9858d9a0a55`  
		Last Modified: Thu, 17 Mar 2022 11:42:26 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7c790b93b28eb9ed542eac0eaf8c5fe2d4c5daa368b0f27bac067fd01bee280`  
		Last Modified: Thu, 17 Mar 2022 11:42:26 GMT  
		Size: 118.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:bullseye` - linux; 386

```console
$ docker pull memcached@sha256:3d0458851092782bb1cfb8fdb3edb27fe63775c3fb68f1879137e691de184e82
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.0 MB (33981668 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b7d3a232500fae88433d6e4117fa6e45b0ed4c529c925734eb2982bf3a3ee54`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 17 Mar 2022 08:15:53 GMT
ADD file:2d6be3846f0e5fabd85bc9409b1e2223cad4c57c76f96e9f81489ba78a72a1f5 in / 
# Thu, 17 Mar 2022 08:15:54 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 17:31:22 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Thu, 17 Mar 2022 17:31:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Mar 2022 17:31:26 GMT
ENV MEMCACHED_VERSION=1.6.14
# Thu, 17 Mar 2022 17:31:26 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Thu, 17 Mar 2022 17:35:17 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 17 Mar 2022 17:35:17 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 17 Mar 2022 17:35:18 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 17 Mar 2022 17:35:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Mar 2022 17:35:18 GMT
USER memcache
# Thu, 17 Mar 2022 17:35:18 GMT
EXPOSE 11211
# Thu, 17 Mar 2022 17:35:18 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:176085117cac9b2cf2cf57b3a10c9811dbd2773497fbac3086b5024070447e97`  
		Last Modified: Thu, 17 Mar 2022 08:24:00 GMT  
		Size: 32.4 MB (32386475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe18ed3f6ff50e5b12a7db917c34de3104619ae31e84d9d83ad2d94a3b8c5822`  
		Last Modified: Thu, 17 Mar 2022 17:40:19 GMT  
		Size: 4.9 KB (4896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc15fd9e0c057bb0a0d077f6c21d0b980b6ec5f9e5292c19d6fd790731f7bfc6`  
		Last Modified: Thu, 17 Mar 2022 17:40:19 GMT  
		Size: 336.6 KB (336638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1f8475d0ca14b4624de06fbe3207cdf07b5c31573192d0acc9b1e600b90c430`  
		Last Modified: Thu, 17 Mar 2022 17:40:20 GMT  
		Size: 1.3 MB (1253253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61e85d2ca17a8c6eb12e9cdc031a20d5c2357cf22bc4ad5353d520e13f60b73a`  
		Last Modified: Thu, 17 Mar 2022 17:40:19 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3194d39d810076bc29397aa1a117ac51d7bc610ffb9b7c90613fdf21203b05a3`  
		Last Modified: Thu, 17 Mar 2022 17:40:19 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:bullseye` - linux; mips64le

```console
$ docker pull memcached@sha256:9148cd77f369a80c3b52dd4f79ddd8073c192da135e99a311f54641a851b4b60
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.0 MB (31012937 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:16b4bbcf6270bfbe61ccbb8083bf46151a57eb6a74f044b2004509978709ee0d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 17 Mar 2022 08:53:04 GMT
ADD file:795ac4eba576bc4c995df2a18b10ce802ee8a05417cdc53f5aa09452ecf2e832 in / 
# Thu, 17 Mar 2022 08:53:08 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 20:37:19 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Thu, 17 Mar 2022 20:37:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Mar 2022 20:37:40 GMT
ENV MEMCACHED_VERSION=1.6.14
# Thu, 17 Mar 2022 20:37:43 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Thu, 17 Mar 2022 20:44:58 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 17 Mar 2022 20:45:00 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 17 Mar 2022 20:45:05 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 17 Mar 2022 20:45:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Mar 2022 20:45:10 GMT
USER memcache
# Thu, 17 Mar 2022 20:45:13 GMT
EXPOSE 11211
# Thu, 17 Mar 2022 20:45:15 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:4799d88734ae94287a665c0e14621a744706cfbe17a0cf27ae9b0cc630927b11`  
		Last Modified: Thu, 17 Mar 2022 10:43:20 GMT  
		Size: 29.6 MB (29639810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a091b8fd61b3c0cafad5676908a202cec423a829bd2fb2bb79011b3ad5fd0845`  
		Last Modified: Thu, 17 Mar 2022 20:45:41 GMT  
		Size: 4.9 KB (4859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7644e6d2f727759be27279ab11b8f3e186b6918c1b3847badb0d04ae020286b`  
		Last Modified: Thu, 17 Mar 2022 20:45:41 GMT  
		Size: 117.1 KB (117098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47e8f3183abaf23ec67f322bc78981d3c838ad27bba488ec924c07d5b1a053a4`  
		Last Modified: Thu, 17 Mar 2022 20:45:41 GMT  
		Size: 1.3 MB (1250762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f0ac34ae7971e4442dd9abb2bbfa522fc4e65445f1ed51d33795cea9b37830e`  
		Last Modified: Thu, 17 Mar 2022 20:45:40 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0564ebbfe5b917d8a4818a435ddb35d5e4bbb4b4d7187189578f1c224d10ce2b`  
		Last Modified: Thu, 17 Mar 2022 20:45:40 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:bullseye` - linux; ppc64le

```console
$ docker pull memcached@sha256:4893f4daa742b31f414b08f98f8e7d0cbedaf63b8d88062bcf3c91a9522a2aab
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.0 MB (36957544 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8db953cc998ed06712eca57fe4ae2b8bb342ce991683fd7592495a21557d0940`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 26 Jan 2022 01:46:51 GMT
ADD file:c03f34c221e57fa5cb625c166d1db9f72d6ba2fa17a3c41a5d04d6875d098949 in / 
# Wed, 26 Jan 2022 01:46:57 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 05:38:39 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 26 Jan 2022 05:38:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 11 Feb 2022 23:47:36 GMT
ENV MEMCACHED_VERSION=1.6.14
# Fri, 11 Feb 2022 23:47:38 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Fri, 11 Feb 2022 23:53:07 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Fri, 11 Feb 2022 23:53:13 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 11 Feb 2022 23:53:34 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 11 Feb 2022 23:53:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Feb 2022 23:53:39 GMT
USER memcache
# Fri, 11 Feb 2022 23:53:41 GMT
EXPOSE 11211
# Fri, 11 Feb 2022 23:53:46 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:3149ee4a73508a4c39107d64a3fdc1b021626a22a0ac95e62fa0cea49ab77fba`  
		Last Modified: Wed, 26 Jan 2022 01:57:01 GMT  
		Size: 35.3 MB (35273030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07bcb451658eb6d9eace467c2e989d96e53c409eb48347a369e9ad80aadcfe96`  
		Last Modified: Wed, 26 Jan 2022 05:45:22 GMT  
		Size: 5.0 KB (4980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8807782e060aa90873de57b2d3ec277632145f166e9c1e3801c57eea7e595cc`  
		Last Modified: Wed, 26 Jan 2022 05:45:22 GMT  
		Size: 356.9 KB (356905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5f2e5d5bb1609e336a37e97218d618550ec5ce28384c32b1141393ef6f04a03`  
		Last Modified: Fri, 11 Feb 2022 23:58:44 GMT  
		Size: 1.3 MB (1322220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76e6da4f290b1cff2fa5b1ad17d42333c67179332511db4da3bd2c5ce12bbdfa`  
		Last Modified: Fri, 11 Feb 2022 23:58:44 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fb140c5468aa121999bc169d30e4ce6b73795cdf67aa21c1dfd3d1194dd0b82`  
		Last Modified: Fri, 11 Feb 2022 23:58:44 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:bullseye` - linux; s390x

```console
$ docker pull memcached@sha256:3e4437e519528ef8d3274dfc333f59f7c8c90099329a1e041fb6a71d5be8a1c5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.2 MB (31225911 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6fbcefffe918634bf299753ebcfe4a7284155e249686c5b5db9ffa92a5c0fc87`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 17 Mar 2022 03:06:58 GMT
ADD file:52f9267b4c57ac585a0d3d47a6f2ae1a71398264173ad4f190332957fa629c67 in / 
# Thu, 17 Mar 2022 03:07:01 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 08:47:34 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Thu, 17 Mar 2022 08:47:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Mar 2022 08:47:37 GMT
ENV MEMCACHED_VERSION=1.6.14
# Thu, 17 Mar 2022 08:47:37 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Thu, 17 Mar 2022 08:50:57 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 17 Mar 2022 08:50:57 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 17 Mar 2022 08:50:58 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 17 Mar 2022 08:50:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Mar 2022 08:50:58 GMT
USER memcache
# Thu, 17 Mar 2022 08:50:58 GMT
EXPOSE 11211
# Thu, 17 Mar 2022 08:50:59 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:d101968410e5005df630b0572aec03c88de55b8de81f3cf7e6a57e1ce2e5a8e5`  
		Last Modified: Thu, 17 Mar 2022 03:12:46 GMT  
		Size: 29.7 MB (29655795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1cad003ec39dc6e2e144c0953bad3bce3807fd1679d2c9e27e510724476e1e6`  
		Last Modified: Thu, 17 Mar 2022 08:55:34 GMT  
		Size: 5.0 KB (5022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13e61c306aebe51ff20adaf4ac683a69d93022d34ed4d09bc2ae7bde9d92ba52`  
		Last Modified: Thu, 17 Mar 2022 08:55:34 GMT  
		Size: 324.1 KB (324147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b5e88f796665ba79a22e6a541cbc3f30242e708c56d6b9af4fd0a7cd23abea6`  
		Last Modified: Thu, 17 Mar 2022 08:55:34 GMT  
		Size: 1.2 MB (1240539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77d35a1cb446cb01584cfbb3a61c40aaa1f358f37c8d723fe2437e6d070dbce3`  
		Last Modified: Thu, 17 Mar 2022 08:55:34 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b237b13dadf10fc593967f3714eaab56b7b00b89d435eb7e01be3f172b5b9b69`  
		Last Modified: Thu, 17 Mar 2022 08:55:33 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:latest`

```console
$ docker pull memcached@sha256:67ceec1841427583fd33842be1a41243351997c4803d05c14f95f0c8c6826f93
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
$ docker pull memcached@sha256:6a51dd2e23a3ead43158d3255ab8c2d9b0b2f0432becf5814c267273c84e8b6a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.0 MB (32965129 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e897df046b27f4dbfae44d31346ef91c2160a46c1b8d5bf652a40e3d76d3914f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 17 Mar 2022 04:03:59 GMT
ADD file:36919ae6bb25e3269eff949443129a01a8a43fb967fe6563939ebe1e1e9b8228 in / 
# Thu, 17 Mar 2022 04:03:59 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 12:47:26 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Thu, 17 Mar 2022 12:47:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Mar 2022 12:47:29 GMT
ENV MEMCACHED_VERSION=1.6.14
# Thu, 17 Mar 2022 12:47:29 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Thu, 17 Mar 2022 12:51:18 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 17 Mar 2022 12:51:18 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 17 Mar 2022 12:51:18 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 17 Mar 2022 12:51:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Mar 2022 12:51:18 GMT
USER memcache
# Thu, 17 Mar 2022 12:51:19 GMT
EXPOSE 11211
# Thu, 17 Mar 2022 12:51:19 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:ae13dd57832654086618a81dbc128846aa092489260c326ee95429b63c3cf213`  
		Last Modified: Thu, 17 Mar 2022 04:10:05 GMT  
		Size: 31.4 MB (31376572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c39e8a8db385456589d2009379dedc9787a9297b0ea679ff564500de9894d325`  
		Last Modified: Thu, 17 Mar 2022 12:55:59 GMT  
		Size: 5.0 KB (4982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fa3e9def276e8e73128ec9d08c6f139621666d0724b33d882ca0943a1a6825b`  
		Last Modified: Thu, 17 Mar 2022 12:55:59 GMT  
		Size: 328.0 KB (328046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9835681ca994d84f0de3da2d9ed0cdb5882c06b58bccdc406102bf4bf8a55700`  
		Last Modified: Thu, 17 Mar 2022 12:55:59 GMT  
		Size: 1.3 MB (1255121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d362d7003189fa875ec372df3c4c9622f2688adb7ed5c9cb2bec35c31b9d523`  
		Last Modified: Thu, 17 Mar 2022 12:55:59 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bd4550226c671e2d98eac87073171c925eebaa0e039ed5e2610d516980dd220`  
		Last Modified: Thu, 17 Mar 2022 12:55:59 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:latest` - linux; arm variant v5

```console
$ docker pull memcached@sha256:084a4198172362acf346afa27655123636800a135bdaaa857d8d57e7e402c4fa
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.5 MB (30467908 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b9e543544c3f8ef04ec918e92a8e98602cbdc37970011b5960685ffd0103780`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 17 Mar 2022 05:19:45 GMT
ADD file:1eb4f937d40230354e20e28ed781234acd4be2b0dab72f87131a3eac66349719 in / 
# Thu, 17 Mar 2022 05:19:46 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 10:06:48 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Thu, 17 Mar 2022 10:06:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Mar 2022 10:07:00 GMT
ENV MEMCACHED_VERSION=1.6.14
# Thu, 17 Mar 2022 10:07:00 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Thu, 17 Mar 2022 10:11:18 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 17 Mar 2022 10:11:18 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 17 Mar 2022 10:11:20 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 17 Mar 2022 10:11:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Mar 2022 10:11:21 GMT
USER memcache
# Thu, 17 Mar 2022 10:11:21 GMT
EXPOSE 11211
# Thu, 17 Mar 2022 10:11:21 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:4da455e7774c0e977d862a56ab6d85f33ce5dd5a77d45a0a74a272e9eae6bea0`  
		Last Modified: Thu, 17 Mar 2022 05:35:01 GMT  
		Size: 28.9 MB (28919702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39450ea3e36758cb1aaf29a3e4a3694a4f1e5d208ece3da6479b6dcd47705309`  
		Last Modified: Thu, 17 Mar 2022 10:12:14 GMT  
		Size: 4.9 KB (4890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b674f1fc0977777c240d7af9fa6d57e8b24d5332791547c80820aa9d1956d037`  
		Last Modified: Thu, 17 Mar 2022 10:12:14 GMT  
		Size: 316.6 KB (316575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de44c6f01b62d4d56baa2601e6706305eaf35c2da9541623a8c94c7fe1e4b8b2`  
		Last Modified: Thu, 17 Mar 2022 10:12:14 GMT  
		Size: 1.2 MB (1226335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18229473d3cfa938b3ba5d7f36b228bc60b7641660ae3242b56e210a50892b0f`  
		Last Modified: Thu, 17 Mar 2022 10:12:14 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e231e6a0756abb2590d1ef0507c610f0aa1b4f42e40a895d310b330662a98a2`  
		Last Modified: Thu, 17 Mar 2022 10:12:14 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:latest` - linux; arm variant v7

```console
$ docker pull memcached@sha256:9fe6c86dfef8c0cf535d443045364d887fd0bc8b44f550a8cbb0dca64e33e732
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.1 MB (28090226 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14dc9d69afed7832780e59eca9bf08aecbca59e357a3c301648a665b42b6659a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 17 Mar 2022 09:31:03 GMT
ADD file:e52f9ee2dc3144d7b9eb3ec90c106aa2a094eb4c5c2aa8cbff5c520a5faaef43 in / 
# Thu, 17 Mar 2022 09:31:04 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 21:53:04 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Thu, 17 Mar 2022 21:53:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Mar 2022 21:53:14 GMT
ENV MEMCACHED_VERSION=1.6.14
# Thu, 17 Mar 2022 21:53:14 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Thu, 17 Mar 2022 21:57:21 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 17 Mar 2022 21:57:22 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 17 Mar 2022 21:57:23 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 17 Mar 2022 21:57:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Mar 2022 21:57:24 GMT
USER memcache
# Thu, 17 Mar 2022 21:57:25 GMT
EXPOSE 11211
# Thu, 17 Mar 2022 21:57:25 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:5e5e708ee1f9fdbc69324391f7d1f816c657e6116eff09e7d2247fa9de3a076a`  
		Last Modified: Thu, 17 Mar 2022 09:46:33 GMT  
		Size: 26.6 MB (26575097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f652a8bcf3f50c242f3e27b3792cd55f9c0436702fe2bcdd4ae3df203aa84100`  
		Last Modified: Thu, 17 Mar 2022 22:10:19 GMT  
		Size: 4.9 KB (4896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c1be80f12d4f19157864e18689a8dd9c0f84c3a6c929949b066e7c29f30c5d7`  
		Last Modified: Thu, 17 Mar 2022 22:10:19 GMT  
		Size: 312.0 KB (311999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37ab28ddd02c6ca7832dec8a6b6508e8e4d95b34c8f4fe17457a1844c4442a7a`  
		Last Modified: Thu, 17 Mar 2022 22:10:19 GMT  
		Size: 1.2 MB (1197826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6d7e30c2d27f64a3117e85e87c00c1d4e79aa91e0bf4e4552c68d4710592d64`  
		Last Modified: Thu, 17 Mar 2022 22:10:19 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7f72f97159e0cf88a536b1a268d9bfa7af992046ce641dddb6710eabf7d08e4`  
		Last Modified: Thu, 17 Mar 2022 22:10:19 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:latest` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:773c0f8c11aa82d0bf14e751ab65784b8993bd7477026d660eb8e970b160aad8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.4 MB (31441503 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1cc644adcd708fa1761227654eacbdd25163b6a5a399599e20c7eabdc2a24a8f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 17 Mar 2022 03:21:57 GMT
ADD file:e52e032f1ace6abd44b3647d43c1b8ae30bac6de804eef09c6ccd793057996fd in / 
# Thu, 17 Mar 2022 03:21:58 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 11:35:48 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Thu, 17 Mar 2022 11:35:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Mar 2022 11:35:52 GMT
ENV MEMCACHED_VERSION=1.6.14
# Thu, 17 Mar 2022 11:35:53 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Thu, 17 Mar 2022 11:38:38 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 17 Mar 2022 11:38:40 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 17 Mar 2022 11:38:40 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 17 Mar 2022 11:38:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Mar 2022 11:38:42 GMT
USER memcache
# Thu, 17 Mar 2022 11:38:43 GMT
EXPOSE 11211
# Thu, 17 Mar 2022 11:38:44 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:32252aec0777ac025a158bc2a8317650a4f2a0a875387011b1165013874f8723`  
		Last Modified: Thu, 17 Mar 2022 03:28:36 GMT  
		Size: 30.1 MB (30063013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:966f1b38b9d3f62f875f8dbd868ecc80c2037b45aadbec50fc16d292be747303`  
		Last Modified: Thu, 17 Mar 2022 11:42:26 GMT  
		Size: 4.9 KB (4903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2898c9abf66c159176811eff24e689c0989d4e7c025c9a7eb0f933d356aec11`  
		Last Modified: Thu, 17 Mar 2022 11:42:26 GMT  
		Size: 119.2 KB (119181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d331819fcfc0b6541dc90aafde95bc8b8a88e453cb3800c977716cff65961a77`  
		Last Modified: Thu, 17 Mar 2022 11:42:26 GMT  
		Size: 1.3 MB (1254002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25a25819b974fbc38bad380c4df00bf1f032cf4eb0112a109c78f9858d9a0a55`  
		Last Modified: Thu, 17 Mar 2022 11:42:26 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7c790b93b28eb9ed542eac0eaf8c5fe2d4c5daa368b0f27bac067fd01bee280`  
		Last Modified: Thu, 17 Mar 2022 11:42:26 GMT  
		Size: 118.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:latest` - linux; 386

```console
$ docker pull memcached@sha256:3d0458851092782bb1cfb8fdb3edb27fe63775c3fb68f1879137e691de184e82
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.0 MB (33981668 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b7d3a232500fae88433d6e4117fa6e45b0ed4c529c925734eb2982bf3a3ee54`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 17 Mar 2022 08:15:53 GMT
ADD file:2d6be3846f0e5fabd85bc9409b1e2223cad4c57c76f96e9f81489ba78a72a1f5 in / 
# Thu, 17 Mar 2022 08:15:54 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 17:31:22 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Thu, 17 Mar 2022 17:31:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Mar 2022 17:31:26 GMT
ENV MEMCACHED_VERSION=1.6.14
# Thu, 17 Mar 2022 17:31:26 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Thu, 17 Mar 2022 17:35:17 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 17 Mar 2022 17:35:17 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 17 Mar 2022 17:35:18 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 17 Mar 2022 17:35:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Mar 2022 17:35:18 GMT
USER memcache
# Thu, 17 Mar 2022 17:35:18 GMT
EXPOSE 11211
# Thu, 17 Mar 2022 17:35:18 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:176085117cac9b2cf2cf57b3a10c9811dbd2773497fbac3086b5024070447e97`  
		Last Modified: Thu, 17 Mar 2022 08:24:00 GMT  
		Size: 32.4 MB (32386475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe18ed3f6ff50e5b12a7db917c34de3104619ae31e84d9d83ad2d94a3b8c5822`  
		Last Modified: Thu, 17 Mar 2022 17:40:19 GMT  
		Size: 4.9 KB (4896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc15fd9e0c057bb0a0d077f6c21d0b980b6ec5f9e5292c19d6fd790731f7bfc6`  
		Last Modified: Thu, 17 Mar 2022 17:40:19 GMT  
		Size: 336.6 KB (336638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1f8475d0ca14b4624de06fbe3207cdf07b5c31573192d0acc9b1e600b90c430`  
		Last Modified: Thu, 17 Mar 2022 17:40:20 GMT  
		Size: 1.3 MB (1253253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61e85d2ca17a8c6eb12e9cdc031a20d5c2357cf22bc4ad5353d520e13f60b73a`  
		Last Modified: Thu, 17 Mar 2022 17:40:19 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3194d39d810076bc29397aa1a117ac51d7bc610ffb9b7c90613fdf21203b05a3`  
		Last Modified: Thu, 17 Mar 2022 17:40:19 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:latest` - linux; mips64le

```console
$ docker pull memcached@sha256:9148cd77f369a80c3b52dd4f79ddd8073c192da135e99a311f54641a851b4b60
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.0 MB (31012937 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:16b4bbcf6270bfbe61ccbb8083bf46151a57eb6a74f044b2004509978709ee0d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 17 Mar 2022 08:53:04 GMT
ADD file:795ac4eba576bc4c995df2a18b10ce802ee8a05417cdc53f5aa09452ecf2e832 in / 
# Thu, 17 Mar 2022 08:53:08 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 20:37:19 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Thu, 17 Mar 2022 20:37:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Mar 2022 20:37:40 GMT
ENV MEMCACHED_VERSION=1.6.14
# Thu, 17 Mar 2022 20:37:43 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Thu, 17 Mar 2022 20:44:58 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 17 Mar 2022 20:45:00 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 17 Mar 2022 20:45:05 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 17 Mar 2022 20:45:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Mar 2022 20:45:10 GMT
USER memcache
# Thu, 17 Mar 2022 20:45:13 GMT
EXPOSE 11211
# Thu, 17 Mar 2022 20:45:15 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:4799d88734ae94287a665c0e14621a744706cfbe17a0cf27ae9b0cc630927b11`  
		Last Modified: Thu, 17 Mar 2022 10:43:20 GMT  
		Size: 29.6 MB (29639810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a091b8fd61b3c0cafad5676908a202cec423a829bd2fb2bb79011b3ad5fd0845`  
		Last Modified: Thu, 17 Mar 2022 20:45:41 GMT  
		Size: 4.9 KB (4859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7644e6d2f727759be27279ab11b8f3e186b6918c1b3847badb0d04ae020286b`  
		Last Modified: Thu, 17 Mar 2022 20:45:41 GMT  
		Size: 117.1 KB (117098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47e8f3183abaf23ec67f322bc78981d3c838ad27bba488ec924c07d5b1a053a4`  
		Last Modified: Thu, 17 Mar 2022 20:45:41 GMT  
		Size: 1.3 MB (1250762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f0ac34ae7971e4442dd9abb2bbfa522fc4e65445f1ed51d33795cea9b37830e`  
		Last Modified: Thu, 17 Mar 2022 20:45:40 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0564ebbfe5b917d8a4818a435ddb35d5e4bbb4b4d7187189578f1c224d10ce2b`  
		Last Modified: Thu, 17 Mar 2022 20:45:40 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:latest` - linux; ppc64le

```console
$ docker pull memcached@sha256:4893f4daa742b31f414b08f98f8e7d0cbedaf63b8d88062bcf3c91a9522a2aab
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.0 MB (36957544 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8db953cc998ed06712eca57fe4ae2b8bb342ce991683fd7592495a21557d0940`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 26 Jan 2022 01:46:51 GMT
ADD file:c03f34c221e57fa5cb625c166d1db9f72d6ba2fa17a3c41a5d04d6875d098949 in / 
# Wed, 26 Jan 2022 01:46:57 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 05:38:39 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 26 Jan 2022 05:38:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 11 Feb 2022 23:47:36 GMT
ENV MEMCACHED_VERSION=1.6.14
# Fri, 11 Feb 2022 23:47:38 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Fri, 11 Feb 2022 23:53:07 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Fri, 11 Feb 2022 23:53:13 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 11 Feb 2022 23:53:34 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 11 Feb 2022 23:53:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Feb 2022 23:53:39 GMT
USER memcache
# Fri, 11 Feb 2022 23:53:41 GMT
EXPOSE 11211
# Fri, 11 Feb 2022 23:53:46 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:3149ee4a73508a4c39107d64a3fdc1b021626a22a0ac95e62fa0cea49ab77fba`  
		Last Modified: Wed, 26 Jan 2022 01:57:01 GMT  
		Size: 35.3 MB (35273030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07bcb451658eb6d9eace467c2e989d96e53c409eb48347a369e9ad80aadcfe96`  
		Last Modified: Wed, 26 Jan 2022 05:45:22 GMT  
		Size: 5.0 KB (4980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8807782e060aa90873de57b2d3ec277632145f166e9c1e3801c57eea7e595cc`  
		Last Modified: Wed, 26 Jan 2022 05:45:22 GMT  
		Size: 356.9 KB (356905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5f2e5d5bb1609e336a37e97218d618550ec5ce28384c32b1141393ef6f04a03`  
		Last Modified: Fri, 11 Feb 2022 23:58:44 GMT  
		Size: 1.3 MB (1322220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76e6da4f290b1cff2fa5b1ad17d42333c67179332511db4da3bd2c5ce12bbdfa`  
		Last Modified: Fri, 11 Feb 2022 23:58:44 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fb140c5468aa121999bc169d30e4ce6b73795cdf67aa21c1dfd3d1194dd0b82`  
		Last Modified: Fri, 11 Feb 2022 23:58:44 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:latest` - linux; s390x

```console
$ docker pull memcached@sha256:3e4437e519528ef8d3274dfc333f59f7c8c90099329a1e041fb6a71d5be8a1c5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.2 MB (31225911 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6fbcefffe918634bf299753ebcfe4a7284155e249686c5b5db9ffa92a5c0fc87`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 17 Mar 2022 03:06:58 GMT
ADD file:52f9267b4c57ac585a0d3d47a6f2ae1a71398264173ad4f190332957fa629c67 in / 
# Thu, 17 Mar 2022 03:07:01 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 08:47:34 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Thu, 17 Mar 2022 08:47:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Mar 2022 08:47:37 GMT
ENV MEMCACHED_VERSION=1.6.14
# Thu, 17 Mar 2022 08:47:37 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Thu, 17 Mar 2022 08:50:57 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 17 Mar 2022 08:50:57 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 17 Mar 2022 08:50:58 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 17 Mar 2022 08:50:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Mar 2022 08:50:58 GMT
USER memcache
# Thu, 17 Mar 2022 08:50:58 GMT
EXPOSE 11211
# Thu, 17 Mar 2022 08:50:59 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:d101968410e5005df630b0572aec03c88de55b8de81f3cf7e6a57e1ce2e5a8e5`  
		Last Modified: Thu, 17 Mar 2022 03:12:46 GMT  
		Size: 29.7 MB (29655795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1cad003ec39dc6e2e144c0953bad3bce3807fd1679d2c9e27e510724476e1e6`  
		Last Modified: Thu, 17 Mar 2022 08:55:34 GMT  
		Size: 5.0 KB (5022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13e61c306aebe51ff20adaf4ac683a69d93022d34ed4d09bc2ae7bde9d92ba52`  
		Last Modified: Thu, 17 Mar 2022 08:55:34 GMT  
		Size: 324.1 KB (324147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b5e88f796665ba79a22e6a541cbc3f30242e708c56d6b9af4fd0a7cd23abea6`  
		Last Modified: Thu, 17 Mar 2022 08:55:34 GMT  
		Size: 1.2 MB (1240539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77d35a1cb446cb01584cfbb3a61c40aaa1f358f37c8d723fe2437e6d070dbce3`  
		Last Modified: Thu, 17 Mar 2022 08:55:34 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b237b13dadf10fc593967f3714eaab56b7b00b89d435eb7e01be3f172b5b9b69`  
		Last Modified: Thu, 17 Mar 2022 08:55:33 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
