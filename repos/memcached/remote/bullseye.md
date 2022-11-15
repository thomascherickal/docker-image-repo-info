## `memcached:bullseye`

```console
$ docker pull memcached@sha256:d22b1e9f55ff911aaca4b0e53d8a2d3c53730da53e7019e6ff92ddd5911b17f8
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
$ docker pull memcached@sha256:6de02d67b123f40b7fa93ac45966ca9c1d3b00d8df5c264f38383fe2da5b3bb8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.0 MB (33011867 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f78b9bd951af33b533f55dc8eccc9a3c4072b2cf593e05760ed3fcd39755672b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 25 Oct 2022 01:43:53 GMT
ADD file:8644a8156a07a656a35c41e2b2a458befb660309f8592e3efd5b43d46156cec2 in / 
# Tue, 25 Oct 2022 01:43:53 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 10:08:27 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 25 Oct 2022 10:08:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 10:08:30 GMT
ENV MEMCACHED_VERSION=1.6.17
# Tue, 25 Oct 2022 10:08:30 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Tue, 25 Oct 2022 10:11:12 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 25 Oct 2022 10:11:12 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 25 Oct 2022 10:11:13 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 25 Oct 2022 10:11:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 25 Oct 2022 10:11:13 GMT
USER memcache
# Tue, 25 Oct 2022 10:11:13 GMT
EXPOSE 11211
# Tue, 25 Oct 2022 10:11:13 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:e9995326b091af7b3ce352fad4d76cf3a3cb62b7a0c35cc5f625e8e649d23c50`  
		Last Modified: Tue, 25 Oct 2022 01:47:55 GMT  
		Size: 31.4 MB (31420038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caa763f84eacc9454d6aba84f7d30792f702fab89932ac20fb4f0659b0412acb`  
		Last Modified: Tue, 25 Oct 2022 10:11:39 GMT  
		Size: 5.0 KB (4981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:506fef44674e3b2fa95ef70b3ce73f3435569f5d5b531a1eef062165a13cccf4`  
		Last Modified: Tue, 25 Oct 2022 10:11:39 GMT  
		Size: 328.9 KB (328873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:678083585bce63dafb61c096df6795560f20ee3a04269d7043b41925bfa3b7e4`  
		Last Modified: Tue, 25 Oct 2022 10:11:39 GMT  
		Size: 1.3 MB (1257569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20edd5fae517075fe06f74718b91c90be417daa2d2ef5aadebe654b81ed55b7c`  
		Last Modified: Tue, 25 Oct 2022 10:11:39 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3bff5c87d1d73be76c801701e5f3d98fc40d984bde6b1dd1c9b6b29cad285ec`  
		Last Modified: Tue, 25 Oct 2022 10:11:39 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:bullseye` - linux; arm variant v5

```console
$ docker pull memcached@sha256:4b56a1657617c107b7b1ab27b7970a14d564ca929fc10d921a9e7871345f2da3
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.5 MB (30465948 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:87e04237d0f19f48581a9bb56d615a12b7fb94459d4e7befc08c69b9df19c402`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 15 Nov 2022 01:49:18 GMT
ADD file:1949af7e583a1b54055a421129c32315fc101e53e2cda05da3171ed461bde0a6 in / 
# Tue, 15 Nov 2022 01:49:19 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 05:54:52 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 15 Nov 2022 05:54:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 05:54:57 GMT
ENV MEMCACHED_VERSION=1.6.17
# Tue, 15 Nov 2022 05:54:57 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Tue, 15 Nov 2022 05:58:11 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 15 Nov 2022 05:58:11 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 15 Nov 2022 05:58:12 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 15 Nov 2022 05:58:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 15 Nov 2022 05:58:12 GMT
USER memcache
# Tue, 15 Nov 2022 05:58:12 GMT
EXPOSE 11211
# Tue, 15 Nov 2022 05:58:12 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:b56836d864a6d857be3d12242b65962f2a2cf0d77c48cfb85bbbdf9d56a7e93d`  
		Last Modified: Tue, 15 Nov 2022 01:54:26 GMT  
		Size: 28.9 MB (28914126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:000168341c6dd2d110b3500733afc4ae73b598a6c48ea468f4b9b55f9d6fdda0`  
		Last Modified: Tue, 15 Nov 2022 05:58:45 GMT  
		Size: 4.9 KB (4889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c3b8ba009d25dbeb519c21fdd50b7513610847be5b72e7c4304a8fce49bf359`  
		Last Modified: Tue, 15 Nov 2022 05:58:45 GMT  
		Size: 317.5 KB (317525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:873440d685712218e3478a9e7b747ccafc83f88ad88b498283acdabfef9e798f`  
		Last Modified: Tue, 15 Nov 2022 05:58:45 GMT  
		Size: 1.2 MB (1229001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f3c05da8d74417e2e4b550cd1ea51384cf04732db4b2b9a110a2856f2e83c50`  
		Last Modified: Tue, 15 Nov 2022 05:58:45 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58d1ad9bf00d6432f66f0cf36580bba9610f73a22097e1f3fbb207b25dd483b0`  
		Last Modified: Tue, 15 Nov 2022 05:58:45 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:bullseye` - linux; arm variant v7

```console
$ docker pull memcached@sha256:c56c8ef5cf9f972419418435f4d2642b997aa99cb509e450ef8d12f3273b00e2
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.1 MB (28098016 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa5502d1d0c5880c2a9c20e076870d38002651a3b38402913c569d8696e139be`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 25 Oct 2022 03:14:27 GMT
ADD file:0d2a17d07f391dfbf63c00d2b826373c98aaf6ab777481e33d4bee6d57c4a0b0 in / 
# Tue, 25 Oct 2022 03:14:27 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 13:28:48 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 25 Oct 2022 13:28:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 13:28:52 GMT
ENV MEMCACHED_VERSION=1.6.17
# Tue, 25 Oct 2022 13:28:52 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Tue, 25 Oct 2022 13:31:54 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 25 Oct 2022 13:31:54 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 25 Oct 2022 13:31:55 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 25 Oct 2022 13:31:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 25 Oct 2022 13:31:55 GMT
USER memcache
# Tue, 25 Oct 2022 13:31:55 GMT
EXPOSE 11211
# Tue, 25 Oct 2022 13:31:55 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:e96255deabf6ae29e08aa044ffd2843f7a10c579cc8207bf0ddf13a90d192020`  
		Last Modified: Tue, 25 Oct 2022 03:21:16 GMT  
		Size: 26.6 MB (26579293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:994ebe67dcc584cc606ff0241a3d40f7443c4b485decaf90f59e4f04a9176b41`  
		Last Modified: Tue, 25 Oct 2022 16:32:39 GMT  
		Size: 4.9 KB (4894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a0560a2515ed4bdca726252cb3f0b53970e473a78fbdeec1aa3a1430c965e83`  
		Last Modified: Tue, 25 Oct 2022 16:32:39 GMT  
		Size: 312.9 KB (312899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bc50e24b968f88c5965d3b72785fe996c6102c86ed494e029b753a0751de62e`  
		Last Modified: Tue, 25 Oct 2022 16:32:39 GMT  
		Size: 1.2 MB (1200522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d367ee67ccc6039d54e1e3e5b668d3aab4be036974a15b661a240123dee134e2`  
		Last Modified: Tue, 25 Oct 2022 16:32:39 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:535cdafbe9a8f392bf7abe74d47b97943f13e82185b02e04ec752b39362e143d`  
		Last Modified: Tue, 25 Oct 2022 16:32:38 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:bullseye` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:d8cc83a978e6ea9e6a8dc1b9a372e804b5c0edc462bc6c43ec768c21e60555ad
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.7 MB (31651307 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:399437df16b99f880af791bf9cd73401698528b10eca7fe9c7c14ffdf85a5759`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 15 Nov 2022 01:41:20 GMT
ADD file:1dad2420090b3d6ef5df8d1f7f2878b22f8687b8dba008a63800f6c74b36dee9 in / 
# Tue, 15 Nov 2022 01:41:20 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 06:33:57 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 15 Nov 2022 06:34:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 06:34:00 GMT
ENV MEMCACHED_VERSION=1.6.17
# Tue, 15 Nov 2022 06:34:00 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Tue, 15 Nov 2022 06:36:44 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 15 Nov 2022 06:36:44 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 15 Nov 2022 06:36:45 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 15 Nov 2022 06:36:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 15 Nov 2022 06:36:45 GMT
USER memcache
# Tue, 15 Nov 2022 06:36:45 GMT
EXPOSE 11211
# Tue, 15 Nov 2022 06:36:45 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:f3ac85625e767ee0ec42b5a2ef93880251cd973b86f77124c4ed39bccd2f8bf9`  
		Last Modified: Tue, 15 Nov 2022 01:44:35 GMT  
		Size: 30.1 MB (30060605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bbbe7e324eeed0563b7f3bf186f31ccc557991bd3f36c45dc3426544be9820f`  
		Last Modified: Tue, 15 Nov 2022 06:37:09 GMT  
		Size: 5.0 KB (5026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e1f82789be9f4cd6a0eac461c0ba1ecff14b86d99d7f771c3d464c632a568a9`  
		Last Modified: Tue, 15 Nov 2022 06:37:10 GMT  
		Size: 326.8 KB (326754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fbd4462ff4cf6ab23c5914b151978478f7628f8e34012c1443560b32d3749d0`  
		Last Modified: Tue, 15 Nov 2022 06:37:10 GMT  
		Size: 1.3 MB (1258516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6d98cc3893d7dc8a5d71153a8ef9f2f5cf1c0902331e4899dc080600924dd60`  
		Last Modified: Tue, 15 Nov 2022 06:37:09 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31aa0dad47e8147e308939249b6a54b60bbf95fce86c886512566ed56e7e849b`  
		Last Modified: Tue, 15 Nov 2022 06:37:09 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:bullseye` - linux; 386

```console
$ docker pull memcached@sha256:e3aee9071cc3ff7c1806ca9b34eb9437af6e6008a745ba7f4147ffc4291d7c54
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.8 MB (33786960 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e6085237b6f886afdb4094f71bac40f442ad1de3b3637e3c1585bfcb04a624c8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 25 Oct 2022 02:22:34 GMT
ADD file:14adaece72e410cf04ac21a101e5b530aab1d5e5a189a2be72d195ec0ac5e6d4 in / 
# Tue, 25 Oct 2022 02:22:35 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 07:20:13 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 25 Oct 2022 07:20:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 07:20:18 GMT
ENV MEMCACHED_VERSION=1.6.17
# Tue, 25 Oct 2022 07:20:19 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Tue, 25 Oct 2022 07:23:04 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 25 Oct 2022 07:23:06 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 25 Oct 2022 07:23:06 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 25 Oct 2022 07:23:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 25 Oct 2022 07:23:08 GMT
USER memcache
# Tue, 25 Oct 2022 07:23:09 GMT
EXPOSE 11211
# Tue, 25 Oct 2022 07:23:10 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:3c83067056c0f1bc4e162249831ac686f3a9a9c64c5366b903581580de8fcac2`  
		Last Modified: Tue, 25 Oct 2022 02:28:26 GMT  
		Size: 32.4 MB (32396384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1232ee56c032ec872d2e5ea991d027c1e52216d1a4051f8d222f68b912d45b42`  
		Last Modified: Tue, 25 Oct 2022 07:24:05 GMT  
		Size: 4.8 KB (4773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4908117cb080710efe912e54b8b241e4e0a629844c3f381b41f2bbf26ff075c`  
		Last Modified: Tue, 25 Oct 2022 07:24:05 GMT  
		Size: 130.1 KB (130136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb0aac8cf1d7145f157fa4fd43ce483440dff87bd5abe02875d25ce0886b695f`  
		Last Modified: Tue, 25 Oct 2022 07:24:05 GMT  
		Size: 1.3 MB (1255260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c924204d5c8e32a0942e6b7d634ee88768dd6ac5ea29087a32a65c99a7ba6ff1`  
		Last Modified: Tue, 25 Oct 2022 07:24:05 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d726eda9f735ceab9f8ed0a9164eb9c0fafdba0f7f63a6062416a91f3429fcba`  
		Last Modified: Tue, 25 Oct 2022 07:24:05 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:bullseye` - linux; mips64le

```console
$ docker pull memcached@sha256:f049bcc1e654030ecc7785662cdcbf3b3b678d37b8c4531b00aac4a3befc8ae1
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.0 MB (31016446 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8012bf67ed2bab40f27be5074e3c13cfbafa7809771f7ca9e37b1a0a8b846f4c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 25 Oct 2022 04:39:25 GMT
ADD file:222c5611b805658925ba615b0e69d40aa3dfa37223bc06f150909f7e944e426b in / 
# Tue, 25 Oct 2022 04:39:29 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 12:41:45 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 25 Oct 2022 12:42:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 12:42:04 GMT
ENV MEMCACHED_VERSION=1.6.17
# Tue, 25 Oct 2022 12:42:07 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Tue, 25 Oct 2022 12:49:20 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 25 Oct 2022 12:49:22 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 25 Oct 2022 12:49:27 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 25 Oct 2022 12:49:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 25 Oct 2022 12:49:32 GMT
USER memcache
# Tue, 25 Oct 2022 12:49:35 GMT
EXPOSE 11211
# Tue, 25 Oct 2022 12:49:38 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:85f344f7fa0587aa4dbdc8d09d838d444853a1789047586a0927fa09fa89bb8f`  
		Last Modified: Tue, 25 Oct 2022 04:47:25 GMT  
		Size: 29.6 MB (29640590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7a12644fc5792f35befe7c202cf030de6c94a66724b8a155a72938de6ba5be8`  
		Last Modified: Tue, 25 Oct 2022 12:50:06 GMT  
		Size: 4.9 KB (4860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2749b6a3da5bbac1ff042ff4b831376fe7ff1dfe8ea46f76ec4fd69b29a6e0c`  
		Last Modified: Tue, 25 Oct 2022 12:50:06 GMT  
		Size: 117.2 KB (117161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0662db55cc1eff4f9bf54440c689f52c2e5539a162498723180d864445dc2b00`  
		Last Modified: Tue, 25 Oct 2022 12:50:07 GMT  
		Size: 1.3 MB (1253428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f93aa5923fe43f7676ff9f6b0fd685956e3263e906141e6a70cc7373718bd1f`  
		Last Modified: Tue, 25 Oct 2022 12:50:06 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1c058e2a644d5a56557615dbc4e91ebf395a9439e7727c6e1178955fd43617e`  
		Last Modified: Tue, 25 Oct 2022 12:50:06 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:bullseye` - linux; ppc64le

```console
$ docker pull memcached@sha256:553421fd8f3d32bb2617bb4b00975fab25b2fe623e26196a61a119d9d7570a2e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.0 MB (36978502 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f5ce94de964ddd8c8e152c3dc692aff36b1167684cc0fb8639d7e043d37328e5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 25 Oct 2022 03:13:50 GMT
ADD file:1f622759c37363caaa6e6b14831ec9369303345c096f3a018eba66a620b08d26 in / 
# Tue, 25 Oct 2022 03:13:52 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 07:48:09 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 25 Oct 2022 07:48:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 07:48:16 GMT
ENV MEMCACHED_VERSION=1.6.17
# Tue, 25 Oct 2022 07:48:16 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Tue, 25 Oct 2022 07:51:10 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 25 Oct 2022 07:51:10 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 25 Oct 2022 07:51:11 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 25 Oct 2022 07:51:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 25 Oct 2022 07:51:12 GMT
USER memcache
# Tue, 25 Oct 2022 07:51:12 GMT
EXPOSE 11211
# Tue, 25 Oct 2022 07:51:13 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:6d95b62526dd55d76e7ec2bd4015a327b5bb37161f2ffe8bc2bb08d34a677716`  
		Last Modified: Tue, 25 Oct 2022 03:19:31 GMT  
		Size: 35.3 MB (35290086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38cdaa5a3d4086114340b1f394822bcb2afcee2d908da54f57225ec71892cb8b`  
		Last Modified: Tue, 25 Oct 2022 07:52:04 GMT  
		Size: 5.0 KB (4980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37a2da29bae3161a010dbd4df1749dce8d78696b30b794728b2db32eaadf6a6e`  
		Last Modified: Tue, 25 Oct 2022 07:52:04 GMT  
		Size: 357.8 KB (357789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec839878fc66a5174fdeaaed2878170b2f118dbfed4fee71fbae773e4d417cd9`  
		Last Modified: Tue, 25 Oct 2022 07:52:04 GMT  
		Size: 1.3 MB (1325239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c246039e792853c8967ab74e3540d8bfb015c0aba44606a2747b0752ffe904e8`  
		Last Modified: Tue, 25 Oct 2022 07:52:03 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f476fff8a8d96fd6768c784e4cd8641659aca9a6cc0d48e598e8a17cb977f69`  
		Last Modified: Tue, 25 Oct 2022 07:52:04 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:bullseye` - linux; s390x

```console
$ docker pull memcached@sha256:88e18a84904384a6520db93e0fbd97bd6bdeace8fafdeab31fce33d166876522
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.2 MB (31223977 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eec81bbdae0d9097a444bac021f2841ce7b087fab94e15356609cea32bbce701`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 25 Oct 2022 01:14:42 GMT
ADD file:1bb8efa7f80e494b9d2831490a7e74810350c1f9ee2d100596d2e1cb4c62f529 in / 
# Tue, 25 Oct 2022 01:14:44 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 03:07:05 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 25 Oct 2022 03:07:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 03:07:08 GMT
ENV MEMCACHED_VERSION=1.6.17
# Tue, 25 Oct 2022 03:07:08 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Tue, 25 Oct 2022 03:10:51 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 25 Oct 2022 03:10:51 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 25 Oct 2022 03:10:52 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 25 Oct 2022 03:10:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 25 Oct 2022 03:10:52 GMT
USER memcache
# Tue, 25 Oct 2022 03:10:52 GMT
EXPOSE 11211
# Tue, 25 Oct 2022 03:10:52 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:abc14eb2518761d53b91fc564a31b657914f96b531f99a74ac8268f0717b007e`  
		Last Modified: Tue, 25 Oct 2022 01:19:01 GMT  
		Size: 29.7 MB (29650722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bdd9cb0b6aed822e02f6c6711350230f4852b1ce3930c0e5a177857d409133a`  
		Last Modified: Tue, 25 Oct 2022 03:11:50 GMT  
		Size: 5.0 KB (5026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0597b9439fdec902e7d8ab65b2f88027f5fe41e918d89a0d1676d9de810e97ca`  
		Last Modified: Tue, 25 Oct 2022 03:11:50 GMT  
		Size: 324.9 KB (324923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e33bdc5b491f361fcedd9c233aa410a0e5e986c2e1725139821a859b085fe34`  
		Last Modified: Tue, 25 Oct 2022 03:11:51 GMT  
		Size: 1.2 MB (1242899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08b443e7a4cb5a761a5e2be38d56de166382ac65f26dc61292b9eecd50c77a9c`  
		Last Modified: Tue, 25 Oct 2022 03:11:50 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06d7ba123cdcd34979aa40c10ffa0180a88acd0826020eb484d6063120689d4b`  
		Last Modified: Tue, 25 Oct 2022 03:11:50 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
