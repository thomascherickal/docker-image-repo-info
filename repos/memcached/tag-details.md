<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `memcached`

-	[`memcached:1`](#memcached1)
-	[`memcached:1-alpine`](#memcached1-alpine)
-	[`memcached:1-alpine3.18`](#memcached1-alpine318)
-	[`memcached:1-bookworm`](#memcached1-bookworm)
-	[`memcached:1.6`](#memcached16)
-	[`memcached:1.6-alpine`](#memcached16-alpine)
-	[`memcached:1.6-alpine3.18`](#memcached16-alpine318)
-	[`memcached:1.6-bookworm`](#memcached16-bookworm)
-	[`memcached:1.6.21`](#memcached1621)
-	[`memcached:1.6.21-alpine`](#memcached1621-alpine)
-	[`memcached:1.6.21-alpine3.18`](#memcached1621-alpine318)
-	[`memcached:1.6.21-bookworm`](#memcached1621-bookworm)
-	[`memcached:alpine`](#memcachedalpine)
-	[`memcached:alpine3.18`](#memcachedalpine318)
-	[`memcached:bookworm`](#memcachedbookworm)
-	[`memcached:latest`](#memcachedlatest)

## `memcached:1`

```console
$ docker pull memcached@sha256:1348f2e27aeea6d2b4e2b25ce9ca7679560164b0e75b6f72e221b574000158f6
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
$ docker pull memcached@sha256:37d77084cbe7c98854989a68a18f22dd677379de8ffc9ee92fbf7b88b2b4d0f9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.0 MB (38973142 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a4d0c1490511995c15a4c1ca7c8413337bed068ea95507aae882010b051ca37e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 12 Jun 2023 23:20:42 GMT
ADD file:ba1250b6ecd5dd09d4914189d72741c2817988994e7da514bf62be439a34bdb5 in / 
# Mon, 12 Jun 2023 23:20:42 GMT
CMD ["bash"]
# Wed, 14 Jun 2023 20:48:19 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 14 Jun 2023 20:48:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 21 Jun 2023 01:04:34 GMT
ENV MEMCACHED_VERSION=1.6.21
# Wed, 21 Jun 2023 01:04:35 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Wed, 21 Jun 2023 01:07:04 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 21 Jun 2023 01:07:04 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 21 Jun 2023 01:07:04 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 21 Jun 2023 01:07:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Jun 2023 01:07:05 GMT
USER memcache
# Wed, 21 Jun 2023 01:07:05 GMT
EXPOSE 11211
# Wed, 21 Jun 2023 01:07:05 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:5b5fe70539cd6989aa19f25826309f9715a9489cf1c057982d6a84c1ad8975c7`  
		Last Modified: Mon, 12 Jun 2023 23:25:49 GMT  
		Size: 29.1 MB (29124744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab209434009a85e82d99c0547bb947940f9e1002ce6e965417396ee22a6820db`  
		Last Modified: Wed, 14 Jun 2023 20:53:33 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2f4dfc49c9cdae8d4df855de7cc0460e5db8c762e73786d4f8fa4f69ba11d6d`  
		Last Modified: Wed, 14 Jun 2023 20:53:33 GMT  
		Size: 2.7 MB (2677239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d5a41694f99632bb3a7c624dab437c8a10e54b92965de823e717f5c12326b1e`  
		Last Modified: Wed, 21 Jun 2023 01:09:52 GMT  
		Size: 7.2 MB (7169627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2be3d7709e1978d4b030abdf5ac129b97f21e09bb489932628899d96288a4a9`  
		Last Modified: Wed, 21 Jun 2023 01:09:50 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8cba3f7cc400544285611f46bbdba004587f84511783fd05aa6562e9337928f`  
		Last Modified: Wed, 21 Jun 2023 01:09:50 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1` - linux; arm variant v5

```console
$ docker pull memcached@sha256:1646b01539b9482149379208acae5c0af1c5aed3aa9d818e8748410e15170943
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.1 MB (35094759 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ad4aa07800c4cf602e699a614c04d8fa80a8617828cfeb89fc05b49791d07e7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 12 Jun 2023 23:48:31 GMT
ADD file:54a716f17b23e4fa49d1d5c0a7f63becc295873c116d19bb4753d34f1ca6affb in / 
# Mon, 12 Jun 2023 23:48:31 GMT
CMD ["bash"]
# Wed, 14 Jun 2023 21:56:18 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 14 Jun 2023 21:56:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 21 Jun 2023 00:52:38 GMT
ENV MEMCACHED_VERSION=1.6.21
# Wed, 21 Jun 2023 00:52:39 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Wed, 21 Jun 2023 00:55:49 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 21 Jun 2023 00:55:49 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 21 Jun 2023 00:55:50 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 21 Jun 2023 00:55:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Jun 2023 00:55:50 GMT
USER memcache
# Wed, 21 Jun 2023 00:55:50 GMT
EXPOSE 11211
# Wed, 21 Jun 2023 00:55:50 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:70c60174b18d99741c33011138b5abf2f4d8eca0384521ccb43db3612078e36f`  
		Last Modified: Mon, 12 Jun 2023 23:51:26 GMT  
		Size: 27.0 MB (26982142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52495c3de01d54b61ec15cd608d6ce2ae4587ca764248265b02cb108f790d5a0`  
		Last Modified: Wed, 14 Jun 2023 22:00:39 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:597daa329781ff62c0581a1a2164e04dd294d665a91e97a05aa46fe3d8765eac`  
		Last Modified: Wed, 14 Jun 2023 22:00:40 GMT  
		Size: 2.3 MB (2281778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d65590b8b7bf9398f99bf1baba8d91966081bdc70d61b0165036ac0d16b3b2f`  
		Last Modified: Wed, 21 Jun 2023 00:56:10 GMT  
		Size: 5.8 MB (5829307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dfab31ab9e5a7944b95a42de61a2d1d591fa1605d1a6e2724f9b2c72f03f1ff`  
		Last Modified: Wed, 21 Jun 2023 00:56:09 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85b6795c5e090ce84e068ec9cb629871f3a70380f1bff62aa7baa8a0783343d2`  
		Last Modified: Wed, 21 Jun 2023 00:56:09 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1` - linux; arm variant v7

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

### `memcached:1` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:d82fec3f72f254431725dc57a8b8922cfb269e018b4407c9e7abb133083b1b32
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.9 MB (37872901 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b25fcbe4e1c3b4ce20a4e4994a494fe7a0d98500c1b5b14f4b92c104898a434c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 04 Jul 2023 01:57:35 GMT
ADD file:71fd66666294148382f2e6a09ae5e277d4c4e9c74402ab64b693a79387b67a09 in / 
# Tue, 04 Jul 2023 01:57:36 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 06:40:00 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 04 Jul 2023 06:40:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 06:40:03 GMT
ENV MEMCACHED_VERSION=1.6.21
# Tue, 04 Jul 2023 06:40:03 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Tue, 04 Jul 2023 06:42:47 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 04 Jul 2023 06:42:47 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 04 Jul 2023 06:42:48 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 04 Jul 2023 06:42:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Jul 2023 06:42:48 GMT
USER memcache
# Tue, 04 Jul 2023 06:42:48 GMT
EXPOSE 11211
# Tue, 04 Jul 2023 06:42:48 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:3ae0c06b4d3aa97d7e0829233dd36cea1666b87074e55fea6bd1ecae066693c7`  
		Last Modified: Tue, 04 Jul 2023 02:01:20 GMT  
		Size: 29.2 MB (29152458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7e0b4333d4768ee800aa733f63a51c54833abe7bd20188154f0869796bb3f8c`  
		Last Modified: Tue, 04 Jul 2023 06:43:03 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fd0e2a70b071a1504381d7831ed736d40261b75692a2fe4ee547186e80ad9b2`  
		Last Modified: Tue, 04 Jul 2023 06:43:03 GMT  
		Size: 2.5 MB (2539167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:382aa3014b4367d16a225a23e5195af1f3a5e51523f9d89461e4b98ddf61aa3d`  
		Last Modified: Tue, 04 Jul 2023 06:43:04 GMT  
		Size: 6.2 MB (6179743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4abaeb5f633e1c888b605fe890a58e527c62021db2516cd8606edad49e9500c0`  
		Last Modified: Tue, 04 Jul 2023 06:43:03 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aedc2da2773982e3f9627ea96874aec7c38a4288cca37a366f29392750f7c38`  
		Last Modified: Tue, 04 Jul 2023 06:43:03 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1` - linux; 386

```console
$ docker pull memcached@sha256:d275ff7e4cd6b5d699c14115419af7ae2c1bfa32312282ff8c9ba0b424cf6be0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.5 MB (39457503 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8785d2e661831af23d884d73d3196f416198d2c57ffa24c50c8cafe16c0da224`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 12 Jun 2023 23:39:20 GMT
ADD file:c7ecc5e2bed99e2cbca26f9f4247cd9bc399749556f4084e9357a9b00bb80530 in / 
# Mon, 12 Jun 2023 23:39:20 GMT
CMD ["bash"]
# Wed, 14 Jun 2023 22:34:28 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 14 Jun 2023 22:34:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 21 Jun 2023 00:46:59 GMT
ENV MEMCACHED_VERSION=1.6.21
# Wed, 21 Jun 2023 00:46:59 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Wed, 21 Jun 2023 00:50:45 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 21 Jun 2023 00:50:45 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 21 Jun 2023 00:50:46 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 21 Jun 2023 00:50:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Jun 2023 00:50:46 GMT
USER memcache
# Wed, 21 Jun 2023 00:50:46 GMT
EXPOSE 11211
# Wed, 21 Jun 2023 00:50:46 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:82a41d17956dd7c8ebb39c9ce936fd26841bdbec98d0a185e3db8154b352edff`  
		Last Modified: Mon, 12 Jun 2023 23:46:21 GMT  
		Size: 30.1 MB (30140741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:039125a8cebc58c43be503e98831cac166a973cb3e68f4b66194142680e76964`  
		Last Modified: Wed, 14 Jun 2023 22:42:09 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:199b04439aa2a5065d0c23f986eccd0dd093be2f49b180b332af4f35d977ab5b`  
		Last Modified: Wed, 14 Jun 2023 22:42:09 GMT  
		Size: 2.7 MB (2685017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e58126d70102e38c764aa423066a897bc811895dc85b8d607eadfcff947049a7`  
		Last Modified: Wed, 21 Jun 2023 00:54:46 GMT  
		Size: 6.6 MB (6630215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b039c50c059c1c3a231a9659c8ade08b537d8ecac9423685ba16cf308626c4e4`  
		Last Modified: Wed, 21 Jun 2023 00:54:44 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1d3e144a63d04f26029dacd020e1ec00baeae59c5cee460a482e70842be2fc2`  
		Last Modified: Wed, 21 Jun 2023 00:54:44 GMT  
		Size: 116.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1` - linux; mips64le

```console
$ docker pull memcached@sha256:76620bca6f37fb4a82e0cc3aa33ba7cc2508c8f93dd4ae4956e9b471ce0995a2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.6 MB (37554107 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f8424fcd7f4d7db2c883a9303136b4305e34813630a9e325332ee830d35c026d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 13 Jun 2023 00:09:02 GMT
ADD file:f91bd2a174259cb69646fc34ba2fc6b8941ad8e171d2d7952a4d8ac3d95e2ad7 in / 
# Tue, 13 Jun 2023 00:09:06 GMT
CMD ["bash"]
# Wed, 14 Jun 2023 18:38:15 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 14 Jun 2023 18:38:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 21 Jun 2023 01:14:52 GMT
ENV MEMCACHED_VERSION=1.6.21
# Wed, 21 Jun 2023 01:14:54 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Wed, 21 Jun 2023 01:21:45 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 21 Jun 2023 01:21:47 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 21 Jun 2023 01:21:52 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 21 Jun 2023 01:21:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Jun 2023 01:21:57 GMT
USER memcache
# Wed, 21 Jun 2023 01:22:00 GMT
EXPOSE 11211
# Wed, 21 Jun 2023 01:22:02 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:3fc28260a4d871ef9781cad2bb064ad7212a5063de3a1d35dba938ce82115e5b`  
		Last Modified: Tue, 13 Jun 2023 00:22:29 GMT  
		Size: 29.1 MB (29118129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79c804aeb794275ae845d32d2939d0e0fefa75cd112f1075aaf2104097050ae8`  
		Last Modified: Wed, 14 Jun 2023 18:46:04 GMT  
		Size: 1.1 KB (1078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf29fcbe26928e2f4086a889098220505bdd4401dc87958f623ade0618efcd28`  
		Last Modified: Wed, 14 Jun 2023 18:46:05 GMT  
		Size: 1.9 MB (1934899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1d2070a6fd2a146f7a7ccda5a6b5c9e7188304b3eb6ad56e85ae5e13af6efff`  
		Last Modified: Wed, 21 Jun 2023 01:22:36 GMT  
		Size: 6.5 MB (6499598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb2d53b7e662ee08ffe5d3ff1b97e2bbec271b2427e8428d38ab879c1a68cbdd`  
		Last Modified: Wed, 21 Jun 2023 01:22:31 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e13b007130a18104c8ce3a24f68b588c6ec439dcb4c22e430edf1baab337bb13`  
		Last Modified: Wed, 21 Jun 2023 01:22:31 GMT  
		Size: 118.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1` - linux; ppc64le

```console
$ docker pull memcached@sha256:0466889ea7a59c3e5075122e0dfac5f9fd4b740dbc54d7ca3355e661704b7df3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.2 MB (43193731 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f99a2d51677ef27121ea5fb73098453983811a697bb67558da1548d6a2b1a4d7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 04 Jul 2023 01:17:51 GMT
ADD file:51887002f5002ccc662adbc6ecf1129e3db375a7a77b93da43cc9a8326b3c4b9 in / 
# Tue, 04 Jul 2023 01:17:53 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 06:45:59 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 04 Jul 2023 06:46:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 06:46:11 GMT
ENV MEMCACHED_VERSION=1.6.21
# Tue, 04 Jul 2023 06:46:12 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Tue, 04 Jul 2023 06:50:32 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 04 Jul 2023 06:50:34 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 04 Jul 2023 06:50:36 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 04 Jul 2023 06:50:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Jul 2023 06:50:36 GMT
USER memcache
# Tue, 04 Jul 2023 06:50:37 GMT
EXPOSE 11211
# Tue, 04 Jul 2023 06:50:37 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:ba99a1aa5a92d949d988e66df7723a542fd81bc30eef9d4269e8a899820d4bb2`  
		Last Modified: Tue, 04 Jul 2023 01:24:36 GMT  
		Size: 33.1 MB (33116716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57bc245122d94a5d6dbd04e3f0d2cc3731cb7e5479f873ad6588885b1a1e7fff`  
		Last Modified: Tue, 04 Jul 2023 06:51:13 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8302634866fb43cf1942126242ebd186c7a31db3f01e63b626c2c6cb31aa01bb`  
		Last Modified: Tue, 04 Jul 2023 06:51:14 GMT  
		Size: 2.9 MB (2891325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85b07e92e6621b42a17464a214cee12ada2ca5c70c139194a0d9d5cdf753e470`  
		Last Modified: Tue, 04 Jul 2023 06:51:16 GMT  
		Size: 7.2 MB (7184153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:060e182005428d5f8ae46505c71da839515e43c949a2109682b933781ad7b42d`  
		Last Modified: Tue, 04 Jul 2023 06:51:13 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd71a227a79337edf4a41188a95ac6c897f53d5cc1ebfa6201b14525057ce473`  
		Last Modified: Tue, 04 Jul 2023 06:51:13 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1` - linux; s390x

```console
$ docker pull memcached@sha256:f90935a3646db47ef74efba3a8ea148e6fa9a6058557fd686664b3a9b83cf5b4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.9 MB (35907614 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:55f50234cc8836dd1977a706a4d7845c857ac2128081a776c895db012f73e5bb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 13 Jun 2023 04:29:41 GMT
ADD file:739f4c23557ec0af5f4ba492c847b5d2f09dd81211c675d0e9eabe865d794e81 in / 
# Tue, 13 Jun 2023 04:29:43 GMT
CMD ["bash"]
# Thu, 15 Jun 2023 06:23:25 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Thu, 15 Jun 2023 06:23:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 21 Jun 2023 00:54:39 GMT
ENV MEMCACHED_VERSION=1.6.21
# Wed, 21 Jun 2023 00:54:39 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Wed, 21 Jun 2023 00:57:46 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 21 Jun 2023 00:57:47 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 21 Jun 2023 00:57:47 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 21 Jun 2023 00:57:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Jun 2023 00:57:47 GMT
USER memcache
# Wed, 21 Jun 2023 00:57:47 GMT
EXPOSE 11211
# Wed, 21 Jun 2023 00:57:48 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:6571b3abd058e377c7bd231c9029aff6eb25486bffb50229076d2e6a356a517f`  
		Last Modified: Tue, 13 Jun 2023 04:34:21 GMT  
		Size: 27.5 MB (27487928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1521043364f590f749ce68598ad1f79907ef04ee2283314cfaab3f72df8e15c`  
		Last Modified: Thu, 15 Jun 2023 06:35:17 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdbc1e75c128be037526f9b133061f5dc6c9baf2f00b5d5b229427bd89eb55b7`  
		Last Modified: Thu, 15 Jun 2023 06:35:18 GMT  
		Size: 2.3 MB (2345340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f3d048c5c76c19c7c7d783cac8384f5698dd61a6aa7ee9067521407789ec9b4`  
		Last Modified: Wed, 21 Jun 2023 01:01:34 GMT  
		Size: 6.1 MB (6072815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c7bfbb7d1965d17408766d01c40f67a94eb422714618a239a48b62cedafdcab`  
		Last Modified: Wed, 21 Jun 2023 01:01:33 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:164d3c9aaa0239a91376552d50ffc16a1e2bf9e3c323e81d2a976556ab25f4a2`  
		Last Modified: Wed, 21 Jun 2023 01:01:33 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:1-alpine`

```console
$ docker pull memcached@sha256:32f2ba37c2ed2ef922efa0190faa71dc3b4f1df4a3e50938a0b3afe3d589a1d9
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
$ docker pull memcached@sha256:574ef430513a38925cc52ae5954677a12e0a57205fed96be5707196a180e5159
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4462428 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f7da63106561ab1f7284992dad2396b234096070b4269971b23c53f2f8498ef`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 14 Jun 2023 20:41:58 GMT
ADD file:1da756d12551a0e3e793e02ef87432d69d4968937bd11bed0af215db19dd94cd in / 
# Wed, 14 Jun 2023 20:41:59 GMT
CMD ["/bin/sh"]
# Wed, 14 Jun 2023 20:50:58 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Wed, 14 Jun 2023 20:50:59 GMT
RUN apk add --no-cache libsasl
# Wed, 21 Jun 2023 01:07:13 GMT
ENV MEMCACHED_VERSION=1.6.21
# Wed, 21 Jun 2023 01:07:13 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Wed, 21 Jun 2023 01:09:21 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Wed, 21 Jun 2023 01:09:21 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 21 Jun 2023 01:09:22 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 21 Jun 2023 01:09:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Jun 2023 01:09:22 GMT
USER memcache
# Wed, 21 Jun 2023 01:09:22 GMT
EXPOSE 11211
# Wed, 21 Jun 2023 01:09:22 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:31e352740f534f9ad170f75378a84fe453d6156e40700b882d737a8f4a6988a3`  
		Last Modified: Wed, 14 Jun 2023 20:42:26 GMT  
		Size: 3.4 MB (3397879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b2b2df106c5026cd33ea4ac655b77f25410ec9f4b8a6756ebc1ceeb79fca3c7`  
		Last Modified: Wed, 14 Jun 2023 20:53:58 GMT  
		Size: 1.3 KB (1266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed63668528d3e2159f55909c66dc48a6f746ce24c2e2f6d963b992aefaa457ce`  
		Last Modified: Wed, 14 Jun 2023 20:53:58 GMT  
		Size: 108.1 KB (108080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05536f2f26c904a5aa1b07720957a37e8b57a223725d76f8d1473dcab297a233`  
		Last Modified: Wed, 21 Jun 2023 01:10:14 GMT  
		Size: 954.8 KB (954811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e448b573a98adc8bd0a4805cb0e1b451aea0d1582f0462aa0b147799a97fad7`  
		Last Modified: Wed, 21 Jun 2023 01:10:13 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3029a709b7be20aeff1e9cebe5c6112cd1df5a0ea3efb58e61380cc75b9296e`  
		Last Modified: Wed, 21 Jun 2023 01:10:13 GMT  
		Size: 117.0 B  
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
$ docker pull memcached@sha256:eb4b801b9c9e9af6565ac003b21af39b06d55943bbc4e59a02d465fdf7f07776
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.4 MB (4399342 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4aa99dd98a2fa001241d907951530f4afebadfd4895545c5d73f31e29b7a35fa`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 14 Jun 2023 20:48:58 GMT
ADD file:289c2fac17119508ced527225d445747cd177111b4a0018a6b04948ecb3b5e29 in / 
# Wed, 14 Jun 2023 20:48:58 GMT
CMD ["/bin/sh"]
# Wed, 14 Jun 2023 20:57:26 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Wed, 14 Jun 2023 20:57:27 GMT
RUN apk add --no-cache libsasl
# Wed, 21 Jun 2023 01:08:09 GMT
ENV MEMCACHED_VERSION=1.6.21
# Wed, 21 Jun 2023 01:08:09 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Wed, 21 Jun 2023 01:10:35 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Wed, 21 Jun 2023 01:10:35 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 21 Jun 2023 01:10:36 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 21 Jun 2023 01:10:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Jun 2023 01:10:36 GMT
USER memcache
# Wed, 21 Jun 2023 01:10:36 GMT
EXPOSE 11211
# Wed, 21 Jun 2023 01:10:36 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:8c6d1654570f041603f4cef49c320c8f6f3e401324913009d92a19132cbf1ac0`  
		Last Modified: Wed, 14 Jun 2023 20:49:23 GMT  
		Size: 3.3 MB (3329251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:666588188768f19b27fb821e02d084406af8fd867cc4595b896b9eed50b2105e`  
		Last Modified: Wed, 14 Jun 2023 21:00:51 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7d958a137d671266f063c0af4d7b0b6d44d9018b77fdbddb8fd412d3c0b1be3`  
		Last Modified: Wed, 14 Jun 2023 21:00:51 GMT  
		Size: 124.1 KB (124137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a66841dcfe05dcef1af82648941fa1ea0e10dbdf022326916d1d74afc99885c6`  
		Last Modified: Wed, 21 Jun 2023 01:11:21 GMT  
		Size: 944.3 KB (944292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b46fdc76bcbc8fa94ae23177ac32b97a4d370a630ec7d3f52bd8aae174e75982`  
		Last Modified: Wed, 21 Jun 2023 01:11:20 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea70db1a59f508c629aef54fb39ac3ada5cfcc3aac7aa1d6ed6cde22e97d3e3b`  
		Last Modified: Wed, 21 Jun 2023 01:11:20 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-alpine` - linux; 386

```console
$ docker pull memcached@sha256:73c987449b9f764e060e2745d29e0ee50f4f7e630ddd23631c517e65f2315bfa
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.3 MB (4282253 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c47771f0d8f2ab5f38441f65fed7a05d87ea44b1de1a502321348997971362c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 14 Jun 2023 22:33:22 GMT
ADD file:94bec00e2c0c7f47c81ec4355a29ca23a81b439797d037b1a5a455f36a25dab4 in / 
# Wed, 14 Jun 2023 22:33:22 GMT
CMD ["/bin/sh"]
# Wed, 14 Jun 2023 22:38:20 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Wed, 14 Jun 2023 22:38:22 GMT
RUN apk add --no-cache libsasl
# Wed, 21 Jun 2023 00:50:52 GMT
ENV MEMCACHED_VERSION=1.6.21
# Wed, 21 Jun 2023 00:50:52 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Wed, 21 Jun 2023 00:54:21 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Wed, 21 Jun 2023 00:54:22 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 21 Jun 2023 00:54:22 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 21 Jun 2023 00:54:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Jun 2023 00:54:22 GMT
USER memcache
# Wed, 21 Jun 2023 00:54:22 GMT
EXPOSE 11211
# Wed, 21 Jun 2023 00:54:23 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:b3f50075abd13aad1cb7d8c1427aa59d7fcac88f3690d3f9c3efdbec80fd0856`  
		Last Modified: Wed, 14 Jun 2023 22:33:48 GMT  
		Size: 3.2 MB (3233951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:358673fc695429dd9142a4904a518e96c418229121d02435d875a993d9e5fac1`  
		Last Modified: Wed, 14 Jun 2023 22:42:32 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ae09e638ab1208326cbfd03f4517b0d1d13f72cfc8add3a055321fe5cf0f53a`  
		Last Modified: Wed, 14 Jun 2023 22:42:32 GMT  
		Size: 109.5 KB (109531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ed35577a5a4360f65bc0361d7bca857e45fad4baf04bcde5e731529377e9f58`  
		Last Modified: Wed, 21 Jun 2023 00:55:07 GMT  
		Size: 937.1 KB (937107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c4024dd0449592764b513374729cea0a478f62deaf32af4b23e536ffca016b6`  
		Last Modified: Wed, 21 Jun 2023 00:55:07 GMT  
		Size: 280.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6d29f640e8837bc0d0ed4b3fc505f71494f0c3ef917245b2399971ca3cb38e8`  
		Last Modified: Wed, 21 Jun 2023 00:55:06 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-alpine` - linux; ppc64le

```console
$ docker pull memcached@sha256:e02abd3f1c109243a103019450a45039503d018c8fcd2fb607798643fbeaed69
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4453245 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7311794e1380b44e42daf3ea3c49269eb71549d5f62a46f6596478d01bda3b02`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 15 Jun 2023 00:39:49 GMT
ADD file:694c636c0dd19fd01accbc189e4c1dc4d063952692c6e7eb26dce02a7adba833 in / 
# Thu, 15 Jun 2023 00:39:49 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 04:20:00 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Thu, 15 Jun 2023 04:20:03 GMT
RUN apk add --no-cache libsasl
# Wed, 21 Jun 2023 01:42:40 GMT
ENV MEMCACHED_VERSION=1.6.21
# Wed, 21 Jun 2023 01:42:40 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Wed, 21 Jun 2023 01:45:42 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Wed, 21 Jun 2023 01:45:43 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 21 Jun 2023 01:45:45 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 21 Jun 2023 01:45:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Jun 2023 01:45:46 GMT
USER memcache
# Wed, 21 Jun 2023 01:45:46 GMT
EXPOSE 11211
# Wed, 21 Jun 2023 01:45:47 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:ffa4a466dbb8eebd7e7f25590a9df12390de9016abf82279c29c9a64aa76491a`  
		Last Modified: Thu, 15 Jun 2023 00:40:26 GMT  
		Size: 3.3 MB (3344781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:607cb6edfb2d0718375d44dbfb94d80d9b5e23a38a6bad8d2fe9c624a0ae354a`  
		Last Modified: Thu, 15 Jun 2023 04:23:36 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f97572f9bc2bc81fb5496a46ecd8b44cdb5b616d0beaecaabb186e3523683a32`  
		Last Modified: Thu, 15 Jun 2023 04:23:37 GMT  
		Size: 123.9 KB (123931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da5b2f6c7aee3051aa1b53ff9a66885509bad54b27aa37aebe382fc1ca4eab1f`  
		Last Modified: Wed, 21 Jun 2023 01:46:43 GMT  
		Size: 982.9 KB (982864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a08963a0c7d8349568389e6f7af0c7a1b55f2b0aea5d25bfa94d415fbb94af9`  
		Last Modified: Wed, 21 Jun 2023 01:46:43 GMT  
		Size: 282.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d866cc948bf60127d37a1f655a84d6b9c17376a21656e660c47efc6d3f499ba2`  
		Last Modified: Wed, 21 Jun 2023 01:46:43 GMT  
		Size: 118.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-alpine` - linux; s390x

```console
$ docker pull memcached@sha256:cd97d93e79c2345a0c10f20a912f29a0ccf5590e15c00df81596397b9567233f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.3 MB (4278263 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f56d14fce8cfd200c86bd00cd28c95574b6bf2863bd203e7644d44a08db84ab`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 15 Jun 2023 05:18:38 GMT
ADD file:a59beca78118ebf4f86cc1685237dc3a29a519401a70668da520beaa3d29eb7a in / 
# Thu, 15 Jun 2023 05:18:38 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 06:27:47 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Thu, 15 Jun 2023 06:27:49 GMT
RUN apk add --no-cache libsasl
# Wed, 21 Jun 2023 00:58:01 GMT
ENV MEMCACHED_VERSION=1.6.21
# Wed, 21 Jun 2023 00:58:01 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Wed, 21 Jun 2023 01:01:08 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Wed, 21 Jun 2023 01:01:09 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 21 Jun 2023 01:01:09 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 21 Jun 2023 01:01:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Jun 2023 01:01:09 GMT
USER memcache
# Wed, 21 Jun 2023 01:01:10 GMT
EXPOSE 11211
# Wed, 21 Jun 2023 01:01:10 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:998cc98447b44e5f0fe799dce691412796ba586ab22eb7c99aebf9d45f34833b`  
		Last Modified: Thu, 15 Jun 2023 05:29:38 GMT  
		Size: 3.2 MB (3213497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:156deb87465a2c5629e5ae28c2a7251d5684baea5a930cf65ff6b478de321202`  
		Last Modified: Thu, 15 Jun 2023 06:36:33 GMT  
		Size: 1.3 KB (1266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19020c60d58f4724218660e819b1b33b5d1428c3c5027492a2ee3c44228231df`  
		Last Modified: Thu, 15 Jun 2023 06:36:33 GMT  
		Size: 112.8 KB (112849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81e76f938f015ccb0b5d2915145432efbc0af21a2f4964e0c9a67bfbbe6a577e`  
		Last Modified: Wed, 21 Jun 2023 01:01:46 GMT  
		Size: 950.3 KB (950254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b613e0a69ced3425a5949c15688d493ef10d80eb28c7bb626f0c092223fe1302`  
		Last Modified: Wed, 21 Jun 2023 01:01:46 GMT  
		Size: 280.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4db4c30d38bb65cd11068e1892913b2fa04add8f27abe601485cc3b09754eb50`  
		Last Modified: Wed, 21 Jun 2023 01:01:46 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:1-alpine3.18`

```console
$ docker pull memcached@sha256:ee437fd9a952b48de768cd5c7a97d43439e05b918e4bc4452e296e8bdafae046
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `memcached:1-alpine3.18` - linux; amd64

```console
$ docker pull memcached@sha256:574ef430513a38925cc52ae5954677a12e0a57205fed96be5707196a180e5159
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4462428 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f7da63106561ab1f7284992dad2396b234096070b4269971b23c53f2f8498ef`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 14 Jun 2023 20:41:58 GMT
ADD file:1da756d12551a0e3e793e02ef87432d69d4968937bd11bed0af215db19dd94cd in / 
# Wed, 14 Jun 2023 20:41:59 GMT
CMD ["/bin/sh"]
# Wed, 14 Jun 2023 20:50:58 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Wed, 14 Jun 2023 20:50:59 GMT
RUN apk add --no-cache libsasl
# Wed, 21 Jun 2023 01:07:13 GMT
ENV MEMCACHED_VERSION=1.6.21
# Wed, 21 Jun 2023 01:07:13 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Wed, 21 Jun 2023 01:09:21 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Wed, 21 Jun 2023 01:09:21 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 21 Jun 2023 01:09:22 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 21 Jun 2023 01:09:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Jun 2023 01:09:22 GMT
USER memcache
# Wed, 21 Jun 2023 01:09:22 GMT
EXPOSE 11211
# Wed, 21 Jun 2023 01:09:22 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:31e352740f534f9ad170f75378a84fe453d6156e40700b882d737a8f4a6988a3`  
		Last Modified: Wed, 14 Jun 2023 20:42:26 GMT  
		Size: 3.4 MB (3397879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b2b2df106c5026cd33ea4ac655b77f25410ec9f4b8a6756ebc1ceeb79fca3c7`  
		Last Modified: Wed, 14 Jun 2023 20:53:58 GMT  
		Size: 1.3 KB (1266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed63668528d3e2159f55909c66dc48a6f746ce24c2e2f6d963b992aefaa457ce`  
		Last Modified: Wed, 14 Jun 2023 20:53:58 GMT  
		Size: 108.1 KB (108080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05536f2f26c904a5aa1b07720957a37e8b57a223725d76f8d1473dcab297a233`  
		Last Modified: Wed, 21 Jun 2023 01:10:14 GMT  
		Size: 954.8 KB (954811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e448b573a98adc8bd0a4805cb0e1b451aea0d1582f0462aa0b147799a97fad7`  
		Last Modified: Wed, 21 Jun 2023 01:10:13 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3029a709b7be20aeff1e9cebe5c6112cd1df5a0ea3efb58e61380cc75b9296e`  
		Last Modified: Wed, 21 Jun 2023 01:10:13 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-alpine3.18` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:eb4b801b9c9e9af6565ac003b21af39b06d55943bbc4e59a02d465fdf7f07776
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.4 MB (4399342 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4aa99dd98a2fa001241d907951530f4afebadfd4895545c5d73f31e29b7a35fa`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 14 Jun 2023 20:48:58 GMT
ADD file:289c2fac17119508ced527225d445747cd177111b4a0018a6b04948ecb3b5e29 in / 
# Wed, 14 Jun 2023 20:48:58 GMT
CMD ["/bin/sh"]
# Wed, 14 Jun 2023 20:57:26 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Wed, 14 Jun 2023 20:57:27 GMT
RUN apk add --no-cache libsasl
# Wed, 21 Jun 2023 01:08:09 GMT
ENV MEMCACHED_VERSION=1.6.21
# Wed, 21 Jun 2023 01:08:09 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Wed, 21 Jun 2023 01:10:35 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Wed, 21 Jun 2023 01:10:35 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 21 Jun 2023 01:10:36 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 21 Jun 2023 01:10:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Jun 2023 01:10:36 GMT
USER memcache
# Wed, 21 Jun 2023 01:10:36 GMT
EXPOSE 11211
# Wed, 21 Jun 2023 01:10:36 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:8c6d1654570f041603f4cef49c320c8f6f3e401324913009d92a19132cbf1ac0`  
		Last Modified: Wed, 14 Jun 2023 20:49:23 GMT  
		Size: 3.3 MB (3329251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:666588188768f19b27fb821e02d084406af8fd867cc4595b896b9eed50b2105e`  
		Last Modified: Wed, 14 Jun 2023 21:00:51 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7d958a137d671266f063c0af4d7b0b6d44d9018b77fdbddb8fd412d3c0b1be3`  
		Last Modified: Wed, 14 Jun 2023 21:00:51 GMT  
		Size: 124.1 KB (124137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a66841dcfe05dcef1af82648941fa1ea0e10dbdf022326916d1d74afc99885c6`  
		Last Modified: Wed, 21 Jun 2023 01:11:21 GMT  
		Size: 944.3 KB (944292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b46fdc76bcbc8fa94ae23177ac32b97a4d370a630ec7d3f52bd8aae174e75982`  
		Last Modified: Wed, 21 Jun 2023 01:11:20 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea70db1a59f508c629aef54fb39ac3ada5cfcc3aac7aa1d6ed6cde22e97d3e3b`  
		Last Modified: Wed, 21 Jun 2023 01:11:20 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-alpine3.18` - linux; 386

```console
$ docker pull memcached@sha256:73c987449b9f764e060e2745d29e0ee50f4f7e630ddd23631c517e65f2315bfa
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.3 MB (4282253 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c47771f0d8f2ab5f38441f65fed7a05d87ea44b1de1a502321348997971362c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 14 Jun 2023 22:33:22 GMT
ADD file:94bec00e2c0c7f47c81ec4355a29ca23a81b439797d037b1a5a455f36a25dab4 in / 
# Wed, 14 Jun 2023 22:33:22 GMT
CMD ["/bin/sh"]
# Wed, 14 Jun 2023 22:38:20 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Wed, 14 Jun 2023 22:38:22 GMT
RUN apk add --no-cache libsasl
# Wed, 21 Jun 2023 00:50:52 GMT
ENV MEMCACHED_VERSION=1.6.21
# Wed, 21 Jun 2023 00:50:52 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Wed, 21 Jun 2023 00:54:21 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Wed, 21 Jun 2023 00:54:22 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 21 Jun 2023 00:54:22 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 21 Jun 2023 00:54:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Jun 2023 00:54:22 GMT
USER memcache
# Wed, 21 Jun 2023 00:54:22 GMT
EXPOSE 11211
# Wed, 21 Jun 2023 00:54:23 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:b3f50075abd13aad1cb7d8c1427aa59d7fcac88f3690d3f9c3efdbec80fd0856`  
		Last Modified: Wed, 14 Jun 2023 22:33:48 GMT  
		Size: 3.2 MB (3233951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:358673fc695429dd9142a4904a518e96c418229121d02435d875a993d9e5fac1`  
		Last Modified: Wed, 14 Jun 2023 22:42:32 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ae09e638ab1208326cbfd03f4517b0d1d13f72cfc8add3a055321fe5cf0f53a`  
		Last Modified: Wed, 14 Jun 2023 22:42:32 GMT  
		Size: 109.5 KB (109531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ed35577a5a4360f65bc0361d7bca857e45fad4baf04bcde5e731529377e9f58`  
		Last Modified: Wed, 21 Jun 2023 00:55:07 GMT  
		Size: 937.1 KB (937107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c4024dd0449592764b513374729cea0a478f62deaf32af4b23e536ffca016b6`  
		Last Modified: Wed, 21 Jun 2023 00:55:07 GMT  
		Size: 280.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6d29f640e8837bc0d0ed4b3fc505f71494f0c3ef917245b2399971ca3cb38e8`  
		Last Modified: Wed, 21 Jun 2023 00:55:06 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-alpine3.18` - linux; ppc64le

```console
$ docker pull memcached@sha256:e02abd3f1c109243a103019450a45039503d018c8fcd2fb607798643fbeaed69
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4453245 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7311794e1380b44e42daf3ea3c49269eb71549d5f62a46f6596478d01bda3b02`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 15 Jun 2023 00:39:49 GMT
ADD file:694c636c0dd19fd01accbc189e4c1dc4d063952692c6e7eb26dce02a7adba833 in / 
# Thu, 15 Jun 2023 00:39:49 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 04:20:00 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Thu, 15 Jun 2023 04:20:03 GMT
RUN apk add --no-cache libsasl
# Wed, 21 Jun 2023 01:42:40 GMT
ENV MEMCACHED_VERSION=1.6.21
# Wed, 21 Jun 2023 01:42:40 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Wed, 21 Jun 2023 01:45:42 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Wed, 21 Jun 2023 01:45:43 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 21 Jun 2023 01:45:45 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 21 Jun 2023 01:45:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Jun 2023 01:45:46 GMT
USER memcache
# Wed, 21 Jun 2023 01:45:46 GMT
EXPOSE 11211
# Wed, 21 Jun 2023 01:45:47 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:ffa4a466dbb8eebd7e7f25590a9df12390de9016abf82279c29c9a64aa76491a`  
		Last Modified: Thu, 15 Jun 2023 00:40:26 GMT  
		Size: 3.3 MB (3344781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:607cb6edfb2d0718375d44dbfb94d80d9b5e23a38a6bad8d2fe9c624a0ae354a`  
		Last Modified: Thu, 15 Jun 2023 04:23:36 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f97572f9bc2bc81fb5496a46ecd8b44cdb5b616d0beaecaabb186e3523683a32`  
		Last Modified: Thu, 15 Jun 2023 04:23:37 GMT  
		Size: 123.9 KB (123931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da5b2f6c7aee3051aa1b53ff9a66885509bad54b27aa37aebe382fc1ca4eab1f`  
		Last Modified: Wed, 21 Jun 2023 01:46:43 GMT  
		Size: 982.9 KB (982864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a08963a0c7d8349568389e6f7af0c7a1b55f2b0aea5d25bfa94d415fbb94af9`  
		Last Modified: Wed, 21 Jun 2023 01:46:43 GMT  
		Size: 282.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d866cc948bf60127d37a1f655a84d6b9c17376a21656e660c47efc6d3f499ba2`  
		Last Modified: Wed, 21 Jun 2023 01:46:43 GMT  
		Size: 118.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-alpine3.18` - linux; s390x

```console
$ docker pull memcached@sha256:cd97d93e79c2345a0c10f20a912f29a0ccf5590e15c00df81596397b9567233f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.3 MB (4278263 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f56d14fce8cfd200c86bd00cd28c95574b6bf2863bd203e7644d44a08db84ab`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 15 Jun 2023 05:18:38 GMT
ADD file:a59beca78118ebf4f86cc1685237dc3a29a519401a70668da520beaa3d29eb7a in / 
# Thu, 15 Jun 2023 05:18:38 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 06:27:47 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Thu, 15 Jun 2023 06:27:49 GMT
RUN apk add --no-cache libsasl
# Wed, 21 Jun 2023 00:58:01 GMT
ENV MEMCACHED_VERSION=1.6.21
# Wed, 21 Jun 2023 00:58:01 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Wed, 21 Jun 2023 01:01:08 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Wed, 21 Jun 2023 01:01:09 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 21 Jun 2023 01:01:09 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 21 Jun 2023 01:01:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Jun 2023 01:01:09 GMT
USER memcache
# Wed, 21 Jun 2023 01:01:10 GMT
EXPOSE 11211
# Wed, 21 Jun 2023 01:01:10 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:998cc98447b44e5f0fe799dce691412796ba586ab22eb7c99aebf9d45f34833b`  
		Last Modified: Thu, 15 Jun 2023 05:29:38 GMT  
		Size: 3.2 MB (3213497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:156deb87465a2c5629e5ae28c2a7251d5684baea5a930cf65ff6b478de321202`  
		Last Modified: Thu, 15 Jun 2023 06:36:33 GMT  
		Size: 1.3 KB (1266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19020c60d58f4724218660e819b1b33b5d1428c3c5027492a2ee3c44228231df`  
		Last Modified: Thu, 15 Jun 2023 06:36:33 GMT  
		Size: 112.8 KB (112849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81e76f938f015ccb0b5d2915145432efbc0af21a2f4964e0c9a67bfbbe6a577e`  
		Last Modified: Wed, 21 Jun 2023 01:01:46 GMT  
		Size: 950.3 KB (950254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b613e0a69ced3425a5949c15688d493ef10d80eb28c7bb626f0c092223fe1302`  
		Last Modified: Wed, 21 Jun 2023 01:01:46 GMT  
		Size: 280.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4db4c30d38bb65cd11068e1892913b2fa04add8f27abe601485cc3b09754eb50`  
		Last Modified: Wed, 21 Jun 2023 01:01:46 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:1-bookworm`

```console
$ docker pull memcached@sha256:6d50bee6d0eaba83831fead39d52d67ede2aefc3acf69a19d503a9488234e1c8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 7
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; s390x

### `memcached:1-bookworm` - linux; amd64

```console
$ docker pull memcached@sha256:37d77084cbe7c98854989a68a18f22dd677379de8ffc9ee92fbf7b88b2b4d0f9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.0 MB (38973142 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a4d0c1490511995c15a4c1ca7c8413337bed068ea95507aae882010b051ca37e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 12 Jun 2023 23:20:42 GMT
ADD file:ba1250b6ecd5dd09d4914189d72741c2817988994e7da514bf62be439a34bdb5 in / 
# Mon, 12 Jun 2023 23:20:42 GMT
CMD ["bash"]
# Wed, 14 Jun 2023 20:48:19 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 14 Jun 2023 20:48:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 21 Jun 2023 01:04:34 GMT
ENV MEMCACHED_VERSION=1.6.21
# Wed, 21 Jun 2023 01:04:35 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Wed, 21 Jun 2023 01:07:04 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 21 Jun 2023 01:07:04 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 21 Jun 2023 01:07:04 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 21 Jun 2023 01:07:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Jun 2023 01:07:05 GMT
USER memcache
# Wed, 21 Jun 2023 01:07:05 GMT
EXPOSE 11211
# Wed, 21 Jun 2023 01:07:05 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:5b5fe70539cd6989aa19f25826309f9715a9489cf1c057982d6a84c1ad8975c7`  
		Last Modified: Mon, 12 Jun 2023 23:25:49 GMT  
		Size: 29.1 MB (29124744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab209434009a85e82d99c0547bb947940f9e1002ce6e965417396ee22a6820db`  
		Last Modified: Wed, 14 Jun 2023 20:53:33 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2f4dfc49c9cdae8d4df855de7cc0460e5db8c762e73786d4f8fa4f69ba11d6d`  
		Last Modified: Wed, 14 Jun 2023 20:53:33 GMT  
		Size: 2.7 MB (2677239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d5a41694f99632bb3a7c624dab437c8a10e54b92965de823e717f5c12326b1e`  
		Last Modified: Wed, 21 Jun 2023 01:09:52 GMT  
		Size: 7.2 MB (7169627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2be3d7709e1978d4b030abdf5ac129b97f21e09bb489932628899d96288a4a9`  
		Last Modified: Wed, 21 Jun 2023 01:09:50 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8cba3f7cc400544285611f46bbdba004587f84511783fd05aa6562e9337928f`  
		Last Modified: Wed, 21 Jun 2023 01:09:50 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-bookworm` - linux; arm variant v5

```console
$ docker pull memcached@sha256:1646b01539b9482149379208acae5c0af1c5aed3aa9d818e8748410e15170943
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.1 MB (35094759 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ad4aa07800c4cf602e699a614c04d8fa80a8617828cfeb89fc05b49791d07e7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 12 Jun 2023 23:48:31 GMT
ADD file:54a716f17b23e4fa49d1d5c0a7f63becc295873c116d19bb4753d34f1ca6affb in / 
# Mon, 12 Jun 2023 23:48:31 GMT
CMD ["bash"]
# Wed, 14 Jun 2023 21:56:18 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 14 Jun 2023 21:56:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 21 Jun 2023 00:52:38 GMT
ENV MEMCACHED_VERSION=1.6.21
# Wed, 21 Jun 2023 00:52:39 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Wed, 21 Jun 2023 00:55:49 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 21 Jun 2023 00:55:49 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 21 Jun 2023 00:55:50 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 21 Jun 2023 00:55:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Jun 2023 00:55:50 GMT
USER memcache
# Wed, 21 Jun 2023 00:55:50 GMT
EXPOSE 11211
# Wed, 21 Jun 2023 00:55:50 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:70c60174b18d99741c33011138b5abf2f4d8eca0384521ccb43db3612078e36f`  
		Last Modified: Mon, 12 Jun 2023 23:51:26 GMT  
		Size: 27.0 MB (26982142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52495c3de01d54b61ec15cd608d6ce2ae4587ca764248265b02cb108f790d5a0`  
		Last Modified: Wed, 14 Jun 2023 22:00:39 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:597daa329781ff62c0581a1a2164e04dd294d665a91e97a05aa46fe3d8765eac`  
		Last Modified: Wed, 14 Jun 2023 22:00:40 GMT  
		Size: 2.3 MB (2281778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d65590b8b7bf9398f99bf1baba8d91966081bdc70d61b0165036ac0d16b3b2f`  
		Last Modified: Wed, 21 Jun 2023 00:56:10 GMT  
		Size: 5.8 MB (5829307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dfab31ab9e5a7944b95a42de61a2d1d591fa1605d1a6e2724f9b2c72f03f1ff`  
		Last Modified: Wed, 21 Jun 2023 00:56:09 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85b6795c5e090ce84e068ec9cb629871f3a70380f1bff62aa7baa8a0783343d2`  
		Last Modified: Wed, 21 Jun 2023 00:56:09 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-bookworm` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:d82fec3f72f254431725dc57a8b8922cfb269e018b4407c9e7abb133083b1b32
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.9 MB (37872901 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b25fcbe4e1c3b4ce20a4e4994a494fe7a0d98500c1b5b14f4b92c104898a434c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 04 Jul 2023 01:57:35 GMT
ADD file:71fd66666294148382f2e6a09ae5e277d4c4e9c74402ab64b693a79387b67a09 in / 
# Tue, 04 Jul 2023 01:57:36 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 06:40:00 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 04 Jul 2023 06:40:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 06:40:03 GMT
ENV MEMCACHED_VERSION=1.6.21
# Tue, 04 Jul 2023 06:40:03 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Tue, 04 Jul 2023 06:42:47 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 04 Jul 2023 06:42:47 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 04 Jul 2023 06:42:48 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 04 Jul 2023 06:42:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Jul 2023 06:42:48 GMT
USER memcache
# Tue, 04 Jul 2023 06:42:48 GMT
EXPOSE 11211
# Tue, 04 Jul 2023 06:42:48 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:3ae0c06b4d3aa97d7e0829233dd36cea1666b87074e55fea6bd1ecae066693c7`  
		Last Modified: Tue, 04 Jul 2023 02:01:20 GMT  
		Size: 29.2 MB (29152458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7e0b4333d4768ee800aa733f63a51c54833abe7bd20188154f0869796bb3f8c`  
		Last Modified: Tue, 04 Jul 2023 06:43:03 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fd0e2a70b071a1504381d7831ed736d40261b75692a2fe4ee547186e80ad9b2`  
		Last Modified: Tue, 04 Jul 2023 06:43:03 GMT  
		Size: 2.5 MB (2539167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:382aa3014b4367d16a225a23e5195af1f3a5e51523f9d89461e4b98ddf61aa3d`  
		Last Modified: Tue, 04 Jul 2023 06:43:04 GMT  
		Size: 6.2 MB (6179743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4abaeb5f633e1c888b605fe890a58e527c62021db2516cd8606edad49e9500c0`  
		Last Modified: Tue, 04 Jul 2023 06:43:03 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aedc2da2773982e3f9627ea96874aec7c38a4288cca37a366f29392750f7c38`  
		Last Modified: Tue, 04 Jul 2023 06:43:03 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-bookworm` - linux; 386

```console
$ docker pull memcached@sha256:d275ff7e4cd6b5d699c14115419af7ae2c1bfa32312282ff8c9ba0b424cf6be0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.5 MB (39457503 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8785d2e661831af23d884d73d3196f416198d2c57ffa24c50c8cafe16c0da224`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 12 Jun 2023 23:39:20 GMT
ADD file:c7ecc5e2bed99e2cbca26f9f4247cd9bc399749556f4084e9357a9b00bb80530 in / 
# Mon, 12 Jun 2023 23:39:20 GMT
CMD ["bash"]
# Wed, 14 Jun 2023 22:34:28 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 14 Jun 2023 22:34:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 21 Jun 2023 00:46:59 GMT
ENV MEMCACHED_VERSION=1.6.21
# Wed, 21 Jun 2023 00:46:59 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Wed, 21 Jun 2023 00:50:45 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 21 Jun 2023 00:50:45 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 21 Jun 2023 00:50:46 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 21 Jun 2023 00:50:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Jun 2023 00:50:46 GMT
USER memcache
# Wed, 21 Jun 2023 00:50:46 GMT
EXPOSE 11211
# Wed, 21 Jun 2023 00:50:46 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:82a41d17956dd7c8ebb39c9ce936fd26841bdbec98d0a185e3db8154b352edff`  
		Last Modified: Mon, 12 Jun 2023 23:46:21 GMT  
		Size: 30.1 MB (30140741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:039125a8cebc58c43be503e98831cac166a973cb3e68f4b66194142680e76964`  
		Last Modified: Wed, 14 Jun 2023 22:42:09 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:199b04439aa2a5065d0c23f986eccd0dd093be2f49b180b332af4f35d977ab5b`  
		Last Modified: Wed, 14 Jun 2023 22:42:09 GMT  
		Size: 2.7 MB (2685017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e58126d70102e38c764aa423066a897bc811895dc85b8d607eadfcff947049a7`  
		Last Modified: Wed, 21 Jun 2023 00:54:46 GMT  
		Size: 6.6 MB (6630215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b039c50c059c1c3a231a9659c8ade08b537d8ecac9423685ba16cf308626c4e4`  
		Last Modified: Wed, 21 Jun 2023 00:54:44 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1d3e144a63d04f26029dacd020e1ec00baeae59c5cee460a482e70842be2fc2`  
		Last Modified: Wed, 21 Jun 2023 00:54:44 GMT  
		Size: 116.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-bookworm` - linux; mips64le

```console
$ docker pull memcached@sha256:76620bca6f37fb4a82e0cc3aa33ba7cc2508c8f93dd4ae4956e9b471ce0995a2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.6 MB (37554107 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f8424fcd7f4d7db2c883a9303136b4305e34813630a9e325332ee830d35c026d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 13 Jun 2023 00:09:02 GMT
ADD file:f91bd2a174259cb69646fc34ba2fc6b8941ad8e171d2d7952a4d8ac3d95e2ad7 in / 
# Tue, 13 Jun 2023 00:09:06 GMT
CMD ["bash"]
# Wed, 14 Jun 2023 18:38:15 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 14 Jun 2023 18:38:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 21 Jun 2023 01:14:52 GMT
ENV MEMCACHED_VERSION=1.6.21
# Wed, 21 Jun 2023 01:14:54 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Wed, 21 Jun 2023 01:21:45 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 21 Jun 2023 01:21:47 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 21 Jun 2023 01:21:52 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 21 Jun 2023 01:21:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Jun 2023 01:21:57 GMT
USER memcache
# Wed, 21 Jun 2023 01:22:00 GMT
EXPOSE 11211
# Wed, 21 Jun 2023 01:22:02 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:3fc28260a4d871ef9781cad2bb064ad7212a5063de3a1d35dba938ce82115e5b`  
		Last Modified: Tue, 13 Jun 2023 00:22:29 GMT  
		Size: 29.1 MB (29118129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79c804aeb794275ae845d32d2939d0e0fefa75cd112f1075aaf2104097050ae8`  
		Last Modified: Wed, 14 Jun 2023 18:46:04 GMT  
		Size: 1.1 KB (1078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf29fcbe26928e2f4086a889098220505bdd4401dc87958f623ade0618efcd28`  
		Last Modified: Wed, 14 Jun 2023 18:46:05 GMT  
		Size: 1.9 MB (1934899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1d2070a6fd2a146f7a7ccda5a6b5c9e7188304b3eb6ad56e85ae5e13af6efff`  
		Last Modified: Wed, 21 Jun 2023 01:22:36 GMT  
		Size: 6.5 MB (6499598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb2d53b7e662ee08ffe5d3ff1b97e2bbec271b2427e8428d38ab879c1a68cbdd`  
		Last Modified: Wed, 21 Jun 2023 01:22:31 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e13b007130a18104c8ce3a24f68b588c6ec439dcb4c22e430edf1baab337bb13`  
		Last Modified: Wed, 21 Jun 2023 01:22:31 GMT  
		Size: 118.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-bookworm` - linux; ppc64le

```console
$ docker pull memcached@sha256:0466889ea7a59c3e5075122e0dfac5f9fd4b740dbc54d7ca3355e661704b7df3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.2 MB (43193731 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f99a2d51677ef27121ea5fb73098453983811a697bb67558da1548d6a2b1a4d7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 04 Jul 2023 01:17:51 GMT
ADD file:51887002f5002ccc662adbc6ecf1129e3db375a7a77b93da43cc9a8326b3c4b9 in / 
# Tue, 04 Jul 2023 01:17:53 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 06:45:59 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 04 Jul 2023 06:46:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 06:46:11 GMT
ENV MEMCACHED_VERSION=1.6.21
# Tue, 04 Jul 2023 06:46:12 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Tue, 04 Jul 2023 06:50:32 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 04 Jul 2023 06:50:34 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 04 Jul 2023 06:50:36 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 04 Jul 2023 06:50:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Jul 2023 06:50:36 GMT
USER memcache
# Tue, 04 Jul 2023 06:50:37 GMT
EXPOSE 11211
# Tue, 04 Jul 2023 06:50:37 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:ba99a1aa5a92d949d988e66df7723a542fd81bc30eef9d4269e8a899820d4bb2`  
		Last Modified: Tue, 04 Jul 2023 01:24:36 GMT  
		Size: 33.1 MB (33116716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57bc245122d94a5d6dbd04e3f0d2cc3731cb7e5479f873ad6588885b1a1e7fff`  
		Last Modified: Tue, 04 Jul 2023 06:51:13 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8302634866fb43cf1942126242ebd186c7a31db3f01e63b626c2c6cb31aa01bb`  
		Last Modified: Tue, 04 Jul 2023 06:51:14 GMT  
		Size: 2.9 MB (2891325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85b07e92e6621b42a17464a214cee12ada2ca5c70c139194a0d9d5cdf753e470`  
		Last Modified: Tue, 04 Jul 2023 06:51:16 GMT  
		Size: 7.2 MB (7184153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:060e182005428d5f8ae46505c71da839515e43c949a2109682b933781ad7b42d`  
		Last Modified: Tue, 04 Jul 2023 06:51:13 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd71a227a79337edf4a41188a95ac6c897f53d5cc1ebfa6201b14525057ce473`  
		Last Modified: Tue, 04 Jul 2023 06:51:13 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-bookworm` - linux; s390x

```console
$ docker pull memcached@sha256:f90935a3646db47ef74efba3a8ea148e6fa9a6058557fd686664b3a9b83cf5b4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.9 MB (35907614 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:55f50234cc8836dd1977a706a4d7845c857ac2128081a776c895db012f73e5bb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 13 Jun 2023 04:29:41 GMT
ADD file:739f4c23557ec0af5f4ba492c847b5d2f09dd81211c675d0e9eabe865d794e81 in / 
# Tue, 13 Jun 2023 04:29:43 GMT
CMD ["bash"]
# Thu, 15 Jun 2023 06:23:25 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Thu, 15 Jun 2023 06:23:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 21 Jun 2023 00:54:39 GMT
ENV MEMCACHED_VERSION=1.6.21
# Wed, 21 Jun 2023 00:54:39 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Wed, 21 Jun 2023 00:57:46 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 21 Jun 2023 00:57:47 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 21 Jun 2023 00:57:47 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 21 Jun 2023 00:57:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Jun 2023 00:57:47 GMT
USER memcache
# Wed, 21 Jun 2023 00:57:47 GMT
EXPOSE 11211
# Wed, 21 Jun 2023 00:57:48 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:6571b3abd058e377c7bd231c9029aff6eb25486bffb50229076d2e6a356a517f`  
		Last Modified: Tue, 13 Jun 2023 04:34:21 GMT  
		Size: 27.5 MB (27487928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1521043364f590f749ce68598ad1f79907ef04ee2283314cfaab3f72df8e15c`  
		Last Modified: Thu, 15 Jun 2023 06:35:17 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdbc1e75c128be037526f9b133061f5dc6c9baf2f00b5d5b229427bd89eb55b7`  
		Last Modified: Thu, 15 Jun 2023 06:35:18 GMT  
		Size: 2.3 MB (2345340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f3d048c5c76c19c7c7d783cac8384f5698dd61a6aa7ee9067521407789ec9b4`  
		Last Modified: Wed, 21 Jun 2023 01:01:34 GMT  
		Size: 6.1 MB (6072815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c7bfbb7d1965d17408766d01c40f67a94eb422714618a239a48b62cedafdcab`  
		Last Modified: Wed, 21 Jun 2023 01:01:33 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:164d3c9aaa0239a91376552d50ffc16a1e2bf9e3c323e81d2a976556ab25f4a2`  
		Last Modified: Wed, 21 Jun 2023 01:01:33 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:1.6`

```console
$ docker pull memcached@sha256:1348f2e27aeea6d2b4e2b25ce9ca7679560164b0e75b6f72e221b574000158f6
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
$ docker pull memcached@sha256:37d77084cbe7c98854989a68a18f22dd677379de8ffc9ee92fbf7b88b2b4d0f9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.0 MB (38973142 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a4d0c1490511995c15a4c1ca7c8413337bed068ea95507aae882010b051ca37e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 12 Jun 2023 23:20:42 GMT
ADD file:ba1250b6ecd5dd09d4914189d72741c2817988994e7da514bf62be439a34bdb5 in / 
# Mon, 12 Jun 2023 23:20:42 GMT
CMD ["bash"]
# Wed, 14 Jun 2023 20:48:19 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 14 Jun 2023 20:48:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 21 Jun 2023 01:04:34 GMT
ENV MEMCACHED_VERSION=1.6.21
# Wed, 21 Jun 2023 01:04:35 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Wed, 21 Jun 2023 01:07:04 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 21 Jun 2023 01:07:04 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 21 Jun 2023 01:07:04 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 21 Jun 2023 01:07:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Jun 2023 01:07:05 GMT
USER memcache
# Wed, 21 Jun 2023 01:07:05 GMT
EXPOSE 11211
# Wed, 21 Jun 2023 01:07:05 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:5b5fe70539cd6989aa19f25826309f9715a9489cf1c057982d6a84c1ad8975c7`  
		Last Modified: Mon, 12 Jun 2023 23:25:49 GMT  
		Size: 29.1 MB (29124744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab209434009a85e82d99c0547bb947940f9e1002ce6e965417396ee22a6820db`  
		Last Modified: Wed, 14 Jun 2023 20:53:33 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2f4dfc49c9cdae8d4df855de7cc0460e5db8c762e73786d4f8fa4f69ba11d6d`  
		Last Modified: Wed, 14 Jun 2023 20:53:33 GMT  
		Size: 2.7 MB (2677239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d5a41694f99632bb3a7c624dab437c8a10e54b92965de823e717f5c12326b1e`  
		Last Modified: Wed, 21 Jun 2023 01:09:52 GMT  
		Size: 7.2 MB (7169627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2be3d7709e1978d4b030abdf5ac129b97f21e09bb489932628899d96288a4a9`  
		Last Modified: Wed, 21 Jun 2023 01:09:50 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8cba3f7cc400544285611f46bbdba004587f84511783fd05aa6562e9337928f`  
		Last Modified: Wed, 21 Jun 2023 01:09:50 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6` - linux; arm variant v5

```console
$ docker pull memcached@sha256:1646b01539b9482149379208acae5c0af1c5aed3aa9d818e8748410e15170943
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.1 MB (35094759 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ad4aa07800c4cf602e699a614c04d8fa80a8617828cfeb89fc05b49791d07e7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 12 Jun 2023 23:48:31 GMT
ADD file:54a716f17b23e4fa49d1d5c0a7f63becc295873c116d19bb4753d34f1ca6affb in / 
# Mon, 12 Jun 2023 23:48:31 GMT
CMD ["bash"]
# Wed, 14 Jun 2023 21:56:18 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 14 Jun 2023 21:56:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 21 Jun 2023 00:52:38 GMT
ENV MEMCACHED_VERSION=1.6.21
# Wed, 21 Jun 2023 00:52:39 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Wed, 21 Jun 2023 00:55:49 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 21 Jun 2023 00:55:49 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 21 Jun 2023 00:55:50 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 21 Jun 2023 00:55:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Jun 2023 00:55:50 GMT
USER memcache
# Wed, 21 Jun 2023 00:55:50 GMT
EXPOSE 11211
# Wed, 21 Jun 2023 00:55:50 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:70c60174b18d99741c33011138b5abf2f4d8eca0384521ccb43db3612078e36f`  
		Last Modified: Mon, 12 Jun 2023 23:51:26 GMT  
		Size: 27.0 MB (26982142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52495c3de01d54b61ec15cd608d6ce2ae4587ca764248265b02cb108f790d5a0`  
		Last Modified: Wed, 14 Jun 2023 22:00:39 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:597daa329781ff62c0581a1a2164e04dd294d665a91e97a05aa46fe3d8765eac`  
		Last Modified: Wed, 14 Jun 2023 22:00:40 GMT  
		Size: 2.3 MB (2281778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d65590b8b7bf9398f99bf1baba8d91966081bdc70d61b0165036ac0d16b3b2f`  
		Last Modified: Wed, 21 Jun 2023 00:56:10 GMT  
		Size: 5.8 MB (5829307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dfab31ab9e5a7944b95a42de61a2d1d591fa1605d1a6e2724f9b2c72f03f1ff`  
		Last Modified: Wed, 21 Jun 2023 00:56:09 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85b6795c5e090ce84e068ec9cb629871f3a70380f1bff62aa7baa8a0783343d2`  
		Last Modified: Wed, 21 Jun 2023 00:56:09 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6` - linux; arm variant v7

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

### `memcached:1.6` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:d82fec3f72f254431725dc57a8b8922cfb269e018b4407c9e7abb133083b1b32
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.9 MB (37872901 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b25fcbe4e1c3b4ce20a4e4994a494fe7a0d98500c1b5b14f4b92c104898a434c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 04 Jul 2023 01:57:35 GMT
ADD file:71fd66666294148382f2e6a09ae5e277d4c4e9c74402ab64b693a79387b67a09 in / 
# Tue, 04 Jul 2023 01:57:36 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 06:40:00 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 04 Jul 2023 06:40:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 06:40:03 GMT
ENV MEMCACHED_VERSION=1.6.21
# Tue, 04 Jul 2023 06:40:03 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Tue, 04 Jul 2023 06:42:47 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 04 Jul 2023 06:42:47 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 04 Jul 2023 06:42:48 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 04 Jul 2023 06:42:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Jul 2023 06:42:48 GMT
USER memcache
# Tue, 04 Jul 2023 06:42:48 GMT
EXPOSE 11211
# Tue, 04 Jul 2023 06:42:48 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:3ae0c06b4d3aa97d7e0829233dd36cea1666b87074e55fea6bd1ecae066693c7`  
		Last Modified: Tue, 04 Jul 2023 02:01:20 GMT  
		Size: 29.2 MB (29152458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7e0b4333d4768ee800aa733f63a51c54833abe7bd20188154f0869796bb3f8c`  
		Last Modified: Tue, 04 Jul 2023 06:43:03 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fd0e2a70b071a1504381d7831ed736d40261b75692a2fe4ee547186e80ad9b2`  
		Last Modified: Tue, 04 Jul 2023 06:43:03 GMT  
		Size: 2.5 MB (2539167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:382aa3014b4367d16a225a23e5195af1f3a5e51523f9d89461e4b98ddf61aa3d`  
		Last Modified: Tue, 04 Jul 2023 06:43:04 GMT  
		Size: 6.2 MB (6179743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4abaeb5f633e1c888b605fe890a58e527c62021db2516cd8606edad49e9500c0`  
		Last Modified: Tue, 04 Jul 2023 06:43:03 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aedc2da2773982e3f9627ea96874aec7c38a4288cca37a366f29392750f7c38`  
		Last Modified: Tue, 04 Jul 2023 06:43:03 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6` - linux; 386

```console
$ docker pull memcached@sha256:d275ff7e4cd6b5d699c14115419af7ae2c1bfa32312282ff8c9ba0b424cf6be0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.5 MB (39457503 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8785d2e661831af23d884d73d3196f416198d2c57ffa24c50c8cafe16c0da224`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 12 Jun 2023 23:39:20 GMT
ADD file:c7ecc5e2bed99e2cbca26f9f4247cd9bc399749556f4084e9357a9b00bb80530 in / 
# Mon, 12 Jun 2023 23:39:20 GMT
CMD ["bash"]
# Wed, 14 Jun 2023 22:34:28 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 14 Jun 2023 22:34:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 21 Jun 2023 00:46:59 GMT
ENV MEMCACHED_VERSION=1.6.21
# Wed, 21 Jun 2023 00:46:59 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Wed, 21 Jun 2023 00:50:45 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 21 Jun 2023 00:50:45 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 21 Jun 2023 00:50:46 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 21 Jun 2023 00:50:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Jun 2023 00:50:46 GMT
USER memcache
# Wed, 21 Jun 2023 00:50:46 GMT
EXPOSE 11211
# Wed, 21 Jun 2023 00:50:46 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:82a41d17956dd7c8ebb39c9ce936fd26841bdbec98d0a185e3db8154b352edff`  
		Last Modified: Mon, 12 Jun 2023 23:46:21 GMT  
		Size: 30.1 MB (30140741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:039125a8cebc58c43be503e98831cac166a973cb3e68f4b66194142680e76964`  
		Last Modified: Wed, 14 Jun 2023 22:42:09 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:199b04439aa2a5065d0c23f986eccd0dd093be2f49b180b332af4f35d977ab5b`  
		Last Modified: Wed, 14 Jun 2023 22:42:09 GMT  
		Size: 2.7 MB (2685017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e58126d70102e38c764aa423066a897bc811895dc85b8d607eadfcff947049a7`  
		Last Modified: Wed, 21 Jun 2023 00:54:46 GMT  
		Size: 6.6 MB (6630215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b039c50c059c1c3a231a9659c8ade08b537d8ecac9423685ba16cf308626c4e4`  
		Last Modified: Wed, 21 Jun 2023 00:54:44 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1d3e144a63d04f26029dacd020e1ec00baeae59c5cee460a482e70842be2fc2`  
		Last Modified: Wed, 21 Jun 2023 00:54:44 GMT  
		Size: 116.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6` - linux; mips64le

```console
$ docker pull memcached@sha256:76620bca6f37fb4a82e0cc3aa33ba7cc2508c8f93dd4ae4956e9b471ce0995a2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.6 MB (37554107 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f8424fcd7f4d7db2c883a9303136b4305e34813630a9e325332ee830d35c026d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 13 Jun 2023 00:09:02 GMT
ADD file:f91bd2a174259cb69646fc34ba2fc6b8941ad8e171d2d7952a4d8ac3d95e2ad7 in / 
# Tue, 13 Jun 2023 00:09:06 GMT
CMD ["bash"]
# Wed, 14 Jun 2023 18:38:15 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 14 Jun 2023 18:38:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 21 Jun 2023 01:14:52 GMT
ENV MEMCACHED_VERSION=1.6.21
# Wed, 21 Jun 2023 01:14:54 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Wed, 21 Jun 2023 01:21:45 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 21 Jun 2023 01:21:47 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 21 Jun 2023 01:21:52 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 21 Jun 2023 01:21:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Jun 2023 01:21:57 GMT
USER memcache
# Wed, 21 Jun 2023 01:22:00 GMT
EXPOSE 11211
# Wed, 21 Jun 2023 01:22:02 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:3fc28260a4d871ef9781cad2bb064ad7212a5063de3a1d35dba938ce82115e5b`  
		Last Modified: Tue, 13 Jun 2023 00:22:29 GMT  
		Size: 29.1 MB (29118129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79c804aeb794275ae845d32d2939d0e0fefa75cd112f1075aaf2104097050ae8`  
		Last Modified: Wed, 14 Jun 2023 18:46:04 GMT  
		Size: 1.1 KB (1078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf29fcbe26928e2f4086a889098220505bdd4401dc87958f623ade0618efcd28`  
		Last Modified: Wed, 14 Jun 2023 18:46:05 GMT  
		Size: 1.9 MB (1934899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1d2070a6fd2a146f7a7ccda5a6b5c9e7188304b3eb6ad56e85ae5e13af6efff`  
		Last Modified: Wed, 21 Jun 2023 01:22:36 GMT  
		Size: 6.5 MB (6499598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb2d53b7e662ee08ffe5d3ff1b97e2bbec271b2427e8428d38ab879c1a68cbdd`  
		Last Modified: Wed, 21 Jun 2023 01:22:31 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e13b007130a18104c8ce3a24f68b588c6ec439dcb4c22e430edf1baab337bb13`  
		Last Modified: Wed, 21 Jun 2023 01:22:31 GMT  
		Size: 118.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6` - linux; ppc64le

```console
$ docker pull memcached@sha256:0466889ea7a59c3e5075122e0dfac5f9fd4b740dbc54d7ca3355e661704b7df3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.2 MB (43193731 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f99a2d51677ef27121ea5fb73098453983811a697bb67558da1548d6a2b1a4d7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 04 Jul 2023 01:17:51 GMT
ADD file:51887002f5002ccc662adbc6ecf1129e3db375a7a77b93da43cc9a8326b3c4b9 in / 
# Tue, 04 Jul 2023 01:17:53 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 06:45:59 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 04 Jul 2023 06:46:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 06:46:11 GMT
ENV MEMCACHED_VERSION=1.6.21
# Tue, 04 Jul 2023 06:46:12 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Tue, 04 Jul 2023 06:50:32 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 04 Jul 2023 06:50:34 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 04 Jul 2023 06:50:36 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 04 Jul 2023 06:50:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Jul 2023 06:50:36 GMT
USER memcache
# Tue, 04 Jul 2023 06:50:37 GMT
EXPOSE 11211
# Tue, 04 Jul 2023 06:50:37 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:ba99a1aa5a92d949d988e66df7723a542fd81bc30eef9d4269e8a899820d4bb2`  
		Last Modified: Tue, 04 Jul 2023 01:24:36 GMT  
		Size: 33.1 MB (33116716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57bc245122d94a5d6dbd04e3f0d2cc3731cb7e5479f873ad6588885b1a1e7fff`  
		Last Modified: Tue, 04 Jul 2023 06:51:13 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8302634866fb43cf1942126242ebd186c7a31db3f01e63b626c2c6cb31aa01bb`  
		Last Modified: Tue, 04 Jul 2023 06:51:14 GMT  
		Size: 2.9 MB (2891325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85b07e92e6621b42a17464a214cee12ada2ca5c70c139194a0d9d5cdf753e470`  
		Last Modified: Tue, 04 Jul 2023 06:51:16 GMT  
		Size: 7.2 MB (7184153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:060e182005428d5f8ae46505c71da839515e43c949a2109682b933781ad7b42d`  
		Last Modified: Tue, 04 Jul 2023 06:51:13 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd71a227a79337edf4a41188a95ac6c897f53d5cc1ebfa6201b14525057ce473`  
		Last Modified: Tue, 04 Jul 2023 06:51:13 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6` - linux; s390x

```console
$ docker pull memcached@sha256:f90935a3646db47ef74efba3a8ea148e6fa9a6058557fd686664b3a9b83cf5b4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.9 MB (35907614 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:55f50234cc8836dd1977a706a4d7845c857ac2128081a776c895db012f73e5bb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 13 Jun 2023 04:29:41 GMT
ADD file:739f4c23557ec0af5f4ba492c847b5d2f09dd81211c675d0e9eabe865d794e81 in / 
# Tue, 13 Jun 2023 04:29:43 GMT
CMD ["bash"]
# Thu, 15 Jun 2023 06:23:25 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Thu, 15 Jun 2023 06:23:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 21 Jun 2023 00:54:39 GMT
ENV MEMCACHED_VERSION=1.6.21
# Wed, 21 Jun 2023 00:54:39 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Wed, 21 Jun 2023 00:57:46 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 21 Jun 2023 00:57:47 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 21 Jun 2023 00:57:47 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 21 Jun 2023 00:57:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Jun 2023 00:57:47 GMT
USER memcache
# Wed, 21 Jun 2023 00:57:47 GMT
EXPOSE 11211
# Wed, 21 Jun 2023 00:57:48 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:6571b3abd058e377c7bd231c9029aff6eb25486bffb50229076d2e6a356a517f`  
		Last Modified: Tue, 13 Jun 2023 04:34:21 GMT  
		Size: 27.5 MB (27487928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1521043364f590f749ce68598ad1f79907ef04ee2283314cfaab3f72df8e15c`  
		Last Modified: Thu, 15 Jun 2023 06:35:17 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdbc1e75c128be037526f9b133061f5dc6c9baf2f00b5d5b229427bd89eb55b7`  
		Last Modified: Thu, 15 Jun 2023 06:35:18 GMT  
		Size: 2.3 MB (2345340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f3d048c5c76c19c7c7d783cac8384f5698dd61a6aa7ee9067521407789ec9b4`  
		Last Modified: Wed, 21 Jun 2023 01:01:34 GMT  
		Size: 6.1 MB (6072815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c7bfbb7d1965d17408766d01c40f67a94eb422714618a239a48b62cedafdcab`  
		Last Modified: Wed, 21 Jun 2023 01:01:33 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:164d3c9aaa0239a91376552d50ffc16a1e2bf9e3c323e81d2a976556ab25f4a2`  
		Last Modified: Wed, 21 Jun 2023 01:01:33 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:1.6-alpine`

```console
$ docker pull memcached@sha256:32f2ba37c2ed2ef922efa0190faa71dc3b4f1df4a3e50938a0b3afe3d589a1d9
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
$ docker pull memcached@sha256:574ef430513a38925cc52ae5954677a12e0a57205fed96be5707196a180e5159
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4462428 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f7da63106561ab1f7284992dad2396b234096070b4269971b23c53f2f8498ef`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 14 Jun 2023 20:41:58 GMT
ADD file:1da756d12551a0e3e793e02ef87432d69d4968937bd11bed0af215db19dd94cd in / 
# Wed, 14 Jun 2023 20:41:59 GMT
CMD ["/bin/sh"]
# Wed, 14 Jun 2023 20:50:58 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Wed, 14 Jun 2023 20:50:59 GMT
RUN apk add --no-cache libsasl
# Wed, 21 Jun 2023 01:07:13 GMT
ENV MEMCACHED_VERSION=1.6.21
# Wed, 21 Jun 2023 01:07:13 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Wed, 21 Jun 2023 01:09:21 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Wed, 21 Jun 2023 01:09:21 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 21 Jun 2023 01:09:22 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 21 Jun 2023 01:09:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Jun 2023 01:09:22 GMT
USER memcache
# Wed, 21 Jun 2023 01:09:22 GMT
EXPOSE 11211
# Wed, 21 Jun 2023 01:09:22 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:31e352740f534f9ad170f75378a84fe453d6156e40700b882d737a8f4a6988a3`  
		Last Modified: Wed, 14 Jun 2023 20:42:26 GMT  
		Size: 3.4 MB (3397879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b2b2df106c5026cd33ea4ac655b77f25410ec9f4b8a6756ebc1ceeb79fca3c7`  
		Last Modified: Wed, 14 Jun 2023 20:53:58 GMT  
		Size: 1.3 KB (1266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed63668528d3e2159f55909c66dc48a6f746ce24c2e2f6d963b992aefaa457ce`  
		Last Modified: Wed, 14 Jun 2023 20:53:58 GMT  
		Size: 108.1 KB (108080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05536f2f26c904a5aa1b07720957a37e8b57a223725d76f8d1473dcab297a233`  
		Last Modified: Wed, 21 Jun 2023 01:10:14 GMT  
		Size: 954.8 KB (954811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e448b573a98adc8bd0a4805cb0e1b451aea0d1582f0462aa0b147799a97fad7`  
		Last Modified: Wed, 21 Jun 2023 01:10:13 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3029a709b7be20aeff1e9cebe5c6112cd1df5a0ea3efb58e61380cc75b9296e`  
		Last Modified: Wed, 21 Jun 2023 01:10:13 GMT  
		Size: 117.0 B  
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
$ docker pull memcached@sha256:eb4b801b9c9e9af6565ac003b21af39b06d55943bbc4e59a02d465fdf7f07776
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.4 MB (4399342 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4aa99dd98a2fa001241d907951530f4afebadfd4895545c5d73f31e29b7a35fa`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 14 Jun 2023 20:48:58 GMT
ADD file:289c2fac17119508ced527225d445747cd177111b4a0018a6b04948ecb3b5e29 in / 
# Wed, 14 Jun 2023 20:48:58 GMT
CMD ["/bin/sh"]
# Wed, 14 Jun 2023 20:57:26 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Wed, 14 Jun 2023 20:57:27 GMT
RUN apk add --no-cache libsasl
# Wed, 21 Jun 2023 01:08:09 GMT
ENV MEMCACHED_VERSION=1.6.21
# Wed, 21 Jun 2023 01:08:09 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Wed, 21 Jun 2023 01:10:35 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Wed, 21 Jun 2023 01:10:35 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 21 Jun 2023 01:10:36 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 21 Jun 2023 01:10:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Jun 2023 01:10:36 GMT
USER memcache
# Wed, 21 Jun 2023 01:10:36 GMT
EXPOSE 11211
# Wed, 21 Jun 2023 01:10:36 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:8c6d1654570f041603f4cef49c320c8f6f3e401324913009d92a19132cbf1ac0`  
		Last Modified: Wed, 14 Jun 2023 20:49:23 GMT  
		Size: 3.3 MB (3329251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:666588188768f19b27fb821e02d084406af8fd867cc4595b896b9eed50b2105e`  
		Last Modified: Wed, 14 Jun 2023 21:00:51 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7d958a137d671266f063c0af4d7b0b6d44d9018b77fdbddb8fd412d3c0b1be3`  
		Last Modified: Wed, 14 Jun 2023 21:00:51 GMT  
		Size: 124.1 KB (124137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a66841dcfe05dcef1af82648941fa1ea0e10dbdf022326916d1d74afc99885c6`  
		Last Modified: Wed, 21 Jun 2023 01:11:21 GMT  
		Size: 944.3 KB (944292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b46fdc76bcbc8fa94ae23177ac32b97a4d370a630ec7d3f52bd8aae174e75982`  
		Last Modified: Wed, 21 Jun 2023 01:11:20 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea70db1a59f508c629aef54fb39ac3ada5cfcc3aac7aa1d6ed6cde22e97d3e3b`  
		Last Modified: Wed, 21 Jun 2023 01:11:20 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-alpine` - linux; 386

```console
$ docker pull memcached@sha256:73c987449b9f764e060e2745d29e0ee50f4f7e630ddd23631c517e65f2315bfa
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.3 MB (4282253 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c47771f0d8f2ab5f38441f65fed7a05d87ea44b1de1a502321348997971362c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 14 Jun 2023 22:33:22 GMT
ADD file:94bec00e2c0c7f47c81ec4355a29ca23a81b439797d037b1a5a455f36a25dab4 in / 
# Wed, 14 Jun 2023 22:33:22 GMT
CMD ["/bin/sh"]
# Wed, 14 Jun 2023 22:38:20 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Wed, 14 Jun 2023 22:38:22 GMT
RUN apk add --no-cache libsasl
# Wed, 21 Jun 2023 00:50:52 GMT
ENV MEMCACHED_VERSION=1.6.21
# Wed, 21 Jun 2023 00:50:52 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Wed, 21 Jun 2023 00:54:21 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Wed, 21 Jun 2023 00:54:22 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 21 Jun 2023 00:54:22 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 21 Jun 2023 00:54:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Jun 2023 00:54:22 GMT
USER memcache
# Wed, 21 Jun 2023 00:54:22 GMT
EXPOSE 11211
# Wed, 21 Jun 2023 00:54:23 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:b3f50075abd13aad1cb7d8c1427aa59d7fcac88f3690d3f9c3efdbec80fd0856`  
		Last Modified: Wed, 14 Jun 2023 22:33:48 GMT  
		Size: 3.2 MB (3233951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:358673fc695429dd9142a4904a518e96c418229121d02435d875a993d9e5fac1`  
		Last Modified: Wed, 14 Jun 2023 22:42:32 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ae09e638ab1208326cbfd03f4517b0d1d13f72cfc8add3a055321fe5cf0f53a`  
		Last Modified: Wed, 14 Jun 2023 22:42:32 GMT  
		Size: 109.5 KB (109531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ed35577a5a4360f65bc0361d7bca857e45fad4baf04bcde5e731529377e9f58`  
		Last Modified: Wed, 21 Jun 2023 00:55:07 GMT  
		Size: 937.1 KB (937107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c4024dd0449592764b513374729cea0a478f62deaf32af4b23e536ffca016b6`  
		Last Modified: Wed, 21 Jun 2023 00:55:07 GMT  
		Size: 280.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6d29f640e8837bc0d0ed4b3fc505f71494f0c3ef917245b2399971ca3cb38e8`  
		Last Modified: Wed, 21 Jun 2023 00:55:06 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-alpine` - linux; ppc64le

```console
$ docker pull memcached@sha256:e02abd3f1c109243a103019450a45039503d018c8fcd2fb607798643fbeaed69
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4453245 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7311794e1380b44e42daf3ea3c49269eb71549d5f62a46f6596478d01bda3b02`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 15 Jun 2023 00:39:49 GMT
ADD file:694c636c0dd19fd01accbc189e4c1dc4d063952692c6e7eb26dce02a7adba833 in / 
# Thu, 15 Jun 2023 00:39:49 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 04:20:00 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Thu, 15 Jun 2023 04:20:03 GMT
RUN apk add --no-cache libsasl
# Wed, 21 Jun 2023 01:42:40 GMT
ENV MEMCACHED_VERSION=1.6.21
# Wed, 21 Jun 2023 01:42:40 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Wed, 21 Jun 2023 01:45:42 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Wed, 21 Jun 2023 01:45:43 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 21 Jun 2023 01:45:45 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 21 Jun 2023 01:45:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Jun 2023 01:45:46 GMT
USER memcache
# Wed, 21 Jun 2023 01:45:46 GMT
EXPOSE 11211
# Wed, 21 Jun 2023 01:45:47 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:ffa4a466dbb8eebd7e7f25590a9df12390de9016abf82279c29c9a64aa76491a`  
		Last Modified: Thu, 15 Jun 2023 00:40:26 GMT  
		Size: 3.3 MB (3344781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:607cb6edfb2d0718375d44dbfb94d80d9b5e23a38a6bad8d2fe9c624a0ae354a`  
		Last Modified: Thu, 15 Jun 2023 04:23:36 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f97572f9bc2bc81fb5496a46ecd8b44cdb5b616d0beaecaabb186e3523683a32`  
		Last Modified: Thu, 15 Jun 2023 04:23:37 GMT  
		Size: 123.9 KB (123931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da5b2f6c7aee3051aa1b53ff9a66885509bad54b27aa37aebe382fc1ca4eab1f`  
		Last Modified: Wed, 21 Jun 2023 01:46:43 GMT  
		Size: 982.9 KB (982864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a08963a0c7d8349568389e6f7af0c7a1b55f2b0aea5d25bfa94d415fbb94af9`  
		Last Modified: Wed, 21 Jun 2023 01:46:43 GMT  
		Size: 282.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d866cc948bf60127d37a1f655a84d6b9c17376a21656e660c47efc6d3f499ba2`  
		Last Modified: Wed, 21 Jun 2023 01:46:43 GMT  
		Size: 118.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-alpine` - linux; s390x

```console
$ docker pull memcached@sha256:cd97d93e79c2345a0c10f20a912f29a0ccf5590e15c00df81596397b9567233f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.3 MB (4278263 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f56d14fce8cfd200c86bd00cd28c95574b6bf2863bd203e7644d44a08db84ab`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 15 Jun 2023 05:18:38 GMT
ADD file:a59beca78118ebf4f86cc1685237dc3a29a519401a70668da520beaa3d29eb7a in / 
# Thu, 15 Jun 2023 05:18:38 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 06:27:47 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Thu, 15 Jun 2023 06:27:49 GMT
RUN apk add --no-cache libsasl
# Wed, 21 Jun 2023 00:58:01 GMT
ENV MEMCACHED_VERSION=1.6.21
# Wed, 21 Jun 2023 00:58:01 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Wed, 21 Jun 2023 01:01:08 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Wed, 21 Jun 2023 01:01:09 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 21 Jun 2023 01:01:09 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 21 Jun 2023 01:01:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Jun 2023 01:01:09 GMT
USER memcache
# Wed, 21 Jun 2023 01:01:10 GMT
EXPOSE 11211
# Wed, 21 Jun 2023 01:01:10 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:998cc98447b44e5f0fe799dce691412796ba586ab22eb7c99aebf9d45f34833b`  
		Last Modified: Thu, 15 Jun 2023 05:29:38 GMT  
		Size: 3.2 MB (3213497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:156deb87465a2c5629e5ae28c2a7251d5684baea5a930cf65ff6b478de321202`  
		Last Modified: Thu, 15 Jun 2023 06:36:33 GMT  
		Size: 1.3 KB (1266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19020c60d58f4724218660e819b1b33b5d1428c3c5027492a2ee3c44228231df`  
		Last Modified: Thu, 15 Jun 2023 06:36:33 GMT  
		Size: 112.8 KB (112849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81e76f938f015ccb0b5d2915145432efbc0af21a2f4964e0c9a67bfbbe6a577e`  
		Last Modified: Wed, 21 Jun 2023 01:01:46 GMT  
		Size: 950.3 KB (950254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b613e0a69ced3425a5949c15688d493ef10d80eb28c7bb626f0c092223fe1302`  
		Last Modified: Wed, 21 Jun 2023 01:01:46 GMT  
		Size: 280.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4db4c30d38bb65cd11068e1892913b2fa04add8f27abe601485cc3b09754eb50`  
		Last Modified: Wed, 21 Jun 2023 01:01:46 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:1.6-alpine3.18`

```console
$ docker pull memcached@sha256:ee437fd9a952b48de768cd5c7a97d43439e05b918e4bc4452e296e8bdafae046
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `memcached:1.6-alpine3.18` - linux; amd64

```console
$ docker pull memcached@sha256:574ef430513a38925cc52ae5954677a12e0a57205fed96be5707196a180e5159
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4462428 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f7da63106561ab1f7284992dad2396b234096070b4269971b23c53f2f8498ef`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 14 Jun 2023 20:41:58 GMT
ADD file:1da756d12551a0e3e793e02ef87432d69d4968937bd11bed0af215db19dd94cd in / 
# Wed, 14 Jun 2023 20:41:59 GMT
CMD ["/bin/sh"]
# Wed, 14 Jun 2023 20:50:58 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Wed, 14 Jun 2023 20:50:59 GMT
RUN apk add --no-cache libsasl
# Wed, 21 Jun 2023 01:07:13 GMT
ENV MEMCACHED_VERSION=1.6.21
# Wed, 21 Jun 2023 01:07:13 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Wed, 21 Jun 2023 01:09:21 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Wed, 21 Jun 2023 01:09:21 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 21 Jun 2023 01:09:22 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 21 Jun 2023 01:09:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Jun 2023 01:09:22 GMT
USER memcache
# Wed, 21 Jun 2023 01:09:22 GMT
EXPOSE 11211
# Wed, 21 Jun 2023 01:09:22 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:31e352740f534f9ad170f75378a84fe453d6156e40700b882d737a8f4a6988a3`  
		Last Modified: Wed, 14 Jun 2023 20:42:26 GMT  
		Size: 3.4 MB (3397879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b2b2df106c5026cd33ea4ac655b77f25410ec9f4b8a6756ebc1ceeb79fca3c7`  
		Last Modified: Wed, 14 Jun 2023 20:53:58 GMT  
		Size: 1.3 KB (1266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed63668528d3e2159f55909c66dc48a6f746ce24c2e2f6d963b992aefaa457ce`  
		Last Modified: Wed, 14 Jun 2023 20:53:58 GMT  
		Size: 108.1 KB (108080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05536f2f26c904a5aa1b07720957a37e8b57a223725d76f8d1473dcab297a233`  
		Last Modified: Wed, 21 Jun 2023 01:10:14 GMT  
		Size: 954.8 KB (954811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e448b573a98adc8bd0a4805cb0e1b451aea0d1582f0462aa0b147799a97fad7`  
		Last Modified: Wed, 21 Jun 2023 01:10:13 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3029a709b7be20aeff1e9cebe5c6112cd1df5a0ea3efb58e61380cc75b9296e`  
		Last Modified: Wed, 21 Jun 2023 01:10:13 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-alpine3.18` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:eb4b801b9c9e9af6565ac003b21af39b06d55943bbc4e59a02d465fdf7f07776
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.4 MB (4399342 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4aa99dd98a2fa001241d907951530f4afebadfd4895545c5d73f31e29b7a35fa`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 14 Jun 2023 20:48:58 GMT
ADD file:289c2fac17119508ced527225d445747cd177111b4a0018a6b04948ecb3b5e29 in / 
# Wed, 14 Jun 2023 20:48:58 GMT
CMD ["/bin/sh"]
# Wed, 14 Jun 2023 20:57:26 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Wed, 14 Jun 2023 20:57:27 GMT
RUN apk add --no-cache libsasl
# Wed, 21 Jun 2023 01:08:09 GMT
ENV MEMCACHED_VERSION=1.6.21
# Wed, 21 Jun 2023 01:08:09 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Wed, 21 Jun 2023 01:10:35 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Wed, 21 Jun 2023 01:10:35 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 21 Jun 2023 01:10:36 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 21 Jun 2023 01:10:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Jun 2023 01:10:36 GMT
USER memcache
# Wed, 21 Jun 2023 01:10:36 GMT
EXPOSE 11211
# Wed, 21 Jun 2023 01:10:36 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:8c6d1654570f041603f4cef49c320c8f6f3e401324913009d92a19132cbf1ac0`  
		Last Modified: Wed, 14 Jun 2023 20:49:23 GMT  
		Size: 3.3 MB (3329251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:666588188768f19b27fb821e02d084406af8fd867cc4595b896b9eed50b2105e`  
		Last Modified: Wed, 14 Jun 2023 21:00:51 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7d958a137d671266f063c0af4d7b0b6d44d9018b77fdbddb8fd412d3c0b1be3`  
		Last Modified: Wed, 14 Jun 2023 21:00:51 GMT  
		Size: 124.1 KB (124137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a66841dcfe05dcef1af82648941fa1ea0e10dbdf022326916d1d74afc99885c6`  
		Last Modified: Wed, 21 Jun 2023 01:11:21 GMT  
		Size: 944.3 KB (944292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b46fdc76bcbc8fa94ae23177ac32b97a4d370a630ec7d3f52bd8aae174e75982`  
		Last Modified: Wed, 21 Jun 2023 01:11:20 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea70db1a59f508c629aef54fb39ac3ada5cfcc3aac7aa1d6ed6cde22e97d3e3b`  
		Last Modified: Wed, 21 Jun 2023 01:11:20 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-alpine3.18` - linux; 386

```console
$ docker pull memcached@sha256:73c987449b9f764e060e2745d29e0ee50f4f7e630ddd23631c517e65f2315bfa
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.3 MB (4282253 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c47771f0d8f2ab5f38441f65fed7a05d87ea44b1de1a502321348997971362c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 14 Jun 2023 22:33:22 GMT
ADD file:94bec00e2c0c7f47c81ec4355a29ca23a81b439797d037b1a5a455f36a25dab4 in / 
# Wed, 14 Jun 2023 22:33:22 GMT
CMD ["/bin/sh"]
# Wed, 14 Jun 2023 22:38:20 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Wed, 14 Jun 2023 22:38:22 GMT
RUN apk add --no-cache libsasl
# Wed, 21 Jun 2023 00:50:52 GMT
ENV MEMCACHED_VERSION=1.6.21
# Wed, 21 Jun 2023 00:50:52 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Wed, 21 Jun 2023 00:54:21 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Wed, 21 Jun 2023 00:54:22 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 21 Jun 2023 00:54:22 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 21 Jun 2023 00:54:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Jun 2023 00:54:22 GMT
USER memcache
# Wed, 21 Jun 2023 00:54:22 GMT
EXPOSE 11211
# Wed, 21 Jun 2023 00:54:23 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:b3f50075abd13aad1cb7d8c1427aa59d7fcac88f3690d3f9c3efdbec80fd0856`  
		Last Modified: Wed, 14 Jun 2023 22:33:48 GMT  
		Size: 3.2 MB (3233951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:358673fc695429dd9142a4904a518e96c418229121d02435d875a993d9e5fac1`  
		Last Modified: Wed, 14 Jun 2023 22:42:32 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ae09e638ab1208326cbfd03f4517b0d1d13f72cfc8add3a055321fe5cf0f53a`  
		Last Modified: Wed, 14 Jun 2023 22:42:32 GMT  
		Size: 109.5 KB (109531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ed35577a5a4360f65bc0361d7bca857e45fad4baf04bcde5e731529377e9f58`  
		Last Modified: Wed, 21 Jun 2023 00:55:07 GMT  
		Size: 937.1 KB (937107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c4024dd0449592764b513374729cea0a478f62deaf32af4b23e536ffca016b6`  
		Last Modified: Wed, 21 Jun 2023 00:55:07 GMT  
		Size: 280.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6d29f640e8837bc0d0ed4b3fc505f71494f0c3ef917245b2399971ca3cb38e8`  
		Last Modified: Wed, 21 Jun 2023 00:55:06 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-alpine3.18` - linux; ppc64le

```console
$ docker pull memcached@sha256:e02abd3f1c109243a103019450a45039503d018c8fcd2fb607798643fbeaed69
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4453245 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7311794e1380b44e42daf3ea3c49269eb71549d5f62a46f6596478d01bda3b02`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 15 Jun 2023 00:39:49 GMT
ADD file:694c636c0dd19fd01accbc189e4c1dc4d063952692c6e7eb26dce02a7adba833 in / 
# Thu, 15 Jun 2023 00:39:49 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 04:20:00 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Thu, 15 Jun 2023 04:20:03 GMT
RUN apk add --no-cache libsasl
# Wed, 21 Jun 2023 01:42:40 GMT
ENV MEMCACHED_VERSION=1.6.21
# Wed, 21 Jun 2023 01:42:40 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Wed, 21 Jun 2023 01:45:42 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Wed, 21 Jun 2023 01:45:43 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 21 Jun 2023 01:45:45 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 21 Jun 2023 01:45:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Jun 2023 01:45:46 GMT
USER memcache
# Wed, 21 Jun 2023 01:45:46 GMT
EXPOSE 11211
# Wed, 21 Jun 2023 01:45:47 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:ffa4a466dbb8eebd7e7f25590a9df12390de9016abf82279c29c9a64aa76491a`  
		Last Modified: Thu, 15 Jun 2023 00:40:26 GMT  
		Size: 3.3 MB (3344781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:607cb6edfb2d0718375d44dbfb94d80d9b5e23a38a6bad8d2fe9c624a0ae354a`  
		Last Modified: Thu, 15 Jun 2023 04:23:36 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f97572f9bc2bc81fb5496a46ecd8b44cdb5b616d0beaecaabb186e3523683a32`  
		Last Modified: Thu, 15 Jun 2023 04:23:37 GMT  
		Size: 123.9 KB (123931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da5b2f6c7aee3051aa1b53ff9a66885509bad54b27aa37aebe382fc1ca4eab1f`  
		Last Modified: Wed, 21 Jun 2023 01:46:43 GMT  
		Size: 982.9 KB (982864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a08963a0c7d8349568389e6f7af0c7a1b55f2b0aea5d25bfa94d415fbb94af9`  
		Last Modified: Wed, 21 Jun 2023 01:46:43 GMT  
		Size: 282.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d866cc948bf60127d37a1f655a84d6b9c17376a21656e660c47efc6d3f499ba2`  
		Last Modified: Wed, 21 Jun 2023 01:46:43 GMT  
		Size: 118.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-alpine3.18` - linux; s390x

```console
$ docker pull memcached@sha256:cd97d93e79c2345a0c10f20a912f29a0ccf5590e15c00df81596397b9567233f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.3 MB (4278263 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f56d14fce8cfd200c86bd00cd28c95574b6bf2863bd203e7644d44a08db84ab`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 15 Jun 2023 05:18:38 GMT
ADD file:a59beca78118ebf4f86cc1685237dc3a29a519401a70668da520beaa3d29eb7a in / 
# Thu, 15 Jun 2023 05:18:38 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 06:27:47 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Thu, 15 Jun 2023 06:27:49 GMT
RUN apk add --no-cache libsasl
# Wed, 21 Jun 2023 00:58:01 GMT
ENV MEMCACHED_VERSION=1.6.21
# Wed, 21 Jun 2023 00:58:01 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Wed, 21 Jun 2023 01:01:08 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Wed, 21 Jun 2023 01:01:09 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 21 Jun 2023 01:01:09 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 21 Jun 2023 01:01:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Jun 2023 01:01:09 GMT
USER memcache
# Wed, 21 Jun 2023 01:01:10 GMT
EXPOSE 11211
# Wed, 21 Jun 2023 01:01:10 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:998cc98447b44e5f0fe799dce691412796ba586ab22eb7c99aebf9d45f34833b`  
		Last Modified: Thu, 15 Jun 2023 05:29:38 GMT  
		Size: 3.2 MB (3213497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:156deb87465a2c5629e5ae28c2a7251d5684baea5a930cf65ff6b478de321202`  
		Last Modified: Thu, 15 Jun 2023 06:36:33 GMT  
		Size: 1.3 KB (1266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19020c60d58f4724218660e819b1b33b5d1428c3c5027492a2ee3c44228231df`  
		Last Modified: Thu, 15 Jun 2023 06:36:33 GMT  
		Size: 112.8 KB (112849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81e76f938f015ccb0b5d2915145432efbc0af21a2f4964e0c9a67bfbbe6a577e`  
		Last Modified: Wed, 21 Jun 2023 01:01:46 GMT  
		Size: 950.3 KB (950254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b613e0a69ced3425a5949c15688d493ef10d80eb28c7bb626f0c092223fe1302`  
		Last Modified: Wed, 21 Jun 2023 01:01:46 GMT  
		Size: 280.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4db4c30d38bb65cd11068e1892913b2fa04add8f27abe601485cc3b09754eb50`  
		Last Modified: Wed, 21 Jun 2023 01:01:46 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:1.6-bookworm`

```console
$ docker pull memcached@sha256:6d50bee6d0eaba83831fead39d52d67ede2aefc3acf69a19d503a9488234e1c8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 7
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; s390x

### `memcached:1.6-bookworm` - linux; amd64

```console
$ docker pull memcached@sha256:37d77084cbe7c98854989a68a18f22dd677379de8ffc9ee92fbf7b88b2b4d0f9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.0 MB (38973142 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a4d0c1490511995c15a4c1ca7c8413337bed068ea95507aae882010b051ca37e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 12 Jun 2023 23:20:42 GMT
ADD file:ba1250b6ecd5dd09d4914189d72741c2817988994e7da514bf62be439a34bdb5 in / 
# Mon, 12 Jun 2023 23:20:42 GMT
CMD ["bash"]
# Wed, 14 Jun 2023 20:48:19 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 14 Jun 2023 20:48:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 21 Jun 2023 01:04:34 GMT
ENV MEMCACHED_VERSION=1.6.21
# Wed, 21 Jun 2023 01:04:35 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Wed, 21 Jun 2023 01:07:04 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 21 Jun 2023 01:07:04 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 21 Jun 2023 01:07:04 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 21 Jun 2023 01:07:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Jun 2023 01:07:05 GMT
USER memcache
# Wed, 21 Jun 2023 01:07:05 GMT
EXPOSE 11211
# Wed, 21 Jun 2023 01:07:05 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:5b5fe70539cd6989aa19f25826309f9715a9489cf1c057982d6a84c1ad8975c7`  
		Last Modified: Mon, 12 Jun 2023 23:25:49 GMT  
		Size: 29.1 MB (29124744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab209434009a85e82d99c0547bb947940f9e1002ce6e965417396ee22a6820db`  
		Last Modified: Wed, 14 Jun 2023 20:53:33 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2f4dfc49c9cdae8d4df855de7cc0460e5db8c762e73786d4f8fa4f69ba11d6d`  
		Last Modified: Wed, 14 Jun 2023 20:53:33 GMT  
		Size: 2.7 MB (2677239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d5a41694f99632bb3a7c624dab437c8a10e54b92965de823e717f5c12326b1e`  
		Last Modified: Wed, 21 Jun 2023 01:09:52 GMT  
		Size: 7.2 MB (7169627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2be3d7709e1978d4b030abdf5ac129b97f21e09bb489932628899d96288a4a9`  
		Last Modified: Wed, 21 Jun 2023 01:09:50 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8cba3f7cc400544285611f46bbdba004587f84511783fd05aa6562e9337928f`  
		Last Modified: Wed, 21 Jun 2023 01:09:50 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-bookworm` - linux; arm variant v5

```console
$ docker pull memcached@sha256:1646b01539b9482149379208acae5c0af1c5aed3aa9d818e8748410e15170943
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.1 MB (35094759 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ad4aa07800c4cf602e699a614c04d8fa80a8617828cfeb89fc05b49791d07e7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 12 Jun 2023 23:48:31 GMT
ADD file:54a716f17b23e4fa49d1d5c0a7f63becc295873c116d19bb4753d34f1ca6affb in / 
# Mon, 12 Jun 2023 23:48:31 GMT
CMD ["bash"]
# Wed, 14 Jun 2023 21:56:18 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 14 Jun 2023 21:56:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 21 Jun 2023 00:52:38 GMT
ENV MEMCACHED_VERSION=1.6.21
# Wed, 21 Jun 2023 00:52:39 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Wed, 21 Jun 2023 00:55:49 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 21 Jun 2023 00:55:49 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 21 Jun 2023 00:55:50 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 21 Jun 2023 00:55:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Jun 2023 00:55:50 GMT
USER memcache
# Wed, 21 Jun 2023 00:55:50 GMT
EXPOSE 11211
# Wed, 21 Jun 2023 00:55:50 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:70c60174b18d99741c33011138b5abf2f4d8eca0384521ccb43db3612078e36f`  
		Last Modified: Mon, 12 Jun 2023 23:51:26 GMT  
		Size: 27.0 MB (26982142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52495c3de01d54b61ec15cd608d6ce2ae4587ca764248265b02cb108f790d5a0`  
		Last Modified: Wed, 14 Jun 2023 22:00:39 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:597daa329781ff62c0581a1a2164e04dd294d665a91e97a05aa46fe3d8765eac`  
		Last Modified: Wed, 14 Jun 2023 22:00:40 GMT  
		Size: 2.3 MB (2281778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d65590b8b7bf9398f99bf1baba8d91966081bdc70d61b0165036ac0d16b3b2f`  
		Last Modified: Wed, 21 Jun 2023 00:56:10 GMT  
		Size: 5.8 MB (5829307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dfab31ab9e5a7944b95a42de61a2d1d591fa1605d1a6e2724f9b2c72f03f1ff`  
		Last Modified: Wed, 21 Jun 2023 00:56:09 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85b6795c5e090ce84e068ec9cb629871f3a70380f1bff62aa7baa8a0783343d2`  
		Last Modified: Wed, 21 Jun 2023 00:56:09 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-bookworm` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:d82fec3f72f254431725dc57a8b8922cfb269e018b4407c9e7abb133083b1b32
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.9 MB (37872901 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b25fcbe4e1c3b4ce20a4e4994a494fe7a0d98500c1b5b14f4b92c104898a434c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 04 Jul 2023 01:57:35 GMT
ADD file:71fd66666294148382f2e6a09ae5e277d4c4e9c74402ab64b693a79387b67a09 in / 
# Tue, 04 Jul 2023 01:57:36 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 06:40:00 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 04 Jul 2023 06:40:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 06:40:03 GMT
ENV MEMCACHED_VERSION=1.6.21
# Tue, 04 Jul 2023 06:40:03 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Tue, 04 Jul 2023 06:42:47 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 04 Jul 2023 06:42:47 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 04 Jul 2023 06:42:48 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 04 Jul 2023 06:42:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Jul 2023 06:42:48 GMT
USER memcache
# Tue, 04 Jul 2023 06:42:48 GMT
EXPOSE 11211
# Tue, 04 Jul 2023 06:42:48 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:3ae0c06b4d3aa97d7e0829233dd36cea1666b87074e55fea6bd1ecae066693c7`  
		Last Modified: Tue, 04 Jul 2023 02:01:20 GMT  
		Size: 29.2 MB (29152458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7e0b4333d4768ee800aa733f63a51c54833abe7bd20188154f0869796bb3f8c`  
		Last Modified: Tue, 04 Jul 2023 06:43:03 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fd0e2a70b071a1504381d7831ed736d40261b75692a2fe4ee547186e80ad9b2`  
		Last Modified: Tue, 04 Jul 2023 06:43:03 GMT  
		Size: 2.5 MB (2539167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:382aa3014b4367d16a225a23e5195af1f3a5e51523f9d89461e4b98ddf61aa3d`  
		Last Modified: Tue, 04 Jul 2023 06:43:04 GMT  
		Size: 6.2 MB (6179743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4abaeb5f633e1c888b605fe890a58e527c62021db2516cd8606edad49e9500c0`  
		Last Modified: Tue, 04 Jul 2023 06:43:03 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aedc2da2773982e3f9627ea96874aec7c38a4288cca37a366f29392750f7c38`  
		Last Modified: Tue, 04 Jul 2023 06:43:03 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-bookworm` - linux; 386

```console
$ docker pull memcached@sha256:d275ff7e4cd6b5d699c14115419af7ae2c1bfa32312282ff8c9ba0b424cf6be0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.5 MB (39457503 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8785d2e661831af23d884d73d3196f416198d2c57ffa24c50c8cafe16c0da224`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 12 Jun 2023 23:39:20 GMT
ADD file:c7ecc5e2bed99e2cbca26f9f4247cd9bc399749556f4084e9357a9b00bb80530 in / 
# Mon, 12 Jun 2023 23:39:20 GMT
CMD ["bash"]
# Wed, 14 Jun 2023 22:34:28 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 14 Jun 2023 22:34:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 21 Jun 2023 00:46:59 GMT
ENV MEMCACHED_VERSION=1.6.21
# Wed, 21 Jun 2023 00:46:59 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Wed, 21 Jun 2023 00:50:45 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 21 Jun 2023 00:50:45 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 21 Jun 2023 00:50:46 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 21 Jun 2023 00:50:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Jun 2023 00:50:46 GMT
USER memcache
# Wed, 21 Jun 2023 00:50:46 GMT
EXPOSE 11211
# Wed, 21 Jun 2023 00:50:46 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:82a41d17956dd7c8ebb39c9ce936fd26841bdbec98d0a185e3db8154b352edff`  
		Last Modified: Mon, 12 Jun 2023 23:46:21 GMT  
		Size: 30.1 MB (30140741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:039125a8cebc58c43be503e98831cac166a973cb3e68f4b66194142680e76964`  
		Last Modified: Wed, 14 Jun 2023 22:42:09 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:199b04439aa2a5065d0c23f986eccd0dd093be2f49b180b332af4f35d977ab5b`  
		Last Modified: Wed, 14 Jun 2023 22:42:09 GMT  
		Size: 2.7 MB (2685017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e58126d70102e38c764aa423066a897bc811895dc85b8d607eadfcff947049a7`  
		Last Modified: Wed, 21 Jun 2023 00:54:46 GMT  
		Size: 6.6 MB (6630215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b039c50c059c1c3a231a9659c8ade08b537d8ecac9423685ba16cf308626c4e4`  
		Last Modified: Wed, 21 Jun 2023 00:54:44 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1d3e144a63d04f26029dacd020e1ec00baeae59c5cee460a482e70842be2fc2`  
		Last Modified: Wed, 21 Jun 2023 00:54:44 GMT  
		Size: 116.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-bookworm` - linux; mips64le

```console
$ docker pull memcached@sha256:76620bca6f37fb4a82e0cc3aa33ba7cc2508c8f93dd4ae4956e9b471ce0995a2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.6 MB (37554107 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f8424fcd7f4d7db2c883a9303136b4305e34813630a9e325332ee830d35c026d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 13 Jun 2023 00:09:02 GMT
ADD file:f91bd2a174259cb69646fc34ba2fc6b8941ad8e171d2d7952a4d8ac3d95e2ad7 in / 
# Tue, 13 Jun 2023 00:09:06 GMT
CMD ["bash"]
# Wed, 14 Jun 2023 18:38:15 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 14 Jun 2023 18:38:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 21 Jun 2023 01:14:52 GMT
ENV MEMCACHED_VERSION=1.6.21
# Wed, 21 Jun 2023 01:14:54 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Wed, 21 Jun 2023 01:21:45 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 21 Jun 2023 01:21:47 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 21 Jun 2023 01:21:52 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 21 Jun 2023 01:21:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Jun 2023 01:21:57 GMT
USER memcache
# Wed, 21 Jun 2023 01:22:00 GMT
EXPOSE 11211
# Wed, 21 Jun 2023 01:22:02 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:3fc28260a4d871ef9781cad2bb064ad7212a5063de3a1d35dba938ce82115e5b`  
		Last Modified: Tue, 13 Jun 2023 00:22:29 GMT  
		Size: 29.1 MB (29118129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79c804aeb794275ae845d32d2939d0e0fefa75cd112f1075aaf2104097050ae8`  
		Last Modified: Wed, 14 Jun 2023 18:46:04 GMT  
		Size: 1.1 KB (1078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf29fcbe26928e2f4086a889098220505bdd4401dc87958f623ade0618efcd28`  
		Last Modified: Wed, 14 Jun 2023 18:46:05 GMT  
		Size: 1.9 MB (1934899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1d2070a6fd2a146f7a7ccda5a6b5c9e7188304b3eb6ad56e85ae5e13af6efff`  
		Last Modified: Wed, 21 Jun 2023 01:22:36 GMT  
		Size: 6.5 MB (6499598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb2d53b7e662ee08ffe5d3ff1b97e2bbec271b2427e8428d38ab879c1a68cbdd`  
		Last Modified: Wed, 21 Jun 2023 01:22:31 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e13b007130a18104c8ce3a24f68b588c6ec439dcb4c22e430edf1baab337bb13`  
		Last Modified: Wed, 21 Jun 2023 01:22:31 GMT  
		Size: 118.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-bookworm` - linux; ppc64le

```console
$ docker pull memcached@sha256:0466889ea7a59c3e5075122e0dfac5f9fd4b740dbc54d7ca3355e661704b7df3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.2 MB (43193731 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f99a2d51677ef27121ea5fb73098453983811a697bb67558da1548d6a2b1a4d7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 04 Jul 2023 01:17:51 GMT
ADD file:51887002f5002ccc662adbc6ecf1129e3db375a7a77b93da43cc9a8326b3c4b9 in / 
# Tue, 04 Jul 2023 01:17:53 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 06:45:59 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 04 Jul 2023 06:46:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 06:46:11 GMT
ENV MEMCACHED_VERSION=1.6.21
# Tue, 04 Jul 2023 06:46:12 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Tue, 04 Jul 2023 06:50:32 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 04 Jul 2023 06:50:34 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 04 Jul 2023 06:50:36 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 04 Jul 2023 06:50:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Jul 2023 06:50:36 GMT
USER memcache
# Tue, 04 Jul 2023 06:50:37 GMT
EXPOSE 11211
# Tue, 04 Jul 2023 06:50:37 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:ba99a1aa5a92d949d988e66df7723a542fd81bc30eef9d4269e8a899820d4bb2`  
		Last Modified: Tue, 04 Jul 2023 01:24:36 GMT  
		Size: 33.1 MB (33116716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57bc245122d94a5d6dbd04e3f0d2cc3731cb7e5479f873ad6588885b1a1e7fff`  
		Last Modified: Tue, 04 Jul 2023 06:51:13 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8302634866fb43cf1942126242ebd186c7a31db3f01e63b626c2c6cb31aa01bb`  
		Last Modified: Tue, 04 Jul 2023 06:51:14 GMT  
		Size: 2.9 MB (2891325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85b07e92e6621b42a17464a214cee12ada2ca5c70c139194a0d9d5cdf753e470`  
		Last Modified: Tue, 04 Jul 2023 06:51:16 GMT  
		Size: 7.2 MB (7184153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:060e182005428d5f8ae46505c71da839515e43c949a2109682b933781ad7b42d`  
		Last Modified: Tue, 04 Jul 2023 06:51:13 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd71a227a79337edf4a41188a95ac6c897f53d5cc1ebfa6201b14525057ce473`  
		Last Modified: Tue, 04 Jul 2023 06:51:13 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-bookworm` - linux; s390x

```console
$ docker pull memcached@sha256:f90935a3646db47ef74efba3a8ea148e6fa9a6058557fd686664b3a9b83cf5b4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.9 MB (35907614 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:55f50234cc8836dd1977a706a4d7845c857ac2128081a776c895db012f73e5bb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 13 Jun 2023 04:29:41 GMT
ADD file:739f4c23557ec0af5f4ba492c847b5d2f09dd81211c675d0e9eabe865d794e81 in / 
# Tue, 13 Jun 2023 04:29:43 GMT
CMD ["bash"]
# Thu, 15 Jun 2023 06:23:25 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Thu, 15 Jun 2023 06:23:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 21 Jun 2023 00:54:39 GMT
ENV MEMCACHED_VERSION=1.6.21
# Wed, 21 Jun 2023 00:54:39 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Wed, 21 Jun 2023 00:57:46 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 21 Jun 2023 00:57:47 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 21 Jun 2023 00:57:47 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 21 Jun 2023 00:57:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Jun 2023 00:57:47 GMT
USER memcache
# Wed, 21 Jun 2023 00:57:47 GMT
EXPOSE 11211
# Wed, 21 Jun 2023 00:57:48 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:6571b3abd058e377c7bd231c9029aff6eb25486bffb50229076d2e6a356a517f`  
		Last Modified: Tue, 13 Jun 2023 04:34:21 GMT  
		Size: 27.5 MB (27487928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1521043364f590f749ce68598ad1f79907ef04ee2283314cfaab3f72df8e15c`  
		Last Modified: Thu, 15 Jun 2023 06:35:17 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdbc1e75c128be037526f9b133061f5dc6c9baf2f00b5d5b229427bd89eb55b7`  
		Last Modified: Thu, 15 Jun 2023 06:35:18 GMT  
		Size: 2.3 MB (2345340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f3d048c5c76c19c7c7d783cac8384f5698dd61a6aa7ee9067521407789ec9b4`  
		Last Modified: Wed, 21 Jun 2023 01:01:34 GMT  
		Size: 6.1 MB (6072815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c7bfbb7d1965d17408766d01c40f67a94eb422714618a239a48b62cedafdcab`  
		Last Modified: Wed, 21 Jun 2023 01:01:33 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:164d3c9aaa0239a91376552d50ffc16a1e2bf9e3c323e81d2a976556ab25f4a2`  
		Last Modified: Wed, 21 Jun 2023 01:01:33 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:1.6.21`

```console
$ docker pull memcached@sha256:6d50bee6d0eaba83831fead39d52d67ede2aefc3acf69a19d503a9488234e1c8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 7
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; s390x

### `memcached:1.6.21` - linux; amd64

```console
$ docker pull memcached@sha256:37d77084cbe7c98854989a68a18f22dd677379de8ffc9ee92fbf7b88b2b4d0f9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.0 MB (38973142 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a4d0c1490511995c15a4c1ca7c8413337bed068ea95507aae882010b051ca37e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 12 Jun 2023 23:20:42 GMT
ADD file:ba1250b6ecd5dd09d4914189d72741c2817988994e7da514bf62be439a34bdb5 in / 
# Mon, 12 Jun 2023 23:20:42 GMT
CMD ["bash"]
# Wed, 14 Jun 2023 20:48:19 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 14 Jun 2023 20:48:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 21 Jun 2023 01:04:34 GMT
ENV MEMCACHED_VERSION=1.6.21
# Wed, 21 Jun 2023 01:04:35 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Wed, 21 Jun 2023 01:07:04 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 21 Jun 2023 01:07:04 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 21 Jun 2023 01:07:04 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 21 Jun 2023 01:07:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Jun 2023 01:07:05 GMT
USER memcache
# Wed, 21 Jun 2023 01:07:05 GMT
EXPOSE 11211
# Wed, 21 Jun 2023 01:07:05 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:5b5fe70539cd6989aa19f25826309f9715a9489cf1c057982d6a84c1ad8975c7`  
		Last Modified: Mon, 12 Jun 2023 23:25:49 GMT  
		Size: 29.1 MB (29124744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab209434009a85e82d99c0547bb947940f9e1002ce6e965417396ee22a6820db`  
		Last Modified: Wed, 14 Jun 2023 20:53:33 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2f4dfc49c9cdae8d4df855de7cc0460e5db8c762e73786d4f8fa4f69ba11d6d`  
		Last Modified: Wed, 14 Jun 2023 20:53:33 GMT  
		Size: 2.7 MB (2677239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d5a41694f99632bb3a7c624dab437c8a10e54b92965de823e717f5c12326b1e`  
		Last Modified: Wed, 21 Jun 2023 01:09:52 GMT  
		Size: 7.2 MB (7169627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2be3d7709e1978d4b030abdf5ac129b97f21e09bb489932628899d96288a4a9`  
		Last Modified: Wed, 21 Jun 2023 01:09:50 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8cba3f7cc400544285611f46bbdba004587f84511783fd05aa6562e9337928f`  
		Last Modified: Wed, 21 Jun 2023 01:09:50 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.21` - linux; arm variant v5

```console
$ docker pull memcached@sha256:1646b01539b9482149379208acae5c0af1c5aed3aa9d818e8748410e15170943
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.1 MB (35094759 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ad4aa07800c4cf602e699a614c04d8fa80a8617828cfeb89fc05b49791d07e7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 12 Jun 2023 23:48:31 GMT
ADD file:54a716f17b23e4fa49d1d5c0a7f63becc295873c116d19bb4753d34f1ca6affb in / 
# Mon, 12 Jun 2023 23:48:31 GMT
CMD ["bash"]
# Wed, 14 Jun 2023 21:56:18 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 14 Jun 2023 21:56:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 21 Jun 2023 00:52:38 GMT
ENV MEMCACHED_VERSION=1.6.21
# Wed, 21 Jun 2023 00:52:39 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Wed, 21 Jun 2023 00:55:49 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 21 Jun 2023 00:55:49 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 21 Jun 2023 00:55:50 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 21 Jun 2023 00:55:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Jun 2023 00:55:50 GMT
USER memcache
# Wed, 21 Jun 2023 00:55:50 GMT
EXPOSE 11211
# Wed, 21 Jun 2023 00:55:50 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:70c60174b18d99741c33011138b5abf2f4d8eca0384521ccb43db3612078e36f`  
		Last Modified: Mon, 12 Jun 2023 23:51:26 GMT  
		Size: 27.0 MB (26982142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52495c3de01d54b61ec15cd608d6ce2ae4587ca764248265b02cb108f790d5a0`  
		Last Modified: Wed, 14 Jun 2023 22:00:39 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:597daa329781ff62c0581a1a2164e04dd294d665a91e97a05aa46fe3d8765eac`  
		Last Modified: Wed, 14 Jun 2023 22:00:40 GMT  
		Size: 2.3 MB (2281778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d65590b8b7bf9398f99bf1baba8d91966081bdc70d61b0165036ac0d16b3b2f`  
		Last Modified: Wed, 21 Jun 2023 00:56:10 GMT  
		Size: 5.8 MB (5829307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dfab31ab9e5a7944b95a42de61a2d1d591fa1605d1a6e2724f9b2c72f03f1ff`  
		Last Modified: Wed, 21 Jun 2023 00:56:09 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85b6795c5e090ce84e068ec9cb629871f3a70380f1bff62aa7baa8a0783343d2`  
		Last Modified: Wed, 21 Jun 2023 00:56:09 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.21` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:d82fec3f72f254431725dc57a8b8922cfb269e018b4407c9e7abb133083b1b32
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.9 MB (37872901 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b25fcbe4e1c3b4ce20a4e4994a494fe7a0d98500c1b5b14f4b92c104898a434c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 04 Jul 2023 01:57:35 GMT
ADD file:71fd66666294148382f2e6a09ae5e277d4c4e9c74402ab64b693a79387b67a09 in / 
# Tue, 04 Jul 2023 01:57:36 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 06:40:00 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 04 Jul 2023 06:40:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 06:40:03 GMT
ENV MEMCACHED_VERSION=1.6.21
# Tue, 04 Jul 2023 06:40:03 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Tue, 04 Jul 2023 06:42:47 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 04 Jul 2023 06:42:47 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 04 Jul 2023 06:42:48 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 04 Jul 2023 06:42:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Jul 2023 06:42:48 GMT
USER memcache
# Tue, 04 Jul 2023 06:42:48 GMT
EXPOSE 11211
# Tue, 04 Jul 2023 06:42:48 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:3ae0c06b4d3aa97d7e0829233dd36cea1666b87074e55fea6bd1ecae066693c7`  
		Last Modified: Tue, 04 Jul 2023 02:01:20 GMT  
		Size: 29.2 MB (29152458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7e0b4333d4768ee800aa733f63a51c54833abe7bd20188154f0869796bb3f8c`  
		Last Modified: Tue, 04 Jul 2023 06:43:03 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fd0e2a70b071a1504381d7831ed736d40261b75692a2fe4ee547186e80ad9b2`  
		Last Modified: Tue, 04 Jul 2023 06:43:03 GMT  
		Size: 2.5 MB (2539167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:382aa3014b4367d16a225a23e5195af1f3a5e51523f9d89461e4b98ddf61aa3d`  
		Last Modified: Tue, 04 Jul 2023 06:43:04 GMT  
		Size: 6.2 MB (6179743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4abaeb5f633e1c888b605fe890a58e527c62021db2516cd8606edad49e9500c0`  
		Last Modified: Tue, 04 Jul 2023 06:43:03 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aedc2da2773982e3f9627ea96874aec7c38a4288cca37a366f29392750f7c38`  
		Last Modified: Tue, 04 Jul 2023 06:43:03 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.21` - linux; 386

```console
$ docker pull memcached@sha256:d275ff7e4cd6b5d699c14115419af7ae2c1bfa32312282ff8c9ba0b424cf6be0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.5 MB (39457503 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8785d2e661831af23d884d73d3196f416198d2c57ffa24c50c8cafe16c0da224`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 12 Jun 2023 23:39:20 GMT
ADD file:c7ecc5e2bed99e2cbca26f9f4247cd9bc399749556f4084e9357a9b00bb80530 in / 
# Mon, 12 Jun 2023 23:39:20 GMT
CMD ["bash"]
# Wed, 14 Jun 2023 22:34:28 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 14 Jun 2023 22:34:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 21 Jun 2023 00:46:59 GMT
ENV MEMCACHED_VERSION=1.6.21
# Wed, 21 Jun 2023 00:46:59 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Wed, 21 Jun 2023 00:50:45 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 21 Jun 2023 00:50:45 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 21 Jun 2023 00:50:46 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 21 Jun 2023 00:50:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Jun 2023 00:50:46 GMT
USER memcache
# Wed, 21 Jun 2023 00:50:46 GMT
EXPOSE 11211
# Wed, 21 Jun 2023 00:50:46 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:82a41d17956dd7c8ebb39c9ce936fd26841bdbec98d0a185e3db8154b352edff`  
		Last Modified: Mon, 12 Jun 2023 23:46:21 GMT  
		Size: 30.1 MB (30140741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:039125a8cebc58c43be503e98831cac166a973cb3e68f4b66194142680e76964`  
		Last Modified: Wed, 14 Jun 2023 22:42:09 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:199b04439aa2a5065d0c23f986eccd0dd093be2f49b180b332af4f35d977ab5b`  
		Last Modified: Wed, 14 Jun 2023 22:42:09 GMT  
		Size: 2.7 MB (2685017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e58126d70102e38c764aa423066a897bc811895dc85b8d607eadfcff947049a7`  
		Last Modified: Wed, 21 Jun 2023 00:54:46 GMT  
		Size: 6.6 MB (6630215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b039c50c059c1c3a231a9659c8ade08b537d8ecac9423685ba16cf308626c4e4`  
		Last Modified: Wed, 21 Jun 2023 00:54:44 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1d3e144a63d04f26029dacd020e1ec00baeae59c5cee460a482e70842be2fc2`  
		Last Modified: Wed, 21 Jun 2023 00:54:44 GMT  
		Size: 116.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.21` - linux; mips64le

```console
$ docker pull memcached@sha256:76620bca6f37fb4a82e0cc3aa33ba7cc2508c8f93dd4ae4956e9b471ce0995a2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.6 MB (37554107 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f8424fcd7f4d7db2c883a9303136b4305e34813630a9e325332ee830d35c026d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 13 Jun 2023 00:09:02 GMT
ADD file:f91bd2a174259cb69646fc34ba2fc6b8941ad8e171d2d7952a4d8ac3d95e2ad7 in / 
# Tue, 13 Jun 2023 00:09:06 GMT
CMD ["bash"]
# Wed, 14 Jun 2023 18:38:15 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 14 Jun 2023 18:38:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 21 Jun 2023 01:14:52 GMT
ENV MEMCACHED_VERSION=1.6.21
# Wed, 21 Jun 2023 01:14:54 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Wed, 21 Jun 2023 01:21:45 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 21 Jun 2023 01:21:47 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 21 Jun 2023 01:21:52 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 21 Jun 2023 01:21:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Jun 2023 01:21:57 GMT
USER memcache
# Wed, 21 Jun 2023 01:22:00 GMT
EXPOSE 11211
# Wed, 21 Jun 2023 01:22:02 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:3fc28260a4d871ef9781cad2bb064ad7212a5063de3a1d35dba938ce82115e5b`  
		Last Modified: Tue, 13 Jun 2023 00:22:29 GMT  
		Size: 29.1 MB (29118129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79c804aeb794275ae845d32d2939d0e0fefa75cd112f1075aaf2104097050ae8`  
		Last Modified: Wed, 14 Jun 2023 18:46:04 GMT  
		Size: 1.1 KB (1078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf29fcbe26928e2f4086a889098220505bdd4401dc87958f623ade0618efcd28`  
		Last Modified: Wed, 14 Jun 2023 18:46:05 GMT  
		Size: 1.9 MB (1934899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1d2070a6fd2a146f7a7ccda5a6b5c9e7188304b3eb6ad56e85ae5e13af6efff`  
		Last Modified: Wed, 21 Jun 2023 01:22:36 GMT  
		Size: 6.5 MB (6499598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb2d53b7e662ee08ffe5d3ff1b97e2bbec271b2427e8428d38ab879c1a68cbdd`  
		Last Modified: Wed, 21 Jun 2023 01:22:31 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e13b007130a18104c8ce3a24f68b588c6ec439dcb4c22e430edf1baab337bb13`  
		Last Modified: Wed, 21 Jun 2023 01:22:31 GMT  
		Size: 118.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.21` - linux; ppc64le

```console
$ docker pull memcached@sha256:0466889ea7a59c3e5075122e0dfac5f9fd4b740dbc54d7ca3355e661704b7df3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.2 MB (43193731 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f99a2d51677ef27121ea5fb73098453983811a697bb67558da1548d6a2b1a4d7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 04 Jul 2023 01:17:51 GMT
ADD file:51887002f5002ccc662adbc6ecf1129e3db375a7a77b93da43cc9a8326b3c4b9 in / 
# Tue, 04 Jul 2023 01:17:53 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 06:45:59 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 04 Jul 2023 06:46:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 06:46:11 GMT
ENV MEMCACHED_VERSION=1.6.21
# Tue, 04 Jul 2023 06:46:12 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Tue, 04 Jul 2023 06:50:32 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 04 Jul 2023 06:50:34 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 04 Jul 2023 06:50:36 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 04 Jul 2023 06:50:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Jul 2023 06:50:36 GMT
USER memcache
# Tue, 04 Jul 2023 06:50:37 GMT
EXPOSE 11211
# Tue, 04 Jul 2023 06:50:37 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:ba99a1aa5a92d949d988e66df7723a542fd81bc30eef9d4269e8a899820d4bb2`  
		Last Modified: Tue, 04 Jul 2023 01:24:36 GMT  
		Size: 33.1 MB (33116716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57bc245122d94a5d6dbd04e3f0d2cc3731cb7e5479f873ad6588885b1a1e7fff`  
		Last Modified: Tue, 04 Jul 2023 06:51:13 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8302634866fb43cf1942126242ebd186c7a31db3f01e63b626c2c6cb31aa01bb`  
		Last Modified: Tue, 04 Jul 2023 06:51:14 GMT  
		Size: 2.9 MB (2891325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85b07e92e6621b42a17464a214cee12ada2ca5c70c139194a0d9d5cdf753e470`  
		Last Modified: Tue, 04 Jul 2023 06:51:16 GMT  
		Size: 7.2 MB (7184153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:060e182005428d5f8ae46505c71da839515e43c949a2109682b933781ad7b42d`  
		Last Modified: Tue, 04 Jul 2023 06:51:13 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd71a227a79337edf4a41188a95ac6c897f53d5cc1ebfa6201b14525057ce473`  
		Last Modified: Tue, 04 Jul 2023 06:51:13 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.21` - linux; s390x

```console
$ docker pull memcached@sha256:f90935a3646db47ef74efba3a8ea148e6fa9a6058557fd686664b3a9b83cf5b4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.9 MB (35907614 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:55f50234cc8836dd1977a706a4d7845c857ac2128081a776c895db012f73e5bb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 13 Jun 2023 04:29:41 GMT
ADD file:739f4c23557ec0af5f4ba492c847b5d2f09dd81211c675d0e9eabe865d794e81 in / 
# Tue, 13 Jun 2023 04:29:43 GMT
CMD ["bash"]
# Thu, 15 Jun 2023 06:23:25 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Thu, 15 Jun 2023 06:23:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 21 Jun 2023 00:54:39 GMT
ENV MEMCACHED_VERSION=1.6.21
# Wed, 21 Jun 2023 00:54:39 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Wed, 21 Jun 2023 00:57:46 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 21 Jun 2023 00:57:47 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 21 Jun 2023 00:57:47 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 21 Jun 2023 00:57:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Jun 2023 00:57:47 GMT
USER memcache
# Wed, 21 Jun 2023 00:57:47 GMT
EXPOSE 11211
# Wed, 21 Jun 2023 00:57:48 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:6571b3abd058e377c7bd231c9029aff6eb25486bffb50229076d2e6a356a517f`  
		Last Modified: Tue, 13 Jun 2023 04:34:21 GMT  
		Size: 27.5 MB (27487928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1521043364f590f749ce68598ad1f79907ef04ee2283314cfaab3f72df8e15c`  
		Last Modified: Thu, 15 Jun 2023 06:35:17 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdbc1e75c128be037526f9b133061f5dc6c9baf2f00b5d5b229427bd89eb55b7`  
		Last Modified: Thu, 15 Jun 2023 06:35:18 GMT  
		Size: 2.3 MB (2345340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f3d048c5c76c19c7c7d783cac8384f5698dd61a6aa7ee9067521407789ec9b4`  
		Last Modified: Wed, 21 Jun 2023 01:01:34 GMT  
		Size: 6.1 MB (6072815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c7bfbb7d1965d17408766d01c40f67a94eb422714618a239a48b62cedafdcab`  
		Last Modified: Wed, 21 Jun 2023 01:01:33 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:164d3c9aaa0239a91376552d50ffc16a1e2bf9e3c323e81d2a976556ab25f4a2`  
		Last Modified: Wed, 21 Jun 2023 01:01:33 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:1.6.21-alpine`

```console
$ docker pull memcached@sha256:ee437fd9a952b48de768cd5c7a97d43439e05b918e4bc4452e296e8bdafae046
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `memcached:1.6.21-alpine` - linux; amd64

```console
$ docker pull memcached@sha256:574ef430513a38925cc52ae5954677a12e0a57205fed96be5707196a180e5159
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4462428 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f7da63106561ab1f7284992dad2396b234096070b4269971b23c53f2f8498ef`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 14 Jun 2023 20:41:58 GMT
ADD file:1da756d12551a0e3e793e02ef87432d69d4968937bd11bed0af215db19dd94cd in / 
# Wed, 14 Jun 2023 20:41:59 GMT
CMD ["/bin/sh"]
# Wed, 14 Jun 2023 20:50:58 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Wed, 14 Jun 2023 20:50:59 GMT
RUN apk add --no-cache libsasl
# Wed, 21 Jun 2023 01:07:13 GMT
ENV MEMCACHED_VERSION=1.6.21
# Wed, 21 Jun 2023 01:07:13 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Wed, 21 Jun 2023 01:09:21 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Wed, 21 Jun 2023 01:09:21 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 21 Jun 2023 01:09:22 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 21 Jun 2023 01:09:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Jun 2023 01:09:22 GMT
USER memcache
# Wed, 21 Jun 2023 01:09:22 GMT
EXPOSE 11211
# Wed, 21 Jun 2023 01:09:22 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:31e352740f534f9ad170f75378a84fe453d6156e40700b882d737a8f4a6988a3`  
		Last Modified: Wed, 14 Jun 2023 20:42:26 GMT  
		Size: 3.4 MB (3397879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b2b2df106c5026cd33ea4ac655b77f25410ec9f4b8a6756ebc1ceeb79fca3c7`  
		Last Modified: Wed, 14 Jun 2023 20:53:58 GMT  
		Size: 1.3 KB (1266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed63668528d3e2159f55909c66dc48a6f746ce24c2e2f6d963b992aefaa457ce`  
		Last Modified: Wed, 14 Jun 2023 20:53:58 GMT  
		Size: 108.1 KB (108080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05536f2f26c904a5aa1b07720957a37e8b57a223725d76f8d1473dcab297a233`  
		Last Modified: Wed, 21 Jun 2023 01:10:14 GMT  
		Size: 954.8 KB (954811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e448b573a98adc8bd0a4805cb0e1b451aea0d1582f0462aa0b147799a97fad7`  
		Last Modified: Wed, 21 Jun 2023 01:10:13 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3029a709b7be20aeff1e9cebe5c6112cd1df5a0ea3efb58e61380cc75b9296e`  
		Last Modified: Wed, 21 Jun 2023 01:10:13 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.21-alpine` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:eb4b801b9c9e9af6565ac003b21af39b06d55943bbc4e59a02d465fdf7f07776
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.4 MB (4399342 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4aa99dd98a2fa001241d907951530f4afebadfd4895545c5d73f31e29b7a35fa`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 14 Jun 2023 20:48:58 GMT
ADD file:289c2fac17119508ced527225d445747cd177111b4a0018a6b04948ecb3b5e29 in / 
# Wed, 14 Jun 2023 20:48:58 GMT
CMD ["/bin/sh"]
# Wed, 14 Jun 2023 20:57:26 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Wed, 14 Jun 2023 20:57:27 GMT
RUN apk add --no-cache libsasl
# Wed, 21 Jun 2023 01:08:09 GMT
ENV MEMCACHED_VERSION=1.6.21
# Wed, 21 Jun 2023 01:08:09 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Wed, 21 Jun 2023 01:10:35 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Wed, 21 Jun 2023 01:10:35 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 21 Jun 2023 01:10:36 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 21 Jun 2023 01:10:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Jun 2023 01:10:36 GMT
USER memcache
# Wed, 21 Jun 2023 01:10:36 GMT
EXPOSE 11211
# Wed, 21 Jun 2023 01:10:36 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:8c6d1654570f041603f4cef49c320c8f6f3e401324913009d92a19132cbf1ac0`  
		Last Modified: Wed, 14 Jun 2023 20:49:23 GMT  
		Size: 3.3 MB (3329251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:666588188768f19b27fb821e02d084406af8fd867cc4595b896b9eed50b2105e`  
		Last Modified: Wed, 14 Jun 2023 21:00:51 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7d958a137d671266f063c0af4d7b0b6d44d9018b77fdbddb8fd412d3c0b1be3`  
		Last Modified: Wed, 14 Jun 2023 21:00:51 GMT  
		Size: 124.1 KB (124137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a66841dcfe05dcef1af82648941fa1ea0e10dbdf022326916d1d74afc99885c6`  
		Last Modified: Wed, 21 Jun 2023 01:11:21 GMT  
		Size: 944.3 KB (944292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b46fdc76bcbc8fa94ae23177ac32b97a4d370a630ec7d3f52bd8aae174e75982`  
		Last Modified: Wed, 21 Jun 2023 01:11:20 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea70db1a59f508c629aef54fb39ac3ada5cfcc3aac7aa1d6ed6cde22e97d3e3b`  
		Last Modified: Wed, 21 Jun 2023 01:11:20 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.21-alpine` - linux; 386

```console
$ docker pull memcached@sha256:73c987449b9f764e060e2745d29e0ee50f4f7e630ddd23631c517e65f2315bfa
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.3 MB (4282253 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c47771f0d8f2ab5f38441f65fed7a05d87ea44b1de1a502321348997971362c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 14 Jun 2023 22:33:22 GMT
ADD file:94bec00e2c0c7f47c81ec4355a29ca23a81b439797d037b1a5a455f36a25dab4 in / 
# Wed, 14 Jun 2023 22:33:22 GMT
CMD ["/bin/sh"]
# Wed, 14 Jun 2023 22:38:20 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Wed, 14 Jun 2023 22:38:22 GMT
RUN apk add --no-cache libsasl
# Wed, 21 Jun 2023 00:50:52 GMT
ENV MEMCACHED_VERSION=1.6.21
# Wed, 21 Jun 2023 00:50:52 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Wed, 21 Jun 2023 00:54:21 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Wed, 21 Jun 2023 00:54:22 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 21 Jun 2023 00:54:22 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 21 Jun 2023 00:54:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Jun 2023 00:54:22 GMT
USER memcache
# Wed, 21 Jun 2023 00:54:22 GMT
EXPOSE 11211
# Wed, 21 Jun 2023 00:54:23 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:b3f50075abd13aad1cb7d8c1427aa59d7fcac88f3690d3f9c3efdbec80fd0856`  
		Last Modified: Wed, 14 Jun 2023 22:33:48 GMT  
		Size: 3.2 MB (3233951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:358673fc695429dd9142a4904a518e96c418229121d02435d875a993d9e5fac1`  
		Last Modified: Wed, 14 Jun 2023 22:42:32 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ae09e638ab1208326cbfd03f4517b0d1d13f72cfc8add3a055321fe5cf0f53a`  
		Last Modified: Wed, 14 Jun 2023 22:42:32 GMT  
		Size: 109.5 KB (109531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ed35577a5a4360f65bc0361d7bca857e45fad4baf04bcde5e731529377e9f58`  
		Last Modified: Wed, 21 Jun 2023 00:55:07 GMT  
		Size: 937.1 KB (937107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c4024dd0449592764b513374729cea0a478f62deaf32af4b23e536ffca016b6`  
		Last Modified: Wed, 21 Jun 2023 00:55:07 GMT  
		Size: 280.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6d29f640e8837bc0d0ed4b3fc505f71494f0c3ef917245b2399971ca3cb38e8`  
		Last Modified: Wed, 21 Jun 2023 00:55:06 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.21-alpine` - linux; ppc64le

```console
$ docker pull memcached@sha256:e02abd3f1c109243a103019450a45039503d018c8fcd2fb607798643fbeaed69
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4453245 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7311794e1380b44e42daf3ea3c49269eb71549d5f62a46f6596478d01bda3b02`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 15 Jun 2023 00:39:49 GMT
ADD file:694c636c0dd19fd01accbc189e4c1dc4d063952692c6e7eb26dce02a7adba833 in / 
# Thu, 15 Jun 2023 00:39:49 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 04:20:00 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Thu, 15 Jun 2023 04:20:03 GMT
RUN apk add --no-cache libsasl
# Wed, 21 Jun 2023 01:42:40 GMT
ENV MEMCACHED_VERSION=1.6.21
# Wed, 21 Jun 2023 01:42:40 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Wed, 21 Jun 2023 01:45:42 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Wed, 21 Jun 2023 01:45:43 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 21 Jun 2023 01:45:45 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 21 Jun 2023 01:45:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Jun 2023 01:45:46 GMT
USER memcache
# Wed, 21 Jun 2023 01:45:46 GMT
EXPOSE 11211
# Wed, 21 Jun 2023 01:45:47 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:ffa4a466dbb8eebd7e7f25590a9df12390de9016abf82279c29c9a64aa76491a`  
		Last Modified: Thu, 15 Jun 2023 00:40:26 GMT  
		Size: 3.3 MB (3344781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:607cb6edfb2d0718375d44dbfb94d80d9b5e23a38a6bad8d2fe9c624a0ae354a`  
		Last Modified: Thu, 15 Jun 2023 04:23:36 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f97572f9bc2bc81fb5496a46ecd8b44cdb5b616d0beaecaabb186e3523683a32`  
		Last Modified: Thu, 15 Jun 2023 04:23:37 GMT  
		Size: 123.9 KB (123931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da5b2f6c7aee3051aa1b53ff9a66885509bad54b27aa37aebe382fc1ca4eab1f`  
		Last Modified: Wed, 21 Jun 2023 01:46:43 GMT  
		Size: 982.9 KB (982864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a08963a0c7d8349568389e6f7af0c7a1b55f2b0aea5d25bfa94d415fbb94af9`  
		Last Modified: Wed, 21 Jun 2023 01:46:43 GMT  
		Size: 282.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d866cc948bf60127d37a1f655a84d6b9c17376a21656e660c47efc6d3f499ba2`  
		Last Modified: Wed, 21 Jun 2023 01:46:43 GMT  
		Size: 118.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.21-alpine` - linux; s390x

```console
$ docker pull memcached@sha256:cd97d93e79c2345a0c10f20a912f29a0ccf5590e15c00df81596397b9567233f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.3 MB (4278263 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f56d14fce8cfd200c86bd00cd28c95574b6bf2863bd203e7644d44a08db84ab`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 15 Jun 2023 05:18:38 GMT
ADD file:a59beca78118ebf4f86cc1685237dc3a29a519401a70668da520beaa3d29eb7a in / 
# Thu, 15 Jun 2023 05:18:38 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 06:27:47 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Thu, 15 Jun 2023 06:27:49 GMT
RUN apk add --no-cache libsasl
# Wed, 21 Jun 2023 00:58:01 GMT
ENV MEMCACHED_VERSION=1.6.21
# Wed, 21 Jun 2023 00:58:01 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Wed, 21 Jun 2023 01:01:08 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Wed, 21 Jun 2023 01:01:09 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 21 Jun 2023 01:01:09 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 21 Jun 2023 01:01:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Jun 2023 01:01:09 GMT
USER memcache
# Wed, 21 Jun 2023 01:01:10 GMT
EXPOSE 11211
# Wed, 21 Jun 2023 01:01:10 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:998cc98447b44e5f0fe799dce691412796ba586ab22eb7c99aebf9d45f34833b`  
		Last Modified: Thu, 15 Jun 2023 05:29:38 GMT  
		Size: 3.2 MB (3213497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:156deb87465a2c5629e5ae28c2a7251d5684baea5a930cf65ff6b478de321202`  
		Last Modified: Thu, 15 Jun 2023 06:36:33 GMT  
		Size: 1.3 KB (1266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19020c60d58f4724218660e819b1b33b5d1428c3c5027492a2ee3c44228231df`  
		Last Modified: Thu, 15 Jun 2023 06:36:33 GMT  
		Size: 112.8 KB (112849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81e76f938f015ccb0b5d2915145432efbc0af21a2f4964e0c9a67bfbbe6a577e`  
		Last Modified: Wed, 21 Jun 2023 01:01:46 GMT  
		Size: 950.3 KB (950254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b613e0a69ced3425a5949c15688d493ef10d80eb28c7bb626f0c092223fe1302`  
		Last Modified: Wed, 21 Jun 2023 01:01:46 GMT  
		Size: 280.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4db4c30d38bb65cd11068e1892913b2fa04add8f27abe601485cc3b09754eb50`  
		Last Modified: Wed, 21 Jun 2023 01:01:46 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:1.6.21-alpine3.18`

```console
$ docker pull memcached@sha256:ee437fd9a952b48de768cd5c7a97d43439e05b918e4bc4452e296e8bdafae046
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `memcached:1.6.21-alpine3.18` - linux; amd64

```console
$ docker pull memcached@sha256:574ef430513a38925cc52ae5954677a12e0a57205fed96be5707196a180e5159
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4462428 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f7da63106561ab1f7284992dad2396b234096070b4269971b23c53f2f8498ef`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 14 Jun 2023 20:41:58 GMT
ADD file:1da756d12551a0e3e793e02ef87432d69d4968937bd11bed0af215db19dd94cd in / 
# Wed, 14 Jun 2023 20:41:59 GMT
CMD ["/bin/sh"]
# Wed, 14 Jun 2023 20:50:58 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Wed, 14 Jun 2023 20:50:59 GMT
RUN apk add --no-cache libsasl
# Wed, 21 Jun 2023 01:07:13 GMT
ENV MEMCACHED_VERSION=1.6.21
# Wed, 21 Jun 2023 01:07:13 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Wed, 21 Jun 2023 01:09:21 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Wed, 21 Jun 2023 01:09:21 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 21 Jun 2023 01:09:22 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 21 Jun 2023 01:09:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Jun 2023 01:09:22 GMT
USER memcache
# Wed, 21 Jun 2023 01:09:22 GMT
EXPOSE 11211
# Wed, 21 Jun 2023 01:09:22 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:31e352740f534f9ad170f75378a84fe453d6156e40700b882d737a8f4a6988a3`  
		Last Modified: Wed, 14 Jun 2023 20:42:26 GMT  
		Size: 3.4 MB (3397879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b2b2df106c5026cd33ea4ac655b77f25410ec9f4b8a6756ebc1ceeb79fca3c7`  
		Last Modified: Wed, 14 Jun 2023 20:53:58 GMT  
		Size: 1.3 KB (1266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed63668528d3e2159f55909c66dc48a6f746ce24c2e2f6d963b992aefaa457ce`  
		Last Modified: Wed, 14 Jun 2023 20:53:58 GMT  
		Size: 108.1 KB (108080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05536f2f26c904a5aa1b07720957a37e8b57a223725d76f8d1473dcab297a233`  
		Last Modified: Wed, 21 Jun 2023 01:10:14 GMT  
		Size: 954.8 KB (954811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e448b573a98adc8bd0a4805cb0e1b451aea0d1582f0462aa0b147799a97fad7`  
		Last Modified: Wed, 21 Jun 2023 01:10:13 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3029a709b7be20aeff1e9cebe5c6112cd1df5a0ea3efb58e61380cc75b9296e`  
		Last Modified: Wed, 21 Jun 2023 01:10:13 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.21-alpine3.18` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:eb4b801b9c9e9af6565ac003b21af39b06d55943bbc4e59a02d465fdf7f07776
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.4 MB (4399342 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4aa99dd98a2fa001241d907951530f4afebadfd4895545c5d73f31e29b7a35fa`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 14 Jun 2023 20:48:58 GMT
ADD file:289c2fac17119508ced527225d445747cd177111b4a0018a6b04948ecb3b5e29 in / 
# Wed, 14 Jun 2023 20:48:58 GMT
CMD ["/bin/sh"]
# Wed, 14 Jun 2023 20:57:26 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Wed, 14 Jun 2023 20:57:27 GMT
RUN apk add --no-cache libsasl
# Wed, 21 Jun 2023 01:08:09 GMT
ENV MEMCACHED_VERSION=1.6.21
# Wed, 21 Jun 2023 01:08:09 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Wed, 21 Jun 2023 01:10:35 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Wed, 21 Jun 2023 01:10:35 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 21 Jun 2023 01:10:36 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 21 Jun 2023 01:10:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Jun 2023 01:10:36 GMT
USER memcache
# Wed, 21 Jun 2023 01:10:36 GMT
EXPOSE 11211
# Wed, 21 Jun 2023 01:10:36 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:8c6d1654570f041603f4cef49c320c8f6f3e401324913009d92a19132cbf1ac0`  
		Last Modified: Wed, 14 Jun 2023 20:49:23 GMT  
		Size: 3.3 MB (3329251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:666588188768f19b27fb821e02d084406af8fd867cc4595b896b9eed50b2105e`  
		Last Modified: Wed, 14 Jun 2023 21:00:51 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7d958a137d671266f063c0af4d7b0b6d44d9018b77fdbddb8fd412d3c0b1be3`  
		Last Modified: Wed, 14 Jun 2023 21:00:51 GMT  
		Size: 124.1 KB (124137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a66841dcfe05dcef1af82648941fa1ea0e10dbdf022326916d1d74afc99885c6`  
		Last Modified: Wed, 21 Jun 2023 01:11:21 GMT  
		Size: 944.3 KB (944292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b46fdc76bcbc8fa94ae23177ac32b97a4d370a630ec7d3f52bd8aae174e75982`  
		Last Modified: Wed, 21 Jun 2023 01:11:20 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea70db1a59f508c629aef54fb39ac3ada5cfcc3aac7aa1d6ed6cde22e97d3e3b`  
		Last Modified: Wed, 21 Jun 2023 01:11:20 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.21-alpine3.18` - linux; 386

```console
$ docker pull memcached@sha256:73c987449b9f764e060e2745d29e0ee50f4f7e630ddd23631c517e65f2315bfa
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.3 MB (4282253 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c47771f0d8f2ab5f38441f65fed7a05d87ea44b1de1a502321348997971362c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 14 Jun 2023 22:33:22 GMT
ADD file:94bec00e2c0c7f47c81ec4355a29ca23a81b439797d037b1a5a455f36a25dab4 in / 
# Wed, 14 Jun 2023 22:33:22 GMT
CMD ["/bin/sh"]
# Wed, 14 Jun 2023 22:38:20 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Wed, 14 Jun 2023 22:38:22 GMT
RUN apk add --no-cache libsasl
# Wed, 21 Jun 2023 00:50:52 GMT
ENV MEMCACHED_VERSION=1.6.21
# Wed, 21 Jun 2023 00:50:52 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Wed, 21 Jun 2023 00:54:21 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Wed, 21 Jun 2023 00:54:22 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 21 Jun 2023 00:54:22 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 21 Jun 2023 00:54:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Jun 2023 00:54:22 GMT
USER memcache
# Wed, 21 Jun 2023 00:54:22 GMT
EXPOSE 11211
# Wed, 21 Jun 2023 00:54:23 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:b3f50075abd13aad1cb7d8c1427aa59d7fcac88f3690d3f9c3efdbec80fd0856`  
		Last Modified: Wed, 14 Jun 2023 22:33:48 GMT  
		Size: 3.2 MB (3233951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:358673fc695429dd9142a4904a518e96c418229121d02435d875a993d9e5fac1`  
		Last Modified: Wed, 14 Jun 2023 22:42:32 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ae09e638ab1208326cbfd03f4517b0d1d13f72cfc8add3a055321fe5cf0f53a`  
		Last Modified: Wed, 14 Jun 2023 22:42:32 GMT  
		Size: 109.5 KB (109531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ed35577a5a4360f65bc0361d7bca857e45fad4baf04bcde5e731529377e9f58`  
		Last Modified: Wed, 21 Jun 2023 00:55:07 GMT  
		Size: 937.1 KB (937107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c4024dd0449592764b513374729cea0a478f62deaf32af4b23e536ffca016b6`  
		Last Modified: Wed, 21 Jun 2023 00:55:07 GMT  
		Size: 280.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6d29f640e8837bc0d0ed4b3fc505f71494f0c3ef917245b2399971ca3cb38e8`  
		Last Modified: Wed, 21 Jun 2023 00:55:06 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.21-alpine3.18` - linux; ppc64le

```console
$ docker pull memcached@sha256:e02abd3f1c109243a103019450a45039503d018c8fcd2fb607798643fbeaed69
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4453245 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7311794e1380b44e42daf3ea3c49269eb71549d5f62a46f6596478d01bda3b02`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 15 Jun 2023 00:39:49 GMT
ADD file:694c636c0dd19fd01accbc189e4c1dc4d063952692c6e7eb26dce02a7adba833 in / 
# Thu, 15 Jun 2023 00:39:49 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 04:20:00 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Thu, 15 Jun 2023 04:20:03 GMT
RUN apk add --no-cache libsasl
# Wed, 21 Jun 2023 01:42:40 GMT
ENV MEMCACHED_VERSION=1.6.21
# Wed, 21 Jun 2023 01:42:40 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Wed, 21 Jun 2023 01:45:42 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Wed, 21 Jun 2023 01:45:43 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 21 Jun 2023 01:45:45 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 21 Jun 2023 01:45:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Jun 2023 01:45:46 GMT
USER memcache
# Wed, 21 Jun 2023 01:45:46 GMT
EXPOSE 11211
# Wed, 21 Jun 2023 01:45:47 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:ffa4a466dbb8eebd7e7f25590a9df12390de9016abf82279c29c9a64aa76491a`  
		Last Modified: Thu, 15 Jun 2023 00:40:26 GMT  
		Size: 3.3 MB (3344781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:607cb6edfb2d0718375d44dbfb94d80d9b5e23a38a6bad8d2fe9c624a0ae354a`  
		Last Modified: Thu, 15 Jun 2023 04:23:36 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f97572f9bc2bc81fb5496a46ecd8b44cdb5b616d0beaecaabb186e3523683a32`  
		Last Modified: Thu, 15 Jun 2023 04:23:37 GMT  
		Size: 123.9 KB (123931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da5b2f6c7aee3051aa1b53ff9a66885509bad54b27aa37aebe382fc1ca4eab1f`  
		Last Modified: Wed, 21 Jun 2023 01:46:43 GMT  
		Size: 982.9 KB (982864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a08963a0c7d8349568389e6f7af0c7a1b55f2b0aea5d25bfa94d415fbb94af9`  
		Last Modified: Wed, 21 Jun 2023 01:46:43 GMT  
		Size: 282.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d866cc948bf60127d37a1f655a84d6b9c17376a21656e660c47efc6d3f499ba2`  
		Last Modified: Wed, 21 Jun 2023 01:46:43 GMT  
		Size: 118.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.21-alpine3.18` - linux; s390x

```console
$ docker pull memcached@sha256:cd97d93e79c2345a0c10f20a912f29a0ccf5590e15c00df81596397b9567233f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.3 MB (4278263 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f56d14fce8cfd200c86bd00cd28c95574b6bf2863bd203e7644d44a08db84ab`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 15 Jun 2023 05:18:38 GMT
ADD file:a59beca78118ebf4f86cc1685237dc3a29a519401a70668da520beaa3d29eb7a in / 
# Thu, 15 Jun 2023 05:18:38 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 06:27:47 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Thu, 15 Jun 2023 06:27:49 GMT
RUN apk add --no-cache libsasl
# Wed, 21 Jun 2023 00:58:01 GMT
ENV MEMCACHED_VERSION=1.6.21
# Wed, 21 Jun 2023 00:58:01 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Wed, 21 Jun 2023 01:01:08 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Wed, 21 Jun 2023 01:01:09 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 21 Jun 2023 01:01:09 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 21 Jun 2023 01:01:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Jun 2023 01:01:09 GMT
USER memcache
# Wed, 21 Jun 2023 01:01:10 GMT
EXPOSE 11211
# Wed, 21 Jun 2023 01:01:10 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:998cc98447b44e5f0fe799dce691412796ba586ab22eb7c99aebf9d45f34833b`  
		Last Modified: Thu, 15 Jun 2023 05:29:38 GMT  
		Size: 3.2 MB (3213497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:156deb87465a2c5629e5ae28c2a7251d5684baea5a930cf65ff6b478de321202`  
		Last Modified: Thu, 15 Jun 2023 06:36:33 GMT  
		Size: 1.3 KB (1266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19020c60d58f4724218660e819b1b33b5d1428c3c5027492a2ee3c44228231df`  
		Last Modified: Thu, 15 Jun 2023 06:36:33 GMT  
		Size: 112.8 KB (112849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81e76f938f015ccb0b5d2915145432efbc0af21a2f4964e0c9a67bfbbe6a577e`  
		Last Modified: Wed, 21 Jun 2023 01:01:46 GMT  
		Size: 950.3 KB (950254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b613e0a69ced3425a5949c15688d493ef10d80eb28c7bb626f0c092223fe1302`  
		Last Modified: Wed, 21 Jun 2023 01:01:46 GMT  
		Size: 280.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4db4c30d38bb65cd11068e1892913b2fa04add8f27abe601485cc3b09754eb50`  
		Last Modified: Wed, 21 Jun 2023 01:01:46 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:1.6.21-bookworm`

```console
$ docker pull memcached@sha256:6d50bee6d0eaba83831fead39d52d67ede2aefc3acf69a19d503a9488234e1c8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 7
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; s390x

### `memcached:1.6.21-bookworm` - linux; amd64

```console
$ docker pull memcached@sha256:37d77084cbe7c98854989a68a18f22dd677379de8ffc9ee92fbf7b88b2b4d0f9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.0 MB (38973142 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a4d0c1490511995c15a4c1ca7c8413337bed068ea95507aae882010b051ca37e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 12 Jun 2023 23:20:42 GMT
ADD file:ba1250b6ecd5dd09d4914189d72741c2817988994e7da514bf62be439a34bdb5 in / 
# Mon, 12 Jun 2023 23:20:42 GMT
CMD ["bash"]
# Wed, 14 Jun 2023 20:48:19 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 14 Jun 2023 20:48:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 21 Jun 2023 01:04:34 GMT
ENV MEMCACHED_VERSION=1.6.21
# Wed, 21 Jun 2023 01:04:35 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Wed, 21 Jun 2023 01:07:04 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 21 Jun 2023 01:07:04 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 21 Jun 2023 01:07:04 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 21 Jun 2023 01:07:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Jun 2023 01:07:05 GMT
USER memcache
# Wed, 21 Jun 2023 01:07:05 GMT
EXPOSE 11211
# Wed, 21 Jun 2023 01:07:05 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:5b5fe70539cd6989aa19f25826309f9715a9489cf1c057982d6a84c1ad8975c7`  
		Last Modified: Mon, 12 Jun 2023 23:25:49 GMT  
		Size: 29.1 MB (29124744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab209434009a85e82d99c0547bb947940f9e1002ce6e965417396ee22a6820db`  
		Last Modified: Wed, 14 Jun 2023 20:53:33 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2f4dfc49c9cdae8d4df855de7cc0460e5db8c762e73786d4f8fa4f69ba11d6d`  
		Last Modified: Wed, 14 Jun 2023 20:53:33 GMT  
		Size: 2.7 MB (2677239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d5a41694f99632bb3a7c624dab437c8a10e54b92965de823e717f5c12326b1e`  
		Last Modified: Wed, 21 Jun 2023 01:09:52 GMT  
		Size: 7.2 MB (7169627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2be3d7709e1978d4b030abdf5ac129b97f21e09bb489932628899d96288a4a9`  
		Last Modified: Wed, 21 Jun 2023 01:09:50 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8cba3f7cc400544285611f46bbdba004587f84511783fd05aa6562e9337928f`  
		Last Modified: Wed, 21 Jun 2023 01:09:50 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.21-bookworm` - linux; arm variant v5

```console
$ docker pull memcached@sha256:1646b01539b9482149379208acae5c0af1c5aed3aa9d818e8748410e15170943
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.1 MB (35094759 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ad4aa07800c4cf602e699a614c04d8fa80a8617828cfeb89fc05b49791d07e7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 12 Jun 2023 23:48:31 GMT
ADD file:54a716f17b23e4fa49d1d5c0a7f63becc295873c116d19bb4753d34f1ca6affb in / 
# Mon, 12 Jun 2023 23:48:31 GMT
CMD ["bash"]
# Wed, 14 Jun 2023 21:56:18 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 14 Jun 2023 21:56:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 21 Jun 2023 00:52:38 GMT
ENV MEMCACHED_VERSION=1.6.21
# Wed, 21 Jun 2023 00:52:39 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Wed, 21 Jun 2023 00:55:49 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 21 Jun 2023 00:55:49 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 21 Jun 2023 00:55:50 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 21 Jun 2023 00:55:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Jun 2023 00:55:50 GMT
USER memcache
# Wed, 21 Jun 2023 00:55:50 GMT
EXPOSE 11211
# Wed, 21 Jun 2023 00:55:50 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:70c60174b18d99741c33011138b5abf2f4d8eca0384521ccb43db3612078e36f`  
		Last Modified: Mon, 12 Jun 2023 23:51:26 GMT  
		Size: 27.0 MB (26982142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52495c3de01d54b61ec15cd608d6ce2ae4587ca764248265b02cb108f790d5a0`  
		Last Modified: Wed, 14 Jun 2023 22:00:39 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:597daa329781ff62c0581a1a2164e04dd294d665a91e97a05aa46fe3d8765eac`  
		Last Modified: Wed, 14 Jun 2023 22:00:40 GMT  
		Size: 2.3 MB (2281778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d65590b8b7bf9398f99bf1baba8d91966081bdc70d61b0165036ac0d16b3b2f`  
		Last Modified: Wed, 21 Jun 2023 00:56:10 GMT  
		Size: 5.8 MB (5829307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dfab31ab9e5a7944b95a42de61a2d1d591fa1605d1a6e2724f9b2c72f03f1ff`  
		Last Modified: Wed, 21 Jun 2023 00:56:09 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85b6795c5e090ce84e068ec9cb629871f3a70380f1bff62aa7baa8a0783343d2`  
		Last Modified: Wed, 21 Jun 2023 00:56:09 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.21-bookworm` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:d82fec3f72f254431725dc57a8b8922cfb269e018b4407c9e7abb133083b1b32
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.9 MB (37872901 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b25fcbe4e1c3b4ce20a4e4994a494fe7a0d98500c1b5b14f4b92c104898a434c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 04 Jul 2023 01:57:35 GMT
ADD file:71fd66666294148382f2e6a09ae5e277d4c4e9c74402ab64b693a79387b67a09 in / 
# Tue, 04 Jul 2023 01:57:36 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 06:40:00 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 04 Jul 2023 06:40:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 06:40:03 GMT
ENV MEMCACHED_VERSION=1.6.21
# Tue, 04 Jul 2023 06:40:03 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Tue, 04 Jul 2023 06:42:47 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 04 Jul 2023 06:42:47 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 04 Jul 2023 06:42:48 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 04 Jul 2023 06:42:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Jul 2023 06:42:48 GMT
USER memcache
# Tue, 04 Jul 2023 06:42:48 GMT
EXPOSE 11211
# Tue, 04 Jul 2023 06:42:48 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:3ae0c06b4d3aa97d7e0829233dd36cea1666b87074e55fea6bd1ecae066693c7`  
		Last Modified: Tue, 04 Jul 2023 02:01:20 GMT  
		Size: 29.2 MB (29152458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7e0b4333d4768ee800aa733f63a51c54833abe7bd20188154f0869796bb3f8c`  
		Last Modified: Tue, 04 Jul 2023 06:43:03 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fd0e2a70b071a1504381d7831ed736d40261b75692a2fe4ee547186e80ad9b2`  
		Last Modified: Tue, 04 Jul 2023 06:43:03 GMT  
		Size: 2.5 MB (2539167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:382aa3014b4367d16a225a23e5195af1f3a5e51523f9d89461e4b98ddf61aa3d`  
		Last Modified: Tue, 04 Jul 2023 06:43:04 GMT  
		Size: 6.2 MB (6179743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4abaeb5f633e1c888b605fe890a58e527c62021db2516cd8606edad49e9500c0`  
		Last Modified: Tue, 04 Jul 2023 06:43:03 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aedc2da2773982e3f9627ea96874aec7c38a4288cca37a366f29392750f7c38`  
		Last Modified: Tue, 04 Jul 2023 06:43:03 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.21-bookworm` - linux; 386

```console
$ docker pull memcached@sha256:d275ff7e4cd6b5d699c14115419af7ae2c1bfa32312282ff8c9ba0b424cf6be0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.5 MB (39457503 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8785d2e661831af23d884d73d3196f416198d2c57ffa24c50c8cafe16c0da224`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 12 Jun 2023 23:39:20 GMT
ADD file:c7ecc5e2bed99e2cbca26f9f4247cd9bc399749556f4084e9357a9b00bb80530 in / 
# Mon, 12 Jun 2023 23:39:20 GMT
CMD ["bash"]
# Wed, 14 Jun 2023 22:34:28 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 14 Jun 2023 22:34:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 21 Jun 2023 00:46:59 GMT
ENV MEMCACHED_VERSION=1.6.21
# Wed, 21 Jun 2023 00:46:59 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Wed, 21 Jun 2023 00:50:45 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 21 Jun 2023 00:50:45 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 21 Jun 2023 00:50:46 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 21 Jun 2023 00:50:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Jun 2023 00:50:46 GMT
USER memcache
# Wed, 21 Jun 2023 00:50:46 GMT
EXPOSE 11211
# Wed, 21 Jun 2023 00:50:46 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:82a41d17956dd7c8ebb39c9ce936fd26841bdbec98d0a185e3db8154b352edff`  
		Last Modified: Mon, 12 Jun 2023 23:46:21 GMT  
		Size: 30.1 MB (30140741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:039125a8cebc58c43be503e98831cac166a973cb3e68f4b66194142680e76964`  
		Last Modified: Wed, 14 Jun 2023 22:42:09 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:199b04439aa2a5065d0c23f986eccd0dd093be2f49b180b332af4f35d977ab5b`  
		Last Modified: Wed, 14 Jun 2023 22:42:09 GMT  
		Size: 2.7 MB (2685017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e58126d70102e38c764aa423066a897bc811895dc85b8d607eadfcff947049a7`  
		Last Modified: Wed, 21 Jun 2023 00:54:46 GMT  
		Size: 6.6 MB (6630215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b039c50c059c1c3a231a9659c8ade08b537d8ecac9423685ba16cf308626c4e4`  
		Last Modified: Wed, 21 Jun 2023 00:54:44 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1d3e144a63d04f26029dacd020e1ec00baeae59c5cee460a482e70842be2fc2`  
		Last Modified: Wed, 21 Jun 2023 00:54:44 GMT  
		Size: 116.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.21-bookworm` - linux; mips64le

```console
$ docker pull memcached@sha256:76620bca6f37fb4a82e0cc3aa33ba7cc2508c8f93dd4ae4956e9b471ce0995a2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.6 MB (37554107 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f8424fcd7f4d7db2c883a9303136b4305e34813630a9e325332ee830d35c026d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 13 Jun 2023 00:09:02 GMT
ADD file:f91bd2a174259cb69646fc34ba2fc6b8941ad8e171d2d7952a4d8ac3d95e2ad7 in / 
# Tue, 13 Jun 2023 00:09:06 GMT
CMD ["bash"]
# Wed, 14 Jun 2023 18:38:15 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 14 Jun 2023 18:38:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 21 Jun 2023 01:14:52 GMT
ENV MEMCACHED_VERSION=1.6.21
# Wed, 21 Jun 2023 01:14:54 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Wed, 21 Jun 2023 01:21:45 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 21 Jun 2023 01:21:47 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 21 Jun 2023 01:21:52 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 21 Jun 2023 01:21:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Jun 2023 01:21:57 GMT
USER memcache
# Wed, 21 Jun 2023 01:22:00 GMT
EXPOSE 11211
# Wed, 21 Jun 2023 01:22:02 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:3fc28260a4d871ef9781cad2bb064ad7212a5063de3a1d35dba938ce82115e5b`  
		Last Modified: Tue, 13 Jun 2023 00:22:29 GMT  
		Size: 29.1 MB (29118129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79c804aeb794275ae845d32d2939d0e0fefa75cd112f1075aaf2104097050ae8`  
		Last Modified: Wed, 14 Jun 2023 18:46:04 GMT  
		Size: 1.1 KB (1078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf29fcbe26928e2f4086a889098220505bdd4401dc87958f623ade0618efcd28`  
		Last Modified: Wed, 14 Jun 2023 18:46:05 GMT  
		Size: 1.9 MB (1934899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1d2070a6fd2a146f7a7ccda5a6b5c9e7188304b3eb6ad56e85ae5e13af6efff`  
		Last Modified: Wed, 21 Jun 2023 01:22:36 GMT  
		Size: 6.5 MB (6499598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb2d53b7e662ee08ffe5d3ff1b97e2bbec271b2427e8428d38ab879c1a68cbdd`  
		Last Modified: Wed, 21 Jun 2023 01:22:31 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e13b007130a18104c8ce3a24f68b588c6ec439dcb4c22e430edf1baab337bb13`  
		Last Modified: Wed, 21 Jun 2023 01:22:31 GMT  
		Size: 118.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.21-bookworm` - linux; ppc64le

```console
$ docker pull memcached@sha256:0466889ea7a59c3e5075122e0dfac5f9fd4b740dbc54d7ca3355e661704b7df3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.2 MB (43193731 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f99a2d51677ef27121ea5fb73098453983811a697bb67558da1548d6a2b1a4d7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 04 Jul 2023 01:17:51 GMT
ADD file:51887002f5002ccc662adbc6ecf1129e3db375a7a77b93da43cc9a8326b3c4b9 in / 
# Tue, 04 Jul 2023 01:17:53 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 06:45:59 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 04 Jul 2023 06:46:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 06:46:11 GMT
ENV MEMCACHED_VERSION=1.6.21
# Tue, 04 Jul 2023 06:46:12 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Tue, 04 Jul 2023 06:50:32 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 04 Jul 2023 06:50:34 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 04 Jul 2023 06:50:36 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 04 Jul 2023 06:50:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Jul 2023 06:50:36 GMT
USER memcache
# Tue, 04 Jul 2023 06:50:37 GMT
EXPOSE 11211
# Tue, 04 Jul 2023 06:50:37 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:ba99a1aa5a92d949d988e66df7723a542fd81bc30eef9d4269e8a899820d4bb2`  
		Last Modified: Tue, 04 Jul 2023 01:24:36 GMT  
		Size: 33.1 MB (33116716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57bc245122d94a5d6dbd04e3f0d2cc3731cb7e5479f873ad6588885b1a1e7fff`  
		Last Modified: Tue, 04 Jul 2023 06:51:13 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8302634866fb43cf1942126242ebd186c7a31db3f01e63b626c2c6cb31aa01bb`  
		Last Modified: Tue, 04 Jul 2023 06:51:14 GMT  
		Size: 2.9 MB (2891325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85b07e92e6621b42a17464a214cee12ada2ca5c70c139194a0d9d5cdf753e470`  
		Last Modified: Tue, 04 Jul 2023 06:51:16 GMT  
		Size: 7.2 MB (7184153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:060e182005428d5f8ae46505c71da839515e43c949a2109682b933781ad7b42d`  
		Last Modified: Tue, 04 Jul 2023 06:51:13 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd71a227a79337edf4a41188a95ac6c897f53d5cc1ebfa6201b14525057ce473`  
		Last Modified: Tue, 04 Jul 2023 06:51:13 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.21-bookworm` - linux; s390x

```console
$ docker pull memcached@sha256:f90935a3646db47ef74efba3a8ea148e6fa9a6058557fd686664b3a9b83cf5b4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.9 MB (35907614 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:55f50234cc8836dd1977a706a4d7845c857ac2128081a776c895db012f73e5bb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 13 Jun 2023 04:29:41 GMT
ADD file:739f4c23557ec0af5f4ba492c847b5d2f09dd81211c675d0e9eabe865d794e81 in / 
# Tue, 13 Jun 2023 04:29:43 GMT
CMD ["bash"]
# Thu, 15 Jun 2023 06:23:25 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Thu, 15 Jun 2023 06:23:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 21 Jun 2023 00:54:39 GMT
ENV MEMCACHED_VERSION=1.6.21
# Wed, 21 Jun 2023 00:54:39 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Wed, 21 Jun 2023 00:57:46 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 21 Jun 2023 00:57:47 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 21 Jun 2023 00:57:47 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 21 Jun 2023 00:57:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Jun 2023 00:57:47 GMT
USER memcache
# Wed, 21 Jun 2023 00:57:47 GMT
EXPOSE 11211
# Wed, 21 Jun 2023 00:57:48 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:6571b3abd058e377c7bd231c9029aff6eb25486bffb50229076d2e6a356a517f`  
		Last Modified: Tue, 13 Jun 2023 04:34:21 GMT  
		Size: 27.5 MB (27487928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1521043364f590f749ce68598ad1f79907ef04ee2283314cfaab3f72df8e15c`  
		Last Modified: Thu, 15 Jun 2023 06:35:17 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdbc1e75c128be037526f9b133061f5dc6c9baf2f00b5d5b229427bd89eb55b7`  
		Last Modified: Thu, 15 Jun 2023 06:35:18 GMT  
		Size: 2.3 MB (2345340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f3d048c5c76c19c7c7d783cac8384f5698dd61a6aa7ee9067521407789ec9b4`  
		Last Modified: Wed, 21 Jun 2023 01:01:34 GMT  
		Size: 6.1 MB (6072815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c7bfbb7d1965d17408766d01c40f67a94eb422714618a239a48b62cedafdcab`  
		Last Modified: Wed, 21 Jun 2023 01:01:33 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:164d3c9aaa0239a91376552d50ffc16a1e2bf9e3c323e81d2a976556ab25f4a2`  
		Last Modified: Wed, 21 Jun 2023 01:01:33 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:alpine`

```console
$ docker pull memcached@sha256:32f2ba37c2ed2ef922efa0190faa71dc3b4f1df4a3e50938a0b3afe3d589a1d9
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
$ docker pull memcached@sha256:574ef430513a38925cc52ae5954677a12e0a57205fed96be5707196a180e5159
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4462428 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f7da63106561ab1f7284992dad2396b234096070b4269971b23c53f2f8498ef`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 14 Jun 2023 20:41:58 GMT
ADD file:1da756d12551a0e3e793e02ef87432d69d4968937bd11bed0af215db19dd94cd in / 
# Wed, 14 Jun 2023 20:41:59 GMT
CMD ["/bin/sh"]
# Wed, 14 Jun 2023 20:50:58 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Wed, 14 Jun 2023 20:50:59 GMT
RUN apk add --no-cache libsasl
# Wed, 21 Jun 2023 01:07:13 GMT
ENV MEMCACHED_VERSION=1.6.21
# Wed, 21 Jun 2023 01:07:13 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Wed, 21 Jun 2023 01:09:21 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Wed, 21 Jun 2023 01:09:21 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 21 Jun 2023 01:09:22 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 21 Jun 2023 01:09:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Jun 2023 01:09:22 GMT
USER memcache
# Wed, 21 Jun 2023 01:09:22 GMT
EXPOSE 11211
# Wed, 21 Jun 2023 01:09:22 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:31e352740f534f9ad170f75378a84fe453d6156e40700b882d737a8f4a6988a3`  
		Last Modified: Wed, 14 Jun 2023 20:42:26 GMT  
		Size: 3.4 MB (3397879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b2b2df106c5026cd33ea4ac655b77f25410ec9f4b8a6756ebc1ceeb79fca3c7`  
		Last Modified: Wed, 14 Jun 2023 20:53:58 GMT  
		Size: 1.3 KB (1266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed63668528d3e2159f55909c66dc48a6f746ce24c2e2f6d963b992aefaa457ce`  
		Last Modified: Wed, 14 Jun 2023 20:53:58 GMT  
		Size: 108.1 KB (108080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05536f2f26c904a5aa1b07720957a37e8b57a223725d76f8d1473dcab297a233`  
		Last Modified: Wed, 21 Jun 2023 01:10:14 GMT  
		Size: 954.8 KB (954811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e448b573a98adc8bd0a4805cb0e1b451aea0d1582f0462aa0b147799a97fad7`  
		Last Modified: Wed, 21 Jun 2023 01:10:13 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3029a709b7be20aeff1e9cebe5c6112cd1df5a0ea3efb58e61380cc75b9296e`  
		Last Modified: Wed, 21 Jun 2023 01:10:13 GMT  
		Size: 117.0 B  
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
$ docker pull memcached@sha256:eb4b801b9c9e9af6565ac003b21af39b06d55943bbc4e59a02d465fdf7f07776
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.4 MB (4399342 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4aa99dd98a2fa001241d907951530f4afebadfd4895545c5d73f31e29b7a35fa`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 14 Jun 2023 20:48:58 GMT
ADD file:289c2fac17119508ced527225d445747cd177111b4a0018a6b04948ecb3b5e29 in / 
# Wed, 14 Jun 2023 20:48:58 GMT
CMD ["/bin/sh"]
# Wed, 14 Jun 2023 20:57:26 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Wed, 14 Jun 2023 20:57:27 GMT
RUN apk add --no-cache libsasl
# Wed, 21 Jun 2023 01:08:09 GMT
ENV MEMCACHED_VERSION=1.6.21
# Wed, 21 Jun 2023 01:08:09 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Wed, 21 Jun 2023 01:10:35 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Wed, 21 Jun 2023 01:10:35 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 21 Jun 2023 01:10:36 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 21 Jun 2023 01:10:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Jun 2023 01:10:36 GMT
USER memcache
# Wed, 21 Jun 2023 01:10:36 GMT
EXPOSE 11211
# Wed, 21 Jun 2023 01:10:36 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:8c6d1654570f041603f4cef49c320c8f6f3e401324913009d92a19132cbf1ac0`  
		Last Modified: Wed, 14 Jun 2023 20:49:23 GMT  
		Size: 3.3 MB (3329251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:666588188768f19b27fb821e02d084406af8fd867cc4595b896b9eed50b2105e`  
		Last Modified: Wed, 14 Jun 2023 21:00:51 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7d958a137d671266f063c0af4d7b0b6d44d9018b77fdbddb8fd412d3c0b1be3`  
		Last Modified: Wed, 14 Jun 2023 21:00:51 GMT  
		Size: 124.1 KB (124137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a66841dcfe05dcef1af82648941fa1ea0e10dbdf022326916d1d74afc99885c6`  
		Last Modified: Wed, 21 Jun 2023 01:11:21 GMT  
		Size: 944.3 KB (944292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b46fdc76bcbc8fa94ae23177ac32b97a4d370a630ec7d3f52bd8aae174e75982`  
		Last Modified: Wed, 21 Jun 2023 01:11:20 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea70db1a59f508c629aef54fb39ac3ada5cfcc3aac7aa1d6ed6cde22e97d3e3b`  
		Last Modified: Wed, 21 Jun 2023 01:11:20 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:alpine` - linux; 386

```console
$ docker pull memcached@sha256:73c987449b9f764e060e2745d29e0ee50f4f7e630ddd23631c517e65f2315bfa
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.3 MB (4282253 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c47771f0d8f2ab5f38441f65fed7a05d87ea44b1de1a502321348997971362c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 14 Jun 2023 22:33:22 GMT
ADD file:94bec00e2c0c7f47c81ec4355a29ca23a81b439797d037b1a5a455f36a25dab4 in / 
# Wed, 14 Jun 2023 22:33:22 GMT
CMD ["/bin/sh"]
# Wed, 14 Jun 2023 22:38:20 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Wed, 14 Jun 2023 22:38:22 GMT
RUN apk add --no-cache libsasl
# Wed, 21 Jun 2023 00:50:52 GMT
ENV MEMCACHED_VERSION=1.6.21
# Wed, 21 Jun 2023 00:50:52 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Wed, 21 Jun 2023 00:54:21 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Wed, 21 Jun 2023 00:54:22 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 21 Jun 2023 00:54:22 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 21 Jun 2023 00:54:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Jun 2023 00:54:22 GMT
USER memcache
# Wed, 21 Jun 2023 00:54:22 GMT
EXPOSE 11211
# Wed, 21 Jun 2023 00:54:23 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:b3f50075abd13aad1cb7d8c1427aa59d7fcac88f3690d3f9c3efdbec80fd0856`  
		Last Modified: Wed, 14 Jun 2023 22:33:48 GMT  
		Size: 3.2 MB (3233951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:358673fc695429dd9142a4904a518e96c418229121d02435d875a993d9e5fac1`  
		Last Modified: Wed, 14 Jun 2023 22:42:32 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ae09e638ab1208326cbfd03f4517b0d1d13f72cfc8add3a055321fe5cf0f53a`  
		Last Modified: Wed, 14 Jun 2023 22:42:32 GMT  
		Size: 109.5 KB (109531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ed35577a5a4360f65bc0361d7bca857e45fad4baf04bcde5e731529377e9f58`  
		Last Modified: Wed, 21 Jun 2023 00:55:07 GMT  
		Size: 937.1 KB (937107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c4024dd0449592764b513374729cea0a478f62deaf32af4b23e536ffca016b6`  
		Last Modified: Wed, 21 Jun 2023 00:55:07 GMT  
		Size: 280.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6d29f640e8837bc0d0ed4b3fc505f71494f0c3ef917245b2399971ca3cb38e8`  
		Last Modified: Wed, 21 Jun 2023 00:55:06 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:alpine` - linux; ppc64le

```console
$ docker pull memcached@sha256:e02abd3f1c109243a103019450a45039503d018c8fcd2fb607798643fbeaed69
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4453245 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7311794e1380b44e42daf3ea3c49269eb71549d5f62a46f6596478d01bda3b02`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 15 Jun 2023 00:39:49 GMT
ADD file:694c636c0dd19fd01accbc189e4c1dc4d063952692c6e7eb26dce02a7adba833 in / 
# Thu, 15 Jun 2023 00:39:49 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 04:20:00 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Thu, 15 Jun 2023 04:20:03 GMT
RUN apk add --no-cache libsasl
# Wed, 21 Jun 2023 01:42:40 GMT
ENV MEMCACHED_VERSION=1.6.21
# Wed, 21 Jun 2023 01:42:40 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Wed, 21 Jun 2023 01:45:42 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Wed, 21 Jun 2023 01:45:43 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 21 Jun 2023 01:45:45 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 21 Jun 2023 01:45:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Jun 2023 01:45:46 GMT
USER memcache
# Wed, 21 Jun 2023 01:45:46 GMT
EXPOSE 11211
# Wed, 21 Jun 2023 01:45:47 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:ffa4a466dbb8eebd7e7f25590a9df12390de9016abf82279c29c9a64aa76491a`  
		Last Modified: Thu, 15 Jun 2023 00:40:26 GMT  
		Size: 3.3 MB (3344781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:607cb6edfb2d0718375d44dbfb94d80d9b5e23a38a6bad8d2fe9c624a0ae354a`  
		Last Modified: Thu, 15 Jun 2023 04:23:36 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f97572f9bc2bc81fb5496a46ecd8b44cdb5b616d0beaecaabb186e3523683a32`  
		Last Modified: Thu, 15 Jun 2023 04:23:37 GMT  
		Size: 123.9 KB (123931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da5b2f6c7aee3051aa1b53ff9a66885509bad54b27aa37aebe382fc1ca4eab1f`  
		Last Modified: Wed, 21 Jun 2023 01:46:43 GMT  
		Size: 982.9 KB (982864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a08963a0c7d8349568389e6f7af0c7a1b55f2b0aea5d25bfa94d415fbb94af9`  
		Last Modified: Wed, 21 Jun 2023 01:46:43 GMT  
		Size: 282.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d866cc948bf60127d37a1f655a84d6b9c17376a21656e660c47efc6d3f499ba2`  
		Last Modified: Wed, 21 Jun 2023 01:46:43 GMT  
		Size: 118.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:alpine` - linux; s390x

```console
$ docker pull memcached@sha256:cd97d93e79c2345a0c10f20a912f29a0ccf5590e15c00df81596397b9567233f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.3 MB (4278263 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f56d14fce8cfd200c86bd00cd28c95574b6bf2863bd203e7644d44a08db84ab`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 15 Jun 2023 05:18:38 GMT
ADD file:a59beca78118ebf4f86cc1685237dc3a29a519401a70668da520beaa3d29eb7a in / 
# Thu, 15 Jun 2023 05:18:38 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 06:27:47 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Thu, 15 Jun 2023 06:27:49 GMT
RUN apk add --no-cache libsasl
# Wed, 21 Jun 2023 00:58:01 GMT
ENV MEMCACHED_VERSION=1.6.21
# Wed, 21 Jun 2023 00:58:01 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Wed, 21 Jun 2023 01:01:08 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Wed, 21 Jun 2023 01:01:09 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 21 Jun 2023 01:01:09 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 21 Jun 2023 01:01:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Jun 2023 01:01:09 GMT
USER memcache
# Wed, 21 Jun 2023 01:01:10 GMT
EXPOSE 11211
# Wed, 21 Jun 2023 01:01:10 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:998cc98447b44e5f0fe799dce691412796ba586ab22eb7c99aebf9d45f34833b`  
		Last Modified: Thu, 15 Jun 2023 05:29:38 GMT  
		Size: 3.2 MB (3213497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:156deb87465a2c5629e5ae28c2a7251d5684baea5a930cf65ff6b478de321202`  
		Last Modified: Thu, 15 Jun 2023 06:36:33 GMT  
		Size: 1.3 KB (1266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19020c60d58f4724218660e819b1b33b5d1428c3c5027492a2ee3c44228231df`  
		Last Modified: Thu, 15 Jun 2023 06:36:33 GMT  
		Size: 112.8 KB (112849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81e76f938f015ccb0b5d2915145432efbc0af21a2f4964e0c9a67bfbbe6a577e`  
		Last Modified: Wed, 21 Jun 2023 01:01:46 GMT  
		Size: 950.3 KB (950254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b613e0a69ced3425a5949c15688d493ef10d80eb28c7bb626f0c092223fe1302`  
		Last Modified: Wed, 21 Jun 2023 01:01:46 GMT  
		Size: 280.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4db4c30d38bb65cd11068e1892913b2fa04add8f27abe601485cc3b09754eb50`  
		Last Modified: Wed, 21 Jun 2023 01:01:46 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:alpine3.18`

```console
$ docker pull memcached@sha256:ee437fd9a952b48de768cd5c7a97d43439e05b918e4bc4452e296e8bdafae046
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `memcached:alpine3.18` - linux; amd64

```console
$ docker pull memcached@sha256:574ef430513a38925cc52ae5954677a12e0a57205fed96be5707196a180e5159
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4462428 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f7da63106561ab1f7284992dad2396b234096070b4269971b23c53f2f8498ef`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 14 Jun 2023 20:41:58 GMT
ADD file:1da756d12551a0e3e793e02ef87432d69d4968937bd11bed0af215db19dd94cd in / 
# Wed, 14 Jun 2023 20:41:59 GMT
CMD ["/bin/sh"]
# Wed, 14 Jun 2023 20:50:58 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Wed, 14 Jun 2023 20:50:59 GMT
RUN apk add --no-cache libsasl
# Wed, 21 Jun 2023 01:07:13 GMT
ENV MEMCACHED_VERSION=1.6.21
# Wed, 21 Jun 2023 01:07:13 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Wed, 21 Jun 2023 01:09:21 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Wed, 21 Jun 2023 01:09:21 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 21 Jun 2023 01:09:22 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 21 Jun 2023 01:09:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Jun 2023 01:09:22 GMT
USER memcache
# Wed, 21 Jun 2023 01:09:22 GMT
EXPOSE 11211
# Wed, 21 Jun 2023 01:09:22 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:31e352740f534f9ad170f75378a84fe453d6156e40700b882d737a8f4a6988a3`  
		Last Modified: Wed, 14 Jun 2023 20:42:26 GMT  
		Size: 3.4 MB (3397879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b2b2df106c5026cd33ea4ac655b77f25410ec9f4b8a6756ebc1ceeb79fca3c7`  
		Last Modified: Wed, 14 Jun 2023 20:53:58 GMT  
		Size: 1.3 KB (1266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed63668528d3e2159f55909c66dc48a6f746ce24c2e2f6d963b992aefaa457ce`  
		Last Modified: Wed, 14 Jun 2023 20:53:58 GMT  
		Size: 108.1 KB (108080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05536f2f26c904a5aa1b07720957a37e8b57a223725d76f8d1473dcab297a233`  
		Last Modified: Wed, 21 Jun 2023 01:10:14 GMT  
		Size: 954.8 KB (954811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e448b573a98adc8bd0a4805cb0e1b451aea0d1582f0462aa0b147799a97fad7`  
		Last Modified: Wed, 21 Jun 2023 01:10:13 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3029a709b7be20aeff1e9cebe5c6112cd1df5a0ea3efb58e61380cc75b9296e`  
		Last Modified: Wed, 21 Jun 2023 01:10:13 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:alpine3.18` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:eb4b801b9c9e9af6565ac003b21af39b06d55943bbc4e59a02d465fdf7f07776
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.4 MB (4399342 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4aa99dd98a2fa001241d907951530f4afebadfd4895545c5d73f31e29b7a35fa`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 14 Jun 2023 20:48:58 GMT
ADD file:289c2fac17119508ced527225d445747cd177111b4a0018a6b04948ecb3b5e29 in / 
# Wed, 14 Jun 2023 20:48:58 GMT
CMD ["/bin/sh"]
# Wed, 14 Jun 2023 20:57:26 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Wed, 14 Jun 2023 20:57:27 GMT
RUN apk add --no-cache libsasl
# Wed, 21 Jun 2023 01:08:09 GMT
ENV MEMCACHED_VERSION=1.6.21
# Wed, 21 Jun 2023 01:08:09 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Wed, 21 Jun 2023 01:10:35 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Wed, 21 Jun 2023 01:10:35 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 21 Jun 2023 01:10:36 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 21 Jun 2023 01:10:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Jun 2023 01:10:36 GMT
USER memcache
# Wed, 21 Jun 2023 01:10:36 GMT
EXPOSE 11211
# Wed, 21 Jun 2023 01:10:36 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:8c6d1654570f041603f4cef49c320c8f6f3e401324913009d92a19132cbf1ac0`  
		Last Modified: Wed, 14 Jun 2023 20:49:23 GMT  
		Size: 3.3 MB (3329251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:666588188768f19b27fb821e02d084406af8fd867cc4595b896b9eed50b2105e`  
		Last Modified: Wed, 14 Jun 2023 21:00:51 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7d958a137d671266f063c0af4d7b0b6d44d9018b77fdbddb8fd412d3c0b1be3`  
		Last Modified: Wed, 14 Jun 2023 21:00:51 GMT  
		Size: 124.1 KB (124137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a66841dcfe05dcef1af82648941fa1ea0e10dbdf022326916d1d74afc99885c6`  
		Last Modified: Wed, 21 Jun 2023 01:11:21 GMT  
		Size: 944.3 KB (944292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b46fdc76bcbc8fa94ae23177ac32b97a4d370a630ec7d3f52bd8aae174e75982`  
		Last Modified: Wed, 21 Jun 2023 01:11:20 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea70db1a59f508c629aef54fb39ac3ada5cfcc3aac7aa1d6ed6cde22e97d3e3b`  
		Last Modified: Wed, 21 Jun 2023 01:11:20 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:alpine3.18` - linux; 386

```console
$ docker pull memcached@sha256:73c987449b9f764e060e2745d29e0ee50f4f7e630ddd23631c517e65f2315bfa
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.3 MB (4282253 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c47771f0d8f2ab5f38441f65fed7a05d87ea44b1de1a502321348997971362c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 14 Jun 2023 22:33:22 GMT
ADD file:94bec00e2c0c7f47c81ec4355a29ca23a81b439797d037b1a5a455f36a25dab4 in / 
# Wed, 14 Jun 2023 22:33:22 GMT
CMD ["/bin/sh"]
# Wed, 14 Jun 2023 22:38:20 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Wed, 14 Jun 2023 22:38:22 GMT
RUN apk add --no-cache libsasl
# Wed, 21 Jun 2023 00:50:52 GMT
ENV MEMCACHED_VERSION=1.6.21
# Wed, 21 Jun 2023 00:50:52 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Wed, 21 Jun 2023 00:54:21 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Wed, 21 Jun 2023 00:54:22 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 21 Jun 2023 00:54:22 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 21 Jun 2023 00:54:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Jun 2023 00:54:22 GMT
USER memcache
# Wed, 21 Jun 2023 00:54:22 GMT
EXPOSE 11211
# Wed, 21 Jun 2023 00:54:23 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:b3f50075abd13aad1cb7d8c1427aa59d7fcac88f3690d3f9c3efdbec80fd0856`  
		Last Modified: Wed, 14 Jun 2023 22:33:48 GMT  
		Size: 3.2 MB (3233951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:358673fc695429dd9142a4904a518e96c418229121d02435d875a993d9e5fac1`  
		Last Modified: Wed, 14 Jun 2023 22:42:32 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ae09e638ab1208326cbfd03f4517b0d1d13f72cfc8add3a055321fe5cf0f53a`  
		Last Modified: Wed, 14 Jun 2023 22:42:32 GMT  
		Size: 109.5 KB (109531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ed35577a5a4360f65bc0361d7bca857e45fad4baf04bcde5e731529377e9f58`  
		Last Modified: Wed, 21 Jun 2023 00:55:07 GMT  
		Size: 937.1 KB (937107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c4024dd0449592764b513374729cea0a478f62deaf32af4b23e536ffca016b6`  
		Last Modified: Wed, 21 Jun 2023 00:55:07 GMT  
		Size: 280.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6d29f640e8837bc0d0ed4b3fc505f71494f0c3ef917245b2399971ca3cb38e8`  
		Last Modified: Wed, 21 Jun 2023 00:55:06 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:alpine3.18` - linux; ppc64le

```console
$ docker pull memcached@sha256:e02abd3f1c109243a103019450a45039503d018c8fcd2fb607798643fbeaed69
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4453245 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7311794e1380b44e42daf3ea3c49269eb71549d5f62a46f6596478d01bda3b02`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 15 Jun 2023 00:39:49 GMT
ADD file:694c636c0dd19fd01accbc189e4c1dc4d063952692c6e7eb26dce02a7adba833 in / 
# Thu, 15 Jun 2023 00:39:49 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 04:20:00 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Thu, 15 Jun 2023 04:20:03 GMT
RUN apk add --no-cache libsasl
# Wed, 21 Jun 2023 01:42:40 GMT
ENV MEMCACHED_VERSION=1.6.21
# Wed, 21 Jun 2023 01:42:40 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Wed, 21 Jun 2023 01:45:42 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Wed, 21 Jun 2023 01:45:43 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 21 Jun 2023 01:45:45 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 21 Jun 2023 01:45:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Jun 2023 01:45:46 GMT
USER memcache
# Wed, 21 Jun 2023 01:45:46 GMT
EXPOSE 11211
# Wed, 21 Jun 2023 01:45:47 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:ffa4a466dbb8eebd7e7f25590a9df12390de9016abf82279c29c9a64aa76491a`  
		Last Modified: Thu, 15 Jun 2023 00:40:26 GMT  
		Size: 3.3 MB (3344781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:607cb6edfb2d0718375d44dbfb94d80d9b5e23a38a6bad8d2fe9c624a0ae354a`  
		Last Modified: Thu, 15 Jun 2023 04:23:36 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f97572f9bc2bc81fb5496a46ecd8b44cdb5b616d0beaecaabb186e3523683a32`  
		Last Modified: Thu, 15 Jun 2023 04:23:37 GMT  
		Size: 123.9 KB (123931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da5b2f6c7aee3051aa1b53ff9a66885509bad54b27aa37aebe382fc1ca4eab1f`  
		Last Modified: Wed, 21 Jun 2023 01:46:43 GMT  
		Size: 982.9 KB (982864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a08963a0c7d8349568389e6f7af0c7a1b55f2b0aea5d25bfa94d415fbb94af9`  
		Last Modified: Wed, 21 Jun 2023 01:46:43 GMT  
		Size: 282.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d866cc948bf60127d37a1f655a84d6b9c17376a21656e660c47efc6d3f499ba2`  
		Last Modified: Wed, 21 Jun 2023 01:46:43 GMT  
		Size: 118.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:alpine3.18` - linux; s390x

```console
$ docker pull memcached@sha256:cd97d93e79c2345a0c10f20a912f29a0ccf5590e15c00df81596397b9567233f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.3 MB (4278263 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f56d14fce8cfd200c86bd00cd28c95574b6bf2863bd203e7644d44a08db84ab`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 15 Jun 2023 05:18:38 GMT
ADD file:a59beca78118ebf4f86cc1685237dc3a29a519401a70668da520beaa3d29eb7a in / 
# Thu, 15 Jun 2023 05:18:38 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 06:27:47 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Thu, 15 Jun 2023 06:27:49 GMT
RUN apk add --no-cache libsasl
# Wed, 21 Jun 2023 00:58:01 GMT
ENV MEMCACHED_VERSION=1.6.21
# Wed, 21 Jun 2023 00:58:01 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Wed, 21 Jun 2023 01:01:08 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Wed, 21 Jun 2023 01:01:09 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 21 Jun 2023 01:01:09 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 21 Jun 2023 01:01:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Jun 2023 01:01:09 GMT
USER memcache
# Wed, 21 Jun 2023 01:01:10 GMT
EXPOSE 11211
# Wed, 21 Jun 2023 01:01:10 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:998cc98447b44e5f0fe799dce691412796ba586ab22eb7c99aebf9d45f34833b`  
		Last Modified: Thu, 15 Jun 2023 05:29:38 GMT  
		Size: 3.2 MB (3213497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:156deb87465a2c5629e5ae28c2a7251d5684baea5a930cf65ff6b478de321202`  
		Last Modified: Thu, 15 Jun 2023 06:36:33 GMT  
		Size: 1.3 KB (1266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19020c60d58f4724218660e819b1b33b5d1428c3c5027492a2ee3c44228231df`  
		Last Modified: Thu, 15 Jun 2023 06:36:33 GMT  
		Size: 112.8 KB (112849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81e76f938f015ccb0b5d2915145432efbc0af21a2f4964e0c9a67bfbbe6a577e`  
		Last Modified: Wed, 21 Jun 2023 01:01:46 GMT  
		Size: 950.3 KB (950254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b613e0a69ced3425a5949c15688d493ef10d80eb28c7bb626f0c092223fe1302`  
		Last Modified: Wed, 21 Jun 2023 01:01:46 GMT  
		Size: 280.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4db4c30d38bb65cd11068e1892913b2fa04add8f27abe601485cc3b09754eb50`  
		Last Modified: Wed, 21 Jun 2023 01:01:46 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:bookworm`

```console
$ docker pull memcached@sha256:6d50bee6d0eaba83831fead39d52d67ede2aefc3acf69a19d503a9488234e1c8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 7
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; s390x

### `memcached:bookworm` - linux; amd64

```console
$ docker pull memcached@sha256:37d77084cbe7c98854989a68a18f22dd677379de8ffc9ee92fbf7b88b2b4d0f9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.0 MB (38973142 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a4d0c1490511995c15a4c1ca7c8413337bed068ea95507aae882010b051ca37e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 12 Jun 2023 23:20:42 GMT
ADD file:ba1250b6ecd5dd09d4914189d72741c2817988994e7da514bf62be439a34bdb5 in / 
# Mon, 12 Jun 2023 23:20:42 GMT
CMD ["bash"]
# Wed, 14 Jun 2023 20:48:19 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 14 Jun 2023 20:48:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 21 Jun 2023 01:04:34 GMT
ENV MEMCACHED_VERSION=1.6.21
# Wed, 21 Jun 2023 01:04:35 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Wed, 21 Jun 2023 01:07:04 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 21 Jun 2023 01:07:04 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 21 Jun 2023 01:07:04 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 21 Jun 2023 01:07:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Jun 2023 01:07:05 GMT
USER memcache
# Wed, 21 Jun 2023 01:07:05 GMT
EXPOSE 11211
# Wed, 21 Jun 2023 01:07:05 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:5b5fe70539cd6989aa19f25826309f9715a9489cf1c057982d6a84c1ad8975c7`  
		Last Modified: Mon, 12 Jun 2023 23:25:49 GMT  
		Size: 29.1 MB (29124744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab209434009a85e82d99c0547bb947940f9e1002ce6e965417396ee22a6820db`  
		Last Modified: Wed, 14 Jun 2023 20:53:33 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2f4dfc49c9cdae8d4df855de7cc0460e5db8c762e73786d4f8fa4f69ba11d6d`  
		Last Modified: Wed, 14 Jun 2023 20:53:33 GMT  
		Size: 2.7 MB (2677239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d5a41694f99632bb3a7c624dab437c8a10e54b92965de823e717f5c12326b1e`  
		Last Modified: Wed, 21 Jun 2023 01:09:52 GMT  
		Size: 7.2 MB (7169627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2be3d7709e1978d4b030abdf5ac129b97f21e09bb489932628899d96288a4a9`  
		Last Modified: Wed, 21 Jun 2023 01:09:50 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8cba3f7cc400544285611f46bbdba004587f84511783fd05aa6562e9337928f`  
		Last Modified: Wed, 21 Jun 2023 01:09:50 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:bookworm` - linux; arm variant v5

```console
$ docker pull memcached@sha256:1646b01539b9482149379208acae5c0af1c5aed3aa9d818e8748410e15170943
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.1 MB (35094759 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ad4aa07800c4cf602e699a614c04d8fa80a8617828cfeb89fc05b49791d07e7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 12 Jun 2023 23:48:31 GMT
ADD file:54a716f17b23e4fa49d1d5c0a7f63becc295873c116d19bb4753d34f1ca6affb in / 
# Mon, 12 Jun 2023 23:48:31 GMT
CMD ["bash"]
# Wed, 14 Jun 2023 21:56:18 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 14 Jun 2023 21:56:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 21 Jun 2023 00:52:38 GMT
ENV MEMCACHED_VERSION=1.6.21
# Wed, 21 Jun 2023 00:52:39 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Wed, 21 Jun 2023 00:55:49 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 21 Jun 2023 00:55:49 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 21 Jun 2023 00:55:50 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 21 Jun 2023 00:55:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Jun 2023 00:55:50 GMT
USER memcache
# Wed, 21 Jun 2023 00:55:50 GMT
EXPOSE 11211
# Wed, 21 Jun 2023 00:55:50 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:70c60174b18d99741c33011138b5abf2f4d8eca0384521ccb43db3612078e36f`  
		Last Modified: Mon, 12 Jun 2023 23:51:26 GMT  
		Size: 27.0 MB (26982142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52495c3de01d54b61ec15cd608d6ce2ae4587ca764248265b02cb108f790d5a0`  
		Last Modified: Wed, 14 Jun 2023 22:00:39 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:597daa329781ff62c0581a1a2164e04dd294d665a91e97a05aa46fe3d8765eac`  
		Last Modified: Wed, 14 Jun 2023 22:00:40 GMT  
		Size: 2.3 MB (2281778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d65590b8b7bf9398f99bf1baba8d91966081bdc70d61b0165036ac0d16b3b2f`  
		Last Modified: Wed, 21 Jun 2023 00:56:10 GMT  
		Size: 5.8 MB (5829307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dfab31ab9e5a7944b95a42de61a2d1d591fa1605d1a6e2724f9b2c72f03f1ff`  
		Last Modified: Wed, 21 Jun 2023 00:56:09 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85b6795c5e090ce84e068ec9cb629871f3a70380f1bff62aa7baa8a0783343d2`  
		Last Modified: Wed, 21 Jun 2023 00:56:09 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:bookworm` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:d82fec3f72f254431725dc57a8b8922cfb269e018b4407c9e7abb133083b1b32
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.9 MB (37872901 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b25fcbe4e1c3b4ce20a4e4994a494fe7a0d98500c1b5b14f4b92c104898a434c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 04 Jul 2023 01:57:35 GMT
ADD file:71fd66666294148382f2e6a09ae5e277d4c4e9c74402ab64b693a79387b67a09 in / 
# Tue, 04 Jul 2023 01:57:36 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 06:40:00 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 04 Jul 2023 06:40:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 06:40:03 GMT
ENV MEMCACHED_VERSION=1.6.21
# Tue, 04 Jul 2023 06:40:03 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Tue, 04 Jul 2023 06:42:47 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 04 Jul 2023 06:42:47 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 04 Jul 2023 06:42:48 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 04 Jul 2023 06:42:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Jul 2023 06:42:48 GMT
USER memcache
# Tue, 04 Jul 2023 06:42:48 GMT
EXPOSE 11211
# Tue, 04 Jul 2023 06:42:48 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:3ae0c06b4d3aa97d7e0829233dd36cea1666b87074e55fea6bd1ecae066693c7`  
		Last Modified: Tue, 04 Jul 2023 02:01:20 GMT  
		Size: 29.2 MB (29152458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7e0b4333d4768ee800aa733f63a51c54833abe7bd20188154f0869796bb3f8c`  
		Last Modified: Tue, 04 Jul 2023 06:43:03 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fd0e2a70b071a1504381d7831ed736d40261b75692a2fe4ee547186e80ad9b2`  
		Last Modified: Tue, 04 Jul 2023 06:43:03 GMT  
		Size: 2.5 MB (2539167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:382aa3014b4367d16a225a23e5195af1f3a5e51523f9d89461e4b98ddf61aa3d`  
		Last Modified: Tue, 04 Jul 2023 06:43:04 GMT  
		Size: 6.2 MB (6179743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4abaeb5f633e1c888b605fe890a58e527c62021db2516cd8606edad49e9500c0`  
		Last Modified: Tue, 04 Jul 2023 06:43:03 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aedc2da2773982e3f9627ea96874aec7c38a4288cca37a366f29392750f7c38`  
		Last Modified: Tue, 04 Jul 2023 06:43:03 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:bookworm` - linux; 386

```console
$ docker pull memcached@sha256:d275ff7e4cd6b5d699c14115419af7ae2c1bfa32312282ff8c9ba0b424cf6be0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.5 MB (39457503 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8785d2e661831af23d884d73d3196f416198d2c57ffa24c50c8cafe16c0da224`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 12 Jun 2023 23:39:20 GMT
ADD file:c7ecc5e2bed99e2cbca26f9f4247cd9bc399749556f4084e9357a9b00bb80530 in / 
# Mon, 12 Jun 2023 23:39:20 GMT
CMD ["bash"]
# Wed, 14 Jun 2023 22:34:28 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 14 Jun 2023 22:34:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 21 Jun 2023 00:46:59 GMT
ENV MEMCACHED_VERSION=1.6.21
# Wed, 21 Jun 2023 00:46:59 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Wed, 21 Jun 2023 00:50:45 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 21 Jun 2023 00:50:45 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 21 Jun 2023 00:50:46 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 21 Jun 2023 00:50:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Jun 2023 00:50:46 GMT
USER memcache
# Wed, 21 Jun 2023 00:50:46 GMT
EXPOSE 11211
# Wed, 21 Jun 2023 00:50:46 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:82a41d17956dd7c8ebb39c9ce936fd26841bdbec98d0a185e3db8154b352edff`  
		Last Modified: Mon, 12 Jun 2023 23:46:21 GMT  
		Size: 30.1 MB (30140741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:039125a8cebc58c43be503e98831cac166a973cb3e68f4b66194142680e76964`  
		Last Modified: Wed, 14 Jun 2023 22:42:09 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:199b04439aa2a5065d0c23f986eccd0dd093be2f49b180b332af4f35d977ab5b`  
		Last Modified: Wed, 14 Jun 2023 22:42:09 GMT  
		Size: 2.7 MB (2685017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e58126d70102e38c764aa423066a897bc811895dc85b8d607eadfcff947049a7`  
		Last Modified: Wed, 21 Jun 2023 00:54:46 GMT  
		Size: 6.6 MB (6630215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b039c50c059c1c3a231a9659c8ade08b537d8ecac9423685ba16cf308626c4e4`  
		Last Modified: Wed, 21 Jun 2023 00:54:44 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1d3e144a63d04f26029dacd020e1ec00baeae59c5cee460a482e70842be2fc2`  
		Last Modified: Wed, 21 Jun 2023 00:54:44 GMT  
		Size: 116.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:bookworm` - linux; mips64le

```console
$ docker pull memcached@sha256:76620bca6f37fb4a82e0cc3aa33ba7cc2508c8f93dd4ae4956e9b471ce0995a2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.6 MB (37554107 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f8424fcd7f4d7db2c883a9303136b4305e34813630a9e325332ee830d35c026d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 13 Jun 2023 00:09:02 GMT
ADD file:f91bd2a174259cb69646fc34ba2fc6b8941ad8e171d2d7952a4d8ac3d95e2ad7 in / 
# Tue, 13 Jun 2023 00:09:06 GMT
CMD ["bash"]
# Wed, 14 Jun 2023 18:38:15 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 14 Jun 2023 18:38:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 21 Jun 2023 01:14:52 GMT
ENV MEMCACHED_VERSION=1.6.21
# Wed, 21 Jun 2023 01:14:54 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Wed, 21 Jun 2023 01:21:45 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 21 Jun 2023 01:21:47 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 21 Jun 2023 01:21:52 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 21 Jun 2023 01:21:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Jun 2023 01:21:57 GMT
USER memcache
# Wed, 21 Jun 2023 01:22:00 GMT
EXPOSE 11211
# Wed, 21 Jun 2023 01:22:02 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:3fc28260a4d871ef9781cad2bb064ad7212a5063de3a1d35dba938ce82115e5b`  
		Last Modified: Tue, 13 Jun 2023 00:22:29 GMT  
		Size: 29.1 MB (29118129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79c804aeb794275ae845d32d2939d0e0fefa75cd112f1075aaf2104097050ae8`  
		Last Modified: Wed, 14 Jun 2023 18:46:04 GMT  
		Size: 1.1 KB (1078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf29fcbe26928e2f4086a889098220505bdd4401dc87958f623ade0618efcd28`  
		Last Modified: Wed, 14 Jun 2023 18:46:05 GMT  
		Size: 1.9 MB (1934899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1d2070a6fd2a146f7a7ccda5a6b5c9e7188304b3eb6ad56e85ae5e13af6efff`  
		Last Modified: Wed, 21 Jun 2023 01:22:36 GMT  
		Size: 6.5 MB (6499598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb2d53b7e662ee08ffe5d3ff1b97e2bbec271b2427e8428d38ab879c1a68cbdd`  
		Last Modified: Wed, 21 Jun 2023 01:22:31 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e13b007130a18104c8ce3a24f68b588c6ec439dcb4c22e430edf1baab337bb13`  
		Last Modified: Wed, 21 Jun 2023 01:22:31 GMT  
		Size: 118.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:bookworm` - linux; ppc64le

```console
$ docker pull memcached@sha256:0466889ea7a59c3e5075122e0dfac5f9fd4b740dbc54d7ca3355e661704b7df3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.2 MB (43193731 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f99a2d51677ef27121ea5fb73098453983811a697bb67558da1548d6a2b1a4d7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 04 Jul 2023 01:17:51 GMT
ADD file:51887002f5002ccc662adbc6ecf1129e3db375a7a77b93da43cc9a8326b3c4b9 in / 
# Tue, 04 Jul 2023 01:17:53 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 06:45:59 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 04 Jul 2023 06:46:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 06:46:11 GMT
ENV MEMCACHED_VERSION=1.6.21
# Tue, 04 Jul 2023 06:46:12 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Tue, 04 Jul 2023 06:50:32 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 04 Jul 2023 06:50:34 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 04 Jul 2023 06:50:36 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 04 Jul 2023 06:50:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Jul 2023 06:50:36 GMT
USER memcache
# Tue, 04 Jul 2023 06:50:37 GMT
EXPOSE 11211
# Tue, 04 Jul 2023 06:50:37 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:ba99a1aa5a92d949d988e66df7723a542fd81bc30eef9d4269e8a899820d4bb2`  
		Last Modified: Tue, 04 Jul 2023 01:24:36 GMT  
		Size: 33.1 MB (33116716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57bc245122d94a5d6dbd04e3f0d2cc3731cb7e5479f873ad6588885b1a1e7fff`  
		Last Modified: Tue, 04 Jul 2023 06:51:13 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8302634866fb43cf1942126242ebd186c7a31db3f01e63b626c2c6cb31aa01bb`  
		Last Modified: Tue, 04 Jul 2023 06:51:14 GMT  
		Size: 2.9 MB (2891325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85b07e92e6621b42a17464a214cee12ada2ca5c70c139194a0d9d5cdf753e470`  
		Last Modified: Tue, 04 Jul 2023 06:51:16 GMT  
		Size: 7.2 MB (7184153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:060e182005428d5f8ae46505c71da839515e43c949a2109682b933781ad7b42d`  
		Last Modified: Tue, 04 Jul 2023 06:51:13 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd71a227a79337edf4a41188a95ac6c897f53d5cc1ebfa6201b14525057ce473`  
		Last Modified: Tue, 04 Jul 2023 06:51:13 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:bookworm` - linux; s390x

```console
$ docker pull memcached@sha256:f90935a3646db47ef74efba3a8ea148e6fa9a6058557fd686664b3a9b83cf5b4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.9 MB (35907614 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:55f50234cc8836dd1977a706a4d7845c857ac2128081a776c895db012f73e5bb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 13 Jun 2023 04:29:41 GMT
ADD file:739f4c23557ec0af5f4ba492c847b5d2f09dd81211c675d0e9eabe865d794e81 in / 
# Tue, 13 Jun 2023 04:29:43 GMT
CMD ["bash"]
# Thu, 15 Jun 2023 06:23:25 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Thu, 15 Jun 2023 06:23:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 21 Jun 2023 00:54:39 GMT
ENV MEMCACHED_VERSION=1.6.21
# Wed, 21 Jun 2023 00:54:39 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Wed, 21 Jun 2023 00:57:46 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 21 Jun 2023 00:57:47 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 21 Jun 2023 00:57:47 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 21 Jun 2023 00:57:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Jun 2023 00:57:47 GMT
USER memcache
# Wed, 21 Jun 2023 00:57:47 GMT
EXPOSE 11211
# Wed, 21 Jun 2023 00:57:48 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:6571b3abd058e377c7bd231c9029aff6eb25486bffb50229076d2e6a356a517f`  
		Last Modified: Tue, 13 Jun 2023 04:34:21 GMT  
		Size: 27.5 MB (27487928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1521043364f590f749ce68598ad1f79907ef04ee2283314cfaab3f72df8e15c`  
		Last Modified: Thu, 15 Jun 2023 06:35:17 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdbc1e75c128be037526f9b133061f5dc6c9baf2f00b5d5b229427bd89eb55b7`  
		Last Modified: Thu, 15 Jun 2023 06:35:18 GMT  
		Size: 2.3 MB (2345340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f3d048c5c76c19c7c7d783cac8384f5698dd61a6aa7ee9067521407789ec9b4`  
		Last Modified: Wed, 21 Jun 2023 01:01:34 GMT  
		Size: 6.1 MB (6072815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c7bfbb7d1965d17408766d01c40f67a94eb422714618a239a48b62cedafdcab`  
		Last Modified: Wed, 21 Jun 2023 01:01:33 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:164d3c9aaa0239a91376552d50ffc16a1e2bf9e3c323e81d2a976556ab25f4a2`  
		Last Modified: Wed, 21 Jun 2023 01:01:33 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:latest`

```console
$ docker pull memcached@sha256:1348f2e27aeea6d2b4e2b25ce9ca7679560164b0e75b6f72e221b574000158f6
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
$ docker pull memcached@sha256:37d77084cbe7c98854989a68a18f22dd677379de8ffc9ee92fbf7b88b2b4d0f9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.0 MB (38973142 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a4d0c1490511995c15a4c1ca7c8413337bed068ea95507aae882010b051ca37e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 12 Jun 2023 23:20:42 GMT
ADD file:ba1250b6ecd5dd09d4914189d72741c2817988994e7da514bf62be439a34bdb5 in / 
# Mon, 12 Jun 2023 23:20:42 GMT
CMD ["bash"]
# Wed, 14 Jun 2023 20:48:19 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 14 Jun 2023 20:48:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 21 Jun 2023 01:04:34 GMT
ENV MEMCACHED_VERSION=1.6.21
# Wed, 21 Jun 2023 01:04:35 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Wed, 21 Jun 2023 01:07:04 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 21 Jun 2023 01:07:04 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 21 Jun 2023 01:07:04 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 21 Jun 2023 01:07:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Jun 2023 01:07:05 GMT
USER memcache
# Wed, 21 Jun 2023 01:07:05 GMT
EXPOSE 11211
# Wed, 21 Jun 2023 01:07:05 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:5b5fe70539cd6989aa19f25826309f9715a9489cf1c057982d6a84c1ad8975c7`  
		Last Modified: Mon, 12 Jun 2023 23:25:49 GMT  
		Size: 29.1 MB (29124744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab209434009a85e82d99c0547bb947940f9e1002ce6e965417396ee22a6820db`  
		Last Modified: Wed, 14 Jun 2023 20:53:33 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2f4dfc49c9cdae8d4df855de7cc0460e5db8c762e73786d4f8fa4f69ba11d6d`  
		Last Modified: Wed, 14 Jun 2023 20:53:33 GMT  
		Size: 2.7 MB (2677239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d5a41694f99632bb3a7c624dab437c8a10e54b92965de823e717f5c12326b1e`  
		Last Modified: Wed, 21 Jun 2023 01:09:52 GMT  
		Size: 7.2 MB (7169627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2be3d7709e1978d4b030abdf5ac129b97f21e09bb489932628899d96288a4a9`  
		Last Modified: Wed, 21 Jun 2023 01:09:50 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8cba3f7cc400544285611f46bbdba004587f84511783fd05aa6562e9337928f`  
		Last Modified: Wed, 21 Jun 2023 01:09:50 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:latest` - linux; arm variant v5

```console
$ docker pull memcached@sha256:1646b01539b9482149379208acae5c0af1c5aed3aa9d818e8748410e15170943
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.1 MB (35094759 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ad4aa07800c4cf602e699a614c04d8fa80a8617828cfeb89fc05b49791d07e7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 12 Jun 2023 23:48:31 GMT
ADD file:54a716f17b23e4fa49d1d5c0a7f63becc295873c116d19bb4753d34f1ca6affb in / 
# Mon, 12 Jun 2023 23:48:31 GMT
CMD ["bash"]
# Wed, 14 Jun 2023 21:56:18 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 14 Jun 2023 21:56:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 21 Jun 2023 00:52:38 GMT
ENV MEMCACHED_VERSION=1.6.21
# Wed, 21 Jun 2023 00:52:39 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Wed, 21 Jun 2023 00:55:49 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 21 Jun 2023 00:55:49 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 21 Jun 2023 00:55:50 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 21 Jun 2023 00:55:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Jun 2023 00:55:50 GMT
USER memcache
# Wed, 21 Jun 2023 00:55:50 GMT
EXPOSE 11211
# Wed, 21 Jun 2023 00:55:50 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:70c60174b18d99741c33011138b5abf2f4d8eca0384521ccb43db3612078e36f`  
		Last Modified: Mon, 12 Jun 2023 23:51:26 GMT  
		Size: 27.0 MB (26982142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52495c3de01d54b61ec15cd608d6ce2ae4587ca764248265b02cb108f790d5a0`  
		Last Modified: Wed, 14 Jun 2023 22:00:39 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:597daa329781ff62c0581a1a2164e04dd294d665a91e97a05aa46fe3d8765eac`  
		Last Modified: Wed, 14 Jun 2023 22:00:40 GMT  
		Size: 2.3 MB (2281778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d65590b8b7bf9398f99bf1baba8d91966081bdc70d61b0165036ac0d16b3b2f`  
		Last Modified: Wed, 21 Jun 2023 00:56:10 GMT  
		Size: 5.8 MB (5829307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dfab31ab9e5a7944b95a42de61a2d1d591fa1605d1a6e2724f9b2c72f03f1ff`  
		Last Modified: Wed, 21 Jun 2023 00:56:09 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85b6795c5e090ce84e068ec9cb629871f3a70380f1bff62aa7baa8a0783343d2`  
		Last Modified: Wed, 21 Jun 2023 00:56:09 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:latest` - linux; arm variant v7

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

### `memcached:latest` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:d82fec3f72f254431725dc57a8b8922cfb269e018b4407c9e7abb133083b1b32
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.9 MB (37872901 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b25fcbe4e1c3b4ce20a4e4994a494fe7a0d98500c1b5b14f4b92c104898a434c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 04 Jul 2023 01:57:35 GMT
ADD file:71fd66666294148382f2e6a09ae5e277d4c4e9c74402ab64b693a79387b67a09 in / 
# Tue, 04 Jul 2023 01:57:36 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 06:40:00 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 04 Jul 2023 06:40:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 06:40:03 GMT
ENV MEMCACHED_VERSION=1.6.21
# Tue, 04 Jul 2023 06:40:03 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Tue, 04 Jul 2023 06:42:47 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 04 Jul 2023 06:42:47 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 04 Jul 2023 06:42:48 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 04 Jul 2023 06:42:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Jul 2023 06:42:48 GMT
USER memcache
# Tue, 04 Jul 2023 06:42:48 GMT
EXPOSE 11211
# Tue, 04 Jul 2023 06:42:48 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:3ae0c06b4d3aa97d7e0829233dd36cea1666b87074e55fea6bd1ecae066693c7`  
		Last Modified: Tue, 04 Jul 2023 02:01:20 GMT  
		Size: 29.2 MB (29152458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7e0b4333d4768ee800aa733f63a51c54833abe7bd20188154f0869796bb3f8c`  
		Last Modified: Tue, 04 Jul 2023 06:43:03 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fd0e2a70b071a1504381d7831ed736d40261b75692a2fe4ee547186e80ad9b2`  
		Last Modified: Tue, 04 Jul 2023 06:43:03 GMT  
		Size: 2.5 MB (2539167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:382aa3014b4367d16a225a23e5195af1f3a5e51523f9d89461e4b98ddf61aa3d`  
		Last Modified: Tue, 04 Jul 2023 06:43:04 GMT  
		Size: 6.2 MB (6179743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4abaeb5f633e1c888b605fe890a58e527c62021db2516cd8606edad49e9500c0`  
		Last Modified: Tue, 04 Jul 2023 06:43:03 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aedc2da2773982e3f9627ea96874aec7c38a4288cca37a366f29392750f7c38`  
		Last Modified: Tue, 04 Jul 2023 06:43:03 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:latest` - linux; 386

```console
$ docker pull memcached@sha256:d275ff7e4cd6b5d699c14115419af7ae2c1bfa32312282ff8c9ba0b424cf6be0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.5 MB (39457503 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8785d2e661831af23d884d73d3196f416198d2c57ffa24c50c8cafe16c0da224`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 12 Jun 2023 23:39:20 GMT
ADD file:c7ecc5e2bed99e2cbca26f9f4247cd9bc399749556f4084e9357a9b00bb80530 in / 
# Mon, 12 Jun 2023 23:39:20 GMT
CMD ["bash"]
# Wed, 14 Jun 2023 22:34:28 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 14 Jun 2023 22:34:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 21 Jun 2023 00:46:59 GMT
ENV MEMCACHED_VERSION=1.6.21
# Wed, 21 Jun 2023 00:46:59 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Wed, 21 Jun 2023 00:50:45 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 21 Jun 2023 00:50:45 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 21 Jun 2023 00:50:46 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 21 Jun 2023 00:50:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Jun 2023 00:50:46 GMT
USER memcache
# Wed, 21 Jun 2023 00:50:46 GMT
EXPOSE 11211
# Wed, 21 Jun 2023 00:50:46 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:82a41d17956dd7c8ebb39c9ce936fd26841bdbec98d0a185e3db8154b352edff`  
		Last Modified: Mon, 12 Jun 2023 23:46:21 GMT  
		Size: 30.1 MB (30140741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:039125a8cebc58c43be503e98831cac166a973cb3e68f4b66194142680e76964`  
		Last Modified: Wed, 14 Jun 2023 22:42:09 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:199b04439aa2a5065d0c23f986eccd0dd093be2f49b180b332af4f35d977ab5b`  
		Last Modified: Wed, 14 Jun 2023 22:42:09 GMT  
		Size: 2.7 MB (2685017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e58126d70102e38c764aa423066a897bc811895dc85b8d607eadfcff947049a7`  
		Last Modified: Wed, 21 Jun 2023 00:54:46 GMT  
		Size: 6.6 MB (6630215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b039c50c059c1c3a231a9659c8ade08b537d8ecac9423685ba16cf308626c4e4`  
		Last Modified: Wed, 21 Jun 2023 00:54:44 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1d3e144a63d04f26029dacd020e1ec00baeae59c5cee460a482e70842be2fc2`  
		Last Modified: Wed, 21 Jun 2023 00:54:44 GMT  
		Size: 116.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:latest` - linux; mips64le

```console
$ docker pull memcached@sha256:76620bca6f37fb4a82e0cc3aa33ba7cc2508c8f93dd4ae4956e9b471ce0995a2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.6 MB (37554107 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f8424fcd7f4d7db2c883a9303136b4305e34813630a9e325332ee830d35c026d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 13 Jun 2023 00:09:02 GMT
ADD file:f91bd2a174259cb69646fc34ba2fc6b8941ad8e171d2d7952a4d8ac3d95e2ad7 in / 
# Tue, 13 Jun 2023 00:09:06 GMT
CMD ["bash"]
# Wed, 14 Jun 2023 18:38:15 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 14 Jun 2023 18:38:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 21 Jun 2023 01:14:52 GMT
ENV MEMCACHED_VERSION=1.6.21
# Wed, 21 Jun 2023 01:14:54 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Wed, 21 Jun 2023 01:21:45 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 21 Jun 2023 01:21:47 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 21 Jun 2023 01:21:52 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 21 Jun 2023 01:21:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Jun 2023 01:21:57 GMT
USER memcache
# Wed, 21 Jun 2023 01:22:00 GMT
EXPOSE 11211
# Wed, 21 Jun 2023 01:22:02 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:3fc28260a4d871ef9781cad2bb064ad7212a5063de3a1d35dba938ce82115e5b`  
		Last Modified: Tue, 13 Jun 2023 00:22:29 GMT  
		Size: 29.1 MB (29118129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79c804aeb794275ae845d32d2939d0e0fefa75cd112f1075aaf2104097050ae8`  
		Last Modified: Wed, 14 Jun 2023 18:46:04 GMT  
		Size: 1.1 KB (1078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf29fcbe26928e2f4086a889098220505bdd4401dc87958f623ade0618efcd28`  
		Last Modified: Wed, 14 Jun 2023 18:46:05 GMT  
		Size: 1.9 MB (1934899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1d2070a6fd2a146f7a7ccda5a6b5c9e7188304b3eb6ad56e85ae5e13af6efff`  
		Last Modified: Wed, 21 Jun 2023 01:22:36 GMT  
		Size: 6.5 MB (6499598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb2d53b7e662ee08ffe5d3ff1b97e2bbec271b2427e8428d38ab879c1a68cbdd`  
		Last Modified: Wed, 21 Jun 2023 01:22:31 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e13b007130a18104c8ce3a24f68b588c6ec439dcb4c22e430edf1baab337bb13`  
		Last Modified: Wed, 21 Jun 2023 01:22:31 GMT  
		Size: 118.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:latest` - linux; ppc64le

```console
$ docker pull memcached@sha256:0466889ea7a59c3e5075122e0dfac5f9fd4b740dbc54d7ca3355e661704b7df3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.2 MB (43193731 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f99a2d51677ef27121ea5fb73098453983811a697bb67558da1548d6a2b1a4d7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 04 Jul 2023 01:17:51 GMT
ADD file:51887002f5002ccc662adbc6ecf1129e3db375a7a77b93da43cc9a8326b3c4b9 in / 
# Tue, 04 Jul 2023 01:17:53 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 06:45:59 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 04 Jul 2023 06:46:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 06:46:11 GMT
ENV MEMCACHED_VERSION=1.6.21
# Tue, 04 Jul 2023 06:46:12 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Tue, 04 Jul 2023 06:50:32 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 04 Jul 2023 06:50:34 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 04 Jul 2023 06:50:36 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 04 Jul 2023 06:50:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Jul 2023 06:50:36 GMT
USER memcache
# Tue, 04 Jul 2023 06:50:37 GMT
EXPOSE 11211
# Tue, 04 Jul 2023 06:50:37 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:ba99a1aa5a92d949d988e66df7723a542fd81bc30eef9d4269e8a899820d4bb2`  
		Last Modified: Tue, 04 Jul 2023 01:24:36 GMT  
		Size: 33.1 MB (33116716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57bc245122d94a5d6dbd04e3f0d2cc3731cb7e5479f873ad6588885b1a1e7fff`  
		Last Modified: Tue, 04 Jul 2023 06:51:13 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8302634866fb43cf1942126242ebd186c7a31db3f01e63b626c2c6cb31aa01bb`  
		Last Modified: Tue, 04 Jul 2023 06:51:14 GMT  
		Size: 2.9 MB (2891325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85b07e92e6621b42a17464a214cee12ada2ca5c70c139194a0d9d5cdf753e470`  
		Last Modified: Tue, 04 Jul 2023 06:51:16 GMT  
		Size: 7.2 MB (7184153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:060e182005428d5f8ae46505c71da839515e43c949a2109682b933781ad7b42d`  
		Last Modified: Tue, 04 Jul 2023 06:51:13 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd71a227a79337edf4a41188a95ac6c897f53d5cc1ebfa6201b14525057ce473`  
		Last Modified: Tue, 04 Jul 2023 06:51:13 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:latest` - linux; s390x

```console
$ docker pull memcached@sha256:f90935a3646db47ef74efba3a8ea148e6fa9a6058557fd686664b3a9b83cf5b4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.9 MB (35907614 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:55f50234cc8836dd1977a706a4d7845c857ac2128081a776c895db012f73e5bb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 13 Jun 2023 04:29:41 GMT
ADD file:739f4c23557ec0af5f4ba492c847b5d2f09dd81211c675d0e9eabe865d794e81 in / 
# Tue, 13 Jun 2023 04:29:43 GMT
CMD ["bash"]
# Thu, 15 Jun 2023 06:23:25 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Thu, 15 Jun 2023 06:23:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 21 Jun 2023 00:54:39 GMT
ENV MEMCACHED_VERSION=1.6.21
# Wed, 21 Jun 2023 00:54:39 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Wed, 21 Jun 2023 00:57:46 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 21 Jun 2023 00:57:47 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 21 Jun 2023 00:57:47 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 21 Jun 2023 00:57:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Jun 2023 00:57:47 GMT
USER memcache
# Wed, 21 Jun 2023 00:57:47 GMT
EXPOSE 11211
# Wed, 21 Jun 2023 00:57:48 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:6571b3abd058e377c7bd231c9029aff6eb25486bffb50229076d2e6a356a517f`  
		Last Modified: Tue, 13 Jun 2023 04:34:21 GMT  
		Size: 27.5 MB (27487928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1521043364f590f749ce68598ad1f79907ef04ee2283314cfaab3f72df8e15c`  
		Last Modified: Thu, 15 Jun 2023 06:35:17 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdbc1e75c128be037526f9b133061f5dc6c9baf2f00b5d5b229427bd89eb55b7`  
		Last Modified: Thu, 15 Jun 2023 06:35:18 GMT  
		Size: 2.3 MB (2345340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f3d048c5c76c19c7c7d783cac8384f5698dd61a6aa7ee9067521407789ec9b4`  
		Last Modified: Wed, 21 Jun 2023 01:01:34 GMT  
		Size: 6.1 MB (6072815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c7bfbb7d1965d17408766d01c40f67a94eb422714618a239a48b62cedafdcab`  
		Last Modified: Wed, 21 Jun 2023 01:01:33 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:164d3c9aaa0239a91376552d50ffc16a1e2bf9e3c323e81d2a976556ab25f4a2`  
		Last Modified: Wed, 21 Jun 2023 01:01:33 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
