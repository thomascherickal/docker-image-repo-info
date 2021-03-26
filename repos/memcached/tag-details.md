<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `memcached`

-	[`memcached:1`](#memcached1)
-	[`memcached:1-alpine`](#memcached1-alpine)
-	[`memcached:1.6`](#memcached16)
-	[`memcached:1.6-alpine`](#memcached16-alpine)
-	[`memcached:1.6.9`](#memcached169)
-	[`memcached:1.6.9-alpine`](#memcached169-alpine)
-	[`memcached:alpine`](#memcachedalpine)
-	[`memcached:latest`](#memcachedlatest)

## `memcached:1`

```console
$ docker pull memcached@sha256:aedbed05133579a286baaffce576b360a3860b5644d7e4bd39e8d0a26b847801
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
$ docker pull memcached@sha256:d8559d4ca748485fe7acf3bda5634902385c393b56991153d3259b1919b667b6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.5 MB (30510071 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c17a0df7f0b4ead3f7992531505b74f08210e464636782ff8d4e9f9c3f9ab634`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 12 Mar 2021 02:20:40 GMT
ADD file:3c32f1cd03198e141dd233a7ffd13444157d4150ad917d548f3ee9bf5953ce22 in / 
# Fri, 12 Mar 2021 02:20:41 GMT
CMD ["bash"]
# Sat, 13 Mar 2021 03:51:06 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Sat, 13 Mar 2021 03:51:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 13 Mar 2021 03:51:12 GMT
ENV MEMCACHED_VERSION=1.6.9
# Sat, 13 Mar 2021 03:51:12 GMT
ENV MEMCACHED_SHA1=42ae062094fdf083cfe7b21ff377c781011c2be1
# Sat, 13 Mar 2021 03:55:02 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Sat, 13 Mar 2021 03:55:03 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Sat, 13 Mar 2021 03:55:04 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Sat, 13 Mar 2021 03:55:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 13 Mar 2021 03:55:04 GMT
USER memcache
# Sat, 13 Mar 2021 03:55:04 GMT
EXPOSE 11211
# Sat, 13 Mar 2021 03:55:05 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:6f28985ad1843afd6fd4fe0b42a30bfab63c27d302362e7341e3316e8ba25ced`  
		Last Modified: Fri, 12 Mar 2021 02:26:11 GMT  
		Size: 27.1 MB (27101001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:007083158c847935c98d2d8c07518c8097b91da3a2fd7e15a6dbbb5f7e3de5e4`  
		Last Modified: Sat, 13 Mar 2021 03:59:56 GMT  
		Size: 5.0 KB (4977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44f9cc8fbeb0c17485aa8956f8ad64a7c24d44af44ea7b4883955f47996b189d`  
		Last Modified: Sat, 13 Mar 2021 03:59:57 GMT  
		Size: 2.2 MB (2197036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:955c0e8ce2a3821077059bb8198bc27098ef46dda29831d180cdc995186b345a`  
		Last Modified: Sat, 13 Mar 2021 03:59:56 GMT  
		Size: 1.2 MB (1206649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d8cc0a86221ff10b28b1a07db34deda0dfbc8f255f8a0911c518d91e2f84eba`  
		Last Modified: Sat, 13 Mar 2021 03:59:56 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7156f15be6833cf1ea0a3172ebe80928e5622768ad50c17b274b6004b6cc080`  
		Last Modified: Sat, 13 Mar 2021 03:59:56 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1` - linux; arm variant v5

```console
$ docker pull memcached@sha256:14a89ab8a75e421a79f0e3e65074b106d8b03e9b45fc0b6ff3ca1f7843e2176a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.9 MB (27928037 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a715778439ac19faacf97a009883e33c115543fe3a0f0deace9db3705ea9a7a2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 26 Mar 2021 07:51:46 GMT
ADD file:3dd25698bf1578e8580b2f437a2199bfc3b1818480b874d73622357e955a091f in / 
# Fri, 26 Mar 2021 07:51:48 GMT
CMD ["bash"]
# Fri, 26 Mar 2021 09:39:21 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Fri, 26 Mar 2021 09:39:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 09:39:34 GMT
ENV MEMCACHED_VERSION=1.6.9
# Fri, 26 Mar 2021 09:39:34 GMT
ENV MEMCACHED_SHA1=42ae062094fdf083cfe7b21ff377c781011c2be1
# Fri, 26 Mar 2021 09:43:40 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Fri, 26 Mar 2021 09:43:41 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 26 Mar 2021 09:43:44 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 26 Mar 2021 09:43:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 09:43:46 GMT
USER memcache
# Fri, 26 Mar 2021 09:43:47 GMT
EXPOSE 11211
# Fri, 26 Mar 2021 09:43:47 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:997e59852ec0e1a23e4a179db14793947d60390c392ce15abc0f811e797c49ca`  
		Last Modified: Fri, 26 Mar 2021 08:00:22 GMT  
		Size: 24.8 MB (24846159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bac4aeb1ec3f8bad5601293e2e6ee4892f2099bcdf754eca5a256713b4f4ac78`  
		Last Modified: Fri, 26 Mar 2021 09:44:00 GMT  
		Size: 4.9 KB (4893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c690f09a614f96a09cf57ab424bb57e240adc3cbfd1cc08482f124a479fad552`  
		Last Modified: Fri, 26 Mar 2021 09:44:02 GMT  
		Size: 1.9 MB (1897339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d144d9a91ac96cb9c068f67fc5649459003e9f9a21867638fb49840ed9e85e0`  
		Last Modified: Fri, 26 Mar 2021 09:44:01 GMT  
		Size: 1.2 MB (1179238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3160a064a6625a7ec9c8959cd13f6e9113a5c2cb59cbe8ea826ce8a210068b7e`  
		Last Modified: Fri, 26 Mar 2021 09:44:00 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e4455ba84cf78688e072088f68b9c85bc29af1a497039b5241c6291b5de1843`  
		Last Modified: Fri, 26 Mar 2021 09:44:00 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1` - linux; arm variant v7

```console
$ docker pull memcached@sha256:ca79781006a7d45818e0e9b0d51c954c9c9c4bde8336060bf04fc99cbd7809e3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.7 MB (25676128 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b26ff179f940a940395fc620c44eff4702a61bc989da3d71d318bc699dd4ed08`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 12 Mar 2021 02:00:12 GMT
ADD file:123da9848f87c8ed4c5122a104b8650564c09767725916f822def7b645a019f1 in / 
# Fri, 12 Mar 2021 02:00:14 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 03:08:21 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Fri, 12 Mar 2021 03:08:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 03:08:32 GMT
ENV MEMCACHED_VERSION=1.6.9
# Fri, 12 Mar 2021 03:08:33 GMT
ENV MEMCACHED_SHA1=42ae062094fdf083cfe7b21ff377c781011c2be1
# Fri, 12 Mar 2021 03:11:57 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Fri, 12 Mar 2021 03:11:58 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 12 Mar 2021 03:12:01 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 12 Mar 2021 03:12:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 12 Mar 2021 03:12:03 GMT
USER memcache
# Fri, 12 Mar 2021 03:12:04 GMT
EXPOSE 11211
# Fri, 12 Mar 2021 03:12:05 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:e12d26f75fe8b7fd14712965ff5178762227d07d2151bb35fa21105ddfc4a14a`  
		Last Modified: Fri, 12 Mar 2021 02:10:28 GMT  
		Size: 22.7 MB (22709467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe1e03071b3302ec91defd6b8b861a3be2a50d7165f73c154eea0ddd8339641a`  
		Last Modified: Fri, 12 Mar 2021 03:22:32 GMT  
		Size: 4.9 KB (4899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b11c24c5a0d1d4fa06df54624b6dc7a5d1586210047c31e44511fa513081a49e`  
		Last Modified: Fri, 12 Mar 2021 03:22:33 GMT  
		Size: 1.8 MB (1811657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57458ecd2770995b21c7c8d20108d84bc9b4879cd759054d4f8e122bb54a7451`  
		Last Modified: Fri, 12 Mar 2021 03:22:32 GMT  
		Size: 1.1 MB (1149703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6070aa36c0112c5a66ad85b5eaa4e4c954a217f484a915ff259fd30c5de332e6`  
		Last Modified: Fri, 12 Mar 2021 03:22:32 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1d498de6ccd0c3ffc78632677c24cad8f6acc9add31d9ef7fd69d57144fb0f4`  
		Last Modified: Fri, 12 Mar 2021 03:22:32 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:fe157d34ccde3aa160d90472f6964aaca3c6b0554f2fa4317d8afceeff3c45cc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.1 MB (29116090 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d61a16162561c8b05c0af58a2555c292980d12cc41872efa2096ed9109377dee`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 12 Mar 2021 01:53:53 GMT
ADD file:6130ddc0a939dd72c0614de4aa77de47aa16fe211274bacb31995aa1a0526164 in / 
# Fri, 12 Mar 2021 01:53:56 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 05:45:15 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Fri, 12 Mar 2021 05:45:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 05:45:27 GMT
ENV MEMCACHED_VERSION=1.6.9
# Fri, 12 Mar 2021 05:45:28 GMT
ENV MEMCACHED_SHA1=42ae062094fdf083cfe7b21ff377c781011c2be1
# Fri, 12 Mar 2021 05:48:54 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Fri, 12 Mar 2021 05:48:55 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 12 Mar 2021 05:48:57 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 12 Mar 2021 05:48:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 12 Mar 2021 05:48:59 GMT
USER memcache
# Fri, 12 Mar 2021 05:49:00 GMT
EXPOSE 11211
# Fri, 12 Mar 2021 05:49:00 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:706ee5d0a6b53d9257cbea22d8409fb22c867ab3a001c65f6b8bfd37dace0e58`  
		Last Modified: Fri, 12 Mar 2021 02:01:39 GMT  
		Size: 25.9 MB (25856512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0d9e24f3287f849ddf4e4afe2c8fca91a1031b67a267cd2c779ac2592d59bdf`  
		Last Modified: Fri, 12 Mar 2021 05:49:32 GMT  
		Size: 5.0 KB (5022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c00635c3d3412e964343152daaa8d6a574cff4476029d2dde8fbef8669643dd`  
		Last Modified: Fri, 12 Mar 2021 05:49:33 GMT  
		Size: 2.1 MB (2075174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42b36f1c725910664c120ab3e1137c10c516bc764114217862137f86de0b0a96`  
		Last Modified: Fri, 12 Mar 2021 05:49:32 GMT  
		Size: 1.2 MB (1178974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec7c9cae013d3da2b75c61f808eb35db46f6ea8b4aec6a394c20f9b42341f46c`  
		Last Modified: Fri, 12 Mar 2021 05:49:32 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccaed15ca3b93815844f5b39c66fe6edae8ec39ae3a186a3470e9c8f53909018`  
		Last Modified: Fri, 12 Mar 2021 05:49:32 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1` - linux; 386

```console
$ docker pull memcached@sha256:ef0460019399121409cd24063e18f58e7f89f6c6dd0c9e6405441876555dfc21
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.2 MB (31178982 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91f0b8c30945bbb159fc82df44b331add3a586ea0e9d264dd6e26e9733278cb4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 12 Mar 2021 01:44:27 GMT
ADD file:90c103e04bd6fe0f39733cbf8eb2d8845aed3e4fc3fd1e5c3354df69e40aa615 in / 
# Fri, 12 Mar 2021 01:44:28 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 13:31:23 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Fri, 12 Mar 2021 13:31:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 13:31:28 GMT
ENV MEMCACHED_VERSION=1.6.9
# Fri, 12 Mar 2021 13:31:28 GMT
ENV MEMCACHED_SHA1=42ae062094fdf083cfe7b21ff377c781011c2be1
# Fri, 12 Mar 2021 13:35:32 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Fri, 12 Mar 2021 13:35:32 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 12 Mar 2021 13:35:33 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 12 Mar 2021 13:35:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 12 Mar 2021 13:35:33 GMT
USER memcache
# Fri, 12 Mar 2021 13:35:33 GMT
EXPOSE 11211
# Fri, 12 Mar 2021 13:35:34 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:0898aa7472f57f223652846337cf862f142e109d0c039b41886e7f20c345f85e`  
		Last Modified: Fri, 12 Mar 2021 01:52:08 GMT  
		Size: 27.8 MB (27760948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f32ccac2f28603415b89f000eac53a764ccb5e4a5c7bb96f531886d346046066`  
		Last Modified: Fri, 12 Mar 2021 13:40:40 GMT  
		Size: 4.9 KB (4895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ca797dc44ad9702a16634c4e34b2809570c531a00ea77bc688afbc168ef7ee4`  
		Last Modified: Fri, 12 Mar 2021 13:40:41 GMT  
		Size: 2.2 MB (2208684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e11aea04bae299d4a9ad55384df0c485fc53e5a9ca08c49f9905056753b6d4e6`  
		Last Modified: Fri, 12 Mar 2021 13:40:41 GMT  
		Size: 1.2 MB (1204047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1793a72e67f7bf9006a9aa26f1c569f4f92bc9ac6d93ea73f96d8a05bfd5e0a6`  
		Last Modified: Fri, 12 Mar 2021 13:40:40 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:999651c299c9f7bd71c0b15ecb302b22f3f03f36924d3144b76eb81e619d0184`  
		Last Modified: Fri, 12 Mar 2021 13:40:40 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1` - linux; mips64le

```console
$ docker pull memcached@sha256:8ea232e21a6f020459a12dd1d7aedc8474594927363ba4aec07ce413deb9bed5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.8 MB (28752902 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:068f62f8ad395edfb2fda7af67488827096540267d3151dc47631195b1fc9543`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 12 Mar 2021 02:10:02 GMT
ADD file:491c5ca15fe098b83de42861289c216c693d788a1f9e739a78acefb0cad453c8 in / 
# Fri, 12 Mar 2021 02:10:03 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 08:46:26 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Fri, 12 Mar 2021 08:46:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 08:46:39 GMT
ENV MEMCACHED_VERSION=1.6.9
# Fri, 12 Mar 2021 08:46:39 GMT
ENV MEMCACHED_SHA1=42ae062094fdf083cfe7b21ff377c781011c2be1
# Fri, 12 Mar 2021 08:52:26 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Fri, 12 Mar 2021 08:52:27 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 12 Mar 2021 08:52:28 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 12 Mar 2021 08:52:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 12 Mar 2021 08:52:29 GMT
USER memcache
# Fri, 12 Mar 2021 08:52:29 GMT
EXPOSE 11211
# Fri, 12 Mar 2021 08:52:30 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:d0b6b2cc51bdde474395b8c32ff8012e471727bba69f221cfb79b46e8283f047`  
		Last Modified: Fri, 12 Mar 2021 02:17:07 GMT  
		Size: 25.8 MB (25772338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22086edc87e18d40945456938ba809ad0b1153dcf874df2911314f3fa0d76667`  
		Last Modified: Fri, 12 Mar 2021 08:52:45 GMT  
		Size: 5.0 KB (4978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b808a76ea31d9ba92e88100192f485f4efc2f9c15b24c41990aa202a0ed1a508`  
		Last Modified: Fri, 12 Mar 2021 08:52:46 GMT  
		Size: 1.8 MB (1776385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afada1a8592c3da748b0b5ac6d6a4db3f02704fb3785a7e1cc13a6b4fd5b1010`  
		Last Modified: Fri, 12 Mar 2021 08:52:46 GMT  
		Size: 1.2 MB (1198794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:276d546ec9c236bf7813ab6f11ccc55c6e127f0ea72ccbb36c035dbe52d675f6`  
		Last Modified: Fri, 12 Mar 2021 08:52:45 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a11a440437df39f7b30113415724385ba8643faf61547a4148083c19dd934eaa`  
		Last Modified: Fri, 12 Mar 2021 08:52:45 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1` - linux; ppc64le

```console
$ docker pull memcached@sha256:efd3d67a1afd293b38dc0ebf78641266104fa8f44735e0b6210117d914f67250
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.1 MB (34087167 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:95699b572190f07b90f87f36f5f2e01c0073b7ac7241544c9c5d156985b817b4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 12 Mar 2021 02:32:43 GMT
ADD file:6a0c0cfa71979cf6fdd859dce1e32582f0e55ed382b9e17b77a2001defc2c9db in / 
# Fri, 12 Mar 2021 02:32:50 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 05:42:18 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Fri, 12 Mar 2021 05:42:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 05:42:50 GMT
ENV MEMCACHED_VERSION=1.6.9
# Fri, 12 Mar 2021 05:42:55 GMT
ENV MEMCACHED_SHA1=42ae062094fdf083cfe7b21ff377c781011c2be1
# Fri, 12 Mar 2021 05:51:27 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Fri, 12 Mar 2021 05:51:31 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 12 Mar 2021 05:51:53 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 12 Mar 2021 05:51:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 12 Mar 2021 05:52:07 GMT
USER memcache
# Fri, 12 Mar 2021 05:52:14 GMT
EXPOSE 11211
# Fri, 12 Mar 2021 05:52:21 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:1d686056fdac1848f4fd78ba2b335502055ffe98c79619e21d0c2fb7db95257e`  
		Last Modified: Fri, 12 Mar 2021 02:45:35 GMT  
		Size: 30.5 MB (30525728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73b1efcdfc9b290f77d5235f4f3bec7b09d62026296bb6dfccbdba7354df9caa`  
		Last Modified: Fri, 12 Mar 2021 05:52:55 GMT  
		Size: 5.0 KB (4994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0ae8f3e8315ccb25bd80ff467115a6f3479c6b5acf818ad7e3fcf4af0b2ebe1`  
		Last Modified: Fri, 12 Mar 2021 05:52:56 GMT  
		Size: 2.3 MB (2323017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0f34bd86e0ac5d50a3f227ab5cc3190a8a0973ea12c7e827d9267cad4dad482`  
		Last Modified: Fri, 12 Mar 2021 05:52:55 GMT  
		Size: 1.2 MB (1233020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a188c62ab305cd93f469a414ef7da5b0f1c3e66817ea0439a7530e194f90d05f`  
		Last Modified: Fri, 12 Mar 2021 05:52:55 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b5898f549c8d0705d12413acbc320c216d8a65dd1c312d1da6e8fe53df526e6`  
		Last Modified: Fri, 12 Mar 2021 05:52:55 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1` - linux; s390x

```console
$ docker pull memcached@sha256:5e844fb7cd8aa06589f899a421921d452ade52de1e969ae763d60fecece294e9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.8 MB (28806644 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e79898684368a64d853c29bb82cfb9688df1e0230116c145e7f137796fb3eb4f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 12 Mar 2021 01:46:04 GMT
ADD file:afec039adf230a9186a38b57eed85262696f8d178ac649a445657066f16fe806 in / 
# Fri, 12 Mar 2021 01:46:07 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 02:55:40 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Fri, 12 Mar 2021 02:55:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 02:55:46 GMT
ENV MEMCACHED_VERSION=1.6.9
# Fri, 12 Mar 2021 02:55:46 GMT
ENV MEMCACHED_SHA1=42ae062094fdf083cfe7b21ff377c781011c2be1
# Fri, 12 Mar 2021 02:59:29 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Fri, 12 Mar 2021 02:59:29 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 12 Mar 2021 02:59:30 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 12 Mar 2021 02:59:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 12 Mar 2021 02:59:31 GMT
USER memcache
# Fri, 12 Mar 2021 02:59:31 GMT
EXPOSE 11211
# Fri, 12 Mar 2021 02:59:31 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:d41215965c091534e809ab2e8f4a2c1cebee3de536c2c74a7bc8302bbc8af7e1`  
		Last Modified: Fri, 12 Mar 2021 01:50:30 GMT  
		Size: 25.7 MB (25716294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c86c43c934421c76725f64bbc35ebb36c5f5c8dd181f6f701101068a31671d10`  
		Last Modified: Fri, 12 Mar 2021 02:59:59 GMT  
		Size: 5.0 KB (5025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97631e025d45847d90b38975ee3e031618e6eeedc1077b6ab77612d1edcda2e5`  
		Last Modified: Fri, 12 Mar 2021 02:59:59 GMT  
		Size: 1.9 MB (1886402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e98fc6e9a78adb22f7fb53ccc28169914f61a8f89c7c414f8d7b7eb22460b5f2`  
		Last Modified: Fri, 12 Mar 2021 02:59:59 GMT  
		Size: 1.2 MB (1198516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f9b27ffa18edb87e225a25d6bba459f4ae8a473944cebb847fe0e13a78e84fa`  
		Last Modified: Fri, 12 Mar 2021 02:59:59 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82ff067463b04909884ea6e0adda53fb48c398ee27e4ea1ae7de1dc5d5107151`  
		Last Modified: Fri, 12 Mar 2021 02:59:59 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:1-alpine`

```console
$ docker pull memcached@sha256:a1a84ac6bba5b100e79cff5819072ea05815a3597af2611713313ff77df7b799
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
$ docker pull memcached@sha256:e799e863cd8dd7c6143457541d4e881f29d2a8cc7cf36a9e73afc075b88eaf66
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3835911 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:336eae34e88e7f26ba0efae7e37fae40bf1ec0752a3dd074d2bce3a5be74de7b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 25 Mar 2021 22:19:32 GMT
ADD file:6b081cabb4b256ee07587d249c4989b5b679375529542b81550a65b6f19f274e in / 
# Thu, 25 Mar 2021 22:19:32 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 09:38:12 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Fri, 26 Mar 2021 09:38:13 GMT
RUN apk add --no-cache libsasl
# Fri, 26 Mar 2021 09:38:13 GMT
ENV MEMCACHED_VERSION=1.6.9
# Fri, 26 Mar 2021 09:38:13 GMT
ENV MEMCACHED_SHA1=42ae062094fdf083cfe7b21ff377c781011c2be1
# Fri, 26 Mar 2021 09:42:08 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Fri, 26 Mar 2021 09:42:09 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 26 Mar 2021 09:42:10 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 26 Mar 2021 09:42:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 09:42:10 GMT
USER memcache
# Fri, 26 Mar 2021 09:42:10 GMT
EXPOSE 11211
# Fri, 26 Mar 2021 09:42:10 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:9aae54b2144e5b2b00c610f8805128f4f86822e1e52d3714c463744a431f0f4a`  
		Last Modified: Thu, 25 Mar 2021 22:20:18 GMT  
		Size: 2.8 MB (2811681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaefa880f46a5755d51d3e45077e1fff44e5aa93933777ec97b9bfb3e1c49715`  
		Last Modified: Fri, 26 Mar 2021 09:42:36 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:436a992a8a9c2b399a06843e7951676cc5efb57378f1a726fca25f55b904237b`  
		Last Modified: Fri, 26 Mar 2021 09:42:36 GMT  
		Size: 155.2 KB (155225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9747edb09d86e22df4e111c143640611fbbdbf5a0f237e80d04be2fb931eb722`  
		Last Modified: Fri, 26 Mar 2021 09:42:36 GMT  
		Size: 867.3 KB (867342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19d066699265da7027a01cffac223114af68d0a3976802f8f32b74cda0fe7186`  
		Last Modified: Fri, 26 Mar 2021 09:42:36 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1b3657184e4138b203aec9c7e53a1084c53ef07e21addc6dd924298728967e1`  
		Last Modified: Fri, 26 Mar 2021 09:42:37 GMT  
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
$ docker pull memcached@sha256:7a16955ceb59429c180ba0e27b2110942bf9f5bc2bfcf776c367fa04e2947d61
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.7 MB (3724062 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:01d2695ea7aff546d998d8385f91a0c93c4e6f1f1bedb46f36e5c1c321d67509`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 25 Mar 2021 22:40:10 GMT
ADD file:8d7431f7e3e42b162a1626e7abf4ef7605146671dccc753d490de6b7fe429261 in / 
# Thu, 25 Mar 2021 22:40:23 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 11:55:58 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Fri, 26 Mar 2021 11:56:05 GMT
RUN apk add --no-cache libsasl
# Fri, 26 Mar 2021 11:56:08 GMT
ENV MEMCACHED_VERSION=1.6.9
# Fri, 26 Mar 2021 11:56:11 GMT
ENV MEMCACHED_SHA1=42ae062094fdf083cfe7b21ff377c781011c2be1
# Fri, 26 Mar 2021 11:59:21 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Fri, 26 Mar 2021 11:59:23 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 26 Mar 2021 11:59:25 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 26 Mar 2021 11:59:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 11:59:26 GMT
USER memcache
# Fri, 26 Mar 2021 11:59:27 GMT
EXPOSE 11211
# Fri, 26 Mar 2021 11:59:28 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:5ceb5101e3b0d54efb5f18318982508a04b181b4d5ae52b096dd35dea3a006cc`  
		Last Modified: Thu, 25 Mar 2021 22:44:41 GMT  
		Size: 2.7 MB (2711898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33c67e7215624376f623cadc677e6e078a62b0994949432d87e37d4bc0bd84d7`  
		Last Modified: Fri, 26 Mar 2021 11:59:55 GMT  
		Size: 1.3 KB (1256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d58f5b5b7d00e1ba2d3fdcc8cafc38b603be1002827ac0df0b581b0bb9387ca`  
		Last Modified: Fri, 26 Mar 2021 11:59:55 GMT  
		Size: 157.4 KB (157363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df4c0873fa7bdc463d82bc203d043bfb4b2959f34c3537de34b5a16b54d2dd83`  
		Last Modified: Fri, 26 Mar 2021 11:59:55 GMT  
		Size: 853.1 KB (853138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57ee3d4d0da34f5745af3bc3f88f5e034f7efe899653af6cb58126725451abab`  
		Last Modified: Fri, 26 Mar 2021 11:59:55 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7211bb020587c3ab33ad007f676f6697975abb98bb048f02c82cccf0ae12276`  
		Last Modified: Fri, 26 Mar 2021 11:59:55 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-alpine` - linux; 386

```console
$ docker pull memcached@sha256:ea129f66d114842cd4596d7655d2f04e9b63861794c06211d74b7b1be7f5cfbb
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3867250 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:530c4a3f88e64027883db802c0367dfbd69ba9fb503285c61c29f383d223f80b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 25 Mar 2021 22:38:25 GMT
ADD file:8953415d4b98f486af17a39ba53b38f7262aa590734c18ff9318927e5a705baf in / 
# Thu, 25 Mar 2021 22:38:26 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 10:46:47 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Fri, 26 Mar 2021 10:46:49 GMT
RUN apk add --no-cache libsasl
# Fri, 26 Mar 2021 10:46:49 GMT
ENV MEMCACHED_VERSION=1.6.9
# Fri, 26 Mar 2021 10:46:49 GMT
ENV MEMCACHED_SHA1=42ae062094fdf083cfe7b21ff377c781011c2be1
# Fri, 26 Mar 2021 10:50:57 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Fri, 26 Mar 2021 10:50:57 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 26 Mar 2021 10:50:58 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 26 Mar 2021 10:50:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 10:50:58 GMT
USER memcache
# Fri, 26 Mar 2021 10:50:59 GMT
EXPOSE 11211
# Fri, 26 Mar 2021 10:50:59 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:1fbd1c9912b638ce64a4740e3af7a3a03452f8705b8103950d677f1d79ae8164`  
		Last Modified: Thu, 25 Mar 2021 22:39:34 GMT  
		Size: 2.8 MB (2818129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:741d80ca4d99ded9e0725802bae206c2f75cf810363ec08ff97ac36608ab2c44`  
		Last Modified: Fri, 26 Mar 2021 10:51:39 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aee79c2789c7c2625b2f4b749e93967edce4a64eb9f0175ee1ce48206184fe07`  
		Last Modified: Fri, 26 Mar 2021 10:51:39 GMT  
		Size: 168.7 KB (168723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b298ea91522ee7dcd7d3716875dc9710f0af384ad866b28ab6a95f9f4aacfc36`  
		Last Modified: Fri, 26 Mar 2021 10:51:40 GMT  
		Size: 878.7 KB (878735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89f365d3ac6496ec95cd6a55b24893347ff9fa2a3fec8f0b6d5ac1757c8c2578`  
		Last Modified: Fri, 26 Mar 2021 10:51:39 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc1ff81bdf527601d8b1a55b9a43faf1c2571d8c8a3a1ad261bfef6ad920de05`  
		Last Modified: Fri, 26 Mar 2021 10:51:39 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-alpine` - linux; ppc64le

```console
$ docker pull memcached@sha256:3565226caf1343498d212e8dddf18067c4b6c0a45255fe1bfce7991414be07ff
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3889240 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd5e38aa6a933e9c61f4f1722dea74085d48c2b5e3be4d794a1ba005b9ee4257`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 25 Mar 2021 22:22:28 GMT
ADD file:f91f8e0aa646cb847f6e210056280f9332382ad2f8d6a8839fd9aa69b81c4a2a in / 
# Thu, 25 Mar 2021 22:22:30 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 07:17:34 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Fri, 26 Mar 2021 07:18:03 GMT
RUN apk add --no-cache libsasl
# Fri, 26 Mar 2021 07:18:10 GMT
ENV MEMCACHED_VERSION=1.6.9
# Fri, 26 Mar 2021 07:18:21 GMT
ENV MEMCACHED_SHA1=42ae062094fdf083cfe7b21ff377c781011c2be1
# Fri, 26 Mar 2021 07:22:17 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Fri, 26 Mar 2021 07:22:36 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 26 Mar 2021 07:23:13 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 26 Mar 2021 07:23:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 07:23:59 GMT
USER memcache
# Fri, 26 Mar 2021 07:24:14 GMT
EXPOSE 11211
# Fri, 26 Mar 2021 07:24:25 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:f3b2866c25f0a9167af050d646a7a740ccc88d46e068c90ff28a5c2ec2ee0030`  
		Last Modified: Thu, 25 Mar 2021 22:24:08 GMT  
		Size: 2.8 MB (2813115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b44508f603fc78a9e285af9f3c471b504f550a5e8a0f40e6a2bf7b715c6f777a`  
		Last Modified: Fri, 26 Mar 2021 07:25:02 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08d912e9739268eaf715a74f79cc127aca3a4a148f08b54920481b42ef98688c`  
		Last Modified: Fri, 26 Mar 2021 07:25:02 GMT  
		Size: 179.4 KB (179407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:759ed9ae532838d207b902a238c9494dd4a31357df138e862c4e3ca33cb8489b`  
		Last Modified: Fri, 26 Mar 2021 07:25:02 GMT  
		Size: 895.0 KB (895049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4fc0cf47cb2958e8c26cf38a6df13121c2b6fc0b65261fd9b72503e5f2b5f44`  
		Last Modified: Fri, 26 Mar 2021 07:25:02 GMT  
		Size: 282.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc6309f228ff45d777bd633ce1142b7bafd7daf6ceb8330f9977261f2b2cade4`  
		Last Modified: Fri, 26 Mar 2021 07:25:02 GMT  
		Size: 120.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-alpine` - linux; s390x

```console
$ docker pull memcached@sha256:d3b1ceba59f4053aa3482a6f89186e6f669a3404bfe219d140f87485d92810eb
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.6 MB (3627991 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb3ae3389c5204551f2fdb3f9ec1049e46002666bf93c3a9c59556db44409a19`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 25 Mar 2021 22:41:34 GMT
ADD file:44e2c7cd992fc98df702bef7022e0f8c4ee86312c311ab5ae185fd5fc878edf9 in / 
# Thu, 25 Mar 2021 22:41:34 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 00:01:52 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Fri, 26 Mar 2021 00:01:53 GMT
RUN apk add --no-cache libsasl
# Fri, 26 Mar 2021 00:01:54 GMT
ENV MEMCACHED_VERSION=1.6.9
# Fri, 26 Mar 2021 00:01:54 GMT
ENV MEMCACHED_SHA1=42ae062094fdf083cfe7b21ff377c781011c2be1
# Fri, 26 Mar 2021 00:05:59 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Fri, 26 Mar 2021 00:05:59 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 26 Mar 2021 00:06:00 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 26 Mar 2021 00:06:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 00:06:01 GMT
USER memcache
# Fri, 26 Mar 2021 00:06:01 GMT
EXPOSE 11211
# Fri, 26 Mar 2021 00:06:01 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:a266c0a9554add02ea09a46b8584cb36b7f606b7b4398b9ad7369f899f8360df`  
		Last Modified: Thu, 25 Mar 2021 22:42:07 GMT  
		Size: 2.6 MB (2602387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba7d3fc0e072913222e5431a4623bafe2581832cfa9017ed6f895763ee9f68ec`  
		Last Modified: Fri, 26 Mar 2021 00:06:23 GMT  
		Size: 1.3 KB (1256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42592fd9e69eae21d62d27596306a0184129ade75259eca72565bd3d8952981a`  
		Last Modified: Fri, 26 Mar 2021 00:06:24 GMT  
		Size: 161.2 KB (161193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1e129edd5e146d9cc6a328abaa83a73b63b501b30a6cb0bdedc4011e0b09b74`  
		Last Modified: Fri, 26 Mar 2021 00:06:23 GMT  
		Size: 862.8 KB (862751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e816e90ee5e4b4a419d2458929ef3017531e034768d7e5e38ba964fca8c57f07`  
		Last Modified: Fri, 26 Mar 2021 00:06:23 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2e7804a791461e688f20e06d5c4370728c765d161605d2f47a705f026fe2395`  
		Last Modified: Fri, 26 Mar 2021 00:06:23 GMT  
		Size: 120.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:1.6`

```console
$ docker pull memcached@sha256:aedbed05133579a286baaffce576b360a3860b5644d7e4bd39e8d0a26b847801
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
$ docker pull memcached@sha256:d8559d4ca748485fe7acf3bda5634902385c393b56991153d3259b1919b667b6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.5 MB (30510071 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c17a0df7f0b4ead3f7992531505b74f08210e464636782ff8d4e9f9c3f9ab634`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 12 Mar 2021 02:20:40 GMT
ADD file:3c32f1cd03198e141dd233a7ffd13444157d4150ad917d548f3ee9bf5953ce22 in / 
# Fri, 12 Mar 2021 02:20:41 GMT
CMD ["bash"]
# Sat, 13 Mar 2021 03:51:06 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Sat, 13 Mar 2021 03:51:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 13 Mar 2021 03:51:12 GMT
ENV MEMCACHED_VERSION=1.6.9
# Sat, 13 Mar 2021 03:51:12 GMT
ENV MEMCACHED_SHA1=42ae062094fdf083cfe7b21ff377c781011c2be1
# Sat, 13 Mar 2021 03:55:02 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Sat, 13 Mar 2021 03:55:03 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Sat, 13 Mar 2021 03:55:04 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Sat, 13 Mar 2021 03:55:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 13 Mar 2021 03:55:04 GMT
USER memcache
# Sat, 13 Mar 2021 03:55:04 GMT
EXPOSE 11211
# Sat, 13 Mar 2021 03:55:05 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:6f28985ad1843afd6fd4fe0b42a30bfab63c27d302362e7341e3316e8ba25ced`  
		Last Modified: Fri, 12 Mar 2021 02:26:11 GMT  
		Size: 27.1 MB (27101001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:007083158c847935c98d2d8c07518c8097b91da3a2fd7e15a6dbbb5f7e3de5e4`  
		Last Modified: Sat, 13 Mar 2021 03:59:56 GMT  
		Size: 5.0 KB (4977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44f9cc8fbeb0c17485aa8956f8ad64a7c24d44af44ea7b4883955f47996b189d`  
		Last Modified: Sat, 13 Mar 2021 03:59:57 GMT  
		Size: 2.2 MB (2197036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:955c0e8ce2a3821077059bb8198bc27098ef46dda29831d180cdc995186b345a`  
		Last Modified: Sat, 13 Mar 2021 03:59:56 GMT  
		Size: 1.2 MB (1206649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d8cc0a86221ff10b28b1a07db34deda0dfbc8f255f8a0911c518d91e2f84eba`  
		Last Modified: Sat, 13 Mar 2021 03:59:56 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7156f15be6833cf1ea0a3172ebe80928e5622768ad50c17b274b6004b6cc080`  
		Last Modified: Sat, 13 Mar 2021 03:59:56 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6` - linux; arm variant v5

```console
$ docker pull memcached@sha256:14a89ab8a75e421a79f0e3e65074b106d8b03e9b45fc0b6ff3ca1f7843e2176a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.9 MB (27928037 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a715778439ac19faacf97a009883e33c115543fe3a0f0deace9db3705ea9a7a2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 26 Mar 2021 07:51:46 GMT
ADD file:3dd25698bf1578e8580b2f437a2199bfc3b1818480b874d73622357e955a091f in / 
# Fri, 26 Mar 2021 07:51:48 GMT
CMD ["bash"]
# Fri, 26 Mar 2021 09:39:21 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Fri, 26 Mar 2021 09:39:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 09:39:34 GMT
ENV MEMCACHED_VERSION=1.6.9
# Fri, 26 Mar 2021 09:39:34 GMT
ENV MEMCACHED_SHA1=42ae062094fdf083cfe7b21ff377c781011c2be1
# Fri, 26 Mar 2021 09:43:40 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Fri, 26 Mar 2021 09:43:41 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 26 Mar 2021 09:43:44 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 26 Mar 2021 09:43:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 09:43:46 GMT
USER memcache
# Fri, 26 Mar 2021 09:43:47 GMT
EXPOSE 11211
# Fri, 26 Mar 2021 09:43:47 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:997e59852ec0e1a23e4a179db14793947d60390c392ce15abc0f811e797c49ca`  
		Last Modified: Fri, 26 Mar 2021 08:00:22 GMT  
		Size: 24.8 MB (24846159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bac4aeb1ec3f8bad5601293e2e6ee4892f2099bcdf754eca5a256713b4f4ac78`  
		Last Modified: Fri, 26 Mar 2021 09:44:00 GMT  
		Size: 4.9 KB (4893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c690f09a614f96a09cf57ab424bb57e240adc3cbfd1cc08482f124a479fad552`  
		Last Modified: Fri, 26 Mar 2021 09:44:02 GMT  
		Size: 1.9 MB (1897339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d144d9a91ac96cb9c068f67fc5649459003e9f9a21867638fb49840ed9e85e0`  
		Last Modified: Fri, 26 Mar 2021 09:44:01 GMT  
		Size: 1.2 MB (1179238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3160a064a6625a7ec9c8959cd13f6e9113a5c2cb59cbe8ea826ce8a210068b7e`  
		Last Modified: Fri, 26 Mar 2021 09:44:00 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e4455ba84cf78688e072088f68b9c85bc29af1a497039b5241c6291b5de1843`  
		Last Modified: Fri, 26 Mar 2021 09:44:00 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6` - linux; arm variant v7

```console
$ docker pull memcached@sha256:ca79781006a7d45818e0e9b0d51c954c9c9c4bde8336060bf04fc99cbd7809e3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.7 MB (25676128 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b26ff179f940a940395fc620c44eff4702a61bc989da3d71d318bc699dd4ed08`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 12 Mar 2021 02:00:12 GMT
ADD file:123da9848f87c8ed4c5122a104b8650564c09767725916f822def7b645a019f1 in / 
# Fri, 12 Mar 2021 02:00:14 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 03:08:21 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Fri, 12 Mar 2021 03:08:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 03:08:32 GMT
ENV MEMCACHED_VERSION=1.6.9
# Fri, 12 Mar 2021 03:08:33 GMT
ENV MEMCACHED_SHA1=42ae062094fdf083cfe7b21ff377c781011c2be1
# Fri, 12 Mar 2021 03:11:57 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Fri, 12 Mar 2021 03:11:58 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 12 Mar 2021 03:12:01 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 12 Mar 2021 03:12:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 12 Mar 2021 03:12:03 GMT
USER memcache
# Fri, 12 Mar 2021 03:12:04 GMT
EXPOSE 11211
# Fri, 12 Mar 2021 03:12:05 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:e12d26f75fe8b7fd14712965ff5178762227d07d2151bb35fa21105ddfc4a14a`  
		Last Modified: Fri, 12 Mar 2021 02:10:28 GMT  
		Size: 22.7 MB (22709467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe1e03071b3302ec91defd6b8b861a3be2a50d7165f73c154eea0ddd8339641a`  
		Last Modified: Fri, 12 Mar 2021 03:22:32 GMT  
		Size: 4.9 KB (4899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b11c24c5a0d1d4fa06df54624b6dc7a5d1586210047c31e44511fa513081a49e`  
		Last Modified: Fri, 12 Mar 2021 03:22:33 GMT  
		Size: 1.8 MB (1811657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57458ecd2770995b21c7c8d20108d84bc9b4879cd759054d4f8e122bb54a7451`  
		Last Modified: Fri, 12 Mar 2021 03:22:32 GMT  
		Size: 1.1 MB (1149703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6070aa36c0112c5a66ad85b5eaa4e4c954a217f484a915ff259fd30c5de332e6`  
		Last Modified: Fri, 12 Mar 2021 03:22:32 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1d498de6ccd0c3ffc78632677c24cad8f6acc9add31d9ef7fd69d57144fb0f4`  
		Last Modified: Fri, 12 Mar 2021 03:22:32 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:fe157d34ccde3aa160d90472f6964aaca3c6b0554f2fa4317d8afceeff3c45cc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.1 MB (29116090 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d61a16162561c8b05c0af58a2555c292980d12cc41872efa2096ed9109377dee`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 12 Mar 2021 01:53:53 GMT
ADD file:6130ddc0a939dd72c0614de4aa77de47aa16fe211274bacb31995aa1a0526164 in / 
# Fri, 12 Mar 2021 01:53:56 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 05:45:15 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Fri, 12 Mar 2021 05:45:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 05:45:27 GMT
ENV MEMCACHED_VERSION=1.6.9
# Fri, 12 Mar 2021 05:45:28 GMT
ENV MEMCACHED_SHA1=42ae062094fdf083cfe7b21ff377c781011c2be1
# Fri, 12 Mar 2021 05:48:54 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Fri, 12 Mar 2021 05:48:55 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 12 Mar 2021 05:48:57 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 12 Mar 2021 05:48:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 12 Mar 2021 05:48:59 GMT
USER memcache
# Fri, 12 Mar 2021 05:49:00 GMT
EXPOSE 11211
# Fri, 12 Mar 2021 05:49:00 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:706ee5d0a6b53d9257cbea22d8409fb22c867ab3a001c65f6b8bfd37dace0e58`  
		Last Modified: Fri, 12 Mar 2021 02:01:39 GMT  
		Size: 25.9 MB (25856512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0d9e24f3287f849ddf4e4afe2c8fca91a1031b67a267cd2c779ac2592d59bdf`  
		Last Modified: Fri, 12 Mar 2021 05:49:32 GMT  
		Size: 5.0 KB (5022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c00635c3d3412e964343152daaa8d6a574cff4476029d2dde8fbef8669643dd`  
		Last Modified: Fri, 12 Mar 2021 05:49:33 GMT  
		Size: 2.1 MB (2075174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42b36f1c725910664c120ab3e1137c10c516bc764114217862137f86de0b0a96`  
		Last Modified: Fri, 12 Mar 2021 05:49:32 GMT  
		Size: 1.2 MB (1178974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec7c9cae013d3da2b75c61f808eb35db46f6ea8b4aec6a394c20f9b42341f46c`  
		Last Modified: Fri, 12 Mar 2021 05:49:32 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccaed15ca3b93815844f5b39c66fe6edae8ec39ae3a186a3470e9c8f53909018`  
		Last Modified: Fri, 12 Mar 2021 05:49:32 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6` - linux; 386

```console
$ docker pull memcached@sha256:ef0460019399121409cd24063e18f58e7f89f6c6dd0c9e6405441876555dfc21
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.2 MB (31178982 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91f0b8c30945bbb159fc82df44b331add3a586ea0e9d264dd6e26e9733278cb4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 12 Mar 2021 01:44:27 GMT
ADD file:90c103e04bd6fe0f39733cbf8eb2d8845aed3e4fc3fd1e5c3354df69e40aa615 in / 
# Fri, 12 Mar 2021 01:44:28 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 13:31:23 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Fri, 12 Mar 2021 13:31:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 13:31:28 GMT
ENV MEMCACHED_VERSION=1.6.9
# Fri, 12 Mar 2021 13:31:28 GMT
ENV MEMCACHED_SHA1=42ae062094fdf083cfe7b21ff377c781011c2be1
# Fri, 12 Mar 2021 13:35:32 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Fri, 12 Mar 2021 13:35:32 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 12 Mar 2021 13:35:33 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 12 Mar 2021 13:35:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 12 Mar 2021 13:35:33 GMT
USER memcache
# Fri, 12 Mar 2021 13:35:33 GMT
EXPOSE 11211
# Fri, 12 Mar 2021 13:35:34 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:0898aa7472f57f223652846337cf862f142e109d0c039b41886e7f20c345f85e`  
		Last Modified: Fri, 12 Mar 2021 01:52:08 GMT  
		Size: 27.8 MB (27760948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f32ccac2f28603415b89f000eac53a764ccb5e4a5c7bb96f531886d346046066`  
		Last Modified: Fri, 12 Mar 2021 13:40:40 GMT  
		Size: 4.9 KB (4895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ca797dc44ad9702a16634c4e34b2809570c531a00ea77bc688afbc168ef7ee4`  
		Last Modified: Fri, 12 Mar 2021 13:40:41 GMT  
		Size: 2.2 MB (2208684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e11aea04bae299d4a9ad55384df0c485fc53e5a9ca08c49f9905056753b6d4e6`  
		Last Modified: Fri, 12 Mar 2021 13:40:41 GMT  
		Size: 1.2 MB (1204047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1793a72e67f7bf9006a9aa26f1c569f4f92bc9ac6d93ea73f96d8a05bfd5e0a6`  
		Last Modified: Fri, 12 Mar 2021 13:40:40 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:999651c299c9f7bd71c0b15ecb302b22f3f03f36924d3144b76eb81e619d0184`  
		Last Modified: Fri, 12 Mar 2021 13:40:40 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6` - linux; mips64le

```console
$ docker pull memcached@sha256:8ea232e21a6f020459a12dd1d7aedc8474594927363ba4aec07ce413deb9bed5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.8 MB (28752902 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:068f62f8ad395edfb2fda7af67488827096540267d3151dc47631195b1fc9543`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 12 Mar 2021 02:10:02 GMT
ADD file:491c5ca15fe098b83de42861289c216c693d788a1f9e739a78acefb0cad453c8 in / 
# Fri, 12 Mar 2021 02:10:03 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 08:46:26 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Fri, 12 Mar 2021 08:46:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 08:46:39 GMT
ENV MEMCACHED_VERSION=1.6.9
# Fri, 12 Mar 2021 08:46:39 GMT
ENV MEMCACHED_SHA1=42ae062094fdf083cfe7b21ff377c781011c2be1
# Fri, 12 Mar 2021 08:52:26 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Fri, 12 Mar 2021 08:52:27 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 12 Mar 2021 08:52:28 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 12 Mar 2021 08:52:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 12 Mar 2021 08:52:29 GMT
USER memcache
# Fri, 12 Mar 2021 08:52:29 GMT
EXPOSE 11211
# Fri, 12 Mar 2021 08:52:30 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:d0b6b2cc51bdde474395b8c32ff8012e471727bba69f221cfb79b46e8283f047`  
		Last Modified: Fri, 12 Mar 2021 02:17:07 GMT  
		Size: 25.8 MB (25772338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22086edc87e18d40945456938ba809ad0b1153dcf874df2911314f3fa0d76667`  
		Last Modified: Fri, 12 Mar 2021 08:52:45 GMT  
		Size: 5.0 KB (4978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b808a76ea31d9ba92e88100192f485f4efc2f9c15b24c41990aa202a0ed1a508`  
		Last Modified: Fri, 12 Mar 2021 08:52:46 GMT  
		Size: 1.8 MB (1776385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afada1a8592c3da748b0b5ac6d6a4db3f02704fb3785a7e1cc13a6b4fd5b1010`  
		Last Modified: Fri, 12 Mar 2021 08:52:46 GMT  
		Size: 1.2 MB (1198794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:276d546ec9c236bf7813ab6f11ccc55c6e127f0ea72ccbb36c035dbe52d675f6`  
		Last Modified: Fri, 12 Mar 2021 08:52:45 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a11a440437df39f7b30113415724385ba8643faf61547a4148083c19dd934eaa`  
		Last Modified: Fri, 12 Mar 2021 08:52:45 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6` - linux; ppc64le

```console
$ docker pull memcached@sha256:efd3d67a1afd293b38dc0ebf78641266104fa8f44735e0b6210117d914f67250
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.1 MB (34087167 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:95699b572190f07b90f87f36f5f2e01c0073b7ac7241544c9c5d156985b817b4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 12 Mar 2021 02:32:43 GMT
ADD file:6a0c0cfa71979cf6fdd859dce1e32582f0e55ed382b9e17b77a2001defc2c9db in / 
# Fri, 12 Mar 2021 02:32:50 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 05:42:18 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Fri, 12 Mar 2021 05:42:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 05:42:50 GMT
ENV MEMCACHED_VERSION=1.6.9
# Fri, 12 Mar 2021 05:42:55 GMT
ENV MEMCACHED_SHA1=42ae062094fdf083cfe7b21ff377c781011c2be1
# Fri, 12 Mar 2021 05:51:27 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Fri, 12 Mar 2021 05:51:31 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 12 Mar 2021 05:51:53 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 12 Mar 2021 05:51:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 12 Mar 2021 05:52:07 GMT
USER memcache
# Fri, 12 Mar 2021 05:52:14 GMT
EXPOSE 11211
# Fri, 12 Mar 2021 05:52:21 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:1d686056fdac1848f4fd78ba2b335502055ffe98c79619e21d0c2fb7db95257e`  
		Last Modified: Fri, 12 Mar 2021 02:45:35 GMT  
		Size: 30.5 MB (30525728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73b1efcdfc9b290f77d5235f4f3bec7b09d62026296bb6dfccbdba7354df9caa`  
		Last Modified: Fri, 12 Mar 2021 05:52:55 GMT  
		Size: 5.0 KB (4994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0ae8f3e8315ccb25bd80ff467115a6f3479c6b5acf818ad7e3fcf4af0b2ebe1`  
		Last Modified: Fri, 12 Mar 2021 05:52:56 GMT  
		Size: 2.3 MB (2323017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0f34bd86e0ac5d50a3f227ab5cc3190a8a0973ea12c7e827d9267cad4dad482`  
		Last Modified: Fri, 12 Mar 2021 05:52:55 GMT  
		Size: 1.2 MB (1233020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a188c62ab305cd93f469a414ef7da5b0f1c3e66817ea0439a7530e194f90d05f`  
		Last Modified: Fri, 12 Mar 2021 05:52:55 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b5898f549c8d0705d12413acbc320c216d8a65dd1c312d1da6e8fe53df526e6`  
		Last Modified: Fri, 12 Mar 2021 05:52:55 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6` - linux; s390x

```console
$ docker pull memcached@sha256:5e844fb7cd8aa06589f899a421921d452ade52de1e969ae763d60fecece294e9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.8 MB (28806644 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e79898684368a64d853c29bb82cfb9688df1e0230116c145e7f137796fb3eb4f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 12 Mar 2021 01:46:04 GMT
ADD file:afec039adf230a9186a38b57eed85262696f8d178ac649a445657066f16fe806 in / 
# Fri, 12 Mar 2021 01:46:07 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 02:55:40 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Fri, 12 Mar 2021 02:55:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 02:55:46 GMT
ENV MEMCACHED_VERSION=1.6.9
# Fri, 12 Mar 2021 02:55:46 GMT
ENV MEMCACHED_SHA1=42ae062094fdf083cfe7b21ff377c781011c2be1
# Fri, 12 Mar 2021 02:59:29 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Fri, 12 Mar 2021 02:59:29 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 12 Mar 2021 02:59:30 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 12 Mar 2021 02:59:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 12 Mar 2021 02:59:31 GMT
USER memcache
# Fri, 12 Mar 2021 02:59:31 GMT
EXPOSE 11211
# Fri, 12 Mar 2021 02:59:31 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:d41215965c091534e809ab2e8f4a2c1cebee3de536c2c74a7bc8302bbc8af7e1`  
		Last Modified: Fri, 12 Mar 2021 01:50:30 GMT  
		Size: 25.7 MB (25716294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c86c43c934421c76725f64bbc35ebb36c5f5c8dd181f6f701101068a31671d10`  
		Last Modified: Fri, 12 Mar 2021 02:59:59 GMT  
		Size: 5.0 KB (5025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97631e025d45847d90b38975ee3e031618e6eeedc1077b6ab77612d1edcda2e5`  
		Last Modified: Fri, 12 Mar 2021 02:59:59 GMT  
		Size: 1.9 MB (1886402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e98fc6e9a78adb22f7fb53ccc28169914f61a8f89c7c414f8d7b7eb22460b5f2`  
		Last Modified: Fri, 12 Mar 2021 02:59:59 GMT  
		Size: 1.2 MB (1198516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f9b27ffa18edb87e225a25d6bba459f4ae8a473944cebb847fe0e13a78e84fa`  
		Last Modified: Fri, 12 Mar 2021 02:59:59 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82ff067463b04909884ea6e0adda53fb48c398ee27e4ea1ae7de1dc5d5107151`  
		Last Modified: Fri, 12 Mar 2021 02:59:59 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:1.6-alpine`

```console
$ docker pull memcached@sha256:a1a84ac6bba5b100e79cff5819072ea05815a3597af2611713313ff77df7b799
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
$ docker pull memcached@sha256:e799e863cd8dd7c6143457541d4e881f29d2a8cc7cf36a9e73afc075b88eaf66
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3835911 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:336eae34e88e7f26ba0efae7e37fae40bf1ec0752a3dd074d2bce3a5be74de7b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 25 Mar 2021 22:19:32 GMT
ADD file:6b081cabb4b256ee07587d249c4989b5b679375529542b81550a65b6f19f274e in / 
# Thu, 25 Mar 2021 22:19:32 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 09:38:12 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Fri, 26 Mar 2021 09:38:13 GMT
RUN apk add --no-cache libsasl
# Fri, 26 Mar 2021 09:38:13 GMT
ENV MEMCACHED_VERSION=1.6.9
# Fri, 26 Mar 2021 09:38:13 GMT
ENV MEMCACHED_SHA1=42ae062094fdf083cfe7b21ff377c781011c2be1
# Fri, 26 Mar 2021 09:42:08 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Fri, 26 Mar 2021 09:42:09 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 26 Mar 2021 09:42:10 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 26 Mar 2021 09:42:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 09:42:10 GMT
USER memcache
# Fri, 26 Mar 2021 09:42:10 GMT
EXPOSE 11211
# Fri, 26 Mar 2021 09:42:10 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:9aae54b2144e5b2b00c610f8805128f4f86822e1e52d3714c463744a431f0f4a`  
		Last Modified: Thu, 25 Mar 2021 22:20:18 GMT  
		Size: 2.8 MB (2811681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaefa880f46a5755d51d3e45077e1fff44e5aa93933777ec97b9bfb3e1c49715`  
		Last Modified: Fri, 26 Mar 2021 09:42:36 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:436a992a8a9c2b399a06843e7951676cc5efb57378f1a726fca25f55b904237b`  
		Last Modified: Fri, 26 Mar 2021 09:42:36 GMT  
		Size: 155.2 KB (155225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9747edb09d86e22df4e111c143640611fbbdbf5a0f237e80d04be2fb931eb722`  
		Last Modified: Fri, 26 Mar 2021 09:42:36 GMT  
		Size: 867.3 KB (867342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19d066699265da7027a01cffac223114af68d0a3976802f8f32b74cda0fe7186`  
		Last Modified: Fri, 26 Mar 2021 09:42:36 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1b3657184e4138b203aec9c7e53a1084c53ef07e21addc6dd924298728967e1`  
		Last Modified: Fri, 26 Mar 2021 09:42:37 GMT  
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
$ docker pull memcached@sha256:7a16955ceb59429c180ba0e27b2110942bf9f5bc2bfcf776c367fa04e2947d61
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.7 MB (3724062 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:01d2695ea7aff546d998d8385f91a0c93c4e6f1f1bedb46f36e5c1c321d67509`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 25 Mar 2021 22:40:10 GMT
ADD file:8d7431f7e3e42b162a1626e7abf4ef7605146671dccc753d490de6b7fe429261 in / 
# Thu, 25 Mar 2021 22:40:23 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 11:55:58 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Fri, 26 Mar 2021 11:56:05 GMT
RUN apk add --no-cache libsasl
# Fri, 26 Mar 2021 11:56:08 GMT
ENV MEMCACHED_VERSION=1.6.9
# Fri, 26 Mar 2021 11:56:11 GMT
ENV MEMCACHED_SHA1=42ae062094fdf083cfe7b21ff377c781011c2be1
# Fri, 26 Mar 2021 11:59:21 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Fri, 26 Mar 2021 11:59:23 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 26 Mar 2021 11:59:25 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 26 Mar 2021 11:59:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 11:59:26 GMT
USER memcache
# Fri, 26 Mar 2021 11:59:27 GMT
EXPOSE 11211
# Fri, 26 Mar 2021 11:59:28 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:5ceb5101e3b0d54efb5f18318982508a04b181b4d5ae52b096dd35dea3a006cc`  
		Last Modified: Thu, 25 Mar 2021 22:44:41 GMT  
		Size: 2.7 MB (2711898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33c67e7215624376f623cadc677e6e078a62b0994949432d87e37d4bc0bd84d7`  
		Last Modified: Fri, 26 Mar 2021 11:59:55 GMT  
		Size: 1.3 KB (1256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d58f5b5b7d00e1ba2d3fdcc8cafc38b603be1002827ac0df0b581b0bb9387ca`  
		Last Modified: Fri, 26 Mar 2021 11:59:55 GMT  
		Size: 157.4 KB (157363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df4c0873fa7bdc463d82bc203d043bfb4b2959f34c3537de34b5a16b54d2dd83`  
		Last Modified: Fri, 26 Mar 2021 11:59:55 GMT  
		Size: 853.1 KB (853138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57ee3d4d0da34f5745af3bc3f88f5e034f7efe899653af6cb58126725451abab`  
		Last Modified: Fri, 26 Mar 2021 11:59:55 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7211bb020587c3ab33ad007f676f6697975abb98bb048f02c82cccf0ae12276`  
		Last Modified: Fri, 26 Mar 2021 11:59:55 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-alpine` - linux; 386

```console
$ docker pull memcached@sha256:ea129f66d114842cd4596d7655d2f04e9b63861794c06211d74b7b1be7f5cfbb
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3867250 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:530c4a3f88e64027883db802c0367dfbd69ba9fb503285c61c29f383d223f80b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 25 Mar 2021 22:38:25 GMT
ADD file:8953415d4b98f486af17a39ba53b38f7262aa590734c18ff9318927e5a705baf in / 
# Thu, 25 Mar 2021 22:38:26 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 10:46:47 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Fri, 26 Mar 2021 10:46:49 GMT
RUN apk add --no-cache libsasl
# Fri, 26 Mar 2021 10:46:49 GMT
ENV MEMCACHED_VERSION=1.6.9
# Fri, 26 Mar 2021 10:46:49 GMT
ENV MEMCACHED_SHA1=42ae062094fdf083cfe7b21ff377c781011c2be1
# Fri, 26 Mar 2021 10:50:57 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Fri, 26 Mar 2021 10:50:57 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 26 Mar 2021 10:50:58 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 26 Mar 2021 10:50:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 10:50:58 GMT
USER memcache
# Fri, 26 Mar 2021 10:50:59 GMT
EXPOSE 11211
# Fri, 26 Mar 2021 10:50:59 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:1fbd1c9912b638ce64a4740e3af7a3a03452f8705b8103950d677f1d79ae8164`  
		Last Modified: Thu, 25 Mar 2021 22:39:34 GMT  
		Size: 2.8 MB (2818129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:741d80ca4d99ded9e0725802bae206c2f75cf810363ec08ff97ac36608ab2c44`  
		Last Modified: Fri, 26 Mar 2021 10:51:39 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aee79c2789c7c2625b2f4b749e93967edce4a64eb9f0175ee1ce48206184fe07`  
		Last Modified: Fri, 26 Mar 2021 10:51:39 GMT  
		Size: 168.7 KB (168723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b298ea91522ee7dcd7d3716875dc9710f0af384ad866b28ab6a95f9f4aacfc36`  
		Last Modified: Fri, 26 Mar 2021 10:51:40 GMT  
		Size: 878.7 KB (878735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89f365d3ac6496ec95cd6a55b24893347ff9fa2a3fec8f0b6d5ac1757c8c2578`  
		Last Modified: Fri, 26 Mar 2021 10:51:39 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc1ff81bdf527601d8b1a55b9a43faf1c2571d8c8a3a1ad261bfef6ad920de05`  
		Last Modified: Fri, 26 Mar 2021 10:51:39 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-alpine` - linux; ppc64le

```console
$ docker pull memcached@sha256:3565226caf1343498d212e8dddf18067c4b6c0a45255fe1bfce7991414be07ff
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3889240 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd5e38aa6a933e9c61f4f1722dea74085d48c2b5e3be4d794a1ba005b9ee4257`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 25 Mar 2021 22:22:28 GMT
ADD file:f91f8e0aa646cb847f6e210056280f9332382ad2f8d6a8839fd9aa69b81c4a2a in / 
# Thu, 25 Mar 2021 22:22:30 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 07:17:34 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Fri, 26 Mar 2021 07:18:03 GMT
RUN apk add --no-cache libsasl
# Fri, 26 Mar 2021 07:18:10 GMT
ENV MEMCACHED_VERSION=1.6.9
# Fri, 26 Mar 2021 07:18:21 GMT
ENV MEMCACHED_SHA1=42ae062094fdf083cfe7b21ff377c781011c2be1
# Fri, 26 Mar 2021 07:22:17 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Fri, 26 Mar 2021 07:22:36 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 26 Mar 2021 07:23:13 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 26 Mar 2021 07:23:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 07:23:59 GMT
USER memcache
# Fri, 26 Mar 2021 07:24:14 GMT
EXPOSE 11211
# Fri, 26 Mar 2021 07:24:25 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:f3b2866c25f0a9167af050d646a7a740ccc88d46e068c90ff28a5c2ec2ee0030`  
		Last Modified: Thu, 25 Mar 2021 22:24:08 GMT  
		Size: 2.8 MB (2813115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b44508f603fc78a9e285af9f3c471b504f550a5e8a0f40e6a2bf7b715c6f777a`  
		Last Modified: Fri, 26 Mar 2021 07:25:02 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08d912e9739268eaf715a74f79cc127aca3a4a148f08b54920481b42ef98688c`  
		Last Modified: Fri, 26 Mar 2021 07:25:02 GMT  
		Size: 179.4 KB (179407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:759ed9ae532838d207b902a238c9494dd4a31357df138e862c4e3ca33cb8489b`  
		Last Modified: Fri, 26 Mar 2021 07:25:02 GMT  
		Size: 895.0 KB (895049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4fc0cf47cb2958e8c26cf38a6df13121c2b6fc0b65261fd9b72503e5f2b5f44`  
		Last Modified: Fri, 26 Mar 2021 07:25:02 GMT  
		Size: 282.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc6309f228ff45d777bd633ce1142b7bafd7daf6ceb8330f9977261f2b2cade4`  
		Last Modified: Fri, 26 Mar 2021 07:25:02 GMT  
		Size: 120.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-alpine` - linux; s390x

```console
$ docker pull memcached@sha256:d3b1ceba59f4053aa3482a6f89186e6f669a3404bfe219d140f87485d92810eb
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.6 MB (3627991 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb3ae3389c5204551f2fdb3f9ec1049e46002666bf93c3a9c59556db44409a19`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 25 Mar 2021 22:41:34 GMT
ADD file:44e2c7cd992fc98df702bef7022e0f8c4ee86312c311ab5ae185fd5fc878edf9 in / 
# Thu, 25 Mar 2021 22:41:34 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 00:01:52 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Fri, 26 Mar 2021 00:01:53 GMT
RUN apk add --no-cache libsasl
# Fri, 26 Mar 2021 00:01:54 GMT
ENV MEMCACHED_VERSION=1.6.9
# Fri, 26 Mar 2021 00:01:54 GMT
ENV MEMCACHED_SHA1=42ae062094fdf083cfe7b21ff377c781011c2be1
# Fri, 26 Mar 2021 00:05:59 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Fri, 26 Mar 2021 00:05:59 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 26 Mar 2021 00:06:00 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 26 Mar 2021 00:06:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 00:06:01 GMT
USER memcache
# Fri, 26 Mar 2021 00:06:01 GMT
EXPOSE 11211
# Fri, 26 Mar 2021 00:06:01 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:a266c0a9554add02ea09a46b8584cb36b7f606b7b4398b9ad7369f899f8360df`  
		Last Modified: Thu, 25 Mar 2021 22:42:07 GMT  
		Size: 2.6 MB (2602387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba7d3fc0e072913222e5431a4623bafe2581832cfa9017ed6f895763ee9f68ec`  
		Last Modified: Fri, 26 Mar 2021 00:06:23 GMT  
		Size: 1.3 KB (1256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42592fd9e69eae21d62d27596306a0184129ade75259eca72565bd3d8952981a`  
		Last Modified: Fri, 26 Mar 2021 00:06:24 GMT  
		Size: 161.2 KB (161193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1e129edd5e146d9cc6a328abaa83a73b63b501b30a6cb0bdedc4011e0b09b74`  
		Last Modified: Fri, 26 Mar 2021 00:06:23 GMT  
		Size: 862.8 KB (862751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e816e90ee5e4b4a419d2458929ef3017531e034768d7e5e38ba964fca8c57f07`  
		Last Modified: Fri, 26 Mar 2021 00:06:23 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2e7804a791461e688f20e06d5c4370728c765d161605d2f47a705f026fe2395`  
		Last Modified: Fri, 26 Mar 2021 00:06:23 GMT  
		Size: 120.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:1.6.9`

```console
$ docker pull memcached@sha256:aedbed05133579a286baaffce576b360a3860b5644d7e4bd39e8d0a26b847801
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

### `memcached:1.6.9` - linux; amd64

```console
$ docker pull memcached@sha256:d8559d4ca748485fe7acf3bda5634902385c393b56991153d3259b1919b667b6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.5 MB (30510071 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c17a0df7f0b4ead3f7992531505b74f08210e464636782ff8d4e9f9c3f9ab634`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 12 Mar 2021 02:20:40 GMT
ADD file:3c32f1cd03198e141dd233a7ffd13444157d4150ad917d548f3ee9bf5953ce22 in / 
# Fri, 12 Mar 2021 02:20:41 GMT
CMD ["bash"]
# Sat, 13 Mar 2021 03:51:06 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Sat, 13 Mar 2021 03:51:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 13 Mar 2021 03:51:12 GMT
ENV MEMCACHED_VERSION=1.6.9
# Sat, 13 Mar 2021 03:51:12 GMT
ENV MEMCACHED_SHA1=42ae062094fdf083cfe7b21ff377c781011c2be1
# Sat, 13 Mar 2021 03:55:02 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Sat, 13 Mar 2021 03:55:03 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Sat, 13 Mar 2021 03:55:04 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Sat, 13 Mar 2021 03:55:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 13 Mar 2021 03:55:04 GMT
USER memcache
# Sat, 13 Mar 2021 03:55:04 GMT
EXPOSE 11211
# Sat, 13 Mar 2021 03:55:05 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:6f28985ad1843afd6fd4fe0b42a30bfab63c27d302362e7341e3316e8ba25ced`  
		Last Modified: Fri, 12 Mar 2021 02:26:11 GMT  
		Size: 27.1 MB (27101001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:007083158c847935c98d2d8c07518c8097b91da3a2fd7e15a6dbbb5f7e3de5e4`  
		Last Modified: Sat, 13 Mar 2021 03:59:56 GMT  
		Size: 5.0 KB (4977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44f9cc8fbeb0c17485aa8956f8ad64a7c24d44af44ea7b4883955f47996b189d`  
		Last Modified: Sat, 13 Mar 2021 03:59:57 GMT  
		Size: 2.2 MB (2197036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:955c0e8ce2a3821077059bb8198bc27098ef46dda29831d180cdc995186b345a`  
		Last Modified: Sat, 13 Mar 2021 03:59:56 GMT  
		Size: 1.2 MB (1206649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d8cc0a86221ff10b28b1a07db34deda0dfbc8f255f8a0911c518d91e2f84eba`  
		Last Modified: Sat, 13 Mar 2021 03:59:56 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7156f15be6833cf1ea0a3172ebe80928e5622768ad50c17b274b6004b6cc080`  
		Last Modified: Sat, 13 Mar 2021 03:59:56 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.9` - linux; arm variant v5

```console
$ docker pull memcached@sha256:14a89ab8a75e421a79f0e3e65074b106d8b03e9b45fc0b6ff3ca1f7843e2176a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.9 MB (27928037 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a715778439ac19faacf97a009883e33c115543fe3a0f0deace9db3705ea9a7a2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 26 Mar 2021 07:51:46 GMT
ADD file:3dd25698bf1578e8580b2f437a2199bfc3b1818480b874d73622357e955a091f in / 
# Fri, 26 Mar 2021 07:51:48 GMT
CMD ["bash"]
# Fri, 26 Mar 2021 09:39:21 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Fri, 26 Mar 2021 09:39:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 09:39:34 GMT
ENV MEMCACHED_VERSION=1.6.9
# Fri, 26 Mar 2021 09:39:34 GMT
ENV MEMCACHED_SHA1=42ae062094fdf083cfe7b21ff377c781011c2be1
# Fri, 26 Mar 2021 09:43:40 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Fri, 26 Mar 2021 09:43:41 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 26 Mar 2021 09:43:44 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 26 Mar 2021 09:43:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 09:43:46 GMT
USER memcache
# Fri, 26 Mar 2021 09:43:47 GMT
EXPOSE 11211
# Fri, 26 Mar 2021 09:43:47 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:997e59852ec0e1a23e4a179db14793947d60390c392ce15abc0f811e797c49ca`  
		Last Modified: Fri, 26 Mar 2021 08:00:22 GMT  
		Size: 24.8 MB (24846159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bac4aeb1ec3f8bad5601293e2e6ee4892f2099bcdf754eca5a256713b4f4ac78`  
		Last Modified: Fri, 26 Mar 2021 09:44:00 GMT  
		Size: 4.9 KB (4893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c690f09a614f96a09cf57ab424bb57e240adc3cbfd1cc08482f124a479fad552`  
		Last Modified: Fri, 26 Mar 2021 09:44:02 GMT  
		Size: 1.9 MB (1897339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d144d9a91ac96cb9c068f67fc5649459003e9f9a21867638fb49840ed9e85e0`  
		Last Modified: Fri, 26 Mar 2021 09:44:01 GMT  
		Size: 1.2 MB (1179238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3160a064a6625a7ec9c8959cd13f6e9113a5c2cb59cbe8ea826ce8a210068b7e`  
		Last Modified: Fri, 26 Mar 2021 09:44:00 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e4455ba84cf78688e072088f68b9c85bc29af1a497039b5241c6291b5de1843`  
		Last Modified: Fri, 26 Mar 2021 09:44:00 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.9` - linux; arm variant v7

```console
$ docker pull memcached@sha256:ca79781006a7d45818e0e9b0d51c954c9c9c4bde8336060bf04fc99cbd7809e3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.7 MB (25676128 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b26ff179f940a940395fc620c44eff4702a61bc989da3d71d318bc699dd4ed08`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 12 Mar 2021 02:00:12 GMT
ADD file:123da9848f87c8ed4c5122a104b8650564c09767725916f822def7b645a019f1 in / 
# Fri, 12 Mar 2021 02:00:14 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 03:08:21 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Fri, 12 Mar 2021 03:08:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 03:08:32 GMT
ENV MEMCACHED_VERSION=1.6.9
# Fri, 12 Mar 2021 03:08:33 GMT
ENV MEMCACHED_SHA1=42ae062094fdf083cfe7b21ff377c781011c2be1
# Fri, 12 Mar 2021 03:11:57 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Fri, 12 Mar 2021 03:11:58 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 12 Mar 2021 03:12:01 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 12 Mar 2021 03:12:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 12 Mar 2021 03:12:03 GMT
USER memcache
# Fri, 12 Mar 2021 03:12:04 GMT
EXPOSE 11211
# Fri, 12 Mar 2021 03:12:05 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:e12d26f75fe8b7fd14712965ff5178762227d07d2151bb35fa21105ddfc4a14a`  
		Last Modified: Fri, 12 Mar 2021 02:10:28 GMT  
		Size: 22.7 MB (22709467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe1e03071b3302ec91defd6b8b861a3be2a50d7165f73c154eea0ddd8339641a`  
		Last Modified: Fri, 12 Mar 2021 03:22:32 GMT  
		Size: 4.9 KB (4899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b11c24c5a0d1d4fa06df54624b6dc7a5d1586210047c31e44511fa513081a49e`  
		Last Modified: Fri, 12 Mar 2021 03:22:33 GMT  
		Size: 1.8 MB (1811657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57458ecd2770995b21c7c8d20108d84bc9b4879cd759054d4f8e122bb54a7451`  
		Last Modified: Fri, 12 Mar 2021 03:22:32 GMT  
		Size: 1.1 MB (1149703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6070aa36c0112c5a66ad85b5eaa4e4c954a217f484a915ff259fd30c5de332e6`  
		Last Modified: Fri, 12 Mar 2021 03:22:32 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1d498de6ccd0c3ffc78632677c24cad8f6acc9add31d9ef7fd69d57144fb0f4`  
		Last Modified: Fri, 12 Mar 2021 03:22:32 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.9` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:fe157d34ccde3aa160d90472f6964aaca3c6b0554f2fa4317d8afceeff3c45cc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.1 MB (29116090 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d61a16162561c8b05c0af58a2555c292980d12cc41872efa2096ed9109377dee`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 12 Mar 2021 01:53:53 GMT
ADD file:6130ddc0a939dd72c0614de4aa77de47aa16fe211274bacb31995aa1a0526164 in / 
# Fri, 12 Mar 2021 01:53:56 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 05:45:15 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Fri, 12 Mar 2021 05:45:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 05:45:27 GMT
ENV MEMCACHED_VERSION=1.6.9
# Fri, 12 Mar 2021 05:45:28 GMT
ENV MEMCACHED_SHA1=42ae062094fdf083cfe7b21ff377c781011c2be1
# Fri, 12 Mar 2021 05:48:54 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Fri, 12 Mar 2021 05:48:55 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 12 Mar 2021 05:48:57 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 12 Mar 2021 05:48:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 12 Mar 2021 05:48:59 GMT
USER memcache
# Fri, 12 Mar 2021 05:49:00 GMT
EXPOSE 11211
# Fri, 12 Mar 2021 05:49:00 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:706ee5d0a6b53d9257cbea22d8409fb22c867ab3a001c65f6b8bfd37dace0e58`  
		Last Modified: Fri, 12 Mar 2021 02:01:39 GMT  
		Size: 25.9 MB (25856512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0d9e24f3287f849ddf4e4afe2c8fca91a1031b67a267cd2c779ac2592d59bdf`  
		Last Modified: Fri, 12 Mar 2021 05:49:32 GMT  
		Size: 5.0 KB (5022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c00635c3d3412e964343152daaa8d6a574cff4476029d2dde8fbef8669643dd`  
		Last Modified: Fri, 12 Mar 2021 05:49:33 GMT  
		Size: 2.1 MB (2075174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42b36f1c725910664c120ab3e1137c10c516bc764114217862137f86de0b0a96`  
		Last Modified: Fri, 12 Mar 2021 05:49:32 GMT  
		Size: 1.2 MB (1178974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec7c9cae013d3da2b75c61f808eb35db46f6ea8b4aec6a394c20f9b42341f46c`  
		Last Modified: Fri, 12 Mar 2021 05:49:32 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccaed15ca3b93815844f5b39c66fe6edae8ec39ae3a186a3470e9c8f53909018`  
		Last Modified: Fri, 12 Mar 2021 05:49:32 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.9` - linux; 386

```console
$ docker pull memcached@sha256:ef0460019399121409cd24063e18f58e7f89f6c6dd0c9e6405441876555dfc21
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.2 MB (31178982 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91f0b8c30945bbb159fc82df44b331add3a586ea0e9d264dd6e26e9733278cb4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 12 Mar 2021 01:44:27 GMT
ADD file:90c103e04bd6fe0f39733cbf8eb2d8845aed3e4fc3fd1e5c3354df69e40aa615 in / 
# Fri, 12 Mar 2021 01:44:28 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 13:31:23 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Fri, 12 Mar 2021 13:31:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 13:31:28 GMT
ENV MEMCACHED_VERSION=1.6.9
# Fri, 12 Mar 2021 13:31:28 GMT
ENV MEMCACHED_SHA1=42ae062094fdf083cfe7b21ff377c781011c2be1
# Fri, 12 Mar 2021 13:35:32 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Fri, 12 Mar 2021 13:35:32 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 12 Mar 2021 13:35:33 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 12 Mar 2021 13:35:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 12 Mar 2021 13:35:33 GMT
USER memcache
# Fri, 12 Mar 2021 13:35:33 GMT
EXPOSE 11211
# Fri, 12 Mar 2021 13:35:34 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:0898aa7472f57f223652846337cf862f142e109d0c039b41886e7f20c345f85e`  
		Last Modified: Fri, 12 Mar 2021 01:52:08 GMT  
		Size: 27.8 MB (27760948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f32ccac2f28603415b89f000eac53a764ccb5e4a5c7bb96f531886d346046066`  
		Last Modified: Fri, 12 Mar 2021 13:40:40 GMT  
		Size: 4.9 KB (4895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ca797dc44ad9702a16634c4e34b2809570c531a00ea77bc688afbc168ef7ee4`  
		Last Modified: Fri, 12 Mar 2021 13:40:41 GMT  
		Size: 2.2 MB (2208684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e11aea04bae299d4a9ad55384df0c485fc53e5a9ca08c49f9905056753b6d4e6`  
		Last Modified: Fri, 12 Mar 2021 13:40:41 GMT  
		Size: 1.2 MB (1204047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1793a72e67f7bf9006a9aa26f1c569f4f92bc9ac6d93ea73f96d8a05bfd5e0a6`  
		Last Modified: Fri, 12 Mar 2021 13:40:40 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:999651c299c9f7bd71c0b15ecb302b22f3f03f36924d3144b76eb81e619d0184`  
		Last Modified: Fri, 12 Mar 2021 13:40:40 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.9` - linux; mips64le

```console
$ docker pull memcached@sha256:8ea232e21a6f020459a12dd1d7aedc8474594927363ba4aec07ce413deb9bed5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.8 MB (28752902 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:068f62f8ad395edfb2fda7af67488827096540267d3151dc47631195b1fc9543`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 12 Mar 2021 02:10:02 GMT
ADD file:491c5ca15fe098b83de42861289c216c693d788a1f9e739a78acefb0cad453c8 in / 
# Fri, 12 Mar 2021 02:10:03 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 08:46:26 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Fri, 12 Mar 2021 08:46:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 08:46:39 GMT
ENV MEMCACHED_VERSION=1.6.9
# Fri, 12 Mar 2021 08:46:39 GMT
ENV MEMCACHED_SHA1=42ae062094fdf083cfe7b21ff377c781011c2be1
# Fri, 12 Mar 2021 08:52:26 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Fri, 12 Mar 2021 08:52:27 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 12 Mar 2021 08:52:28 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 12 Mar 2021 08:52:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 12 Mar 2021 08:52:29 GMT
USER memcache
# Fri, 12 Mar 2021 08:52:29 GMT
EXPOSE 11211
# Fri, 12 Mar 2021 08:52:30 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:d0b6b2cc51bdde474395b8c32ff8012e471727bba69f221cfb79b46e8283f047`  
		Last Modified: Fri, 12 Mar 2021 02:17:07 GMT  
		Size: 25.8 MB (25772338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22086edc87e18d40945456938ba809ad0b1153dcf874df2911314f3fa0d76667`  
		Last Modified: Fri, 12 Mar 2021 08:52:45 GMT  
		Size: 5.0 KB (4978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b808a76ea31d9ba92e88100192f485f4efc2f9c15b24c41990aa202a0ed1a508`  
		Last Modified: Fri, 12 Mar 2021 08:52:46 GMT  
		Size: 1.8 MB (1776385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afada1a8592c3da748b0b5ac6d6a4db3f02704fb3785a7e1cc13a6b4fd5b1010`  
		Last Modified: Fri, 12 Mar 2021 08:52:46 GMT  
		Size: 1.2 MB (1198794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:276d546ec9c236bf7813ab6f11ccc55c6e127f0ea72ccbb36c035dbe52d675f6`  
		Last Modified: Fri, 12 Mar 2021 08:52:45 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a11a440437df39f7b30113415724385ba8643faf61547a4148083c19dd934eaa`  
		Last Modified: Fri, 12 Mar 2021 08:52:45 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.9` - linux; ppc64le

```console
$ docker pull memcached@sha256:efd3d67a1afd293b38dc0ebf78641266104fa8f44735e0b6210117d914f67250
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.1 MB (34087167 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:95699b572190f07b90f87f36f5f2e01c0073b7ac7241544c9c5d156985b817b4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 12 Mar 2021 02:32:43 GMT
ADD file:6a0c0cfa71979cf6fdd859dce1e32582f0e55ed382b9e17b77a2001defc2c9db in / 
# Fri, 12 Mar 2021 02:32:50 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 05:42:18 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Fri, 12 Mar 2021 05:42:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 05:42:50 GMT
ENV MEMCACHED_VERSION=1.6.9
# Fri, 12 Mar 2021 05:42:55 GMT
ENV MEMCACHED_SHA1=42ae062094fdf083cfe7b21ff377c781011c2be1
# Fri, 12 Mar 2021 05:51:27 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Fri, 12 Mar 2021 05:51:31 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 12 Mar 2021 05:51:53 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 12 Mar 2021 05:51:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 12 Mar 2021 05:52:07 GMT
USER memcache
# Fri, 12 Mar 2021 05:52:14 GMT
EXPOSE 11211
# Fri, 12 Mar 2021 05:52:21 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:1d686056fdac1848f4fd78ba2b335502055ffe98c79619e21d0c2fb7db95257e`  
		Last Modified: Fri, 12 Mar 2021 02:45:35 GMT  
		Size: 30.5 MB (30525728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73b1efcdfc9b290f77d5235f4f3bec7b09d62026296bb6dfccbdba7354df9caa`  
		Last Modified: Fri, 12 Mar 2021 05:52:55 GMT  
		Size: 5.0 KB (4994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0ae8f3e8315ccb25bd80ff467115a6f3479c6b5acf818ad7e3fcf4af0b2ebe1`  
		Last Modified: Fri, 12 Mar 2021 05:52:56 GMT  
		Size: 2.3 MB (2323017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0f34bd86e0ac5d50a3f227ab5cc3190a8a0973ea12c7e827d9267cad4dad482`  
		Last Modified: Fri, 12 Mar 2021 05:52:55 GMT  
		Size: 1.2 MB (1233020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a188c62ab305cd93f469a414ef7da5b0f1c3e66817ea0439a7530e194f90d05f`  
		Last Modified: Fri, 12 Mar 2021 05:52:55 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b5898f549c8d0705d12413acbc320c216d8a65dd1c312d1da6e8fe53df526e6`  
		Last Modified: Fri, 12 Mar 2021 05:52:55 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.9` - linux; s390x

```console
$ docker pull memcached@sha256:5e844fb7cd8aa06589f899a421921d452ade52de1e969ae763d60fecece294e9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.8 MB (28806644 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e79898684368a64d853c29bb82cfb9688df1e0230116c145e7f137796fb3eb4f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 12 Mar 2021 01:46:04 GMT
ADD file:afec039adf230a9186a38b57eed85262696f8d178ac649a445657066f16fe806 in / 
# Fri, 12 Mar 2021 01:46:07 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 02:55:40 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Fri, 12 Mar 2021 02:55:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 02:55:46 GMT
ENV MEMCACHED_VERSION=1.6.9
# Fri, 12 Mar 2021 02:55:46 GMT
ENV MEMCACHED_SHA1=42ae062094fdf083cfe7b21ff377c781011c2be1
# Fri, 12 Mar 2021 02:59:29 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Fri, 12 Mar 2021 02:59:29 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 12 Mar 2021 02:59:30 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 12 Mar 2021 02:59:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 12 Mar 2021 02:59:31 GMT
USER memcache
# Fri, 12 Mar 2021 02:59:31 GMT
EXPOSE 11211
# Fri, 12 Mar 2021 02:59:31 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:d41215965c091534e809ab2e8f4a2c1cebee3de536c2c74a7bc8302bbc8af7e1`  
		Last Modified: Fri, 12 Mar 2021 01:50:30 GMT  
		Size: 25.7 MB (25716294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c86c43c934421c76725f64bbc35ebb36c5f5c8dd181f6f701101068a31671d10`  
		Last Modified: Fri, 12 Mar 2021 02:59:59 GMT  
		Size: 5.0 KB (5025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97631e025d45847d90b38975ee3e031618e6eeedc1077b6ab77612d1edcda2e5`  
		Last Modified: Fri, 12 Mar 2021 02:59:59 GMT  
		Size: 1.9 MB (1886402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e98fc6e9a78adb22f7fb53ccc28169914f61a8f89c7c414f8d7b7eb22460b5f2`  
		Last Modified: Fri, 12 Mar 2021 02:59:59 GMT  
		Size: 1.2 MB (1198516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f9b27ffa18edb87e225a25d6bba459f4ae8a473944cebb847fe0e13a78e84fa`  
		Last Modified: Fri, 12 Mar 2021 02:59:59 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82ff067463b04909884ea6e0adda53fb48c398ee27e4ea1ae7de1dc5d5107151`  
		Last Modified: Fri, 12 Mar 2021 02:59:59 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:1.6.9-alpine`

```console
$ docker pull memcached@sha256:a1a84ac6bba5b100e79cff5819072ea05815a3597af2611713313ff77df7b799
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

### `memcached:1.6.9-alpine` - linux; amd64

```console
$ docker pull memcached@sha256:e799e863cd8dd7c6143457541d4e881f29d2a8cc7cf36a9e73afc075b88eaf66
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3835911 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:336eae34e88e7f26ba0efae7e37fae40bf1ec0752a3dd074d2bce3a5be74de7b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 25 Mar 2021 22:19:32 GMT
ADD file:6b081cabb4b256ee07587d249c4989b5b679375529542b81550a65b6f19f274e in / 
# Thu, 25 Mar 2021 22:19:32 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 09:38:12 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Fri, 26 Mar 2021 09:38:13 GMT
RUN apk add --no-cache libsasl
# Fri, 26 Mar 2021 09:38:13 GMT
ENV MEMCACHED_VERSION=1.6.9
# Fri, 26 Mar 2021 09:38:13 GMT
ENV MEMCACHED_SHA1=42ae062094fdf083cfe7b21ff377c781011c2be1
# Fri, 26 Mar 2021 09:42:08 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Fri, 26 Mar 2021 09:42:09 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 26 Mar 2021 09:42:10 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 26 Mar 2021 09:42:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 09:42:10 GMT
USER memcache
# Fri, 26 Mar 2021 09:42:10 GMT
EXPOSE 11211
# Fri, 26 Mar 2021 09:42:10 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:9aae54b2144e5b2b00c610f8805128f4f86822e1e52d3714c463744a431f0f4a`  
		Last Modified: Thu, 25 Mar 2021 22:20:18 GMT  
		Size: 2.8 MB (2811681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaefa880f46a5755d51d3e45077e1fff44e5aa93933777ec97b9bfb3e1c49715`  
		Last Modified: Fri, 26 Mar 2021 09:42:36 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:436a992a8a9c2b399a06843e7951676cc5efb57378f1a726fca25f55b904237b`  
		Last Modified: Fri, 26 Mar 2021 09:42:36 GMT  
		Size: 155.2 KB (155225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9747edb09d86e22df4e111c143640611fbbdbf5a0f237e80d04be2fb931eb722`  
		Last Modified: Fri, 26 Mar 2021 09:42:36 GMT  
		Size: 867.3 KB (867342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19d066699265da7027a01cffac223114af68d0a3976802f8f32b74cda0fe7186`  
		Last Modified: Fri, 26 Mar 2021 09:42:36 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1b3657184e4138b203aec9c7e53a1084c53ef07e21addc6dd924298728967e1`  
		Last Modified: Fri, 26 Mar 2021 09:42:37 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.9-alpine` - linux; arm variant v6

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

### `memcached:1.6.9-alpine` - linux; arm variant v7

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

### `memcached:1.6.9-alpine` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:7a16955ceb59429c180ba0e27b2110942bf9f5bc2bfcf776c367fa04e2947d61
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.7 MB (3724062 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:01d2695ea7aff546d998d8385f91a0c93c4e6f1f1bedb46f36e5c1c321d67509`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 25 Mar 2021 22:40:10 GMT
ADD file:8d7431f7e3e42b162a1626e7abf4ef7605146671dccc753d490de6b7fe429261 in / 
# Thu, 25 Mar 2021 22:40:23 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 11:55:58 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Fri, 26 Mar 2021 11:56:05 GMT
RUN apk add --no-cache libsasl
# Fri, 26 Mar 2021 11:56:08 GMT
ENV MEMCACHED_VERSION=1.6.9
# Fri, 26 Mar 2021 11:56:11 GMT
ENV MEMCACHED_SHA1=42ae062094fdf083cfe7b21ff377c781011c2be1
# Fri, 26 Mar 2021 11:59:21 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Fri, 26 Mar 2021 11:59:23 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 26 Mar 2021 11:59:25 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 26 Mar 2021 11:59:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 11:59:26 GMT
USER memcache
# Fri, 26 Mar 2021 11:59:27 GMT
EXPOSE 11211
# Fri, 26 Mar 2021 11:59:28 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:5ceb5101e3b0d54efb5f18318982508a04b181b4d5ae52b096dd35dea3a006cc`  
		Last Modified: Thu, 25 Mar 2021 22:44:41 GMT  
		Size: 2.7 MB (2711898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33c67e7215624376f623cadc677e6e078a62b0994949432d87e37d4bc0bd84d7`  
		Last Modified: Fri, 26 Mar 2021 11:59:55 GMT  
		Size: 1.3 KB (1256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d58f5b5b7d00e1ba2d3fdcc8cafc38b603be1002827ac0df0b581b0bb9387ca`  
		Last Modified: Fri, 26 Mar 2021 11:59:55 GMT  
		Size: 157.4 KB (157363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df4c0873fa7bdc463d82bc203d043bfb4b2959f34c3537de34b5a16b54d2dd83`  
		Last Modified: Fri, 26 Mar 2021 11:59:55 GMT  
		Size: 853.1 KB (853138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57ee3d4d0da34f5745af3bc3f88f5e034f7efe899653af6cb58126725451abab`  
		Last Modified: Fri, 26 Mar 2021 11:59:55 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7211bb020587c3ab33ad007f676f6697975abb98bb048f02c82cccf0ae12276`  
		Last Modified: Fri, 26 Mar 2021 11:59:55 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.9-alpine` - linux; 386

```console
$ docker pull memcached@sha256:ea129f66d114842cd4596d7655d2f04e9b63861794c06211d74b7b1be7f5cfbb
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3867250 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:530c4a3f88e64027883db802c0367dfbd69ba9fb503285c61c29f383d223f80b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 25 Mar 2021 22:38:25 GMT
ADD file:8953415d4b98f486af17a39ba53b38f7262aa590734c18ff9318927e5a705baf in / 
# Thu, 25 Mar 2021 22:38:26 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 10:46:47 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Fri, 26 Mar 2021 10:46:49 GMT
RUN apk add --no-cache libsasl
# Fri, 26 Mar 2021 10:46:49 GMT
ENV MEMCACHED_VERSION=1.6.9
# Fri, 26 Mar 2021 10:46:49 GMT
ENV MEMCACHED_SHA1=42ae062094fdf083cfe7b21ff377c781011c2be1
# Fri, 26 Mar 2021 10:50:57 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Fri, 26 Mar 2021 10:50:57 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 26 Mar 2021 10:50:58 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 26 Mar 2021 10:50:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 10:50:58 GMT
USER memcache
# Fri, 26 Mar 2021 10:50:59 GMT
EXPOSE 11211
# Fri, 26 Mar 2021 10:50:59 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:1fbd1c9912b638ce64a4740e3af7a3a03452f8705b8103950d677f1d79ae8164`  
		Last Modified: Thu, 25 Mar 2021 22:39:34 GMT  
		Size: 2.8 MB (2818129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:741d80ca4d99ded9e0725802bae206c2f75cf810363ec08ff97ac36608ab2c44`  
		Last Modified: Fri, 26 Mar 2021 10:51:39 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aee79c2789c7c2625b2f4b749e93967edce4a64eb9f0175ee1ce48206184fe07`  
		Last Modified: Fri, 26 Mar 2021 10:51:39 GMT  
		Size: 168.7 KB (168723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b298ea91522ee7dcd7d3716875dc9710f0af384ad866b28ab6a95f9f4aacfc36`  
		Last Modified: Fri, 26 Mar 2021 10:51:40 GMT  
		Size: 878.7 KB (878735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89f365d3ac6496ec95cd6a55b24893347ff9fa2a3fec8f0b6d5ac1757c8c2578`  
		Last Modified: Fri, 26 Mar 2021 10:51:39 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc1ff81bdf527601d8b1a55b9a43faf1c2571d8c8a3a1ad261bfef6ad920de05`  
		Last Modified: Fri, 26 Mar 2021 10:51:39 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.9-alpine` - linux; ppc64le

```console
$ docker pull memcached@sha256:3565226caf1343498d212e8dddf18067c4b6c0a45255fe1bfce7991414be07ff
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3889240 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd5e38aa6a933e9c61f4f1722dea74085d48c2b5e3be4d794a1ba005b9ee4257`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 25 Mar 2021 22:22:28 GMT
ADD file:f91f8e0aa646cb847f6e210056280f9332382ad2f8d6a8839fd9aa69b81c4a2a in / 
# Thu, 25 Mar 2021 22:22:30 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 07:17:34 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Fri, 26 Mar 2021 07:18:03 GMT
RUN apk add --no-cache libsasl
# Fri, 26 Mar 2021 07:18:10 GMT
ENV MEMCACHED_VERSION=1.6.9
# Fri, 26 Mar 2021 07:18:21 GMT
ENV MEMCACHED_SHA1=42ae062094fdf083cfe7b21ff377c781011c2be1
# Fri, 26 Mar 2021 07:22:17 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Fri, 26 Mar 2021 07:22:36 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 26 Mar 2021 07:23:13 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 26 Mar 2021 07:23:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 07:23:59 GMT
USER memcache
# Fri, 26 Mar 2021 07:24:14 GMT
EXPOSE 11211
# Fri, 26 Mar 2021 07:24:25 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:f3b2866c25f0a9167af050d646a7a740ccc88d46e068c90ff28a5c2ec2ee0030`  
		Last Modified: Thu, 25 Mar 2021 22:24:08 GMT  
		Size: 2.8 MB (2813115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b44508f603fc78a9e285af9f3c471b504f550a5e8a0f40e6a2bf7b715c6f777a`  
		Last Modified: Fri, 26 Mar 2021 07:25:02 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08d912e9739268eaf715a74f79cc127aca3a4a148f08b54920481b42ef98688c`  
		Last Modified: Fri, 26 Mar 2021 07:25:02 GMT  
		Size: 179.4 KB (179407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:759ed9ae532838d207b902a238c9494dd4a31357df138e862c4e3ca33cb8489b`  
		Last Modified: Fri, 26 Mar 2021 07:25:02 GMT  
		Size: 895.0 KB (895049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4fc0cf47cb2958e8c26cf38a6df13121c2b6fc0b65261fd9b72503e5f2b5f44`  
		Last Modified: Fri, 26 Mar 2021 07:25:02 GMT  
		Size: 282.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc6309f228ff45d777bd633ce1142b7bafd7daf6ceb8330f9977261f2b2cade4`  
		Last Modified: Fri, 26 Mar 2021 07:25:02 GMT  
		Size: 120.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.9-alpine` - linux; s390x

```console
$ docker pull memcached@sha256:d3b1ceba59f4053aa3482a6f89186e6f669a3404bfe219d140f87485d92810eb
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.6 MB (3627991 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb3ae3389c5204551f2fdb3f9ec1049e46002666bf93c3a9c59556db44409a19`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 25 Mar 2021 22:41:34 GMT
ADD file:44e2c7cd992fc98df702bef7022e0f8c4ee86312c311ab5ae185fd5fc878edf9 in / 
# Thu, 25 Mar 2021 22:41:34 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 00:01:52 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Fri, 26 Mar 2021 00:01:53 GMT
RUN apk add --no-cache libsasl
# Fri, 26 Mar 2021 00:01:54 GMT
ENV MEMCACHED_VERSION=1.6.9
# Fri, 26 Mar 2021 00:01:54 GMT
ENV MEMCACHED_SHA1=42ae062094fdf083cfe7b21ff377c781011c2be1
# Fri, 26 Mar 2021 00:05:59 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Fri, 26 Mar 2021 00:05:59 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 26 Mar 2021 00:06:00 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 26 Mar 2021 00:06:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 00:06:01 GMT
USER memcache
# Fri, 26 Mar 2021 00:06:01 GMT
EXPOSE 11211
# Fri, 26 Mar 2021 00:06:01 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:a266c0a9554add02ea09a46b8584cb36b7f606b7b4398b9ad7369f899f8360df`  
		Last Modified: Thu, 25 Mar 2021 22:42:07 GMT  
		Size: 2.6 MB (2602387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba7d3fc0e072913222e5431a4623bafe2581832cfa9017ed6f895763ee9f68ec`  
		Last Modified: Fri, 26 Mar 2021 00:06:23 GMT  
		Size: 1.3 KB (1256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42592fd9e69eae21d62d27596306a0184129ade75259eca72565bd3d8952981a`  
		Last Modified: Fri, 26 Mar 2021 00:06:24 GMT  
		Size: 161.2 KB (161193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1e129edd5e146d9cc6a328abaa83a73b63b501b30a6cb0bdedc4011e0b09b74`  
		Last Modified: Fri, 26 Mar 2021 00:06:23 GMT  
		Size: 862.8 KB (862751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e816e90ee5e4b4a419d2458929ef3017531e034768d7e5e38ba964fca8c57f07`  
		Last Modified: Fri, 26 Mar 2021 00:06:23 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2e7804a791461e688f20e06d5c4370728c765d161605d2f47a705f026fe2395`  
		Last Modified: Fri, 26 Mar 2021 00:06:23 GMT  
		Size: 120.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:alpine`

```console
$ docker pull memcached@sha256:a1a84ac6bba5b100e79cff5819072ea05815a3597af2611713313ff77df7b799
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
$ docker pull memcached@sha256:e799e863cd8dd7c6143457541d4e881f29d2a8cc7cf36a9e73afc075b88eaf66
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3835911 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:336eae34e88e7f26ba0efae7e37fae40bf1ec0752a3dd074d2bce3a5be74de7b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 25 Mar 2021 22:19:32 GMT
ADD file:6b081cabb4b256ee07587d249c4989b5b679375529542b81550a65b6f19f274e in / 
# Thu, 25 Mar 2021 22:19:32 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 09:38:12 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Fri, 26 Mar 2021 09:38:13 GMT
RUN apk add --no-cache libsasl
# Fri, 26 Mar 2021 09:38:13 GMT
ENV MEMCACHED_VERSION=1.6.9
# Fri, 26 Mar 2021 09:38:13 GMT
ENV MEMCACHED_SHA1=42ae062094fdf083cfe7b21ff377c781011c2be1
# Fri, 26 Mar 2021 09:42:08 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Fri, 26 Mar 2021 09:42:09 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 26 Mar 2021 09:42:10 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 26 Mar 2021 09:42:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 09:42:10 GMT
USER memcache
# Fri, 26 Mar 2021 09:42:10 GMT
EXPOSE 11211
# Fri, 26 Mar 2021 09:42:10 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:9aae54b2144e5b2b00c610f8805128f4f86822e1e52d3714c463744a431f0f4a`  
		Last Modified: Thu, 25 Mar 2021 22:20:18 GMT  
		Size: 2.8 MB (2811681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaefa880f46a5755d51d3e45077e1fff44e5aa93933777ec97b9bfb3e1c49715`  
		Last Modified: Fri, 26 Mar 2021 09:42:36 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:436a992a8a9c2b399a06843e7951676cc5efb57378f1a726fca25f55b904237b`  
		Last Modified: Fri, 26 Mar 2021 09:42:36 GMT  
		Size: 155.2 KB (155225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9747edb09d86e22df4e111c143640611fbbdbf5a0f237e80d04be2fb931eb722`  
		Last Modified: Fri, 26 Mar 2021 09:42:36 GMT  
		Size: 867.3 KB (867342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19d066699265da7027a01cffac223114af68d0a3976802f8f32b74cda0fe7186`  
		Last Modified: Fri, 26 Mar 2021 09:42:36 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1b3657184e4138b203aec9c7e53a1084c53ef07e21addc6dd924298728967e1`  
		Last Modified: Fri, 26 Mar 2021 09:42:37 GMT  
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
$ docker pull memcached@sha256:7a16955ceb59429c180ba0e27b2110942bf9f5bc2bfcf776c367fa04e2947d61
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.7 MB (3724062 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:01d2695ea7aff546d998d8385f91a0c93c4e6f1f1bedb46f36e5c1c321d67509`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 25 Mar 2021 22:40:10 GMT
ADD file:8d7431f7e3e42b162a1626e7abf4ef7605146671dccc753d490de6b7fe429261 in / 
# Thu, 25 Mar 2021 22:40:23 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 11:55:58 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Fri, 26 Mar 2021 11:56:05 GMT
RUN apk add --no-cache libsasl
# Fri, 26 Mar 2021 11:56:08 GMT
ENV MEMCACHED_VERSION=1.6.9
# Fri, 26 Mar 2021 11:56:11 GMT
ENV MEMCACHED_SHA1=42ae062094fdf083cfe7b21ff377c781011c2be1
# Fri, 26 Mar 2021 11:59:21 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Fri, 26 Mar 2021 11:59:23 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 26 Mar 2021 11:59:25 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 26 Mar 2021 11:59:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 11:59:26 GMT
USER memcache
# Fri, 26 Mar 2021 11:59:27 GMT
EXPOSE 11211
# Fri, 26 Mar 2021 11:59:28 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:5ceb5101e3b0d54efb5f18318982508a04b181b4d5ae52b096dd35dea3a006cc`  
		Last Modified: Thu, 25 Mar 2021 22:44:41 GMT  
		Size: 2.7 MB (2711898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33c67e7215624376f623cadc677e6e078a62b0994949432d87e37d4bc0bd84d7`  
		Last Modified: Fri, 26 Mar 2021 11:59:55 GMT  
		Size: 1.3 KB (1256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d58f5b5b7d00e1ba2d3fdcc8cafc38b603be1002827ac0df0b581b0bb9387ca`  
		Last Modified: Fri, 26 Mar 2021 11:59:55 GMT  
		Size: 157.4 KB (157363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df4c0873fa7bdc463d82bc203d043bfb4b2959f34c3537de34b5a16b54d2dd83`  
		Last Modified: Fri, 26 Mar 2021 11:59:55 GMT  
		Size: 853.1 KB (853138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57ee3d4d0da34f5745af3bc3f88f5e034f7efe899653af6cb58126725451abab`  
		Last Modified: Fri, 26 Mar 2021 11:59:55 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7211bb020587c3ab33ad007f676f6697975abb98bb048f02c82cccf0ae12276`  
		Last Modified: Fri, 26 Mar 2021 11:59:55 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:alpine` - linux; 386

```console
$ docker pull memcached@sha256:ea129f66d114842cd4596d7655d2f04e9b63861794c06211d74b7b1be7f5cfbb
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3867250 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:530c4a3f88e64027883db802c0367dfbd69ba9fb503285c61c29f383d223f80b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 25 Mar 2021 22:38:25 GMT
ADD file:8953415d4b98f486af17a39ba53b38f7262aa590734c18ff9318927e5a705baf in / 
# Thu, 25 Mar 2021 22:38:26 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 10:46:47 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Fri, 26 Mar 2021 10:46:49 GMT
RUN apk add --no-cache libsasl
# Fri, 26 Mar 2021 10:46:49 GMT
ENV MEMCACHED_VERSION=1.6.9
# Fri, 26 Mar 2021 10:46:49 GMT
ENV MEMCACHED_SHA1=42ae062094fdf083cfe7b21ff377c781011c2be1
# Fri, 26 Mar 2021 10:50:57 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Fri, 26 Mar 2021 10:50:57 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 26 Mar 2021 10:50:58 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 26 Mar 2021 10:50:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 10:50:58 GMT
USER memcache
# Fri, 26 Mar 2021 10:50:59 GMT
EXPOSE 11211
# Fri, 26 Mar 2021 10:50:59 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:1fbd1c9912b638ce64a4740e3af7a3a03452f8705b8103950d677f1d79ae8164`  
		Last Modified: Thu, 25 Mar 2021 22:39:34 GMT  
		Size: 2.8 MB (2818129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:741d80ca4d99ded9e0725802bae206c2f75cf810363ec08ff97ac36608ab2c44`  
		Last Modified: Fri, 26 Mar 2021 10:51:39 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aee79c2789c7c2625b2f4b749e93967edce4a64eb9f0175ee1ce48206184fe07`  
		Last Modified: Fri, 26 Mar 2021 10:51:39 GMT  
		Size: 168.7 KB (168723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b298ea91522ee7dcd7d3716875dc9710f0af384ad866b28ab6a95f9f4aacfc36`  
		Last Modified: Fri, 26 Mar 2021 10:51:40 GMT  
		Size: 878.7 KB (878735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89f365d3ac6496ec95cd6a55b24893347ff9fa2a3fec8f0b6d5ac1757c8c2578`  
		Last Modified: Fri, 26 Mar 2021 10:51:39 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc1ff81bdf527601d8b1a55b9a43faf1c2571d8c8a3a1ad261bfef6ad920de05`  
		Last Modified: Fri, 26 Mar 2021 10:51:39 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:alpine` - linux; ppc64le

```console
$ docker pull memcached@sha256:3565226caf1343498d212e8dddf18067c4b6c0a45255fe1bfce7991414be07ff
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3889240 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd5e38aa6a933e9c61f4f1722dea74085d48c2b5e3be4d794a1ba005b9ee4257`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 25 Mar 2021 22:22:28 GMT
ADD file:f91f8e0aa646cb847f6e210056280f9332382ad2f8d6a8839fd9aa69b81c4a2a in / 
# Thu, 25 Mar 2021 22:22:30 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 07:17:34 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Fri, 26 Mar 2021 07:18:03 GMT
RUN apk add --no-cache libsasl
# Fri, 26 Mar 2021 07:18:10 GMT
ENV MEMCACHED_VERSION=1.6.9
# Fri, 26 Mar 2021 07:18:21 GMT
ENV MEMCACHED_SHA1=42ae062094fdf083cfe7b21ff377c781011c2be1
# Fri, 26 Mar 2021 07:22:17 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Fri, 26 Mar 2021 07:22:36 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 26 Mar 2021 07:23:13 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 26 Mar 2021 07:23:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 07:23:59 GMT
USER memcache
# Fri, 26 Mar 2021 07:24:14 GMT
EXPOSE 11211
# Fri, 26 Mar 2021 07:24:25 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:f3b2866c25f0a9167af050d646a7a740ccc88d46e068c90ff28a5c2ec2ee0030`  
		Last Modified: Thu, 25 Mar 2021 22:24:08 GMT  
		Size: 2.8 MB (2813115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b44508f603fc78a9e285af9f3c471b504f550a5e8a0f40e6a2bf7b715c6f777a`  
		Last Modified: Fri, 26 Mar 2021 07:25:02 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08d912e9739268eaf715a74f79cc127aca3a4a148f08b54920481b42ef98688c`  
		Last Modified: Fri, 26 Mar 2021 07:25:02 GMT  
		Size: 179.4 KB (179407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:759ed9ae532838d207b902a238c9494dd4a31357df138e862c4e3ca33cb8489b`  
		Last Modified: Fri, 26 Mar 2021 07:25:02 GMT  
		Size: 895.0 KB (895049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4fc0cf47cb2958e8c26cf38a6df13121c2b6fc0b65261fd9b72503e5f2b5f44`  
		Last Modified: Fri, 26 Mar 2021 07:25:02 GMT  
		Size: 282.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc6309f228ff45d777bd633ce1142b7bafd7daf6ceb8330f9977261f2b2cade4`  
		Last Modified: Fri, 26 Mar 2021 07:25:02 GMT  
		Size: 120.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:alpine` - linux; s390x

```console
$ docker pull memcached@sha256:d3b1ceba59f4053aa3482a6f89186e6f669a3404bfe219d140f87485d92810eb
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.6 MB (3627991 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb3ae3389c5204551f2fdb3f9ec1049e46002666bf93c3a9c59556db44409a19`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 25 Mar 2021 22:41:34 GMT
ADD file:44e2c7cd992fc98df702bef7022e0f8c4ee86312c311ab5ae185fd5fc878edf9 in / 
# Thu, 25 Mar 2021 22:41:34 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 00:01:52 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Fri, 26 Mar 2021 00:01:53 GMT
RUN apk add --no-cache libsasl
# Fri, 26 Mar 2021 00:01:54 GMT
ENV MEMCACHED_VERSION=1.6.9
# Fri, 26 Mar 2021 00:01:54 GMT
ENV MEMCACHED_SHA1=42ae062094fdf083cfe7b21ff377c781011c2be1
# Fri, 26 Mar 2021 00:05:59 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Fri, 26 Mar 2021 00:05:59 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 26 Mar 2021 00:06:00 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 26 Mar 2021 00:06:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 00:06:01 GMT
USER memcache
# Fri, 26 Mar 2021 00:06:01 GMT
EXPOSE 11211
# Fri, 26 Mar 2021 00:06:01 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:a266c0a9554add02ea09a46b8584cb36b7f606b7b4398b9ad7369f899f8360df`  
		Last Modified: Thu, 25 Mar 2021 22:42:07 GMT  
		Size: 2.6 MB (2602387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba7d3fc0e072913222e5431a4623bafe2581832cfa9017ed6f895763ee9f68ec`  
		Last Modified: Fri, 26 Mar 2021 00:06:23 GMT  
		Size: 1.3 KB (1256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42592fd9e69eae21d62d27596306a0184129ade75259eca72565bd3d8952981a`  
		Last Modified: Fri, 26 Mar 2021 00:06:24 GMT  
		Size: 161.2 KB (161193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1e129edd5e146d9cc6a328abaa83a73b63b501b30a6cb0bdedc4011e0b09b74`  
		Last Modified: Fri, 26 Mar 2021 00:06:23 GMT  
		Size: 862.8 KB (862751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e816e90ee5e4b4a419d2458929ef3017531e034768d7e5e38ba964fca8c57f07`  
		Last Modified: Fri, 26 Mar 2021 00:06:23 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2e7804a791461e688f20e06d5c4370728c765d161605d2f47a705f026fe2395`  
		Last Modified: Fri, 26 Mar 2021 00:06:23 GMT  
		Size: 120.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:latest`

```console
$ docker pull memcached@sha256:aedbed05133579a286baaffce576b360a3860b5644d7e4bd39e8d0a26b847801
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
$ docker pull memcached@sha256:d8559d4ca748485fe7acf3bda5634902385c393b56991153d3259b1919b667b6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.5 MB (30510071 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c17a0df7f0b4ead3f7992531505b74f08210e464636782ff8d4e9f9c3f9ab634`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 12 Mar 2021 02:20:40 GMT
ADD file:3c32f1cd03198e141dd233a7ffd13444157d4150ad917d548f3ee9bf5953ce22 in / 
# Fri, 12 Mar 2021 02:20:41 GMT
CMD ["bash"]
# Sat, 13 Mar 2021 03:51:06 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Sat, 13 Mar 2021 03:51:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 13 Mar 2021 03:51:12 GMT
ENV MEMCACHED_VERSION=1.6.9
# Sat, 13 Mar 2021 03:51:12 GMT
ENV MEMCACHED_SHA1=42ae062094fdf083cfe7b21ff377c781011c2be1
# Sat, 13 Mar 2021 03:55:02 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Sat, 13 Mar 2021 03:55:03 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Sat, 13 Mar 2021 03:55:04 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Sat, 13 Mar 2021 03:55:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 13 Mar 2021 03:55:04 GMT
USER memcache
# Sat, 13 Mar 2021 03:55:04 GMT
EXPOSE 11211
# Sat, 13 Mar 2021 03:55:05 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:6f28985ad1843afd6fd4fe0b42a30bfab63c27d302362e7341e3316e8ba25ced`  
		Last Modified: Fri, 12 Mar 2021 02:26:11 GMT  
		Size: 27.1 MB (27101001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:007083158c847935c98d2d8c07518c8097b91da3a2fd7e15a6dbbb5f7e3de5e4`  
		Last Modified: Sat, 13 Mar 2021 03:59:56 GMT  
		Size: 5.0 KB (4977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44f9cc8fbeb0c17485aa8956f8ad64a7c24d44af44ea7b4883955f47996b189d`  
		Last Modified: Sat, 13 Mar 2021 03:59:57 GMT  
		Size: 2.2 MB (2197036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:955c0e8ce2a3821077059bb8198bc27098ef46dda29831d180cdc995186b345a`  
		Last Modified: Sat, 13 Mar 2021 03:59:56 GMT  
		Size: 1.2 MB (1206649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d8cc0a86221ff10b28b1a07db34deda0dfbc8f255f8a0911c518d91e2f84eba`  
		Last Modified: Sat, 13 Mar 2021 03:59:56 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7156f15be6833cf1ea0a3172ebe80928e5622768ad50c17b274b6004b6cc080`  
		Last Modified: Sat, 13 Mar 2021 03:59:56 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:latest` - linux; arm variant v5

```console
$ docker pull memcached@sha256:14a89ab8a75e421a79f0e3e65074b106d8b03e9b45fc0b6ff3ca1f7843e2176a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.9 MB (27928037 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a715778439ac19faacf97a009883e33c115543fe3a0f0deace9db3705ea9a7a2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 26 Mar 2021 07:51:46 GMT
ADD file:3dd25698bf1578e8580b2f437a2199bfc3b1818480b874d73622357e955a091f in / 
# Fri, 26 Mar 2021 07:51:48 GMT
CMD ["bash"]
# Fri, 26 Mar 2021 09:39:21 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Fri, 26 Mar 2021 09:39:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 09:39:34 GMT
ENV MEMCACHED_VERSION=1.6.9
# Fri, 26 Mar 2021 09:39:34 GMT
ENV MEMCACHED_SHA1=42ae062094fdf083cfe7b21ff377c781011c2be1
# Fri, 26 Mar 2021 09:43:40 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Fri, 26 Mar 2021 09:43:41 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 26 Mar 2021 09:43:44 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 26 Mar 2021 09:43:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 09:43:46 GMT
USER memcache
# Fri, 26 Mar 2021 09:43:47 GMT
EXPOSE 11211
# Fri, 26 Mar 2021 09:43:47 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:997e59852ec0e1a23e4a179db14793947d60390c392ce15abc0f811e797c49ca`  
		Last Modified: Fri, 26 Mar 2021 08:00:22 GMT  
		Size: 24.8 MB (24846159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bac4aeb1ec3f8bad5601293e2e6ee4892f2099bcdf754eca5a256713b4f4ac78`  
		Last Modified: Fri, 26 Mar 2021 09:44:00 GMT  
		Size: 4.9 KB (4893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c690f09a614f96a09cf57ab424bb57e240adc3cbfd1cc08482f124a479fad552`  
		Last Modified: Fri, 26 Mar 2021 09:44:02 GMT  
		Size: 1.9 MB (1897339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d144d9a91ac96cb9c068f67fc5649459003e9f9a21867638fb49840ed9e85e0`  
		Last Modified: Fri, 26 Mar 2021 09:44:01 GMT  
		Size: 1.2 MB (1179238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3160a064a6625a7ec9c8959cd13f6e9113a5c2cb59cbe8ea826ce8a210068b7e`  
		Last Modified: Fri, 26 Mar 2021 09:44:00 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e4455ba84cf78688e072088f68b9c85bc29af1a497039b5241c6291b5de1843`  
		Last Modified: Fri, 26 Mar 2021 09:44:00 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:latest` - linux; arm variant v7

```console
$ docker pull memcached@sha256:ca79781006a7d45818e0e9b0d51c954c9c9c4bde8336060bf04fc99cbd7809e3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.7 MB (25676128 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b26ff179f940a940395fc620c44eff4702a61bc989da3d71d318bc699dd4ed08`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 12 Mar 2021 02:00:12 GMT
ADD file:123da9848f87c8ed4c5122a104b8650564c09767725916f822def7b645a019f1 in / 
# Fri, 12 Mar 2021 02:00:14 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 03:08:21 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Fri, 12 Mar 2021 03:08:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 03:08:32 GMT
ENV MEMCACHED_VERSION=1.6.9
# Fri, 12 Mar 2021 03:08:33 GMT
ENV MEMCACHED_SHA1=42ae062094fdf083cfe7b21ff377c781011c2be1
# Fri, 12 Mar 2021 03:11:57 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Fri, 12 Mar 2021 03:11:58 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 12 Mar 2021 03:12:01 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 12 Mar 2021 03:12:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 12 Mar 2021 03:12:03 GMT
USER memcache
# Fri, 12 Mar 2021 03:12:04 GMT
EXPOSE 11211
# Fri, 12 Mar 2021 03:12:05 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:e12d26f75fe8b7fd14712965ff5178762227d07d2151bb35fa21105ddfc4a14a`  
		Last Modified: Fri, 12 Mar 2021 02:10:28 GMT  
		Size: 22.7 MB (22709467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe1e03071b3302ec91defd6b8b861a3be2a50d7165f73c154eea0ddd8339641a`  
		Last Modified: Fri, 12 Mar 2021 03:22:32 GMT  
		Size: 4.9 KB (4899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b11c24c5a0d1d4fa06df54624b6dc7a5d1586210047c31e44511fa513081a49e`  
		Last Modified: Fri, 12 Mar 2021 03:22:33 GMT  
		Size: 1.8 MB (1811657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57458ecd2770995b21c7c8d20108d84bc9b4879cd759054d4f8e122bb54a7451`  
		Last Modified: Fri, 12 Mar 2021 03:22:32 GMT  
		Size: 1.1 MB (1149703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6070aa36c0112c5a66ad85b5eaa4e4c954a217f484a915ff259fd30c5de332e6`  
		Last Modified: Fri, 12 Mar 2021 03:22:32 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1d498de6ccd0c3ffc78632677c24cad8f6acc9add31d9ef7fd69d57144fb0f4`  
		Last Modified: Fri, 12 Mar 2021 03:22:32 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:latest` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:fe157d34ccde3aa160d90472f6964aaca3c6b0554f2fa4317d8afceeff3c45cc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.1 MB (29116090 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d61a16162561c8b05c0af58a2555c292980d12cc41872efa2096ed9109377dee`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 12 Mar 2021 01:53:53 GMT
ADD file:6130ddc0a939dd72c0614de4aa77de47aa16fe211274bacb31995aa1a0526164 in / 
# Fri, 12 Mar 2021 01:53:56 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 05:45:15 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Fri, 12 Mar 2021 05:45:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 05:45:27 GMT
ENV MEMCACHED_VERSION=1.6.9
# Fri, 12 Mar 2021 05:45:28 GMT
ENV MEMCACHED_SHA1=42ae062094fdf083cfe7b21ff377c781011c2be1
# Fri, 12 Mar 2021 05:48:54 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Fri, 12 Mar 2021 05:48:55 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 12 Mar 2021 05:48:57 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 12 Mar 2021 05:48:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 12 Mar 2021 05:48:59 GMT
USER memcache
# Fri, 12 Mar 2021 05:49:00 GMT
EXPOSE 11211
# Fri, 12 Mar 2021 05:49:00 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:706ee5d0a6b53d9257cbea22d8409fb22c867ab3a001c65f6b8bfd37dace0e58`  
		Last Modified: Fri, 12 Mar 2021 02:01:39 GMT  
		Size: 25.9 MB (25856512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0d9e24f3287f849ddf4e4afe2c8fca91a1031b67a267cd2c779ac2592d59bdf`  
		Last Modified: Fri, 12 Mar 2021 05:49:32 GMT  
		Size: 5.0 KB (5022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c00635c3d3412e964343152daaa8d6a574cff4476029d2dde8fbef8669643dd`  
		Last Modified: Fri, 12 Mar 2021 05:49:33 GMT  
		Size: 2.1 MB (2075174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42b36f1c725910664c120ab3e1137c10c516bc764114217862137f86de0b0a96`  
		Last Modified: Fri, 12 Mar 2021 05:49:32 GMT  
		Size: 1.2 MB (1178974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec7c9cae013d3da2b75c61f808eb35db46f6ea8b4aec6a394c20f9b42341f46c`  
		Last Modified: Fri, 12 Mar 2021 05:49:32 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccaed15ca3b93815844f5b39c66fe6edae8ec39ae3a186a3470e9c8f53909018`  
		Last Modified: Fri, 12 Mar 2021 05:49:32 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:latest` - linux; 386

```console
$ docker pull memcached@sha256:ef0460019399121409cd24063e18f58e7f89f6c6dd0c9e6405441876555dfc21
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.2 MB (31178982 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91f0b8c30945bbb159fc82df44b331add3a586ea0e9d264dd6e26e9733278cb4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 12 Mar 2021 01:44:27 GMT
ADD file:90c103e04bd6fe0f39733cbf8eb2d8845aed3e4fc3fd1e5c3354df69e40aa615 in / 
# Fri, 12 Mar 2021 01:44:28 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 13:31:23 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Fri, 12 Mar 2021 13:31:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 13:31:28 GMT
ENV MEMCACHED_VERSION=1.6.9
# Fri, 12 Mar 2021 13:31:28 GMT
ENV MEMCACHED_SHA1=42ae062094fdf083cfe7b21ff377c781011c2be1
# Fri, 12 Mar 2021 13:35:32 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Fri, 12 Mar 2021 13:35:32 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 12 Mar 2021 13:35:33 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 12 Mar 2021 13:35:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 12 Mar 2021 13:35:33 GMT
USER memcache
# Fri, 12 Mar 2021 13:35:33 GMT
EXPOSE 11211
# Fri, 12 Mar 2021 13:35:34 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:0898aa7472f57f223652846337cf862f142e109d0c039b41886e7f20c345f85e`  
		Last Modified: Fri, 12 Mar 2021 01:52:08 GMT  
		Size: 27.8 MB (27760948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f32ccac2f28603415b89f000eac53a764ccb5e4a5c7bb96f531886d346046066`  
		Last Modified: Fri, 12 Mar 2021 13:40:40 GMT  
		Size: 4.9 KB (4895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ca797dc44ad9702a16634c4e34b2809570c531a00ea77bc688afbc168ef7ee4`  
		Last Modified: Fri, 12 Mar 2021 13:40:41 GMT  
		Size: 2.2 MB (2208684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e11aea04bae299d4a9ad55384df0c485fc53e5a9ca08c49f9905056753b6d4e6`  
		Last Modified: Fri, 12 Mar 2021 13:40:41 GMT  
		Size: 1.2 MB (1204047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1793a72e67f7bf9006a9aa26f1c569f4f92bc9ac6d93ea73f96d8a05bfd5e0a6`  
		Last Modified: Fri, 12 Mar 2021 13:40:40 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:999651c299c9f7bd71c0b15ecb302b22f3f03f36924d3144b76eb81e619d0184`  
		Last Modified: Fri, 12 Mar 2021 13:40:40 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:latest` - linux; mips64le

```console
$ docker pull memcached@sha256:8ea232e21a6f020459a12dd1d7aedc8474594927363ba4aec07ce413deb9bed5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.8 MB (28752902 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:068f62f8ad395edfb2fda7af67488827096540267d3151dc47631195b1fc9543`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 12 Mar 2021 02:10:02 GMT
ADD file:491c5ca15fe098b83de42861289c216c693d788a1f9e739a78acefb0cad453c8 in / 
# Fri, 12 Mar 2021 02:10:03 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 08:46:26 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Fri, 12 Mar 2021 08:46:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 08:46:39 GMT
ENV MEMCACHED_VERSION=1.6.9
# Fri, 12 Mar 2021 08:46:39 GMT
ENV MEMCACHED_SHA1=42ae062094fdf083cfe7b21ff377c781011c2be1
# Fri, 12 Mar 2021 08:52:26 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Fri, 12 Mar 2021 08:52:27 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 12 Mar 2021 08:52:28 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 12 Mar 2021 08:52:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 12 Mar 2021 08:52:29 GMT
USER memcache
# Fri, 12 Mar 2021 08:52:29 GMT
EXPOSE 11211
# Fri, 12 Mar 2021 08:52:30 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:d0b6b2cc51bdde474395b8c32ff8012e471727bba69f221cfb79b46e8283f047`  
		Last Modified: Fri, 12 Mar 2021 02:17:07 GMT  
		Size: 25.8 MB (25772338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22086edc87e18d40945456938ba809ad0b1153dcf874df2911314f3fa0d76667`  
		Last Modified: Fri, 12 Mar 2021 08:52:45 GMT  
		Size: 5.0 KB (4978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b808a76ea31d9ba92e88100192f485f4efc2f9c15b24c41990aa202a0ed1a508`  
		Last Modified: Fri, 12 Mar 2021 08:52:46 GMT  
		Size: 1.8 MB (1776385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afada1a8592c3da748b0b5ac6d6a4db3f02704fb3785a7e1cc13a6b4fd5b1010`  
		Last Modified: Fri, 12 Mar 2021 08:52:46 GMT  
		Size: 1.2 MB (1198794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:276d546ec9c236bf7813ab6f11ccc55c6e127f0ea72ccbb36c035dbe52d675f6`  
		Last Modified: Fri, 12 Mar 2021 08:52:45 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a11a440437df39f7b30113415724385ba8643faf61547a4148083c19dd934eaa`  
		Last Modified: Fri, 12 Mar 2021 08:52:45 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:latest` - linux; ppc64le

```console
$ docker pull memcached@sha256:efd3d67a1afd293b38dc0ebf78641266104fa8f44735e0b6210117d914f67250
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.1 MB (34087167 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:95699b572190f07b90f87f36f5f2e01c0073b7ac7241544c9c5d156985b817b4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 12 Mar 2021 02:32:43 GMT
ADD file:6a0c0cfa71979cf6fdd859dce1e32582f0e55ed382b9e17b77a2001defc2c9db in / 
# Fri, 12 Mar 2021 02:32:50 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 05:42:18 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Fri, 12 Mar 2021 05:42:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 05:42:50 GMT
ENV MEMCACHED_VERSION=1.6.9
# Fri, 12 Mar 2021 05:42:55 GMT
ENV MEMCACHED_SHA1=42ae062094fdf083cfe7b21ff377c781011c2be1
# Fri, 12 Mar 2021 05:51:27 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Fri, 12 Mar 2021 05:51:31 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 12 Mar 2021 05:51:53 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 12 Mar 2021 05:51:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 12 Mar 2021 05:52:07 GMT
USER memcache
# Fri, 12 Mar 2021 05:52:14 GMT
EXPOSE 11211
# Fri, 12 Mar 2021 05:52:21 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:1d686056fdac1848f4fd78ba2b335502055ffe98c79619e21d0c2fb7db95257e`  
		Last Modified: Fri, 12 Mar 2021 02:45:35 GMT  
		Size: 30.5 MB (30525728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73b1efcdfc9b290f77d5235f4f3bec7b09d62026296bb6dfccbdba7354df9caa`  
		Last Modified: Fri, 12 Mar 2021 05:52:55 GMT  
		Size: 5.0 KB (4994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0ae8f3e8315ccb25bd80ff467115a6f3479c6b5acf818ad7e3fcf4af0b2ebe1`  
		Last Modified: Fri, 12 Mar 2021 05:52:56 GMT  
		Size: 2.3 MB (2323017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0f34bd86e0ac5d50a3f227ab5cc3190a8a0973ea12c7e827d9267cad4dad482`  
		Last Modified: Fri, 12 Mar 2021 05:52:55 GMT  
		Size: 1.2 MB (1233020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a188c62ab305cd93f469a414ef7da5b0f1c3e66817ea0439a7530e194f90d05f`  
		Last Modified: Fri, 12 Mar 2021 05:52:55 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b5898f549c8d0705d12413acbc320c216d8a65dd1c312d1da6e8fe53df526e6`  
		Last Modified: Fri, 12 Mar 2021 05:52:55 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:latest` - linux; s390x

```console
$ docker pull memcached@sha256:5e844fb7cd8aa06589f899a421921d452ade52de1e969ae763d60fecece294e9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.8 MB (28806644 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e79898684368a64d853c29bb82cfb9688df1e0230116c145e7f137796fb3eb4f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 12 Mar 2021 01:46:04 GMT
ADD file:afec039adf230a9186a38b57eed85262696f8d178ac649a445657066f16fe806 in / 
# Fri, 12 Mar 2021 01:46:07 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 02:55:40 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Fri, 12 Mar 2021 02:55:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 02:55:46 GMT
ENV MEMCACHED_VERSION=1.6.9
# Fri, 12 Mar 2021 02:55:46 GMT
ENV MEMCACHED_SHA1=42ae062094fdf083cfe7b21ff377c781011c2be1
# Fri, 12 Mar 2021 02:59:29 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Fri, 12 Mar 2021 02:59:29 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 12 Mar 2021 02:59:30 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 12 Mar 2021 02:59:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 12 Mar 2021 02:59:31 GMT
USER memcache
# Fri, 12 Mar 2021 02:59:31 GMT
EXPOSE 11211
# Fri, 12 Mar 2021 02:59:31 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:d41215965c091534e809ab2e8f4a2c1cebee3de536c2c74a7bc8302bbc8af7e1`  
		Last Modified: Fri, 12 Mar 2021 01:50:30 GMT  
		Size: 25.7 MB (25716294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c86c43c934421c76725f64bbc35ebb36c5f5c8dd181f6f701101068a31671d10`  
		Last Modified: Fri, 12 Mar 2021 02:59:59 GMT  
		Size: 5.0 KB (5025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97631e025d45847d90b38975ee3e031618e6eeedc1077b6ab77612d1edcda2e5`  
		Last Modified: Fri, 12 Mar 2021 02:59:59 GMT  
		Size: 1.9 MB (1886402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e98fc6e9a78adb22f7fb53ccc28169914f61a8f89c7c414f8d7b7eb22460b5f2`  
		Last Modified: Fri, 12 Mar 2021 02:59:59 GMT  
		Size: 1.2 MB (1198516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f9b27ffa18edb87e225a25d6bba459f4ae8a473944cebb847fe0e13a78e84fa`  
		Last Modified: Fri, 12 Mar 2021 02:59:59 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82ff067463b04909884ea6e0adda53fb48c398ee27e4ea1ae7de1dc5d5107151`  
		Last Modified: Fri, 12 Mar 2021 02:59:59 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
