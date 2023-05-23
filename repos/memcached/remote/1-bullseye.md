## `memcached:1-bullseye`

```console
$ docker pull memcached@sha256:0451628d4eced8a4b7f74946bae89e4bb401cb7dc2d7547b4087c3e40159dc25
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
$ docker pull memcached@sha256:ca633f743f7ffe76281d119891271f072e4bdb471b4cf2447be145a9afd97d2c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.0 MB (32997994 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a78754495cd58c1fd188f1147b890bd9de6c8a3bf9cbea69c917e578a7fa6842`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 23 May 2023 01:20:14 GMT
ADD file:88252a7f118b4d6f55dd5baf49dbcaa053c9d6172c652963c1151fa76f625e44 in / 
# Tue, 23 May 2023 01:20:14 GMT
CMD ["bash"]
# Tue, 23 May 2023 04:02:50 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 23 May 2023 04:02:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 04:02:54 GMT
ENV MEMCACHED_VERSION=1.6.20
# Tue, 23 May 2023 04:02:54 GMT
ENV MEMCACHED_SHA1=face85ed6fad41432ad818445b24eca55bccdd78
# Tue, 23 May 2023 04:05:05 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 23 May 2023 04:05:05 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 23 May 2023 04:05:06 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 23 May 2023 04:05:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 23 May 2023 04:05:06 GMT
USER memcache
# Tue, 23 May 2023 04:05:06 GMT
EXPOSE 11211
# Tue, 23 May 2023 04:05:06 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:f03b40093957615593f2ed142961afb6b540507e0b47e3f7626ba5e02efbbbf1`  
		Last Modified: Tue, 23 May 2023 01:24:08 GMT  
		Size: 31.4 MB (31403586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42850af464e5357c0c0ef63860ee73ed7775c9aef90ca1740dd84ddd5ee0f335`  
		Last Modified: Tue, 23 May 2023 04:05:24 GMT  
		Size: 5.0 KB (4985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66835158f1e39645e904689d36678623f36b00a888fc225a06013a2fed77d655`  
		Last Modified: Tue, 23 May 2023 04:05:25 GMT  
		Size: 328.2 KB (328211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4027e4df9c701a98771edfdd41af6ab6b8f6b9fd653d71e05461cb4f02293c92`  
		Last Modified: Tue, 23 May 2023 04:05:25 GMT  
		Size: 1.3 MB (1260804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e874830b2907232a137b7908511711e2e6a06330862f1add300c590a317ee84f`  
		Last Modified: Tue, 23 May 2023 04:05:24 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26b333375d5837211965b1039e5bb045858f570932d51f28a9dc35ca00ca4f9e`  
		Last Modified: Tue, 23 May 2023 04:05:25 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-bullseye` - linux; arm variant v5

```console
$ docker pull memcached@sha256:c404758a207fe4f509162eca52ef26769974e1d686c3c8ad1ec0c6e626b22a22
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.5 MB (30455216 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bf992b3a512ece139ddadb76e26a2cff05ebae7ffc1daea581963e7252298c00`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 23 May 2023 00:48:41 GMT
ADD file:868f634f5ddb80ed9e9c719ccaf5d564d96fe819f0b000ecc734311baf5da99b in / 
# Tue, 23 May 2023 00:48:42 GMT
CMD ["bash"]
# Tue, 23 May 2023 02:09:30 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 23 May 2023 02:09:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 02:09:35 GMT
ENV MEMCACHED_VERSION=1.6.20
# Tue, 23 May 2023 02:09:35 GMT
ENV MEMCACHED_SHA1=face85ed6fad41432ad818445b24eca55bccdd78
# Tue, 23 May 2023 02:12:32 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 23 May 2023 02:12:32 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 23 May 2023 02:12:33 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 23 May 2023 02:12:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 23 May 2023 02:12:33 GMT
USER memcache
# Tue, 23 May 2023 02:12:33 GMT
EXPOSE 11211
# Tue, 23 May 2023 02:12:33 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:812967ccba449e7a96044b2d48ffc62816b22eb17641844c4dfffbe3b3ec6f21`  
		Last Modified: Tue, 23 May 2023 00:51:19 GMT  
		Size: 28.9 MB (28903411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84451fbc913c4b973850f5fb43d3979f7bf2724deb5cf22abf16651cab686c35`  
		Last Modified: Tue, 23 May 2023 02:12:49 GMT  
		Size: 4.9 KB (4896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b7b5e1e0bcae71757cc5515cc40c9e2c25e708af7c50ef48e081a3c871211f6`  
		Last Modified: Tue, 23 May 2023 02:12:45 GMT  
		Size: 316.8 KB (316756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a15a1d27de70ccb8bf0f2f9e372fe2649815e5a6e34d7f154b767f6f7b650d7`  
		Last Modified: Tue, 23 May 2023 02:12:45 GMT  
		Size: 1.2 MB (1229750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:560c1993cde0bd89664f6ed97a32f19d812ef6f053ae4ff002dfa7cb62ba78eb`  
		Last Modified: Tue, 23 May 2023 02:12:45 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd31dad32b9632171223a1aefee69195b4854504edc31b5635cc428779e8e3da`  
		Last Modified: Tue, 23 May 2023 02:12:45 GMT  
		Size: 118.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-bullseye` - linux; arm variant v7

```console
$ docker pull memcached@sha256:2841be0a36134563966c09a6ed68b21053d20342ec8736cf92763c28077ead43
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.1 MB (28094215 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6cf74ffa940dd93988fc0beb6698c5796563c82a40b7dd668153969f64d2e6ca`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 09 Feb 2023 06:12:09 GMT
ADD file:5f1a343224e8486690bd90dd1e50c8d84b3d770c51bb6829544e5cf650c0419c in / 
# Thu, 09 Feb 2023 06:12:10 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 07:52:31 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Thu, 09 Feb 2023 07:52:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 07:52:35 GMT
ENV MEMCACHED_VERSION=1.6.18
# Thu, 09 Feb 2023 07:52:35 GMT
ENV MEMCACHED_SHA1=be16909bb75ab972ee5fe438312501de01c4725a
# Thu, 09 Feb 2023 07:55:44 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 09 Feb 2023 07:55:44 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 09 Feb 2023 07:55:44 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 09 Feb 2023 07:55:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 09 Feb 2023 07:55:44 GMT
USER memcache
# Thu, 09 Feb 2023 07:55:45 GMT
EXPOSE 11211
# Thu, 09 Feb 2023 07:55:45 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:e7318f6106ad75d7d482ae9dddf4d927b0872ef3ddb6e1330aa691fc8d17279e`  
		Last Modified: Thu, 09 Feb 2023 06:19:19 GMT  
		Size: 26.6 MB (26577666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de49d9d72daf1680b5f1b9532dd2eb0162829f36c8db9669935462636fbf99d9`  
		Last Modified: Thu, 09 Feb 2023 08:06:11 GMT  
		Size: 4.9 KB (4895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0beac9d5bcac946f8c54c72b8a9c136914b1aa7a5fe2b8c3df4c7d8858ea6559`  
		Last Modified: Thu, 09 Feb 2023 08:06:11 GMT  
		Size: 312.1 KB (312088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4c9e5a265394e4c0f357779e6195a4e82d767a3691a0e77d427e56651c3e54a`  
		Last Modified: Thu, 09 Feb 2023 08:06:11 GMT  
		Size: 1.2 MB (1199163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5ea82ad892fe1ae8623d84e32c8c027087cda8aa49e40d4546ed6942e471c60`  
		Last Modified: Thu, 09 Feb 2023 08:06:11 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa2ae3bcdc0d114ba49a67df022b6f7215fc87f1f50e64939fcfbbec4eaadee5`  
		Last Modified: Thu, 09 Feb 2023 08:06:11 GMT  
		Size: 118.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-bullseye` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:9aa25dce22ae1d09335424de2d3d6d4a700f83b749079a30ba52eab857ddbd2e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.6 MB (31644695 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3506b3d165a9a044fb954cfdb6ed7a12b666312ccb7c47b04995a1b928e34a6a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 23 May 2023 00:43:15 GMT
ADD file:0fee550e337f1bd111a7ef785a9553674f25649f37deffa4aa8107ef6445d259 in / 
# Tue, 23 May 2023 00:43:15 GMT
CMD ["bash"]
# Tue, 23 May 2023 02:25:54 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 23 May 2023 02:25:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 02:25:57 GMT
ENV MEMCACHED_VERSION=1.6.20
# Tue, 23 May 2023 02:25:57 GMT
ENV MEMCACHED_SHA1=face85ed6fad41432ad818445b24eca55bccdd78
# Tue, 23 May 2023 02:28:32 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 23 May 2023 02:28:32 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 23 May 2023 02:28:32 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 23 May 2023 02:28:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 23 May 2023 02:28:32 GMT
USER memcache
# Tue, 23 May 2023 02:28:32 GMT
EXPOSE 11211
# Tue, 23 May 2023 02:28:33 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:d981f2c20c93e1c57a46cd87bc5b9a554be5323072a0d0ab4b354aabd237bbcf`  
		Last Modified: Tue, 23 May 2023 00:46:07 GMT  
		Size: 30.1 MB (30052747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed8feb48b1ed5a0b6fa01a6752c376895e1d2cbe717acd45d605a10edbe8845b`  
		Last Modified: Tue, 23 May 2023 02:28:55 GMT  
		Size: 5.0 KB (5028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6311f568e9253840f0cff67f8cc84f463244d4bb0fbee7b4e9a18a6e18961afc`  
		Last Modified: Tue, 23 May 2023 02:28:55 GMT  
		Size: 326.0 KB (326041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:950a3fe52fca58ee21c66b369de8989197b5a97864727e122cfc8bf62acbc01b`  
		Last Modified: Tue, 23 May 2023 02:28:55 GMT  
		Size: 1.3 MB (1260471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:258a14874b3f3fff515f9aa8dce780652d1e1f0022f4701b0f260cccf7ffa770`  
		Last Modified: Tue, 23 May 2023 02:28:54 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa2e868f1cfde537bb80123ad1b79bec504aba69049574865c0fbd70dd5d2127`  
		Last Modified: Tue, 23 May 2023 02:28:54 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-bullseye` - linux; 386

```console
$ docker pull memcached@sha256:f19ce197b6f1192acc27632ef7a76094d614a9ef1528ed8bf80b00cc0f024e6d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.0 MB (33987798 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a42ad3e18eba32fbe39df2218dd5d2a69a71a737915da0793e19b364dd0a359`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 23 May 2023 00:39:30 GMT
ADD file:8319fc1c1a3c0f2a6bb03636fe1fd0eb7fa52c58505d279e4366627452ea2104 in / 
# Tue, 23 May 2023 00:39:30 GMT
CMD ["bash"]
# Tue, 23 May 2023 05:37:49 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 23 May 2023 05:37:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 05:37:53 GMT
ENV MEMCACHED_VERSION=1.6.20
# Tue, 23 May 2023 05:37:53 GMT
ENV MEMCACHED_SHA1=face85ed6fad41432ad818445b24eca55bccdd78
# Tue, 23 May 2023 05:41:30 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 23 May 2023 05:41:31 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 23 May 2023 05:41:31 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 23 May 2023 05:41:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 23 May 2023 05:41:31 GMT
USER memcache
# Tue, 23 May 2023 05:41:31 GMT
EXPOSE 11211
# Tue, 23 May 2023 05:41:31 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:0f5d158483bd0ffef0c106b68514aece2ca0500d2990c830844277cbca7fe0bc`  
		Last Modified: Tue, 23 May 2023 00:44:28 GMT  
		Size: 32.4 MB (32388165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc8e7c3763286b4373179fafbdc01be6edbd6c23484654b0bb654b809abd6b1f`  
		Last Modified: Tue, 23 May 2023 05:41:51 GMT  
		Size: 4.9 KB (4898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6cfb9fd8f876a58629b590338bda06719f3d890fb0519368212f36576c4a355`  
		Last Modified: Tue, 23 May 2023 05:41:51 GMT  
		Size: 336.8 KB (336792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb6dd290e76318eb6037944db1c542492c88da0b32974fbf3f3e8d50a664fb08`  
		Last Modified: Tue, 23 May 2023 05:41:51 GMT  
		Size: 1.3 MB (1257535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3d596fc23eff67628172744a17ae8ac1ce14bb5d4f2484cd790e8c473cefcbf`  
		Last Modified: Tue, 23 May 2023 05:41:51 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:577f90cddde39d1579ce406b68faa54ff26d8006b68cdec8eb97572410882876`  
		Last Modified: Tue, 23 May 2023 05:41:51 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-bullseye` - linux; mips64le

```console
$ docker pull memcached@sha256:3172623d415479f750cd99c97b334b75b82feaa414b66b6e6ff0095cb4eb66c0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.0 MB (31002482 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:24d61981518258ba41d602c237fa04caef815a17e494f61ad65d57cb10a928b5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 23 May 2023 01:10:16 GMT
ADD file:aecd62d945e0ea0cd6759b1b4236075d30d02d2a8142dfb3a2a49736df18d664 in / 
# Tue, 23 May 2023 01:10:21 GMT
CMD ["bash"]
# Tue, 23 May 2023 06:05:28 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 23 May 2023 06:05:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 06:05:46 GMT
ENV MEMCACHED_VERSION=1.6.20
# Tue, 23 May 2023 06:05:49 GMT
ENV MEMCACHED_SHA1=face85ed6fad41432ad818445b24eca55bccdd78
# Tue, 23 May 2023 06:12:21 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 23 May 2023 06:12:23 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 23 May 2023 06:12:27 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 23 May 2023 06:12:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 23 May 2023 06:12:32 GMT
USER memcache
# Tue, 23 May 2023 06:12:35 GMT
EXPOSE 11211
# Tue, 23 May 2023 06:12:38 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:be8a34b2387f64d76e4dfe0d0797f481a7390c39ca0df2675d8de5476ca7f715`  
		Last Modified: Tue, 23 May 2023 01:19:21 GMT  
		Size: 29.6 MB (29623516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a17f317a8b046c392ea255450ca75dd823bb63c1f85e69d4f65825054e16a18`  
		Last Modified: Tue, 23 May 2023 06:13:02 GMT  
		Size: 4.9 KB (4861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed148e234cd4605620655ab83711e3254e3bc13d2d513be7a0f362c4deda7bba`  
		Last Modified: Tue, 23 May 2023 06:13:02 GMT  
		Size: 117.2 KB (117207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65a18cbc21601863e9d88e79e5d0e2fa0c91d59be2572c436b9b2c02f84a4f00`  
		Last Modified: Tue, 23 May 2023 06:13:03 GMT  
		Size: 1.3 MB (1256489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7153354a60c40b36887234ddb98ebb3bc3a032cb69ad25bd49f3c59bdc60817e`  
		Last Modified: Tue, 23 May 2023 06:13:02 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0618ca26ff4d015d39495a908fc4c7ba12948b8e16c3e2c2815c187030b63df2`  
		Last Modified: Tue, 23 May 2023 06:13:02 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-bullseye` - linux; ppc64le

```console
$ docker pull memcached@sha256:2ffa807f861434048d0e841b972890bdb7ceec1d5207344427a74f2037d3e66a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.0 MB (36971524 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fb7fd4722695effa6149f4871d0fe23bd1e303995d02d570fe2bcf30e1855fcd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 23 May 2023 01:17:35 GMT
ADD file:719aea085739ec41c255f35070ca652d4e356c5ee62c8237f8ebc7389feb8e38 in / 
# Tue, 23 May 2023 01:17:37 GMT
CMD ["bash"]
# Tue, 23 May 2023 07:25:18 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 23 May 2023 07:25:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 07:25:25 GMT
ENV MEMCACHED_VERSION=1.6.20
# Tue, 23 May 2023 07:25:25 GMT
ENV MEMCACHED_SHA1=face85ed6fad41432ad818445b24eca55bccdd78
# Tue, 23 May 2023 07:28:44 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 23 May 2023 07:28:44 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 23 May 2023 07:28:45 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 23 May 2023 07:28:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 23 May 2023 07:28:46 GMT
USER memcache
# Tue, 23 May 2023 07:28:46 GMT
EXPOSE 11211
# Tue, 23 May 2023 07:28:46 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:b6c83d2f160e7e38990586d26caa105ff577368a887fd754ae4634cdbfec83ff`  
		Last Modified: Tue, 23 May 2023 01:22:03 GMT  
		Size: 35.3 MB (35280911 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:278b6536bbaa63f2306e3f7b2248d4238d3d7535ac7f1e4b39c618077280bbb9`  
		Last Modified: Tue, 23 May 2023 07:29:09 GMT  
		Size: 5.0 KB (4982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0a3658e2cde2898ac68a5d9a93c662f3ffb7dd101242c0436c96d347fdffd91`  
		Last Modified: Tue, 23 May 2023 07:29:09 GMT  
		Size: 357.0 KB (357041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c394ab17697c8576c5eea1164400a645258bf0cf87cfc95b274d66e7abf4ff2a`  
		Last Modified: Tue, 23 May 2023 07:29:09 GMT  
		Size: 1.3 MB (1328181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ce6ddce2a64f19f72c5190267b085f319f35486f0c905f2562964c31a0f1300`  
		Last Modified: Tue, 23 May 2023 07:29:08 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f938755b546c48b08e2c1d6436bbb995f946e3a6f899d821cd492a5f3f350fa`  
		Last Modified: Tue, 23 May 2023 07:29:09 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-bullseye` - linux; s390x

```console
$ docker pull memcached@sha256:88aa1f69a6961c6d63dceb678257649d43cad68cc4d31c11b79b8e1d949c87ec
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.2 MB (31218466 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e496b8a5a3199e4ef7ab3011639cc7851bdb5e581f22270360cb7b2a4d6f3732`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 23 May 2023 00:42:52 GMT
ADD file:23b1e12559302529556a94a1d4098dbdb454e263265258b940c2b2d23a97c121 in / 
# Tue, 23 May 2023 00:42:54 GMT
CMD ["bash"]
# Tue, 23 May 2023 05:50:20 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 23 May 2023 05:50:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 05:50:23 GMT
ENV MEMCACHED_VERSION=1.6.20
# Tue, 23 May 2023 05:50:23 GMT
ENV MEMCACHED_SHA1=face85ed6fad41432ad818445b24eca55bccdd78
# Tue, 23 May 2023 05:53:21 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 23 May 2023 05:53:21 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 23 May 2023 05:53:22 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 23 May 2023 05:53:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 23 May 2023 05:53:22 GMT
USER memcache
# Tue, 23 May 2023 05:53:22 GMT
EXPOSE 11211
# Tue, 23 May 2023 05:53:22 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:9c24ec455bdb6a9ad0d033c7cce8e71dd5bdbbe53a86d5feeb8d4cb7804fb8e5`  
		Last Modified: Tue, 23 May 2023 00:45:47 GMT  
		Size: 29.6 MB (29642170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a3645d0133cf2c5dc8f1f9e931752f5faa715ca3fd740b5cd311ec07a5a24fa`  
		Last Modified: Tue, 23 May 2023 05:53:56 GMT  
		Size: 5.0 KB (5026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c7cd99b76489bd045bca9140e60b0baac5a6953cdf705335beba2e2bd9c088a`  
		Last Modified: Tue, 23 May 2023 05:53:56 GMT  
		Size: 324.3 KB (324339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0e58ab458a20f2a279f5a99b6f7caebd7ca46b16ec183cb85e997c31e5e74ed`  
		Last Modified: Tue, 23 May 2023 05:53:55 GMT  
		Size: 1.2 MB (1246524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48b42c5920a9a3e5740520ee18e58fb0c6c3c83c2a46e451a2ae909862215468`  
		Last Modified: Tue, 23 May 2023 05:53:55 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a15c14190c128fed537ecce164ef1b29ff9a6346ada062d50d72c8507559ed9a`  
		Last Modified: Tue, 23 May 2023 05:53:55 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
