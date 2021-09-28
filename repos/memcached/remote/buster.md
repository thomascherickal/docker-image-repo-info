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
