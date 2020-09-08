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
$ docker pull memcached@sha256:9cdffaa615cf536e8474900776d50568a912d637649a749c92d118a9cce2ab75
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
$ docker pull memcached@sha256:355abd5b7bc78b4aefb544a11f806117d9b3c3c9ee17d9dfc89598eff9e6c7b8
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.5 MB (30493478 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1412702e49d1f90905c4f6b88157813f256be2aef74f93bc405d749bf2d4bc9e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 04 Aug 2020 15:42:51 GMT
ADD file:3af3091e7d2bb40bc1e6550eb5ea290badc6bbf3339105626f245a963cc11450 in / 
# Tue, 04 Aug 2020 15:42:51 GMT
CMD ["bash"]
# Wed, 05 Aug 2020 00:11:59 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 05 Aug 2020 00:12:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 08 Sep 2020 19:38:38 GMT
ENV MEMCACHED_VERSION=1.6.7
# Tue, 08 Sep 2020 19:38:38 GMT
ENV MEMCACHED_SHA1=49336bb0a4b7ad296422b08148581ed54edf32d0
# Tue, 08 Sep 2020 19:58:10 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 08 Sep 2020 19:58:10 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 08 Sep 2020 19:58:10 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 08 Sep 2020 19:58:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 08 Sep 2020 19:58:11 GMT
USER memcache
# Tue, 08 Sep 2020 19:58:11 GMT
EXPOSE 11211
# Tue, 08 Sep 2020 19:58:11 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:bf59529304463f62efa7179fa1a32718a611528cc4ce9f30c0d1bbc6724ec3fb`  
		Last Modified: Tue, 04 Aug 2020 15:49:09 GMT  
		Size: 27.1 MB (27092121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b529ccb9885e0a07fb36b22af61c8f7c5a9b0551f5177ba1debf8de757b3631c`  
		Last Modified: Wed, 05 Aug 2020 00:21:46 GMT  
		Size: 5.0 KB (4984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85fac251bdd1dc7c979fdff2cac12c56f7545ad74d0cbccae793c2d3e0f271e8`  
		Last Modified: Wed, 05 Aug 2020 00:21:47 GMT  
		Size: 2.2 MB (2196515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60c0a99dabb56d767ce262b4b22be4a626ad6afec3f17f0a7ed2f78f1a41ec1b`  
		Last Modified: Tue, 08 Sep 2020 20:18:16 GMT  
		Size: 1.2 MB (1199450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed2c76ea7ac6f2e3f5fd02bb7c068a1e7d0f70ce2dfc0ba5039205c90dd1f2cf`  
		Last Modified: Tue, 08 Sep 2020 20:18:15 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:087645fe651b24fda3abb9ff4a0031373f4bcb60df2fb39bdf65dbb367ae38fc`  
		Last Modified: Tue, 08 Sep 2020 20:18:15 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1` - linux; arm variant v5

```console
$ docker pull memcached@sha256:45b13f1c38ec693a4b23dddef22b456239af5454437a27adc75a138382532b74
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.9 MB (27911379 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7516c2ec9377d95bfd1f67e9016ec35f378991779622a9c4bbe18f3e6e0cb077`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 04 Aug 2020 03:13:17 GMT
ADD file:1a4c984d1bdb683e240e8bbdfeae45b146e1f8003444ce04a84096e58a437853 in / 
# Tue, 04 Aug 2020 03:13:27 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 06:51:04 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 04 Aug 2020 06:51:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 08 Sep 2020 21:05:50 GMT
ENV MEMCACHED_VERSION=1.6.7
# Tue, 08 Sep 2020 21:06:00 GMT
ENV MEMCACHED_SHA1=49336bb0a4b7ad296422b08148581ed54edf32d0
# Tue, 08 Sep 2020 21:17:20 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 08 Sep 2020 21:17:37 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 08 Sep 2020 21:18:16 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 08 Sep 2020 21:18:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 08 Sep 2020 21:18:33 GMT
USER memcache
# Tue, 08 Sep 2020 21:18:40 GMT
EXPOSE 11211
# Tue, 08 Sep 2020 21:18:47 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:4eb4ac68461c572fdc826bae247c43484a232f91f165666714ce0f5f052b0bab`  
		Last Modified: Tue, 04 Aug 2020 03:34:09 GMT  
		Size: 24.8 MB (24836059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cb53bba0491bf847d6fccec1e97acf8b40962d63009b9d14e88dd262072722c`  
		Last Modified: Tue, 04 Aug 2020 07:02:42 GMT  
		Size: 4.9 KB (4896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43a44e4bfe83944a327bc58ffbfb7eef92252ca9078f7781a6452da48f852499`  
		Last Modified: Tue, 04 Aug 2020 07:02:42 GMT  
		Size: 1.9 MB (1896867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b272b500ec6183577a6b13721c41bd6c7d1686ffe22fe761b226fea78109fd7`  
		Last Modified: Tue, 08 Sep 2020 21:19:01 GMT  
		Size: 1.2 MB (1173148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db2c0a741733ce4c321f325cf3a6306edaac69edb68f63ca04017648923ce2c4`  
		Last Modified: Tue, 08 Sep 2020 21:19:01 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b763edbb9dd540a12cdbaa66b09c4462b45cb25ce9b4413f6ba8e75890459c0`  
		Last Modified: Tue, 08 Sep 2020 21:19:01 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1` - linux; arm variant v7

```console
$ docker pull memcached@sha256:2144f5d0ed52bbfe4170b2f27957a05b77b7a18e399a8f0acb523f1ee91332cd
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.7 MB (25651244 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5380de28b2ec24580bfbe5a9b563fda4b9ee55df259ae10ef0159079669aa6b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 04 Aug 2020 04:56:49 GMT
ADD file:16169b615697a126ae57dc01f7c4902fb9d9bc1e8595af43293700fa030808cc in / 
# Tue, 04 Aug 2020 04:56:51 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 11:21:50 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 04 Aug 2020 11:22:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 11:22:03 GMT
ENV MEMCACHED_VERSION=1.6.6
# Tue, 04 Aug 2020 11:22:05 GMT
ENV MEMCACHED_SHA1=d8895b12dc9fc82b389f1713e2c09cc6ca3d03e4
# Tue, 04 Aug 2020 11:32:23 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 04 Aug 2020 11:32:24 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 04 Aug 2020 11:32:27 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 04 Aug 2020 11:32:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Aug 2020 11:32:29 GMT
USER memcache
# Tue, 04 Aug 2020 11:32:30 GMT
EXPOSE 11211
# Tue, 04 Aug 2020 11:32:30 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:d7fe0a1b85ffd3158c62ab2e06ab004dc957cd133ba7129fb9c69c4586f407c9`  
		Last Modified: Tue, 04 Aug 2020 05:05:19 GMT  
		Size: 22.7 MB (22699792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a552abd0d66729ea122ed43216a635d2b40c0c34b82d247448a62280bda2b1b`  
		Last Modified: Tue, 04 Aug 2020 11:32:49 GMT  
		Size: 4.9 KB (4895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe0572bbccbb4def0fbbff844d9aefa4723ad29312e0b2952505927355e6da5a`  
		Last Modified: Tue, 04 Aug 2020 11:32:50 GMT  
		Size: 1.8 MB (1811523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f0c7c1daf8e87852846cbec2c963c032cd1de0f40ba57df3329e18c2572946d`  
		Last Modified: Tue, 04 Aug 2020 11:32:50 GMT  
		Size: 1.1 MB (1134625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f17117691f08ee67cafe0d9ef1d29943dd301aea76f85c550119df2c555c2d8`  
		Last Modified: Tue, 04 Aug 2020 11:32:50 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63cdfdb6ebae5cb43273e7c9c13a91ba971c74630c5eaaddccaea894d296f9e8`  
		Last Modified: Tue, 04 Aug 2020 11:32:50 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:8b8d4040593aaa099462192d942483db796bb14d06afee08b8f98bba575258b7
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.1 MB (29099944 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba6a2a00e032b0a3b41f234b4cd1ee7de2255f1f7315bc0ad1ec2186e379a469`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 04 Aug 2020 06:57:29 GMT
ADD file:90ba7821623ab55fc1073647cc611cc45f5e306ade734910e587021971483eec in / 
# Tue, 04 Aug 2020 06:57:31 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 14:50:02 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 04 Aug 2020 14:50:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 08 Sep 2020 21:04:00 GMT
ENV MEMCACHED_VERSION=1.6.7
# Tue, 08 Sep 2020 21:04:09 GMT
ENV MEMCACHED_SHA1=49336bb0a4b7ad296422b08148581ed54edf32d0
# Tue, 08 Sep 2020 21:15:12 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 08 Sep 2020 21:15:19 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 08 Sep 2020 21:15:35 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 08 Sep 2020 21:15:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 08 Sep 2020 21:15:37 GMT
USER memcache
# Tue, 08 Sep 2020 21:15:38 GMT
EXPOSE 11211
# Tue, 08 Sep 2020 21:15:38 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:3742235f1882fee5cca1effc4ca0f0c7c180bbe169800a85daedcf3968b0d8f0`  
		Last Modified: Tue, 04 Aug 2020 07:04:03 GMT  
		Size: 25.8 MB (25849301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d9010ac788ddccd1668bdc1b6eb6896fc768e4ad050fdcfe39e0f3c6fc4269b`  
		Last Modified: Tue, 04 Aug 2020 15:01:00 GMT  
		Size: 5.0 KB (5024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:064151e7e34f6f91e46091d50428c5f0aad91b86432a93fbf8363b0c7cf43f48`  
		Last Modified: Tue, 04 Aug 2020 15:00:59 GMT  
		Size: 2.1 MB (2075003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1e261d39aaa0c8d085e073c40bce6ab4d17492978f19d2ebcf6b8527b4c755b`  
		Last Modified: Tue, 08 Sep 2020 21:27:04 GMT  
		Size: 1.2 MB (1170207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:340cde0def1487d362e2a355d781db751ec18c50e06d3749d07920b5665a238e`  
		Last Modified: Tue, 08 Sep 2020 21:27:05 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0dc0954cc2aa31fe25c0ccc4baf6c2dc9855faa9c93070d64f19da484cb362f`  
		Last Modified: Tue, 08 Sep 2020 21:27:05 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1` - linux; 386

```console
$ docker pull memcached@sha256:f0d08a896e1a4e545e5caf597c0d88d1a9d5dd9c49ffafff25c5b1293a9f7eec
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.2 MB (31161322 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc41ce3e1c9b5084b98d7961997e919ecfc4e9bb01fe696c0e21ae1ff16ae0f2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 04 Aug 2020 03:37:35 GMT
ADD file:cc791c21e6022a12dd1445a35f4cca9392ad8edfe34ea5852f3e87862c943628 in / 
# Tue, 04 Aug 2020 03:37:35 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 05:58:02 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 04 Aug 2020 05:58:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 08 Sep 2020 19:54:32 GMT
ENV MEMCACHED_VERSION=1.6.7
# Tue, 08 Sep 2020 19:54:32 GMT
ENV MEMCACHED_SHA1=49336bb0a4b7ad296422b08148581ed54edf32d0
# Tue, 08 Sep 2020 20:04:14 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 08 Sep 2020 20:04:14 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 08 Sep 2020 20:04:15 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 08 Sep 2020 20:04:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 08 Sep 2020 20:04:15 GMT
USER memcache
# Tue, 08 Sep 2020 20:04:16 GMT
EXPOSE 11211
# Tue, 08 Sep 2020 20:04:16 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:23ad22c16ab9d635a179d5d341096c34912941507b0c77ac97083b9795d8516f`  
		Last Modified: Tue, 04 Aug 2020 03:42:33 GMT  
		Size: 27.8 MB (27750435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f95eecb817da01910205081ea555757eb2fc5f1fd3a0844775943d55e1a10f4f`  
		Last Modified: Tue, 04 Aug 2020 06:08:21 GMT  
		Size: 4.9 KB (4894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b54cd9b7aa7674853d5ce4059daf598ccb281afb321a8f8d09a9b6e40223a9e7`  
		Last Modified: Tue, 04 Aug 2020 06:08:22 GMT  
		Size: 2.2 MB (2208142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:516ee7394637045940f9a0678b447be8f6b23ee3c9140baed49b5291be183b43`  
		Last Modified: Tue, 08 Sep 2020 20:14:40 GMT  
		Size: 1.2 MB (1197445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b2882adacd9ea9fd9e0e7002a6e785fae3eecd005b6d3f60667335adf2bf4d2`  
		Last Modified: Tue, 08 Sep 2020 20:14:39 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:752587d11a4176c1da4c2d1b00a16ffccd29ff01097c315a4ae64794ec760349`  
		Last Modified: Tue, 08 Sep 2020 20:14:39 GMT  
		Size: 119.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1` - linux; mips64le

```console
$ docker pull memcached@sha256:c1037de0c972b61f44c483a79f39039f734780f592133f26b6ead3cf9487101f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.7 MB (28726687 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f8cac462c662ef1bf25313d9053734ace48d255b60cad631b177adb6b7db6ee`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 04 Aug 2020 06:42:23 GMT
ADD file:4164c71b841ba2c1f213c9fdc073ec3d4c7d79dadfcd9d771768750a3085d616 in / 
# Tue, 04 Aug 2020 06:42:24 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 11:05:29 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 04 Aug 2020 11:05:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 11:05:42 GMT
ENV MEMCACHED_VERSION=1.6.6
# Tue, 04 Aug 2020 11:05:42 GMT
ENV MEMCACHED_SHA1=d8895b12dc9fc82b389f1713e2c09cc6ca3d03e4
# Tue, 04 Aug 2020 11:17:25 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 04 Aug 2020 11:17:25 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 04 Aug 2020 11:17:27 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 04 Aug 2020 11:17:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Aug 2020 11:17:28 GMT
USER memcache
# Tue, 04 Aug 2020 11:17:28 GMT
EXPOSE 11211
# Tue, 04 Aug 2020 11:17:28 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:1333f76e75c0136aa2eb56b14271ef57d1f975f40fe2a56536d99b7c86c3aa29`  
		Last Modified: Tue, 04 Aug 2020 06:48:41 GMT  
		Size: 25.8 MB (25762724 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e8b074644a235b1bb35f407f447fc6f33e3511e5cf837f33d1ccf0b9a039f4b`  
		Last Modified: Tue, 04 Aug 2020 11:17:48 GMT  
		Size: 5.0 KB (4980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:358e4488d4f6c21470ee9d8366dc5f304ade7c0ef3852eea9d2678e8b3102810`  
		Last Modified: Tue, 04 Aug 2020 11:17:49 GMT  
		Size: 1.8 MB (1776037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07209a5f05b07eff5f25acb525649cbca01da609b40355269d50a0b1a8afd1c7`  
		Last Modified: Tue, 04 Aug 2020 11:17:48 GMT  
		Size: 1.2 MB (1182538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:662db051984f433760ae7b7564ca3b00d4822012405825bae37fc850edd7bc79`  
		Last Modified: Tue, 04 Aug 2020 11:17:47 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7ee1c64bb768a6837da56bfbc48058253ec0cdb0666155f4810c2a16bd18851`  
		Last Modified: Tue, 04 Aug 2020 11:17:47 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1` - linux; ppc64le

```console
$ docker pull memcached@sha256:92643ad382b13ec8a5833b8e73e95ed5dc6ea7d1f04146fd495b66791f99d876
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.1 MB (34071500 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c77d50f314b2c2877792edab86d1db23e830478326e35ee02dd4cfdd8656dde4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 04 Aug 2020 04:45:34 GMT
ADD file:3bab6d2b62fe6a548ee28480d9eebf3251e942c4bb66362b87396b73af7aa586 in / 
# Tue, 04 Aug 2020 04:45:40 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 09:12:47 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 04 Aug 2020 09:13:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 08 Sep 2020 20:46:58 GMT
ENV MEMCACHED_VERSION=1.6.7
# Tue, 08 Sep 2020 20:47:05 GMT
ENV MEMCACHED_SHA1=49336bb0a4b7ad296422b08148581ed54edf32d0
# Tue, 08 Sep 2020 21:01:47 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 08 Sep 2020 21:01:51 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 08 Sep 2020 21:02:04 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 08 Sep 2020 21:02:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 08 Sep 2020 21:02:17 GMT
USER memcache
# Tue, 08 Sep 2020 21:02:24 GMT
EXPOSE 11211
# Tue, 08 Sep 2020 21:02:29 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:0827434caf9c0b71f95b3bcbe29d60f4f887199db59b3994d9315c478def41c3`  
		Last Modified: Tue, 04 Aug 2020 04:53:24 GMT  
		Size: 30.5 MB (30517844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:148c6ee7500ba1bf209ecab4590fcbcccc43e47abc7b4c327f95def3fb988a24`  
		Last Modified: Tue, 04 Aug 2020 09:26:02 GMT  
		Size: 5.0 KB (4984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b12a8a57075aa4c0c08c713d3f6901ab119bac72ca37a1155ef71a64d7cce6c`  
		Last Modified: Tue, 04 Aug 2020 09:26:03 GMT  
		Size: 2.3 MB (2322731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7760164dbee558e327c1ba89f2d6706a978d87b884f56558b6ba026110d966b`  
		Last Modified: Tue, 08 Sep 2020 21:13:49 GMT  
		Size: 1.2 MB (1225532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ead7201825bf4619985e151116fb21bf149927b6b1384bb8a2d2cf1f38271a81`  
		Last Modified: Tue, 08 Sep 2020 21:13:49 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4b36e2776fcec754f6f51e67d7580f566da6ef03ae5deadca6535f3a2f7bd18`  
		Last Modified: Tue, 08 Sep 2020 21:13:50 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1` - linux; s390x

```console
$ docker pull memcached@sha256:33252d5979791433f6abd86d4cd681e52d53e34b985e7e5c40831b39e76b03c8
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.8 MB (28789297 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:512f36fcfab08338e9c9d98c61771ba16dd3231bb06e1d716f4d7d8b58b7a8dd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 04 Aug 2020 01:17:16 GMT
ADD file:2ffa27c57800f9370adbaecca870158ec38c3d25a58b8803e2447c5e9320c5bb in / 
# Tue, 04 Aug 2020 01:17:17 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 02:50:25 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 04 Aug 2020 02:50:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 08 Sep 2020 19:56:37 GMT
ENV MEMCACHED_VERSION=1.6.7
# Tue, 08 Sep 2020 19:56:37 GMT
ENV MEMCACHED_SHA1=49336bb0a4b7ad296422b08148581ed54edf32d0
# Tue, 08 Sep 2020 20:05:26 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 08 Sep 2020 20:05:26 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 08 Sep 2020 20:05:26 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 08 Sep 2020 20:05:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 08 Sep 2020 20:05:27 GMT
USER memcache
# Tue, 08 Sep 2020 20:05:27 GMT
EXPOSE 11211
# Tue, 08 Sep 2020 20:05:27 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:0c46adfa2de4a7b7eb1fe2f0cb928f9e15a4cc94b7b975f13392f397cbfb0f2c`  
		Last Modified: Tue, 04 Aug 2020 01:20:03 GMT  
		Size: 25.7 MB (25707641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e4b36fc30f49aa14be390857b0e79628a680feeffb91e7c86f6381aeddcbf5c`  
		Last Modified: Tue, 04 Aug 2020 02:59:46 GMT  
		Size: 5.0 KB (5024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61f47a7c59d5f7d947ab1b93bb5d74d64ee1e84f8358eb1d78a4195ae8e4fa4e`  
		Last Modified: Tue, 04 Aug 2020 02:59:46 GMT  
		Size: 1.9 MB (1886090 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0683d3462c39632079df86d4267c6a0710f7bf718aaad9bd7468918022618cb6`  
		Last Modified: Tue, 08 Sep 2020 20:14:49 GMT  
		Size: 1.2 MB (1190135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06c729cc605ad7546ad2c9c45eda0473f5469a44ab7490cf1351134f839d6daf`  
		Last Modified: Tue, 08 Sep 2020 20:14:49 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7a2f84d1b6b2f9800f3fc44acccea46505b7891a807dcc8b1e5b5516d88b38c`  
		Last Modified: Tue, 08 Sep 2020 20:14:48 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:1.6`

```console
$ docker pull memcached@sha256:9cdffaa615cf536e8474900776d50568a912d637649a749c92d118a9cce2ab75
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
$ docker pull memcached@sha256:355abd5b7bc78b4aefb544a11f806117d9b3c3c9ee17d9dfc89598eff9e6c7b8
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.5 MB (30493478 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1412702e49d1f90905c4f6b88157813f256be2aef74f93bc405d749bf2d4bc9e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 04 Aug 2020 15:42:51 GMT
ADD file:3af3091e7d2bb40bc1e6550eb5ea290badc6bbf3339105626f245a963cc11450 in / 
# Tue, 04 Aug 2020 15:42:51 GMT
CMD ["bash"]
# Wed, 05 Aug 2020 00:11:59 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 05 Aug 2020 00:12:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 08 Sep 2020 19:38:38 GMT
ENV MEMCACHED_VERSION=1.6.7
# Tue, 08 Sep 2020 19:38:38 GMT
ENV MEMCACHED_SHA1=49336bb0a4b7ad296422b08148581ed54edf32d0
# Tue, 08 Sep 2020 19:58:10 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 08 Sep 2020 19:58:10 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 08 Sep 2020 19:58:10 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 08 Sep 2020 19:58:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 08 Sep 2020 19:58:11 GMT
USER memcache
# Tue, 08 Sep 2020 19:58:11 GMT
EXPOSE 11211
# Tue, 08 Sep 2020 19:58:11 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:bf59529304463f62efa7179fa1a32718a611528cc4ce9f30c0d1bbc6724ec3fb`  
		Last Modified: Tue, 04 Aug 2020 15:49:09 GMT  
		Size: 27.1 MB (27092121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b529ccb9885e0a07fb36b22af61c8f7c5a9b0551f5177ba1debf8de757b3631c`  
		Last Modified: Wed, 05 Aug 2020 00:21:46 GMT  
		Size: 5.0 KB (4984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85fac251bdd1dc7c979fdff2cac12c56f7545ad74d0cbccae793c2d3e0f271e8`  
		Last Modified: Wed, 05 Aug 2020 00:21:47 GMT  
		Size: 2.2 MB (2196515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60c0a99dabb56d767ce262b4b22be4a626ad6afec3f17f0a7ed2f78f1a41ec1b`  
		Last Modified: Tue, 08 Sep 2020 20:18:16 GMT  
		Size: 1.2 MB (1199450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed2c76ea7ac6f2e3f5fd02bb7c068a1e7d0f70ce2dfc0ba5039205c90dd1f2cf`  
		Last Modified: Tue, 08 Sep 2020 20:18:15 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:087645fe651b24fda3abb9ff4a0031373f4bcb60df2fb39bdf65dbb367ae38fc`  
		Last Modified: Tue, 08 Sep 2020 20:18:15 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6` - linux; arm variant v5

```console
$ docker pull memcached@sha256:45b13f1c38ec693a4b23dddef22b456239af5454437a27adc75a138382532b74
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.9 MB (27911379 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7516c2ec9377d95bfd1f67e9016ec35f378991779622a9c4bbe18f3e6e0cb077`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 04 Aug 2020 03:13:17 GMT
ADD file:1a4c984d1bdb683e240e8bbdfeae45b146e1f8003444ce04a84096e58a437853 in / 
# Tue, 04 Aug 2020 03:13:27 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 06:51:04 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 04 Aug 2020 06:51:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 08 Sep 2020 21:05:50 GMT
ENV MEMCACHED_VERSION=1.6.7
# Tue, 08 Sep 2020 21:06:00 GMT
ENV MEMCACHED_SHA1=49336bb0a4b7ad296422b08148581ed54edf32d0
# Tue, 08 Sep 2020 21:17:20 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 08 Sep 2020 21:17:37 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 08 Sep 2020 21:18:16 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 08 Sep 2020 21:18:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 08 Sep 2020 21:18:33 GMT
USER memcache
# Tue, 08 Sep 2020 21:18:40 GMT
EXPOSE 11211
# Tue, 08 Sep 2020 21:18:47 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:4eb4ac68461c572fdc826bae247c43484a232f91f165666714ce0f5f052b0bab`  
		Last Modified: Tue, 04 Aug 2020 03:34:09 GMT  
		Size: 24.8 MB (24836059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cb53bba0491bf847d6fccec1e97acf8b40962d63009b9d14e88dd262072722c`  
		Last Modified: Tue, 04 Aug 2020 07:02:42 GMT  
		Size: 4.9 KB (4896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43a44e4bfe83944a327bc58ffbfb7eef92252ca9078f7781a6452da48f852499`  
		Last Modified: Tue, 04 Aug 2020 07:02:42 GMT  
		Size: 1.9 MB (1896867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b272b500ec6183577a6b13721c41bd6c7d1686ffe22fe761b226fea78109fd7`  
		Last Modified: Tue, 08 Sep 2020 21:19:01 GMT  
		Size: 1.2 MB (1173148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db2c0a741733ce4c321f325cf3a6306edaac69edb68f63ca04017648923ce2c4`  
		Last Modified: Tue, 08 Sep 2020 21:19:01 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b763edbb9dd540a12cdbaa66b09c4462b45cb25ce9b4413f6ba8e75890459c0`  
		Last Modified: Tue, 08 Sep 2020 21:19:01 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6` - linux; arm variant v7

```console
$ docker pull memcached@sha256:2144f5d0ed52bbfe4170b2f27957a05b77b7a18e399a8f0acb523f1ee91332cd
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.7 MB (25651244 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5380de28b2ec24580bfbe5a9b563fda4b9ee55df259ae10ef0159079669aa6b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 04 Aug 2020 04:56:49 GMT
ADD file:16169b615697a126ae57dc01f7c4902fb9d9bc1e8595af43293700fa030808cc in / 
# Tue, 04 Aug 2020 04:56:51 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 11:21:50 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 04 Aug 2020 11:22:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 11:22:03 GMT
ENV MEMCACHED_VERSION=1.6.6
# Tue, 04 Aug 2020 11:22:05 GMT
ENV MEMCACHED_SHA1=d8895b12dc9fc82b389f1713e2c09cc6ca3d03e4
# Tue, 04 Aug 2020 11:32:23 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 04 Aug 2020 11:32:24 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 04 Aug 2020 11:32:27 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 04 Aug 2020 11:32:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Aug 2020 11:32:29 GMT
USER memcache
# Tue, 04 Aug 2020 11:32:30 GMT
EXPOSE 11211
# Tue, 04 Aug 2020 11:32:30 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:d7fe0a1b85ffd3158c62ab2e06ab004dc957cd133ba7129fb9c69c4586f407c9`  
		Last Modified: Tue, 04 Aug 2020 05:05:19 GMT  
		Size: 22.7 MB (22699792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a552abd0d66729ea122ed43216a635d2b40c0c34b82d247448a62280bda2b1b`  
		Last Modified: Tue, 04 Aug 2020 11:32:49 GMT  
		Size: 4.9 KB (4895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe0572bbccbb4def0fbbff844d9aefa4723ad29312e0b2952505927355e6da5a`  
		Last Modified: Tue, 04 Aug 2020 11:32:50 GMT  
		Size: 1.8 MB (1811523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f0c7c1daf8e87852846cbec2c963c032cd1de0f40ba57df3329e18c2572946d`  
		Last Modified: Tue, 04 Aug 2020 11:32:50 GMT  
		Size: 1.1 MB (1134625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f17117691f08ee67cafe0d9ef1d29943dd301aea76f85c550119df2c555c2d8`  
		Last Modified: Tue, 04 Aug 2020 11:32:50 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63cdfdb6ebae5cb43273e7c9c13a91ba971c74630c5eaaddccaea894d296f9e8`  
		Last Modified: Tue, 04 Aug 2020 11:32:50 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:8b8d4040593aaa099462192d942483db796bb14d06afee08b8f98bba575258b7
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.1 MB (29099944 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba6a2a00e032b0a3b41f234b4cd1ee7de2255f1f7315bc0ad1ec2186e379a469`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 04 Aug 2020 06:57:29 GMT
ADD file:90ba7821623ab55fc1073647cc611cc45f5e306ade734910e587021971483eec in / 
# Tue, 04 Aug 2020 06:57:31 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 14:50:02 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 04 Aug 2020 14:50:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 08 Sep 2020 21:04:00 GMT
ENV MEMCACHED_VERSION=1.6.7
# Tue, 08 Sep 2020 21:04:09 GMT
ENV MEMCACHED_SHA1=49336bb0a4b7ad296422b08148581ed54edf32d0
# Tue, 08 Sep 2020 21:15:12 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 08 Sep 2020 21:15:19 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 08 Sep 2020 21:15:35 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 08 Sep 2020 21:15:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 08 Sep 2020 21:15:37 GMT
USER memcache
# Tue, 08 Sep 2020 21:15:38 GMT
EXPOSE 11211
# Tue, 08 Sep 2020 21:15:38 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:3742235f1882fee5cca1effc4ca0f0c7c180bbe169800a85daedcf3968b0d8f0`  
		Last Modified: Tue, 04 Aug 2020 07:04:03 GMT  
		Size: 25.8 MB (25849301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d9010ac788ddccd1668bdc1b6eb6896fc768e4ad050fdcfe39e0f3c6fc4269b`  
		Last Modified: Tue, 04 Aug 2020 15:01:00 GMT  
		Size: 5.0 KB (5024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:064151e7e34f6f91e46091d50428c5f0aad91b86432a93fbf8363b0c7cf43f48`  
		Last Modified: Tue, 04 Aug 2020 15:00:59 GMT  
		Size: 2.1 MB (2075003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1e261d39aaa0c8d085e073c40bce6ab4d17492978f19d2ebcf6b8527b4c755b`  
		Last Modified: Tue, 08 Sep 2020 21:27:04 GMT  
		Size: 1.2 MB (1170207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:340cde0def1487d362e2a355d781db751ec18c50e06d3749d07920b5665a238e`  
		Last Modified: Tue, 08 Sep 2020 21:27:05 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0dc0954cc2aa31fe25c0ccc4baf6c2dc9855faa9c93070d64f19da484cb362f`  
		Last Modified: Tue, 08 Sep 2020 21:27:05 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6` - linux; 386

```console
$ docker pull memcached@sha256:f0d08a896e1a4e545e5caf597c0d88d1a9d5dd9c49ffafff25c5b1293a9f7eec
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.2 MB (31161322 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc41ce3e1c9b5084b98d7961997e919ecfc4e9bb01fe696c0e21ae1ff16ae0f2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 04 Aug 2020 03:37:35 GMT
ADD file:cc791c21e6022a12dd1445a35f4cca9392ad8edfe34ea5852f3e87862c943628 in / 
# Tue, 04 Aug 2020 03:37:35 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 05:58:02 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 04 Aug 2020 05:58:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 08 Sep 2020 19:54:32 GMT
ENV MEMCACHED_VERSION=1.6.7
# Tue, 08 Sep 2020 19:54:32 GMT
ENV MEMCACHED_SHA1=49336bb0a4b7ad296422b08148581ed54edf32d0
# Tue, 08 Sep 2020 20:04:14 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 08 Sep 2020 20:04:14 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 08 Sep 2020 20:04:15 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 08 Sep 2020 20:04:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 08 Sep 2020 20:04:15 GMT
USER memcache
# Tue, 08 Sep 2020 20:04:16 GMT
EXPOSE 11211
# Tue, 08 Sep 2020 20:04:16 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:23ad22c16ab9d635a179d5d341096c34912941507b0c77ac97083b9795d8516f`  
		Last Modified: Tue, 04 Aug 2020 03:42:33 GMT  
		Size: 27.8 MB (27750435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f95eecb817da01910205081ea555757eb2fc5f1fd3a0844775943d55e1a10f4f`  
		Last Modified: Tue, 04 Aug 2020 06:08:21 GMT  
		Size: 4.9 KB (4894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b54cd9b7aa7674853d5ce4059daf598ccb281afb321a8f8d09a9b6e40223a9e7`  
		Last Modified: Tue, 04 Aug 2020 06:08:22 GMT  
		Size: 2.2 MB (2208142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:516ee7394637045940f9a0678b447be8f6b23ee3c9140baed49b5291be183b43`  
		Last Modified: Tue, 08 Sep 2020 20:14:40 GMT  
		Size: 1.2 MB (1197445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b2882adacd9ea9fd9e0e7002a6e785fae3eecd005b6d3f60667335adf2bf4d2`  
		Last Modified: Tue, 08 Sep 2020 20:14:39 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:752587d11a4176c1da4c2d1b00a16ffccd29ff01097c315a4ae64794ec760349`  
		Last Modified: Tue, 08 Sep 2020 20:14:39 GMT  
		Size: 119.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6` - linux; mips64le

```console
$ docker pull memcached@sha256:c1037de0c972b61f44c483a79f39039f734780f592133f26b6ead3cf9487101f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.7 MB (28726687 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f8cac462c662ef1bf25313d9053734ace48d255b60cad631b177adb6b7db6ee`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 04 Aug 2020 06:42:23 GMT
ADD file:4164c71b841ba2c1f213c9fdc073ec3d4c7d79dadfcd9d771768750a3085d616 in / 
# Tue, 04 Aug 2020 06:42:24 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 11:05:29 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 04 Aug 2020 11:05:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 11:05:42 GMT
ENV MEMCACHED_VERSION=1.6.6
# Tue, 04 Aug 2020 11:05:42 GMT
ENV MEMCACHED_SHA1=d8895b12dc9fc82b389f1713e2c09cc6ca3d03e4
# Tue, 04 Aug 2020 11:17:25 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 04 Aug 2020 11:17:25 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 04 Aug 2020 11:17:27 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 04 Aug 2020 11:17:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Aug 2020 11:17:28 GMT
USER memcache
# Tue, 04 Aug 2020 11:17:28 GMT
EXPOSE 11211
# Tue, 04 Aug 2020 11:17:28 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:1333f76e75c0136aa2eb56b14271ef57d1f975f40fe2a56536d99b7c86c3aa29`  
		Last Modified: Tue, 04 Aug 2020 06:48:41 GMT  
		Size: 25.8 MB (25762724 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e8b074644a235b1bb35f407f447fc6f33e3511e5cf837f33d1ccf0b9a039f4b`  
		Last Modified: Tue, 04 Aug 2020 11:17:48 GMT  
		Size: 5.0 KB (4980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:358e4488d4f6c21470ee9d8366dc5f304ade7c0ef3852eea9d2678e8b3102810`  
		Last Modified: Tue, 04 Aug 2020 11:17:49 GMT  
		Size: 1.8 MB (1776037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07209a5f05b07eff5f25acb525649cbca01da609b40355269d50a0b1a8afd1c7`  
		Last Modified: Tue, 04 Aug 2020 11:17:48 GMT  
		Size: 1.2 MB (1182538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:662db051984f433760ae7b7564ca3b00d4822012405825bae37fc850edd7bc79`  
		Last Modified: Tue, 04 Aug 2020 11:17:47 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7ee1c64bb768a6837da56bfbc48058253ec0cdb0666155f4810c2a16bd18851`  
		Last Modified: Tue, 04 Aug 2020 11:17:47 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6` - linux; ppc64le

```console
$ docker pull memcached@sha256:92643ad382b13ec8a5833b8e73e95ed5dc6ea7d1f04146fd495b66791f99d876
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.1 MB (34071500 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c77d50f314b2c2877792edab86d1db23e830478326e35ee02dd4cfdd8656dde4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 04 Aug 2020 04:45:34 GMT
ADD file:3bab6d2b62fe6a548ee28480d9eebf3251e942c4bb66362b87396b73af7aa586 in / 
# Tue, 04 Aug 2020 04:45:40 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 09:12:47 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 04 Aug 2020 09:13:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 08 Sep 2020 20:46:58 GMT
ENV MEMCACHED_VERSION=1.6.7
# Tue, 08 Sep 2020 20:47:05 GMT
ENV MEMCACHED_SHA1=49336bb0a4b7ad296422b08148581ed54edf32d0
# Tue, 08 Sep 2020 21:01:47 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 08 Sep 2020 21:01:51 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 08 Sep 2020 21:02:04 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 08 Sep 2020 21:02:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 08 Sep 2020 21:02:17 GMT
USER memcache
# Tue, 08 Sep 2020 21:02:24 GMT
EXPOSE 11211
# Tue, 08 Sep 2020 21:02:29 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:0827434caf9c0b71f95b3bcbe29d60f4f887199db59b3994d9315c478def41c3`  
		Last Modified: Tue, 04 Aug 2020 04:53:24 GMT  
		Size: 30.5 MB (30517844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:148c6ee7500ba1bf209ecab4590fcbcccc43e47abc7b4c327f95def3fb988a24`  
		Last Modified: Tue, 04 Aug 2020 09:26:02 GMT  
		Size: 5.0 KB (4984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b12a8a57075aa4c0c08c713d3f6901ab119bac72ca37a1155ef71a64d7cce6c`  
		Last Modified: Tue, 04 Aug 2020 09:26:03 GMT  
		Size: 2.3 MB (2322731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7760164dbee558e327c1ba89f2d6706a978d87b884f56558b6ba026110d966b`  
		Last Modified: Tue, 08 Sep 2020 21:13:49 GMT  
		Size: 1.2 MB (1225532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ead7201825bf4619985e151116fb21bf149927b6b1384bb8a2d2cf1f38271a81`  
		Last Modified: Tue, 08 Sep 2020 21:13:49 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4b36e2776fcec754f6f51e67d7580f566da6ef03ae5deadca6535f3a2f7bd18`  
		Last Modified: Tue, 08 Sep 2020 21:13:50 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6` - linux; s390x

```console
$ docker pull memcached@sha256:33252d5979791433f6abd86d4cd681e52d53e34b985e7e5c40831b39e76b03c8
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.8 MB (28789297 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:512f36fcfab08338e9c9d98c61771ba16dd3231bb06e1d716f4d7d8b58b7a8dd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 04 Aug 2020 01:17:16 GMT
ADD file:2ffa27c57800f9370adbaecca870158ec38c3d25a58b8803e2447c5e9320c5bb in / 
# Tue, 04 Aug 2020 01:17:17 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 02:50:25 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 04 Aug 2020 02:50:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 08 Sep 2020 19:56:37 GMT
ENV MEMCACHED_VERSION=1.6.7
# Tue, 08 Sep 2020 19:56:37 GMT
ENV MEMCACHED_SHA1=49336bb0a4b7ad296422b08148581ed54edf32d0
# Tue, 08 Sep 2020 20:05:26 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 08 Sep 2020 20:05:26 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 08 Sep 2020 20:05:26 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 08 Sep 2020 20:05:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 08 Sep 2020 20:05:27 GMT
USER memcache
# Tue, 08 Sep 2020 20:05:27 GMT
EXPOSE 11211
# Tue, 08 Sep 2020 20:05:27 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:0c46adfa2de4a7b7eb1fe2f0cb928f9e15a4cc94b7b975f13392f397cbfb0f2c`  
		Last Modified: Tue, 04 Aug 2020 01:20:03 GMT  
		Size: 25.7 MB (25707641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e4b36fc30f49aa14be390857b0e79628a680feeffb91e7c86f6381aeddcbf5c`  
		Last Modified: Tue, 04 Aug 2020 02:59:46 GMT  
		Size: 5.0 KB (5024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61f47a7c59d5f7d947ab1b93bb5d74d64ee1e84f8358eb1d78a4195ae8e4fa4e`  
		Last Modified: Tue, 04 Aug 2020 02:59:46 GMT  
		Size: 1.9 MB (1886090 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0683d3462c39632079df86d4267c6a0710f7bf718aaad9bd7468918022618cb6`  
		Last Modified: Tue, 08 Sep 2020 20:14:49 GMT  
		Size: 1.2 MB (1190135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06c729cc605ad7546ad2c9c45eda0473f5469a44ab7490cf1351134f839d6daf`  
		Last Modified: Tue, 08 Sep 2020 20:14:49 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7a2f84d1b6b2f9800f3fc44acccea46505b7891a807dcc8b1e5b5516d88b38c`  
		Last Modified: Tue, 08 Sep 2020 20:14:48 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:1.6.7`

```console
$ docker pull memcached@sha256:9b3c5e29e205933f871efd4f7083de35b76b89a503a2c96890d7565e1e62f222
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `memcached:1.6.7` - linux; amd64

```console
$ docker pull memcached@sha256:355abd5b7bc78b4aefb544a11f806117d9b3c3c9ee17d9dfc89598eff9e6c7b8
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.5 MB (30493478 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1412702e49d1f90905c4f6b88157813f256be2aef74f93bc405d749bf2d4bc9e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 04 Aug 2020 15:42:51 GMT
ADD file:3af3091e7d2bb40bc1e6550eb5ea290badc6bbf3339105626f245a963cc11450 in / 
# Tue, 04 Aug 2020 15:42:51 GMT
CMD ["bash"]
# Wed, 05 Aug 2020 00:11:59 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 05 Aug 2020 00:12:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 08 Sep 2020 19:38:38 GMT
ENV MEMCACHED_VERSION=1.6.7
# Tue, 08 Sep 2020 19:38:38 GMT
ENV MEMCACHED_SHA1=49336bb0a4b7ad296422b08148581ed54edf32d0
# Tue, 08 Sep 2020 19:58:10 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 08 Sep 2020 19:58:10 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 08 Sep 2020 19:58:10 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 08 Sep 2020 19:58:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 08 Sep 2020 19:58:11 GMT
USER memcache
# Tue, 08 Sep 2020 19:58:11 GMT
EXPOSE 11211
# Tue, 08 Sep 2020 19:58:11 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:bf59529304463f62efa7179fa1a32718a611528cc4ce9f30c0d1bbc6724ec3fb`  
		Last Modified: Tue, 04 Aug 2020 15:49:09 GMT  
		Size: 27.1 MB (27092121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b529ccb9885e0a07fb36b22af61c8f7c5a9b0551f5177ba1debf8de757b3631c`  
		Last Modified: Wed, 05 Aug 2020 00:21:46 GMT  
		Size: 5.0 KB (4984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85fac251bdd1dc7c979fdff2cac12c56f7545ad74d0cbccae793c2d3e0f271e8`  
		Last Modified: Wed, 05 Aug 2020 00:21:47 GMT  
		Size: 2.2 MB (2196515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60c0a99dabb56d767ce262b4b22be4a626ad6afec3f17f0a7ed2f78f1a41ec1b`  
		Last Modified: Tue, 08 Sep 2020 20:18:16 GMT  
		Size: 1.2 MB (1199450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed2c76ea7ac6f2e3f5fd02bb7c068a1e7d0f70ce2dfc0ba5039205c90dd1f2cf`  
		Last Modified: Tue, 08 Sep 2020 20:18:15 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:087645fe651b24fda3abb9ff4a0031373f4bcb60df2fb39bdf65dbb367ae38fc`  
		Last Modified: Tue, 08 Sep 2020 20:18:15 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.7` - linux; arm variant v5

```console
$ docker pull memcached@sha256:45b13f1c38ec693a4b23dddef22b456239af5454437a27adc75a138382532b74
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.9 MB (27911379 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7516c2ec9377d95bfd1f67e9016ec35f378991779622a9c4bbe18f3e6e0cb077`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 04 Aug 2020 03:13:17 GMT
ADD file:1a4c984d1bdb683e240e8bbdfeae45b146e1f8003444ce04a84096e58a437853 in / 
# Tue, 04 Aug 2020 03:13:27 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 06:51:04 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 04 Aug 2020 06:51:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 08 Sep 2020 21:05:50 GMT
ENV MEMCACHED_VERSION=1.6.7
# Tue, 08 Sep 2020 21:06:00 GMT
ENV MEMCACHED_SHA1=49336bb0a4b7ad296422b08148581ed54edf32d0
# Tue, 08 Sep 2020 21:17:20 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 08 Sep 2020 21:17:37 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 08 Sep 2020 21:18:16 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 08 Sep 2020 21:18:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 08 Sep 2020 21:18:33 GMT
USER memcache
# Tue, 08 Sep 2020 21:18:40 GMT
EXPOSE 11211
# Tue, 08 Sep 2020 21:18:47 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:4eb4ac68461c572fdc826bae247c43484a232f91f165666714ce0f5f052b0bab`  
		Last Modified: Tue, 04 Aug 2020 03:34:09 GMT  
		Size: 24.8 MB (24836059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cb53bba0491bf847d6fccec1e97acf8b40962d63009b9d14e88dd262072722c`  
		Last Modified: Tue, 04 Aug 2020 07:02:42 GMT  
		Size: 4.9 KB (4896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43a44e4bfe83944a327bc58ffbfb7eef92252ca9078f7781a6452da48f852499`  
		Last Modified: Tue, 04 Aug 2020 07:02:42 GMT  
		Size: 1.9 MB (1896867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b272b500ec6183577a6b13721c41bd6c7d1686ffe22fe761b226fea78109fd7`  
		Last Modified: Tue, 08 Sep 2020 21:19:01 GMT  
		Size: 1.2 MB (1173148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db2c0a741733ce4c321f325cf3a6306edaac69edb68f63ca04017648923ce2c4`  
		Last Modified: Tue, 08 Sep 2020 21:19:01 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b763edbb9dd540a12cdbaa66b09c4462b45cb25ce9b4413f6ba8e75890459c0`  
		Last Modified: Tue, 08 Sep 2020 21:19:01 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.7` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:8b8d4040593aaa099462192d942483db796bb14d06afee08b8f98bba575258b7
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.1 MB (29099944 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba6a2a00e032b0a3b41f234b4cd1ee7de2255f1f7315bc0ad1ec2186e379a469`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 04 Aug 2020 06:57:29 GMT
ADD file:90ba7821623ab55fc1073647cc611cc45f5e306ade734910e587021971483eec in / 
# Tue, 04 Aug 2020 06:57:31 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 14:50:02 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 04 Aug 2020 14:50:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 08 Sep 2020 21:04:00 GMT
ENV MEMCACHED_VERSION=1.6.7
# Tue, 08 Sep 2020 21:04:09 GMT
ENV MEMCACHED_SHA1=49336bb0a4b7ad296422b08148581ed54edf32d0
# Tue, 08 Sep 2020 21:15:12 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 08 Sep 2020 21:15:19 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 08 Sep 2020 21:15:35 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 08 Sep 2020 21:15:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 08 Sep 2020 21:15:37 GMT
USER memcache
# Tue, 08 Sep 2020 21:15:38 GMT
EXPOSE 11211
# Tue, 08 Sep 2020 21:15:38 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:3742235f1882fee5cca1effc4ca0f0c7c180bbe169800a85daedcf3968b0d8f0`  
		Last Modified: Tue, 04 Aug 2020 07:04:03 GMT  
		Size: 25.8 MB (25849301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d9010ac788ddccd1668bdc1b6eb6896fc768e4ad050fdcfe39e0f3c6fc4269b`  
		Last Modified: Tue, 04 Aug 2020 15:01:00 GMT  
		Size: 5.0 KB (5024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:064151e7e34f6f91e46091d50428c5f0aad91b86432a93fbf8363b0c7cf43f48`  
		Last Modified: Tue, 04 Aug 2020 15:00:59 GMT  
		Size: 2.1 MB (2075003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1e261d39aaa0c8d085e073c40bce6ab4d17492978f19d2ebcf6b8527b4c755b`  
		Last Modified: Tue, 08 Sep 2020 21:27:04 GMT  
		Size: 1.2 MB (1170207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:340cde0def1487d362e2a355d781db751ec18c50e06d3749d07920b5665a238e`  
		Last Modified: Tue, 08 Sep 2020 21:27:05 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0dc0954cc2aa31fe25c0ccc4baf6c2dc9855faa9c93070d64f19da484cb362f`  
		Last Modified: Tue, 08 Sep 2020 21:27:05 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.7` - linux; 386

```console
$ docker pull memcached@sha256:f0d08a896e1a4e545e5caf597c0d88d1a9d5dd9c49ffafff25c5b1293a9f7eec
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.2 MB (31161322 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc41ce3e1c9b5084b98d7961997e919ecfc4e9bb01fe696c0e21ae1ff16ae0f2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 04 Aug 2020 03:37:35 GMT
ADD file:cc791c21e6022a12dd1445a35f4cca9392ad8edfe34ea5852f3e87862c943628 in / 
# Tue, 04 Aug 2020 03:37:35 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 05:58:02 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 04 Aug 2020 05:58:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 08 Sep 2020 19:54:32 GMT
ENV MEMCACHED_VERSION=1.6.7
# Tue, 08 Sep 2020 19:54:32 GMT
ENV MEMCACHED_SHA1=49336bb0a4b7ad296422b08148581ed54edf32d0
# Tue, 08 Sep 2020 20:04:14 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 08 Sep 2020 20:04:14 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 08 Sep 2020 20:04:15 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 08 Sep 2020 20:04:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 08 Sep 2020 20:04:15 GMT
USER memcache
# Tue, 08 Sep 2020 20:04:16 GMT
EXPOSE 11211
# Tue, 08 Sep 2020 20:04:16 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:23ad22c16ab9d635a179d5d341096c34912941507b0c77ac97083b9795d8516f`  
		Last Modified: Tue, 04 Aug 2020 03:42:33 GMT  
		Size: 27.8 MB (27750435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f95eecb817da01910205081ea555757eb2fc5f1fd3a0844775943d55e1a10f4f`  
		Last Modified: Tue, 04 Aug 2020 06:08:21 GMT  
		Size: 4.9 KB (4894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b54cd9b7aa7674853d5ce4059daf598ccb281afb321a8f8d09a9b6e40223a9e7`  
		Last Modified: Tue, 04 Aug 2020 06:08:22 GMT  
		Size: 2.2 MB (2208142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:516ee7394637045940f9a0678b447be8f6b23ee3c9140baed49b5291be183b43`  
		Last Modified: Tue, 08 Sep 2020 20:14:40 GMT  
		Size: 1.2 MB (1197445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b2882adacd9ea9fd9e0e7002a6e785fae3eecd005b6d3f60667335adf2bf4d2`  
		Last Modified: Tue, 08 Sep 2020 20:14:39 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:752587d11a4176c1da4c2d1b00a16ffccd29ff01097c315a4ae64794ec760349`  
		Last Modified: Tue, 08 Sep 2020 20:14:39 GMT  
		Size: 119.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.7` - linux; ppc64le

```console
$ docker pull memcached@sha256:92643ad382b13ec8a5833b8e73e95ed5dc6ea7d1f04146fd495b66791f99d876
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.1 MB (34071500 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c77d50f314b2c2877792edab86d1db23e830478326e35ee02dd4cfdd8656dde4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 04 Aug 2020 04:45:34 GMT
ADD file:3bab6d2b62fe6a548ee28480d9eebf3251e942c4bb66362b87396b73af7aa586 in / 
# Tue, 04 Aug 2020 04:45:40 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 09:12:47 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 04 Aug 2020 09:13:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 08 Sep 2020 20:46:58 GMT
ENV MEMCACHED_VERSION=1.6.7
# Tue, 08 Sep 2020 20:47:05 GMT
ENV MEMCACHED_SHA1=49336bb0a4b7ad296422b08148581ed54edf32d0
# Tue, 08 Sep 2020 21:01:47 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 08 Sep 2020 21:01:51 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 08 Sep 2020 21:02:04 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 08 Sep 2020 21:02:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 08 Sep 2020 21:02:17 GMT
USER memcache
# Tue, 08 Sep 2020 21:02:24 GMT
EXPOSE 11211
# Tue, 08 Sep 2020 21:02:29 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:0827434caf9c0b71f95b3bcbe29d60f4f887199db59b3994d9315c478def41c3`  
		Last Modified: Tue, 04 Aug 2020 04:53:24 GMT  
		Size: 30.5 MB (30517844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:148c6ee7500ba1bf209ecab4590fcbcccc43e47abc7b4c327f95def3fb988a24`  
		Last Modified: Tue, 04 Aug 2020 09:26:02 GMT  
		Size: 5.0 KB (4984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b12a8a57075aa4c0c08c713d3f6901ab119bac72ca37a1155ef71a64d7cce6c`  
		Last Modified: Tue, 04 Aug 2020 09:26:03 GMT  
		Size: 2.3 MB (2322731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7760164dbee558e327c1ba89f2d6706a978d87b884f56558b6ba026110d966b`  
		Last Modified: Tue, 08 Sep 2020 21:13:49 GMT  
		Size: 1.2 MB (1225532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ead7201825bf4619985e151116fb21bf149927b6b1384bb8a2d2cf1f38271a81`  
		Last Modified: Tue, 08 Sep 2020 21:13:49 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4b36e2776fcec754f6f51e67d7580f566da6ef03ae5deadca6535f3a2f7bd18`  
		Last Modified: Tue, 08 Sep 2020 21:13:50 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.7` - linux; s390x

```console
$ docker pull memcached@sha256:33252d5979791433f6abd86d4cd681e52d53e34b985e7e5c40831b39e76b03c8
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.8 MB (28789297 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:512f36fcfab08338e9c9d98c61771ba16dd3231bb06e1d716f4d7d8b58b7a8dd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 04 Aug 2020 01:17:16 GMT
ADD file:2ffa27c57800f9370adbaecca870158ec38c3d25a58b8803e2447c5e9320c5bb in / 
# Tue, 04 Aug 2020 01:17:17 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 02:50:25 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 04 Aug 2020 02:50:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 08 Sep 2020 19:56:37 GMT
ENV MEMCACHED_VERSION=1.6.7
# Tue, 08 Sep 2020 19:56:37 GMT
ENV MEMCACHED_SHA1=49336bb0a4b7ad296422b08148581ed54edf32d0
# Tue, 08 Sep 2020 20:05:26 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 08 Sep 2020 20:05:26 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 08 Sep 2020 20:05:26 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 08 Sep 2020 20:05:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 08 Sep 2020 20:05:27 GMT
USER memcache
# Tue, 08 Sep 2020 20:05:27 GMT
EXPOSE 11211
# Tue, 08 Sep 2020 20:05:27 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:0c46adfa2de4a7b7eb1fe2f0cb928f9e15a4cc94b7b975f13392f397cbfb0f2c`  
		Last Modified: Tue, 04 Aug 2020 01:20:03 GMT  
		Size: 25.7 MB (25707641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e4b36fc30f49aa14be390857b0e79628a680feeffb91e7c86f6381aeddcbf5c`  
		Last Modified: Tue, 04 Aug 2020 02:59:46 GMT  
		Size: 5.0 KB (5024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61f47a7c59d5f7d947ab1b93bb5d74d64ee1e84f8358eb1d78a4195ae8e4fa4e`  
		Last Modified: Tue, 04 Aug 2020 02:59:46 GMT  
		Size: 1.9 MB (1886090 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0683d3462c39632079df86d4267c6a0710f7bf718aaad9bd7468918022618cb6`  
		Last Modified: Tue, 08 Sep 2020 20:14:49 GMT  
		Size: 1.2 MB (1190135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06c729cc605ad7546ad2c9c45eda0473f5469a44ab7490cf1351134f839d6daf`  
		Last Modified: Tue, 08 Sep 2020 20:14:49 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7a2f84d1b6b2f9800f3fc44acccea46505b7891a807dcc8b1e5b5516d88b38c`  
		Last Modified: Tue, 08 Sep 2020 20:14:48 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:1.6.7-alpine`

```console
$ docker pull memcached@sha256:788be093d2d88abdfa19b8f4624e0b604f574b840c9f6d49b467f4cd489c5182
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
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
$ docker pull memcached@sha256:eeb70c064ec36d136c3559fbaadec9df11f3ab745e4280f17c6580ff93d47615
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
$ docker pull memcached@sha256:b46c1524cef5a4dc4c624ab5260500e3ea1f126dceca799a68f736af6f962378
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3826350 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8fcb8b1e1fb28d77c405eab2623c8376361a0724faee61e4b00d87604f2ac589`
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
# Thu, 11 Jun 2020 20:31:59 GMT
ENV MEMCACHED_VERSION=1.6.6
# Thu, 11 Jun 2020 20:32:00 GMT
ENV MEMCACHED_SHA1=d8895b12dc9fc82b389f1713e2c09cc6ca3d03e4
# Thu, 11 Jun 2020 20:42:44 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		dpkg-dev dpkg 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		tar 		wget 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& make test 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Thu, 11 Jun 2020 20:42:45 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 11 Jun 2020 20:42:47 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 11 Jun 2020 20:42:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 11 Jun 2020 20:42:49 GMT
USER memcache
# Thu, 11 Jun 2020 20:42:50 GMT
EXPOSE 11211
# Thu, 11 Jun 2020 20:42:50 GMT
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
	-	`sha256:d24ea3e7feb7ae4cc898f3549467c5d200b739020fbb1204666c7c2bf0f2049a`  
		Last Modified: Thu, 11 Jun 2020 20:43:16 GMT  
		Size: 1.4 MB (1404102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:121fd71ab3ff327ca2cd4606b6472ae6dbed82f3363bb087ba6fbe4fc1a5d8c3`  
		Last Modified: Thu, 11 Jun 2020 20:43:17 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7d2f107913e874d41a62b7b6c286ea0b3bea2a4a35c2e10ce334966a8fe8e48`  
		Last Modified: Thu, 11 Jun 2020 20:43:17 GMT  
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
$ docker pull memcached@sha256:eeb70c064ec36d136c3559fbaadec9df11f3ab745e4280f17c6580ff93d47615
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
$ docker pull memcached@sha256:b46c1524cef5a4dc4c624ab5260500e3ea1f126dceca799a68f736af6f962378
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3826350 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8fcb8b1e1fb28d77c405eab2623c8376361a0724faee61e4b00d87604f2ac589`
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
# Thu, 11 Jun 2020 20:31:59 GMT
ENV MEMCACHED_VERSION=1.6.6
# Thu, 11 Jun 2020 20:32:00 GMT
ENV MEMCACHED_SHA1=d8895b12dc9fc82b389f1713e2c09cc6ca3d03e4
# Thu, 11 Jun 2020 20:42:44 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		dpkg-dev dpkg 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		tar 		wget 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& make test 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Thu, 11 Jun 2020 20:42:45 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 11 Jun 2020 20:42:47 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 11 Jun 2020 20:42:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 11 Jun 2020 20:42:49 GMT
USER memcache
# Thu, 11 Jun 2020 20:42:50 GMT
EXPOSE 11211
# Thu, 11 Jun 2020 20:42:50 GMT
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
	-	`sha256:d24ea3e7feb7ae4cc898f3549467c5d200b739020fbb1204666c7c2bf0f2049a`  
		Last Modified: Thu, 11 Jun 2020 20:43:16 GMT  
		Size: 1.4 MB (1404102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:121fd71ab3ff327ca2cd4606b6472ae6dbed82f3363bb087ba6fbe4fc1a5d8c3`  
		Last Modified: Thu, 11 Jun 2020 20:43:17 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7d2f107913e874d41a62b7b6c286ea0b3bea2a4a35c2e10ce334966a8fe8e48`  
		Last Modified: Thu, 11 Jun 2020 20:43:17 GMT  
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
$ docker pull memcached@sha256:eeb70c064ec36d136c3559fbaadec9df11f3ab745e4280f17c6580ff93d47615
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
$ docker pull memcached@sha256:b46c1524cef5a4dc4c624ab5260500e3ea1f126dceca799a68f736af6f962378
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3826350 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8fcb8b1e1fb28d77c405eab2623c8376361a0724faee61e4b00d87604f2ac589`
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
# Thu, 11 Jun 2020 20:31:59 GMT
ENV MEMCACHED_VERSION=1.6.6
# Thu, 11 Jun 2020 20:32:00 GMT
ENV MEMCACHED_SHA1=d8895b12dc9fc82b389f1713e2c09cc6ca3d03e4
# Thu, 11 Jun 2020 20:42:44 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		dpkg-dev dpkg 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		tar 		wget 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& make test 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Thu, 11 Jun 2020 20:42:45 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 11 Jun 2020 20:42:47 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 11 Jun 2020 20:42:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 11 Jun 2020 20:42:49 GMT
USER memcache
# Thu, 11 Jun 2020 20:42:50 GMT
EXPOSE 11211
# Thu, 11 Jun 2020 20:42:50 GMT
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
	-	`sha256:d24ea3e7feb7ae4cc898f3549467c5d200b739020fbb1204666c7c2bf0f2049a`  
		Last Modified: Thu, 11 Jun 2020 20:43:16 GMT  
		Size: 1.4 MB (1404102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:121fd71ab3ff327ca2cd4606b6472ae6dbed82f3363bb087ba6fbe4fc1a5d8c3`  
		Last Modified: Thu, 11 Jun 2020 20:43:17 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7d2f107913e874d41a62b7b6c286ea0b3bea2a4a35c2e10ce334966a8fe8e48`  
		Last Modified: Thu, 11 Jun 2020 20:43:17 GMT  
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
$ docker pull memcached@sha256:9cdffaa615cf536e8474900776d50568a912d637649a749c92d118a9cce2ab75
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
$ docker pull memcached@sha256:355abd5b7bc78b4aefb544a11f806117d9b3c3c9ee17d9dfc89598eff9e6c7b8
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.5 MB (30493478 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1412702e49d1f90905c4f6b88157813f256be2aef74f93bc405d749bf2d4bc9e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 04 Aug 2020 15:42:51 GMT
ADD file:3af3091e7d2bb40bc1e6550eb5ea290badc6bbf3339105626f245a963cc11450 in / 
# Tue, 04 Aug 2020 15:42:51 GMT
CMD ["bash"]
# Wed, 05 Aug 2020 00:11:59 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 05 Aug 2020 00:12:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 08 Sep 2020 19:38:38 GMT
ENV MEMCACHED_VERSION=1.6.7
# Tue, 08 Sep 2020 19:38:38 GMT
ENV MEMCACHED_SHA1=49336bb0a4b7ad296422b08148581ed54edf32d0
# Tue, 08 Sep 2020 19:58:10 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 08 Sep 2020 19:58:10 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 08 Sep 2020 19:58:10 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 08 Sep 2020 19:58:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 08 Sep 2020 19:58:11 GMT
USER memcache
# Tue, 08 Sep 2020 19:58:11 GMT
EXPOSE 11211
# Tue, 08 Sep 2020 19:58:11 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:bf59529304463f62efa7179fa1a32718a611528cc4ce9f30c0d1bbc6724ec3fb`  
		Last Modified: Tue, 04 Aug 2020 15:49:09 GMT  
		Size: 27.1 MB (27092121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b529ccb9885e0a07fb36b22af61c8f7c5a9b0551f5177ba1debf8de757b3631c`  
		Last Modified: Wed, 05 Aug 2020 00:21:46 GMT  
		Size: 5.0 KB (4984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85fac251bdd1dc7c979fdff2cac12c56f7545ad74d0cbccae793c2d3e0f271e8`  
		Last Modified: Wed, 05 Aug 2020 00:21:47 GMT  
		Size: 2.2 MB (2196515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60c0a99dabb56d767ce262b4b22be4a626ad6afec3f17f0a7ed2f78f1a41ec1b`  
		Last Modified: Tue, 08 Sep 2020 20:18:16 GMT  
		Size: 1.2 MB (1199450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed2c76ea7ac6f2e3f5fd02bb7c068a1e7d0f70ce2dfc0ba5039205c90dd1f2cf`  
		Last Modified: Tue, 08 Sep 2020 20:18:15 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:087645fe651b24fda3abb9ff4a0031373f4bcb60df2fb39bdf65dbb367ae38fc`  
		Last Modified: Tue, 08 Sep 2020 20:18:15 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:latest` - linux; arm variant v5

```console
$ docker pull memcached@sha256:45b13f1c38ec693a4b23dddef22b456239af5454437a27adc75a138382532b74
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.9 MB (27911379 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7516c2ec9377d95bfd1f67e9016ec35f378991779622a9c4bbe18f3e6e0cb077`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 04 Aug 2020 03:13:17 GMT
ADD file:1a4c984d1bdb683e240e8bbdfeae45b146e1f8003444ce04a84096e58a437853 in / 
# Tue, 04 Aug 2020 03:13:27 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 06:51:04 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 04 Aug 2020 06:51:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 08 Sep 2020 21:05:50 GMT
ENV MEMCACHED_VERSION=1.6.7
# Tue, 08 Sep 2020 21:06:00 GMT
ENV MEMCACHED_SHA1=49336bb0a4b7ad296422b08148581ed54edf32d0
# Tue, 08 Sep 2020 21:17:20 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 08 Sep 2020 21:17:37 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 08 Sep 2020 21:18:16 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 08 Sep 2020 21:18:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 08 Sep 2020 21:18:33 GMT
USER memcache
# Tue, 08 Sep 2020 21:18:40 GMT
EXPOSE 11211
# Tue, 08 Sep 2020 21:18:47 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:4eb4ac68461c572fdc826bae247c43484a232f91f165666714ce0f5f052b0bab`  
		Last Modified: Tue, 04 Aug 2020 03:34:09 GMT  
		Size: 24.8 MB (24836059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cb53bba0491bf847d6fccec1e97acf8b40962d63009b9d14e88dd262072722c`  
		Last Modified: Tue, 04 Aug 2020 07:02:42 GMT  
		Size: 4.9 KB (4896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43a44e4bfe83944a327bc58ffbfb7eef92252ca9078f7781a6452da48f852499`  
		Last Modified: Tue, 04 Aug 2020 07:02:42 GMT  
		Size: 1.9 MB (1896867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b272b500ec6183577a6b13721c41bd6c7d1686ffe22fe761b226fea78109fd7`  
		Last Modified: Tue, 08 Sep 2020 21:19:01 GMT  
		Size: 1.2 MB (1173148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db2c0a741733ce4c321f325cf3a6306edaac69edb68f63ca04017648923ce2c4`  
		Last Modified: Tue, 08 Sep 2020 21:19:01 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b763edbb9dd540a12cdbaa66b09c4462b45cb25ce9b4413f6ba8e75890459c0`  
		Last Modified: Tue, 08 Sep 2020 21:19:01 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:latest` - linux; arm variant v7

```console
$ docker pull memcached@sha256:2144f5d0ed52bbfe4170b2f27957a05b77b7a18e399a8f0acb523f1ee91332cd
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.7 MB (25651244 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5380de28b2ec24580bfbe5a9b563fda4b9ee55df259ae10ef0159079669aa6b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 04 Aug 2020 04:56:49 GMT
ADD file:16169b615697a126ae57dc01f7c4902fb9d9bc1e8595af43293700fa030808cc in / 
# Tue, 04 Aug 2020 04:56:51 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 11:21:50 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 04 Aug 2020 11:22:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 11:22:03 GMT
ENV MEMCACHED_VERSION=1.6.6
# Tue, 04 Aug 2020 11:22:05 GMT
ENV MEMCACHED_SHA1=d8895b12dc9fc82b389f1713e2c09cc6ca3d03e4
# Tue, 04 Aug 2020 11:32:23 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 04 Aug 2020 11:32:24 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 04 Aug 2020 11:32:27 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 04 Aug 2020 11:32:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Aug 2020 11:32:29 GMT
USER memcache
# Tue, 04 Aug 2020 11:32:30 GMT
EXPOSE 11211
# Tue, 04 Aug 2020 11:32:30 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:d7fe0a1b85ffd3158c62ab2e06ab004dc957cd133ba7129fb9c69c4586f407c9`  
		Last Modified: Tue, 04 Aug 2020 05:05:19 GMT  
		Size: 22.7 MB (22699792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a552abd0d66729ea122ed43216a635d2b40c0c34b82d247448a62280bda2b1b`  
		Last Modified: Tue, 04 Aug 2020 11:32:49 GMT  
		Size: 4.9 KB (4895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe0572bbccbb4def0fbbff844d9aefa4723ad29312e0b2952505927355e6da5a`  
		Last Modified: Tue, 04 Aug 2020 11:32:50 GMT  
		Size: 1.8 MB (1811523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f0c7c1daf8e87852846cbec2c963c032cd1de0f40ba57df3329e18c2572946d`  
		Last Modified: Tue, 04 Aug 2020 11:32:50 GMT  
		Size: 1.1 MB (1134625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f17117691f08ee67cafe0d9ef1d29943dd301aea76f85c550119df2c555c2d8`  
		Last Modified: Tue, 04 Aug 2020 11:32:50 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63cdfdb6ebae5cb43273e7c9c13a91ba971c74630c5eaaddccaea894d296f9e8`  
		Last Modified: Tue, 04 Aug 2020 11:32:50 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:latest` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:8b8d4040593aaa099462192d942483db796bb14d06afee08b8f98bba575258b7
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.1 MB (29099944 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba6a2a00e032b0a3b41f234b4cd1ee7de2255f1f7315bc0ad1ec2186e379a469`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 04 Aug 2020 06:57:29 GMT
ADD file:90ba7821623ab55fc1073647cc611cc45f5e306ade734910e587021971483eec in / 
# Tue, 04 Aug 2020 06:57:31 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 14:50:02 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 04 Aug 2020 14:50:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 08 Sep 2020 21:04:00 GMT
ENV MEMCACHED_VERSION=1.6.7
# Tue, 08 Sep 2020 21:04:09 GMT
ENV MEMCACHED_SHA1=49336bb0a4b7ad296422b08148581ed54edf32d0
# Tue, 08 Sep 2020 21:15:12 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 08 Sep 2020 21:15:19 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 08 Sep 2020 21:15:35 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 08 Sep 2020 21:15:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 08 Sep 2020 21:15:37 GMT
USER memcache
# Tue, 08 Sep 2020 21:15:38 GMT
EXPOSE 11211
# Tue, 08 Sep 2020 21:15:38 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:3742235f1882fee5cca1effc4ca0f0c7c180bbe169800a85daedcf3968b0d8f0`  
		Last Modified: Tue, 04 Aug 2020 07:04:03 GMT  
		Size: 25.8 MB (25849301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d9010ac788ddccd1668bdc1b6eb6896fc768e4ad050fdcfe39e0f3c6fc4269b`  
		Last Modified: Tue, 04 Aug 2020 15:01:00 GMT  
		Size: 5.0 KB (5024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:064151e7e34f6f91e46091d50428c5f0aad91b86432a93fbf8363b0c7cf43f48`  
		Last Modified: Tue, 04 Aug 2020 15:00:59 GMT  
		Size: 2.1 MB (2075003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1e261d39aaa0c8d085e073c40bce6ab4d17492978f19d2ebcf6b8527b4c755b`  
		Last Modified: Tue, 08 Sep 2020 21:27:04 GMT  
		Size: 1.2 MB (1170207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:340cde0def1487d362e2a355d781db751ec18c50e06d3749d07920b5665a238e`  
		Last Modified: Tue, 08 Sep 2020 21:27:05 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0dc0954cc2aa31fe25c0ccc4baf6c2dc9855faa9c93070d64f19da484cb362f`  
		Last Modified: Tue, 08 Sep 2020 21:27:05 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:latest` - linux; 386

```console
$ docker pull memcached@sha256:f0d08a896e1a4e545e5caf597c0d88d1a9d5dd9c49ffafff25c5b1293a9f7eec
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.2 MB (31161322 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc41ce3e1c9b5084b98d7961997e919ecfc4e9bb01fe696c0e21ae1ff16ae0f2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 04 Aug 2020 03:37:35 GMT
ADD file:cc791c21e6022a12dd1445a35f4cca9392ad8edfe34ea5852f3e87862c943628 in / 
# Tue, 04 Aug 2020 03:37:35 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 05:58:02 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 04 Aug 2020 05:58:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 08 Sep 2020 19:54:32 GMT
ENV MEMCACHED_VERSION=1.6.7
# Tue, 08 Sep 2020 19:54:32 GMT
ENV MEMCACHED_SHA1=49336bb0a4b7ad296422b08148581ed54edf32d0
# Tue, 08 Sep 2020 20:04:14 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 08 Sep 2020 20:04:14 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 08 Sep 2020 20:04:15 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 08 Sep 2020 20:04:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 08 Sep 2020 20:04:15 GMT
USER memcache
# Tue, 08 Sep 2020 20:04:16 GMT
EXPOSE 11211
# Tue, 08 Sep 2020 20:04:16 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:23ad22c16ab9d635a179d5d341096c34912941507b0c77ac97083b9795d8516f`  
		Last Modified: Tue, 04 Aug 2020 03:42:33 GMT  
		Size: 27.8 MB (27750435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f95eecb817da01910205081ea555757eb2fc5f1fd3a0844775943d55e1a10f4f`  
		Last Modified: Tue, 04 Aug 2020 06:08:21 GMT  
		Size: 4.9 KB (4894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b54cd9b7aa7674853d5ce4059daf598ccb281afb321a8f8d09a9b6e40223a9e7`  
		Last Modified: Tue, 04 Aug 2020 06:08:22 GMT  
		Size: 2.2 MB (2208142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:516ee7394637045940f9a0678b447be8f6b23ee3c9140baed49b5291be183b43`  
		Last Modified: Tue, 08 Sep 2020 20:14:40 GMT  
		Size: 1.2 MB (1197445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b2882adacd9ea9fd9e0e7002a6e785fae3eecd005b6d3f60667335adf2bf4d2`  
		Last Modified: Tue, 08 Sep 2020 20:14:39 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:752587d11a4176c1da4c2d1b00a16ffccd29ff01097c315a4ae64794ec760349`  
		Last Modified: Tue, 08 Sep 2020 20:14:39 GMT  
		Size: 119.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:latest` - linux; mips64le

```console
$ docker pull memcached@sha256:c1037de0c972b61f44c483a79f39039f734780f592133f26b6ead3cf9487101f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.7 MB (28726687 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f8cac462c662ef1bf25313d9053734ace48d255b60cad631b177adb6b7db6ee`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 04 Aug 2020 06:42:23 GMT
ADD file:4164c71b841ba2c1f213c9fdc073ec3d4c7d79dadfcd9d771768750a3085d616 in / 
# Tue, 04 Aug 2020 06:42:24 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 11:05:29 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 04 Aug 2020 11:05:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 11:05:42 GMT
ENV MEMCACHED_VERSION=1.6.6
# Tue, 04 Aug 2020 11:05:42 GMT
ENV MEMCACHED_SHA1=d8895b12dc9fc82b389f1713e2c09cc6ca3d03e4
# Tue, 04 Aug 2020 11:17:25 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 04 Aug 2020 11:17:25 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 04 Aug 2020 11:17:27 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 04 Aug 2020 11:17:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Aug 2020 11:17:28 GMT
USER memcache
# Tue, 04 Aug 2020 11:17:28 GMT
EXPOSE 11211
# Tue, 04 Aug 2020 11:17:28 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:1333f76e75c0136aa2eb56b14271ef57d1f975f40fe2a56536d99b7c86c3aa29`  
		Last Modified: Tue, 04 Aug 2020 06:48:41 GMT  
		Size: 25.8 MB (25762724 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e8b074644a235b1bb35f407f447fc6f33e3511e5cf837f33d1ccf0b9a039f4b`  
		Last Modified: Tue, 04 Aug 2020 11:17:48 GMT  
		Size: 5.0 KB (4980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:358e4488d4f6c21470ee9d8366dc5f304ade7c0ef3852eea9d2678e8b3102810`  
		Last Modified: Tue, 04 Aug 2020 11:17:49 GMT  
		Size: 1.8 MB (1776037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07209a5f05b07eff5f25acb525649cbca01da609b40355269d50a0b1a8afd1c7`  
		Last Modified: Tue, 04 Aug 2020 11:17:48 GMT  
		Size: 1.2 MB (1182538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:662db051984f433760ae7b7564ca3b00d4822012405825bae37fc850edd7bc79`  
		Last Modified: Tue, 04 Aug 2020 11:17:47 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7ee1c64bb768a6837da56bfbc48058253ec0cdb0666155f4810c2a16bd18851`  
		Last Modified: Tue, 04 Aug 2020 11:17:47 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:latest` - linux; ppc64le

```console
$ docker pull memcached@sha256:92643ad382b13ec8a5833b8e73e95ed5dc6ea7d1f04146fd495b66791f99d876
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.1 MB (34071500 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c77d50f314b2c2877792edab86d1db23e830478326e35ee02dd4cfdd8656dde4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 04 Aug 2020 04:45:34 GMT
ADD file:3bab6d2b62fe6a548ee28480d9eebf3251e942c4bb66362b87396b73af7aa586 in / 
# Tue, 04 Aug 2020 04:45:40 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 09:12:47 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 04 Aug 2020 09:13:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 08 Sep 2020 20:46:58 GMT
ENV MEMCACHED_VERSION=1.6.7
# Tue, 08 Sep 2020 20:47:05 GMT
ENV MEMCACHED_SHA1=49336bb0a4b7ad296422b08148581ed54edf32d0
# Tue, 08 Sep 2020 21:01:47 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 08 Sep 2020 21:01:51 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 08 Sep 2020 21:02:04 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 08 Sep 2020 21:02:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 08 Sep 2020 21:02:17 GMT
USER memcache
# Tue, 08 Sep 2020 21:02:24 GMT
EXPOSE 11211
# Tue, 08 Sep 2020 21:02:29 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:0827434caf9c0b71f95b3bcbe29d60f4f887199db59b3994d9315c478def41c3`  
		Last Modified: Tue, 04 Aug 2020 04:53:24 GMT  
		Size: 30.5 MB (30517844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:148c6ee7500ba1bf209ecab4590fcbcccc43e47abc7b4c327f95def3fb988a24`  
		Last Modified: Tue, 04 Aug 2020 09:26:02 GMT  
		Size: 5.0 KB (4984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b12a8a57075aa4c0c08c713d3f6901ab119bac72ca37a1155ef71a64d7cce6c`  
		Last Modified: Tue, 04 Aug 2020 09:26:03 GMT  
		Size: 2.3 MB (2322731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7760164dbee558e327c1ba89f2d6706a978d87b884f56558b6ba026110d966b`  
		Last Modified: Tue, 08 Sep 2020 21:13:49 GMT  
		Size: 1.2 MB (1225532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ead7201825bf4619985e151116fb21bf149927b6b1384bb8a2d2cf1f38271a81`  
		Last Modified: Tue, 08 Sep 2020 21:13:49 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4b36e2776fcec754f6f51e67d7580f566da6ef03ae5deadca6535f3a2f7bd18`  
		Last Modified: Tue, 08 Sep 2020 21:13:50 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:latest` - linux; s390x

```console
$ docker pull memcached@sha256:33252d5979791433f6abd86d4cd681e52d53e34b985e7e5c40831b39e76b03c8
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.8 MB (28789297 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:512f36fcfab08338e9c9d98c61771ba16dd3231bb06e1d716f4d7d8b58b7a8dd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 04 Aug 2020 01:17:16 GMT
ADD file:2ffa27c57800f9370adbaecca870158ec38c3d25a58b8803e2447c5e9320c5bb in / 
# Tue, 04 Aug 2020 01:17:17 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 02:50:25 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 04 Aug 2020 02:50:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 08 Sep 2020 19:56:37 GMT
ENV MEMCACHED_VERSION=1.6.7
# Tue, 08 Sep 2020 19:56:37 GMT
ENV MEMCACHED_SHA1=49336bb0a4b7ad296422b08148581ed54edf32d0
# Tue, 08 Sep 2020 20:05:26 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 08 Sep 2020 20:05:26 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 08 Sep 2020 20:05:26 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 08 Sep 2020 20:05:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 08 Sep 2020 20:05:27 GMT
USER memcache
# Tue, 08 Sep 2020 20:05:27 GMT
EXPOSE 11211
# Tue, 08 Sep 2020 20:05:27 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:0c46adfa2de4a7b7eb1fe2f0cb928f9e15a4cc94b7b975f13392f397cbfb0f2c`  
		Last Modified: Tue, 04 Aug 2020 01:20:03 GMT  
		Size: 25.7 MB (25707641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e4b36fc30f49aa14be390857b0e79628a680feeffb91e7c86f6381aeddcbf5c`  
		Last Modified: Tue, 04 Aug 2020 02:59:46 GMT  
		Size: 5.0 KB (5024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61f47a7c59d5f7d947ab1b93bb5d74d64ee1e84f8358eb1d78a4195ae8e4fa4e`  
		Last Modified: Tue, 04 Aug 2020 02:59:46 GMT  
		Size: 1.9 MB (1886090 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0683d3462c39632079df86d4267c6a0710f7bf718aaad9bd7468918022618cb6`  
		Last Modified: Tue, 08 Sep 2020 20:14:49 GMT  
		Size: 1.2 MB (1190135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06c729cc605ad7546ad2c9c45eda0473f5469a44ab7490cf1351134f839d6daf`  
		Last Modified: Tue, 08 Sep 2020 20:14:49 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7a2f84d1b6b2f9800f3fc44acccea46505b7891a807dcc8b1e5b5516d88b38c`  
		Last Modified: Tue, 08 Sep 2020 20:14:48 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
