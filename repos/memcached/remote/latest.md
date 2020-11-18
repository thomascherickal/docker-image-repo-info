## `memcached:latest`

```console
$ docker pull memcached@sha256:6fa41b34b096939f4af649052a98f2d0435964b4a74e9197a843cb06d28f06ee
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
$ docker pull memcached@sha256:d620f67ebe439008b39954f2e897a9574c720ea0c3406c037806f5424e15b5d6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.5 MB (30506631 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ea9366871048879586f83b4d92f4b8ef5d55a7a85cb66acb5e3c8a923f35ba0`
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
# Tue, 17 Nov 2020 23:59:19 GMT
ENV MEMCACHED_VERSION=1.6.8
# Tue, 17 Nov 2020 23:59:20 GMT
ENV MEMCACHED_SHA1=8f3efd851efc5b822bd991b93d06a271b2fac052
# Wed, 18 Nov 2020 00:03:56 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 18 Nov 2020 00:03:56 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 18 Nov 2020 00:03:57 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 18 Nov 2020 00:03:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 18 Nov 2020 00:03:58 GMT
USER memcache
# Wed, 18 Nov 2020 00:03:58 GMT
EXPOSE 11211
# Wed, 18 Nov 2020 00:03:58 GMT
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
	-	`sha256:05486a32734659c9867a15b445a105b6026838bfaf1e9642bba14af0af341870`  
		Last Modified: Wed, 18 Nov 2020 00:04:27 GMT  
		Size: 1.2 MB (1199327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53a8b6d476a1cbc5b9cca8f037dda5ce359056d8a9f64daada9051c8913dc382`  
		Last Modified: Wed, 18 Nov 2020 00:04:26 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d447334cbf94d0e763387f256e05ee97184294f2769790d659222272e3f44d7d`  
		Last Modified: Wed, 18 Nov 2020 00:04:26 GMT  
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
$ docker pull memcached@sha256:e44b115a31d1b633a6ded862b6ad94fa150fc7c7bdf9ff2926aa645295a4ff9f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.7 MB (25675013 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c6d825045793e84f98e272e95ad0be858166711b463b13642f21b6cae8d45669`
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
# Tue, 17 Nov 2020 22:43:10 GMT
ENV MEMCACHED_VERSION=1.6.8
# Tue, 17 Nov 2020 22:43:11 GMT
ENV MEMCACHED_SHA1=8f3efd851efc5b822bd991b93d06a271b2fac052
# Tue, 17 Nov 2020 22:46:28 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 17 Nov 2020 22:46:29 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 17 Nov 2020 22:46:31 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 17 Nov 2020 22:46:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 17 Nov 2020 22:46:34 GMT
USER memcache
# Tue, 17 Nov 2020 22:46:35 GMT
EXPOSE 11211
# Tue, 17 Nov 2020 22:46:36 GMT
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
	-	`sha256:02426179161d04a3173fa79c1756a81985dda1049e173c9d5ce118699afb5e6c`  
		Last Modified: Tue, 17 Nov 2020 22:47:05 GMT  
		Size: 1.1 MB (1144001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1512149d4c9e710e6bcd483ae8b0a60982495be4955e5a1fe5ef304d9ed2cc41`  
		Last Modified: Tue, 17 Nov 2020 22:47:03 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ffbef6aa533d73e4737ae4e4a915dfa014b1f05da2ff31a0e8bcf1da45d8140`  
		Last Modified: Tue, 17 Nov 2020 22:47:04 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:latest` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:9ea97e86c6d2b998c788cebd8351207978529774ece3462b920876b3215de27d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.1 MB (29113104 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc63ad6bb1916e14a554fcbf81c0e9ef60e1cd44aff5972fe640c38b5e468f6e`
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
# Wed, 18 Nov 2020 01:22:53 GMT
ENV MEMCACHED_VERSION=1.6.8
# Wed, 18 Nov 2020 01:22:54 GMT
ENV MEMCACHED_SHA1=8f3efd851efc5b822bd991b93d06a271b2fac052
# Wed, 18 Nov 2020 01:26:19 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 18 Nov 2020 01:26:20 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 18 Nov 2020 01:26:24 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 18 Nov 2020 01:26:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 18 Nov 2020 01:26:27 GMT
USER memcache
# Wed, 18 Nov 2020 01:26:29 GMT
EXPOSE 11211
# Wed, 18 Nov 2020 01:26:29 GMT
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
	-	`sha256:fff186e158dab8c6456dadf2222ed10e7ec7ee2e69e0fbd2d7051d70777a11cd`  
		Last Modified: Wed, 18 Nov 2020 01:26:58 GMT  
		Size: 1.2 MB (1170190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d5d3e53f6a35c22082b1588842125563ef8b80856bf8834c5914979a87cd780`  
		Last Modified: Wed, 18 Nov 2020 01:26:58 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a06a0a2856704a0ac5f358d24e26a037ce7c100c93ae209c26d8f283bf1db02b`  
		Last Modified: Wed, 18 Nov 2020 01:26:58 GMT  
		Size: 119.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:latest` - linux; 386

```console
$ docker pull memcached@sha256:c0d1c2a68d0839f481ebb185a6fd6d7e24bc2b0f7a5448a2f188d1e83394b236
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.2 MB (31160996 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ea44aff3a200e90e6b2403e5c6b1bb36c54d648723ac3a9ecf210c8343bc2e72`
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
# Tue, 27 Oct 2020 17:50:33 GMT
ENV MEMCACHED_VERSION=1.6.8
# Tue, 27 Oct 2020 17:50:34 GMT
ENV MEMCACHED_SHA1=8f3efd851efc5b822bd991b93d06a271b2fac052
# Fri, 30 Oct 2020 05:24:16 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Fri, 30 Oct 2020 05:24:16 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 30 Oct 2020 05:24:17 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 30 Oct 2020 05:24:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 30 Oct 2020 05:24:17 GMT
USER memcache
# Fri, 30 Oct 2020 05:24:17 GMT
EXPOSE 11211
# Fri, 30 Oct 2020 05:24:17 GMT
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
	-	`sha256:00526a406b91287278c9c09425d176a22e2268390abeedba865b8639eba8b43c`  
		Last Modified: Fri, 30 Oct 2020 05:24:42 GMT  
		Size: 1.2 MB (1197342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3b610e27be132d61fd5e68bfa3faecff173f72218631f10e3c7849ef84f5e29`  
		Last Modified: Fri, 30 Oct 2020 05:24:42 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d25842fc35f822f92b7eba7bef938db0ebae981718f2788f8116269361f39fe1`  
		Last Modified: Fri, 30 Oct 2020 05:24:42 GMT  
		Size: 118.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:latest` - linux; mips64le

```console
$ docker pull memcached@sha256:6c96841fb22c6aff75d7f24286b9e374792adda5b6cc0b00d8f17120a7072a2c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.7 MB (28735728 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eaa8455c9b46bc55bd05b6b287b6272f96553f71a97db6c74c62b5ded36a8c1d`
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
# Fri, 30 Oct 2020 03:01:49 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Fri, 30 Oct 2020 03:01:49 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 30 Oct 2020 03:01:51 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 30 Oct 2020 03:01:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 30 Oct 2020 03:01:52 GMT
USER memcache
# Fri, 30 Oct 2020 03:01:52 GMT
EXPOSE 11211
# Fri, 30 Oct 2020 03:01:52 GMT
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
	-	`sha256:6c8ce9d9c36756b87a3f9f73b2acb356b42ea5f4fe9cb3b1b066c996bfb5c0ca`  
		Last Modified: Fri, 30 Oct 2020 03:02:20 GMT  
		Size: 1.2 MB (1191733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d0f5dfadc15ec5e9eac076e5ecfca236be9e48d8c6980d6cfa0259da1a8e434`  
		Last Modified: Fri, 30 Oct 2020 03:02:19 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10a63597942f04f03939e3a395e033d08d25c40a31d2873bb5b10a79655b5d8e`  
		Last Modified: Fri, 30 Oct 2020 03:02:19 GMT  
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
$ docker pull memcached@sha256:2ba9ffada04413aa9be2298417a3517afd5711758e730ffcc81d0e744e78518b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.8 MB (28803008 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e09b79390db2d70d71a341e1c5ceb71618524c34511cd2054838b65a1f37c125`
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
# Wed, 18 Nov 2020 01:46:40 GMT
ENV MEMCACHED_VERSION=1.6.8
# Wed, 18 Nov 2020 01:46:41 GMT
ENV MEMCACHED_SHA1=8f3efd851efc5b822bd991b93d06a271b2fac052
# Wed, 18 Nov 2020 01:52:35 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 18 Nov 2020 01:52:35 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 18 Nov 2020 01:52:37 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 18 Nov 2020 01:52:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 18 Nov 2020 01:52:39 GMT
USER memcache
# Wed, 18 Nov 2020 01:52:39 GMT
EXPOSE 11211
# Wed, 18 Nov 2020 01:52:40 GMT
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
	-	`sha256:3935947d09c9f13e9275af6187a6985a4416cc977d517745a0f2ca8f589af95e`  
		Last Modified: Wed, 18 Nov 2020 01:53:06 GMT  
		Size: 1.2 MB (1190338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:657f5f32a2438d45137214b10fb93c955640e1e88be391bfe2bcb2036c868001`  
		Last Modified: Wed, 18 Nov 2020 01:53:05 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1c9152632048d40f576ec28d298582ccdb858a3ab7324bcca0a8d652d18fdbc`  
		Last Modified: Wed, 18 Nov 2020 01:53:05 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
