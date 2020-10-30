<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `memcached`

-	[`memcached:1`](#memcached1)
-	[`memcached:1.6`](#memcached16)
-	[`memcached:1.6.8`](#memcached168)
-	[`memcached:1.6.8-alpine`](#memcached168-alpine)
-	[`memcached:1.6-alpine`](#memcached16-alpine)
-	[`memcached:1-alpine`](#memcached1-alpine)
-	[`memcached:alpine`](#memcachedalpine)
-	[`memcached:latest`](#memcachedlatest)

## `memcached:1`

```console
$ docker pull memcached@sha256:2c765a372d3e82565bc12bba67a0eb246baf536fd296ff6cb2e21c4036a62831
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
$ docker pull memcached@sha256:7be440dd3cc068fa2be188a7183890a8ff36e25e5a0c2edab25a4b6b460817c6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.5 MB (30493455 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:556880cb3d94c1509adc3eaf68dadf7d5e7325c5e5d2dcb86a8d0f8e0b4e4529`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 13 Oct 2020 01:39:05 GMT
ADD file:0dc53e7886c35bc21ae6c4f6cedda54d56ae9c9e9cd367678f1a72e68b3c43d4 in / 
# Tue, 13 Oct 2020 01:39:05 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 07:40:55 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 13 Oct 2020 07:41:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Oct 2020 17:51:22 GMT
ENV MEMCACHED_VERSION=1.6.8
# Tue, 27 Oct 2020 17:51:22 GMT
ENV MEMCACHED_SHA1=8f3efd851efc5b822bd991b93d06a271b2fac052
# Fri, 30 Oct 2020 01:59:43 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Fri, 30 Oct 2020 01:59:44 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 30 Oct 2020 01:59:44 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 30 Oct 2020 01:59:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 30 Oct 2020 01:59:45 GMT
USER memcache
# Fri, 30 Oct 2020 01:59:45 GMT
EXPOSE 11211
# Fri, 30 Oct 2020 01:59:45 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:bb79b6b2107fea8e8a47133a660b78e3a546998fcf0427be39ac9a0af4a97e90`  
		Last Modified: Tue, 13 Oct 2020 01:48:17 GMT  
		Size: 27.1 MB (27092228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5fbfe4d7c9b06eab9107d9ee46dbff27ea09707a40bdbdbea1d34078e65142a`  
		Last Modified: Tue, 13 Oct 2020 08:01:25 GMT  
		Size: 5.0 KB (4983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ed56f4a4fee8ed574be57dd51df7dc9f5bbdb041e9704be5a9ae0072a8a48b7`  
		Last Modified: Tue, 13 Oct 2020 08:01:26 GMT  
		Size: 2.2 MB (2196479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0186bf1dbc662c1e09f0a98b1182f4f1406a4b69b308ef63e0122450cfbca1b`  
		Last Modified: Fri, 30 Oct 2020 02:04:29 GMT  
		Size: 1.2 MB (1199359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f36909c1fe5329c92a34b3cde57aa972e7a53e582b7068c66d5e6af5e95bd86`  
		Last Modified: Fri, 30 Oct 2020 02:04:28 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e82197d1329427273caed560c08d7606a51afbb9bb34d2e4c0ed8bed4691cd3`  
		Last Modified: Fri, 30 Oct 2020 02:04:29 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1` - linux; arm variant v5

```console
$ docker pull memcached@sha256:281302b1776f2c06bbd2889f393368d96c44bcf61a889b7bb892b3b646629dfe
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.9 MB (27911064 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5cf13656486a2eb6df7a579ba2a4e613c12a4869f2bcd85097752033b87b1925`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 13 Oct 2020 01:52:17 GMT
ADD file:b71c0fa4957d6b65af37231a105f3d17cdbafe5c7d6c37b5843ebf619c608aaa in / 
# Tue, 13 Oct 2020 01:52:27 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 02:22:47 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 13 Oct 2020 02:23:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Oct 2020 17:48:42 GMT
ENV MEMCACHED_VERSION=1.6.8
# Tue, 27 Oct 2020 17:48:43 GMT
ENV MEMCACHED_SHA1=8f3efd851efc5b822bd991b93d06a271b2fac052
# Fri, 30 Oct 2020 01:54:09 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Fri, 30 Oct 2020 01:54:10 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 30 Oct 2020 01:54:12 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 30 Oct 2020 01:54:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 30 Oct 2020 01:54:14 GMT
USER memcache
# Fri, 30 Oct 2020 01:54:15 GMT
EXPOSE 11211
# Fri, 30 Oct 2020 01:54:16 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:f991c1e1ee2c48f16625b6b61310bf3c0616c0dbda4762019117e86fd29cf9ce`  
		Last Modified: Tue, 13 Oct 2020 02:01:27 GMT  
		Size: 24.8 MB (24835992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1b39a87be5bf0605d95ec4fc44790226547fdbcbad21c2add60885e9a1eabee`  
		Last Modified: Tue, 13 Oct 2020 02:34:18 GMT  
		Size: 4.9 KB (4897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d6238e630abdd7bca871de31aed93435c3e250ba2af1a0aaaabbec9d93d4452`  
		Last Modified: Tue, 13 Oct 2020 02:34:18 GMT  
		Size: 1.9 MB (1896831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a06241971793ab22b3a7ab4db8c18fc14c5b20227169c41d8bfce8fb6d67daa`  
		Last Modified: Fri, 30 Oct 2020 01:54:40 GMT  
		Size: 1.2 MB (1172937 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebc8ed09958e4b60fdf69ea8d28015f4cd3491968a22eced8fbf02720e2441bc`  
		Last Modified: Fri, 30 Oct 2020 01:54:40 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cb0a67800b722bbe27460d77886606a93383f456390e153365e2c38ae8cd602`  
		Last Modified: Fri, 30 Oct 2020 01:54:40 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1` - linux; arm variant v7

```console
$ docker pull memcached@sha256:3eb85207ec7eee29d5490f1f5b618eb232e57ad2654c929784518b7e42a589eb
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.7 MB (25660769 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b0e3423db692c288e1ce77ef4dccf8da40c46880e5bf18d42e6d8962016acce`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 13 Oct 2020 00:59:29 GMT
ADD file:e423f30ca19eb205a98de21b0545d0a764cfc4f832a9a9631542354d914d98d9 in / 
# Tue, 13 Oct 2020 00:59:31 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 04:26:19 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 13 Oct 2020 04:26:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Oct 2020 17:52:08 GMT
ENV MEMCACHED_VERSION=1.6.8
# Tue, 27 Oct 2020 17:52:09 GMT
ENV MEMCACHED_SHA1=8f3efd851efc5b822bd991b93d06a271b2fac052
# Tue, 27 Oct 2020 18:02:11 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 27 Oct 2020 18:02:12 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 27 Oct 2020 18:02:15 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 27 Oct 2020 18:02:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 27 Oct 2020 18:02:17 GMT
USER memcache
# Tue, 27 Oct 2020 18:02:18 GMT
EXPOSE 11211
# Tue, 27 Oct 2020 18:02:19 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:d6d8411ad43db0022fa0fce094cd2e8b1dd2f8a09d6880ed9beb6b4204867027`  
		Last Modified: Tue, 13 Oct 2020 01:08:28 GMT  
		Size: 22.7 MB (22699849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e36226ec0f789bddc127720ec631e27d952fb15b96b7848f3834950832523090`  
		Last Modified: Tue, 13 Oct 2020 04:37:29 GMT  
		Size: 4.9 KB (4895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46d8cf8973d9daad3ec5b519371371403ed2da2e65fa64c43d9122e8b8d602dd`  
		Last Modified: Tue, 13 Oct 2020 04:37:30 GMT  
		Size: 1.8 MB (1811537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc6baa5172a099a2af7b8031778e24fb072fc19291862933280eda0de2c1f873`  
		Last Modified: Tue, 27 Oct 2020 18:12:59 GMT  
		Size: 1.1 MB (1144080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79a4d1aadb5fa75c62ccfcb25624f53a840376fd2d43e3f2a37c4638437f36e5`  
		Last Modified: Tue, 27 Oct 2020 18:12:58 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61e633bd02bf4bd63bb51de860e7a23925d24c287faa53882423e30f3f283dff`  
		Last Modified: Tue, 27 Oct 2020 18:12:58 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:d3355e1e1ca991f55ddc098c2f4795182e1c74228ddce7128898604bf04db22c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.1 MB (29100019 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a0715facdf2c1c1981d8ef7df462d2498fea30e381c80f46f6c8a2a2852d50e4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 13 Oct 2020 01:41:09 GMT
ADD file:3488b1423094a75be5bb5956e9187827b8dd35d7a1f2b14081f8e74a1629e7d0 in / 
# Tue, 13 Oct 2020 01:41:11 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 08:18:46 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 13 Oct 2020 08:18:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Oct 2020 17:50:52 GMT
ENV MEMCACHED_VERSION=1.6.8
# Tue, 27 Oct 2020 17:50:53 GMT
ENV MEMCACHED_SHA1=8f3efd851efc5b822bd991b93d06a271b2fac052
# Tue, 27 Oct 2020 18:01:23 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 27 Oct 2020 18:01:24 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 27 Oct 2020 18:01:27 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 27 Oct 2020 18:01:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 27 Oct 2020 18:01:28 GMT
USER memcache
# Tue, 27 Oct 2020 18:01:29 GMT
EXPOSE 11211
# Tue, 27 Oct 2020 18:01:29 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:4e6164a63b7b4cf981546947e191644c122214975d40b51ede0536791ebec3d4`  
		Last Modified: Tue, 13 Oct 2020 01:48:17 GMT  
		Size: 25.8 MB (25849329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5f7daf8dcdb72260976fee433136d1d7b10f4488b985960ff0cc9680258a37e`  
		Last Modified: Tue, 13 Oct 2020 08:29:40 GMT  
		Size: 5.0 KB (5026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3afc9b2342454a24b6fc4247345875720b7dce42da90e83c7b9a4abf57ff9257`  
		Last Modified: Tue, 13 Oct 2020 08:29:41 GMT  
		Size: 2.1 MB (2074972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:603fd7cc62d57991fc13951bf2f7e62b72e84aa1f942d74260c20c67319f7881`  
		Last Modified: Tue, 27 Oct 2020 18:12:12 GMT  
		Size: 1.2 MB (1170284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1741db6c55c297ff2a3645680bd6edd02a39a5414eb5eeac865437cf557a1965`  
		Last Modified: Tue, 27 Oct 2020 18:12:11 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4449d89ef06347eb4b3344c8149350461269d63e8c8e80e622fc44c2ac2a6f29`  
		Last Modified: Tue, 27 Oct 2020 18:12:11 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1` - linux; 386

```console
$ docker pull memcached@sha256:2de59fa093416ca4d4f33c162b006bedc526d2026d762c0bc434318fe947d32c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.2 MB (31161101 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2743c23aca6cb3863b084988e69eaad5de3ebf0cb317f57121ea69ba42d110af`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 13 Oct 2020 01:41:03 GMT
ADD file:51108b89c70ce0773c897be520c84454660f38b84ba556da49c7fe77e5d52416 in / 
# Tue, 13 Oct 2020 01:41:03 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 07:16:07 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 13 Oct 2020 07:16:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 07:16:13 GMT
ENV MEMCACHED_VERSION=1.6.7
# Tue, 13 Oct 2020 07:16:13 GMT
ENV MEMCACHED_SHA1=49336bb0a4b7ad296422b08148581ed54edf32d0
# Tue, 13 Oct 2020 07:36:28 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 13 Oct 2020 07:36:28 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 13 Oct 2020 07:36:29 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 13 Oct 2020 07:36:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Oct 2020 07:36:29 GMT
USER memcache
# Tue, 13 Oct 2020 07:36:30 GMT
EXPOSE 11211
# Tue, 13 Oct 2020 07:36:30 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:97e4efec21eea92209464547d0f52a0f773c505cf4ea9d8090cef667bde145b8`  
		Last Modified: Tue, 13 Oct 2020 01:48:54 GMT  
		Size: 27.8 MB (27750243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1e2733549a0a03eff9da2ad1035504ef29480a7fed2edb9ac19fcc6605081ec`  
		Last Modified: Tue, 13 Oct 2020 07:36:49 GMT  
		Size: 4.9 KB (4896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4434320f582eaf5fce7418fb99c35a07380e61385ed8d9ec07d383d46e426d06`  
		Last Modified: Tue, 13 Oct 2020 07:36:51 GMT  
		Size: 2.2 MB (2208112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0faf39e12c14d25e5dc802ddbe8f0068b4cc492ebf1e078998ddf38205c836dd`  
		Last Modified: Tue, 13 Oct 2020 07:36:49 GMT  
		Size: 1.2 MB (1197441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b95b4020f31dffe1467a69cfe85d22f7c6fa9d76da3678c72c99f23254899fb`  
		Last Modified: Tue, 13 Oct 2020 07:36:49 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5193dc6218dcc26a610b8c2175d11514acaf9dfa3239c9175399e84e805af6e`  
		Last Modified: Tue, 13 Oct 2020 07:36:49 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1` - linux; mips64le

```console
$ docker pull memcached@sha256:17830abbb92982a00a2a744bef4361b22205ce49e383d5aa64ed87fe355b73e8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.7 MB (28735721 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a0f82dfc53875f944220d793d546db85f16426855ed9bcf92643bf446dc1b45`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 13 Oct 2020 01:09:50 GMT
ADD file:c2ad270f70511601478158cfe3854499c0b4887f049b78b66903412a811a428a in / 
# Tue, 13 Oct 2020 01:09:50 GMT
CMD ["bash"]
# Tue, 27 Oct 2020 17:50:08 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 27 Oct 2020 17:50:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Oct 2020 17:50:20 GMT
ENV MEMCACHED_VERSION=1.6.8
# Tue, 27 Oct 2020 17:50:21 GMT
ENV MEMCACHED_SHA1=8f3efd851efc5b822bd991b93d06a271b2fac052
# Wed, 28 Oct 2020 04:30:47 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 28 Oct 2020 04:30:47 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 28 Oct 2020 04:30:49 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 28 Oct 2020 04:30:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 28 Oct 2020 04:30:49 GMT
USER memcache
# Wed, 28 Oct 2020 04:30:50 GMT
EXPOSE 11211
# Wed, 28 Oct 2020 04:30:50 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:9bc77d453b2242ec513032b61e23061712b79c3ba0c60114232d743e5ab4e4fa`  
		Last Modified: Tue, 13 Oct 2020 01:16:41 GMT  
		Size: 25.8 MB (25762577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac83b13333509b8c185fea403b7631388624cc708325d7b746192c2d84d61c30`  
		Last Modified: Wed, 28 Oct 2020 04:31:10 GMT  
		Size: 5.0 KB (4986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b9c5336b4ffdcc16c62c61e285bced1eb40b5f252a0415b6393dc002e8f2eb8`  
		Last Modified: Wed, 28 Oct 2020 04:31:11 GMT  
		Size: 1.8 MB (1776027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7a4b59edf43de7ce3f3c4bbbd099c545e953b12913a9896ee2d266756346cb2`  
		Last Modified: Wed, 28 Oct 2020 04:31:11 GMT  
		Size: 1.2 MB (1191725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b84ace4a71dbe705a2cfc2673e134f77a1a04af75a13cbed6c072e6a6aeb1959`  
		Last Modified: Wed, 28 Oct 2020 04:31:10 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3552aec564382a3d8d830a584ee44b0d9ac151ab28e895c6882cc7c49867a7e3`  
		Last Modified: Wed, 28 Oct 2020 04:31:10 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1` - linux; ppc64le

```console
$ docker pull memcached@sha256:63c6b668e4938f19c9241f75a6b1531450c923fe79c562e6e6c50cfb6cec2a73
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.1 MB (34071374 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:98fbacd51c7d4950a68cd17040fbbf8b66e12570881a73a3090011d15078efb3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 13 Oct 2020 01:38:54 GMT
ADD file:9992867f855c9bed54df6d26f3d8076689aff8a51e808fefba7d3b66dab250e5 in / 
# Tue, 13 Oct 2020 01:38:59 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 10:01:29 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 13 Oct 2020 10:01:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Oct 2020 17:54:17 GMT
ENV MEMCACHED_VERSION=1.6.8
# Tue, 27 Oct 2020 17:54:22 GMT
ENV MEMCACHED_SHA1=8f3efd851efc5b822bd991b93d06a271b2fac052
# Tue, 27 Oct 2020 18:06:37 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 27 Oct 2020 18:06:40 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 27 Oct 2020 18:06:51 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 27 Oct 2020 18:06:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 27 Oct 2020 18:07:06 GMT
USER memcache
# Tue, 27 Oct 2020 18:07:11 GMT
EXPOSE 11211
# Tue, 27 Oct 2020 18:07:15 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:523555c6877c72cfcdec912b4d0053c298b1c97835efc7c6b0211585a06bd563`  
		Last Modified: Tue, 13 Oct 2020 01:50:10 GMT  
		Size: 30.5 MB (30517878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d6959d8bd92e8076720fb05de0ab3aa2972b4ed7c8aa85a1041abfbe2d8b56d`  
		Last Modified: Tue, 13 Oct 2020 10:16:27 GMT  
		Size: 5.0 KB (4984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bff6c7a70d59d80356167379e564384edc47a14264bcf7c91253653d4fa25071`  
		Last Modified: Tue, 13 Oct 2020 10:16:28 GMT  
		Size: 2.3 MB (2322777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56f5e94b0b94ab1f9c233ca3f5e3baa17b07f384cdd6fb8a1376bc4b3a1a22b9`  
		Last Modified: Tue, 27 Oct 2020 18:18:43 GMT  
		Size: 1.2 MB (1225330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7382b7d44dc710539db62bbeef153180b699ea1f735ad8f0eafb2999212cb26`  
		Last Modified: Tue, 27 Oct 2020 18:18:43 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98b83690c808dc9c5fc3ce938c34e970f6f109eeb8ad63515817b142c91cd0a5`  
		Last Modified: Tue, 27 Oct 2020 18:18:43 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1` - linux; s390x

```console
$ docker pull memcached@sha256:e11001edc21564af26a9f33a46dc3e1f6ee37e5571e60ce0d1c3fd3e1a9b629b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.8 MB (28789423 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5908f7dcace1ea65f0f60df58c4b3eb55a4d998703b4833ac64755eab9b67f6b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 13 Oct 2020 01:42:26 GMT
ADD file:f932c1176fdc9bf45ced816290f83e6231df3dffa3b7f8de1a3bb0adcff1588b in / 
# Tue, 13 Oct 2020 01:42:27 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 02:44:44 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 13 Oct 2020 02:44:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Oct 2020 17:50:18 GMT
ENV MEMCACHED_VERSION=1.6.8
# Tue, 27 Oct 2020 17:50:18 GMT
ENV MEMCACHED_SHA1=8f3efd851efc5b822bd991b93d06a271b2fac052
# Thu, 29 Oct 2020 23:59:00 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 29 Oct 2020 23:59:01 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 29 Oct 2020 23:59:03 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 29 Oct 2020 23:59:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 29 Oct 2020 23:59:04 GMT
USER memcache
# Thu, 29 Oct 2020 23:59:04 GMT
EXPOSE 11211
# Thu, 29 Oct 2020 23:59:04 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:2a4f9dc00d797c86c4ffce3b50bea9037c2eb4637f045ad3fd68cf151577b639`  
		Last Modified: Tue, 13 Oct 2020 01:45:45 GMT  
		Size: 25.7 MB (25707519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:307f2e192d445f2ae2ac5cf8ca173572473106ec1cedc16591ec31c2deed4602`  
		Last Modified: Tue, 13 Oct 2020 02:54:35 GMT  
		Size: 5.0 KB (5025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52a19707e552eac63bdd433244f456e992ca13a66f297d1fc326581c1d9e4f6d`  
		Last Modified: Tue, 13 Oct 2020 02:54:35 GMT  
		Size: 1.9 MB (1886119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:397803f765cfd9441284c39d53f61e465182b3e2955d49b556fcc2fd1ef4fcf5`  
		Last Modified: Fri, 30 Oct 2020 00:03:22 GMT  
		Size: 1.2 MB (1190355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19b4081264507735ea4c811cabeecb378f570f273f5a2cb577d8a49e42ea02b4`  
		Last Modified: Fri, 30 Oct 2020 00:03:22 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56c4bffa4499b85119f852d11d10aaca8ba7eb8488b9ff595b418f79a12ec769`  
		Last Modified: Fri, 30 Oct 2020 00:03:23 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:1.6`

```console
$ docker pull memcached@sha256:2c765a372d3e82565bc12bba67a0eb246baf536fd296ff6cb2e21c4036a62831
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
$ docker pull memcached@sha256:7be440dd3cc068fa2be188a7183890a8ff36e25e5a0c2edab25a4b6b460817c6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.5 MB (30493455 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:556880cb3d94c1509adc3eaf68dadf7d5e7325c5e5d2dcb86a8d0f8e0b4e4529`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 13 Oct 2020 01:39:05 GMT
ADD file:0dc53e7886c35bc21ae6c4f6cedda54d56ae9c9e9cd367678f1a72e68b3c43d4 in / 
# Tue, 13 Oct 2020 01:39:05 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 07:40:55 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 13 Oct 2020 07:41:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Oct 2020 17:51:22 GMT
ENV MEMCACHED_VERSION=1.6.8
# Tue, 27 Oct 2020 17:51:22 GMT
ENV MEMCACHED_SHA1=8f3efd851efc5b822bd991b93d06a271b2fac052
# Fri, 30 Oct 2020 01:59:43 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Fri, 30 Oct 2020 01:59:44 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 30 Oct 2020 01:59:44 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 30 Oct 2020 01:59:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 30 Oct 2020 01:59:45 GMT
USER memcache
# Fri, 30 Oct 2020 01:59:45 GMT
EXPOSE 11211
# Fri, 30 Oct 2020 01:59:45 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:bb79b6b2107fea8e8a47133a660b78e3a546998fcf0427be39ac9a0af4a97e90`  
		Last Modified: Tue, 13 Oct 2020 01:48:17 GMT  
		Size: 27.1 MB (27092228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5fbfe4d7c9b06eab9107d9ee46dbff27ea09707a40bdbdbea1d34078e65142a`  
		Last Modified: Tue, 13 Oct 2020 08:01:25 GMT  
		Size: 5.0 KB (4983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ed56f4a4fee8ed574be57dd51df7dc9f5bbdb041e9704be5a9ae0072a8a48b7`  
		Last Modified: Tue, 13 Oct 2020 08:01:26 GMT  
		Size: 2.2 MB (2196479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0186bf1dbc662c1e09f0a98b1182f4f1406a4b69b308ef63e0122450cfbca1b`  
		Last Modified: Fri, 30 Oct 2020 02:04:29 GMT  
		Size: 1.2 MB (1199359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f36909c1fe5329c92a34b3cde57aa972e7a53e582b7068c66d5e6af5e95bd86`  
		Last Modified: Fri, 30 Oct 2020 02:04:28 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e82197d1329427273caed560c08d7606a51afbb9bb34d2e4c0ed8bed4691cd3`  
		Last Modified: Fri, 30 Oct 2020 02:04:29 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6` - linux; arm variant v5

```console
$ docker pull memcached@sha256:281302b1776f2c06bbd2889f393368d96c44bcf61a889b7bb892b3b646629dfe
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.9 MB (27911064 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5cf13656486a2eb6df7a579ba2a4e613c12a4869f2bcd85097752033b87b1925`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 13 Oct 2020 01:52:17 GMT
ADD file:b71c0fa4957d6b65af37231a105f3d17cdbafe5c7d6c37b5843ebf619c608aaa in / 
# Tue, 13 Oct 2020 01:52:27 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 02:22:47 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 13 Oct 2020 02:23:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Oct 2020 17:48:42 GMT
ENV MEMCACHED_VERSION=1.6.8
# Tue, 27 Oct 2020 17:48:43 GMT
ENV MEMCACHED_SHA1=8f3efd851efc5b822bd991b93d06a271b2fac052
# Fri, 30 Oct 2020 01:54:09 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Fri, 30 Oct 2020 01:54:10 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 30 Oct 2020 01:54:12 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 30 Oct 2020 01:54:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 30 Oct 2020 01:54:14 GMT
USER memcache
# Fri, 30 Oct 2020 01:54:15 GMT
EXPOSE 11211
# Fri, 30 Oct 2020 01:54:16 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:f991c1e1ee2c48f16625b6b61310bf3c0616c0dbda4762019117e86fd29cf9ce`  
		Last Modified: Tue, 13 Oct 2020 02:01:27 GMT  
		Size: 24.8 MB (24835992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1b39a87be5bf0605d95ec4fc44790226547fdbcbad21c2add60885e9a1eabee`  
		Last Modified: Tue, 13 Oct 2020 02:34:18 GMT  
		Size: 4.9 KB (4897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d6238e630abdd7bca871de31aed93435c3e250ba2af1a0aaaabbec9d93d4452`  
		Last Modified: Tue, 13 Oct 2020 02:34:18 GMT  
		Size: 1.9 MB (1896831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a06241971793ab22b3a7ab4db8c18fc14c5b20227169c41d8bfce8fb6d67daa`  
		Last Modified: Fri, 30 Oct 2020 01:54:40 GMT  
		Size: 1.2 MB (1172937 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebc8ed09958e4b60fdf69ea8d28015f4cd3491968a22eced8fbf02720e2441bc`  
		Last Modified: Fri, 30 Oct 2020 01:54:40 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cb0a67800b722bbe27460d77886606a93383f456390e153365e2c38ae8cd602`  
		Last Modified: Fri, 30 Oct 2020 01:54:40 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6` - linux; arm variant v7

```console
$ docker pull memcached@sha256:3eb85207ec7eee29d5490f1f5b618eb232e57ad2654c929784518b7e42a589eb
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.7 MB (25660769 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b0e3423db692c288e1ce77ef4dccf8da40c46880e5bf18d42e6d8962016acce`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 13 Oct 2020 00:59:29 GMT
ADD file:e423f30ca19eb205a98de21b0545d0a764cfc4f832a9a9631542354d914d98d9 in / 
# Tue, 13 Oct 2020 00:59:31 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 04:26:19 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 13 Oct 2020 04:26:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Oct 2020 17:52:08 GMT
ENV MEMCACHED_VERSION=1.6.8
# Tue, 27 Oct 2020 17:52:09 GMT
ENV MEMCACHED_SHA1=8f3efd851efc5b822bd991b93d06a271b2fac052
# Tue, 27 Oct 2020 18:02:11 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 27 Oct 2020 18:02:12 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 27 Oct 2020 18:02:15 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 27 Oct 2020 18:02:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 27 Oct 2020 18:02:17 GMT
USER memcache
# Tue, 27 Oct 2020 18:02:18 GMT
EXPOSE 11211
# Tue, 27 Oct 2020 18:02:19 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:d6d8411ad43db0022fa0fce094cd2e8b1dd2f8a09d6880ed9beb6b4204867027`  
		Last Modified: Tue, 13 Oct 2020 01:08:28 GMT  
		Size: 22.7 MB (22699849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e36226ec0f789bddc127720ec631e27d952fb15b96b7848f3834950832523090`  
		Last Modified: Tue, 13 Oct 2020 04:37:29 GMT  
		Size: 4.9 KB (4895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46d8cf8973d9daad3ec5b519371371403ed2da2e65fa64c43d9122e8b8d602dd`  
		Last Modified: Tue, 13 Oct 2020 04:37:30 GMT  
		Size: 1.8 MB (1811537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc6baa5172a099a2af7b8031778e24fb072fc19291862933280eda0de2c1f873`  
		Last Modified: Tue, 27 Oct 2020 18:12:59 GMT  
		Size: 1.1 MB (1144080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79a4d1aadb5fa75c62ccfcb25624f53a840376fd2d43e3f2a37c4638437f36e5`  
		Last Modified: Tue, 27 Oct 2020 18:12:58 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61e633bd02bf4bd63bb51de860e7a23925d24c287faa53882423e30f3f283dff`  
		Last Modified: Tue, 27 Oct 2020 18:12:58 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:d3355e1e1ca991f55ddc098c2f4795182e1c74228ddce7128898604bf04db22c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.1 MB (29100019 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a0715facdf2c1c1981d8ef7df462d2498fea30e381c80f46f6c8a2a2852d50e4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 13 Oct 2020 01:41:09 GMT
ADD file:3488b1423094a75be5bb5956e9187827b8dd35d7a1f2b14081f8e74a1629e7d0 in / 
# Tue, 13 Oct 2020 01:41:11 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 08:18:46 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 13 Oct 2020 08:18:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Oct 2020 17:50:52 GMT
ENV MEMCACHED_VERSION=1.6.8
# Tue, 27 Oct 2020 17:50:53 GMT
ENV MEMCACHED_SHA1=8f3efd851efc5b822bd991b93d06a271b2fac052
# Tue, 27 Oct 2020 18:01:23 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 27 Oct 2020 18:01:24 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 27 Oct 2020 18:01:27 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 27 Oct 2020 18:01:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 27 Oct 2020 18:01:28 GMT
USER memcache
# Tue, 27 Oct 2020 18:01:29 GMT
EXPOSE 11211
# Tue, 27 Oct 2020 18:01:29 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:4e6164a63b7b4cf981546947e191644c122214975d40b51ede0536791ebec3d4`  
		Last Modified: Tue, 13 Oct 2020 01:48:17 GMT  
		Size: 25.8 MB (25849329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5f7daf8dcdb72260976fee433136d1d7b10f4488b985960ff0cc9680258a37e`  
		Last Modified: Tue, 13 Oct 2020 08:29:40 GMT  
		Size: 5.0 KB (5026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3afc9b2342454a24b6fc4247345875720b7dce42da90e83c7b9a4abf57ff9257`  
		Last Modified: Tue, 13 Oct 2020 08:29:41 GMT  
		Size: 2.1 MB (2074972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:603fd7cc62d57991fc13951bf2f7e62b72e84aa1f942d74260c20c67319f7881`  
		Last Modified: Tue, 27 Oct 2020 18:12:12 GMT  
		Size: 1.2 MB (1170284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1741db6c55c297ff2a3645680bd6edd02a39a5414eb5eeac865437cf557a1965`  
		Last Modified: Tue, 27 Oct 2020 18:12:11 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4449d89ef06347eb4b3344c8149350461269d63e8c8e80e622fc44c2ac2a6f29`  
		Last Modified: Tue, 27 Oct 2020 18:12:11 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6` - linux; 386

```console
$ docker pull memcached@sha256:2de59fa093416ca4d4f33c162b006bedc526d2026d762c0bc434318fe947d32c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.2 MB (31161101 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2743c23aca6cb3863b084988e69eaad5de3ebf0cb317f57121ea69ba42d110af`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 13 Oct 2020 01:41:03 GMT
ADD file:51108b89c70ce0773c897be520c84454660f38b84ba556da49c7fe77e5d52416 in / 
# Tue, 13 Oct 2020 01:41:03 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 07:16:07 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 13 Oct 2020 07:16:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 07:16:13 GMT
ENV MEMCACHED_VERSION=1.6.7
# Tue, 13 Oct 2020 07:16:13 GMT
ENV MEMCACHED_SHA1=49336bb0a4b7ad296422b08148581ed54edf32d0
# Tue, 13 Oct 2020 07:36:28 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 13 Oct 2020 07:36:28 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 13 Oct 2020 07:36:29 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 13 Oct 2020 07:36:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Oct 2020 07:36:29 GMT
USER memcache
# Tue, 13 Oct 2020 07:36:30 GMT
EXPOSE 11211
# Tue, 13 Oct 2020 07:36:30 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:97e4efec21eea92209464547d0f52a0f773c505cf4ea9d8090cef667bde145b8`  
		Last Modified: Tue, 13 Oct 2020 01:48:54 GMT  
		Size: 27.8 MB (27750243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1e2733549a0a03eff9da2ad1035504ef29480a7fed2edb9ac19fcc6605081ec`  
		Last Modified: Tue, 13 Oct 2020 07:36:49 GMT  
		Size: 4.9 KB (4896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4434320f582eaf5fce7418fb99c35a07380e61385ed8d9ec07d383d46e426d06`  
		Last Modified: Tue, 13 Oct 2020 07:36:51 GMT  
		Size: 2.2 MB (2208112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0faf39e12c14d25e5dc802ddbe8f0068b4cc492ebf1e078998ddf38205c836dd`  
		Last Modified: Tue, 13 Oct 2020 07:36:49 GMT  
		Size: 1.2 MB (1197441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b95b4020f31dffe1467a69cfe85d22f7c6fa9d76da3678c72c99f23254899fb`  
		Last Modified: Tue, 13 Oct 2020 07:36:49 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5193dc6218dcc26a610b8c2175d11514acaf9dfa3239c9175399e84e805af6e`  
		Last Modified: Tue, 13 Oct 2020 07:36:49 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6` - linux; mips64le

```console
$ docker pull memcached@sha256:17830abbb92982a00a2a744bef4361b22205ce49e383d5aa64ed87fe355b73e8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.7 MB (28735721 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a0f82dfc53875f944220d793d546db85f16426855ed9bcf92643bf446dc1b45`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 13 Oct 2020 01:09:50 GMT
ADD file:c2ad270f70511601478158cfe3854499c0b4887f049b78b66903412a811a428a in / 
# Tue, 13 Oct 2020 01:09:50 GMT
CMD ["bash"]
# Tue, 27 Oct 2020 17:50:08 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 27 Oct 2020 17:50:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Oct 2020 17:50:20 GMT
ENV MEMCACHED_VERSION=1.6.8
# Tue, 27 Oct 2020 17:50:21 GMT
ENV MEMCACHED_SHA1=8f3efd851efc5b822bd991b93d06a271b2fac052
# Wed, 28 Oct 2020 04:30:47 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 28 Oct 2020 04:30:47 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 28 Oct 2020 04:30:49 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 28 Oct 2020 04:30:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 28 Oct 2020 04:30:49 GMT
USER memcache
# Wed, 28 Oct 2020 04:30:50 GMT
EXPOSE 11211
# Wed, 28 Oct 2020 04:30:50 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:9bc77d453b2242ec513032b61e23061712b79c3ba0c60114232d743e5ab4e4fa`  
		Last Modified: Tue, 13 Oct 2020 01:16:41 GMT  
		Size: 25.8 MB (25762577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac83b13333509b8c185fea403b7631388624cc708325d7b746192c2d84d61c30`  
		Last Modified: Wed, 28 Oct 2020 04:31:10 GMT  
		Size: 5.0 KB (4986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b9c5336b4ffdcc16c62c61e285bced1eb40b5f252a0415b6393dc002e8f2eb8`  
		Last Modified: Wed, 28 Oct 2020 04:31:11 GMT  
		Size: 1.8 MB (1776027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7a4b59edf43de7ce3f3c4bbbd099c545e953b12913a9896ee2d266756346cb2`  
		Last Modified: Wed, 28 Oct 2020 04:31:11 GMT  
		Size: 1.2 MB (1191725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b84ace4a71dbe705a2cfc2673e134f77a1a04af75a13cbed6c072e6a6aeb1959`  
		Last Modified: Wed, 28 Oct 2020 04:31:10 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3552aec564382a3d8d830a584ee44b0d9ac151ab28e895c6882cc7c49867a7e3`  
		Last Modified: Wed, 28 Oct 2020 04:31:10 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6` - linux; ppc64le

```console
$ docker pull memcached@sha256:63c6b668e4938f19c9241f75a6b1531450c923fe79c562e6e6c50cfb6cec2a73
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.1 MB (34071374 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:98fbacd51c7d4950a68cd17040fbbf8b66e12570881a73a3090011d15078efb3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 13 Oct 2020 01:38:54 GMT
ADD file:9992867f855c9bed54df6d26f3d8076689aff8a51e808fefba7d3b66dab250e5 in / 
# Tue, 13 Oct 2020 01:38:59 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 10:01:29 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 13 Oct 2020 10:01:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Oct 2020 17:54:17 GMT
ENV MEMCACHED_VERSION=1.6.8
# Tue, 27 Oct 2020 17:54:22 GMT
ENV MEMCACHED_SHA1=8f3efd851efc5b822bd991b93d06a271b2fac052
# Tue, 27 Oct 2020 18:06:37 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 27 Oct 2020 18:06:40 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 27 Oct 2020 18:06:51 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 27 Oct 2020 18:06:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 27 Oct 2020 18:07:06 GMT
USER memcache
# Tue, 27 Oct 2020 18:07:11 GMT
EXPOSE 11211
# Tue, 27 Oct 2020 18:07:15 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:523555c6877c72cfcdec912b4d0053c298b1c97835efc7c6b0211585a06bd563`  
		Last Modified: Tue, 13 Oct 2020 01:50:10 GMT  
		Size: 30.5 MB (30517878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d6959d8bd92e8076720fb05de0ab3aa2972b4ed7c8aa85a1041abfbe2d8b56d`  
		Last Modified: Tue, 13 Oct 2020 10:16:27 GMT  
		Size: 5.0 KB (4984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bff6c7a70d59d80356167379e564384edc47a14264bcf7c91253653d4fa25071`  
		Last Modified: Tue, 13 Oct 2020 10:16:28 GMT  
		Size: 2.3 MB (2322777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56f5e94b0b94ab1f9c233ca3f5e3baa17b07f384cdd6fb8a1376bc4b3a1a22b9`  
		Last Modified: Tue, 27 Oct 2020 18:18:43 GMT  
		Size: 1.2 MB (1225330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7382b7d44dc710539db62bbeef153180b699ea1f735ad8f0eafb2999212cb26`  
		Last Modified: Tue, 27 Oct 2020 18:18:43 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98b83690c808dc9c5fc3ce938c34e970f6f109eeb8ad63515817b142c91cd0a5`  
		Last Modified: Tue, 27 Oct 2020 18:18:43 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6` - linux; s390x

```console
$ docker pull memcached@sha256:e11001edc21564af26a9f33a46dc3e1f6ee37e5571e60ce0d1c3fd3e1a9b629b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.8 MB (28789423 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5908f7dcace1ea65f0f60df58c4b3eb55a4d998703b4833ac64755eab9b67f6b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 13 Oct 2020 01:42:26 GMT
ADD file:f932c1176fdc9bf45ced816290f83e6231df3dffa3b7f8de1a3bb0adcff1588b in / 
# Tue, 13 Oct 2020 01:42:27 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 02:44:44 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 13 Oct 2020 02:44:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Oct 2020 17:50:18 GMT
ENV MEMCACHED_VERSION=1.6.8
# Tue, 27 Oct 2020 17:50:18 GMT
ENV MEMCACHED_SHA1=8f3efd851efc5b822bd991b93d06a271b2fac052
# Thu, 29 Oct 2020 23:59:00 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 29 Oct 2020 23:59:01 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 29 Oct 2020 23:59:03 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 29 Oct 2020 23:59:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 29 Oct 2020 23:59:04 GMT
USER memcache
# Thu, 29 Oct 2020 23:59:04 GMT
EXPOSE 11211
# Thu, 29 Oct 2020 23:59:04 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:2a4f9dc00d797c86c4ffce3b50bea9037c2eb4637f045ad3fd68cf151577b639`  
		Last Modified: Tue, 13 Oct 2020 01:45:45 GMT  
		Size: 25.7 MB (25707519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:307f2e192d445f2ae2ac5cf8ca173572473106ec1cedc16591ec31c2deed4602`  
		Last Modified: Tue, 13 Oct 2020 02:54:35 GMT  
		Size: 5.0 KB (5025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52a19707e552eac63bdd433244f456e992ca13a66f297d1fc326581c1d9e4f6d`  
		Last Modified: Tue, 13 Oct 2020 02:54:35 GMT  
		Size: 1.9 MB (1886119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:397803f765cfd9441284c39d53f61e465182b3e2955d49b556fcc2fd1ef4fcf5`  
		Last Modified: Fri, 30 Oct 2020 00:03:22 GMT  
		Size: 1.2 MB (1190355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19b4081264507735ea4c811cabeecb378f570f273f5a2cb577d8a49e42ea02b4`  
		Last Modified: Fri, 30 Oct 2020 00:03:22 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56c4bffa4499b85119f852d11d10aaca8ba7eb8488b9ff595b418f79a12ec769`  
		Last Modified: Fri, 30 Oct 2020 00:03:23 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:1.6.8`

```console
$ docker pull memcached@sha256:5218a165ca8c591fbfe5d80f35377b9d7bff21cfa67f01950b1972525b3ebecf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; s390x

### `memcached:1.6.8` - linux; amd64

```console
$ docker pull memcached@sha256:7be440dd3cc068fa2be188a7183890a8ff36e25e5a0c2edab25a4b6b460817c6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.5 MB (30493455 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:556880cb3d94c1509adc3eaf68dadf7d5e7325c5e5d2dcb86a8d0f8e0b4e4529`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 13 Oct 2020 01:39:05 GMT
ADD file:0dc53e7886c35bc21ae6c4f6cedda54d56ae9c9e9cd367678f1a72e68b3c43d4 in / 
# Tue, 13 Oct 2020 01:39:05 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 07:40:55 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 13 Oct 2020 07:41:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Oct 2020 17:51:22 GMT
ENV MEMCACHED_VERSION=1.6.8
# Tue, 27 Oct 2020 17:51:22 GMT
ENV MEMCACHED_SHA1=8f3efd851efc5b822bd991b93d06a271b2fac052
# Fri, 30 Oct 2020 01:59:43 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Fri, 30 Oct 2020 01:59:44 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 30 Oct 2020 01:59:44 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 30 Oct 2020 01:59:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 30 Oct 2020 01:59:45 GMT
USER memcache
# Fri, 30 Oct 2020 01:59:45 GMT
EXPOSE 11211
# Fri, 30 Oct 2020 01:59:45 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:bb79b6b2107fea8e8a47133a660b78e3a546998fcf0427be39ac9a0af4a97e90`  
		Last Modified: Tue, 13 Oct 2020 01:48:17 GMT  
		Size: 27.1 MB (27092228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5fbfe4d7c9b06eab9107d9ee46dbff27ea09707a40bdbdbea1d34078e65142a`  
		Last Modified: Tue, 13 Oct 2020 08:01:25 GMT  
		Size: 5.0 KB (4983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ed56f4a4fee8ed574be57dd51df7dc9f5bbdb041e9704be5a9ae0072a8a48b7`  
		Last Modified: Tue, 13 Oct 2020 08:01:26 GMT  
		Size: 2.2 MB (2196479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0186bf1dbc662c1e09f0a98b1182f4f1406a4b69b308ef63e0122450cfbca1b`  
		Last Modified: Fri, 30 Oct 2020 02:04:29 GMT  
		Size: 1.2 MB (1199359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f36909c1fe5329c92a34b3cde57aa972e7a53e582b7068c66d5e6af5e95bd86`  
		Last Modified: Fri, 30 Oct 2020 02:04:28 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e82197d1329427273caed560c08d7606a51afbb9bb34d2e4c0ed8bed4691cd3`  
		Last Modified: Fri, 30 Oct 2020 02:04:29 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.8` - linux; arm variant v5

```console
$ docker pull memcached@sha256:281302b1776f2c06bbd2889f393368d96c44bcf61a889b7bb892b3b646629dfe
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.9 MB (27911064 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5cf13656486a2eb6df7a579ba2a4e613c12a4869f2bcd85097752033b87b1925`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 13 Oct 2020 01:52:17 GMT
ADD file:b71c0fa4957d6b65af37231a105f3d17cdbafe5c7d6c37b5843ebf619c608aaa in / 
# Tue, 13 Oct 2020 01:52:27 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 02:22:47 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 13 Oct 2020 02:23:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Oct 2020 17:48:42 GMT
ENV MEMCACHED_VERSION=1.6.8
# Tue, 27 Oct 2020 17:48:43 GMT
ENV MEMCACHED_SHA1=8f3efd851efc5b822bd991b93d06a271b2fac052
# Fri, 30 Oct 2020 01:54:09 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Fri, 30 Oct 2020 01:54:10 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 30 Oct 2020 01:54:12 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 30 Oct 2020 01:54:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 30 Oct 2020 01:54:14 GMT
USER memcache
# Fri, 30 Oct 2020 01:54:15 GMT
EXPOSE 11211
# Fri, 30 Oct 2020 01:54:16 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:f991c1e1ee2c48f16625b6b61310bf3c0616c0dbda4762019117e86fd29cf9ce`  
		Last Modified: Tue, 13 Oct 2020 02:01:27 GMT  
		Size: 24.8 MB (24835992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1b39a87be5bf0605d95ec4fc44790226547fdbcbad21c2add60885e9a1eabee`  
		Last Modified: Tue, 13 Oct 2020 02:34:18 GMT  
		Size: 4.9 KB (4897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d6238e630abdd7bca871de31aed93435c3e250ba2af1a0aaaabbec9d93d4452`  
		Last Modified: Tue, 13 Oct 2020 02:34:18 GMT  
		Size: 1.9 MB (1896831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a06241971793ab22b3a7ab4db8c18fc14c5b20227169c41d8bfce8fb6d67daa`  
		Last Modified: Fri, 30 Oct 2020 01:54:40 GMT  
		Size: 1.2 MB (1172937 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebc8ed09958e4b60fdf69ea8d28015f4cd3491968a22eced8fbf02720e2441bc`  
		Last Modified: Fri, 30 Oct 2020 01:54:40 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cb0a67800b722bbe27460d77886606a93383f456390e153365e2c38ae8cd602`  
		Last Modified: Fri, 30 Oct 2020 01:54:40 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.8` - linux; arm variant v7

```console
$ docker pull memcached@sha256:3eb85207ec7eee29d5490f1f5b618eb232e57ad2654c929784518b7e42a589eb
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.7 MB (25660769 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b0e3423db692c288e1ce77ef4dccf8da40c46880e5bf18d42e6d8962016acce`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 13 Oct 2020 00:59:29 GMT
ADD file:e423f30ca19eb205a98de21b0545d0a764cfc4f832a9a9631542354d914d98d9 in / 
# Tue, 13 Oct 2020 00:59:31 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 04:26:19 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 13 Oct 2020 04:26:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Oct 2020 17:52:08 GMT
ENV MEMCACHED_VERSION=1.6.8
# Tue, 27 Oct 2020 17:52:09 GMT
ENV MEMCACHED_SHA1=8f3efd851efc5b822bd991b93d06a271b2fac052
# Tue, 27 Oct 2020 18:02:11 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 27 Oct 2020 18:02:12 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 27 Oct 2020 18:02:15 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 27 Oct 2020 18:02:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 27 Oct 2020 18:02:17 GMT
USER memcache
# Tue, 27 Oct 2020 18:02:18 GMT
EXPOSE 11211
# Tue, 27 Oct 2020 18:02:19 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:d6d8411ad43db0022fa0fce094cd2e8b1dd2f8a09d6880ed9beb6b4204867027`  
		Last Modified: Tue, 13 Oct 2020 01:08:28 GMT  
		Size: 22.7 MB (22699849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e36226ec0f789bddc127720ec631e27d952fb15b96b7848f3834950832523090`  
		Last Modified: Tue, 13 Oct 2020 04:37:29 GMT  
		Size: 4.9 KB (4895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46d8cf8973d9daad3ec5b519371371403ed2da2e65fa64c43d9122e8b8d602dd`  
		Last Modified: Tue, 13 Oct 2020 04:37:30 GMT  
		Size: 1.8 MB (1811537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc6baa5172a099a2af7b8031778e24fb072fc19291862933280eda0de2c1f873`  
		Last Modified: Tue, 27 Oct 2020 18:12:59 GMT  
		Size: 1.1 MB (1144080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79a4d1aadb5fa75c62ccfcb25624f53a840376fd2d43e3f2a37c4638437f36e5`  
		Last Modified: Tue, 27 Oct 2020 18:12:58 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61e633bd02bf4bd63bb51de860e7a23925d24c287faa53882423e30f3f283dff`  
		Last Modified: Tue, 27 Oct 2020 18:12:58 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.8` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:d3355e1e1ca991f55ddc098c2f4795182e1c74228ddce7128898604bf04db22c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.1 MB (29100019 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a0715facdf2c1c1981d8ef7df462d2498fea30e381c80f46f6c8a2a2852d50e4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 13 Oct 2020 01:41:09 GMT
ADD file:3488b1423094a75be5bb5956e9187827b8dd35d7a1f2b14081f8e74a1629e7d0 in / 
# Tue, 13 Oct 2020 01:41:11 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 08:18:46 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 13 Oct 2020 08:18:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Oct 2020 17:50:52 GMT
ENV MEMCACHED_VERSION=1.6.8
# Tue, 27 Oct 2020 17:50:53 GMT
ENV MEMCACHED_SHA1=8f3efd851efc5b822bd991b93d06a271b2fac052
# Tue, 27 Oct 2020 18:01:23 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 27 Oct 2020 18:01:24 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 27 Oct 2020 18:01:27 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 27 Oct 2020 18:01:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 27 Oct 2020 18:01:28 GMT
USER memcache
# Tue, 27 Oct 2020 18:01:29 GMT
EXPOSE 11211
# Tue, 27 Oct 2020 18:01:29 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:4e6164a63b7b4cf981546947e191644c122214975d40b51ede0536791ebec3d4`  
		Last Modified: Tue, 13 Oct 2020 01:48:17 GMT  
		Size: 25.8 MB (25849329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5f7daf8dcdb72260976fee433136d1d7b10f4488b985960ff0cc9680258a37e`  
		Last Modified: Tue, 13 Oct 2020 08:29:40 GMT  
		Size: 5.0 KB (5026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3afc9b2342454a24b6fc4247345875720b7dce42da90e83c7b9a4abf57ff9257`  
		Last Modified: Tue, 13 Oct 2020 08:29:41 GMT  
		Size: 2.1 MB (2074972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:603fd7cc62d57991fc13951bf2f7e62b72e84aa1f942d74260c20c67319f7881`  
		Last Modified: Tue, 27 Oct 2020 18:12:12 GMT  
		Size: 1.2 MB (1170284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1741db6c55c297ff2a3645680bd6edd02a39a5414eb5eeac865437cf557a1965`  
		Last Modified: Tue, 27 Oct 2020 18:12:11 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4449d89ef06347eb4b3344c8149350461269d63e8c8e80e622fc44c2ac2a6f29`  
		Last Modified: Tue, 27 Oct 2020 18:12:11 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.8` - linux; mips64le

```console
$ docker pull memcached@sha256:17830abbb92982a00a2a744bef4361b22205ce49e383d5aa64ed87fe355b73e8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.7 MB (28735721 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a0f82dfc53875f944220d793d546db85f16426855ed9bcf92643bf446dc1b45`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 13 Oct 2020 01:09:50 GMT
ADD file:c2ad270f70511601478158cfe3854499c0b4887f049b78b66903412a811a428a in / 
# Tue, 13 Oct 2020 01:09:50 GMT
CMD ["bash"]
# Tue, 27 Oct 2020 17:50:08 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 27 Oct 2020 17:50:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Oct 2020 17:50:20 GMT
ENV MEMCACHED_VERSION=1.6.8
# Tue, 27 Oct 2020 17:50:21 GMT
ENV MEMCACHED_SHA1=8f3efd851efc5b822bd991b93d06a271b2fac052
# Wed, 28 Oct 2020 04:30:47 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 28 Oct 2020 04:30:47 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 28 Oct 2020 04:30:49 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 28 Oct 2020 04:30:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 28 Oct 2020 04:30:49 GMT
USER memcache
# Wed, 28 Oct 2020 04:30:50 GMT
EXPOSE 11211
# Wed, 28 Oct 2020 04:30:50 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:9bc77d453b2242ec513032b61e23061712b79c3ba0c60114232d743e5ab4e4fa`  
		Last Modified: Tue, 13 Oct 2020 01:16:41 GMT  
		Size: 25.8 MB (25762577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac83b13333509b8c185fea403b7631388624cc708325d7b746192c2d84d61c30`  
		Last Modified: Wed, 28 Oct 2020 04:31:10 GMT  
		Size: 5.0 KB (4986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b9c5336b4ffdcc16c62c61e285bced1eb40b5f252a0415b6393dc002e8f2eb8`  
		Last Modified: Wed, 28 Oct 2020 04:31:11 GMT  
		Size: 1.8 MB (1776027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7a4b59edf43de7ce3f3c4bbbd099c545e953b12913a9896ee2d266756346cb2`  
		Last Modified: Wed, 28 Oct 2020 04:31:11 GMT  
		Size: 1.2 MB (1191725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b84ace4a71dbe705a2cfc2673e134f77a1a04af75a13cbed6c072e6a6aeb1959`  
		Last Modified: Wed, 28 Oct 2020 04:31:10 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3552aec564382a3d8d830a584ee44b0d9ac151ab28e895c6882cc7c49867a7e3`  
		Last Modified: Wed, 28 Oct 2020 04:31:10 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.8` - linux; ppc64le

```console
$ docker pull memcached@sha256:63c6b668e4938f19c9241f75a6b1531450c923fe79c562e6e6c50cfb6cec2a73
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.1 MB (34071374 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:98fbacd51c7d4950a68cd17040fbbf8b66e12570881a73a3090011d15078efb3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 13 Oct 2020 01:38:54 GMT
ADD file:9992867f855c9bed54df6d26f3d8076689aff8a51e808fefba7d3b66dab250e5 in / 
# Tue, 13 Oct 2020 01:38:59 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 10:01:29 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 13 Oct 2020 10:01:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Oct 2020 17:54:17 GMT
ENV MEMCACHED_VERSION=1.6.8
# Tue, 27 Oct 2020 17:54:22 GMT
ENV MEMCACHED_SHA1=8f3efd851efc5b822bd991b93d06a271b2fac052
# Tue, 27 Oct 2020 18:06:37 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 27 Oct 2020 18:06:40 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 27 Oct 2020 18:06:51 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 27 Oct 2020 18:06:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 27 Oct 2020 18:07:06 GMT
USER memcache
# Tue, 27 Oct 2020 18:07:11 GMT
EXPOSE 11211
# Tue, 27 Oct 2020 18:07:15 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:523555c6877c72cfcdec912b4d0053c298b1c97835efc7c6b0211585a06bd563`  
		Last Modified: Tue, 13 Oct 2020 01:50:10 GMT  
		Size: 30.5 MB (30517878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d6959d8bd92e8076720fb05de0ab3aa2972b4ed7c8aa85a1041abfbe2d8b56d`  
		Last Modified: Tue, 13 Oct 2020 10:16:27 GMT  
		Size: 5.0 KB (4984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bff6c7a70d59d80356167379e564384edc47a14264bcf7c91253653d4fa25071`  
		Last Modified: Tue, 13 Oct 2020 10:16:28 GMT  
		Size: 2.3 MB (2322777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56f5e94b0b94ab1f9c233ca3f5e3baa17b07f384cdd6fb8a1376bc4b3a1a22b9`  
		Last Modified: Tue, 27 Oct 2020 18:18:43 GMT  
		Size: 1.2 MB (1225330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7382b7d44dc710539db62bbeef153180b699ea1f735ad8f0eafb2999212cb26`  
		Last Modified: Tue, 27 Oct 2020 18:18:43 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98b83690c808dc9c5fc3ce938c34e970f6f109eeb8ad63515817b142c91cd0a5`  
		Last Modified: Tue, 27 Oct 2020 18:18:43 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.8` - linux; s390x

```console
$ docker pull memcached@sha256:e11001edc21564af26a9f33a46dc3e1f6ee37e5571e60ce0d1c3fd3e1a9b629b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.8 MB (28789423 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5908f7dcace1ea65f0f60df58c4b3eb55a4d998703b4833ac64755eab9b67f6b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 13 Oct 2020 01:42:26 GMT
ADD file:f932c1176fdc9bf45ced816290f83e6231df3dffa3b7f8de1a3bb0adcff1588b in / 
# Tue, 13 Oct 2020 01:42:27 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 02:44:44 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 13 Oct 2020 02:44:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Oct 2020 17:50:18 GMT
ENV MEMCACHED_VERSION=1.6.8
# Tue, 27 Oct 2020 17:50:18 GMT
ENV MEMCACHED_SHA1=8f3efd851efc5b822bd991b93d06a271b2fac052
# Thu, 29 Oct 2020 23:59:00 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 29 Oct 2020 23:59:01 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 29 Oct 2020 23:59:03 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 29 Oct 2020 23:59:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 29 Oct 2020 23:59:04 GMT
USER memcache
# Thu, 29 Oct 2020 23:59:04 GMT
EXPOSE 11211
# Thu, 29 Oct 2020 23:59:04 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:2a4f9dc00d797c86c4ffce3b50bea9037c2eb4637f045ad3fd68cf151577b639`  
		Last Modified: Tue, 13 Oct 2020 01:45:45 GMT  
		Size: 25.7 MB (25707519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:307f2e192d445f2ae2ac5cf8ca173572473106ec1cedc16591ec31c2deed4602`  
		Last Modified: Tue, 13 Oct 2020 02:54:35 GMT  
		Size: 5.0 KB (5025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52a19707e552eac63bdd433244f456e992ca13a66f297d1fc326581c1d9e4f6d`  
		Last Modified: Tue, 13 Oct 2020 02:54:35 GMT  
		Size: 1.9 MB (1886119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:397803f765cfd9441284c39d53f61e465182b3e2955d49b556fcc2fd1ef4fcf5`  
		Last Modified: Fri, 30 Oct 2020 00:03:22 GMT  
		Size: 1.2 MB (1190355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19b4081264507735ea4c811cabeecb378f570f273f5a2cb577d8a49e42ea02b4`  
		Last Modified: Fri, 30 Oct 2020 00:03:22 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56c4bffa4499b85119f852d11d10aaca8ba7eb8488b9ff595b418f79a12ec769`  
		Last Modified: Fri, 30 Oct 2020 00:03:23 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:1.6.8-alpine`

```console
$ docker pull memcached@sha256:8e31ec2228adcec5846663e069ea192344c4caa11fb96615404eaede343c90ec
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

### `memcached:1.6.8-alpine` - linux; amd64

```console
$ docker pull memcached@sha256:71e3a793caad04dd57811a2aafa94612569c5d087bf1c5c871b603abdd1be630
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4495478 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e67bbd9b6e6573874b2e4563d209c0deadd89685497a754f5e47f9b373adca4d`
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
# Tue, 27 Oct 2020 18:01:01 GMT
ENV MEMCACHED_VERSION=1.6.8
# Tue, 27 Oct 2020 18:01:01 GMT
ENV MEMCACHED_SHA1=8f3efd851efc5b822bd991b93d06a271b2fac052
# Fri, 30 Oct 2020 02:04:11 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		dpkg-dev dpkg 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		tar 		wget 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Fri, 30 Oct 2020 02:04:11 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 30 Oct 2020 02:04:12 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 30 Oct 2020 02:04:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 30 Oct 2020 02:04:12 GMT
USER memcache
# Fri, 30 Oct 2020 02:04:13 GMT
EXPOSE 11211
# Fri, 30 Oct 2020 02:04:13 GMT
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
	-	`sha256:7303d373d89cbdae16f208a75a727b5ddb7f4e2861d02d11d382a9d42fc97cc3`  
		Last Modified: Fri, 30 Oct 2020 02:04:36 GMT  
		Size: 1.7 MB (1681682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ddff243a56604d00107678a49b86150ee4e22c6a0938bd3fbe9ce8a8dee2898`  
		Last Modified: Fri, 30 Oct 2020 02:04:36 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa411362f695820b3836affc1e76d4f6a470257081d90f0e7421231baca366cc`  
		Last Modified: Fri, 30 Oct 2020 02:04:36 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.8-alpine` - linux; arm variant v6

```console
$ docker pull memcached@sha256:7e31d9335251211f92511ec71fb1461f200d1ede4b9e3729b28a209debd4d9f8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.3 MB (4262175 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a88cc287311223e211ffb39fb1cfcc527e16f0b38a477ffecfae69a75f28947`
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
# Tue, 27 Oct 2020 17:50:52 GMT
ENV MEMCACHED_VERSION=1.6.8
# Tue, 27 Oct 2020 17:50:53 GMT
ENV MEMCACHED_SHA1=8f3efd851efc5b822bd991b93d06a271b2fac052
# Fri, 30 Oct 2020 00:28:33 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		dpkg-dev dpkg 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		tar 		wget 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Fri, 30 Oct 2020 00:28:34 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 30 Oct 2020 00:28:37 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 30 Oct 2020 00:28:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 30 Oct 2020 00:28:39 GMT
USER memcache
# Fri, 30 Oct 2020 00:28:40 GMT
EXPOSE 11211
# Fri, 30 Oct 2020 00:28:41 GMT
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
	-	`sha256:869dfda4a629dff09bee12e77e816513663c31197b3369a7a2df12c3d24f9734`  
		Last Modified: Fri, 30 Oct 2020 00:29:05 GMT  
		Size: 1.6 MB (1643699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc13f7ef8df67c31bd40e2ddf5678b3ed840e1901690a0ba39b9ad84e1493c7e`  
		Last Modified: Fri, 30 Oct 2020 00:29:04 GMT  
		Size: 282.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:014ddfe019df6e2dae30fd8acf752c68d3df2f3f3b7f1a3b274ab72f60e684d8`  
		Last Modified: Fri, 30 Oct 2020 00:29:06 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.8-alpine` - linux; arm variant v7

```console
$ docker pull memcached@sha256:cb005e7b4e652cbce090d5772626c2127b55f9bc8f282235a32c8f9f29a2af98
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.0 MB (3952565 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d49f3088ea875b790d47e63bc80ea9172ec25351e126f76d8090e1c95d8bb69c`
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
# Tue, 27 Oct 2020 18:02:39 GMT
ENV MEMCACHED_VERSION=1.6.8
# Tue, 27 Oct 2020 18:02:40 GMT
ENV MEMCACHED_SHA1=8f3efd851efc5b822bd991b93d06a271b2fac052
# Tue, 27 Oct 2020 18:12:34 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		dpkg-dev dpkg 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		tar 		wget 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& make test 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 27 Oct 2020 18:12:35 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 27 Oct 2020 18:12:37 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 27 Oct 2020 18:12:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 27 Oct 2020 18:12:38 GMT
USER memcache
# Tue, 27 Oct 2020 18:12:38 GMT
EXPOSE 11211
# Tue, 27 Oct 2020 18:12:39 GMT
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
	-	`sha256:6d24c3c688587cb0b6aa29bf3cb9be166d022bb6d46ee86740f03d8a204fadf6`  
		Last Modified: Tue, 27 Oct 2020 18:13:08 GMT  
		Size: 1.5 MB (1531399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:203f79e6fe3b93db04f06454f4da7c8dac400de74c97964885e0b94d5e21a69b`  
		Last Modified: Tue, 27 Oct 2020 18:13:08 GMT  
		Size: 283.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af3e72612c1e12f068d1f5c19f1c9c3eea8bb8fd7afed58892475c42e3ee1e3e`  
		Last Modified: Tue, 27 Oct 2020 18:13:08 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.8-alpine` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:1ce1d86238db5d088348cce464a468ac50b26d8aa01fe16c950f278e0cb63d0f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.4 MB (4411120 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:81f941fc95252e6747f1bab7de59cfbb48b440191a01117b53a45861f1902815`
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
# Tue, 27 Oct 2020 18:01:38 GMT
ENV MEMCACHED_VERSION=1.6.8
# Tue, 27 Oct 2020 18:01:38 GMT
ENV MEMCACHED_SHA1=8f3efd851efc5b822bd991b93d06a271b2fac052
# Tue, 27 Oct 2020 18:11:45 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		dpkg-dev dpkg 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		tar 		wget 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& make test 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 27 Oct 2020 18:11:48 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 27 Oct 2020 18:11:50 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 27 Oct 2020 18:11:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 27 Oct 2020 18:11:51 GMT
USER memcache
# Tue, 27 Oct 2020 18:11:52 GMT
EXPOSE 11211
# Tue, 27 Oct 2020 18:11:52 GMT
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
	-	`sha256:67fea89495771922e87061bccf414240a074727d95ece99c45ea8d027fa2b701`  
		Last Modified: Tue, 27 Oct 2020 18:12:21 GMT  
		Size: 1.7 MB (1687219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4745a66b526dd3a41a93a5e02a76afb529118e84b7198e5c793adbab0315e66c`  
		Last Modified: Tue, 27 Oct 2020 18:12:21 GMT  
		Size: 283.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8c659e4bd9d8b6c000e0d82cd2899b5ae3fec40641fbb4c67054d27cc338faf`  
		Last Modified: Tue, 27 Oct 2020 18:12:20 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.8-alpine` - linux; 386

```console
$ docker pull memcached@sha256:c89024e028c1823a713a0ae72e19a38b6fdc372377ec72de6cea84d48a3f095a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4585342 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:41421a77b44c877cc6bb4aa0a29a05da47ba69f789391845b0f383a620c16fba`
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
# Tue, 27 Oct 2020 18:20:12 GMT
ENV MEMCACHED_VERSION=1.6.8
# Tue, 27 Oct 2020 18:20:12 GMT
ENV MEMCACHED_SHA1=8f3efd851efc5b822bd991b93d06a271b2fac052
# Tue, 27 Oct 2020 23:55:05 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		dpkg-dev dpkg 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		tar 		wget 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& make test 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 27 Oct 2020 23:55:05 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 27 Oct 2020 23:55:06 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 27 Oct 2020 23:55:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 27 Oct 2020 23:55:07 GMT
USER memcache
# Tue, 27 Oct 2020 23:55:07 GMT
EXPOSE 11211
# Tue, 27 Oct 2020 23:55:07 GMT
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
	-	`sha256:09d187261acd1699a7536448083deb0fe4bd93125a0930418da3c8332bd6a52d`  
		Last Modified: Tue, 27 Oct 2020 23:55:27 GMT  
		Size: 1.8 MB (1775973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e7e368f966f2b955ec8c4aef5b440bf537f96f1b0b2275fb2981fe931c28d8d`  
		Last Modified: Tue, 27 Oct 2020 23:55:26 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8571d349dd3ca7fc4f303200d3e416fcfc88a390fa66344ef1d660d77ef9975`  
		Last Modified: Tue, 27 Oct 2020 23:55:27 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.8-alpine` - linux; ppc64le

```console
$ docker pull memcached@sha256:b2bcc724008b7866f1fb699f0308392ffdd8fdc3e5baf83c3e0f8c70b90d0eb9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4563777 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:29785833c149a374d3c03717ab9da503269016621376c89b78b7d6a2f3cd3a77`
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
# Tue, 27 Oct 2020 18:17:46 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		dpkg-dev dpkg 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		tar 		wget 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& make test 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 27 Oct 2020 18:17:49 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 27 Oct 2020 18:18:01 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 27 Oct 2020 18:18:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 27 Oct 2020 18:18:10 GMT
USER memcache
# Tue, 27 Oct 2020 18:18:14 GMT
EXPOSE 11211
# Tue, 27 Oct 2020 18:18:17 GMT
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
	-	`sha256:332ffea0c20ec81844b1417d8095ece2defbd4a4439ea55ad44ad30e790ce6cd`  
		Last Modified: Tue, 27 Oct 2020 18:19:02 GMT  
		Size: 1.7 MB (1742570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:392ddf5d69d4f45044e37865a42da609a84e104844687e3f5b9c0532959259dd`  
		Last Modified: Tue, 27 Oct 2020 18:19:01 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64e4999f6d01a1e5e7dff8d914201752111ae601d4d0a005ed699f3978802dde`  
		Last Modified: Tue, 27 Oct 2020 18:19:01 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.8-alpine` - linux; s390x

```console
$ docker pull memcached@sha256:85b524052ca329a4030178cf1cbbc80ff24c9c4ae4f6cdc3470034d4583cb6bb
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.3 MB (4276168 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f32b84ae0ba00026f01b2e172f787c9dd00b848ca611361cf654c422d83968e7`
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
# Tue, 27 Oct 2020 17:59:16 GMT
ENV MEMCACHED_VERSION=1.6.8
# Tue, 27 Oct 2020 17:59:16 GMT
ENV MEMCACHED_SHA1=8f3efd851efc5b822bd991b93d06a271b2fac052
# Fri, 30 Oct 2020 00:03:02 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		dpkg-dev dpkg 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		tar 		wget 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Fri, 30 Oct 2020 00:03:03 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 30 Oct 2020 00:03:04 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 30 Oct 2020 00:03:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 30 Oct 2020 00:03:05 GMT
USER memcache
# Fri, 30 Oct 2020 00:03:05 GMT
EXPOSE 11211
# Fri, 30 Oct 2020 00:03:06 GMT
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
	-	`sha256:2018ea964f59c9aed996180139b672f0113eab71e87ce85d31a4288d15e97b27`  
		Last Modified: Fri, 30 Oct 2020 00:03:32 GMT  
		Size: 1.7 MB (1693103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8737d71a5a761e864ed6a3679653563adfe843f43f330ccd04927a04e68cd35`  
		Last Modified: Fri, 30 Oct 2020 00:03:32 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d97cb533dbe95e5df4a514ea92cb2bb3e072a8210bd2ed19196671c8dc49a13`  
		Last Modified: Fri, 30 Oct 2020 00:03:32 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:1.6-alpine`

```console
$ docker pull memcached@sha256:8e31ec2228adcec5846663e069ea192344c4caa11fb96615404eaede343c90ec
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
$ docker pull memcached@sha256:71e3a793caad04dd57811a2aafa94612569c5d087bf1c5c871b603abdd1be630
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4495478 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e67bbd9b6e6573874b2e4563d209c0deadd89685497a754f5e47f9b373adca4d`
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
# Tue, 27 Oct 2020 18:01:01 GMT
ENV MEMCACHED_VERSION=1.6.8
# Tue, 27 Oct 2020 18:01:01 GMT
ENV MEMCACHED_SHA1=8f3efd851efc5b822bd991b93d06a271b2fac052
# Fri, 30 Oct 2020 02:04:11 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		dpkg-dev dpkg 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		tar 		wget 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Fri, 30 Oct 2020 02:04:11 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 30 Oct 2020 02:04:12 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 30 Oct 2020 02:04:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 30 Oct 2020 02:04:12 GMT
USER memcache
# Fri, 30 Oct 2020 02:04:13 GMT
EXPOSE 11211
# Fri, 30 Oct 2020 02:04:13 GMT
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
	-	`sha256:7303d373d89cbdae16f208a75a727b5ddb7f4e2861d02d11d382a9d42fc97cc3`  
		Last Modified: Fri, 30 Oct 2020 02:04:36 GMT  
		Size: 1.7 MB (1681682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ddff243a56604d00107678a49b86150ee4e22c6a0938bd3fbe9ce8a8dee2898`  
		Last Modified: Fri, 30 Oct 2020 02:04:36 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa411362f695820b3836affc1e76d4f6a470257081d90f0e7421231baca366cc`  
		Last Modified: Fri, 30 Oct 2020 02:04:36 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-alpine` - linux; arm variant v6

```console
$ docker pull memcached@sha256:7e31d9335251211f92511ec71fb1461f200d1ede4b9e3729b28a209debd4d9f8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.3 MB (4262175 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a88cc287311223e211ffb39fb1cfcc527e16f0b38a477ffecfae69a75f28947`
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
# Tue, 27 Oct 2020 17:50:52 GMT
ENV MEMCACHED_VERSION=1.6.8
# Tue, 27 Oct 2020 17:50:53 GMT
ENV MEMCACHED_SHA1=8f3efd851efc5b822bd991b93d06a271b2fac052
# Fri, 30 Oct 2020 00:28:33 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		dpkg-dev dpkg 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		tar 		wget 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Fri, 30 Oct 2020 00:28:34 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 30 Oct 2020 00:28:37 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 30 Oct 2020 00:28:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 30 Oct 2020 00:28:39 GMT
USER memcache
# Fri, 30 Oct 2020 00:28:40 GMT
EXPOSE 11211
# Fri, 30 Oct 2020 00:28:41 GMT
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
	-	`sha256:869dfda4a629dff09bee12e77e816513663c31197b3369a7a2df12c3d24f9734`  
		Last Modified: Fri, 30 Oct 2020 00:29:05 GMT  
		Size: 1.6 MB (1643699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc13f7ef8df67c31bd40e2ddf5678b3ed840e1901690a0ba39b9ad84e1493c7e`  
		Last Modified: Fri, 30 Oct 2020 00:29:04 GMT  
		Size: 282.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:014ddfe019df6e2dae30fd8acf752c68d3df2f3f3b7f1a3b274ab72f60e684d8`  
		Last Modified: Fri, 30 Oct 2020 00:29:06 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-alpine` - linux; arm variant v7

```console
$ docker pull memcached@sha256:cb005e7b4e652cbce090d5772626c2127b55f9bc8f282235a32c8f9f29a2af98
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.0 MB (3952565 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d49f3088ea875b790d47e63bc80ea9172ec25351e126f76d8090e1c95d8bb69c`
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
# Tue, 27 Oct 2020 18:02:39 GMT
ENV MEMCACHED_VERSION=1.6.8
# Tue, 27 Oct 2020 18:02:40 GMT
ENV MEMCACHED_SHA1=8f3efd851efc5b822bd991b93d06a271b2fac052
# Tue, 27 Oct 2020 18:12:34 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		dpkg-dev dpkg 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		tar 		wget 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& make test 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 27 Oct 2020 18:12:35 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 27 Oct 2020 18:12:37 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 27 Oct 2020 18:12:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 27 Oct 2020 18:12:38 GMT
USER memcache
# Tue, 27 Oct 2020 18:12:38 GMT
EXPOSE 11211
# Tue, 27 Oct 2020 18:12:39 GMT
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
	-	`sha256:6d24c3c688587cb0b6aa29bf3cb9be166d022bb6d46ee86740f03d8a204fadf6`  
		Last Modified: Tue, 27 Oct 2020 18:13:08 GMT  
		Size: 1.5 MB (1531399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:203f79e6fe3b93db04f06454f4da7c8dac400de74c97964885e0b94d5e21a69b`  
		Last Modified: Tue, 27 Oct 2020 18:13:08 GMT  
		Size: 283.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af3e72612c1e12f068d1f5c19f1c9c3eea8bb8fd7afed58892475c42e3ee1e3e`  
		Last Modified: Tue, 27 Oct 2020 18:13:08 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-alpine` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:1ce1d86238db5d088348cce464a468ac50b26d8aa01fe16c950f278e0cb63d0f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.4 MB (4411120 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:81f941fc95252e6747f1bab7de59cfbb48b440191a01117b53a45861f1902815`
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
# Tue, 27 Oct 2020 18:01:38 GMT
ENV MEMCACHED_VERSION=1.6.8
# Tue, 27 Oct 2020 18:01:38 GMT
ENV MEMCACHED_SHA1=8f3efd851efc5b822bd991b93d06a271b2fac052
# Tue, 27 Oct 2020 18:11:45 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		dpkg-dev dpkg 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		tar 		wget 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& make test 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 27 Oct 2020 18:11:48 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 27 Oct 2020 18:11:50 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 27 Oct 2020 18:11:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 27 Oct 2020 18:11:51 GMT
USER memcache
# Tue, 27 Oct 2020 18:11:52 GMT
EXPOSE 11211
# Tue, 27 Oct 2020 18:11:52 GMT
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
	-	`sha256:67fea89495771922e87061bccf414240a074727d95ece99c45ea8d027fa2b701`  
		Last Modified: Tue, 27 Oct 2020 18:12:21 GMT  
		Size: 1.7 MB (1687219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4745a66b526dd3a41a93a5e02a76afb529118e84b7198e5c793adbab0315e66c`  
		Last Modified: Tue, 27 Oct 2020 18:12:21 GMT  
		Size: 283.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8c659e4bd9d8b6c000e0d82cd2899b5ae3fec40641fbb4c67054d27cc338faf`  
		Last Modified: Tue, 27 Oct 2020 18:12:20 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-alpine` - linux; 386

```console
$ docker pull memcached@sha256:c89024e028c1823a713a0ae72e19a38b6fdc372377ec72de6cea84d48a3f095a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4585342 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:41421a77b44c877cc6bb4aa0a29a05da47ba69f789391845b0f383a620c16fba`
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
# Tue, 27 Oct 2020 18:20:12 GMT
ENV MEMCACHED_VERSION=1.6.8
# Tue, 27 Oct 2020 18:20:12 GMT
ENV MEMCACHED_SHA1=8f3efd851efc5b822bd991b93d06a271b2fac052
# Tue, 27 Oct 2020 23:55:05 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		dpkg-dev dpkg 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		tar 		wget 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& make test 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 27 Oct 2020 23:55:05 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 27 Oct 2020 23:55:06 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 27 Oct 2020 23:55:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 27 Oct 2020 23:55:07 GMT
USER memcache
# Tue, 27 Oct 2020 23:55:07 GMT
EXPOSE 11211
# Tue, 27 Oct 2020 23:55:07 GMT
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
	-	`sha256:09d187261acd1699a7536448083deb0fe4bd93125a0930418da3c8332bd6a52d`  
		Last Modified: Tue, 27 Oct 2020 23:55:27 GMT  
		Size: 1.8 MB (1775973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e7e368f966f2b955ec8c4aef5b440bf537f96f1b0b2275fb2981fe931c28d8d`  
		Last Modified: Tue, 27 Oct 2020 23:55:26 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8571d349dd3ca7fc4f303200d3e416fcfc88a390fa66344ef1d660d77ef9975`  
		Last Modified: Tue, 27 Oct 2020 23:55:27 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-alpine` - linux; ppc64le

```console
$ docker pull memcached@sha256:b2bcc724008b7866f1fb699f0308392ffdd8fdc3e5baf83c3e0f8c70b90d0eb9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4563777 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:29785833c149a374d3c03717ab9da503269016621376c89b78b7d6a2f3cd3a77`
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
# Tue, 27 Oct 2020 18:17:46 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		dpkg-dev dpkg 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		tar 		wget 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& make test 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 27 Oct 2020 18:17:49 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 27 Oct 2020 18:18:01 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 27 Oct 2020 18:18:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 27 Oct 2020 18:18:10 GMT
USER memcache
# Tue, 27 Oct 2020 18:18:14 GMT
EXPOSE 11211
# Tue, 27 Oct 2020 18:18:17 GMT
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
	-	`sha256:332ffea0c20ec81844b1417d8095ece2defbd4a4439ea55ad44ad30e790ce6cd`  
		Last Modified: Tue, 27 Oct 2020 18:19:02 GMT  
		Size: 1.7 MB (1742570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:392ddf5d69d4f45044e37865a42da609a84e104844687e3f5b9c0532959259dd`  
		Last Modified: Tue, 27 Oct 2020 18:19:01 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64e4999f6d01a1e5e7dff8d914201752111ae601d4d0a005ed699f3978802dde`  
		Last Modified: Tue, 27 Oct 2020 18:19:01 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-alpine` - linux; s390x

```console
$ docker pull memcached@sha256:85b524052ca329a4030178cf1cbbc80ff24c9c4ae4f6cdc3470034d4583cb6bb
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.3 MB (4276168 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f32b84ae0ba00026f01b2e172f787c9dd00b848ca611361cf654c422d83968e7`
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
# Tue, 27 Oct 2020 17:59:16 GMT
ENV MEMCACHED_VERSION=1.6.8
# Tue, 27 Oct 2020 17:59:16 GMT
ENV MEMCACHED_SHA1=8f3efd851efc5b822bd991b93d06a271b2fac052
# Fri, 30 Oct 2020 00:03:02 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		dpkg-dev dpkg 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		tar 		wget 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Fri, 30 Oct 2020 00:03:03 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 30 Oct 2020 00:03:04 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 30 Oct 2020 00:03:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 30 Oct 2020 00:03:05 GMT
USER memcache
# Fri, 30 Oct 2020 00:03:05 GMT
EXPOSE 11211
# Fri, 30 Oct 2020 00:03:06 GMT
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
	-	`sha256:2018ea964f59c9aed996180139b672f0113eab71e87ce85d31a4288d15e97b27`  
		Last Modified: Fri, 30 Oct 2020 00:03:32 GMT  
		Size: 1.7 MB (1693103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8737d71a5a761e864ed6a3679653563adfe843f43f330ccd04927a04e68cd35`  
		Last Modified: Fri, 30 Oct 2020 00:03:32 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d97cb533dbe95e5df4a514ea92cb2bb3e072a8210bd2ed19196671c8dc49a13`  
		Last Modified: Fri, 30 Oct 2020 00:03:32 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:1-alpine`

```console
$ docker pull memcached@sha256:8e31ec2228adcec5846663e069ea192344c4caa11fb96615404eaede343c90ec
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
$ docker pull memcached@sha256:71e3a793caad04dd57811a2aafa94612569c5d087bf1c5c871b603abdd1be630
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4495478 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e67bbd9b6e6573874b2e4563d209c0deadd89685497a754f5e47f9b373adca4d`
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
# Tue, 27 Oct 2020 18:01:01 GMT
ENV MEMCACHED_VERSION=1.6.8
# Tue, 27 Oct 2020 18:01:01 GMT
ENV MEMCACHED_SHA1=8f3efd851efc5b822bd991b93d06a271b2fac052
# Fri, 30 Oct 2020 02:04:11 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		dpkg-dev dpkg 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		tar 		wget 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Fri, 30 Oct 2020 02:04:11 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 30 Oct 2020 02:04:12 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 30 Oct 2020 02:04:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 30 Oct 2020 02:04:12 GMT
USER memcache
# Fri, 30 Oct 2020 02:04:13 GMT
EXPOSE 11211
# Fri, 30 Oct 2020 02:04:13 GMT
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
	-	`sha256:7303d373d89cbdae16f208a75a727b5ddb7f4e2861d02d11d382a9d42fc97cc3`  
		Last Modified: Fri, 30 Oct 2020 02:04:36 GMT  
		Size: 1.7 MB (1681682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ddff243a56604d00107678a49b86150ee4e22c6a0938bd3fbe9ce8a8dee2898`  
		Last Modified: Fri, 30 Oct 2020 02:04:36 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa411362f695820b3836affc1e76d4f6a470257081d90f0e7421231baca366cc`  
		Last Modified: Fri, 30 Oct 2020 02:04:36 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-alpine` - linux; arm variant v6

```console
$ docker pull memcached@sha256:7e31d9335251211f92511ec71fb1461f200d1ede4b9e3729b28a209debd4d9f8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.3 MB (4262175 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a88cc287311223e211ffb39fb1cfcc527e16f0b38a477ffecfae69a75f28947`
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
# Tue, 27 Oct 2020 17:50:52 GMT
ENV MEMCACHED_VERSION=1.6.8
# Tue, 27 Oct 2020 17:50:53 GMT
ENV MEMCACHED_SHA1=8f3efd851efc5b822bd991b93d06a271b2fac052
# Fri, 30 Oct 2020 00:28:33 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		dpkg-dev dpkg 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		tar 		wget 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Fri, 30 Oct 2020 00:28:34 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 30 Oct 2020 00:28:37 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 30 Oct 2020 00:28:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 30 Oct 2020 00:28:39 GMT
USER memcache
# Fri, 30 Oct 2020 00:28:40 GMT
EXPOSE 11211
# Fri, 30 Oct 2020 00:28:41 GMT
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
	-	`sha256:869dfda4a629dff09bee12e77e816513663c31197b3369a7a2df12c3d24f9734`  
		Last Modified: Fri, 30 Oct 2020 00:29:05 GMT  
		Size: 1.6 MB (1643699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc13f7ef8df67c31bd40e2ddf5678b3ed840e1901690a0ba39b9ad84e1493c7e`  
		Last Modified: Fri, 30 Oct 2020 00:29:04 GMT  
		Size: 282.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:014ddfe019df6e2dae30fd8acf752c68d3df2f3f3b7f1a3b274ab72f60e684d8`  
		Last Modified: Fri, 30 Oct 2020 00:29:06 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-alpine` - linux; arm variant v7

```console
$ docker pull memcached@sha256:cb005e7b4e652cbce090d5772626c2127b55f9bc8f282235a32c8f9f29a2af98
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.0 MB (3952565 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d49f3088ea875b790d47e63bc80ea9172ec25351e126f76d8090e1c95d8bb69c`
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
# Tue, 27 Oct 2020 18:02:39 GMT
ENV MEMCACHED_VERSION=1.6.8
# Tue, 27 Oct 2020 18:02:40 GMT
ENV MEMCACHED_SHA1=8f3efd851efc5b822bd991b93d06a271b2fac052
# Tue, 27 Oct 2020 18:12:34 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		dpkg-dev dpkg 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		tar 		wget 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& make test 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 27 Oct 2020 18:12:35 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 27 Oct 2020 18:12:37 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 27 Oct 2020 18:12:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 27 Oct 2020 18:12:38 GMT
USER memcache
# Tue, 27 Oct 2020 18:12:38 GMT
EXPOSE 11211
# Tue, 27 Oct 2020 18:12:39 GMT
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
	-	`sha256:6d24c3c688587cb0b6aa29bf3cb9be166d022bb6d46ee86740f03d8a204fadf6`  
		Last Modified: Tue, 27 Oct 2020 18:13:08 GMT  
		Size: 1.5 MB (1531399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:203f79e6fe3b93db04f06454f4da7c8dac400de74c97964885e0b94d5e21a69b`  
		Last Modified: Tue, 27 Oct 2020 18:13:08 GMT  
		Size: 283.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af3e72612c1e12f068d1f5c19f1c9c3eea8bb8fd7afed58892475c42e3ee1e3e`  
		Last Modified: Tue, 27 Oct 2020 18:13:08 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-alpine` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:1ce1d86238db5d088348cce464a468ac50b26d8aa01fe16c950f278e0cb63d0f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.4 MB (4411120 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:81f941fc95252e6747f1bab7de59cfbb48b440191a01117b53a45861f1902815`
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
# Tue, 27 Oct 2020 18:01:38 GMT
ENV MEMCACHED_VERSION=1.6.8
# Tue, 27 Oct 2020 18:01:38 GMT
ENV MEMCACHED_SHA1=8f3efd851efc5b822bd991b93d06a271b2fac052
# Tue, 27 Oct 2020 18:11:45 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		dpkg-dev dpkg 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		tar 		wget 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& make test 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 27 Oct 2020 18:11:48 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 27 Oct 2020 18:11:50 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 27 Oct 2020 18:11:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 27 Oct 2020 18:11:51 GMT
USER memcache
# Tue, 27 Oct 2020 18:11:52 GMT
EXPOSE 11211
# Tue, 27 Oct 2020 18:11:52 GMT
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
	-	`sha256:67fea89495771922e87061bccf414240a074727d95ece99c45ea8d027fa2b701`  
		Last Modified: Tue, 27 Oct 2020 18:12:21 GMT  
		Size: 1.7 MB (1687219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4745a66b526dd3a41a93a5e02a76afb529118e84b7198e5c793adbab0315e66c`  
		Last Modified: Tue, 27 Oct 2020 18:12:21 GMT  
		Size: 283.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8c659e4bd9d8b6c000e0d82cd2899b5ae3fec40641fbb4c67054d27cc338faf`  
		Last Modified: Tue, 27 Oct 2020 18:12:20 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-alpine` - linux; 386

```console
$ docker pull memcached@sha256:c89024e028c1823a713a0ae72e19a38b6fdc372377ec72de6cea84d48a3f095a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4585342 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:41421a77b44c877cc6bb4aa0a29a05da47ba69f789391845b0f383a620c16fba`
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
# Tue, 27 Oct 2020 18:20:12 GMT
ENV MEMCACHED_VERSION=1.6.8
# Tue, 27 Oct 2020 18:20:12 GMT
ENV MEMCACHED_SHA1=8f3efd851efc5b822bd991b93d06a271b2fac052
# Tue, 27 Oct 2020 23:55:05 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		dpkg-dev dpkg 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		tar 		wget 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& make test 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 27 Oct 2020 23:55:05 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 27 Oct 2020 23:55:06 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 27 Oct 2020 23:55:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 27 Oct 2020 23:55:07 GMT
USER memcache
# Tue, 27 Oct 2020 23:55:07 GMT
EXPOSE 11211
# Tue, 27 Oct 2020 23:55:07 GMT
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
	-	`sha256:09d187261acd1699a7536448083deb0fe4bd93125a0930418da3c8332bd6a52d`  
		Last Modified: Tue, 27 Oct 2020 23:55:27 GMT  
		Size: 1.8 MB (1775973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e7e368f966f2b955ec8c4aef5b440bf537f96f1b0b2275fb2981fe931c28d8d`  
		Last Modified: Tue, 27 Oct 2020 23:55:26 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8571d349dd3ca7fc4f303200d3e416fcfc88a390fa66344ef1d660d77ef9975`  
		Last Modified: Tue, 27 Oct 2020 23:55:27 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-alpine` - linux; ppc64le

```console
$ docker pull memcached@sha256:b2bcc724008b7866f1fb699f0308392ffdd8fdc3e5baf83c3e0f8c70b90d0eb9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4563777 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:29785833c149a374d3c03717ab9da503269016621376c89b78b7d6a2f3cd3a77`
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
# Tue, 27 Oct 2020 18:17:46 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		dpkg-dev dpkg 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		tar 		wget 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& make test 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 27 Oct 2020 18:17:49 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 27 Oct 2020 18:18:01 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 27 Oct 2020 18:18:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 27 Oct 2020 18:18:10 GMT
USER memcache
# Tue, 27 Oct 2020 18:18:14 GMT
EXPOSE 11211
# Tue, 27 Oct 2020 18:18:17 GMT
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
	-	`sha256:332ffea0c20ec81844b1417d8095ece2defbd4a4439ea55ad44ad30e790ce6cd`  
		Last Modified: Tue, 27 Oct 2020 18:19:02 GMT  
		Size: 1.7 MB (1742570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:392ddf5d69d4f45044e37865a42da609a84e104844687e3f5b9c0532959259dd`  
		Last Modified: Tue, 27 Oct 2020 18:19:01 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64e4999f6d01a1e5e7dff8d914201752111ae601d4d0a005ed699f3978802dde`  
		Last Modified: Tue, 27 Oct 2020 18:19:01 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-alpine` - linux; s390x

```console
$ docker pull memcached@sha256:85b524052ca329a4030178cf1cbbc80ff24c9c4ae4f6cdc3470034d4583cb6bb
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.3 MB (4276168 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f32b84ae0ba00026f01b2e172f787c9dd00b848ca611361cf654c422d83968e7`
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
# Tue, 27 Oct 2020 17:59:16 GMT
ENV MEMCACHED_VERSION=1.6.8
# Tue, 27 Oct 2020 17:59:16 GMT
ENV MEMCACHED_SHA1=8f3efd851efc5b822bd991b93d06a271b2fac052
# Fri, 30 Oct 2020 00:03:02 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		dpkg-dev dpkg 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		tar 		wget 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Fri, 30 Oct 2020 00:03:03 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 30 Oct 2020 00:03:04 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 30 Oct 2020 00:03:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 30 Oct 2020 00:03:05 GMT
USER memcache
# Fri, 30 Oct 2020 00:03:05 GMT
EXPOSE 11211
# Fri, 30 Oct 2020 00:03:06 GMT
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
	-	`sha256:2018ea964f59c9aed996180139b672f0113eab71e87ce85d31a4288d15e97b27`  
		Last Modified: Fri, 30 Oct 2020 00:03:32 GMT  
		Size: 1.7 MB (1693103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8737d71a5a761e864ed6a3679653563adfe843f43f330ccd04927a04e68cd35`  
		Last Modified: Fri, 30 Oct 2020 00:03:32 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d97cb533dbe95e5df4a514ea92cb2bb3e072a8210bd2ed19196671c8dc49a13`  
		Last Modified: Fri, 30 Oct 2020 00:03:32 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:alpine`

```console
$ docker pull memcached@sha256:8e31ec2228adcec5846663e069ea192344c4caa11fb96615404eaede343c90ec
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
$ docker pull memcached@sha256:71e3a793caad04dd57811a2aafa94612569c5d087bf1c5c871b603abdd1be630
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4495478 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e67bbd9b6e6573874b2e4563d209c0deadd89685497a754f5e47f9b373adca4d`
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
# Tue, 27 Oct 2020 18:01:01 GMT
ENV MEMCACHED_VERSION=1.6.8
# Tue, 27 Oct 2020 18:01:01 GMT
ENV MEMCACHED_SHA1=8f3efd851efc5b822bd991b93d06a271b2fac052
# Fri, 30 Oct 2020 02:04:11 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		dpkg-dev dpkg 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		tar 		wget 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Fri, 30 Oct 2020 02:04:11 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 30 Oct 2020 02:04:12 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 30 Oct 2020 02:04:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 30 Oct 2020 02:04:12 GMT
USER memcache
# Fri, 30 Oct 2020 02:04:13 GMT
EXPOSE 11211
# Fri, 30 Oct 2020 02:04:13 GMT
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
	-	`sha256:7303d373d89cbdae16f208a75a727b5ddb7f4e2861d02d11d382a9d42fc97cc3`  
		Last Modified: Fri, 30 Oct 2020 02:04:36 GMT  
		Size: 1.7 MB (1681682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ddff243a56604d00107678a49b86150ee4e22c6a0938bd3fbe9ce8a8dee2898`  
		Last Modified: Fri, 30 Oct 2020 02:04:36 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa411362f695820b3836affc1e76d4f6a470257081d90f0e7421231baca366cc`  
		Last Modified: Fri, 30 Oct 2020 02:04:36 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:alpine` - linux; arm variant v6

```console
$ docker pull memcached@sha256:7e31d9335251211f92511ec71fb1461f200d1ede4b9e3729b28a209debd4d9f8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.3 MB (4262175 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a88cc287311223e211ffb39fb1cfcc527e16f0b38a477ffecfae69a75f28947`
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
# Tue, 27 Oct 2020 17:50:52 GMT
ENV MEMCACHED_VERSION=1.6.8
# Tue, 27 Oct 2020 17:50:53 GMT
ENV MEMCACHED_SHA1=8f3efd851efc5b822bd991b93d06a271b2fac052
# Fri, 30 Oct 2020 00:28:33 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		dpkg-dev dpkg 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		tar 		wget 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Fri, 30 Oct 2020 00:28:34 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 30 Oct 2020 00:28:37 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 30 Oct 2020 00:28:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 30 Oct 2020 00:28:39 GMT
USER memcache
# Fri, 30 Oct 2020 00:28:40 GMT
EXPOSE 11211
# Fri, 30 Oct 2020 00:28:41 GMT
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
	-	`sha256:869dfda4a629dff09bee12e77e816513663c31197b3369a7a2df12c3d24f9734`  
		Last Modified: Fri, 30 Oct 2020 00:29:05 GMT  
		Size: 1.6 MB (1643699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc13f7ef8df67c31bd40e2ddf5678b3ed840e1901690a0ba39b9ad84e1493c7e`  
		Last Modified: Fri, 30 Oct 2020 00:29:04 GMT  
		Size: 282.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:014ddfe019df6e2dae30fd8acf752c68d3df2f3f3b7f1a3b274ab72f60e684d8`  
		Last Modified: Fri, 30 Oct 2020 00:29:06 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:alpine` - linux; arm variant v7

```console
$ docker pull memcached@sha256:cb005e7b4e652cbce090d5772626c2127b55f9bc8f282235a32c8f9f29a2af98
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.0 MB (3952565 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d49f3088ea875b790d47e63bc80ea9172ec25351e126f76d8090e1c95d8bb69c`
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
# Tue, 27 Oct 2020 18:02:39 GMT
ENV MEMCACHED_VERSION=1.6.8
# Tue, 27 Oct 2020 18:02:40 GMT
ENV MEMCACHED_SHA1=8f3efd851efc5b822bd991b93d06a271b2fac052
# Tue, 27 Oct 2020 18:12:34 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		dpkg-dev dpkg 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		tar 		wget 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& make test 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 27 Oct 2020 18:12:35 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 27 Oct 2020 18:12:37 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 27 Oct 2020 18:12:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 27 Oct 2020 18:12:38 GMT
USER memcache
# Tue, 27 Oct 2020 18:12:38 GMT
EXPOSE 11211
# Tue, 27 Oct 2020 18:12:39 GMT
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
	-	`sha256:6d24c3c688587cb0b6aa29bf3cb9be166d022bb6d46ee86740f03d8a204fadf6`  
		Last Modified: Tue, 27 Oct 2020 18:13:08 GMT  
		Size: 1.5 MB (1531399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:203f79e6fe3b93db04f06454f4da7c8dac400de74c97964885e0b94d5e21a69b`  
		Last Modified: Tue, 27 Oct 2020 18:13:08 GMT  
		Size: 283.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af3e72612c1e12f068d1f5c19f1c9c3eea8bb8fd7afed58892475c42e3ee1e3e`  
		Last Modified: Tue, 27 Oct 2020 18:13:08 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:alpine` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:1ce1d86238db5d088348cce464a468ac50b26d8aa01fe16c950f278e0cb63d0f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.4 MB (4411120 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:81f941fc95252e6747f1bab7de59cfbb48b440191a01117b53a45861f1902815`
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
# Tue, 27 Oct 2020 18:01:38 GMT
ENV MEMCACHED_VERSION=1.6.8
# Tue, 27 Oct 2020 18:01:38 GMT
ENV MEMCACHED_SHA1=8f3efd851efc5b822bd991b93d06a271b2fac052
# Tue, 27 Oct 2020 18:11:45 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		dpkg-dev dpkg 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		tar 		wget 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& make test 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 27 Oct 2020 18:11:48 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 27 Oct 2020 18:11:50 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 27 Oct 2020 18:11:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 27 Oct 2020 18:11:51 GMT
USER memcache
# Tue, 27 Oct 2020 18:11:52 GMT
EXPOSE 11211
# Tue, 27 Oct 2020 18:11:52 GMT
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
	-	`sha256:67fea89495771922e87061bccf414240a074727d95ece99c45ea8d027fa2b701`  
		Last Modified: Tue, 27 Oct 2020 18:12:21 GMT  
		Size: 1.7 MB (1687219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4745a66b526dd3a41a93a5e02a76afb529118e84b7198e5c793adbab0315e66c`  
		Last Modified: Tue, 27 Oct 2020 18:12:21 GMT  
		Size: 283.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8c659e4bd9d8b6c000e0d82cd2899b5ae3fec40641fbb4c67054d27cc338faf`  
		Last Modified: Tue, 27 Oct 2020 18:12:20 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:alpine` - linux; 386

```console
$ docker pull memcached@sha256:c89024e028c1823a713a0ae72e19a38b6fdc372377ec72de6cea84d48a3f095a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4585342 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:41421a77b44c877cc6bb4aa0a29a05da47ba69f789391845b0f383a620c16fba`
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
# Tue, 27 Oct 2020 18:20:12 GMT
ENV MEMCACHED_VERSION=1.6.8
# Tue, 27 Oct 2020 18:20:12 GMT
ENV MEMCACHED_SHA1=8f3efd851efc5b822bd991b93d06a271b2fac052
# Tue, 27 Oct 2020 23:55:05 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		dpkg-dev dpkg 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		tar 		wget 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& make test 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 27 Oct 2020 23:55:05 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 27 Oct 2020 23:55:06 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 27 Oct 2020 23:55:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 27 Oct 2020 23:55:07 GMT
USER memcache
# Tue, 27 Oct 2020 23:55:07 GMT
EXPOSE 11211
# Tue, 27 Oct 2020 23:55:07 GMT
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
	-	`sha256:09d187261acd1699a7536448083deb0fe4bd93125a0930418da3c8332bd6a52d`  
		Last Modified: Tue, 27 Oct 2020 23:55:27 GMT  
		Size: 1.8 MB (1775973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e7e368f966f2b955ec8c4aef5b440bf537f96f1b0b2275fb2981fe931c28d8d`  
		Last Modified: Tue, 27 Oct 2020 23:55:26 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8571d349dd3ca7fc4f303200d3e416fcfc88a390fa66344ef1d660d77ef9975`  
		Last Modified: Tue, 27 Oct 2020 23:55:27 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:alpine` - linux; ppc64le

```console
$ docker pull memcached@sha256:b2bcc724008b7866f1fb699f0308392ffdd8fdc3e5baf83c3e0f8c70b90d0eb9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4563777 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:29785833c149a374d3c03717ab9da503269016621376c89b78b7d6a2f3cd3a77`
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
# Tue, 27 Oct 2020 18:17:46 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		dpkg-dev dpkg 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		tar 		wget 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& make test 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 27 Oct 2020 18:17:49 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 27 Oct 2020 18:18:01 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 27 Oct 2020 18:18:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 27 Oct 2020 18:18:10 GMT
USER memcache
# Tue, 27 Oct 2020 18:18:14 GMT
EXPOSE 11211
# Tue, 27 Oct 2020 18:18:17 GMT
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
	-	`sha256:332ffea0c20ec81844b1417d8095ece2defbd4a4439ea55ad44ad30e790ce6cd`  
		Last Modified: Tue, 27 Oct 2020 18:19:02 GMT  
		Size: 1.7 MB (1742570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:392ddf5d69d4f45044e37865a42da609a84e104844687e3f5b9c0532959259dd`  
		Last Modified: Tue, 27 Oct 2020 18:19:01 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64e4999f6d01a1e5e7dff8d914201752111ae601d4d0a005ed699f3978802dde`  
		Last Modified: Tue, 27 Oct 2020 18:19:01 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:alpine` - linux; s390x

```console
$ docker pull memcached@sha256:85b524052ca329a4030178cf1cbbc80ff24c9c4ae4f6cdc3470034d4583cb6bb
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.3 MB (4276168 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f32b84ae0ba00026f01b2e172f787c9dd00b848ca611361cf654c422d83968e7`
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
# Tue, 27 Oct 2020 17:59:16 GMT
ENV MEMCACHED_VERSION=1.6.8
# Tue, 27 Oct 2020 17:59:16 GMT
ENV MEMCACHED_SHA1=8f3efd851efc5b822bd991b93d06a271b2fac052
# Fri, 30 Oct 2020 00:03:02 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		dpkg-dev dpkg 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		tar 		wget 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Fri, 30 Oct 2020 00:03:03 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 30 Oct 2020 00:03:04 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 30 Oct 2020 00:03:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 30 Oct 2020 00:03:05 GMT
USER memcache
# Fri, 30 Oct 2020 00:03:05 GMT
EXPOSE 11211
# Fri, 30 Oct 2020 00:03:06 GMT
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
	-	`sha256:2018ea964f59c9aed996180139b672f0113eab71e87ce85d31a4288d15e97b27`  
		Last Modified: Fri, 30 Oct 2020 00:03:32 GMT  
		Size: 1.7 MB (1693103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8737d71a5a761e864ed6a3679653563adfe843f43f330ccd04927a04e68cd35`  
		Last Modified: Fri, 30 Oct 2020 00:03:32 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d97cb533dbe95e5df4a514ea92cb2bb3e072a8210bd2ed19196671c8dc49a13`  
		Last Modified: Fri, 30 Oct 2020 00:03:32 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:latest`

```console
$ docker pull memcached@sha256:2c765a372d3e82565bc12bba67a0eb246baf536fd296ff6cb2e21c4036a62831
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
$ docker pull memcached@sha256:7be440dd3cc068fa2be188a7183890a8ff36e25e5a0c2edab25a4b6b460817c6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.5 MB (30493455 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:556880cb3d94c1509adc3eaf68dadf7d5e7325c5e5d2dcb86a8d0f8e0b4e4529`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 13 Oct 2020 01:39:05 GMT
ADD file:0dc53e7886c35bc21ae6c4f6cedda54d56ae9c9e9cd367678f1a72e68b3c43d4 in / 
# Tue, 13 Oct 2020 01:39:05 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 07:40:55 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 13 Oct 2020 07:41:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Oct 2020 17:51:22 GMT
ENV MEMCACHED_VERSION=1.6.8
# Tue, 27 Oct 2020 17:51:22 GMT
ENV MEMCACHED_SHA1=8f3efd851efc5b822bd991b93d06a271b2fac052
# Fri, 30 Oct 2020 01:59:43 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Fri, 30 Oct 2020 01:59:44 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 30 Oct 2020 01:59:44 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 30 Oct 2020 01:59:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 30 Oct 2020 01:59:45 GMT
USER memcache
# Fri, 30 Oct 2020 01:59:45 GMT
EXPOSE 11211
# Fri, 30 Oct 2020 01:59:45 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:bb79b6b2107fea8e8a47133a660b78e3a546998fcf0427be39ac9a0af4a97e90`  
		Last Modified: Tue, 13 Oct 2020 01:48:17 GMT  
		Size: 27.1 MB (27092228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5fbfe4d7c9b06eab9107d9ee46dbff27ea09707a40bdbdbea1d34078e65142a`  
		Last Modified: Tue, 13 Oct 2020 08:01:25 GMT  
		Size: 5.0 KB (4983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ed56f4a4fee8ed574be57dd51df7dc9f5bbdb041e9704be5a9ae0072a8a48b7`  
		Last Modified: Tue, 13 Oct 2020 08:01:26 GMT  
		Size: 2.2 MB (2196479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0186bf1dbc662c1e09f0a98b1182f4f1406a4b69b308ef63e0122450cfbca1b`  
		Last Modified: Fri, 30 Oct 2020 02:04:29 GMT  
		Size: 1.2 MB (1199359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f36909c1fe5329c92a34b3cde57aa972e7a53e582b7068c66d5e6af5e95bd86`  
		Last Modified: Fri, 30 Oct 2020 02:04:28 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e82197d1329427273caed560c08d7606a51afbb9bb34d2e4c0ed8bed4691cd3`  
		Last Modified: Fri, 30 Oct 2020 02:04:29 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:latest` - linux; arm variant v5

```console
$ docker pull memcached@sha256:281302b1776f2c06bbd2889f393368d96c44bcf61a889b7bb892b3b646629dfe
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.9 MB (27911064 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5cf13656486a2eb6df7a579ba2a4e613c12a4869f2bcd85097752033b87b1925`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 13 Oct 2020 01:52:17 GMT
ADD file:b71c0fa4957d6b65af37231a105f3d17cdbafe5c7d6c37b5843ebf619c608aaa in / 
# Tue, 13 Oct 2020 01:52:27 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 02:22:47 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 13 Oct 2020 02:23:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Oct 2020 17:48:42 GMT
ENV MEMCACHED_VERSION=1.6.8
# Tue, 27 Oct 2020 17:48:43 GMT
ENV MEMCACHED_SHA1=8f3efd851efc5b822bd991b93d06a271b2fac052
# Fri, 30 Oct 2020 01:54:09 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Fri, 30 Oct 2020 01:54:10 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 30 Oct 2020 01:54:12 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 30 Oct 2020 01:54:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 30 Oct 2020 01:54:14 GMT
USER memcache
# Fri, 30 Oct 2020 01:54:15 GMT
EXPOSE 11211
# Fri, 30 Oct 2020 01:54:16 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:f991c1e1ee2c48f16625b6b61310bf3c0616c0dbda4762019117e86fd29cf9ce`  
		Last Modified: Tue, 13 Oct 2020 02:01:27 GMT  
		Size: 24.8 MB (24835992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1b39a87be5bf0605d95ec4fc44790226547fdbcbad21c2add60885e9a1eabee`  
		Last Modified: Tue, 13 Oct 2020 02:34:18 GMT  
		Size: 4.9 KB (4897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d6238e630abdd7bca871de31aed93435c3e250ba2af1a0aaaabbec9d93d4452`  
		Last Modified: Tue, 13 Oct 2020 02:34:18 GMT  
		Size: 1.9 MB (1896831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a06241971793ab22b3a7ab4db8c18fc14c5b20227169c41d8bfce8fb6d67daa`  
		Last Modified: Fri, 30 Oct 2020 01:54:40 GMT  
		Size: 1.2 MB (1172937 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebc8ed09958e4b60fdf69ea8d28015f4cd3491968a22eced8fbf02720e2441bc`  
		Last Modified: Fri, 30 Oct 2020 01:54:40 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cb0a67800b722bbe27460d77886606a93383f456390e153365e2c38ae8cd602`  
		Last Modified: Fri, 30 Oct 2020 01:54:40 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:latest` - linux; arm variant v7

```console
$ docker pull memcached@sha256:3eb85207ec7eee29d5490f1f5b618eb232e57ad2654c929784518b7e42a589eb
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.7 MB (25660769 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b0e3423db692c288e1ce77ef4dccf8da40c46880e5bf18d42e6d8962016acce`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 13 Oct 2020 00:59:29 GMT
ADD file:e423f30ca19eb205a98de21b0545d0a764cfc4f832a9a9631542354d914d98d9 in / 
# Tue, 13 Oct 2020 00:59:31 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 04:26:19 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 13 Oct 2020 04:26:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Oct 2020 17:52:08 GMT
ENV MEMCACHED_VERSION=1.6.8
# Tue, 27 Oct 2020 17:52:09 GMT
ENV MEMCACHED_SHA1=8f3efd851efc5b822bd991b93d06a271b2fac052
# Tue, 27 Oct 2020 18:02:11 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 27 Oct 2020 18:02:12 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 27 Oct 2020 18:02:15 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 27 Oct 2020 18:02:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 27 Oct 2020 18:02:17 GMT
USER memcache
# Tue, 27 Oct 2020 18:02:18 GMT
EXPOSE 11211
# Tue, 27 Oct 2020 18:02:19 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:d6d8411ad43db0022fa0fce094cd2e8b1dd2f8a09d6880ed9beb6b4204867027`  
		Last Modified: Tue, 13 Oct 2020 01:08:28 GMT  
		Size: 22.7 MB (22699849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e36226ec0f789bddc127720ec631e27d952fb15b96b7848f3834950832523090`  
		Last Modified: Tue, 13 Oct 2020 04:37:29 GMT  
		Size: 4.9 KB (4895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46d8cf8973d9daad3ec5b519371371403ed2da2e65fa64c43d9122e8b8d602dd`  
		Last Modified: Tue, 13 Oct 2020 04:37:30 GMT  
		Size: 1.8 MB (1811537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc6baa5172a099a2af7b8031778e24fb072fc19291862933280eda0de2c1f873`  
		Last Modified: Tue, 27 Oct 2020 18:12:59 GMT  
		Size: 1.1 MB (1144080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79a4d1aadb5fa75c62ccfcb25624f53a840376fd2d43e3f2a37c4638437f36e5`  
		Last Modified: Tue, 27 Oct 2020 18:12:58 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61e633bd02bf4bd63bb51de860e7a23925d24c287faa53882423e30f3f283dff`  
		Last Modified: Tue, 27 Oct 2020 18:12:58 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:latest` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:d3355e1e1ca991f55ddc098c2f4795182e1c74228ddce7128898604bf04db22c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.1 MB (29100019 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a0715facdf2c1c1981d8ef7df462d2498fea30e381c80f46f6c8a2a2852d50e4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 13 Oct 2020 01:41:09 GMT
ADD file:3488b1423094a75be5bb5956e9187827b8dd35d7a1f2b14081f8e74a1629e7d0 in / 
# Tue, 13 Oct 2020 01:41:11 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 08:18:46 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 13 Oct 2020 08:18:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Oct 2020 17:50:52 GMT
ENV MEMCACHED_VERSION=1.6.8
# Tue, 27 Oct 2020 17:50:53 GMT
ENV MEMCACHED_SHA1=8f3efd851efc5b822bd991b93d06a271b2fac052
# Tue, 27 Oct 2020 18:01:23 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 27 Oct 2020 18:01:24 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 27 Oct 2020 18:01:27 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 27 Oct 2020 18:01:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 27 Oct 2020 18:01:28 GMT
USER memcache
# Tue, 27 Oct 2020 18:01:29 GMT
EXPOSE 11211
# Tue, 27 Oct 2020 18:01:29 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:4e6164a63b7b4cf981546947e191644c122214975d40b51ede0536791ebec3d4`  
		Last Modified: Tue, 13 Oct 2020 01:48:17 GMT  
		Size: 25.8 MB (25849329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5f7daf8dcdb72260976fee433136d1d7b10f4488b985960ff0cc9680258a37e`  
		Last Modified: Tue, 13 Oct 2020 08:29:40 GMT  
		Size: 5.0 KB (5026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3afc9b2342454a24b6fc4247345875720b7dce42da90e83c7b9a4abf57ff9257`  
		Last Modified: Tue, 13 Oct 2020 08:29:41 GMT  
		Size: 2.1 MB (2074972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:603fd7cc62d57991fc13951bf2f7e62b72e84aa1f942d74260c20c67319f7881`  
		Last Modified: Tue, 27 Oct 2020 18:12:12 GMT  
		Size: 1.2 MB (1170284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1741db6c55c297ff2a3645680bd6edd02a39a5414eb5eeac865437cf557a1965`  
		Last Modified: Tue, 27 Oct 2020 18:12:11 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4449d89ef06347eb4b3344c8149350461269d63e8c8e80e622fc44c2ac2a6f29`  
		Last Modified: Tue, 27 Oct 2020 18:12:11 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:latest` - linux; 386

```console
$ docker pull memcached@sha256:2de59fa093416ca4d4f33c162b006bedc526d2026d762c0bc434318fe947d32c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.2 MB (31161101 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2743c23aca6cb3863b084988e69eaad5de3ebf0cb317f57121ea69ba42d110af`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 13 Oct 2020 01:41:03 GMT
ADD file:51108b89c70ce0773c897be520c84454660f38b84ba556da49c7fe77e5d52416 in / 
# Tue, 13 Oct 2020 01:41:03 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 07:16:07 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 13 Oct 2020 07:16:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 07:16:13 GMT
ENV MEMCACHED_VERSION=1.6.7
# Tue, 13 Oct 2020 07:16:13 GMT
ENV MEMCACHED_SHA1=49336bb0a4b7ad296422b08148581ed54edf32d0
# Tue, 13 Oct 2020 07:36:28 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 13 Oct 2020 07:36:28 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 13 Oct 2020 07:36:29 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 13 Oct 2020 07:36:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Oct 2020 07:36:29 GMT
USER memcache
# Tue, 13 Oct 2020 07:36:30 GMT
EXPOSE 11211
# Tue, 13 Oct 2020 07:36:30 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:97e4efec21eea92209464547d0f52a0f773c505cf4ea9d8090cef667bde145b8`  
		Last Modified: Tue, 13 Oct 2020 01:48:54 GMT  
		Size: 27.8 MB (27750243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1e2733549a0a03eff9da2ad1035504ef29480a7fed2edb9ac19fcc6605081ec`  
		Last Modified: Tue, 13 Oct 2020 07:36:49 GMT  
		Size: 4.9 KB (4896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4434320f582eaf5fce7418fb99c35a07380e61385ed8d9ec07d383d46e426d06`  
		Last Modified: Tue, 13 Oct 2020 07:36:51 GMT  
		Size: 2.2 MB (2208112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0faf39e12c14d25e5dc802ddbe8f0068b4cc492ebf1e078998ddf38205c836dd`  
		Last Modified: Tue, 13 Oct 2020 07:36:49 GMT  
		Size: 1.2 MB (1197441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b95b4020f31dffe1467a69cfe85d22f7c6fa9d76da3678c72c99f23254899fb`  
		Last Modified: Tue, 13 Oct 2020 07:36:49 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5193dc6218dcc26a610b8c2175d11514acaf9dfa3239c9175399e84e805af6e`  
		Last Modified: Tue, 13 Oct 2020 07:36:49 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:latest` - linux; mips64le

```console
$ docker pull memcached@sha256:17830abbb92982a00a2a744bef4361b22205ce49e383d5aa64ed87fe355b73e8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.7 MB (28735721 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a0f82dfc53875f944220d793d546db85f16426855ed9bcf92643bf446dc1b45`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 13 Oct 2020 01:09:50 GMT
ADD file:c2ad270f70511601478158cfe3854499c0b4887f049b78b66903412a811a428a in / 
# Tue, 13 Oct 2020 01:09:50 GMT
CMD ["bash"]
# Tue, 27 Oct 2020 17:50:08 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 27 Oct 2020 17:50:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Oct 2020 17:50:20 GMT
ENV MEMCACHED_VERSION=1.6.8
# Tue, 27 Oct 2020 17:50:21 GMT
ENV MEMCACHED_SHA1=8f3efd851efc5b822bd991b93d06a271b2fac052
# Wed, 28 Oct 2020 04:30:47 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 28 Oct 2020 04:30:47 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 28 Oct 2020 04:30:49 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 28 Oct 2020 04:30:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 28 Oct 2020 04:30:49 GMT
USER memcache
# Wed, 28 Oct 2020 04:30:50 GMT
EXPOSE 11211
# Wed, 28 Oct 2020 04:30:50 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:9bc77d453b2242ec513032b61e23061712b79c3ba0c60114232d743e5ab4e4fa`  
		Last Modified: Tue, 13 Oct 2020 01:16:41 GMT  
		Size: 25.8 MB (25762577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac83b13333509b8c185fea403b7631388624cc708325d7b746192c2d84d61c30`  
		Last Modified: Wed, 28 Oct 2020 04:31:10 GMT  
		Size: 5.0 KB (4986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b9c5336b4ffdcc16c62c61e285bced1eb40b5f252a0415b6393dc002e8f2eb8`  
		Last Modified: Wed, 28 Oct 2020 04:31:11 GMT  
		Size: 1.8 MB (1776027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7a4b59edf43de7ce3f3c4bbbd099c545e953b12913a9896ee2d266756346cb2`  
		Last Modified: Wed, 28 Oct 2020 04:31:11 GMT  
		Size: 1.2 MB (1191725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b84ace4a71dbe705a2cfc2673e134f77a1a04af75a13cbed6c072e6a6aeb1959`  
		Last Modified: Wed, 28 Oct 2020 04:31:10 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3552aec564382a3d8d830a584ee44b0d9ac151ab28e895c6882cc7c49867a7e3`  
		Last Modified: Wed, 28 Oct 2020 04:31:10 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:latest` - linux; ppc64le

```console
$ docker pull memcached@sha256:63c6b668e4938f19c9241f75a6b1531450c923fe79c562e6e6c50cfb6cec2a73
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.1 MB (34071374 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:98fbacd51c7d4950a68cd17040fbbf8b66e12570881a73a3090011d15078efb3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 13 Oct 2020 01:38:54 GMT
ADD file:9992867f855c9bed54df6d26f3d8076689aff8a51e808fefba7d3b66dab250e5 in / 
# Tue, 13 Oct 2020 01:38:59 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 10:01:29 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 13 Oct 2020 10:01:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Oct 2020 17:54:17 GMT
ENV MEMCACHED_VERSION=1.6.8
# Tue, 27 Oct 2020 17:54:22 GMT
ENV MEMCACHED_SHA1=8f3efd851efc5b822bd991b93d06a271b2fac052
# Tue, 27 Oct 2020 18:06:37 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 27 Oct 2020 18:06:40 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 27 Oct 2020 18:06:51 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 27 Oct 2020 18:06:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 27 Oct 2020 18:07:06 GMT
USER memcache
# Tue, 27 Oct 2020 18:07:11 GMT
EXPOSE 11211
# Tue, 27 Oct 2020 18:07:15 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:523555c6877c72cfcdec912b4d0053c298b1c97835efc7c6b0211585a06bd563`  
		Last Modified: Tue, 13 Oct 2020 01:50:10 GMT  
		Size: 30.5 MB (30517878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d6959d8bd92e8076720fb05de0ab3aa2972b4ed7c8aa85a1041abfbe2d8b56d`  
		Last Modified: Tue, 13 Oct 2020 10:16:27 GMT  
		Size: 5.0 KB (4984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bff6c7a70d59d80356167379e564384edc47a14264bcf7c91253653d4fa25071`  
		Last Modified: Tue, 13 Oct 2020 10:16:28 GMT  
		Size: 2.3 MB (2322777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56f5e94b0b94ab1f9c233ca3f5e3baa17b07f384cdd6fb8a1376bc4b3a1a22b9`  
		Last Modified: Tue, 27 Oct 2020 18:18:43 GMT  
		Size: 1.2 MB (1225330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7382b7d44dc710539db62bbeef153180b699ea1f735ad8f0eafb2999212cb26`  
		Last Modified: Tue, 27 Oct 2020 18:18:43 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98b83690c808dc9c5fc3ce938c34e970f6f109eeb8ad63515817b142c91cd0a5`  
		Last Modified: Tue, 27 Oct 2020 18:18:43 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:latest` - linux; s390x

```console
$ docker pull memcached@sha256:e11001edc21564af26a9f33a46dc3e1f6ee37e5571e60ce0d1c3fd3e1a9b629b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.8 MB (28789423 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5908f7dcace1ea65f0f60df58c4b3eb55a4d998703b4833ac64755eab9b67f6b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 13 Oct 2020 01:42:26 GMT
ADD file:f932c1176fdc9bf45ced816290f83e6231df3dffa3b7f8de1a3bb0adcff1588b in / 
# Tue, 13 Oct 2020 01:42:27 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 02:44:44 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 13 Oct 2020 02:44:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Oct 2020 17:50:18 GMT
ENV MEMCACHED_VERSION=1.6.8
# Tue, 27 Oct 2020 17:50:18 GMT
ENV MEMCACHED_SHA1=8f3efd851efc5b822bd991b93d06a271b2fac052
# Thu, 29 Oct 2020 23:59:00 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 29 Oct 2020 23:59:01 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 29 Oct 2020 23:59:03 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 29 Oct 2020 23:59:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 29 Oct 2020 23:59:04 GMT
USER memcache
# Thu, 29 Oct 2020 23:59:04 GMT
EXPOSE 11211
# Thu, 29 Oct 2020 23:59:04 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:2a4f9dc00d797c86c4ffce3b50bea9037c2eb4637f045ad3fd68cf151577b639`  
		Last Modified: Tue, 13 Oct 2020 01:45:45 GMT  
		Size: 25.7 MB (25707519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:307f2e192d445f2ae2ac5cf8ca173572473106ec1cedc16591ec31c2deed4602`  
		Last Modified: Tue, 13 Oct 2020 02:54:35 GMT  
		Size: 5.0 KB (5025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52a19707e552eac63bdd433244f456e992ca13a66f297d1fc326581c1d9e4f6d`  
		Last Modified: Tue, 13 Oct 2020 02:54:35 GMT  
		Size: 1.9 MB (1886119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:397803f765cfd9441284c39d53f61e465182b3e2955d49b556fcc2fd1ef4fcf5`  
		Last Modified: Fri, 30 Oct 2020 00:03:22 GMT  
		Size: 1.2 MB (1190355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19b4081264507735ea4c811cabeecb378f570f273f5a2cb577d8a49e42ea02b4`  
		Last Modified: Fri, 30 Oct 2020 00:03:22 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56c4bffa4499b85119f852d11d10aaca8ba7eb8488b9ff595b418f79a12ec769`  
		Last Modified: Fri, 30 Oct 2020 00:03:23 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
