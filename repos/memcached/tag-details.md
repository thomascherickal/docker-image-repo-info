<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `memcached`

-	[`memcached:1`](#memcached1)
-	[`memcached:1.6`](#memcached16)
-	[`memcached:1.6.7`](#memcached167)
-	[`memcached:1.6.7-alpine`](#memcached167-alpine)
-	[`memcached:1.6-alpine`](#memcached16-alpine)
-	[`memcached:1-alpine`](#memcached1-alpine)
-	[`memcached:alpine`](#memcachedalpine)
-	[`memcached:latest`](#memcachedlatest)

## `memcached:1`

```console
$ docker pull memcached@sha256:d999887e1fbd1ae9c6209459ae28ee0477c034b40ab2c6b492aa6a3dd3a3f564
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
$ docker pull memcached@sha256:7b8d8fbef4feb9386884d0aa2ecd3912aa62f2ec26efea54a57bc8fcf78348b6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.5 MB (30493470 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b4920487992d3dbbe4aa89a7336e06600ab8b41fe8f889212e927f7fbb19593`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 10 Sep 2020 00:23:29 GMT
ADD file:e7407f2294ad23634565820b9669b18ff2a2ca0212a7ec84b9c89d8550859954 in / 
# Thu, 10 Sep 2020 00:23:30 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 06:42:10 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Thu, 10 Sep 2020 06:42:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 06:42:17 GMT
ENV MEMCACHED_VERSION=1.6.7
# Thu, 10 Sep 2020 06:42:18 GMT
ENV MEMCACHED_SHA1=49336bb0a4b7ad296422b08148581ed54edf32d0
# Thu, 10 Sep 2020 06:52:26 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 10 Sep 2020 06:52:26 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 10 Sep 2020 06:52:28 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 10 Sep 2020 06:52:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 10 Sep 2020 06:52:28 GMT
USER memcache
# Thu, 10 Sep 2020 06:52:29 GMT
EXPOSE 11211
# Thu, 10 Sep 2020 06:52:29 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:d121f8d1c4128ebc1e95e5bfad90a0189b84eadbbb2fbaad20cbb26d20b2c8a2`  
		Last Modified: Thu, 10 Sep 2020 00:34:02 GMT  
		Size: 27.1 MB (27092161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd29e75844e2246d981d63970769902be264bae0990bb5befc493e5d15eeeeb3`  
		Last Modified: Thu, 10 Sep 2020 06:52:50 GMT  
		Size: 5.0 KB (4980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1adbe52eab585d7464430faaab2b3f8759b1661558262688357dba99e6967db7`  
		Last Modified: Thu, 10 Sep 2020 06:52:50 GMT  
		Size: 2.2 MB (2196512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e7563db9f0d12fba4b16ab48ba07e143239fc53283b76b6532d09a26ed523e8`  
		Last Modified: Thu, 10 Sep 2020 06:52:50 GMT  
		Size: 1.2 MB (1199409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1018860c7c78773f11445b24c799624ebf7ad0c1a54955ee73a0d1fdf7eeb40`  
		Last Modified: Thu, 10 Sep 2020 06:52:50 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b02cff55081f0c25f0ae11f642177cfec21627dce0ad4f9593653f121d8a2297`  
		Last Modified: Thu, 10 Sep 2020 06:52:50 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1` - linux; arm variant v5

```console
$ docker pull memcached@sha256:db8e75930e7350dc06c594abc4f6eb130088c7a803729f2125820e48992c5e60
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.9 MB (27911252 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ca29ad8c51e933907ffd5cacfd7b034a533f7b15c99c2202743dd723b229f5a3`
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
# Tue, 13 Oct 2020 02:23:01 GMT
ENV MEMCACHED_VERSION=1.6.7
# Tue, 13 Oct 2020 02:23:02 GMT
ENV MEMCACHED_SHA1=49336bb0a4b7ad296422b08148581ed54edf32d0
# Tue, 13 Oct 2020 02:33:45 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 13 Oct 2020 02:33:46 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 13 Oct 2020 02:33:51 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 13 Oct 2020 02:33:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Oct 2020 02:33:53 GMT
USER memcache
# Tue, 13 Oct 2020 02:33:55 GMT
EXPOSE 11211
# Tue, 13 Oct 2020 02:33:57 GMT
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
	-	`sha256:85530c3b6a178a04b529523c2bf5e513e04d7a42f2cdebf26a69b484b56a68e2`  
		Last Modified: Tue, 13 Oct 2020 02:34:18 GMT  
		Size: 1.2 MB (1173125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38d48859b3d5f2dfe3a0ddff8417717ec4274b5d7431850f3434a35d856c8326`  
		Last Modified: Tue, 13 Oct 2020 02:34:18 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84b665bad50ddd6ddfcf2dc2cc9e826499da002347faf18378e77a3dc6f81505`  
		Last Modified: Tue, 13 Oct 2020 02:34:18 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1` - linux; arm variant v7

```console
$ docker pull memcached@sha256:534ab9a71bfdbc6306e5f0e66af8fe0f76bc509560817621b7e31c9dc7f94ac7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.7 MB (25660617 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ef1c3640e673dfff34704d898b5bb45aa552e63246457eb196726184a948b0a7`
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
# Tue, 13 Oct 2020 04:26:30 GMT
ENV MEMCACHED_VERSION=1.6.7
# Tue, 13 Oct 2020 04:26:31 GMT
ENV MEMCACHED_SHA1=49336bb0a4b7ad296422b08148581ed54edf32d0
# Tue, 13 Oct 2020 04:36:50 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 13 Oct 2020 04:36:51 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 13 Oct 2020 04:36:54 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 13 Oct 2020 04:36:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Oct 2020 04:36:56 GMT
USER memcache
# Tue, 13 Oct 2020 04:36:57 GMT
EXPOSE 11211
# Tue, 13 Oct 2020 04:36:57 GMT
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
	-	`sha256:d50f05a1d5be98ec50a0b9c6b32e28b0673ad3db35c5b90500b0a38cd1697589`  
		Last Modified: Tue, 13 Oct 2020 04:37:30 GMT  
		Size: 1.1 MB (1143928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a0ff448c0efd0905dc11c59b70feb4dd6cd02adda52ec427fa68bd0664cf165`  
		Last Modified: Tue, 13 Oct 2020 04:37:29 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c8559eb111bdc28303506d117e61bb26e47daa128d7fdb057bace4acaeeb1c4`  
		Last Modified: Tue, 13 Oct 2020 04:37:29 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:7f9d722d816e4b63c87642fde2b901849b416838b47ab197bb52a4bec0ca01b6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.1 MB (29099929 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ea99cfec94c49c44ccb283458d9addd82f2763524a936bf3962202eecbe4e74`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 09 Sep 2020 23:50:54 GMT
ADD file:d870fb0484ea283840d9cc923c9c3fe36d1bb6b3b5ecfefcce06aa26a22c9414 in / 
# Wed, 09 Sep 2020 23:50:57 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 04:21:07 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Thu, 10 Sep 2020 04:21:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 04:21:19 GMT
ENV MEMCACHED_VERSION=1.6.7
# Thu, 10 Sep 2020 04:21:20 GMT
ENV MEMCACHED_SHA1=49336bb0a4b7ad296422b08148581ed54edf32d0
# Thu, 10 Sep 2020 04:31:42 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 10 Sep 2020 04:31:43 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 10 Sep 2020 04:31:45 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 10 Sep 2020 04:31:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 10 Sep 2020 04:31:46 GMT
USER memcache
# Thu, 10 Sep 2020 04:31:47 GMT
EXPOSE 11211
# Thu, 10 Sep 2020 04:31:48 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:a6d76de28f58f3470aff71c934c0fec4e5d0fad788f8b8bcc50601266fc1b34d`  
		Last Modified: Wed, 09 Sep 2020 23:59:09 GMT  
		Size: 25.8 MB (25849325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4f48bd1f465fe61c5d378a72dea86a5917d8ec222d9eda27c13d06a0388ce45`  
		Last Modified: Thu, 10 Sep 2020 04:32:19 GMT  
		Size: 5.0 KB (5023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6172eb8b991d9ee34cce4d10ae2d0a18036999e58977cb193f2493dba1d0922d`  
		Last Modified: Thu, 10 Sep 2020 04:32:19 GMT  
		Size: 2.1 MB (2075014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c4390371d3044be59e120ad4ac5e0ab67b9eaacd1a1fd97388724d7ffe5a5d8`  
		Last Modified: Thu, 10 Sep 2020 04:32:19 GMT  
		Size: 1.2 MB (1170159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8212b808878005bf5387d12077984b9fd4f2c6127c29515d63fbaabb572648a0`  
		Last Modified: Thu, 10 Sep 2020 04:32:19 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6dd274731a18972c07fee896065b96cd0d476de9b6a13ea57e0a1577e762d14`  
		Last Modified: Thu, 10 Sep 2020 04:32:18 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1` - linux; 386

```console
$ docker pull memcached@sha256:0fb71355a775a0f518e405710c83cff1d60dd0fddf7bb066ec19ce5c98ecb1fe
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.2 MB (31161216 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c69f202ca7e7d00a1d7deb0fdf47bda4a4fc3d57af1ee1e2d39e3e9eb7196ba`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 09 Sep 2020 23:40:19 GMT
ADD file:08dc20c9cd727ebf02cac6e4b287c3009274682174aee9222494491cd6c671b8 in / 
# Wed, 09 Sep 2020 23:40:19 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 02:19:41 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Thu, 10 Sep 2020 02:19:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 02:19:51 GMT
ENV MEMCACHED_VERSION=1.6.7
# Thu, 10 Sep 2020 02:19:52 GMT
ENV MEMCACHED_SHA1=49336bb0a4b7ad296422b08148581ed54edf32d0
# Thu, 10 Sep 2020 02:30:13 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 10 Sep 2020 02:30:13 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 10 Sep 2020 02:30:14 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 10 Sep 2020 02:30:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 10 Sep 2020 02:30:14 GMT
USER memcache
# Thu, 10 Sep 2020 02:30:15 GMT
EXPOSE 11211
# Thu, 10 Sep 2020 02:30:15 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:31e6582dbd9f9a84903d46339df0c393a63d2cbfb001b06b3204653cceafcc61`  
		Last Modified: Wed, 09 Sep 2020 23:46:30 GMT  
		Size: 27.8 MB (27750334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:096b2a6b5e34ad8c96b35f52e3615e85902d5b12f7bdbf4f984988b59ba14ac3`  
		Last Modified: Thu, 10 Sep 2020 02:30:33 GMT  
		Size: 4.9 KB (4895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ece6f6a2e1723d610af9b172d870ab4c9e6e3c132f316e5f7baa2787806fbae6`  
		Last Modified: Thu, 10 Sep 2020 02:30:33 GMT  
		Size: 2.2 MB (2208153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3df397ec8999490a45ed35ff7908dacec384cecced47533e490dd01de7e4a320`  
		Last Modified: Thu, 10 Sep 2020 02:30:34 GMT  
		Size: 1.2 MB (1197426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:debebc596e2e5ea23dca7e24bc712d7ed9942d1db2397c4140b12ce8af1ce21f`  
		Last Modified: Thu, 10 Sep 2020 02:30:33 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08513f3fdf1df7d6009039c5aae413fe16ee6ce6e40bae44f8d5e0b7bd3c8d38`  
		Last Modified: Thu, 10 Sep 2020 02:30:33 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1` - linux; mips64le

```console
$ docker pull memcached@sha256:7c1d3db9aa8a2c9947716b781c9ddc8c4d99e4a48318d3da3bfb2d9d5a553469
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.7 MB (28735881 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a7ac2f3081105bab353608116b822d5ff33be4e865e3e0f0e9f310c2953057b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 10 Sep 2020 00:10:03 GMT
ADD file:dec5e74bd1dacf4dd26507ac5227dfca6591d05d13bdf06c16217b9efff06ed9 in / 
# Thu, 10 Sep 2020 00:10:04 GMT
CMD ["bash"]
# Tue, 15 Sep 2020 03:17:09 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 15 Sep 2020 03:17:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Sep 2020 03:17:21 GMT
ENV MEMCACHED_VERSION=1.6.7
# Tue, 15 Sep 2020 03:17:22 GMT
ENV MEMCACHED_SHA1=49336bb0a4b7ad296422b08148581ed54edf32d0
# Wed, 23 Sep 2020 18:18:56 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 23 Sep 2020 18:18:56 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 23 Sep 2020 18:18:58 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 23 Sep 2020 18:18:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 23 Sep 2020 18:18:59 GMT
USER memcache
# Wed, 23 Sep 2020 18:18:59 GMT
EXPOSE 11211
# Wed, 23 Sep 2020 18:18:59 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:3e11c32dbce8eae675cead1f63aeade46d661eb3764bff6c26bb8ca6e2c364fb`  
		Last Modified: Tue, 15 Sep 2020 01:13:19 GMT  
		Size: 25.8 MB (25762660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88d32d437f1360c92791e6d1f0f490cc78c6209be1870bb6cb66b79c8349fa3d`  
		Last Modified: Wed, 23 Sep 2020 18:19:21 GMT  
		Size: 5.0 KB (4983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:592933aa8d3179edf056c3911fe15c0cf60587f931c74bc5d84b2f6de8d8992e`  
		Last Modified: Wed, 23 Sep 2020 18:19:23 GMT  
		Size: 1.8 MB (1776064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfb94ff2fdc8d15ea207ebec0799b92feeefb4d3334a38c2cd1758d3609dc5b2`  
		Last Modified: Wed, 23 Sep 2020 18:19:23 GMT  
		Size: 1.2 MB (1191765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84ce46a0757ebb411e71d3d59a7c40edbb368b2bdf9472df7da0b18d4f9e0e1a`  
		Last Modified: Wed, 23 Sep 2020 18:19:21 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05dae55a53383b9643fd68465eebc790642fae4074c8b49f937d8b424544c3da`  
		Last Modified: Wed, 23 Sep 2020 18:19:22 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1` - linux; ppc64le

```console
$ docker pull memcached@sha256:9ee0904c2a1eff337f8886c5f9e74a92462f156abb0996c09a7343c80b89a502
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.1 MB (34071624 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d5ce8ca6190b2a43e92824fa399c7fc498dc96544f6edbc45dc40562588828d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 10 Sep 2020 01:06:11 GMT
ADD file:4dede556abae88027bd22f3166fdbc38778a6fcd686c5ce768c3ca024ab3f9cf in / 
# Thu, 10 Sep 2020 01:06:20 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 21:27:40 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Thu, 10 Sep 2020 21:28:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 21:28:09 GMT
ENV MEMCACHED_VERSION=1.6.7
# Thu, 10 Sep 2020 21:28:13 GMT
ENV MEMCACHED_SHA1=49336bb0a4b7ad296422b08148581ed54edf32d0
# Thu, 10 Sep 2020 21:44:40 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 10 Sep 2020 21:44:45 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 10 Sep 2020 21:45:03 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 10 Sep 2020 21:45:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 10 Sep 2020 21:45:16 GMT
USER memcache
# Thu, 10 Sep 2020 21:45:25 GMT
EXPOSE 11211
# Thu, 10 Sep 2020 21:45:31 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:f8aef3d2247e5f990bc767bc99f575b9bcec34aaa37183414eebe28fcd09519d`  
		Last Modified: Thu, 10 Sep 2020 01:28:12 GMT  
		Size: 30.5 MB (30517880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5b7bfeb11b26b80e3f45ddc9eec4e6fa55c578fd1b3735b718e666cb5c661d6`  
		Last Modified: Thu, 10 Sep 2020 21:46:03 GMT  
		Size: 5.0 KB (4988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb81e5357148bb530b5afccd9a6fc7b05010564b011024db6515763ef71c0ce3`  
		Last Modified: Thu, 10 Sep 2020 21:46:03 GMT  
		Size: 2.3 MB (2322772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f5a11e72f2a67deedc2e0a4af04f9fcda2aa1cbd833ef8985418eec3ec2f63e`  
		Last Modified: Thu, 10 Sep 2020 21:46:03 GMT  
		Size: 1.2 MB (1225576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0f3a0aafd05b076f9f6cca15b1674c60464d9c1074391b796ad515cb20b29c4`  
		Last Modified: Thu, 10 Sep 2020 21:46:03 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffa12800e0545bdcc70841732b77e97c7d1eb18ae0d7cf28a25035eca507e057`  
		Last Modified: Thu, 10 Sep 2020 21:46:03 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1` - linux; s390x

```console
$ docker pull memcached@sha256:29246fb608029daf71e59f2826a30d3d1228bfff1e261abdf8e8a6742d558e56
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.8 MB (28789171 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:81a42318833ed3d53d0befe80a053c5f038b58886994eb98f10deab18a17df83`
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
# Tue, 13 Oct 2020 02:44:47 GMT
ENV MEMCACHED_VERSION=1.6.7
# Tue, 13 Oct 2020 02:44:48 GMT
ENV MEMCACHED_SHA1=49336bb0a4b7ad296422b08148581ed54edf32d0
# Tue, 13 Oct 2020 02:54:05 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 13 Oct 2020 02:54:06 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 13 Oct 2020 02:54:07 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 13 Oct 2020 02:54:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Oct 2020 02:54:07 GMT
USER memcache
# Tue, 13 Oct 2020 02:54:07 GMT
EXPOSE 11211
# Tue, 13 Oct 2020 02:54:07 GMT
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
	-	`sha256:cc4afc3e1ed06ea6037b98689f0536544ca7d61153a60fdc589230648e2a984e`  
		Last Modified: Tue, 13 Oct 2020 02:54:35 GMT  
		Size: 1.2 MB (1190100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f259c385180086733d453c3eaeee6fac1efecc084bd34815bf58421ae8fc0e40`  
		Last Modified: Tue, 13 Oct 2020 02:54:35 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98288868e61d43041bb2178e9722e20e72849b117eaa0cbd7cb92d981147f652`  
		Last Modified: Tue, 13 Oct 2020 02:54:35 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:1.6`

```console
$ docker pull memcached@sha256:d999887e1fbd1ae9c6209459ae28ee0477c034b40ab2c6b492aa6a3dd3a3f564
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
$ docker pull memcached@sha256:7b8d8fbef4feb9386884d0aa2ecd3912aa62f2ec26efea54a57bc8fcf78348b6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.5 MB (30493470 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b4920487992d3dbbe4aa89a7336e06600ab8b41fe8f889212e927f7fbb19593`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 10 Sep 2020 00:23:29 GMT
ADD file:e7407f2294ad23634565820b9669b18ff2a2ca0212a7ec84b9c89d8550859954 in / 
# Thu, 10 Sep 2020 00:23:30 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 06:42:10 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Thu, 10 Sep 2020 06:42:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 06:42:17 GMT
ENV MEMCACHED_VERSION=1.6.7
# Thu, 10 Sep 2020 06:42:18 GMT
ENV MEMCACHED_SHA1=49336bb0a4b7ad296422b08148581ed54edf32d0
# Thu, 10 Sep 2020 06:52:26 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 10 Sep 2020 06:52:26 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 10 Sep 2020 06:52:28 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 10 Sep 2020 06:52:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 10 Sep 2020 06:52:28 GMT
USER memcache
# Thu, 10 Sep 2020 06:52:29 GMT
EXPOSE 11211
# Thu, 10 Sep 2020 06:52:29 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:d121f8d1c4128ebc1e95e5bfad90a0189b84eadbbb2fbaad20cbb26d20b2c8a2`  
		Last Modified: Thu, 10 Sep 2020 00:34:02 GMT  
		Size: 27.1 MB (27092161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd29e75844e2246d981d63970769902be264bae0990bb5befc493e5d15eeeeb3`  
		Last Modified: Thu, 10 Sep 2020 06:52:50 GMT  
		Size: 5.0 KB (4980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1adbe52eab585d7464430faaab2b3f8759b1661558262688357dba99e6967db7`  
		Last Modified: Thu, 10 Sep 2020 06:52:50 GMT  
		Size: 2.2 MB (2196512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e7563db9f0d12fba4b16ab48ba07e143239fc53283b76b6532d09a26ed523e8`  
		Last Modified: Thu, 10 Sep 2020 06:52:50 GMT  
		Size: 1.2 MB (1199409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1018860c7c78773f11445b24c799624ebf7ad0c1a54955ee73a0d1fdf7eeb40`  
		Last Modified: Thu, 10 Sep 2020 06:52:50 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b02cff55081f0c25f0ae11f642177cfec21627dce0ad4f9593653f121d8a2297`  
		Last Modified: Thu, 10 Sep 2020 06:52:50 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6` - linux; arm variant v5

```console
$ docker pull memcached@sha256:db8e75930e7350dc06c594abc4f6eb130088c7a803729f2125820e48992c5e60
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.9 MB (27911252 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ca29ad8c51e933907ffd5cacfd7b034a533f7b15c99c2202743dd723b229f5a3`
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
# Tue, 13 Oct 2020 02:23:01 GMT
ENV MEMCACHED_VERSION=1.6.7
# Tue, 13 Oct 2020 02:23:02 GMT
ENV MEMCACHED_SHA1=49336bb0a4b7ad296422b08148581ed54edf32d0
# Tue, 13 Oct 2020 02:33:45 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 13 Oct 2020 02:33:46 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 13 Oct 2020 02:33:51 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 13 Oct 2020 02:33:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Oct 2020 02:33:53 GMT
USER memcache
# Tue, 13 Oct 2020 02:33:55 GMT
EXPOSE 11211
# Tue, 13 Oct 2020 02:33:57 GMT
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
	-	`sha256:85530c3b6a178a04b529523c2bf5e513e04d7a42f2cdebf26a69b484b56a68e2`  
		Last Modified: Tue, 13 Oct 2020 02:34:18 GMT  
		Size: 1.2 MB (1173125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38d48859b3d5f2dfe3a0ddff8417717ec4274b5d7431850f3434a35d856c8326`  
		Last Modified: Tue, 13 Oct 2020 02:34:18 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84b665bad50ddd6ddfcf2dc2cc9e826499da002347faf18378e77a3dc6f81505`  
		Last Modified: Tue, 13 Oct 2020 02:34:18 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6` - linux; arm variant v7

```console
$ docker pull memcached@sha256:534ab9a71bfdbc6306e5f0e66af8fe0f76bc509560817621b7e31c9dc7f94ac7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.7 MB (25660617 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ef1c3640e673dfff34704d898b5bb45aa552e63246457eb196726184a948b0a7`
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
# Tue, 13 Oct 2020 04:26:30 GMT
ENV MEMCACHED_VERSION=1.6.7
# Tue, 13 Oct 2020 04:26:31 GMT
ENV MEMCACHED_SHA1=49336bb0a4b7ad296422b08148581ed54edf32d0
# Tue, 13 Oct 2020 04:36:50 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 13 Oct 2020 04:36:51 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 13 Oct 2020 04:36:54 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 13 Oct 2020 04:36:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Oct 2020 04:36:56 GMT
USER memcache
# Tue, 13 Oct 2020 04:36:57 GMT
EXPOSE 11211
# Tue, 13 Oct 2020 04:36:57 GMT
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
	-	`sha256:d50f05a1d5be98ec50a0b9c6b32e28b0673ad3db35c5b90500b0a38cd1697589`  
		Last Modified: Tue, 13 Oct 2020 04:37:30 GMT  
		Size: 1.1 MB (1143928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a0ff448c0efd0905dc11c59b70feb4dd6cd02adda52ec427fa68bd0664cf165`  
		Last Modified: Tue, 13 Oct 2020 04:37:29 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c8559eb111bdc28303506d117e61bb26e47daa128d7fdb057bace4acaeeb1c4`  
		Last Modified: Tue, 13 Oct 2020 04:37:29 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:7f9d722d816e4b63c87642fde2b901849b416838b47ab197bb52a4bec0ca01b6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.1 MB (29099929 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ea99cfec94c49c44ccb283458d9addd82f2763524a936bf3962202eecbe4e74`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 09 Sep 2020 23:50:54 GMT
ADD file:d870fb0484ea283840d9cc923c9c3fe36d1bb6b3b5ecfefcce06aa26a22c9414 in / 
# Wed, 09 Sep 2020 23:50:57 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 04:21:07 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Thu, 10 Sep 2020 04:21:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 04:21:19 GMT
ENV MEMCACHED_VERSION=1.6.7
# Thu, 10 Sep 2020 04:21:20 GMT
ENV MEMCACHED_SHA1=49336bb0a4b7ad296422b08148581ed54edf32d0
# Thu, 10 Sep 2020 04:31:42 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 10 Sep 2020 04:31:43 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 10 Sep 2020 04:31:45 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 10 Sep 2020 04:31:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 10 Sep 2020 04:31:46 GMT
USER memcache
# Thu, 10 Sep 2020 04:31:47 GMT
EXPOSE 11211
# Thu, 10 Sep 2020 04:31:48 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:a6d76de28f58f3470aff71c934c0fec4e5d0fad788f8b8bcc50601266fc1b34d`  
		Last Modified: Wed, 09 Sep 2020 23:59:09 GMT  
		Size: 25.8 MB (25849325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4f48bd1f465fe61c5d378a72dea86a5917d8ec222d9eda27c13d06a0388ce45`  
		Last Modified: Thu, 10 Sep 2020 04:32:19 GMT  
		Size: 5.0 KB (5023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6172eb8b991d9ee34cce4d10ae2d0a18036999e58977cb193f2493dba1d0922d`  
		Last Modified: Thu, 10 Sep 2020 04:32:19 GMT  
		Size: 2.1 MB (2075014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c4390371d3044be59e120ad4ac5e0ab67b9eaacd1a1fd97388724d7ffe5a5d8`  
		Last Modified: Thu, 10 Sep 2020 04:32:19 GMT  
		Size: 1.2 MB (1170159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8212b808878005bf5387d12077984b9fd4f2c6127c29515d63fbaabb572648a0`  
		Last Modified: Thu, 10 Sep 2020 04:32:19 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6dd274731a18972c07fee896065b96cd0d476de9b6a13ea57e0a1577e762d14`  
		Last Modified: Thu, 10 Sep 2020 04:32:18 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6` - linux; 386

```console
$ docker pull memcached@sha256:0fb71355a775a0f518e405710c83cff1d60dd0fddf7bb066ec19ce5c98ecb1fe
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.2 MB (31161216 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c69f202ca7e7d00a1d7deb0fdf47bda4a4fc3d57af1ee1e2d39e3e9eb7196ba`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 09 Sep 2020 23:40:19 GMT
ADD file:08dc20c9cd727ebf02cac6e4b287c3009274682174aee9222494491cd6c671b8 in / 
# Wed, 09 Sep 2020 23:40:19 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 02:19:41 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Thu, 10 Sep 2020 02:19:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 02:19:51 GMT
ENV MEMCACHED_VERSION=1.6.7
# Thu, 10 Sep 2020 02:19:52 GMT
ENV MEMCACHED_SHA1=49336bb0a4b7ad296422b08148581ed54edf32d0
# Thu, 10 Sep 2020 02:30:13 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 10 Sep 2020 02:30:13 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 10 Sep 2020 02:30:14 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 10 Sep 2020 02:30:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 10 Sep 2020 02:30:14 GMT
USER memcache
# Thu, 10 Sep 2020 02:30:15 GMT
EXPOSE 11211
# Thu, 10 Sep 2020 02:30:15 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:31e6582dbd9f9a84903d46339df0c393a63d2cbfb001b06b3204653cceafcc61`  
		Last Modified: Wed, 09 Sep 2020 23:46:30 GMT  
		Size: 27.8 MB (27750334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:096b2a6b5e34ad8c96b35f52e3615e85902d5b12f7bdbf4f984988b59ba14ac3`  
		Last Modified: Thu, 10 Sep 2020 02:30:33 GMT  
		Size: 4.9 KB (4895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ece6f6a2e1723d610af9b172d870ab4c9e6e3c132f316e5f7baa2787806fbae6`  
		Last Modified: Thu, 10 Sep 2020 02:30:33 GMT  
		Size: 2.2 MB (2208153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3df397ec8999490a45ed35ff7908dacec384cecced47533e490dd01de7e4a320`  
		Last Modified: Thu, 10 Sep 2020 02:30:34 GMT  
		Size: 1.2 MB (1197426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:debebc596e2e5ea23dca7e24bc712d7ed9942d1db2397c4140b12ce8af1ce21f`  
		Last Modified: Thu, 10 Sep 2020 02:30:33 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08513f3fdf1df7d6009039c5aae413fe16ee6ce6e40bae44f8d5e0b7bd3c8d38`  
		Last Modified: Thu, 10 Sep 2020 02:30:33 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6` - linux; mips64le

```console
$ docker pull memcached@sha256:7c1d3db9aa8a2c9947716b781c9ddc8c4d99e4a48318d3da3bfb2d9d5a553469
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.7 MB (28735881 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a7ac2f3081105bab353608116b822d5ff33be4e865e3e0f0e9f310c2953057b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 10 Sep 2020 00:10:03 GMT
ADD file:dec5e74bd1dacf4dd26507ac5227dfca6591d05d13bdf06c16217b9efff06ed9 in / 
# Thu, 10 Sep 2020 00:10:04 GMT
CMD ["bash"]
# Tue, 15 Sep 2020 03:17:09 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 15 Sep 2020 03:17:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Sep 2020 03:17:21 GMT
ENV MEMCACHED_VERSION=1.6.7
# Tue, 15 Sep 2020 03:17:22 GMT
ENV MEMCACHED_SHA1=49336bb0a4b7ad296422b08148581ed54edf32d0
# Wed, 23 Sep 2020 18:18:56 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 23 Sep 2020 18:18:56 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 23 Sep 2020 18:18:58 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 23 Sep 2020 18:18:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 23 Sep 2020 18:18:59 GMT
USER memcache
# Wed, 23 Sep 2020 18:18:59 GMT
EXPOSE 11211
# Wed, 23 Sep 2020 18:18:59 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:3e11c32dbce8eae675cead1f63aeade46d661eb3764bff6c26bb8ca6e2c364fb`  
		Last Modified: Tue, 15 Sep 2020 01:13:19 GMT  
		Size: 25.8 MB (25762660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88d32d437f1360c92791e6d1f0f490cc78c6209be1870bb6cb66b79c8349fa3d`  
		Last Modified: Wed, 23 Sep 2020 18:19:21 GMT  
		Size: 5.0 KB (4983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:592933aa8d3179edf056c3911fe15c0cf60587f931c74bc5d84b2f6de8d8992e`  
		Last Modified: Wed, 23 Sep 2020 18:19:23 GMT  
		Size: 1.8 MB (1776064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfb94ff2fdc8d15ea207ebec0799b92feeefb4d3334a38c2cd1758d3609dc5b2`  
		Last Modified: Wed, 23 Sep 2020 18:19:23 GMT  
		Size: 1.2 MB (1191765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84ce46a0757ebb411e71d3d59a7c40edbb368b2bdf9472df7da0b18d4f9e0e1a`  
		Last Modified: Wed, 23 Sep 2020 18:19:21 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05dae55a53383b9643fd68465eebc790642fae4074c8b49f937d8b424544c3da`  
		Last Modified: Wed, 23 Sep 2020 18:19:22 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6` - linux; ppc64le

```console
$ docker pull memcached@sha256:9ee0904c2a1eff337f8886c5f9e74a92462f156abb0996c09a7343c80b89a502
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.1 MB (34071624 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d5ce8ca6190b2a43e92824fa399c7fc498dc96544f6edbc45dc40562588828d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 10 Sep 2020 01:06:11 GMT
ADD file:4dede556abae88027bd22f3166fdbc38778a6fcd686c5ce768c3ca024ab3f9cf in / 
# Thu, 10 Sep 2020 01:06:20 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 21:27:40 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Thu, 10 Sep 2020 21:28:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 21:28:09 GMT
ENV MEMCACHED_VERSION=1.6.7
# Thu, 10 Sep 2020 21:28:13 GMT
ENV MEMCACHED_SHA1=49336bb0a4b7ad296422b08148581ed54edf32d0
# Thu, 10 Sep 2020 21:44:40 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 10 Sep 2020 21:44:45 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 10 Sep 2020 21:45:03 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 10 Sep 2020 21:45:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 10 Sep 2020 21:45:16 GMT
USER memcache
# Thu, 10 Sep 2020 21:45:25 GMT
EXPOSE 11211
# Thu, 10 Sep 2020 21:45:31 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:f8aef3d2247e5f990bc767bc99f575b9bcec34aaa37183414eebe28fcd09519d`  
		Last Modified: Thu, 10 Sep 2020 01:28:12 GMT  
		Size: 30.5 MB (30517880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5b7bfeb11b26b80e3f45ddc9eec4e6fa55c578fd1b3735b718e666cb5c661d6`  
		Last Modified: Thu, 10 Sep 2020 21:46:03 GMT  
		Size: 5.0 KB (4988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb81e5357148bb530b5afccd9a6fc7b05010564b011024db6515763ef71c0ce3`  
		Last Modified: Thu, 10 Sep 2020 21:46:03 GMT  
		Size: 2.3 MB (2322772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f5a11e72f2a67deedc2e0a4af04f9fcda2aa1cbd833ef8985418eec3ec2f63e`  
		Last Modified: Thu, 10 Sep 2020 21:46:03 GMT  
		Size: 1.2 MB (1225576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0f3a0aafd05b076f9f6cca15b1674c60464d9c1074391b796ad515cb20b29c4`  
		Last Modified: Thu, 10 Sep 2020 21:46:03 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffa12800e0545bdcc70841732b77e97c7d1eb18ae0d7cf28a25035eca507e057`  
		Last Modified: Thu, 10 Sep 2020 21:46:03 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6` - linux; s390x

```console
$ docker pull memcached@sha256:29246fb608029daf71e59f2826a30d3d1228bfff1e261abdf8e8a6742d558e56
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.8 MB (28789171 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:81a42318833ed3d53d0befe80a053c5f038b58886994eb98f10deab18a17df83`
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
# Tue, 13 Oct 2020 02:44:47 GMT
ENV MEMCACHED_VERSION=1.6.7
# Tue, 13 Oct 2020 02:44:48 GMT
ENV MEMCACHED_SHA1=49336bb0a4b7ad296422b08148581ed54edf32d0
# Tue, 13 Oct 2020 02:54:05 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 13 Oct 2020 02:54:06 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 13 Oct 2020 02:54:07 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 13 Oct 2020 02:54:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Oct 2020 02:54:07 GMT
USER memcache
# Tue, 13 Oct 2020 02:54:07 GMT
EXPOSE 11211
# Tue, 13 Oct 2020 02:54:07 GMT
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
	-	`sha256:cc4afc3e1ed06ea6037b98689f0536544ca7d61153a60fdc589230648e2a984e`  
		Last Modified: Tue, 13 Oct 2020 02:54:35 GMT  
		Size: 1.2 MB (1190100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f259c385180086733d453c3eaeee6fac1efecc084bd34815bf58421ae8fc0e40`  
		Last Modified: Tue, 13 Oct 2020 02:54:35 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98288868e61d43041bb2178e9722e20e72849b117eaa0cbd7cb92d981147f652`  
		Last Modified: Tue, 13 Oct 2020 02:54:35 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:1.6.7`

```console
$ docker pull memcached@sha256:d999887e1fbd1ae9c6209459ae28ee0477c034b40ab2c6b492aa6a3dd3a3f564
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

### `memcached:1.6.7` - linux; amd64

```console
$ docker pull memcached@sha256:7b8d8fbef4feb9386884d0aa2ecd3912aa62f2ec26efea54a57bc8fcf78348b6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.5 MB (30493470 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b4920487992d3dbbe4aa89a7336e06600ab8b41fe8f889212e927f7fbb19593`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 10 Sep 2020 00:23:29 GMT
ADD file:e7407f2294ad23634565820b9669b18ff2a2ca0212a7ec84b9c89d8550859954 in / 
# Thu, 10 Sep 2020 00:23:30 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 06:42:10 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Thu, 10 Sep 2020 06:42:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 06:42:17 GMT
ENV MEMCACHED_VERSION=1.6.7
# Thu, 10 Sep 2020 06:42:18 GMT
ENV MEMCACHED_SHA1=49336bb0a4b7ad296422b08148581ed54edf32d0
# Thu, 10 Sep 2020 06:52:26 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 10 Sep 2020 06:52:26 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 10 Sep 2020 06:52:28 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 10 Sep 2020 06:52:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 10 Sep 2020 06:52:28 GMT
USER memcache
# Thu, 10 Sep 2020 06:52:29 GMT
EXPOSE 11211
# Thu, 10 Sep 2020 06:52:29 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:d121f8d1c4128ebc1e95e5bfad90a0189b84eadbbb2fbaad20cbb26d20b2c8a2`  
		Last Modified: Thu, 10 Sep 2020 00:34:02 GMT  
		Size: 27.1 MB (27092161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd29e75844e2246d981d63970769902be264bae0990bb5befc493e5d15eeeeb3`  
		Last Modified: Thu, 10 Sep 2020 06:52:50 GMT  
		Size: 5.0 KB (4980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1adbe52eab585d7464430faaab2b3f8759b1661558262688357dba99e6967db7`  
		Last Modified: Thu, 10 Sep 2020 06:52:50 GMT  
		Size: 2.2 MB (2196512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e7563db9f0d12fba4b16ab48ba07e143239fc53283b76b6532d09a26ed523e8`  
		Last Modified: Thu, 10 Sep 2020 06:52:50 GMT  
		Size: 1.2 MB (1199409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1018860c7c78773f11445b24c799624ebf7ad0c1a54955ee73a0d1fdf7eeb40`  
		Last Modified: Thu, 10 Sep 2020 06:52:50 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b02cff55081f0c25f0ae11f642177cfec21627dce0ad4f9593653f121d8a2297`  
		Last Modified: Thu, 10 Sep 2020 06:52:50 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.7` - linux; arm variant v5

```console
$ docker pull memcached@sha256:db8e75930e7350dc06c594abc4f6eb130088c7a803729f2125820e48992c5e60
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.9 MB (27911252 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ca29ad8c51e933907ffd5cacfd7b034a533f7b15c99c2202743dd723b229f5a3`
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
# Tue, 13 Oct 2020 02:23:01 GMT
ENV MEMCACHED_VERSION=1.6.7
# Tue, 13 Oct 2020 02:23:02 GMT
ENV MEMCACHED_SHA1=49336bb0a4b7ad296422b08148581ed54edf32d0
# Tue, 13 Oct 2020 02:33:45 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 13 Oct 2020 02:33:46 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 13 Oct 2020 02:33:51 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 13 Oct 2020 02:33:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Oct 2020 02:33:53 GMT
USER memcache
# Tue, 13 Oct 2020 02:33:55 GMT
EXPOSE 11211
# Tue, 13 Oct 2020 02:33:57 GMT
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
	-	`sha256:85530c3b6a178a04b529523c2bf5e513e04d7a42f2cdebf26a69b484b56a68e2`  
		Last Modified: Tue, 13 Oct 2020 02:34:18 GMT  
		Size: 1.2 MB (1173125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38d48859b3d5f2dfe3a0ddff8417717ec4274b5d7431850f3434a35d856c8326`  
		Last Modified: Tue, 13 Oct 2020 02:34:18 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84b665bad50ddd6ddfcf2dc2cc9e826499da002347faf18378e77a3dc6f81505`  
		Last Modified: Tue, 13 Oct 2020 02:34:18 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.7` - linux; arm variant v7

```console
$ docker pull memcached@sha256:534ab9a71bfdbc6306e5f0e66af8fe0f76bc509560817621b7e31c9dc7f94ac7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.7 MB (25660617 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ef1c3640e673dfff34704d898b5bb45aa552e63246457eb196726184a948b0a7`
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
# Tue, 13 Oct 2020 04:26:30 GMT
ENV MEMCACHED_VERSION=1.6.7
# Tue, 13 Oct 2020 04:26:31 GMT
ENV MEMCACHED_SHA1=49336bb0a4b7ad296422b08148581ed54edf32d0
# Tue, 13 Oct 2020 04:36:50 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 13 Oct 2020 04:36:51 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 13 Oct 2020 04:36:54 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 13 Oct 2020 04:36:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Oct 2020 04:36:56 GMT
USER memcache
# Tue, 13 Oct 2020 04:36:57 GMT
EXPOSE 11211
# Tue, 13 Oct 2020 04:36:57 GMT
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
	-	`sha256:d50f05a1d5be98ec50a0b9c6b32e28b0673ad3db35c5b90500b0a38cd1697589`  
		Last Modified: Tue, 13 Oct 2020 04:37:30 GMT  
		Size: 1.1 MB (1143928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a0ff448c0efd0905dc11c59b70feb4dd6cd02adda52ec427fa68bd0664cf165`  
		Last Modified: Tue, 13 Oct 2020 04:37:29 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c8559eb111bdc28303506d117e61bb26e47daa128d7fdb057bace4acaeeb1c4`  
		Last Modified: Tue, 13 Oct 2020 04:37:29 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.7` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:7f9d722d816e4b63c87642fde2b901849b416838b47ab197bb52a4bec0ca01b6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.1 MB (29099929 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ea99cfec94c49c44ccb283458d9addd82f2763524a936bf3962202eecbe4e74`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 09 Sep 2020 23:50:54 GMT
ADD file:d870fb0484ea283840d9cc923c9c3fe36d1bb6b3b5ecfefcce06aa26a22c9414 in / 
# Wed, 09 Sep 2020 23:50:57 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 04:21:07 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Thu, 10 Sep 2020 04:21:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 04:21:19 GMT
ENV MEMCACHED_VERSION=1.6.7
# Thu, 10 Sep 2020 04:21:20 GMT
ENV MEMCACHED_SHA1=49336bb0a4b7ad296422b08148581ed54edf32d0
# Thu, 10 Sep 2020 04:31:42 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 10 Sep 2020 04:31:43 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 10 Sep 2020 04:31:45 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 10 Sep 2020 04:31:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 10 Sep 2020 04:31:46 GMT
USER memcache
# Thu, 10 Sep 2020 04:31:47 GMT
EXPOSE 11211
# Thu, 10 Sep 2020 04:31:48 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:a6d76de28f58f3470aff71c934c0fec4e5d0fad788f8b8bcc50601266fc1b34d`  
		Last Modified: Wed, 09 Sep 2020 23:59:09 GMT  
		Size: 25.8 MB (25849325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4f48bd1f465fe61c5d378a72dea86a5917d8ec222d9eda27c13d06a0388ce45`  
		Last Modified: Thu, 10 Sep 2020 04:32:19 GMT  
		Size: 5.0 KB (5023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6172eb8b991d9ee34cce4d10ae2d0a18036999e58977cb193f2493dba1d0922d`  
		Last Modified: Thu, 10 Sep 2020 04:32:19 GMT  
		Size: 2.1 MB (2075014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c4390371d3044be59e120ad4ac5e0ab67b9eaacd1a1fd97388724d7ffe5a5d8`  
		Last Modified: Thu, 10 Sep 2020 04:32:19 GMT  
		Size: 1.2 MB (1170159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8212b808878005bf5387d12077984b9fd4f2c6127c29515d63fbaabb572648a0`  
		Last Modified: Thu, 10 Sep 2020 04:32:19 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6dd274731a18972c07fee896065b96cd0d476de9b6a13ea57e0a1577e762d14`  
		Last Modified: Thu, 10 Sep 2020 04:32:18 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.7` - linux; 386

```console
$ docker pull memcached@sha256:0fb71355a775a0f518e405710c83cff1d60dd0fddf7bb066ec19ce5c98ecb1fe
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.2 MB (31161216 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c69f202ca7e7d00a1d7deb0fdf47bda4a4fc3d57af1ee1e2d39e3e9eb7196ba`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 09 Sep 2020 23:40:19 GMT
ADD file:08dc20c9cd727ebf02cac6e4b287c3009274682174aee9222494491cd6c671b8 in / 
# Wed, 09 Sep 2020 23:40:19 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 02:19:41 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Thu, 10 Sep 2020 02:19:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 02:19:51 GMT
ENV MEMCACHED_VERSION=1.6.7
# Thu, 10 Sep 2020 02:19:52 GMT
ENV MEMCACHED_SHA1=49336bb0a4b7ad296422b08148581ed54edf32d0
# Thu, 10 Sep 2020 02:30:13 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 10 Sep 2020 02:30:13 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 10 Sep 2020 02:30:14 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 10 Sep 2020 02:30:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 10 Sep 2020 02:30:14 GMT
USER memcache
# Thu, 10 Sep 2020 02:30:15 GMT
EXPOSE 11211
# Thu, 10 Sep 2020 02:30:15 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:31e6582dbd9f9a84903d46339df0c393a63d2cbfb001b06b3204653cceafcc61`  
		Last Modified: Wed, 09 Sep 2020 23:46:30 GMT  
		Size: 27.8 MB (27750334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:096b2a6b5e34ad8c96b35f52e3615e85902d5b12f7bdbf4f984988b59ba14ac3`  
		Last Modified: Thu, 10 Sep 2020 02:30:33 GMT  
		Size: 4.9 KB (4895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ece6f6a2e1723d610af9b172d870ab4c9e6e3c132f316e5f7baa2787806fbae6`  
		Last Modified: Thu, 10 Sep 2020 02:30:33 GMT  
		Size: 2.2 MB (2208153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3df397ec8999490a45ed35ff7908dacec384cecced47533e490dd01de7e4a320`  
		Last Modified: Thu, 10 Sep 2020 02:30:34 GMT  
		Size: 1.2 MB (1197426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:debebc596e2e5ea23dca7e24bc712d7ed9942d1db2397c4140b12ce8af1ce21f`  
		Last Modified: Thu, 10 Sep 2020 02:30:33 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08513f3fdf1df7d6009039c5aae413fe16ee6ce6e40bae44f8d5e0b7bd3c8d38`  
		Last Modified: Thu, 10 Sep 2020 02:30:33 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.7` - linux; mips64le

```console
$ docker pull memcached@sha256:7c1d3db9aa8a2c9947716b781c9ddc8c4d99e4a48318d3da3bfb2d9d5a553469
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.7 MB (28735881 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a7ac2f3081105bab353608116b822d5ff33be4e865e3e0f0e9f310c2953057b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 10 Sep 2020 00:10:03 GMT
ADD file:dec5e74bd1dacf4dd26507ac5227dfca6591d05d13bdf06c16217b9efff06ed9 in / 
# Thu, 10 Sep 2020 00:10:04 GMT
CMD ["bash"]
# Tue, 15 Sep 2020 03:17:09 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 15 Sep 2020 03:17:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Sep 2020 03:17:21 GMT
ENV MEMCACHED_VERSION=1.6.7
# Tue, 15 Sep 2020 03:17:22 GMT
ENV MEMCACHED_SHA1=49336bb0a4b7ad296422b08148581ed54edf32d0
# Wed, 23 Sep 2020 18:18:56 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 23 Sep 2020 18:18:56 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 23 Sep 2020 18:18:58 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 23 Sep 2020 18:18:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 23 Sep 2020 18:18:59 GMT
USER memcache
# Wed, 23 Sep 2020 18:18:59 GMT
EXPOSE 11211
# Wed, 23 Sep 2020 18:18:59 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:3e11c32dbce8eae675cead1f63aeade46d661eb3764bff6c26bb8ca6e2c364fb`  
		Last Modified: Tue, 15 Sep 2020 01:13:19 GMT  
		Size: 25.8 MB (25762660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88d32d437f1360c92791e6d1f0f490cc78c6209be1870bb6cb66b79c8349fa3d`  
		Last Modified: Wed, 23 Sep 2020 18:19:21 GMT  
		Size: 5.0 KB (4983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:592933aa8d3179edf056c3911fe15c0cf60587f931c74bc5d84b2f6de8d8992e`  
		Last Modified: Wed, 23 Sep 2020 18:19:23 GMT  
		Size: 1.8 MB (1776064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfb94ff2fdc8d15ea207ebec0799b92feeefb4d3334a38c2cd1758d3609dc5b2`  
		Last Modified: Wed, 23 Sep 2020 18:19:23 GMT  
		Size: 1.2 MB (1191765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84ce46a0757ebb411e71d3d59a7c40edbb368b2bdf9472df7da0b18d4f9e0e1a`  
		Last Modified: Wed, 23 Sep 2020 18:19:21 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05dae55a53383b9643fd68465eebc790642fae4074c8b49f937d8b424544c3da`  
		Last Modified: Wed, 23 Sep 2020 18:19:22 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.7` - linux; ppc64le

```console
$ docker pull memcached@sha256:9ee0904c2a1eff337f8886c5f9e74a92462f156abb0996c09a7343c80b89a502
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.1 MB (34071624 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d5ce8ca6190b2a43e92824fa399c7fc498dc96544f6edbc45dc40562588828d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 10 Sep 2020 01:06:11 GMT
ADD file:4dede556abae88027bd22f3166fdbc38778a6fcd686c5ce768c3ca024ab3f9cf in / 
# Thu, 10 Sep 2020 01:06:20 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 21:27:40 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Thu, 10 Sep 2020 21:28:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 21:28:09 GMT
ENV MEMCACHED_VERSION=1.6.7
# Thu, 10 Sep 2020 21:28:13 GMT
ENV MEMCACHED_SHA1=49336bb0a4b7ad296422b08148581ed54edf32d0
# Thu, 10 Sep 2020 21:44:40 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 10 Sep 2020 21:44:45 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 10 Sep 2020 21:45:03 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 10 Sep 2020 21:45:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 10 Sep 2020 21:45:16 GMT
USER memcache
# Thu, 10 Sep 2020 21:45:25 GMT
EXPOSE 11211
# Thu, 10 Sep 2020 21:45:31 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:f8aef3d2247e5f990bc767bc99f575b9bcec34aaa37183414eebe28fcd09519d`  
		Last Modified: Thu, 10 Sep 2020 01:28:12 GMT  
		Size: 30.5 MB (30517880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5b7bfeb11b26b80e3f45ddc9eec4e6fa55c578fd1b3735b718e666cb5c661d6`  
		Last Modified: Thu, 10 Sep 2020 21:46:03 GMT  
		Size: 5.0 KB (4988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb81e5357148bb530b5afccd9a6fc7b05010564b011024db6515763ef71c0ce3`  
		Last Modified: Thu, 10 Sep 2020 21:46:03 GMT  
		Size: 2.3 MB (2322772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f5a11e72f2a67deedc2e0a4af04f9fcda2aa1cbd833ef8985418eec3ec2f63e`  
		Last Modified: Thu, 10 Sep 2020 21:46:03 GMT  
		Size: 1.2 MB (1225576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0f3a0aafd05b076f9f6cca15b1674c60464d9c1074391b796ad515cb20b29c4`  
		Last Modified: Thu, 10 Sep 2020 21:46:03 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffa12800e0545bdcc70841732b77e97c7d1eb18ae0d7cf28a25035eca507e057`  
		Last Modified: Thu, 10 Sep 2020 21:46:03 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.7` - linux; s390x

```console
$ docker pull memcached@sha256:29246fb608029daf71e59f2826a30d3d1228bfff1e261abdf8e8a6742d558e56
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.8 MB (28789171 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:81a42318833ed3d53d0befe80a053c5f038b58886994eb98f10deab18a17df83`
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
# Tue, 13 Oct 2020 02:44:47 GMT
ENV MEMCACHED_VERSION=1.6.7
# Tue, 13 Oct 2020 02:44:48 GMT
ENV MEMCACHED_SHA1=49336bb0a4b7ad296422b08148581ed54edf32d0
# Tue, 13 Oct 2020 02:54:05 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 13 Oct 2020 02:54:06 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 13 Oct 2020 02:54:07 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 13 Oct 2020 02:54:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Oct 2020 02:54:07 GMT
USER memcache
# Tue, 13 Oct 2020 02:54:07 GMT
EXPOSE 11211
# Tue, 13 Oct 2020 02:54:07 GMT
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
	-	`sha256:cc4afc3e1ed06ea6037b98689f0536544ca7d61153a60fdc589230648e2a984e`  
		Last Modified: Tue, 13 Oct 2020 02:54:35 GMT  
		Size: 1.2 MB (1190100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f259c385180086733d453c3eaeee6fac1efecc084bd34815bf58421ae8fc0e40`  
		Last Modified: Tue, 13 Oct 2020 02:54:35 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98288868e61d43041bb2178e9722e20e72849b117eaa0cbd7cb92d981147f652`  
		Last Modified: Tue, 13 Oct 2020 02:54:35 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:1.6.7-alpine`

```console
$ docker pull memcached@sha256:f082d96b17dcf912e5b0615995b3ab9ed28a400bbe095142e39f01d59edb1103
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

### `memcached:1.6.7-alpine` - linux; amd64

```console
$ docker pull memcached@sha256:77ccfc5250e116838ae941b40fe83fbd10af6b58fc3f424fc060d2c74366c41c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4879276 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:417903261a6412798128441638195daa0a1bd15e1f9ad3518ee56a36dc1f93cf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 29 May 2020 21:19:46 GMT
ADD file:c92c248239f8c7b9b3c067650954815f391b7bcb09023f984972c082ace2a8d0 in / 
# Fri, 29 May 2020 21:19:46 GMT
CMD ["/bin/sh"]
# Thu, 11 Jun 2020 22:36:17 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Thu, 11 Jun 2020 22:36:18 GMT
RUN apk add --no-cache cyrus-sasl-plain
# Tue, 08 Sep 2020 19:58:25 GMT
ENV MEMCACHED_VERSION=1.6.7
# Tue, 08 Sep 2020 19:58:25 GMT
ENV MEMCACHED_SHA1=49336bb0a4b7ad296422b08148581ed54edf32d0
# Tue, 08 Sep 2020 20:17:57 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		dpkg-dev dpkg 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		tar 		wget 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& make test 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 08 Sep 2020 20:17:57 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 08 Sep 2020 20:17:58 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 08 Sep 2020 20:17:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 08 Sep 2020 20:17:58 GMT
USER memcache
# Tue, 08 Sep 2020 20:17:58 GMT
EXPOSE 11211
# Tue, 08 Sep 2020 20:17:59 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:df20fa9351a15782c64e6dddb2d4a6f50bf6d3688060a34c4014b0d9a752eb4c`  
		Last Modified: Fri, 29 May 2020 21:20:06 GMT  
		Size: 2.8 MB (2797541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9da9e0d7f92826205e029bfd978a90f40bc6fdcf5e15730881f4c53893b6c958`  
		Last Modified: Thu, 11 Jun 2020 22:46:20 GMT  
		Size: 1.2 KB (1230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a01e9fc6969fb7eb8c18a96fbe204469f0c2a753cb2851e9a5b48cf1d42efe64`  
		Last Modified: Thu, 11 Jun 2020 22:46:20 GMT  
		Size: 15.3 KB (15282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:402843d6a42d73d92e4e046fbd68a7ede8e634f27d56cb74c4152d29374bfc2f`  
		Last Modified: Tue, 08 Sep 2020 20:18:20 GMT  
		Size: 2.1 MB (2064819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3cd9988120f5b64ce357a2f9d5bae7defaf23f26b29578f0ae3555f8ca44455`  
		Last Modified: Tue, 08 Sep 2020 20:18:20 GMT  
		Size: 283.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2c3f54b6a0ee5c03a5ef2c6ff819d1a12d4d4ca5761175c7c400ff9bb97a311`  
		Last Modified: Tue, 08 Sep 2020 20:18:21 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.7-alpine` - linux; arm variant v6

```console
$ docker pull memcached@sha256:e03f9bd4773341a508783efc5e0dba17a9261998261b9d0300d97462e146bee2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4642127 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:244b1d3b240c8fd5a4a082f45d2ccd20f11fdba80567329d0a85c178a8075685`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 29 May 2020 21:50:55 GMT
ADD file:f46e997a56849423db17e5fc9f0249ab6c73b155245927dba5fcb9dfd65f622f in / 
# Fri, 29 May 2020 21:50:56 GMT
CMD ["/bin/sh"]
# Thu, 11 Jun 2020 19:34:27 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Thu, 11 Jun 2020 19:34:30 GMT
RUN apk add --no-cache cyrus-sasl-plain
# Tue, 08 Sep 2020 20:37:05 GMT
ENV MEMCACHED_VERSION=1.6.7
# Tue, 08 Sep 2020 20:37:13 GMT
ENV MEMCACHED_SHA1=49336bb0a4b7ad296422b08148581ed54edf32d0
# Tue, 08 Sep 2020 20:48:32 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		dpkg-dev dpkg 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		tar 		wget 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& make test 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 08 Sep 2020 20:48:54 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 08 Sep 2020 20:49:25 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 08 Sep 2020 20:49:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 08 Sep 2020 20:49:40 GMT
USER memcache
# Tue, 08 Sep 2020 20:49:47 GMT
EXPOSE 11211
# Tue, 08 Sep 2020 20:49:58 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:b4b72e716706d29f5d2351709c20bf737b94f876a5472a43ff1b6e203c65d27f`  
		Last Modified: Fri, 29 May 2020 21:51:30 GMT  
		Size: 2.6 MB (2603286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07d7bd6b3b6044e07d261038778674ff772f8776c9aa1b04e2c00591dec9d4bb`  
		Last Modified: Thu, 11 Jun 2020 19:45:28 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b80a5ea355d8ff9191648d56b12825dd65d5e619a6c53da85eb7ae4853362c02`  
		Last Modified: Thu, 11 Jun 2020 19:45:29 GMT  
		Size: 14.9 KB (14890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:840a119db59d7756c10a241a3113f6701a7a2dea799799d894613615d101ab86`  
		Last Modified: Tue, 08 Sep 2020 20:50:20 GMT  
		Size: 2.0 MB (2022286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd3161efc183503e07c48bdc064b820190fba6381d49ae7db0066a5e5d999b71`  
		Last Modified: Tue, 08 Sep 2020 20:50:20 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55c40db22205f1918b380ed8a513eab7b73e185ce15693ddb907299c8cd870e7`  
		Last Modified: Tue, 08 Sep 2020 20:50:20 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.7-alpine` - linux; arm variant v7

```console
$ docker pull memcached@sha256:5df58dd4af8c4e69b2d0a71c6a35811934379c618fb3247d0d9b5cd726636c7a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.3 MB (4308981 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e4d85a2b8661ec592eaea28d949c858606735eedea931bad225bdfb76411a579`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 29 May 2020 21:02:07 GMT
ADD file:e97bf0d217846312b19a9f7264604851aedd125c23b4d291eed4c69b880dce26 in / 
# Fri, 29 May 2020 21:02:08 GMT
CMD ["/bin/sh"]
# Thu, 11 Jun 2020 20:31:56 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Thu, 11 Jun 2020 20:31:58 GMT
RUN apk add --no-cache cyrus-sasl-plain
# Tue, 08 Sep 2020 21:31:04 GMT
ENV MEMCACHED_VERSION=1.6.7
# Tue, 08 Sep 2020 21:31:19 GMT
ENV MEMCACHED_SHA1=49336bb0a4b7ad296422b08148581ed54edf32d0
# Tue, 08 Sep 2020 21:42:25 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		dpkg-dev dpkg 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		tar 		wget 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& make test 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 08 Sep 2020 21:42:40 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 08 Sep 2020 21:43:14 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 08 Sep 2020 21:43:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 08 Sep 2020 21:43:27 GMT
USER memcache
# Tue, 08 Sep 2020 21:43:36 GMT
EXPOSE 11211
# Tue, 08 Sep 2020 21:43:45 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:52278dd8e57993669c5b72a9620e89bebdc098f2af2379caaa8945f7403f77a2`  
		Last Modified: Fri, 29 May 2020 21:02:38 GMT  
		Size: 2.4 MB (2406763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a171a50ea23b122e85435c89187bf16a391efa7d74cb2d7aa6cb2c5555bc9830`  
		Last Modified: Thu, 11 Jun 2020 20:43:17 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac40655da815a69db31129873e9e388bba260ee4962ba15f288b81a58e580925`  
		Last Modified: Thu, 11 Jun 2020 20:43:17 GMT  
		Size: 13.8 KB (13821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fb21bd27680eb0bb3a12b0230902e6e669705c89eb00a40b1e447c724630aaf`  
		Last Modified: Tue, 08 Sep 2020 21:44:14 GMT  
		Size: 1.9 MB (1886732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f223b308518beca0559a433993f85b4839c01cc9bd99273e99ca85a41c2789e`  
		Last Modified: Tue, 08 Sep 2020 21:44:13 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c89f21f449a1fe14dd0743b953195690232696f7b71bff23bbbf37c513f58066`  
		Last Modified: Tue, 08 Sep 2020 21:44:13 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.7-alpine` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:0e93e6e8893fe1a57e9ff87a1be7549c1242a220f82728073537827606f866e6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.8 MB (4802209 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:488a4ea2a5396d38953aea7778aa7e954ad63581062a8a72b36db8a850cbe191`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 29 May 2020 21:43:19 GMT
ADD file:7574aee4e37a85460ab889212d52912723a9b30dda1c060548f0deb4a05fc398 in / 
# Fri, 29 May 2020 21:43:20 GMT
CMD ["/bin/sh"]
# Thu, 11 Jun 2020 20:42:19 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Thu, 11 Jun 2020 20:42:27 GMT
RUN apk add --no-cache cyrus-sasl-plain
# Tue, 08 Sep 2020 21:15:58 GMT
ENV MEMCACHED_VERSION=1.6.7
# Tue, 08 Sep 2020 21:16:03 GMT
ENV MEMCACHED_SHA1=49336bb0a4b7ad296422b08148581ed54edf32d0
# Tue, 08 Sep 2020 21:26:35 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		dpkg-dev dpkg 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		tar 		wget 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& make test 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 08 Sep 2020 21:26:36 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 08 Sep 2020 21:26:38 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 08 Sep 2020 21:26:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 08 Sep 2020 21:26:39 GMT
USER memcache
# Tue, 08 Sep 2020 21:26:40 GMT
EXPOSE 11211
# Tue, 08 Sep 2020 21:26:41 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:b538f80385f9b48122e3da068c932a96ea5018afa3c7be79da00437414bd18cd`  
		Last Modified: Fri, 29 May 2020 21:43:57 GMT  
		Size: 2.7 MB (2707964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f6b5a3ebcdb20348b01d4048b7bcffbdcfd27ef2e8bcf97439b88d285b162ca`  
		Last Modified: Thu, 11 Jun 2020 20:54:00 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abf62b7cec62367b3dbf8205df906d5380b0f60394a5688de6270734eddf59c0`  
		Last Modified: Thu, 11 Jun 2020 20:54:01 GMT  
		Size: 15.7 KB (15666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad7fdef1b41af486bfb55bb5ce24c78108a20b09265b270ff707cd7b40664d02`  
		Last Modified: Tue, 08 Sep 2020 21:27:16 GMT  
		Size: 2.1 MB (2076916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa6a7d33c013dbdf201db7eef507d048362838d8bca32018751d804d7cf6d858`  
		Last Modified: Tue, 08 Sep 2020 21:27:16 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9a5d51fa547f310e8cdb76975f971b87f0be63de169c68a9a00fb15249c8816`  
		Last Modified: Tue, 08 Sep 2020 21:27:16 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.7-alpine` - linux; 386

```console
$ docker pull memcached@sha256:31ca3704550a0170a48bc9d320b306102e484250edee144f9d10cc8a79ab0a35
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (4957953 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:20bed8fb2767398a969a48948babafcd8261b38a331c1d859e12fa3e02b1d690`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 29 May 2020 21:38:33 GMT
ADD file:5624441d97aca5eeb82a582941efc3586397098b8391227a9040ebe434cc1d6b in / 
# Fri, 29 May 2020 21:38:33 GMT
CMD ["/bin/sh"]
# Thu, 11 Jun 2020 22:34:33 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Thu, 11 Jun 2020 22:34:34 GMT
RUN apk add --no-cache cyrus-sasl-plain
# Tue, 08 Sep 2020 20:04:27 GMT
ENV MEMCACHED_VERSION=1.6.7
# Tue, 08 Sep 2020 20:04:27 GMT
ENV MEMCACHED_SHA1=49336bb0a4b7ad296422b08148581ed54edf32d0
# Tue, 08 Sep 2020 20:14:20 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		dpkg-dev dpkg 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		tar 		wget 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& make test 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 08 Sep 2020 20:14:20 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 08 Sep 2020 20:14:21 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 08 Sep 2020 20:14:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 08 Sep 2020 20:14:21 GMT
USER memcache
# Tue, 08 Sep 2020 20:14:21 GMT
EXPOSE 11211
# Tue, 08 Sep 2020 20:14:22 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:0625b4155e2a59f647ece47c0cd77ed3196b1f84454fa64ce80cad90e2b9b79e`  
		Last Modified: Fri, 29 May 2020 21:38:53 GMT  
		Size: 2.8 MB (2792298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:053753de6f049436417b1e2a50db73e47b194bd33f797965f6bd5f12c34f4d28`  
		Last Modified: Thu, 11 Jun 2020 22:45:05 GMT  
		Size: 1.2 KB (1231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a293d5635155e323f1e11070a6feb690a2ed40238b9414e2f73de5c4eb21cec3`  
		Last Modified: Thu, 11 Jun 2020 22:45:05 GMT  
		Size: 16.3 KB (16309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d116af020f9edc239ddd492a64b13b60061a8d942d7f8a5e50ef6d21cea4803`  
		Last Modified: Tue, 08 Sep 2020 20:14:44 GMT  
		Size: 2.1 MB (2147710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28f73fb0898406ab5a318c68e66c7ea0282aba028135fe34d3a87d0b04e5f3a6`  
		Last Modified: Tue, 08 Sep 2020 20:14:44 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4284ab01f9851d348bfb5c221d20faba538766b47ec8954ea6cb4b699414998b`  
		Last Modified: Tue, 08 Sep 2020 20:14:44 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.7-alpine` - linux; ppc64le

```console
$ docker pull memcached@sha256:d6751a0596f3ebfb78a0b9f5b10cb4f89485f57f293ae2f4fe29e471ed064eb0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (4954591 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e88c6bbffd1d20b19a59c6e8601d47d463f9e447d017b589f1d8fb9056cdaa8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 29 May 2020 21:23:03 GMT
ADD file:8194808a812370fd2202d80d1667f851bd9eac4c560d69d347fe1964f54343de in / 
# Fri, 29 May 2020 21:23:06 GMT
CMD ["/bin/sh"]
# Thu, 11 Jun 2020 21:28:54 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Thu, 11 Jun 2020 21:29:00 GMT
RUN apk add --no-cache cyrus-sasl-plain
# Tue, 08 Sep 2020 21:02:42 GMT
ENV MEMCACHED_VERSION=1.6.7
# Tue, 08 Sep 2020 21:02:47 GMT
ENV MEMCACHED_SHA1=49336bb0a4b7ad296422b08148581ed54edf32d0
# Tue, 08 Sep 2020 21:12:56 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		dpkg-dev dpkg 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		tar 		wget 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& make test 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 08 Sep 2020 21:12:58 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 08 Sep 2020 21:13:07 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 08 Sep 2020 21:13:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 08 Sep 2020 21:13:15 GMT
USER memcache
# Tue, 08 Sep 2020 21:13:18 GMT
EXPOSE 11211
# Tue, 08 Sep 2020 21:13:21 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:5077f8601dceb5744d875d7740ebc203f674b108a0188f3a31e292b21a4bee64`  
		Last Modified: Fri, 29 May 2020 21:23:37 GMT  
		Size: 2.8 MB (2805199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5da85732ec2c118da92b83669225af1d8b16986733a33a75401b712da2ed1510`  
		Last Modified: Thu, 11 Jun 2020 21:40:05 GMT  
		Size: 1.3 KB (1265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e466bec4d365b2c3064b6a41b20a28dd25fc8648c778f467d7ffd2fca60fce67`  
		Last Modified: Thu, 11 Jun 2020 21:40:05 GMT  
		Size: 16.3 KB (16307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5de324c8b5732e45731bcd408805025e0067d6eb99f5d3a4bc018d3a24c5773`  
		Last Modified: Tue, 08 Sep 2020 21:14:07 GMT  
		Size: 2.1 MB (2131416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6251901b79919688b1fc772326877a528474bb9f6c82f715f029287cf22d2ba3`  
		Last Modified: Tue, 08 Sep 2020 21:14:06 GMT  
		Size: 283.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c67a15198fb6666781fd4ced69393d50c0c09ee6bf766e4c0be6a9915d37e80`  
		Last Modified: Tue, 08 Sep 2020 21:14:06 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.7-alpine` - linux; s390x

```console
$ docker pull memcached@sha256:ac57a3b53de45bfc54993bc36ffd2939b18467759b501bb4f7ef850a86e1a632
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4667972 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0d148284ba37411d02418001c76b7df11b95cc18de4cb0a94545ed2f9d16f1b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 29 May 2020 21:41:39 GMT
ADD file:9799ce3b2f782a28e10b1846cd9b3db827fa99c9bc601feb268456195856814e in / 
# Fri, 29 May 2020 21:41:39 GMT
CMD ["/bin/sh"]
# Thu, 11 Jun 2020 19:41:31 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Thu, 11 Jun 2020 19:41:32 GMT
RUN apk add --no-cache cyrus-sasl-plain
# Tue, 08 Sep 2020 20:05:33 GMT
ENV MEMCACHED_VERSION=1.6.7
# Tue, 08 Sep 2020 20:05:33 GMT
ENV MEMCACHED_SHA1=49336bb0a4b7ad296422b08148581ed54edf32d0
# Tue, 08 Sep 2020 20:14:30 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		dpkg-dev dpkg 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		tar 		wget 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& make test 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 08 Sep 2020 20:14:30 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 08 Sep 2020 20:14:31 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 08 Sep 2020 20:14:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 08 Sep 2020 20:14:31 GMT
USER memcache
# Tue, 08 Sep 2020 20:14:31 GMT
EXPOSE 11211
# Tue, 08 Sep 2020 20:14:31 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:8fb3d41b2e9a59630b51745f257cd2561f96bcd15cf309fcc20120d5fcee8c5b`  
		Last Modified: Fri, 29 May 2020 21:42:03 GMT  
		Size: 2.6 MB (2566189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:844417c2ac824247320ce09147386405c59cd97101ff0d7cdbb939d961eaa2b7`  
		Last Modified: Thu, 11 Jun 2020 19:51:23 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83365eb9bbed49c8b8705426f527c5cace2db28af3c362b07f7edb2a54081b74`  
		Last Modified: Thu, 11 Jun 2020 19:51:23 GMT  
		Size: 15.5 KB (15547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5611c53be4f0d770a1e13e22e4960ce69780ddba187630f7e7b1a734220086f4`  
		Last Modified: Tue, 08 Sep 2020 20:14:55 GMT  
		Size: 2.1 MB (2084574 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe21c4e263557f5a3dc7dd4b9fe6d53fafb6735b7a8adba33498dc66c975f1b3`  
		Last Modified: Tue, 08 Sep 2020 20:14:55 GMT  
		Size: 283.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e86dc35f36a362c5f02870203ead9db5268d33ab3cfa6dc2c103a5365eca7a2`  
		Last Modified: Tue, 08 Sep 2020 20:14:55 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:1.6-alpine`

```console
$ docker pull memcached@sha256:f082d96b17dcf912e5b0615995b3ab9ed28a400bbe095142e39f01d59edb1103
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
$ docker pull memcached@sha256:77ccfc5250e116838ae941b40fe83fbd10af6b58fc3f424fc060d2c74366c41c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4879276 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:417903261a6412798128441638195daa0a1bd15e1f9ad3518ee56a36dc1f93cf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 29 May 2020 21:19:46 GMT
ADD file:c92c248239f8c7b9b3c067650954815f391b7bcb09023f984972c082ace2a8d0 in / 
# Fri, 29 May 2020 21:19:46 GMT
CMD ["/bin/sh"]
# Thu, 11 Jun 2020 22:36:17 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Thu, 11 Jun 2020 22:36:18 GMT
RUN apk add --no-cache cyrus-sasl-plain
# Tue, 08 Sep 2020 19:58:25 GMT
ENV MEMCACHED_VERSION=1.6.7
# Tue, 08 Sep 2020 19:58:25 GMT
ENV MEMCACHED_SHA1=49336bb0a4b7ad296422b08148581ed54edf32d0
# Tue, 08 Sep 2020 20:17:57 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		dpkg-dev dpkg 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		tar 		wget 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& make test 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 08 Sep 2020 20:17:57 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 08 Sep 2020 20:17:58 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 08 Sep 2020 20:17:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 08 Sep 2020 20:17:58 GMT
USER memcache
# Tue, 08 Sep 2020 20:17:58 GMT
EXPOSE 11211
# Tue, 08 Sep 2020 20:17:59 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:df20fa9351a15782c64e6dddb2d4a6f50bf6d3688060a34c4014b0d9a752eb4c`  
		Last Modified: Fri, 29 May 2020 21:20:06 GMT  
		Size: 2.8 MB (2797541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9da9e0d7f92826205e029bfd978a90f40bc6fdcf5e15730881f4c53893b6c958`  
		Last Modified: Thu, 11 Jun 2020 22:46:20 GMT  
		Size: 1.2 KB (1230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a01e9fc6969fb7eb8c18a96fbe204469f0c2a753cb2851e9a5b48cf1d42efe64`  
		Last Modified: Thu, 11 Jun 2020 22:46:20 GMT  
		Size: 15.3 KB (15282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:402843d6a42d73d92e4e046fbd68a7ede8e634f27d56cb74c4152d29374bfc2f`  
		Last Modified: Tue, 08 Sep 2020 20:18:20 GMT  
		Size: 2.1 MB (2064819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3cd9988120f5b64ce357a2f9d5bae7defaf23f26b29578f0ae3555f8ca44455`  
		Last Modified: Tue, 08 Sep 2020 20:18:20 GMT  
		Size: 283.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2c3f54b6a0ee5c03a5ef2c6ff819d1a12d4d4ca5761175c7c400ff9bb97a311`  
		Last Modified: Tue, 08 Sep 2020 20:18:21 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-alpine` - linux; arm variant v6

```console
$ docker pull memcached@sha256:e03f9bd4773341a508783efc5e0dba17a9261998261b9d0300d97462e146bee2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4642127 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:244b1d3b240c8fd5a4a082f45d2ccd20f11fdba80567329d0a85c178a8075685`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 29 May 2020 21:50:55 GMT
ADD file:f46e997a56849423db17e5fc9f0249ab6c73b155245927dba5fcb9dfd65f622f in / 
# Fri, 29 May 2020 21:50:56 GMT
CMD ["/bin/sh"]
# Thu, 11 Jun 2020 19:34:27 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Thu, 11 Jun 2020 19:34:30 GMT
RUN apk add --no-cache cyrus-sasl-plain
# Tue, 08 Sep 2020 20:37:05 GMT
ENV MEMCACHED_VERSION=1.6.7
# Tue, 08 Sep 2020 20:37:13 GMT
ENV MEMCACHED_SHA1=49336bb0a4b7ad296422b08148581ed54edf32d0
# Tue, 08 Sep 2020 20:48:32 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		dpkg-dev dpkg 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		tar 		wget 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& make test 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 08 Sep 2020 20:48:54 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 08 Sep 2020 20:49:25 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 08 Sep 2020 20:49:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 08 Sep 2020 20:49:40 GMT
USER memcache
# Tue, 08 Sep 2020 20:49:47 GMT
EXPOSE 11211
# Tue, 08 Sep 2020 20:49:58 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:b4b72e716706d29f5d2351709c20bf737b94f876a5472a43ff1b6e203c65d27f`  
		Last Modified: Fri, 29 May 2020 21:51:30 GMT  
		Size: 2.6 MB (2603286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07d7bd6b3b6044e07d261038778674ff772f8776c9aa1b04e2c00591dec9d4bb`  
		Last Modified: Thu, 11 Jun 2020 19:45:28 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b80a5ea355d8ff9191648d56b12825dd65d5e619a6c53da85eb7ae4853362c02`  
		Last Modified: Thu, 11 Jun 2020 19:45:29 GMT  
		Size: 14.9 KB (14890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:840a119db59d7756c10a241a3113f6701a7a2dea799799d894613615d101ab86`  
		Last Modified: Tue, 08 Sep 2020 20:50:20 GMT  
		Size: 2.0 MB (2022286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd3161efc183503e07c48bdc064b820190fba6381d49ae7db0066a5e5d999b71`  
		Last Modified: Tue, 08 Sep 2020 20:50:20 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55c40db22205f1918b380ed8a513eab7b73e185ce15693ddb907299c8cd870e7`  
		Last Modified: Tue, 08 Sep 2020 20:50:20 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-alpine` - linux; arm variant v7

```console
$ docker pull memcached@sha256:5df58dd4af8c4e69b2d0a71c6a35811934379c618fb3247d0d9b5cd726636c7a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.3 MB (4308981 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e4d85a2b8661ec592eaea28d949c858606735eedea931bad225bdfb76411a579`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 29 May 2020 21:02:07 GMT
ADD file:e97bf0d217846312b19a9f7264604851aedd125c23b4d291eed4c69b880dce26 in / 
# Fri, 29 May 2020 21:02:08 GMT
CMD ["/bin/sh"]
# Thu, 11 Jun 2020 20:31:56 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Thu, 11 Jun 2020 20:31:58 GMT
RUN apk add --no-cache cyrus-sasl-plain
# Tue, 08 Sep 2020 21:31:04 GMT
ENV MEMCACHED_VERSION=1.6.7
# Tue, 08 Sep 2020 21:31:19 GMT
ENV MEMCACHED_SHA1=49336bb0a4b7ad296422b08148581ed54edf32d0
# Tue, 08 Sep 2020 21:42:25 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		dpkg-dev dpkg 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		tar 		wget 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& make test 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 08 Sep 2020 21:42:40 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 08 Sep 2020 21:43:14 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 08 Sep 2020 21:43:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 08 Sep 2020 21:43:27 GMT
USER memcache
# Tue, 08 Sep 2020 21:43:36 GMT
EXPOSE 11211
# Tue, 08 Sep 2020 21:43:45 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:52278dd8e57993669c5b72a9620e89bebdc098f2af2379caaa8945f7403f77a2`  
		Last Modified: Fri, 29 May 2020 21:02:38 GMT  
		Size: 2.4 MB (2406763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a171a50ea23b122e85435c89187bf16a391efa7d74cb2d7aa6cb2c5555bc9830`  
		Last Modified: Thu, 11 Jun 2020 20:43:17 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac40655da815a69db31129873e9e388bba260ee4962ba15f288b81a58e580925`  
		Last Modified: Thu, 11 Jun 2020 20:43:17 GMT  
		Size: 13.8 KB (13821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fb21bd27680eb0bb3a12b0230902e6e669705c89eb00a40b1e447c724630aaf`  
		Last Modified: Tue, 08 Sep 2020 21:44:14 GMT  
		Size: 1.9 MB (1886732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f223b308518beca0559a433993f85b4839c01cc9bd99273e99ca85a41c2789e`  
		Last Modified: Tue, 08 Sep 2020 21:44:13 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c89f21f449a1fe14dd0743b953195690232696f7b71bff23bbbf37c513f58066`  
		Last Modified: Tue, 08 Sep 2020 21:44:13 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-alpine` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:0e93e6e8893fe1a57e9ff87a1be7549c1242a220f82728073537827606f866e6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.8 MB (4802209 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:488a4ea2a5396d38953aea7778aa7e954ad63581062a8a72b36db8a850cbe191`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 29 May 2020 21:43:19 GMT
ADD file:7574aee4e37a85460ab889212d52912723a9b30dda1c060548f0deb4a05fc398 in / 
# Fri, 29 May 2020 21:43:20 GMT
CMD ["/bin/sh"]
# Thu, 11 Jun 2020 20:42:19 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Thu, 11 Jun 2020 20:42:27 GMT
RUN apk add --no-cache cyrus-sasl-plain
# Tue, 08 Sep 2020 21:15:58 GMT
ENV MEMCACHED_VERSION=1.6.7
# Tue, 08 Sep 2020 21:16:03 GMT
ENV MEMCACHED_SHA1=49336bb0a4b7ad296422b08148581ed54edf32d0
# Tue, 08 Sep 2020 21:26:35 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		dpkg-dev dpkg 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		tar 		wget 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& make test 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 08 Sep 2020 21:26:36 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 08 Sep 2020 21:26:38 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 08 Sep 2020 21:26:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 08 Sep 2020 21:26:39 GMT
USER memcache
# Tue, 08 Sep 2020 21:26:40 GMT
EXPOSE 11211
# Tue, 08 Sep 2020 21:26:41 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:b538f80385f9b48122e3da068c932a96ea5018afa3c7be79da00437414bd18cd`  
		Last Modified: Fri, 29 May 2020 21:43:57 GMT  
		Size: 2.7 MB (2707964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f6b5a3ebcdb20348b01d4048b7bcffbdcfd27ef2e8bcf97439b88d285b162ca`  
		Last Modified: Thu, 11 Jun 2020 20:54:00 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abf62b7cec62367b3dbf8205df906d5380b0f60394a5688de6270734eddf59c0`  
		Last Modified: Thu, 11 Jun 2020 20:54:01 GMT  
		Size: 15.7 KB (15666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad7fdef1b41af486bfb55bb5ce24c78108a20b09265b270ff707cd7b40664d02`  
		Last Modified: Tue, 08 Sep 2020 21:27:16 GMT  
		Size: 2.1 MB (2076916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa6a7d33c013dbdf201db7eef507d048362838d8bca32018751d804d7cf6d858`  
		Last Modified: Tue, 08 Sep 2020 21:27:16 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9a5d51fa547f310e8cdb76975f971b87f0be63de169c68a9a00fb15249c8816`  
		Last Modified: Tue, 08 Sep 2020 21:27:16 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-alpine` - linux; 386

```console
$ docker pull memcached@sha256:31ca3704550a0170a48bc9d320b306102e484250edee144f9d10cc8a79ab0a35
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (4957953 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:20bed8fb2767398a969a48948babafcd8261b38a331c1d859e12fa3e02b1d690`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 29 May 2020 21:38:33 GMT
ADD file:5624441d97aca5eeb82a582941efc3586397098b8391227a9040ebe434cc1d6b in / 
# Fri, 29 May 2020 21:38:33 GMT
CMD ["/bin/sh"]
# Thu, 11 Jun 2020 22:34:33 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Thu, 11 Jun 2020 22:34:34 GMT
RUN apk add --no-cache cyrus-sasl-plain
# Tue, 08 Sep 2020 20:04:27 GMT
ENV MEMCACHED_VERSION=1.6.7
# Tue, 08 Sep 2020 20:04:27 GMT
ENV MEMCACHED_SHA1=49336bb0a4b7ad296422b08148581ed54edf32d0
# Tue, 08 Sep 2020 20:14:20 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		dpkg-dev dpkg 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		tar 		wget 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& make test 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 08 Sep 2020 20:14:20 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 08 Sep 2020 20:14:21 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 08 Sep 2020 20:14:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 08 Sep 2020 20:14:21 GMT
USER memcache
# Tue, 08 Sep 2020 20:14:21 GMT
EXPOSE 11211
# Tue, 08 Sep 2020 20:14:22 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:0625b4155e2a59f647ece47c0cd77ed3196b1f84454fa64ce80cad90e2b9b79e`  
		Last Modified: Fri, 29 May 2020 21:38:53 GMT  
		Size: 2.8 MB (2792298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:053753de6f049436417b1e2a50db73e47b194bd33f797965f6bd5f12c34f4d28`  
		Last Modified: Thu, 11 Jun 2020 22:45:05 GMT  
		Size: 1.2 KB (1231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a293d5635155e323f1e11070a6feb690a2ed40238b9414e2f73de5c4eb21cec3`  
		Last Modified: Thu, 11 Jun 2020 22:45:05 GMT  
		Size: 16.3 KB (16309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d116af020f9edc239ddd492a64b13b60061a8d942d7f8a5e50ef6d21cea4803`  
		Last Modified: Tue, 08 Sep 2020 20:14:44 GMT  
		Size: 2.1 MB (2147710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28f73fb0898406ab5a318c68e66c7ea0282aba028135fe34d3a87d0b04e5f3a6`  
		Last Modified: Tue, 08 Sep 2020 20:14:44 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4284ab01f9851d348bfb5c221d20faba538766b47ec8954ea6cb4b699414998b`  
		Last Modified: Tue, 08 Sep 2020 20:14:44 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-alpine` - linux; ppc64le

```console
$ docker pull memcached@sha256:d6751a0596f3ebfb78a0b9f5b10cb4f89485f57f293ae2f4fe29e471ed064eb0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (4954591 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e88c6bbffd1d20b19a59c6e8601d47d463f9e447d017b589f1d8fb9056cdaa8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 29 May 2020 21:23:03 GMT
ADD file:8194808a812370fd2202d80d1667f851bd9eac4c560d69d347fe1964f54343de in / 
# Fri, 29 May 2020 21:23:06 GMT
CMD ["/bin/sh"]
# Thu, 11 Jun 2020 21:28:54 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Thu, 11 Jun 2020 21:29:00 GMT
RUN apk add --no-cache cyrus-sasl-plain
# Tue, 08 Sep 2020 21:02:42 GMT
ENV MEMCACHED_VERSION=1.6.7
# Tue, 08 Sep 2020 21:02:47 GMT
ENV MEMCACHED_SHA1=49336bb0a4b7ad296422b08148581ed54edf32d0
# Tue, 08 Sep 2020 21:12:56 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		dpkg-dev dpkg 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		tar 		wget 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& make test 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 08 Sep 2020 21:12:58 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 08 Sep 2020 21:13:07 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 08 Sep 2020 21:13:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 08 Sep 2020 21:13:15 GMT
USER memcache
# Tue, 08 Sep 2020 21:13:18 GMT
EXPOSE 11211
# Tue, 08 Sep 2020 21:13:21 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:5077f8601dceb5744d875d7740ebc203f674b108a0188f3a31e292b21a4bee64`  
		Last Modified: Fri, 29 May 2020 21:23:37 GMT  
		Size: 2.8 MB (2805199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5da85732ec2c118da92b83669225af1d8b16986733a33a75401b712da2ed1510`  
		Last Modified: Thu, 11 Jun 2020 21:40:05 GMT  
		Size: 1.3 KB (1265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e466bec4d365b2c3064b6a41b20a28dd25fc8648c778f467d7ffd2fca60fce67`  
		Last Modified: Thu, 11 Jun 2020 21:40:05 GMT  
		Size: 16.3 KB (16307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5de324c8b5732e45731bcd408805025e0067d6eb99f5d3a4bc018d3a24c5773`  
		Last Modified: Tue, 08 Sep 2020 21:14:07 GMT  
		Size: 2.1 MB (2131416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6251901b79919688b1fc772326877a528474bb9f6c82f715f029287cf22d2ba3`  
		Last Modified: Tue, 08 Sep 2020 21:14:06 GMT  
		Size: 283.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c67a15198fb6666781fd4ced69393d50c0c09ee6bf766e4c0be6a9915d37e80`  
		Last Modified: Tue, 08 Sep 2020 21:14:06 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-alpine` - linux; s390x

```console
$ docker pull memcached@sha256:ac57a3b53de45bfc54993bc36ffd2939b18467759b501bb4f7ef850a86e1a632
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4667972 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0d148284ba37411d02418001c76b7df11b95cc18de4cb0a94545ed2f9d16f1b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 29 May 2020 21:41:39 GMT
ADD file:9799ce3b2f782a28e10b1846cd9b3db827fa99c9bc601feb268456195856814e in / 
# Fri, 29 May 2020 21:41:39 GMT
CMD ["/bin/sh"]
# Thu, 11 Jun 2020 19:41:31 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Thu, 11 Jun 2020 19:41:32 GMT
RUN apk add --no-cache cyrus-sasl-plain
# Tue, 08 Sep 2020 20:05:33 GMT
ENV MEMCACHED_VERSION=1.6.7
# Tue, 08 Sep 2020 20:05:33 GMT
ENV MEMCACHED_SHA1=49336bb0a4b7ad296422b08148581ed54edf32d0
# Tue, 08 Sep 2020 20:14:30 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		dpkg-dev dpkg 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		tar 		wget 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& make test 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 08 Sep 2020 20:14:30 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 08 Sep 2020 20:14:31 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 08 Sep 2020 20:14:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 08 Sep 2020 20:14:31 GMT
USER memcache
# Tue, 08 Sep 2020 20:14:31 GMT
EXPOSE 11211
# Tue, 08 Sep 2020 20:14:31 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:8fb3d41b2e9a59630b51745f257cd2561f96bcd15cf309fcc20120d5fcee8c5b`  
		Last Modified: Fri, 29 May 2020 21:42:03 GMT  
		Size: 2.6 MB (2566189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:844417c2ac824247320ce09147386405c59cd97101ff0d7cdbb939d961eaa2b7`  
		Last Modified: Thu, 11 Jun 2020 19:51:23 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83365eb9bbed49c8b8705426f527c5cace2db28af3c362b07f7edb2a54081b74`  
		Last Modified: Thu, 11 Jun 2020 19:51:23 GMT  
		Size: 15.5 KB (15547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5611c53be4f0d770a1e13e22e4960ce69780ddba187630f7e7b1a734220086f4`  
		Last Modified: Tue, 08 Sep 2020 20:14:55 GMT  
		Size: 2.1 MB (2084574 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe21c4e263557f5a3dc7dd4b9fe6d53fafb6735b7a8adba33498dc66c975f1b3`  
		Last Modified: Tue, 08 Sep 2020 20:14:55 GMT  
		Size: 283.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e86dc35f36a362c5f02870203ead9db5268d33ab3cfa6dc2c103a5365eca7a2`  
		Last Modified: Tue, 08 Sep 2020 20:14:55 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:1-alpine`

```console
$ docker pull memcached@sha256:f082d96b17dcf912e5b0615995b3ab9ed28a400bbe095142e39f01d59edb1103
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
$ docker pull memcached@sha256:77ccfc5250e116838ae941b40fe83fbd10af6b58fc3f424fc060d2c74366c41c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4879276 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:417903261a6412798128441638195daa0a1bd15e1f9ad3518ee56a36dc1f93cf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 29 May 2020 21:19:46 GMT
ADD file:c92c248239f8c7b9b3c067650954815f391b7bcb09023f984972c082ace2a8d0 in / 
# Fri, 29 May 2020 21:19:46 GMT
CMD ["/bin/sh"]
# Thu, 11 Jun 2020 22:36:17 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Thu, 11 Jun 2020 22:36:18 GMT
RUN apk add --no-cache cyrus-sasl-plain
# Tue, 08 Sep 2020 19:58:25 GMT
ENV MEMCACHED_VERSION=1.6.7
# Tue, 08 Sep 2020 19:58:25 GMT
ENV MEMCACHED_SHA1=49336bb0a4b7ad296422b08148581ed54edf32d0
# Tue, 08 Sep 2020 20:17:57 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		dpkg-dev dpkg 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		tar 		wget 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& make test 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 08 Sep 2020 20:17:57 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 08 Sep 2020 20:17:58 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 08 Sep 2020 20:17:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 08 Sep 2020 20:17:58 GMT
USER memcache
# Tue, 08 Sep 2020 20:17:58 GMT
EXPOSE 11211
# Tue, 08 Sep 2020 20:17:59 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:df20fa9351a15782c64e6dddb2d4a6f50bf6d3688060a34c4014b0d9a752eb4c`  
		Last Modified: Fri, 29 May 2020 21:20:06 GMT  
		Size: 2.8 MB (2797541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9da9e0d7f92826205e029bfd978a90f40bc6fdcf5e15730881f4c53893b6c958`  
		Last Modified: Thu, 11 Jun 2020 22:46:20 GMT  
		Size: 1.2 KB (1230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a01e9fc6969fb7eb8c18a96fbe204469f0c2a753cb2851e9a5b48cf1d42efe64`  
		Last Modified: Thu, 11 Jun 2020 22:46:20 GMT  
		Size: 15.3 KB (15282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:402843d6a42d73d92e4e046fbd68a7ede8e634f27d56cb74c4152d29374bfc2f`  
		Last Modified: Tue, 08 Sep 2020 20:18:20 GMT  
		Size: 2.1 MB (2064819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3cd9988120f5b64ce357a2f9d5bae7defaf23f26b29578f0ae3555f8ca44455`  
		Last Modified: Tue, 08 Sep 2020 20:18:20 GMT  
		Size: 283.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2c3f54b6a0ee5c03a5ef2c6ff819d1a12d4d4ca5761175c7c400ff9bb97a311`  
		Last Modified: Tue, 08 Sep 2020 20:18:21 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-alpine` - linux; arm variant v6

```console
$ docker pull memcached@sha256:e03f9bd4773341a508783efc5e0dba17a9261998261b9d0300d97462e146bee2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4642127 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:244b1d3b240c8fd5a4a082f45d2ccd20f11fdba80567329d0a85c178a8075685`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 29 May 2020 21:50:55 GMT
ADD file:f46e997a56849423db17e5fc9f0249ab6c73b155245927dba5fcb9dfd65f622f in / 
# Fri, 29 May 2020 21:50:56 GMT
CMD ["/bin/sh"]
# Thu, 11 Jun 2020 19:34:27 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Thu, 11 Jun 2020 19:34:30 GMT
RUN apk add --no-cache cyrus-sasl-plain
# Tue, 08 Sep 2020 20:37:05 GMT
ENV MEMCACHED_VERSION=1.6.7
# Tue, 08 Sep 2020 20:37:13 GMT
ENV MEMCACHED_SHA1=49336bb0a4b7ad296422b08148581ed54edf32d0
# Tue, 08 Sep 2020 20:48:32 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		dpkg-dev dpkg 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		tar 		wget 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& make test 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 08 Sep 2020 20:48:54 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 08 Sep 2020 20:49:25 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 08 Sep 2020 20:49:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 08 Sep 2020 20:49:40 GMT
USER memcache
# Tue, 08 Sep 2020 20:49:47 GMT
EXPOSE 11211
# Tue, 08 Sep 2020 20:49:58 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:b4b72e716706d29f5d2351709c20bf737b94f876a5472a43ff1b6e203c65d27f`  
		Last Modified: Fri, 29 May 2020 21:51:30 GMT  
		Size: 2.6 MB (2603286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07d7bd6b3b6044e07d261038778674ff772f8776c9aa1b04e2c00591dec9d4bb`  
		Last Modified: Thu, 11 Jun 2020 19:45:28 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b80a5ea355d8ff9191648d56b12825dd65d5e619a6c53da85eb7ae4853362c02`  
		Last Modified: Thu, 11 Jun 2020 19:45:29 GMT  
		Size: 14.9 KB (14890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:840a119db59d7756c10a241a3113f6701a7a2dea799799d894613615d101ab86`  
		Last Modified: Tue, 08 Sep 2020 20:50:20 GMT  
		Size: 2.0 MB (2022286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd3161efc183503e07c48bdc064b820190fba6381d49ae7db0066a5e5d999b71`  
		Last Modified: Tue, 08 Sep 2020 20:50:20 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55c40db22205f1918b380ed8a513eab7b73e185ce15693ddb907299c8cd870e7`  
		Last Modified: Tue, 08 Sep 2020 20:50:20 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-alpine` - linux; arm variant v7

```console
$ docker pull memcached@sha256:5df58dd4af8c4e69b2d0a71c6a35811934379c618fb3247d0d9b5cd726636c7a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.3 MB (4308981 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e4d85a2b8661ec592eaea28d949c858606735eedea931bad225bdfb76411a579`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 29 May 2020 21:02:07 GMT
ADD file:e97bf0d217846312b19a9f7264604851aedd125c23b4d291eed4c69b880dce26 in / 
# Fri, 29 May 2020 21:02:08 GMT
CMD ["/bin/sh"]
# Thu, 11 Jun 2020 20:31:56 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Thu, 11 Jun 2020 20:31:58 GMT
RUN apk add --no-cache cyrus-sasl-plain
# Tue, 08 Sep 2020 21:31:04 GMT
ENV MEMCACHED_VERSION=1.6.7
# Tue, 08 Sep 2020 21:31:19 GMT
ENV MEMCACHED_SHA1=49336bb0a4b7ad296422b08148581ed54edf32d0
# Tue, 08 Sep 2020 21:42:25 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		dpkg-dev dpkg 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		tar 		wget 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& make test 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 08 Sep 2020 21:42:40 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 08 Sep 2020 21:43:14 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 08 Sep 2020 21:43:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 08 Sep 2020 21:43:27 GMT
USER memcache
# Tue, 08 Sep 2020 21:43:36 GMT
EXPOSE 11211
# Tue, 08 Sep 2020 21:43:45 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:52278dd8e57993669c5b72a9620e89bebdc098f2af2379caaa8945f7403f77a2`  
		Last Modified: Fri, 29 May 2020 21:02:38 GMT  
		Size: 2.4 MB (2406763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a171a50ea23b122e85435c89187bf16a391efa7d74cb2d7aa6cb2c5555bc9830`  
		Last Modified: Thu, 11 Jun 2020 20:43:17 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac40655da815a69db31129873e9e388bba260ee4962ba15f288b81a58e580925`  
		Last Modified: Thu, 11 Jun 2020 20:43:17 GMT  
		Size: 13.8 KB (13821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fb21bd27680eb0bb3a12b0230902e6e669705c89eb00a40b1e447c724630aaf`  
		Last Modified: Tue, 08 Sep 2020 21:44:14 GMT  
		Size: 1.9 MB (1886732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f223b308518beca0559a433993f85b4839c01cc9bd99273e99ca85a41c2789e`  
		Last Modified: Tue, 08 Sep 2020 21:44:13 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c89f21f449a1fe14dd0743b953195690232696f7b71bff23bbbf37c513f58066`  
		Last Modified: Tue, 08 Sep 2020 21:44:13 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-alpine` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:0e93e6e8893fe1a57e9ff87a1be7549c1242a220f82728073537827606f866e6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.8 MB (4802209 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:488a4ea2a5396d38953aea7778aa7e954ad63581062a8a72b36db8a850cbe191`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 29 May 2020 21:43:19 GMT
ADD file:7574aee4e37a85460ab889212d52912723a9b30dda1c060548f0deb4a05fc398 in / 
# Fri, 29 May 2020 21:43:20 GMT
CMD ["/bin/sh"]
# Thu, 11 Jun 2020 20:42:19 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Thu, 11 Jun 2020 20:42:27 GMT
RUN apk add --no-cache cyrus-sasl-plain
# Tue, 08 Sep 2020 21:15:58 GMT
ENV MEMCACHED_VERSION=1.6.7
# Tue, 08 Sep 2020 21:16:03 GMT
ENV MEMCACHED_SHA1=49336bb0a4b7ad296422b08148581ed54edf32d0
# Tue, 08 Sep 2020 21:26:35 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		dpkg-dev dpkg 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		tar 		wget 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& make test 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 08 Sep 2020 21:26:36 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 08 Sep 2020 21:26:38 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 08 Sep 2020 21:26:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 08 Sep 2020 21:26:39 GMT
USER memcache
# Tue, 08 Sep 2020 21:26:40 GMT
EXPOSE 11211
# Tue, 08 Sep 2020 21:26:41 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:b538f80385f9b48122e3da068c932a96ea5018afa3c7be79da00437414bd18cd`  
		Last Modified: Fri, 29 May 2020 21:43:57 GMT  
		Size: 2.7 MB (2707964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f6b5a3ebcdb20348b01d4048b7bcffbdcfd27ef2e8bcf97439b88d285b162ca`  
		Last Modified: Thu, 11 Jun 2020 20:54:00 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abf62b7cec62367b3dbf8205df906d5380b0f60394a5688de6270734eddf59c0`  
		Last Modified: Thu, 11 Jun 2020 20:54:01 GMT  
		Size: 15.7 KB (15666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad7fdef1b41af486bfb55bb5ce24c78108a20b09265b270ff707cd7b40664d02`  
		Last Modified: Tue, 08 Sep 2020 21:27:16 GMT  
		Size: 2.1 MB (2076916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa6a7d33c013dbdf201db7eef507d048362838d8bca32018751d804d7cf6d858`  
		Last Modified: Tue, 08 Sep 2020 21:27:16 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9a5d51fa547f310e8cdb76975f971b87f0be63de169c68a9a00fb15249c8816`  
		Last Modified: Tue, 08 Sep 2020 21:27:16 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-alpine` - linux; 386

```console
$ docker pull memcached@sha256:31ca3704550a0170a48bc9d320b306102e484250edee144f9d10cc8a79ab0a35
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (4957953 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:20bed8fb2767398a969a48948babafcd8261b38a331c1d859e12fa3e02b1d690`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 29 May 2020 21:38:33 GMT
ADD file:5624441d97aca5eeb82a582941efc3586397098b8391227a9040ebe434cc1d6b in / 
# Fri, 29 May 2020 21:38:33 GMT
CMD ["/bin/sh"]
# Thu, 11 Jun 2020 22:34:33 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Thu, 11 Jun 2020 22:34:34 GMT
RUN apk add --no-cache cyrus-sasl-plain
# Tue, 08 Sep 2020 20:04:27 GMT
ENV MEMCACHED_VERSION=1.6.7
# Tue, 08 Sep 2020 20:04:27 GMT
ENV MEMCACHED_SHA1=49336bb0a4b7ad296422b08148581ed54edf32d0
# Tue, 08 Sep 2020 20:14:20 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		dpkg-dev dpkg 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		tar 		wget 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& make test 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 08 Sep 2020 20:14:20 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 08 Sep 2020 20:14:21 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 08 Sep 2020 20:14:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 08 Sep 2020 20:14:21 GMT
USER memcache
# Tue, 08 Sep 2020 20:14:21 GMT
EXPOSE 11211
# Tue, 08 Sep 2020 20:14:22 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:0625b4155e2a59f647ece47c0cd77ed3196b1f84454fa64ce80cad90e2b9b79e`  
		Last Modified: Fri, 29 May 2020 21:38:53 GMT  
		Size: 2.8 MB (2792298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:053753de6f049436417b1e2a50db73e47b194bd33f797965f6bd5f12c34f4d28`  
		Last Modified: Thu, 11 Jun 2020 22:45:05 GMT  
		Size: 1.2 KB (1231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a293d5635155e323f1e11070a6feb690a2ed40238b9414e2f73de5c4eb21cec3`  
		Last Modified: Thu, 11 Jun 2020 22:45:05 GMT  
		Size: 16.3 KB (16309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d116af020f9edc239ddd492a64b13b60061a8d942d7f8a5e50ef6d21cea4803`  
		Last Modified: Tue, 08 Sep 2020 20:14:44 GMT  
		Size: 2.1 MB (2147710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28f73fb0898406ab5a318c68e66c7ea0282aba028135fe34d3a87d0b04e5f3a6`  
		Last Modified: Tue, 08 Sep 2020 20:14:44 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4284ab01f9851d348bfb5c221d20faba538766b47ec8954ea6cb4b699414998b`  
		Last Modified: Tue, 08 Sep 2020 20:14:44 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-alpine` - linux; ppc64le

```console
$ docker pull memcached@sha256:d6751a0596f3ebfb78a0b9f5b10cb4f89485f57f293ae2f4fe29e471ed064eb0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (4954591 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e88c6bbffd1d20b19a59c6e8601d47d463f9e447d017b589f1d8fb9056cdaa8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 29 May 2020 21:23:03 GMT
ADD file:8194808a812370fd2202d80d1667f851bd9eac4c560d69d347fe1964f54343de in / 
# Fri, 29 May 2020 21:23:06 GMT
CMD ["/bin/sh"]
# Thu, 11 Jun 2020 21:28:54 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Thu, 11 Jun 2020 21:29:00 GMT
RUN apk add --no-cache cyrus-sasl-plain
# Tue, 08 Sep 2020 21:02:42 GMT
ENV MEMCACHED_VERSION=1.6.7
# Tue, 08 Sep 2020 21:02:47 GMT
ENV MEMCACHED_SHA1=49336bb0a4b7ad296422b08148581ed54edf32d0
# Tue, 08 Sep 2020 21:12:56 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		dpkg-dev dpkg 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		tar 		wget 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& make test 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 08 Sep 2020 21:12:58 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 08 Sep 2020 21:13:07 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 08 Sep 2020 21:13:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 08 Sep 2020 21:13:15 GMT
USER memcache
# Tue, 08 Sep 2020 21:13:18 GMT
EXPOSE 11211
# Tue, 08 Sep 2020 21:13:21 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:5077f8601dceb5744d875d7740ebc203f674b108a0188f3a31e292b21a4bee64`  
		Last Modified: Fri, 29 May 2020 21:23:37 GMT  
		Size: 2.8 MB (2805199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5da85732ec2c118da92b83669225af1d8b16986733a33a75401b712da2ed1510`  
		Last Modified: Thu, 11 Jun 2020 21:40:05 GMT  
		Size: 1.3 KB (1265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e466bec4d365b2c3064b6a41b20a28dd25fc8648c778f467d7ffd2fca60fce67`  
		Last Modified: Thu, 11 Jun 2020 21:40:05 GMT  
		Size: 16.3 KB (16307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5de324c8b5732e45731bcd408805025e0067d6eb99f5d3a4bc018d3a24c5773`  
		Last Modified: Tue, 08 Sep 2020 21:14:07 GMT  
		Size: 2.1 MB (2131416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6251901b79919688b1fc772326877a528474bb9f6c82f715f029287cf22d2ba3`  
		Last Modified: Tue, 08 Sep 2020 21:14:06 GMT  
		Size: 283.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c67a15198fb6666781fd4ced69393d50c0c09ee6bf766e4c0be6a9915d37e80`  
		Last Modified: Tue, 08 Sep 2020 21:14:06 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-alpine` - linux; s390x

```console
$ docker pull memcached@sha256:ac57a3b53de45bfc54993bc36ffd2939b18467759b501bb4f7ef850a86e1a632
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4667972 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0d148284ba37411d02418001c76b7df11b95cc18de4cb0a94545ed2f9d16f1b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 29 May 2020 21:41:39 GMT
ADD file:9799ce3b2f782a28e10b1846cd9b3db827fa99c9bc601feb268456195856814e in / 
# Fri, 29 May 2020 21:41:39 GMT
CMD ["/bin/sh"]
# Thu, 11 Jun 2020 19:41:31 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Thu, 11 Jun 2020 19:41:32 GMT
RUN apk add --no-cache cyrus-sasl-plain
# Tue, 08 Sep 2020 20:05:33 GMT
ENV MEMCACHED_VERSION=1.6.7
# Tue, 08 Sep 2020 20:05:33 GMT
ENV MEMCACHED_SHA1=49336bb0a4b7ad296422b08148581ed54edf32d0
# Tue, 08 Sep 2020 20:14:30 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		dpkg-dev dpkg 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		tar 		wget 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& make test 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 08 Sep 2020 20:14:30 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 08 Sep 2020 20:14:31 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 08 Sep 2020 20:14:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 08 Sep 2020 20:14:31 GMT
USER memcache
# Tue, 08 Sep 2020 20:14:31 GMT
EXPOSE 11211
# Tue, 08 Sep 2020 20:14:31 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:8fb3d41b2e9a59630b51745f257cd2561f96bcd15cf309fcc20120d5fcee8c5b`  
		Last Modified: Fri, 29 May 2020 21:42:03 GMT  
		Size: 2.6 MB (2566189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:844417c2ac824247320ce09147386405c59cd97101ff0d7cdbb939d961eaa2b7`  
		Last Modified: Thu, 11 Jun 2020 19:51:23 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83365eb9bbed49c8b8705426f527c5cace2db28af3c362b07f7edb2a54081b74`  
		Last Modified: Thu, 11 Jun 2020 19:51:23 GMT  
		Size: 15.5 KB (15547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5611c53be4f0d770a1e13e22e4960ce69780ddba187630f7e7b1a734220086f4`  
		Last Modified: Tue, 08 Sep 2020 20:14:55 GMT  
		Size: 2.1 MB (2084574 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe21c4e263557f5a3dc7dd4b9fe6d53fafb6735b7a8adba33498dc66c975f1b3`  
		Last Modified: Tue, 08 Sep 2020 20:14:55 GMT  
		Size: 283.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e86dc35f36a362c5f02870203ead9db5268d33ab3cfa6dc2c103a5365eca7a2`  
		Last Modified: Tue, 08 Sep 2020 20:14:55 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:alpine`

```console
$ docker pull memcached@sha256:f082d96b17dcf912e5b0615995b3ab9ed28a400bbe095142e39f01d59edb1103
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
$ docker pull memcached@sha256:77ccfc5250e116838ae941b40fe83fbd10af6b58fc3f424fc060d2c74366c41c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4879276 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:417903261a6412798128441638195daa0a1bd15e1f9ad3518ee56a36dc1f93cf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 29 May 2020 21:19:46 GMT
ADD file:c92c248239f8c7b9b3c067650954815f391b7bcb09023f984972c082ace2a8d0 in / 
# Fri, 29 May 2020 21:19:46 GMT
CMD ["/bin/sh"]
# Thu, 11 Jun 2020 22:36:17 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Thu, 11 Jun 2020 22:36:18 GMT
RUN apk add --no-cache cyrus-sasl-plain
# Tue, 08 Sep 2020 19:58:25 GMT
ENV MEMCACHED_VERSION=1.6.7
# Tue, 08 Sep 2020 19:58:25 GMT
ENV MEMCACHED_SHA1=49336bb0a4b7ad296422b08148581ed54edf32d0
# Tue, 08 Sep 2020 20:17:57 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		dpkg-dev dpkg 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		tar 		wget 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& make test 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 08 Sep 2020 20:17:57 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 08 Sep 2020 20:17:58 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 08 Sep 2020 20:17:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 08 Sep 2020 20:17:58 GMT
USER memcache
# Tue, 08 Sep 2020 20:17:58 GMT
EXPOSE 11211
# Tue, 08 Sep 2020 20:17:59 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:df20fa9351a15782c64e6dddb2d4a6f50bf6d3688060a34c4014b0d9a752eb4c`  
		Last Modified: Fri, 29 May 2020 21:20:06 GMT  
		Size: 2.8 MB (2797541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9da9e0d7f92826205e029bfd978a90f40bc6fdcf5e15730881f4c53893b6c958`  
		Last Modified: Thu, 11 Jun 2020 22:46:20 GMT  
		Size: 1.2 KB (1230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a01e9fc6969fb7eb8c18a96fbe204469f0c2a753cb2851e9a5b48cf1d42efe64`  
		Last Modified: Thu, 11 Jun 2020 22:46:20 GMT  
		Size: 15.3 KB (15282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:402843d6a42d73d92e4e046fbd68a7ede8e634f27d56cb74c4152d29374bfc2f`  
		Last Modified: Tue, 08 Sep 2020 20:18:20 GMT  
		Size: 2.1 MB (2064819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3cd9988120f5b64ce357a2f9d5bae7defaf23f26b29578f0ae3555f8ca44455`  
		Last Modified: Tue, 08 Sep 2020 20:18:20 GMT  
		Size: 283.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2c3f54b6a0ee5c03a5ef2c6ff819d1a12d4d4ca5761175c7c400ff9bb97a311`  
		Last Modified: Tue, 08 Sep 2020 20:18:21 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:alpine` - linux; arm variant v6

```console
$ docker pull memcached@sha256:e03f9bd4773341a508783efc5e0dba17a9261998261b9d0300d97462e146bee2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4642127 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:244b1d3b240c8fd5a4a082f45d2ccd20f11fdba80567329d0a85c178a8075685`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 29 May 2020 21:50:55 GMT
ADD file:f46e997a56849423db17e5fc9f0249ab6c73b155245927dba5fcb9dfd65f622f in / 
# Fri, 29 May 2020 21:50:56 GMT
CMD ["/bin/sh"]
# Thu, 11 Jun 2020 19:34:27 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Thu, 11 Jun 2020 19:34:30 GMT
RUN apk add --no-cache cyrus-sasl-plain
# Tue, 08 Sep 2020 20:37:05 GMT
ENV MEMCACHED_VERSION=1.6.7
# Tue, 08 Sep 2020 20:37:13 GMT
ENV MEMCACHED_SHA1=49336bb0a4b7ad296422b08148581ed54edf32d0
# Tue, 08 Sep 2020 20:48:32 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		dpkg-dev dpkg 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		tar 		wget 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& make test 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 08 Sep 2020 20:48:54 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 08 Sep 2020 20:49:25 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 08 Sep 2020 20:49:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 08 Sep 2020 20:49:40 GMT
USER memcache
# Tue, 08 Sep 2020 20:49:47 GMT
EXPOSE 11211
# Tue, 08 Sep 2020 20:49:58 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:b4b72e716706d29f5d2351709c20bf737b94f876a5472a43ff1b6e203c65d27f`  
		Last Modified: Fri, 29 May 2020 21:51:30 GMT  
		Size: 2.6 MB (2603286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07d7bd6b3b6044e07d261038778674ff772f8776c9aa1b04e2c00591dec9d4bb`  
		Last Modified: Thu, 11 Jun 2020 19:45:28 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b80a5ea355d8ff9191648d56b12825dd65d5e619a6c53da85eb7ae4853362c02`  
		Last Modified: Thu, 11 Jun 2020 19:45:29 GMT  
		Size: 14.9 KB (14890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:840a119db59d7756c10a241a3113f6701a7a2dea799799d894613615d101ab86`  
		Last Modified: Tue, 08 Sep 2020 20:50:20 GMT  
		Size: 2.0 MB (2022286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd3161efc183503e07c48bdc064b820190fba6381d49ae7db0066a5e5d999b71`  
		Last Modified: Tue, 08 Sep 2020 20:50:20 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55c40db22205f1918b380ed8a513eab7b73e185ce15693ddb907299c8cd870e7`  
		Last Modified: Tue, 08 Sep 2020 20:50:20 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:alpine` - linux; arm variant v7

```console
$ docker pull memcached@sha256:5df58dd4af8c4e69b2d0a71c6a35811934379c618fb3247d0d9b5cd726636c7a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.3 MB (4308981 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e4d85a2b8661ec592eaea28d949c858606735eedea931bad225bdfb76411a579`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 29 May 2020 21:02:07 GMT
ADD file:e97bf0d217846312b19a9f7264604851aedd125c23b4d291eed4c69b880dce26 in / 
# Fri, 29 May 2020 21:02:08 GMT
CMD ["/bin/sh"]
# Thu, 11 Jun 2020 20:31:56 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Thu, 11 Jun 2020 20:31:58 GMT
RUN apk add --no-cache cyrus-sasl-plain
# Tue, 08 Sep 2020 21:31:04 GMT
ENV MEMCACHED_VERSION=1.6.7
# Tue, 08 Sep 2020 21:31:19 GMT
ENV MEMCACHED_SHA1=49336bb0a4b7ad296422b08148581ed54edf32d0
# Tue, 08 Sep 2020 21:42:25 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		dpkg-dev dpkg 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		tar 		wget 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& make test 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 08 Sep 2020 21:42:40 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 08 Sep 2020 21:43:14 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 08 Sep 2020 21:43:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 08 Sep 2020 21:43:27 GMT
USER memcache
# Tue, 08 Sep 2020 21:43:36 GMT
EXPOSE 11211
# Tue, 08 Sep 2020 21:43:45 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:52278dd8e57993669c5b72a9620e89bebdc098f2af2379caaa8945f7403f77a2`  
		Last Modified: Fri, 29 May 2020 21:02:38 GMT  
		Size: 2.4 MB (2406763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a171a50ea23b122e85435c89187bf16a391efa7d74cb2d7aa6cb2c5555bc9830`  
		Last Modified: Thu, 11 Jun 2020 20:43:17 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac40655da815a69db31129873e9e388bba260ee4962ba15f288b81a58e580925`  
		Last Modified: Thu, 11 Jun 2020 20:43:17 GMT  
		Size: 13.8 KB (13821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fb21bd27680eb0bb3a12b0230902e6e669705c89eb00a40b1e447c724630aaf`  
		Last Modified: Tue, 08 Sep 2020 21:44:14 GMT  
		Size: 1.9 MB (1886732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f223b308518beca0559a433993f85b4839c01cc9bd99273e99ca85a41c2789e`  
		Last Modified: Tue, 08 Sep 2020 21:44:13 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c89f21f449a1fe14dd0743b953195690232696f7b71bff23bbbf37c513f58066`  
		Last Modified: Tue, 08 Sep 2020 21:44:13 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:alpine` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:0e93e6e8893fe1a57e9ff87a1be7549c1242a220f82728073537827606f866e6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.8 MB (4802209 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:488a4ea2a5396d38953aea7778aa7e954ad63581062a8a72b36db8a850cbe191`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 29 May 2020 21:43:19 GMT
ADD file:7574aee4e37a85460ab889212d52912723a9b30dda1c060548f0deb4a05fc398 in / 
# Fri, 29 May 2020 21:43:20 GMT
CMD ["/bin/sh"]
# Thu, 11 Jun 2020 20:42:19 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Thu, 11 Jun 2020 20:42:27 GMT
RUN apk add --no-cache cyrus-sasl-plain
# Tue, 08 Sep 2020 21:15:58 GMT
ENV MEMCACHED_VERSION=1.6.7
# Tue, 08 Sep 2020 21:16:03 GMT
ENV MEMCACHED_SHA1=49336bb0a4b7ad296422b08148581ed54edf32d0
# Tue, 08 Sep 2020 21:26:35 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		dpkg-dev dpkg 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		tar 		wget 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& make test 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 08 Sep 2020 21:26:36 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 08 Sep 2020 21:26:38 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 08 Sep 2020 21:26:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 08 Sep 2020 21:26:39 GMT
USER memcache
# Tue, 08 Sep 2020 21:26:40 GMT
EXPOSE 11211
# Tue, 08 Sep 2020 21:26:41 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:b538f80385f9b48122e3da068c932a96ea5018afa3c7be79da00437414bd18cd`  
		Last Modified: Fri, 29 May 2020 21:43:57 GMT  
		Size: 2.7 MB (2707964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f6b5a3ebcdb20348b01d4048b7bcffbdcfd27ef2e8bcf97439b88d285b162ca`  
		Last Modified: Thu, 11 Jun 2020 20:54:00 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abf62b7cec62367b3dbf8205df906d5380b0f60394a5688de6270734eddf59c0`  
		Last Modified: Thu, 11 Jun 2020 20:54:01 GMT  
		Size: 15.7 KB (15666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad7fdef1b41af486bfb55bb5ce24c78108a20b09265b270ff707cd7b40664d02`  
		Last Modified: Tue, 08 Sep 2020 21:27:16 GMT  
		Size: 2.1 MB (2076916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa6a7d33c013dbdf201db7eef507d048362838d8bca32018751d804d7cf6d858`  
		Last Modified: Tue, 08 Sep 2020 21:27:16 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9a5d51fa547f310e8cdb76975f971b87f0be63de169c68a9a00fb15249c8816`  
		Last Modified: Tue, 08 Sep 2020 21:27:16 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:alpine` - linux; 386

```console
$ docker pull memcached@sha256:31ca3704550a0170a48bc9d320b306102e484250edee144f9d10cc8a79ab0a35
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (4957953 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:20bed8fb2767398a969a48948babafcd8261b38a331c1d859e12fa3e02b1d690`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 29 May 2020 21:38:33 GMT
ADD file:5624441d97aca5eeb82a582941efc3586397098b8391227a9040ebe434cc1d6b in / 
# Fri, 29 May 2020 21:38:33 GMT
CMD ["/bin/sh"]
# Thu, 11 Jun 2020 22:34:33 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Thu, 11 Jun 2020 22:34:34 GMT
RUN apk add --no-cache cyrus-sasl-plain
# Tue, 08 Sep 2020 20:04:27 GMT
ENV MEMCACHED_VERSION=1.6.7
# Tue, 08 Sep 2020 20:04:27 GMT
ENV MEMCACHED_SHA1=49336bb0a4b7ad296422b08148581ed54edf32d0
# Tue, 08 Sep 2020 20:14:20 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		dpkg-dev dpkg 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		tar 		wget 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& make test 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 08 Sep 2020 20:14:20 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 08 Sep 2020 20:14:21 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 08 Sep 2020 20:14:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 08 Sep 2020 20:14:21 GMT
USER memcache
# Tue, 08 Sep 2020 20:14:21 GMT
EXPOSE 11211
# Tue, 08 Sep 2020 20:14:22 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:0625b4155e2a59f647ece47c0cd77ed3196b1f84454fa64ce80cad90e2b9b79e`  
		Last Modified: Fri, 29 May 2020 21:38:53 GMT  
		Size: 2.8 MB (2792298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:053753de6f049436417b1e2a50db73e47b194bd33f797965f6bd5f12c34f4d28`  
		Last Modified: Thu, 11 Jun 2020 22:45:05 GMT  
		Size: 1.2 KB (1231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a293d5635155e323f1e11070a6feb690a2ed40238b9414e2f73de5c4eb21cec3`  
		Last Modified: Thu, 11 Jun 2020 22:45:05 GMT  
		Size: 16.3 KB (16309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d116af020f9edc239ddd492a64b13b60061a8d942d7f8a5e50ef6d21cea4803`  
		Last Modified: Tue, 08 Sep 2020 20:14:44 GMT  
		Size: 2.1 MB (2147710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28f73fb0898406ab5a318c68e66c7ea0282aba028135fe34d3a87d0b04e5f3a6`  
		Last Modified: Tue, 08 Sep 2020 20:14:44 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4284ab01f9851d348bfb5c221d20faba538766b47ec8954ea6cb4b699414998b`  
		Last Modified: Tue, 08 Sep 2020 20:14:44 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:alpine` - linux; ppc64le

```console
$ docker pull memcached@sha256:d6751a0596f3ebfb78a0b9f5b10cb4f89485f57f293ae2f4fe29e471ed064eb0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (4954591 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e88c6bbffd1d20b19a59c6e8601d47d463f9e447d017b589f1d8fb9056cdaa8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 29 May 2020 21:23:03 GMT
ADD file:8194808a812370fd2202d80d1667f851bd9eac4c560d69d347fe1964f54343de in / 
# Fri, 29 May 2020 21:23:06 GMT
CMD ["/bin/sh"]
# Thu, 11 Jun 2020 21:28:54 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Thu, 11 Jun 2020 21:29:00 GMT
RUN apk add --no-cache cyrus-sasl-plain
# Tue, 08 Sep 2020 21:02:42 GMT
ENV MEMCACHED_VERSION=1.6.7
# Tue, 08 Sep 2020 21:02:47 GMT
ENV MEMCACHED_SHA1=49336bb0a4b7ad296422b08148581ed54edf32d0
# Tue, 08 Sep 2020 21:12:56 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		dpkg-dev dpkg 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		tar 		wget 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& make test 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 08 Sep 2020 21:12:58 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 08 Sep 2020 21:13:07 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 08 Sep 2020 21:13:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 08 Sep 2020 21:13:15 GMT
USER memcache
# Tue, 08 Sep 2020 21:13:18 GMT
EXPOSE 11211
# Tue, 08 Sep 2020 21:13:21 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:5077f8601dceb5744d875d7740ebc203f674b108a0188f3a31e292b21a4bee64`  
		Last Modified: Fri, 29 May 2020 21:23:37 GMT  
		Size: 2.8 MB (2805199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5da85732ec2c118da92b83669225af1d8b16986733a33a75401b712da2ed1510`  
		Last Modified: Thu, 11 Jun 2020 21:40:05 GMT  
		Size: 1.3 KB (1265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e466bec4d365b2c3064b6a41b20a28dd25fc8648c778f467d7ffd2fca60fce67`  
		Last Modified: Thu, 11 Jun 2020 21:40:05 GMT  
		Size: 16.3 KB (16307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5de324c8b5732e45731bcd408805025e0067d6eb99f5d3a4bc018d3a24c5773`  
		Last Modified: Tue, 08 Sep 2020 21:14:07 GMT  
		Size: 2.1 MB (2131416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6251901b79919688b1fc772326877a528474bb9f6c82f715f029287cf22d2ba3`  
		Last Modified: Tue, 08 Sep 2020 21:14:06 GMT  
		Size: 283.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c67a15198fb6666781fd4ced69393d50c0c09ee6bf766e4c0be6a9915d37e80`  
		Last Modified: Tue, 08 Sep 2020 21:14:06 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:alpine` - linux; s390x

```console
$ docker pull memcached@sha256:ac57a3b53de45bfc54993bc36ffd2939b18467759b501bb4f7ef850a86e1a632
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4667972 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0d148284ba37411d02418001c76b7df11b95cc18de4cb0a94545ed2f9d16f1b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 29 May 2020 21:41:39 GMT
ADD file:9799ce3b2f782a28e10b1846cd9b3db827fa99c9bc601feb268456195856814e in / 
# Fri, 29 May 2020 21:41:39 GMT
CMD ["/bin/sh"]
# Thu, 11 Jun 2020 19:41:31 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Thu, 11 Jun 2020 19:41:32 GMT
RUN apk add --no-cache cyrus-sasl-plain
# Tue, 08 Sep 2020 20:05:33 GMT
ENV MEMCACHED_VERSION=1.6.7
# Tue, 08 Sep 2020 20:05:33 GMT
ENV MEMCACHED_SHA1=49336bb0a4b7ad296422b08148581ed54edf32d0
# Tue, 08 Sep 2020 20:14:30 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		dpkg-dev dpkg 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		tar 		wget 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& make test 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 08 Sep 2020 20:14:30 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 08 Sep 2020 20:14:31 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 08 Sep 2020 20:14:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 08 Sep 2020 20:14:31 GMT
USER memcache
# Tue, 08 Sep 2020 20:14:31 GMT
EXPOSE 11211
# Tue, 08 Sep 2020 20:14:31 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:8fb3d41b2e9a59630b51745f257cd2561f96bcd15cf309fcc20120d5fcee8c5b`  
		Last Modified: Fri, 29 May 2020 21:42:03 GMT  
		Size: 2.6 MB (2566189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:844417c2ac824247320ce09147386405c59cd97101ff0d7cdbb939d961eaa2b7`  
		Last Modified: Thu, 11 Jun 2020 19:51:23 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83365eb9bbed49c8b8705426f527c5cace2db28af3c362b07f7edb2a54081b74`  
		Last Modified: Thu, 11 Jun 2020 19:51:23 GMT  
		Size: 15.5 KB (15547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5611c53be4f0d770a1e13e22e4960ce69780ddba187630f7e7b1a734220086f4`  
		Last Modified: Tue, 08 Sep 2020 20:14:55 GMT  
		Size: 2.1 MB (2084574 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe21c4e263557f5a3dc7dd4b9fe6d53fafb6735b7a8adba33498dc66c975f1b3`  
		Last Modified: Tue, 08 Sep 2020 20:14:55 GMT  
		Size: 283.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e86dc35f36a362c5f02870203ead9db5268d33ab3cfa6dc2c103a5365eca7a2`  
		Last Modified: Tue, 08 Sep 2020 20:14:55 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:latest`

```console
$ docker pull memcached@sha256:d999887e1fbd1ae9c6209459ae28ee0477c034b40ab2c6b492aa6a3dd3a3f564
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
$ docker pull memcached@sha256:7b8d8fbef4feb9386884d0aa2ecd3912aa62f2ec26efea54a57bc8fcf78348b6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.5 MB (30493470 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b4920487992d3dbbe4aa89a7336e06600ab8b41fe8f889212e927f7fbb19593`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 10 Sep 2020 00:23:29 GMT
ADD file:e7407f2294ad23634565820b9669b18ff2a2ca0212a7ec84b9c89d8550859954 in / 
# Thu, 10 Sep 2020 00:23:30 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 06:42:10 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Thu, 10 Sep 2020 06:42:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 06:42:17 GMT
ENV MEMCACHED_VERSION=1.6.7
# Thu, 10 Sep 2020 06:42:18 GMT
ENV MEMCACHED_SHA1=49336bb0a4b7ad296422b08148581ed54edf32d0
# Thu, 10 Sep 2020 06:52:26 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 10 Sep 2020 06:52:26 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 10 Sep 2020 06:52:28 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 10 Sep 2020 06:52:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 10 Sep 2020 06:52:28 GMT
USER memcache
# Thu, 10 Sep 2020 06:52:29 GMT
EXPOSE 11211
# Thu, 10 Sep 2020 06:52:29 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:d121f8d1c4128ebc1e95e5bfad90a0189b84eadbbb2fbaad20cbb26d20b2c8a2`  
		Last Modified: Thu, 10 Sep 2020 00:34:02 GMT  
		Size: 27.1 MB (27092161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd29e75844e2246d981d63970769902be264bae0990bb5befc493e5d15eeeeb3`  
		Last Modified: Thu, 10 Sep 2020 06:52:50 GMT  
		Size: 5.0 KB (4980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1adbe52eab585d7464430faaab2b3f8759b1661558262688357dba99e6967db7`  
		Last Modified: Thu, 10 Sep 2020 06:52:50 GMT  
		Size: 2.2 MB (2196512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e7563db9f0d12fba4b16ab48ba07e143239fc53283b76b6532d09a26ed523e8`  
		Last Modified: Thu, 10 Sep 2020 06:52:50 GMT  
		Size: 1.2 MB (1199409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1018860c7c78773f11445b24c799624ebf7ad0c1a54955ee73a0d1fdf7eeb40`  
		Last Modified: Thu, 10 Sep 2020 06:52:50 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b02cff55081f0c25f0ae11f642177cfec21627dce0ad4f9593653f121d8a2297`  
		Last Modified: Thu, 10 Sep 2020 06:52:50 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:latest` - linux; arm variant v5

```console
$ docker pull memcached@sha256:db8e75930e7350dc06c594abc4f6eb130088c7a803729f2125820e48992c5e60
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.9 MB (27911252 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ca29ad8c51e933907ffd5cacfd7b034a533f7b15c99c2202743dd723b229f5a3`
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
# Tue, 13 Oct 2020 02:23:01 GMT
ENV MEMCACHED_VERSION=1.6.7
# Tue, 13 Oct 2020 02:23:02 GMT
ENV MEMCACHED_SHA1=49336bb0a4b7ad296422b08148581ed54edf32d0
# Tue, 13 Oct 2020 02:33:45 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 13 Oct 2020 02:33:46 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 13 Oct 2020 02:33:51 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 13 Oct 2020 02:33:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Oct 2020 02:33:53 GMT
USER memcache
# Tue, 13 Oct 2020 02:33:55 GMT
EXPOSE 11211
# Tue, 13 Oct 2020 02:33:57 GMT
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
	-	`sha256:85530c3b6a178a04b529523c2bf5e513e04d7a42f2cdebf26a69b484b56a68e2`  
		Last Modified: Tue, 13 Oct 2020 02:34:18 GMT  
		Size: 1.2 MB (1173125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38d48859b3d5f2dfe3a0ddff8417717ec4274b5d7431850f3434a35d856c8326`  
		Last Modified: Tue, 13 Oct 2020 02:34:18 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84b665bad50ddd6ddfcf2dc2cc9e826499da002347faf18378e77a3dc6f81505`  
		Last Modified: Tue, 13 Oct 2020 02:34:18 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:latest` - linux; arm variant v7

```console
$ docker pull memcached@sha256:534ab9a71bfdbc6306e5f0e66af8fe0f76bc509560817621b7e31c9dc7f94ac7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.7 MB (25660617 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ef1c3640e673dfff34704d898b5bb45aa552e63246457eb196726184a948b0a7`
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
# Tue, 13 Oct 2020 04:26:30 GMT
ENV MEMCACHED_VERSION=1.6.7
# Tue, 13 Oct 2020 04:26:31 GMT
ENV MEMCACHED_SHA1=49336bb0a4b7ad296422b08148581ed54edf32d0
# Tue, 13 Oct 2020 04:36:50 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 13 Oct 2020 04:36:51 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 13 Oct 2020 04:36:54 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 13 Oct 2020 04:36:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Oct 2020 04:36:56 GMT
USER memcache
# Tue, 13 Oct 2020 04:36:57 GMT
EXPOSE 11211
# Tue, 13 Oct 2020 04:36:57 GMT
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
	-	`sha256:d50f05a1d5be98ec50a0b9c6b32e28b0673ad3db35c5b90500b0a38cd1697589`  
		Last Modified: Tue, 13 Oct 2020 04:37:30 GMT  
		Size: 1.1 MB (1143928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a0ff448c0efd0905dc11c59b70feb4dd6cd02adda52ec427fa68bd0664cf165`  
		Last Modified: Tue, 13 Oct 2020 04:37:29 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c8559eb111bdc28303506d117e61bb26e47daa128d7fdb057bace4acaeeb1c4`  
		Last Modified: Tue, 13 Oct 2020 04:37:29 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:latest` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:7f9d722d816e4b63c87642fde2b901849b416838b47ab197bb52a4bec0ca01b6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.1 MB (29099929 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ea99cfec94c49c44ccb283458d9addd82f2763524a936bf3962202eecbe4e74`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 09 Sep 2020 23:50:54 GMT
ADD file:d870fb0484ea283840d9cc923c9c3fe36d1bb6b3b5ecfefcce06aa26a22c9414 in / 
# Wed, 09 Sep 2020 23:50:57 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 04:21:07 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Thu, 10 Sep 2020 04:21:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 04:21:19 GMT
ENV MEMCACHED_VERSION=1.6.7
# Thu, 10 Sep 2020 04:21:20 GMT
ENV MEMCACHED_SHA1=49336bb0a4b7ad296422b08148581ed54edf32d0
# Thu, 10 Sep 2020 04:31:42 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 10 Sep 2020 04:31:43 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 10 Sep 2020 04:31:45 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 10 Sep 2020 04:31:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 10 Sep 2020 04:31:46 GMT
USER memcache
# Thu, 10 Sep 2020 04:31:47 GMT
EXPOSE 11211
# Thu, 10 Sep 2020 04:31:48 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:a6d76de28f58f3470aff71c934c0fec4e5d0fad788f8b8bcc50601266fc1b34d`  
		Last Modified: Wed, 09 Sep 2020 23:59:09 GMT  
		Size: 25.8 MB (25849325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4f48bd1f465fe61c5d378a72dea86a5917d8ec222d9eda27c13d06a0388ce45`  
		Last Modified: Thu, 10 Sep 2020 04:32:19 GMT  
		Size: 5.0 KB (5023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6172eb8b991d9ee34cce4d10ae2d0a18036999e58977cb193f2493dba1d0922d`  
		Last Modified: Thu, 10 Sep 2020 04:32:19 GMT  
		Size: 2.1 MB (2075014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c4390371d3044be59e120ad4ac5e0ab67b9eaacd1a1fd97388724d7ffe5a5d8`  
		Last Modified: Thu, 10 Sep 2020 04:32:19 GMT  
		Size: 1.2 MB (1170159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8212b808878005bf5387d12077984b9fd4f2c6127c29515d63fbaabb572648a0`  
		Last Modified: Thu, 10 Sep 2020 04:32:19 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6dd274731a18972c07fee896065b96cd0d476de9b6a13ea57e0a1577e762d14`  
		Last Modified: Thu, 10 Sep 2020 04:32:18 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:latest` - linux; 386

```console
$ docker pull memcached@sha256:0fb71355a775a0f518e405710c83cff1d60dd0fddf7bb066ec19ce5c98ecb1fe
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.2 MB (31161216 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c69f202ca7e7d00a1d7deb0fdf47bda4a4fc3d57af1ee1e2d39e3e9eb7196ba`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 09 Sep 2020 23:40:19 GMT
ADD file:08dc20c9cd727ebf02cac6e4b287c3009274682174aee9222494491cd6c671b8 in / 
# Wed, 09 Sep 2020 23:40:19 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 02:19:41 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Thu, 10 Sep 2020 02:19:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 02:19:51 GMT
ENV MEMCACHED_VERSION=1.6.7
# Thu, 10 Sep 2020 02:19:52 GMT
ENV MEMCACHED_SHA1=49336bb0a4b7ad296422b08148581ed54edf32d0
# Thu, 10 Sep 2020 02:30:13 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 10 Sep 2020 02:30:13 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 10 Sep 2020 02:30:14 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 10 Sep 2020 02:30:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 10 Sep 2020 02:30:14 GMT
USER memcache
# Thu, 10 Sep 2020 02:30:15 GMT
EXPOSE 11211
# Thu, 10 Sep 2020 02:30:15 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:31e6582dbd9f9a84903d46339df0c393a63d2cbfb001b06b3204653cceafcc61`  
		Last Modified: Wed, 09 Sep 2020 23:46:30 GMT  
		Size: 27.8 MB (27750334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:096b2a6b5e34ad8c96b35f52e3615e85902d5b12f7bdbf4f984988b59ba14ac3`  
		Last Modified: Thu, 10 Sep 2020 02:30:33 GMT  
		Size: 4.9 KB (4895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ece6f6a2e1723d610af9b172d870ab4c9e6e3c132f316e5f7baa2787806fbae6`  
		Last Modified: Thu, 10 Sep 2020 02:30:33 GMT  
		Size: 2.2 MB (2208153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3df397ec8999490a45ed35ff7908dacec384cecced47533e490dd01de7e4a320`  
		Last Modified: Thu, 10 Sep 2020 02:30:34 GMT  
		Size: 1.2 MB (1197426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:debebc596e2e5ea23dca7e24bc712d7ed9942d1db2397c4140b12ce8af1ce21f`  
		Last Modified: Thu, 10 Sep 2020 02:30:33 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08513f3fdf1df7d6009039c5aae413fe16ee6ce6e40bae44f8d5e0b7bd3c8d38`  
		Last Modified: Thu, 10 Sep 2020 02:30:33 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:latest` - linux; mips64le

```console
$ docker pull memcached@sha256:7c1d3db9aa8a2c9947716b781c9ddc8c4d99e4a48318d3da3bfb2d9d5a553469
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.7 MB (28735881 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a7ac2f3081105bab353608116b822d5ff33be4e865e3e0f0e9f310c2953057b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 10 Sep 2020 00:10:03 GMT
ADD file:dec5e74bd1dacf4dd26507ac5227dfca6591d05d13bdf06c16217b9efff06ed9 in / 
# Thu, 10 Sep 2020 00:10:04 GMT
CMD ["bash"]
# Tue, 15 Sep 2020 03:17:09 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 15 Sep 2020 03:17:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Sep 2020 03:17:21 GMT
ENV MEMCACHED_VERSION=1.6.7
# Tue, 15 Sep 2020 03:17:22 GMT
ENV MEMCACHED_SHA1=49336bb0a4b7ad296422b08148581ed54edf32d0
# Wed, 23 Sep 2020 18:18:56 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 23 Sep 2020 18:18:56 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 23 Sep 2020 18:18:58 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 23 Sep 2020 18:18:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 23 Sep 2020 18:18:59 GMT
USER memcache
# Wed, 23 Sep 2020 18:18:59 GMT
EXPOSE 11211
# Wed, 23 Sep 2020 18:18:59 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:3e11c32dbce8eae675cead1f63aeade46d661eb3764bff6c26bb8ca6e2c364fb`  
		Last Modified: Tue, 15 Sep 2020 01:13:19 GMT  
		Size: 25.8 MB (25762660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88d32d437f1360c92791e6d1f0f490cc78c6209be1870bb6cb66b79c8349fa3d`  
		Last Modified: Wed, 23 Sep 2020 18:19:21 GMT  
		Size: 5.0 KB (4983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:592933aa8d3179edf056c3911fe15c0cf60587f931c74bc5d84b2f6de8d8992e`  
		Last Modified: Wed, 23 Sep 2020 18:19:23 GMT  
		Size: 1.8 MB (1776064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfb94ff2fdc8d15ea207ebec0799b92feeefb4d3334a38c2cd1758d3609dc5b2`  
		Last Modified: Wed, 23 Sep 2020 18:19:23 GMT  
		Size: 1.2 MB (1191765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84ce46a0757ebb411e71d3d59a7c40edbb368b2bdf9472df7da0b18d4f9e0e1a`  
		Last Modified: Wed, 23 Sep 2020 18:19:21 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05dae55a53383b9643fd68465eebc790642fae4074c8b49f937d8b424544c3da`  
		Last Modified: Wed, 23 Sep 2020 18:19:22 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:latest` - linux; ppc64le

```console
$ docker pull memcached@sha256:9ee0904c2a1eff337f8886c5f9e74a92462f156abb0996c09a7343c80b89a502
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.1 MB (34071624 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d5ce8ca6190b2a43e92824fa399c7fc498dc96544f6edbc45dc40562588828d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 10 Sep 2020 01:06:11 GMT
ADD file:4dede556abae88027bd22f3166fdbc38778a6fcd686c5ce768c3ca024ab3f9cf in / 
# Thu, 10 Sep 2020 01:06:20 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 21:27:40 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Thu, 10 Sep 2020 21:28:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 21:28:09 GMT
ENV MEMCACHED_VERSION=1.6.7
# Thu, 10 Sep 2020 21:28:13 GMT
ENV MEMCACHED_SHA1=49336bb0a4b7ad296422b08148581ed54edf32d0
# Thu, 10 Sep 2020 21:44:40 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 10 Sep 2020 21:44:45 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 10 Sep 2020 21:45:03 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 10 Sep 2020 21:45:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 10 Sep 2020 21:45:16 GMT
USER memcache
# Thu, 10 Sep 2020 21:45:25 GMT
EXPOSE 11211
# Thu, 10 Sep 2020 21:45:31 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:f8aef3d2247e5f990bc767bc99f575b9bcec34aaa37183414eebe28fcd09519d`  
		Last Modified: Thu, 10 Sep 2020 01:28:12 GMT  
		Size: 30.5 MB (30517880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5b7bfeb11b26b80e3f45ddc9eec4e6fa55c578fd1b3735b718e666cb5c661d6`  
		Last Modified: Thu, 10 Sep 2020 21:46:03 GMT  
		Size: 5.0 KB (4988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb81e5357148bb530b5afccd9a6fc7b05010564b011024db6515763ef71c0ce3`  
		Last Modified: Thu, 10 Sep 2020 21:46:03 GMT  
		Size: 2.3 MB (2322772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f5a11e72f2a67deedc2e0a4af04f9fcda2aa1cbd833ef8985418eec3ec2f63e`  
		Last Modified: Thu, 10 Sep 2020 21:46:03 GMT  
		Size: 1.2 MB (1225576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0f3a0aafd05b076f9f6cca15b1674c60464d9c1074391b796ad515cb20b29c4`  
		Last Modified: Thu, 10 Sep 2020 21:46:03 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffa12800e0545bdcc70841732b77e97c7d1eb18ae0d7cf28a25035eca507e057`  
		Last Modified: Thu, 10 Sep 2020 21:46:03 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:latest` - linux; s390x

```console
$ docker pull memcached@sha256:29246fb608029daf71e59f2826a30d3d1228bfff1e261abdf8e8a6742d558e56
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.8 MB (28789171 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:81a42318833ed3d53d0befe80a053c5f038b58886994eb98f10deab18a17df83`
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
# Tue, 13 Oct 2020 02:44:47 GMT
ENV MEMCACHED_VERSION=1.6.7
# Tue, 13 Oct 2020 02:44:48 GMT
ENV MEMCACHED_SHA1=49336bb0a4b7ad296422b08148581ed54edf32d0
# Tue, 13 Oct 2020 02:54:05 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 13 Oct 2020 02:54:06 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 13 Oct 2020 02:54:07 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 13 Oct 2020 02:54:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Oct 2020 02:54:07 GMT
USER memcache
# Tue, 13 Oct 2020 02:54:07 GMT
EXPOSE 11211
# Tue, 13 Oct 2020 02:54:07 GMT
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
	-	`sha256:cc4afc3e1ed06ea6037b98689f0536544ca7d61153a60fdc589230648e2a984e`  
		Last Modified: Tue, 13 Oct 2020 02:54:35 GMT  
		Size: 1.2 MB (1190100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f259c385180086733d453c3eaeee6fac1efecc084bd34815bf58421ae8fc0e40`  
		Last Modified: Tue, 13 Oct 2020 02:54:35 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98288868e61d43041bb2178e9722e20e72849b117eaa0cbd7cb92d981147f652`  
		Last Modified: Tue, 13 Oct 2020 02:54:35 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
