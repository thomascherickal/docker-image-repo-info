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
-	[`memcached:1.6.20`](#memcached1620)
-	[`memcached:1.6.20-alpine`](#memcached1620-alpine)
-	[`memcached:1.6.20-alpine3.18`](#memcached1620-alpine318)
-	[`memcached:1.6.20-bookworm`](#memcached1620-bookworm)
-	[`memcached:alpine`](#memcachedalpine)
-	[`memcached:alpine3.18`](#memcachedalpine318)
-	[`memcached:bookworm`](#memcachedbookworm)
-	[`memcached:latest`](#memcachedlatest)

## `memcached:1`

```console
$ docker pull memcached@sha256:791d3a3f4bed25f726ff2e0fea1bbc1038a5154dfadfc2d19cd2e8dd4c5a1a05
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
$ docker pull memcached@sha256:533c607824b2f5781b179e175fcdf055577a3f076fb0a0fdcd13487c7c92125f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.0 MB (38973406 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cbcfa8d0003c80b0bba4004f4b15b4a5600b9dd481ac2d887bc31e794f067464`
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
# Wed, 14 Jun 2023 20:48:24 GMT
ENV MEMCACHED_VERSION=1.6.20
# Wed, 14 Jun 2023 20:48:24 GMT
ENV MEMCACHED_SHA1=face85ed6fad41432ad818445b24eca55bccdd78
# Wed, 14 Jun 2023 20:50:40 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 14 Jun 2023 20:50:40 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 14 Jun 2023 20:50:41 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 14 Jun 2023 20:50:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Jun 2023 20:50:41 GMT
USER memcache
# Wed, 14 Jun 2023 20:50:41 GMT
EXPOSE 11211
# Wed, 14 Jun 2023 20:50:41 GMT
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
	-	`sha256:96a3de0d22592d9a254814d5b77e3a84e73d2f055d162503fe811f731a320701`  
		Last Modified: Wed, 14 Jun 2023 20:53:34 GMT  
		Size: 7.2 MB (7169888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a38b201fb7fc8d917459453ee1c0218cf9845c96b885a02b02999f81b21c6bb`  
		Last Modified: Wed, 14 Jun 2023 20:53:33 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6f5720dc1980c886ee7e8d6067ed87e102bb31824e557a85fbd54273542debf`  
		Last Modified: Wed, 14 Jun 2023 20:53:33 GMT  
		Size: 120.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1` - linux; arm variant v5

```console
$ docker pull memcached@sha256:bb4a530ed3dc36e702635724bf49a6703694d36a7bcfdeabb2b0d3ff6b101143
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.1 MB (35095204 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f00b0d176a0550d5b0d3f94dc00489066995ce4a1be3e688924144b9077256f`
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
# Wed, 14 Jun 2023 21:56:26 GMT
ENV MEMCACHED_VERSION=1.6.20
# Wed, 14 Jun 2023 21:56:27 GMT
ENV MEMCACHED_SHA1=face85ed6fad41432ad818445b24eca55bccdd78
# Wed, 14 Jun 2023 22:00:10 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 14 Jun 2023 22:00:10 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 14 Jun 2023 22:00:12 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 14 Jun 2023 22:00:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Jun 2023 22:00:12 GMT
USER memcache
# Wed, 14 Jun 2023 22:00:12 GMT
EXPOSE 11211
# Wed, 14 Jun 2023 22:00:13 GMT
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
	-	`sha256:feb8e13d6ab7efa5799bc12cdb4d8f410166028673257b803f31b6bc9d0eb70c`  
		Last Modified: Wed, 14 Jun 2023 22:00:42 GMT  
		Size: 5.8 MB (5829749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cf20cb3e5676ee2969940d8133531dcd0df55159ccb7dbd567cc83b2bc02384`  
		Last Modified: Wed, 14 Jun 2023 22:00:39 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04bc2d45321e126b2795ea784886ac10a0b3c5724ccf555f0d20f2c7ee4225f1`  
		Last Modified: Wed, 14 Jun 2023 22:00:39 GMT  
		Size: 121.0 B  
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
$ docker pull memcached@sha256:3464bfccdfad0dc788e056949d59fc0b665ec165654b3a8502a2f4a3868a3dc7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.9 MB (37872888 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:20f33353745665e05e1722aa9af40e06b3f58778f8e758e786eaad30054de61f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 12 Jun 2023 23:40:13 GMT
ADD file:f75c3fe22fec548b35a86a9a5802fdc97497f5d253cf630d65f13282169d3f3f in / 
# Mon, 12 Jun 2023 23:40:14 GMT
CMD ["bash"]
# Wed, 14 Jun 2023 20:54:33 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 14 Jun 2023 20:54:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 14 Jun 2023 20:54:37 GMT
ENV MEMCACHED_VERSION=1.6.20
# Wed, 14 Jun 2023 20:54:37 GMT
ENV MEMCACHED_SHA1=face85ed6fad41432ad818445b24eca55bccdd78
# Wed, 14 Jun 2023 20:57:13 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 14 Jun 2023 20:57:13 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 14 Jun 2023 20:57:14 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 14 Jun 2023 20:57:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Jun 2023 20:57:14 GMT
USER memcache
# Wed, 14 Jun 2023 20:57:14 GMT
EXPOSE 11211
# Wed, 14 Jun 2023 20:57:14 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:95039a22a7cc3ae41d71f075e6e09e91e8da850fb5f80aba2f4a09f254520539`  
		Last Modified: Mon, 12 Jun 2023 23:44:08 GMT  
		Size: 29.2 MB (29152534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6da70104cc8ee465752315034f04011354e6149243e2bc69b9da49e6855df4b8`  
		Last Modified: Wed, 14 Jun 2023 21:00:29 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a7b40152f53e05b8cbcfe09be5b1598fcc05cf4f9ffad3b296eca43305450da`  
		Last Modified: Wed, 14 Jun 2023 21:00:30 GMT  
		Size: 2.5 MB (2539179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bf09d04f9c61af195486f42915b137b8612584f982737f5e465d02648a6dc8a`  
		Last Modified: Wed, 14 Jun 2023 21:00:30 GMT  
		Size: 6.2 MB (6179640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e71555e51295eeceeab1a9ab6bebb21108fbbe59e01349857c51932deea0f64`  
		Last Modified: Wed, 14 Jun 2023 21:00:29 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15cd3195dbfc5cedaf71b7c156002599dfb94219b51f85c966a1bee80bc37e65`  
		Last Modified: Wed, 14 Jun 2023 21:00:29 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1` - linux; 386

```console
$ docker pull memcached@sha256:7c2fdc7c597b4f6efd737d9b8f1e78841cda31e4492a6ae32f3d6f1ab6911cb8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.5 MB (39457716 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a1e668084859e8f39e52c33d0d7a68506127f94d95c61ffb7f43f9441843fa3b`
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
# Wed, 14 Jun 2023 22:34:33 GMT
ENV MEMCACHED_VERSION=1.6.20
# Wed, 14 Jun 2023 22:34:33 GMT
ENV MEMCACHED_SHA1=face85ed6fad41432ad818445b24eca55bccdd78
# Wed, 14 Jun 2023 22:38:16 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 14 Jun 2023 22:38:17 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 14 Jun 2023 22:38:17 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 14 Jun 2023 22:38:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Jun 2023 22:38:17 GMT
USER memcache
# Wed, 14 Jun 2023 22:38:17 GMT
EXPOSE 11211
# Wed, 14 Jun 2023 22:38:18 GMT
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
	-	`sha256:2896f0aba2db45558c3b7f796cc22aa198f38d579fdc6ddf35893d5ea553c080`  
		Last Modified: Wed, 14 Jun 2023 22:42:10 GMT  
		Size: 6.6 MB (6630422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17e035509d03f0bd9a08582ab075babcb6e7dcbe048f9968c81ae996df72e6aa`  
		Last Modified: Wed, 14 Jun 2023 22:42:09 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc5b3164ed6a8d968b1da11795198c4d6ce05822ff371f41d2c7eb373d44141b`  
		Last Modified: Wed, 14 Jun 2023 22:42:09 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1` - linux; mips64le

```console
$ docker pull memcached@sha256:d2855c4deb19365dd1c83b81c9e1fa36f7873cc8b3dd02f8f01de10200bf208e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.6 MB (37554221 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7068fffc8ee0a4607e1586297977a273786efb52e1782f11396ee5f7a5150c0f`
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
# Wed, 14 Jun 2023 18:38:39 GMT
ENV MEMCACHED_VERSION=1.6.20
# Wed, 14 Jun 2023 18:38:41 GMT
ENV MEMCACHED_SHA1=face85ed6fad41432ad818445b24eca55bccdd78
# Wed, 14 Jun 2023 18:45:20 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 14 Jun 2023 18:45:23 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 14 Jun 2023 18:45:27 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 14 Jun 2023 18:45:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Jun 2023 18:45:32 GMT
USER memcache
# Wed, 14 Jun 2023 18:45:35 GMT
EXPOSE 11211
# Wed, 14 Jun 2023 18:45:38 GMT
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
	-	`sha256:76d4e9cc234d41e69eba3bf411cb1d3ebe17e2fefbffb0c3458d613f2545337e`  
		Last Modified: Wed, 14 Jun 2023 18:46:09 GMT  
		Size: 6.5 MB (6499709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0988c34e4840378b9876eba362b50458e769389d0cc626698bef65e46c721458`  
		Last Modified: Wed, 14 Jun 2023 18:46:04 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db55745458426cdf0d23fd0589fd440e2d328e4d5ffb00a9ef6d2e0225cec8bf`  
		Last Modified: Wed, 14 Jun 2023 18:46:04 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1` - linux; ppc64le

```console
$ docker pull memcached@sha256:0e023c41d9c6a8d04edad22ecea59cfcf424d0dc3895c442a9e7a4575961d53d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.2 MB (43193448 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a85a60b74a9575a203aba1a5f800dfe479b80cde8ff577ccd5e7e77bdaab64c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 12 Jun 2023 23:17:34 GMT
ADD file:3f8b9849acb625537f99921ef80190de7b03afdc287a5d1113a92cc41ae24be2 in / 
# Mon, 12 Jun 2023 23:17:36 GMT
CMD ["bash"]
# Wed, 14 Jun 2023 18:15:42 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 14 Jun 2023 18:15:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 14 Jun 2023 18:15:50 GMT
ENV MEMCACHED_VERSION=1.6.20
# Wed, 14 Jun 2023 18:15:51 GMT
ENV MEMCACHED_SHA1=face85ed6fad41432ad818445b24eca55bccdd78
# Wed, 14 Jun 2023 18:19:27 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 14 Jun 2023 18:19:28 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 14 Jun 2023 18:19:30 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 14 Jun 2023 18:19:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Jun 2023 18:19:31 GMT
USER memcache
# Wed, 14 Jun 2023 18:19:32 GMT
EXPOSE 11211
# Wed, 14 Jun 2023 18:19:32 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:9f041b53cef30007c43057f2520876c85ed6bee6be5aaee867dfb31a053d6cca`  
		Last Modified: Mon, 12 Jun 2023 23:24:09 GMT  
		Size: 33.1 MB (33116725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2a2d84b1fee81412bbd9bb301c77e6dfacfac70c2f1485de806658b49b06e08`  
		Last Modified: Wed, 14 Jun 2023 18:19:49 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca8bb5af043b48c9fe0e110ee13c139ceb715570346140fc86092d582d38b52b`  
		Last Modified: Wed, 14 Jun 2023 18:19:50 GMT  
		Size: 2.9 MB (2891306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e2d7805a151ec1618da95ad34cb2fdc6ae889b9f7908aaca6d063ca864f3e24`  
		Last Modified: Wed, 14 Jun 2023 18:19:52 GMT  
		Size: 7.2 MB (7183881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc5db4b315753422be0d08638f594b1ec64484c44f68942473f903387853b3bd`  
		Last Modified: Wed, 14 Jun 2023 18:19:49 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a8a9b2ed7c41d27d92f9db3c21beec2a2e288b0bc54a19aa1d3574b6085eaa6`  
		Last Modified: Wed, 14 Jun 2023 18:19:49 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1` - linux; s390x

```console
$ docker pull memcached@sha256:7bbe5a63846bc51d11850be291c164685b55f4d65a48ea07e8a6df50e489b658
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.9 MB (35907698 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d7e906c7eff45be64cda148363028a1270de09239533ca7dfee428108e20a155`
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
# Thu, 15 Jun 2023 06:23:29 GMT
ENV MEMCACHED_VERSION=1.6.20
# Thu, 15 Jun 2023 06:23:29 GMT
ENV MEMCACHED_SHA1=face85ed6fad41432ad818445b24eca55bccdd78
# Thu, 15 Jun 2023 06:26:33 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 15 Jun 2023 06:26:33 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 15 Jun 2023 06:26:34 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 15 Jun 2023 06:26:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 15 Jun 2023 06:26:35 GMT
USER memcache
# Thu, 15 Jun 2023 06:26:35 GMT
EXPOSE 11211
# Thu, 15 Jun 2023 06:26:35 GMT
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
	-	`sha256:a7ba1840ae9bcaa91375ac3b538e9ad379ec203bf9c6616bff06ec2a9ca6616a`  
		Last Modified: Thu, 15 Jun 2023 06:35:18 GMT  
		Size: 6.1 MB (6072893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d4533d005f06d7358727f3d1a167ee982d65ec08c863bd2171511918dab48d4`  
		Last Modified: Thu, 15 Jun 2023 06:35:17 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:769590255adfb1d384255f87732ddc4f78483e8203987ffba90f56f4102080e7`  
		Last Modified: Thu, 15 Jun 2023 06:35:17 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:1-alpine`

```console
$ docker pull memcached@sha256:bb867cdf4270f78a89270fab6532b2d27aa02dec52e62ba08d6cf02809ce37de
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
$ docker pull memcached@sha256:a7a04bc20ec122d9f024dff57494853d5dc9705fb97af9170cc31a1f531dcaa5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4462373 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:15429daa972e1d57884e75ecc7f784564ae7cf089c25671dd118a0025f806b6f`
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
# Wed, 14 Jun 2023 20:50:59 GMT
ENV MEMCACHED_VERSION=1.6.20
# Wed, 14 Jun 2023 20:50:59 GMT
ENV MEMCACHED_SHA1=face85ed6fad41432ad818445b24eca55bccdd78
# Wed, 14 Jun 2023 20:53:09 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Wed, 14 Jun 2023 20:53:09 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 14 Jun 2023 20:53:09 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 14 Jun 2023 20:53:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Jun 2023 20:53:09 GMT
USER memcache
# Wed, 14 Jun 2023 20:53:09 GMT
EXPOSE 11211
# Wed, 14 Jun 2023 20:53:09 GMT
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
	-	`sha256:bc06ea6ffc2a4279c91e26e37b450afb1e0f1007815b19a7146d52b016dddc61`  
		Last Modified: Wed, 14 Jun 2023 20:53:59 GMT  
		Size: 954.7 KB (954748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:098e9e56712cb64736718f40b476d8eeb9410130c28ce94fe1bc2d380d9083cf`  
		Last Modified: Wed, 14 Jun 2023 20:53:59 GMT  
		Size: 282.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5c14818f6fb630a615284b18f945c89c0563530c25f07af955d0f85504020e9`  
		Last Modified: Wed, 14 Jun 2023 20:53:58 GMT  
		Size: 118.0 B  
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
$ docker pull memcached@sha256:e59934ff7bef6e6053b618f65923d2c1fa7235a008fb20f4fe9db13f8d6dc167
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.4 MB (4399194 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dab6918acf63bcf26d1a95d40666c44f281aa14f0d4e27884d4c2f4b227dd9b3`
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
# Wed, 14 Jun 2023 20:57:27 GMT
ENV MEMCACHED_VERSION=1.6.20
# Wed, 14 Jun 2023 20:57:27 GMT
ENV MEMCACHED_SHA1=face85ed6fad41432ad818445b24eca55bccdd78
# Wed, 14 Jun 2023 20:59:54 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Wed, 14 Jun 2023 20:59:54 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 14 Jun 2023 20:59:55 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 14 Jun 2023 20:59:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Jun 2023 20:59:55 GMT
USER memcache
# Wed, 14 Jun 2023 20:59:55 GMT
EXPOSE 11211
# Wed, 14 Jun 2023 20:59:55 GMT
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
	-	`sha256:eddee3cdc367d6f8265fe941f97020460db6cb5555711640b2ad62bd5c2a613c`  
		Last Modified: Wed, 14 Jun 2023 21:00:51 GMT  
		Size: 944.1 KB (944138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfec1ffcd9427d8fb06b908c1d3e0715a9db99c94c46f7896890a98b95c5f049`  
		Last Modified: Wed, 14 Jun 2023 21:00:51 GMT  
		Size: 280.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aea835bd4a5d779b88da37bc977813dd1ed9d228f5e78e3459edde4fa6f155e2`  
		Last Modified: Wed, 14 Jun 2023 21:00:51 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-alpine` - linux; 386

```console
$ docker pull memcached@sha256:a919915b23bf734458584f42947ebf9a743a84c8c93d2e2ea784e1bc230aaa59
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.3 MB (4282199 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2764bc1af6a7d65fbfe6ad34b4c7d1799646f8d940c1b23b550f5b577d86b8b9`
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
# Wed, 14 Jun 2023 22:38:22 GMT
ENV MEMCACHED_VERSION=1.6.20
# Wed, 14 Jun 2023 22:38:22 GMT
ENV MEMCACHED_SHA1=face85ed6fad41432ad818445b24eca55bccdd78
# Wed, 14 Jun 2023 22:41:49 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Wed, 14 Jun 2023 22:41:49 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 14 Jun 2023 22:41:50 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 14 Jun 2023 22:41:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Jun 2023 22:41:50 GMT
USER memcache
# Wed, 14 Jun 2023 22:41:50 GMT
EXPOSE 11211
# Wed, 14 Jun 2023 22:41:50 GMT
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
	-	`sha256:e6eae361cc7d0f997a631fbe78920dacf40cb6d4751c30ee1692dbeac08bc37f`  
		Last Modified: Wed, 14 Jun 2023 22:42:32 GMT  
		Size: 937.0 KB (937049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26d07209b7ab8b880d78464e8fda28a770a3be477f9566a419967691b487705f`  
		Last Modified: Wed, 14 Jun 2023 22:42:32 GMT  
		Size: 280.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af5afdbe7d4d8e1bd1297aa2dfcdc690485f3965c75a5eb520d5681c789048c5`  
		Last Modified: Wed, 14 Jun 2023 22:42:32 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-alpine` - linux; ppc64le

```console
$ docker pull memcached@sha256:4ac2ba7993ef774f28a06c635dfb14927d19a5d624e1d935a9d17231df0f153f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4453208 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d545989d562d3df14a6b1e5f35cfa997c5f02dcbe213a92d66f3aaad767c1feb`
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
# Thu, 15 Jun 2023 04:20:03 GMT
ENV MEMCACHED_VERSION=1.6.20
# Thu, 15 Jun 2023 04:20:03 GMT
ENV MEMCACHED_SHA1=face85ed6fad41432ad818445b24eca55bccdd78
# Thu, 15 Jun 2023 04:23:03 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Thu, 15 Jun 2023 04:23:04 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 15 Jun 2023 04:23:05 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 15 Jun 2023 04:23:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 15 Jun 2023 04:23:05 GMT
USER memcache
# Thu, 15 Jun 2023 04:23:06 GMT
EXPOSE 11211
# Thu, 15 Jun 2023 04:23:06 GMT
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
	-	`sha256:b035d841131485b85fca254bc1f51878eeb4efb089ca292b6912144e0744dcfa`  
		Last Modified: Thu, 15 Jun 2023 04:23:37 GMT  
		Size: 982.8 KB (982821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49b24d1f64de4f01a1b2c94bbd8b53bfd5d55c0d2c842418f679f2dc3122f93d`  
		Last Modified: Thu, 15 Jun 2023 04:23:37 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:400968138d2a427cec2d804e2fb8b52908236f9823f026c8d3f5f90f5fbbed0b`  
		Last Modified: Thu, 15 Jun 2023 04:23:36 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-alpine` - linux; s390x

```console
$ docker pull memcached@sha256:441c53da2edef09782ae8d67860d08a92c2c8c9e4abf7f0a48977db69a803953
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.3 MB (4278165 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1023dcfb4b4b8c4b0993be67253a28f023a74ff3b9eaa67976766f6d256f73a7`
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
# Thu, 15 Jun 2023 06:27:49 GMT
ENV MEMCACHED_VERSION=1.6.20
# Thu, 15 Jun 2023 06:27:50 GMT
ENV MEMCACHED_SHA1=face85ed6fad41432ad818445b24eca55bccdd78
# Thu, 15 Jun 2023 06:31:41 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Thu, 15 Jun 2023 06:31:42 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 15 Jun 2023 06:31:44 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 15 Jun 2023 06:31:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 15 Jun 2023 06:31:45 GMT
USER memcache
# Thu, 15 Jun 2023 06:31:45 GMT
EXPOSE 11211
# Thu, 15 Jun 2023 06:31:45 GMT
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
	-	`sha256:baa4da6084d6df86753b54ce48182165eb8c080ba843e13fa42fb2503ab59c27`  
		Last Modified: Thu, 15 Jun 2023 06:36:33 GMT  
		Size: 950.1 KB (950145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fc33101b6e87a2752ae5e82c32aa4480ef0000c174eb363eadfe98755991b38`  
		Last Modified: Thu, 15 Jun 2023 06:36:33 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c8630e5ca40a95cae4c251c954b07bae6331ac9d08eeff70d12d3263339dca0`  
		Last Modified: Thu, 15 Jun 2023 06:36:33 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:1-alpine3.18`

```console
$ docker pull memcached@sha256:2943c39203d6df11309370bbd8e3896daddfac79f1a6414a9a9cc2381e70da81
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
$ docker pull memcached@sha256:a7a04bc20ec122d9f024dff57494853d5dc9705fb97af9170cc31a1f531dcaa5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4462373 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:15429daa972e1d57884e75ecc7f784564ae7cf089c25671dd118a0025f806b6f`
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
# Wed, 14 Jun 2023 20:50:59 GMT
ENV MEMCACHED_VERSION=1.6.20
# Wed, 14 Jun 2023 20:50:59 GMT
ENV MEMCACHED_SHA1=face85ed6fad41432ad818445b24eca55bccdd78
# Wed, 14 Jun 2023 20:53:09 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Wed, 14 Jun 2023 20:53:09 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 14 Jun 2023 20:53:09 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 14 Jun 2023 20:53:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Jun 2023 20:53:09 GMT
USER memcache
# Wed, 14 Jun 2023 20:53:09 GMT
EXPOSE 11211
# Wed, 14 Jun 2023 20:53:09 GMT
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
	-	`sha256:bc06ea6ffc2a4279c91e26e37b450afb1e0f1007815b19a7146d52b016dddc61`  
		Last Modified: Wed, 14 Jun 2023 20:53:59 GMT  
		Size: 954.7 KB (954748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:098e9e56712cb64736718f40b476d8eeb9410130c28ce94fe1bc2d380d9083cf`  
		Last Modified: Wed, 14 Jun 2023 20:53:59 GMT  
		Size: 282.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5c14818f6fb630a615284b18f945c89c0563530c25f07af955d0f85504020e9`  
		Last Modified: Wed, 14 Jun 2023 20:53:58 GMT  
		Size: 118.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-alpine3.18` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:e59934ff7bef6e6053b618f65923d2c1fa7235a008fb20f4fe9db13f8d6dc167
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.4 MB (4399194 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dab6918acf63bcf26d1a95d40666c44f281aa14f0d4e27884d4c2f4b227dd9b3`
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
# Wed, 14 Jun 2023 20:57:27 GMT
ENV MEMCACHED_VERSION=1.6.20
# Wed, 14 Jun 2023 20:57:27 GMT
ENV MEMCACHED_SHA1=face85ed6fad41432ad818445b24eca55bccdd78
# Wed, 14 Jun 2023 20:59:54 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Wed, 14 Jun 2023 20:59:54 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 14 Jun 2023 20:59:55 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 14 Jun 2023 20:59:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Jun 2023 20:59:55 GMT
USER memcache
# Wed, 14 Jun 2023 20:59:55 GMT
EXPOSE 11211
# Wed, 14 Jun 2023 20:59:55 GMT
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
	-	`sha256:eddee3cdc367d6f8265fe941f97020460db6cb5555711640b2ad62bd5c2a613c`  
		Last Modified: Wed, 14 Jun 2023 21:00:51 GMT  
		Size: 944.1 KB (944138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfec1ffcd9427d8fb06b908c1d3e0715a9db99c94c46f7896890a98b95c5f049`  
		Last Modified: Wed, 14 Jun 2023 21:00:51 GMT  
		Size: 280.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aea835bd4a5d779b88da37bc977813dd1ed9d228f5e78e3459edde4fa6f155e2`  
		Last Modified: Wed, 14 Jun 2023 21:00:51 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-alpine3.18` - linux; 386

```console
$ docker pull memcached@sha256:a919915b23bf734458584f42947ebf9a743a84c8c93d2e2ea784e1bc230aaa59
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.3 MB (4282199 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2764bc1af6a7d65fbfe6ad34b4c7d1799646f8d940c1b23b550f5b577d86b8b9`
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
# Wed, 14 Jun 2023 22:38:22 GMT
ENV MEMCACHED_VERSION=1.6.20
# Wed, 14 Jun 2023 22:38:22 GMT
ENV MEMCACHED_SHA1=face85ed6fad41432ad818445b24eca55bccdd78
# Wed, 14 Jun 2023 22:41:49 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Wed, 14 Jun 2023 22:41:49 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 14 Jun 2023 22:41:50 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 14 Jun 2023 22:41:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Jun 2023 22:41:50 GMT
USER memcache
# Wed, 14 Jun 2023 22:41:50 GMT
EXPOSE 11211
# Wed, 14 Jun 2023 22:41:50 GMT
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
	-	`sha256:e6eae361cc7d0f997a631fbe78920dacf40cb6d4751c30ee1692dbeac08bc37f`  
		Last Modified: Wed, 14 Jun 2023 22:42:32 GMT  
		Size: 937.0 KB (937049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26d07209b7ab8b880d78464e8fda28a770a3be477f9566a419967691b487705f`  
		Last Modified: Wed, 14 Jun 2023 22:42:32 GMT  
		Size: 280.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af5afdbe7d4d8e1bd1297aa2dfcdc690485f3965c75a5eb520d5681c789048c5`  
		Last Modified: Wed, 14 Jun 2023 22:42:32 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-alpine3.18` - linux; ppc64le

```console
$ docker pull memcached@sha256:4ac2ba7993ef774f28a06c635dfb14927d19a5d624e1d935a9d17231df0f153f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4453208 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d545989d562d3df14a6b1e5f35cfa997c5f02dcbe213a92d66f3aaad767c1feb`
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
# Thu, 15 Jun 2023 04:20:03 GMT
ENV MEMCACHED_VERSION=1.6.20
# Thu, 15 Jun 2023 04:20:03 GMT
ENV MEMCACHED_SHA1=face85ed6fad41432ad818445b24eca55bccdd78
# Thu, 15 Jun 2023 04:23:03 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Thu, 15 Jun 2023 04:23:04 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 15 Jun 2023 04:23:05 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 15 Jun 2023 04:23:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 15 Jun 2023 04:23:05 GMT
USER memcache
# Thu, 15 Jun 2023 04:23:06 GMT
EXPOSE 11211
# Thu, 15 Jun 2023 04:23:06 GMT
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
	-	`sha256:b035d841131485b85fca254bc1f51878eeb4efb089ca292b6912144e0744dcfa`  
		Last Modified: Thu, 15 Jun 2023 04:23:37 GMT  
		Size: 982.8 KB (982821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49b24d1f64de4f01a1b2c94bbd8b53bfd5d55c0d2c842418f679f2dc3122f93d`  
		Last Modified: Thu, 15 Jun 2023 04:23:37 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:400968138d2a427cec2d804e2fb8b52908236f9823f026c8d3f5f90f5fbbed0b`  
		Last Modified: Thu, 15 Jun 2023 04:23:36 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-alpine3.18` - linux; s390x

```console
$ docker pull memcached@sha256:441c53da2edef09782ae8d67860d08a92c2c8c9e4abf7f0a48977db69a803953
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.3 MB (4278165 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1023dcfb4b4b8c4b0993be67253a28f023a74ff3b9eaa67976766f6d256f73a7`
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
# Thu, 15 Jun 2023 06:27:49 GMT
ENV MEMCACHED_VERSION=1.6.20
# Thu, 15 Jun 2023 06:27:50 GMT
ENV MEMCACHED_SHA1=face85ed6fad41432ad818445b24eca55bccdd78
# Thu, 15 Jun 2023 06:31:41 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Thu, 15 Jun 2023 06:31:42 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 15 Jun 2023 06:31:44 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 15 Jun 2023 06:31:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 15 Jun 2023 06:31:45 GMT
USER memcache
# Thu, 15 Jun 2023 06:31:45 GMT
EXPOSE 11211
# Thu, 15 Jun 2023 06:31:45 GMT
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
	-	`sha256:baa4da6084d6df86753b54ce48182165eb8c080ba843e13fa42fb2503ab59c27`  
		Last Modified: Thu, 15 Jun 2023 06:36:33 GMT  
		Size: 950.1 KB (950145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fc33101b6e87a2752ae5e82c32aa4480ef0000c174eb363eadfe98755991b38`  
		Last Modified: Thu, 15 Jun 2023 06:36:33 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c8630e5ca40a95cae4c251c954b07bae6331ac9d08eeff70d12d3263339dca0`  
		Last Modified: Thu, 15 Jun 2023 06:36:33 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:1-bookworm`

```console
$ docker pull memcached@sha256:8b7a3ce027c33dc2142b3826dae320dacdb9987fa86267c15505a80147f926b7
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
$ docker pull memcached@sha256:533c607824b2f5781b179e175fcdf055577a3f076fb0a0fdcd13487c7c92125f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.0 MB (38973406 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cbcfa8d0003c80b0bba4004f4b15b4a5600b9dd481ac2d887bc31e794f067464`
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
# Wed, 14 Jun 2023 20:48:24 GMT
ENV MEMCACHED_VERSION=1.6.20
# Wed, 14 Jun 2023 20:48:24 GMT
ENV MEMCACHED_SHA1=face85ed6fad41432ad818445b24eca55bccdd78
# Wed, 14 Jun 2023 20:50:40 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 14 Jun 2023 20:50:40 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 14 Jun 2023 20:50:41 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 14 Jun 2023 20:50:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Jun 2023 20:50:41 GMT
USER memcache
# Wed, 14 Jun 2023 20:50:41 GMT
EXPOSE 11211
# Wed, 14 Jun 2023 20:50:41 GMT
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
	-	`sha256:96a3de0d22592d9a254814d5b77e3a84e73d2f055d162503fe811f731a320701`  
		Last Modified: Wed, 14 Jun 2023 20:53:34 GMT  
		Size: 7.2 MB (7169888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a38b201fb7fc8d917459453ee1c0218cf9845c96b885a02b02999f81b21c6bb`  
		Last Modified: Wed, 14 Jun 2023 20:53:33 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6f5720dc1980c886ee7e8d6067ed87e102bb31824e557a85fbd54273542debf`  
		Last Modified: Wed, 14 Jun 2023 20:53:33 GMT  
		Size: 120.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-bookworm` - linux; arm variant v5

```console
$ docker pull memcached@sha256:bb4a530ed3dc36e702635724bf49a6703694d36a7bcfdeabb2b0d3ff6b101143
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.1 MB (35095204 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f00b0d176a0550d5b0d3f94dc00489066995ce4a1be3e688924144b9077256f`
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
# Wed, 14 Jun 2023 21:56:26 GMT
ENV MEMCACHED_VERSION=1.6.20
# Wed, 14 Jun 2023 21:56:27 GMT
ENV MEMCACHED_SHA1=face85ed6fad41432ad818445b24eca55bccdd78
# Wed, 14 Jun 2023 22:00:10 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 14 Jun 2023 22:00:10 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 14 Jun 2023 22:00:12 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 14 Jun 2023 22:00:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Jun 2023 22:00:12 GMT
USER memcache
# Wed, 14 Jun 2023 22:00:12 GMT
EXPOSE 11211
# Wed, 14 Jun 2023 22:00:13 GMT
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
	-	`sha256:feb8e13d6ab7efa5799bc12cdb4d8f410166028673257b803f31b6bc9d0eb70c`  
		Last Modified: Wed, 14 Jun 2023 22:00:42 GMT  
		Size: 5.8 MB (5829749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cf20cb3e5676ee2969940d8133531dcd0df55159ccb7dbd567cc83b2bc02384`  
		Last Modified: Wed, 14 Jun 2023 22:00:39 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04bc2d45321e126b2795ea784886ac10a0b3c5724ccf555f0d20f2c7ee4225f1`  
		Last Modified: Wed, 14 Jun 2023 22:00:39 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-bookworm` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:3464bfccdfad0dc788e056949d59fc0b665ec165654b3a8502a2f4a3868a3dc7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.9 MB (37872888 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:20f33353745665e05e1722aa9af40e06b3f58778f8e758e786eaad30054de61f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 12 Jun 2023 23:40:13 GMT
ADD file:f75c3fe22fec548b35a86a9a5802fdc97497f5d253cf630d65f13282169d3f3f in / 
# Mon, 12 Jun 2023 23:40:14 GMT
CMD ["bash"]
# Wed, 14 Jun 2023 20:54:33 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 14 Jun 2023 20:54:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 14 Jun 2023 20:54:37 GMT
ENV MEMCACHED_VERSION=1.6.20
# Wed, 14 Jun 2023 20:54:37 GMT
ENV MEMCACHED_SHA1=face85ed6fad41432ad818445b24eca55bccdd78
# Wed, 14 Jun 2023 20:57:13 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 14 Jun 2023 20:57:13 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 14 Jun 2023 20:57:14 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 14 Jun 2023 20:57:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Jun 2023 20:57:14 GMT
USER memcache
# Wed, 14 Jun 2023 20:57:14 GMT
EXPOSE 11211
# Wed, 14 Jun 2023 20:57:14 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:95039a22a7cc3ae41d71f075e6e09e91e8da850fb5f80aba2f4a09f254520539`  
		Last Modified: Mon, 12 Jun 2023 23:44:08 GMT  
		Size: 29.2 MB (29152534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6da70104cc8ee465752315034f04011354e6149243e2bc69b9da49e6855df4b8`  
		Last Modified: Wed, 14 Jun 2023 21:00:29 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a7b40152f53e05b8cbcfe09be5b1598fcc05cf4f9ffad3b296eca43305450da`  
		Last Modified: Wed, 14 Jun 2023 21:00:30 GMT  
		Size: 2.5 MB (2539179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bf09d04f9c61af195486f42915b137b8612584f982737f5e465d02648a6dc8a`  
		Last Modified: Wed, 14 Jun 2023 21:00:30 GMT  
		Size: 6.2 MB (6179640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e71555e51295eeceeab1a9ab6bebb21108fbbe59e01349857c51932deea0f64`  
		Last Modified: Wed, 14 Jun 2023 21:00:29 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15cd3195dbfc5cedaf71b7c156002599dfb94219b51f85c966a1bee80bc37e65`  
		Last Modified: Wed, 14 Jun 2023 21:00:29 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-bookworm` - linux; 386

```console
$ docker pull memcached@sha256:7c2fdc7c597b4f6efd737d9b8f1e78841cda31e4492a6ae32f3d6f1ab6911cb8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.5 MB (39457716 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a1e668084859e8f39e52c33d0d7a68506127f94d95c61ffb7f43f9441843fa3b`
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
# Wed, 14 Jun 2023 22:34:33 GMT
ENV MEMCACHED_VERSION=1.6.20
# Wed, 14 Jun 2023 22:34:33 GMT
ENV MEMCACHED_SHA1=face85ed6fad41432ad818445b24eca55bccdd78
# Wed, 14 Jun 2023 22:38:16 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 14 Jun 2023 22:38:17 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 14 Jun 2023 22:38:17 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 14 Jun 2023 22:38:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Jun 2023 22:38:17 GMT
USER memcache
# Wed, 14 Jun 2023 22:38:17 GMT
EXPOSE 11211
# Wed, 14 Jun 2023 22:38:18 GMT
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
	-	`sha256:2896f0aba2db45558c3b7f796cc22aa198f38d579fdc6ddf35893d5ea553c080`  
		Last Modified: Wed, 14 Jun 2023 22:42:10 GMT  
		Size: 6.6 MB (6630422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17e035509d03f0bd9a08582ab075babcb6e7dcbe048f9968c81ae996df72e6aa`  
		Last Modified: Wed, 14 Jun 2023 22:42:09 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc5b3164ed6a8d968b1da11795198c4d6ce05822ff371f41d2c7eb373d44141b`  
		Last Modified: Wed, 14 Jun 2023 22:42:09 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-bookworm` - linux; mips64le

```console
$ docker pull memcached@sha256:d2855c4deb19365dd1c83b81c9e1fa36f7873cc8b3dd02f8f01de10200bf208e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.6 MB (37554221 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7068fffc8ee0a4607e1586297977a273786efb52e1782f11396ee5f7a5150c0f`
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
# Wed, 14 Jun 2023 18:38:39 GMT
ENV MEMCACHED_VERSION=1.6.20
# Wed, 14 Jun 2023 18:38:41 GMT
ENV MEMCACHED_SHA1=face85ed6fad41432ad818445b24eca55bccdd78
# Wed, 14 Jun 2023 18:45:20 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 14 Jun 2023 18:45:23 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 14 Jun 2023 18:45:27 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 14 Jun 2023 18:45:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Jun 2023 18:45:32 GMT
USER memcache
# Wed, 14 Jun 2023 18:45:35 GMT
EXPOSE 11211
# Wed, 14 Jun 2023 18:45:38 GMT
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
	-	`sha256:76d4e9cc234d41e69eba3bf411cb1d3ebe17e2fefbffb0c3458d613f2545337e`  
		Last Modified: Wed, 14 Jun 2023 18:46:09 GMT  
		Size: 6.5 MB (6499709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0988c34e4840378b9876eba362b50458e769389d0cc626698bef65e46c721458`  
		Last Modified: Wed, 14 Jun 2023 18:46:04 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db55745458426cdf0d23fd0589fd440e2d328e4d5ffb00a9ef6d2e0225cec8bf`  
		Last Modified: Wed, 14 Jun 2023 18:46:04 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-bookworm` - linux; ppc64le

```console
$ docker pull memcached@sha256:0e023c41d9c6a8d04edad22ecea59cfcf424d0dc3895c442a9e7a4575961d53d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.2 MB (43193448 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a85a60b74a9575a203aba1a5f800dfe479b80cde8ff577ccd5e7e77bdaab64c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 12 Jun 2023 23:17:34 GMT
ADD file:3f8b9849acb625537f99921ef80190de7b03afdc287a5d1113a92cc41ae24be2 in / 
# Mon, 12 Jun 2023 23:17:36 GMT
CMD ["bash"]
# Wed, 14 Jun 2023 18:15:42 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 14 Jun 2023 18:15:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 14 Jun 2023 18:15:50 GMT
ENV MEMCACHED_VERSION=1.6.20
# Wed, 14 Jun 2023 18:15:51 GMT
ENV MEMCACHED_SHA1=face85ed6fad41432ad818445b24eca55bccdd78
# Wed, 14 Jun 2023 18:19:27 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 14 Jun 2023 18:19:28 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 14 Jun 2023 18:19:30 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 14 Jun 2023 18:19:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Jun 2023 18:19:31 GMT
USER memcache
# Wed, 14 Jun 2023 18:19:32 GMT
EXPOSE 11211
# Wed, 14 Jun 2023 18:19:32 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:9f041b53cef30007c43057f2520876c85ed6bee6be5aaee867dfb31a053d6cca`  
		Last Modified: Mon, 12 Jun 2023 23:24:09 GMT  
		Size: 33.1 MB (33116725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2a2d84b1fee81412bbd9bb301c77e6dfacfac70c2f1485de806658b49b06e08`  
		Last Modified: Wed, 14 Jun 2023 18:19:49 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca8bb5af043b48c9fe0e110ee13c139ceb715570346140fc86092d582d38b52b`  
		Last Modified: Wed, 14 Jun 2023 18:19:50 GMT  
		Size: 2.9 MB (2891306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e2d7805a151ec1618da95ad34cb2fdc6ae889b9f7908aaca6d063ca864f3e24`  
		Last Modified: Wed, 14 Jun 2023 18:19:52 GMT  
		Size: 7.2 MB (7183881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc5db4b315753422be0d08638f594b1ec64484c44f68942473f903387853b3bd`  
		Last Modified: Wed, 14 Jun 2023 18:19:49 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a8a9b2ed7c41d27d92f9db3c21beec2a2e288b0bc54a19aa1d3574b6085eaa6`  
		Last Modified: Wed, 14 Jun 2023 18:19:49 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-bookworm` - linux; s390x

```console
$ docker pull memcached@sha256:7bbe5a63846bc51d11850be291c164685b55f4d65a48ea07e8a6df50e489b658
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.9 MB (35907698 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d7e906c7eff45be64cda148363028a1270de09239533ca7dfee428108e20a155`
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
# Thu, 15 Jun 2023 06:23:29 GMT
ENV MEMCACHED_VERSION=1.6.20
# Thu, 15 Jun 2023 06:23:29 GMT
ENV MEMCACHED_SHA1=face85ed6fad41432ad818445b24eca55bccdd78
# Thu, 15 Jun 2023 06:26:33 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 15 Jun 2023 06:26:33 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 15 Jun 2023 06:26:34 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 15 Jun 2023 06:26:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 15 Jun 2023 06:26:35 GMT
USER memcache
# Thu, 15 Jun 2023 06:26:35 GMT
EXPOSE 11211
# Thu, 15 Jun 2023 06:26:35 GMT
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
	-	`sha256:a7ba1840ae9bcaa91375ac3b538e9ad379ec203bf9c6616bff06ec2a9ca6616a`  
		Last Modified: Thu, 15 Jun 2023 06:35:18 GMT  
		Size: 6.1 MB (6072893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d4533d005f06d7358727f3d1a167ee982d65ec08c863bd2171511918dab48d4`  
		Last Modified: Thu, 15 Jun 2023 06:35:17 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:769590255adfb1d384255f87732ddc4f78483e8203987ffba90f56f4102080e7`  
		Last Modified: Thu, 15 Jun 2023 06:35:17 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:1.6`

```console
$ docker pull memcached@sha256:791d3a3f4bed25f726ff2e0fea1bbc1038a5154dfadfc2d19cd2e8dd4c5a1a05
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
$ docker pull memcached@sha256:533c607824b2f5781b179e175fcdf055577a3f076fb0a0fdcd13487c7c92125f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.0 MB (38973406 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cbcfa8d0003c80b0bba4004f4b15b4a5600b9dd481ac2d887bc31e794f067464`
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
# Wed, 14 Jun 2023 20:48:24 GMT
ENV MEMCACHED_VERSION=1.6.20
# Wed, 14 Jun 2023 20:48:24 GMT
ENV MEMCACHED_SHA1=face85ed6fad41432ad818445b24eca55bccdd78
# Wed, 14 Jun 2023 20:50:40 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 14 Jun 2023 20:50:40 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 14 Jun 2023 20:50:41 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 14 Jun 2023 20:50:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Jun 2023 20:50:41 GMT
USER memcache
# Wed, 14 Jun 2023 20:50:41 GMT
EXPOSE 11211
# Wed, 14 Jun 2023 20:50:41 GMT
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
	-	`sha256:96a3de0d22592d9a254814d5b77e3a84e73d2f055d162503fe811f731a320701`  
		Last Modified: Wed, 14 Jun 2023 20:53:34 GMT  
		Size: 7.2 MB (7169888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a38b201fb7fc8d917459453ee1c0218cf9845c96b885a02b02999f81b21c6bb`  
		Last Modified: Wed, 14 Jun 2023 20:53:33 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6f5720dc1980c886ee7e8d6067ed87e102bb31824e557a85fbd54273542debf`  
		Last Modified: Wed, 14 Jun 2023 20:53:33 GMT  
		Size: 120.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6` - linux; arm variant v5

```console
$ docker pull memcached@sha256:bb4a530ed3dc36e702635724bf49a6703694d36a7bcfdeabb2b0d3ff6b101143
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.1 MB (35095204 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f00b0d176a0550d5b0d3f94dc00489066995ce4a1be3e688924144b9077256f`
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
# Wed, 14 Jun 2023 21:56:26 GMT
ENV MEMCACHED_VERSION=1.6.20
# Wed, 14 Jun 2023 21:56:27 GMT
ENV MEMCACHED_SHA1=face85ed6fad41432ad818445b24eca55bccdd78
# Wed, 14 Jun 2023 22:00:10 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 14 Jun 2023 22:00:10 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 14 Jun 2023 22:00:12 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 14 Jun 2023 22:00:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Jun 2023 22:00:12 GMT
USER memcache
# Wed, 14 Jun 2023 22:00:12 GMT
EXPOSE 11211
# Wed, 14 Jun 2023 22:00:13 GMT
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
	-	`sha256:feb8e13d6ab7efa5799bc12cdb4d8f410166028673257b803f31b6bc9d0eb70c`  
		Last Modified: Wed, 14 Jun 2023 22:00:42 GMT  
		Size: 5.8 MB (5829749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cf20cb3e5676ee2969940d8133531dcd0df55159ccb7dbd567cc83b2bc02384`  
		Last Modified: Wed, 14 Jun 2023 22:00:39 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04bc2d45321e126b2795ea784886ac10a0b3c5724ccf555f0d20f2c7ee4225f1`  
		Last Modified: Wed, 14 Jun 2023 22:00:39 GMT  
		Size: 121.0 B  
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
$ docker pull memcached@sha256:3464bfccdfad0dc788e056949d59fc0b665ec165654b3a8502a2f4a3868a3dc7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.9 MB (37872888 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:20f33353745665e05e1722aa9af40e06b3f58778f8e758e786eaad30054de61f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 12 Jun 2023 23:40:13 GMT
ADD file:f75c3fe22fec548b35a86a9a5802fdc97497f5d253cf630d65f13282169d3f3f in / 
# Mon, 12 Jun 2023 23:40:14 GMT
CMD ["bash"]
# Wed, 14 Jun 2023 20:54:33 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 14 Jun 2023 20:54:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 14 Jun 2023 20:54:37 GMT
ENV MEMCACHED_VERSION=1.6.20
# Wed, 14 Jun 2023 20:54:37 GMT
ENV MEMCACHED_SHA1=face85ed6fad41432ad818445b24eca55bccdd78
# Wed, 14 Jun 2023 20:57:13 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 14 Jun 2023 20:57:13 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 14 Jun 2023 20:57:14 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 14 Jun 2023 20:57:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Jun 2023 20:57:14 GMT
USER memcache
# Wed, 14 Jun 2023 20:57:14 GMT
EXPOSE 11211
# Wed, 14 Jun 2023 20:57:14 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:95039a22a7cc3ae41d71f075e6e09e91e8da850fb5f80aba2f4a09f254520539`  
		Last Modified: Mon, 12 Jun 2023 23:44:08 GMT  
		Size: 29.2 MB (29152534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6da70104cc8ee465752315034f04011354e6149243e2bc69b9da49e6855df4b8`  
		Last Modified: Wed, 14 Jun 2023 21:00:29 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a7b40152f53e05b8cbcfe09be5b1598fcc05cf4f9ffad3b296eca43305450da`  
		Last Modified: Wed, 14 Jun 2023 21:00:30 GMT  
		Size: 2.5 MB (2539179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bf09d04f9c61af195486f42915b137b8612584f982737f5e465d02648a6dc8a`  
		Last Modified: Wed, 14 Jun 2023 21:00:30 GMT  
		Size: 6.2 MB (6179640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e71555e51295eeceeab1a9ab6bebb21108fbbe59e01349857c51932deea0f64`  
		Last Modified: Wed, 14 Jun 2023 21:00:29 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15cd3195dbfc5cedaf71b7c156002599dfb94219b51f85c966a1bee80bc37e65`  
		Last Modified: Wed, 14 Jun 2023 21:00:29 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6` - linux; 386

```console
$ docker pull memcached@sha256:7c2fdc7c597b4f6efd737d9b8f1e78841cda31e4492a6ae32f3d6f1ab6911cb8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.5 MB (39457716 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a1e668084859e8f39e52c33d0d7a68506127f94d95c61ffb7f43f9441843fa3b`
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
# Wed, 14 Jun 2023 22:34:33 GMT
ENV MEMCACHED_VERSION=1.6.20
# Wed, 14 Jun 2023 22:34:33 GMT
ENV MEMCACHED_SHA1=face85ed6fad41432ad818445b24eca55bccdd78
# Wed, 14 Jun 2023 22:38:16 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 14 Jun 2023 22:38:17 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 14 Jun 2023 22:38:17 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 14 Jun 2023 22:38:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Jun 2023 22:38:17 GMT
USER memcache
# Wed, 14 Jun 2023 22:38:17 GMT
EXPOSE 11211
# Wed, 14 Jun 2023 22:38:18 GMT
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
	-	`sha256:2896f0aba2db45558c3b7f796cc22aa198f38d579fdc6ddf35893d5ea553c080`  
		Last Modified: Wed, 14 Jun 2023 22:42:10 GMT  
		Size: 6.6 MB (6630422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17e035509d03f0bd9a08582ab075babcb6e7dcbe048f9968c81ae996df72e6aa`  
		Last Modified: Wed, 14 Jun 2023 22:42:09 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc5b3164ed6a8d968b1da11795198c4d6ce05822ff371f41d2c7eb373d44141b`  
		Last Modified: Wed, 14 Jun 2023 22:42:09 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6` - linux; mips64le

```console
$ docker pull memcached@sha256:d2855c4deb19365dd1c83b81c9e1fa36f7873cc8b3dd02f8f01de10200bf208e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.6 MB (37554221 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7068fffc8ee0a4607e1586297977a273786efb52e1782f11396ee5f7a5150c0f`
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
# Wed, 14 Jun 2023 18:38:39 GMT
ENV MEMCACHED_VERSION=1.6.20
# Wed, 14 Jun 2023 18:38:41 GMT
ENV MEMCACHED_SHA1=face85ed6fad41432ad818445b24eca55bccdd78
# Wed, 14 Jun 2023 18:45:20 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 14 Jun 2023 18:45:23 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 14 Jun 2023 18:45:27 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 14 Jun 2023 18:45:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Jun 2023 18:45:32 GMT
USER memcache
# Wed, 14 Jun 2023 18:45:35 GMT
EXPOSE 11211
# Wed, 14 Jun 2023 18:45:38 GMT
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
	-	`sha256:76d4e9cc234d41e69eba3bf411cb1d3ebe17e2fefbffb0c3458d613f2545337e`  
		Last Modified: Wed, 14 Jun 2023 18:46:09 GMT  
		Size: 6.5 MB (6499709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0988c34e4840378b9876eba362b50458e769389d0cc626698bef65e46c721458`  
		Last Modified: Wed, 14 Jun 2023 18:46:04 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db55745458426cdf0d23fd0589fd440e2d328e4d5ffb00a9ef6d2e0225cec8bf`  
		Last Modified: Wed, 14 Jun 2023 18:46:04 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6` - linux; ppc64le

```console
$ docker pull memcached@sha256:0e023c41d9c6a8d04edad22ecea59cfcf424d0dc3895c442a9e7a4575961d53d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.2 MB (43193448 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a85a60b74a9575a203aba1a5f800dfe479b80cde8ff577ccd5e7e77bdaab64c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 12 Jun 2023 23:17:34 GMT
ADD file:3f8b9849acb625537f99921ef80190de7b03afdc287a5d1113a92cc41ae24be2 in / 
# Mon, 12 Jun 2023 23:17:36 GMT
CMD ["bash"]
# Wed, 14 Jun 2023 18:15:42 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 14 Jun 2023 18:15:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 14 Jun 2023 18:15:50 GMT
ENV MEMCACHED_VERSION=1.6.20
# Wed, 14 Jun 2023 18:15:51 GMT
ENV MEMCACHED_SHA1=face85ed6fad41432ad818445b24eca55bccdd78
# Wed, 14 Jun 2023 18:19:27 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 14 Jun 2023 18:19:28 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 14 Jun 2023 18:19:30 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 14 Jun 2023 18:19:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Jun 2023 18:19:31 GMT
USER memcache
# Wed, 14 Jun 2023 18:19:32 GMT
EXPOSE 11211
# Wed, 14 Jun 2023 18:19:32 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:9f041b53cef30007c43057f2520876c85ed6bee6be5aaee867dfb31a053d6cca`  
		Last Modified: Mon, 12 Jun 2023 23:24:09 GMT  
		Size: 33.1 MB (33116725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2a2d84b1fee81412bbd9bb301c77e6dfacfac70c2f1485de806658b49b06e08`  
		Last Modified: Wed, 14 Jun 2023 18:19:49 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca8bb5af043b48c9fe0e110ee13c139ceb715570346140fc86092d582d38b52b`  
		Last Modified: Wed, 14 Jun 2023 18:19:50 GMT  
		Size: 2.9 MB (2891306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e2d7805a151ec1618da95ad34cb2fdc6ae889b9f7908aaca6d063ca864f3e24`  
		Last Modified: Wed, 14 Jun 2023 18:19:52 GMT  
		Size: 7.2 MB (7183881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc5db4b315753422be0d08638f594b1ec64484c44f68942473f903387853b3bd`  
		Last Modified: Wed, 14 Jun 2023 18:19:49 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a8a9b2ed7c41d27d92f9db3c21beec2a2e288b0bc54a19aa1d3574b6085eaa6`  
		Last Modified: Wed, 14 Jun 2023 18:19:49 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6` - linux; s390x

```console
$ docker pull memcached@sha256:7bbe5a63846bc51d11850be291c164685b55f4d65a48ea07e8a6df50e489b658
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.9 MB (35907698 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d7e906c7eff45be64cda148363028a1270de09239533ca7dfee428108e20a155`
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
# Thu, 15 Jun 2023 06:23:29 GMT
ENV MEMCACHED_VERSION=1.6.20
# Thu, 15 Jun 2023 06:23:29 GMT
ENV MEMCACHED_SHA1=face85ed6fad41432ad818445b24eca55bccdd78
# Thu, 15 Jun 2023 06:26:33 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 15 Jun 2023 06:26:33 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 15 Jun 2023 06:26:34 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 15 Jun 2023 06:26:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 15 Jun 2023 06:26:35 GMT
USER memcache
# Thu, 15 Jun 2023 06:26:35 GMT
EXPOSE 11211
# Thu, 15 Jun 2023 06:26:35 GMT
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
	-	`sha256:a7ba1840ae9bcaa91375ac3b538e9ad379ec203bf9c6616bff06ec2a9ca6616a`  
		Last Modified: Thu, 15 Jun 2023 06:35:18 GMT  
		Size: 6.1 MB (6072893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d4533d005f06d7358727f3d1a167ee982d65ec08c863bd2171511918dab48d4`  
		Last Modified: Thu, 15 Jun 2023 06:35:17 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:769590255adfb1d384255f87732ddc4f78483e8203987ffba90f56f4102080e7`  
		Last Modified: Thu, 15 Jun 2023 06:35:17 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:1.6-alpine`

```console
$ docker pull memcached@sha256:bb867cdf4270f78a89270fab6532b2d27aa02dec52e62ba08d6cf02809ce37de
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
$ docker pull memcached@sha256:a7a04bc20ec122d9f024dff57494853d5dc9705fb97af9170cc31a1f531dcaa5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4462373 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:15429daa972e1d57884e75ecc7f784564ae7cf089c25671dd118a0025f806b6f`
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
# Wed, 14 Jun 2023 20:50:59 GMT
ENV MEMCACHED_VERSION=1.6.20
# Wed, 14 Jun 2023 20:50:59 GMT
ENV MEMCACHED_SHA1=face85ed6fad41432ad818445b24eca55bccdd78
# Wed, 14 Jun 2023 20:53:09 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Wed, 14 Jun 2023 20:53:09 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 14 Jun 2023 20:53:09 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 14 Jun 2023 20:53:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Jun 2023 20:53:09 GMT
USER memcache
# Wed, 14 Jun 2023 20:53:09 GMT
EXPOSE 11211
# Wed, 14 Jun 2023 20:53:09 GMT
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
	-	`sha256:bc06ea6ffc2a4279c91e26e37b450afb1e0f1007815b19a7146d52b016dddc61`  
		Last Modified: Wed, 14 Jun 2023 20:53:59 GMT  
		Size: 954.7 KB (954748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:098e9e56712cb64736718f40b476d8eeb9410130c28ce94fe1bc2d380d9083cf`  
		Last Modified: Wed, 14 Jun 2023 20:53:59 GMT  
		Size: 282.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5c14818f6fb630a615284b18f945c89c0563530c25f07af955d0f85504020e9`  
		Last Modified: Wed, 14 Jun 2023 20:53:58 GMT  
		Size: 118.0 B  
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
$ docker pull memcached@sha256:e59934ff7bef6e6053b618f65923d2c1fa7235a008fb20f4fe9db13f8d6dc167
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.4 MB (4399194 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dab6918acf63bcf26d1a95d40666c44f281aa14f0d4e27884d4c2f4b227dd9b3`
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
# Wed, 14 Jun 2023 20:57:27 GMT
ENV MEMCACHED_VERSION=1.6.20
# Wed, 14 Jun 2023 20:57:27 GMT
ENV MEMCACHED_SHA1=face85ed6fad41432ad818445b24eca55bccdd78
# Wed, 14 Jun 2023 20:59:54 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Wed, 14 Jun 2023 20:59:54 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 14 Jun 2023 20:59:55 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 14 Jun 2023 20:59:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Jun 2023 20:59:55 GMT
USER memcache
# Wed, 14 Jun 2023 20:59:55 GMT
EXPOSE 11211
# Wed, 14 Jun 2023 20:59:55 GMT
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
	-	`sha256:eddee3cdc367d6f8265fe941f97020460db6cb5555711640b2ad62bd5c2a613c`  
		Last Modified: Wed, 14 Jun 2023 21:00:51 GMT  
		Size: 944.1 KB (944138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfec1ffcd9427d8fb06b908c1d3e0715a9db99c94c46f7896890a98b95c5f049`  
		Last Modified: Wed, 14 Jun 2023 21:00:51 GMT  
		Size: 280.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aea835bd4a5d779b88da37bc977813dd1ed9d228f5e78e3459edde4fa6f155e2`  
		Last Modified: Wed, 14 Jun 2023 21:00:51 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-alpine` - linux; 386

```console
$ docker pull memcached@sha256:a919915b23bf734458584f42947ebf9a743a84c8c93d2e2ea784e1bc230aaa59
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.3 MB (4282199 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2764bc1af6a7d65fbfe6ad34b4c7d1799646f8d940c1b23b550f5b577d86b8b9`
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
# Wed, 14 Jun 2023 22:38:22 GMT
ENV MEMCACHED_VERSION=1.6.20
# Wed, 14 Jun 2023 22:38:22 GMT
ENV MEMCACHED_SHA1=face85ed6fad41432ad818445b24eca55bccdd78
# Wed, 14 Jun 2023 22:41:49 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Wed, 14 Jun 2023 22:41:49 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 14 Jun 2023 22:41:50 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 14 Jun 2023 22:41:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Jun 2023 22:41:50 GMT
USER memcache
# Wed, 14 Jun 2023 22:41:50 GMT
EXPOSE 11211
# Wed, 14 Jun 2023 22:41:50 GMT
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
	-	`sha256:e6eae361cc7d0f997a631fbe78920dacf40cb6d4751c30ee1692dbeac08bc37f`  
		Last Modified: Wed, 14 Jun 2023 22:42:32 GMT  
		Size: 937.0 KB (937049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26d07209b7ab8b880d78464e8fda28a770a3be477f9566a419967691b487705f`  
		Last Modified: Wed, 14 Jun 2023 22:42:32 GMT  
		Size: 280.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af5afdbe7d4d8e1bd1297aa2dfcdc690485f3965c75a5eb520d5681c789048c5`  
		Last Modified: Wed, 14 Jun 2023 22:42:32 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-alpine` - linux; ppc64le

```console
$ docker pull memcached@sha256:4ac2ba7993ef774f28a06c635dfb14927d19a5d624e1d935a9d17231df0f153f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4453208 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d545989d562d3df14a6b1e5f35cfa997c5f02dcbe213a92d66f3aaad767c1feb`
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
# Thu, 15 Jun 2023 04:20:03 GMT
ENV MEMCACHED_VERSION=1.6.20
# Thu, 15 Jun 2023 04:20:03 GMT
ENV MEMCACHED_SHA1=face85ed6fad41432ad818445b24eca55bccdd78
# Thu, 15 Jun 2023 04:23:03 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Thu, 15 Jun 2023 04:23:04 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 15 Jun 2023 04:23:05 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 15 Jun 2023 04:23:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 15 Jun 2023 04:23:05 GMT
USER memcache
# Thu, 15 Jun 2023 04:23:06 GMT
EXPOSE 11211
# Thu, 15 Jun 2023 04:23:06 GMT
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
	-	`sha256:b035d841131485b85fca254bc1f51878eeb4efb089ca292b6912144e0744dcfa`  
		Last Modified: Thu, 15 Jun 2023 04:23:37 GMT  
		Size: 982.8 KB (982821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49b24d1f64de4f01a1b2c94bbd8b53bfd5d55c0d2c842418f679f2dc3122f93d`  
		Last Modified: Thu, 15 Jun 2023 04:23:37 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:400968138d2a427cec2d804e2fb8b52908236f9823f026c8d3f5f90f5fbbed0b`  
		Last Modified: Thu, 15 Jun 2023 04:23:36 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-alpine` - linux; s390x

```console
$ docker pull memcached@sha256:441c53da2edef09782ae8d67860d08a92c2c8c9e4abf7f0a48977db69a803953
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.3 MB (4278165 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1023dcfb4b4b8c4b0993be67253a28f023a74ff3b9eaa67976766f6d256f73a7`
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
# Thu, 15 Jun 2023 06:27:49 GMT
ENV MEMCACHED_VERSION=1.6.20
# Thu, 15 Jun 2023 06:27:50 GMT
ENV MEMCACHED_SHA1=face85ed6fad41432ad818445b24eca55bccdd78
# Thu, 15 Jun 2023 06:31:41 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Thu, 15 Jun 2023 06:31:42 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 15 Jun 2023 06:31:44 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 15 Jun 2023 06:31:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 15 Jun 2023 06:31:45 GMT
USER memcache
# Thu, 15 Jun 2023 06:31:45 GMT
EXPOSE 11211
# Thu, 15 Jun 2023 06:31:45 GMT
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
	-	`sha256:baa4da6084d6df86753b54ce48182165eb8c080ba843e13fa42fb2503ab59c27`  
		Last Modified: Thu, 15 Jun 2023 06:36:33 GMT  
		Size: 950.1 KB (950145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fc33101b6e87a2752ae5e82c32aa4480ef0000c174eb363eadfe98755991b38`  
		Last Modified: Thu, 15 Jun 2023 06:36:33 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c8630e5ca40a95cae4c251c954b07bae6331ac9d08eeff70d12d3263339dca0`  
		Last Modified: Thu, 15 Jun 2023 06:36:33 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:1.6-alpine3.18`

```console
$ docker pull memcached@sha256:2943c39203d6df11309370bbd8e3896daddfac79f1a6414a9a9cc2381e70da81
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
$ docker pull memcached@sha256:a7a04bc20ec122d9f024dff57494853d5dc9705fb97af9170cc31a1f531dcaa5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4462373 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:15429daa972e1d57884e75ecc7f784564ae7cf089c25671dd118a0025f806b6f`
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
# Wed, 14 Jun 2023 20:50:59 GMT
ENV MEMCACHED_VERSION=1.6.20
# Wed, 14 Jun 2023 20:50:59 GMT
ENV MEMCACHED_SHA1=face85ed6fad41432ad818445b24eca55bccdd78
# Wed, 14 Jun 2023 20:53:09 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Wed, 14 Jun 2023 20:53:09 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 14 Jun 2023 20:53:09 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 14 Jun 2023 20:53:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Jun 2023 20:53:09 GMT
USER memcache
# Wed, 14 Jun 2023 20:53:09 GMT
EXPOSE 11211
# Wed, 14 Jun 2023 20:53:09 GMT
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
	-	`sha256:bc06ea6ffc2a4279c91e26e37b450afb1e0f1007815b19a7146d52b016dddc61`  
		Last Modified: Wed, 14 Jun 2023 20:53:59 GMT  
		Size: 954.7 KB (954748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:098e9e56712cb64736718f40b476d8eeb9410130c28ce94fe1bc2d380d9083cf`  
		Last Modified: Wed, 14 Jun 2023 20:53:59 GMT  
		Size: 282.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5c14818f6fb630a615284b18f945c89c0563530c25f07af955d0f85504020e9`  
		Last Modified: Wed, 14 Jun 2023 20:53:58 GMT  
		Size: 118.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-alpine3.18` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:e59934ff7bef6e6053b618f65923d2c1fa7235a008fb20f4fe9db13f8d6dc167
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.4 MB (4399194 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dab6918acf63bcf26d1a95d40666c44f281aa14f0d4e27884d4c2f4b227dd9b3`
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
# Wed, 14 Jun 2023 20:57:27 GMT
ENV MEMCACHED_VERSION=1.6.20
# Wed, 14 Jun 2023 20:57:27 GMT
ENV MEMCACHED_SHA1=face85ed6fad41432ad818445b24eca55bccdd78
# Wed, 14 Jun 2023 20:59:54 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Wed, 14 Jun 2023 20:59:54 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 14 Jun 2023 20:59:55 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 14 Jun 2023 20:59:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Jun 2023 20:59:55 GMT
USER memcache
# Wed, 14 Jun 2023 20:59:55 GMT
EXPOSE 11211
# Wed, 14 Jun 2023 20:59:55 GMT
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
	-	`sha256:eddee3cdc367d6f8265fe941f97020460db6cb5555711640b2ad62bd5c2a613c`  
		Last Modified: Wed, 14 Jun 2023 21:00:51 GMT  
		Size: 944.1 KB (944138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfec1ffcd9427d8fb06b908c1d3e0715a9db99c94c46f7896890a98b95c5f049`  
		Last Modified: Wed, 14 Jun 2023 21:00:51 GMT  
		Size: 280.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aea835bd4a5d779b88da37bc977813dd1ed9d228f5e78e3459edde4fa6f155e2`  
		Last Modified: Wed, 14 Jun 2023 21:00:51 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-alpine3.18` - linux; 386

```console
$ docker pull memcached@sha256:a919915b23bf734458584f42947ebf9a743a84c8c93d2e2ea784e1bc230aaa59
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.3 MB (4282199 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2764bc1af6a7d65fbfe6ad34b4c7d1799646f8d940c1b23b550f5b577d86b8b9`
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
# Wed, 14 Jun 2023 22:38:22 GMT
ENV MEMCACHED_VERSION=1.6.20
# Wed, 14 Jun 2023 22:38:22 GMT
ENV MEMCACHED_SHA1=face85ed6fad41432ad818445b24eca55bccdd78
# Wed, 14 Jun 2023 22:41:49 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Wed, 14 Jun 2023 22:41:49 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 14 Jun 2023 22:41:50 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 14 Jun 2023 22:41:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Jun 2023 22:41:50 GMT
USER memcache
# Wed, 14 Jun 2023 22:41:50 GMT
EXPOSE 11211
# Wed, 14 Jun 2023 22:41:50 GMT
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
	-	`sha256:e6eae361cc7d0f997a631fbe78920dacf40cb6d4751c30ee1692dbeac08bc37f`  
		Last Modified: Wed, 14 Jun 2023 22:42:32 GMT  
		Size: 937.0 KB (937049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26d07209b7ab8b880d78464e8fda28a770a3be477f9566a419967691b487705f`  
		Last Modified: Wed, 14 Jun 2023 22:42:32 GMT  
		Size: 280.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af5afdbe7d4d8e1bd1297aa2dfcdc690485f3965c75a5eb520d5681c789048c5`  
		Last Modified: Wed, 14 Jun 2023 22:42:32 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-alpine3.18` - linux; ppc64le

```console
$ docker pull memcached@sha256:4ac2ba7993ef774f28a06c635dfb14927d19a5d624e1d935a9d17231df0f153f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4453208 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d545989d562d3df14a6b1e5f35cfa997c5f02dcbe213a92d66f3aaad767c1feb`
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
# Thu, 15 Jun 2023 04:20:03 GMT
ENV MEMCACHED_VERSION=1.6.20
# Thu, 15 Jun 2023 04:20:03 GMT
ENV MEMCACHED_SHA1=face85ed6fad41432ad818445b24eca55bccdd78
# Thu, 15 Jun 2023 04:23:03 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Thu, 15 Jun 2023 04:23:04 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 15 Jun 2023 04:23:05 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 15 Jun 2023 04:23:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 15 Jun 2023 04:23:05 GMT
USER memcache
# Thu, 15 Jun 2023 04:23:06 GMT
EXPOSE 11211
# Thu, 15 Jun 2023 04:23:06 GMT
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
	-	`sha256:b035d841131485b85fca254bc1f51878eeb4efb089ca292b6912144e0744dcfa`  
		Last Modified: Thu, 15 Jun 2023 04:23:37 GMT  
		Size: 982.8 KB (982821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49b24d1f64de4f01a1b2c94bbd8b53bfd5d55c0d2c842418f679f2dc3122f93d`  
		Last Modified: Thu, 15 Jun 2023 04:23:37 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:400968138d2a427cec2d804e2fb8b52908236f9823f026c8d3f5f90f5fbbed0b`  
		Last Modified: Thu, 15 Jun 2023 04:23:36 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-alpine3.18` - linux; s390x

```console
$ docker pull memcached@sha256:441c53da2edef09782ae8d67860d08a92c2c8c9e4abf7f0a48977db69a803953
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.3 MB (4278165 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1023dcfb4b4b8c4b0993be67253a28f023a74ff3b9eaa67976766f6d256f73a7`
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
# Thu, 15 Jun 2023 06:27:49 GMT
ENV MEMCACHED_VERSION=1.6.20
# Thu, 15 Jun 2023 06:27:50 GMT
ENV MEMCACHED_SHA1=face85ed6fad41432ad818445b24eca55bccdd78
# Thu, 15 Jun 2023 06:31:41 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Thu, 15 Jun 2023 06:31:42 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 15 Jun 2023 06:31:44 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 15 Jun 2023 06:31:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 15 Jun 2023 06:31:45 GMT
USER memcache
# Thu, 15 Jun 2023 06:31:45 GMT
EXPOSE 11211
# Thu, 15 Jun 2023 06:31:45 GMT
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
	-	`sha256:baa4da6084d6df86753b54ce48182165eb8c080ba843e13fa42fb2503ab59c27`  
		Last Modified: Thu, 15 Jun 2023 06:36:33 GMT  
		Size: 950.1 KB (950145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fc33101b6e87a2752ae5e82c32aa4480ef0000c174eb363eadfe98755991b38`  
		Last Modified: Thu, 15 Jun 2023 06:36:33 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c8630e5ca40a95cae4c251c954b07bae6331ac9d08eeff70d12d3263339dca0`  
		Last Modified: Thu, 15 Jun 2023 06:36:33 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:1.6-bookworm`

```console
$ docker pull memcached@sha256:8b7a3ce027c33dc2142b3826dae320dacdb9987fa86267c15505a80147f926b7
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
$ docker pull memcached@sha256:533c607824b2f5781b179e175fcdf055577a3f076fb0a0fdcd13487c7c92125f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.0 MB (38973406 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cbcfa8d0003c80b0bba4004f4b15b4a5600b9dd481ac2d887bc31e794f067464`
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
# Wed, 14 Jun 2023 20:48:24 GMT
ENV MEMCACHED_VERSION=1.6.20
# Wed, 14 Jun 2023 20:48:24 GMT
ENV MEMCACHED_SHA1=face85ed6fad41432ad818445b24eca55bccdd78
# Wed, 14 Jun 2023 20:50:40 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 14 Jun 2023 20:50:40 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 14 Jun 2023 20:50:41 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 14 Jun 2023 20:50:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Jun 2023 20:50:41 GMT
USER memcache
# Wed, 14 Jun 2023 20:50:41 GMT
EXPOSE 11211
# Wed, 14 Jun 2023 20:50:41 GMT
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
	-	`sha256:96a3de0d22592d9a254814d5b77e3a84e73d2f055d162503fe811f731a320701`  
		Last Modified: Wed, 14 Jun 2023 20:53:34 GMT  
		Size: 7.2 MB (7169888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a38b201fb7fc8d917459453ee1c0218cf9845c96b885a02b02999f81b21c6bb`  
		Last Modified: Wed, 14 Jun 2023 20:53:33 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6f5720dc1980c886ee7e8d6067ed87e102bb31824e557a85fbd54273542debf`  
		Last Modified: Wed, 14 Jun 2023 20:53:33 GMT  
		Size: 120.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-bookworm` - linux; arm variant v5

```console
$ docker pull memcached@sha256:bb4a530ed3dc36e702635724bf49a6703694d36a7bcfdeabb2b0d3ff6b101143
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.1 MB (35095204 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f00b0d176a0550d5b0d3f94dc00489066995ce4a1be3e688924144b9077256f`
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
# Wed, 14 Jun 2023 21:56:26 GMT
ENV MEMCACHED_VERSION=1.6.20
# Wed, 14 Jun 2023 21:56:27 GMT
ENV MEMCACHED_SHA1=face85ed6fad41432ad818445b24eca55bccdd78
# Wed, 14 Jun 2023 22:00:10 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 14 Jun 2023 22:00:10 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 14 Jun 2023 22:00:12 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 14 Jun 2023 22:00:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Jun 2023 22:00:12 GMT
USER memcache
# Wed, 14 Jun 2023 22:00:12 GMT
EXPOSE 11211
# Wed, 14 Jun 2023 22:00:13 GMT
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
	-	`sha256:feb8e13d6ab7efa5799bc12cdb4d8f410166028673257b803f31b6bc9d0eb70c`  
		Last Modified: Wed, 14 Jun 2023 22:00:42 GMT  
		Size: 5.8 MB (5829749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cf20cb3e5676ee2969940d8133531dcd0df55159ccb7dbd567cc83b2bc02384`  
		Last Modified: Wed, 14 Jun 2023 22:00:39 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04bc2d45321e126b2795ea784886ac10a0b3c5724ccf555f0d20f2c7ee4225f1`  
		Last Modified: Wed, 14 Jun 2023 22:00:39 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-bookworm` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:3464bfccdfad0dc788e056949d59fc0b665ec165654b3a8502a2f4a3868a3dc7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.9 MB (37872888 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:20f33353745665e05e1722aa9af40e06b3f58778f8e758e786eaad30054de61f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 12 Jun 2023 23:40:13 GMT
ADD file:f75c3fe22fec548b35a86a9a5802fdc97497f5d253cf630d65f13282169d3f3f in / 
# Mon, 12 Jun 2023 23:40:14 GMT
CMD ["bash"]
# Wed, 14 Jun 2023 20:54:33 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 14 Jun 2023 20:54:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 14 Jun 2023 20:54:37 GMT
ENV MEMCACHED_VERSION=1.6.20
# Wed, 14 Jun 2023 20:54:37 GMT
ENV MEMCACHED_SHA1=face85ed6fad41432ad818445b24eca55bccdd78
# Wed, 14 Jun 2023 20:57:13 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 14 Jun 2023 20:57:13 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 14 Jun 2023 20:57:14 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 14 Jun 2023 20:57:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Jun 2023 20:57:14 GMT
USER memcache
# Wed, 14 Jun 2023 20:57:14 GMT
EXPOSE 11211
# Wed, 14 Jun 2023 20:57:14 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:95039a22a7cc3ae41d71f075e6e09e91e8da850fb5f80aba2f4a09f254520539`  
		Last Modified: Mon, 12 Jun 2023 23:44:08 GMT  
		Size: 29.2 MB (29152534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6da70104cc8ee465752315034f04011354e6149243e2bc69b9da49e6855df4b8`  
		Last Modified: Wed, 14 Jun 2023 21:00:29 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a7b40152f53e05b8cbcfe09be5b1598fcc05cf4f9ffad3b296eca43305450da`  
		Last Modified: Wed, 14 Jun 2023 21:00:30 GMT  
		Size: 2.5 MB (2539179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bf09d04f9c61af195486f42915b137b8612584f982737f5e465d02648a6dc8a`  
		Last Modified: Wed, 14 Jun 2023 21:00:30 GMT  
		Size: 6.2 MB (6179640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e71555e51295eeceeab1a9ab6bebb21108fbbe59e01349857c51932deea0f64`  
		Last Modified: Wed, 14 Jun 2023 21:00:29 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15cd3195dbfc5cedaf71b7c156002599dfb94219b51f85c966a1bee80bc37e65`  
		Last Modified: Wed, 14 Jun 2023 21:00:29 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-bookworm` - linux; 386

```console
$ docker pull memcached@sha256:7c2fdc7c597b4f6efd737d9b8f1e78841cda31e4492a6ae32f3d6f1ab6911cb8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.5 MB (39457716 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a1e668084859e8f39e52c33d0d7a68506127f94d95c61ffb7f43f9441843fa3b`
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
# Wed, 14 Jun 2023 22:34:33 GMT
ENV MEMCACHED_VERSION=1.6.20
# Wed, 14 Jun 2023 22:34:33 GMT
ENV MEMCACHED_SHA1=face85ed6fad41432ad818445b24eca55bccdd78
# Wed, 14 Jun 2023 22:38:16 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 14 Jun 2023 22:38:17 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 14 Jun 2023 22:38:17 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 14 Jun 2023 22:38:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Jun 2023 22:38:17 GMT
USER memcache
# Wed, 14 Jun 2023 22:38:17 GMT
EXPOSE 11211
# Wed, 14 Jun 2023 22:38:18 GMT
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
	-	`sha256:2896f0aba2db45558c3b7f796cc22aa198f38d579fdc6ddf35893d5ea553c080`  
		Last Modified: Wed, 14 Jun 2023 22:42:10 GMT  
		Size: 6.6 MB (6630422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17e035509d03f0bd9a08582ab075babcb6e7dcbe048f9968c81ae996df72e6aa`  
		Last Modified: Wed, 14 Jun 2023 22:42:09 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc5b3164ed6a8d968b1da11795198c4d6ce05822ff371f41d2c7eb373d44141b`  
		Last Modified: Wed, 14 Jun 2023 22:42:09 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-bookworm` - linux; mips64le

```console
$ docker pull memcached@sha256:d2855c4deb19365dd1c83b81c9e1fa36f7873cc8b3dd02f8f01de10200bf208e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.6 MB (37554221 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7068fffc8ee0a4607e1586297977a273786efb52e1782f11396ee5f7a5150c0f`
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
# Wed, 14 Jun 2023 18:38:39 GMT
ENV MEMCACHED_VERSION=1.6.20
# Wed, 14 Jun 2023 18:38:41 GMT
ENV MEMCACHED_SHA1=face85ed6fad41432ad818445b24eca55bccdd78
# Wed, 14 Jun 2023 18:45:20 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 14 Jun 2023 18:45:23 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 14 Jun 2023 18:45:27 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 14 Jun 2023 18:45:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Jun 2023 18:45:32 GMT
USER memcache
# Wed, 14 Jun 2023 18:45:35 GMT
EXPOSE 11211
# Wed, 14 Jun 2023 18:45:38 GMT
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
	-	`sha256:76d4e9cc234d41e69eba3bf411cb1d3ebe17e2fefbffb0c3458d613f2545337e`  
		Last Modified: Wed, 14 Jun 2023 18:46:09 GMT  
		Size: 6.5 MB (6499709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0988c34e4840378b9876eba362b50458e769389d0cc626698bef65e46c721458`  
		Last Modified: Wed, 14 Jun 2023 18:46:04 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db55745458426cdf0d23fd0589fd440e2d328e4d5ffb00a9ef6d2e0225cec8bf`  
		Last Modified: Wed, 14 Jun 2023 18:46:04 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-bookworm` - linux; ppc64le

```console
$ docker pull memcached@sha256:0e023c41d9c6a8d04edad22ecea59cfcf424d0dc3895c442a9e7a4575961d53d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.2 MB (43193448 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a85a60b74a9575a203aba1a5f800dfe479b80cde8ff577ccd5e7e77bdaab64c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 12 Jun 2023 23:17:34 GMT
ADD file:3f8b9849acb625537f99921ef80190de7b03afdc287a5d1113a92cc41ae24be2 in / 
# Mon, 12 Jun 2023 23:17:36 GMT
CMD ["bash"]
# Wed, 14 Jun 2023 18:15:42 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 14 Jun 2023 18:15:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 14 Jun 2023 18:15:50 GMT
ENV MEMCACHED_VERSION=1.6.20
# Wed, 14 Jun 2023 18:15:51 GMT
ENV MEMCACHED_SHA1=face85ed6fad41432ad818445b24eca55bccdd78
# Wed, 14 Jun 2023 18:19:27 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 14 Jun 2023 18:19:28 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 14 Jun 2023 18:19:30 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 14 Jun 2023 18:19:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Jun 2023 18:19:31 GMT
USER memcache
# Wed, 14 Jun 2023 18:19:32 GMT
EXPOSE 11211
# Wed, 14 Jun 2023 18:19:32 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:9f041b53cef30007c43057f2520876c85ed6bee6be5aaee867dfb31a053d6cca`  
		Last Modified: Mon, 12 Jun 2023 23:24:09 GMT  
		Size: 33.1 MB (33116725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2a2d84b1fee81412bbd9bb301c77e6dfacfac70c2f1485de806658b49b06e08`  
		Last Modified: Wed, 14 Jun 2023 18:19:49 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca8bb5af043b48c9fe0e110ee13c139ceb715570346140fc86092d582d38b52b`  
		Last Modified: Wed, 14 Jun 2023 18:19:50 GMT  
		Size: 2.9 MB (2891306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e2d7805a151ec1618da95ad34cb2fdc6ae889b9f7908aaca6d063ca864f3e24`  
		Last Modified: Wed, 14 Jun 2023 18:19:52 GMT  
		Size: 7.2 MB (7183881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc5db4b315753422be0d08638f594b1ec64484c44f68942473f903387853b3bd`  
		Last Modified: Wed, 14 Jun 2023 18:19:49 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a8a9b2ed7c41d27d92f9db3c21beec2a2e288b0bc54a19aa1d3574b6085eaa6`  
		Last Modified: Wed, 14 Jun 2023 18:19:49 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-bookworm` - linux; s390x

```console
$ docker pull memcached@sha256:7bbe5a63846bc51d11850be291c164685b55f4d65a48ea07e8a6df50e489b658
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.9 MB (35907698 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d7e906c7eff45be64cda148363028a1270de09239533ca7dfee428108e20a155`
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
# Thu, 15 Jun 2023 06:23:29 GMT
ENV MEMCACHED_VERSION=1.6.20
# Thu, 15 Jun 2023 06:23:29 GMT
ENV MEMCACHED_SHA1=face85ed6fad41432ad818445b24eca55bccdd78
# Thu, 15 Jun 2023 06:26:33 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 15 Jun 2023 06:26:33 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 15 Jun 2023 06:26:34 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 15 Jun 2023 06:26:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 15 Jun 2023 06:26:35 GMT
USER memcache
# Thu, 15 Jun 2023 06:26:35 GMT
EXPOSE 11211
# Thu, 15 Jun 2023 06:26:35 GMT
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
	-	`sha256:a7ba1840ae9bcaa91375ac3b538e9ad379ec203bf9c6616bff06ec2a9ca6616a`  
		Last Modified: Thu, 15 Jun 2023 06:35:18 GMT  
		Size: 6.1 MB (6072893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d4533d005f06d7358727f3d1a167ee982d65ec08c863bd2171511918dab48d4`  
		Last Modified: Thu, 15 Jun 2023 06:35:17 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:769590255adfb1d384255f87732ddc4f78483e8203987ffba90f56f4102080e7`  
		Last Modified: Thu, 15 Jun 2023 06:35:17 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:1.6.20`

```console
$ docker pull memcached@sha256:8b7a3ce027c33dc2142b3826dae320dacdb9987fa86267c15505a80147f926b7
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

### `memcached:1.6.20` - linux; amd64

```console
$ docker pull memcached@sha256:533c607824b2f5781b179e175fcdf055577a3f076fb0a0fdcd13487c7c92125f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.0 MB (38973406 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cbcfa8d0003c80b0bba4004f4b15b4a5600b9dd481ac2d887bc31e794f067464`
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
# Wed, 14 Jun 2023 20:48:24 GMT
ENV MEMCACHED_VERSION=1.6.20
# Wed, 14 Jun 2023 20:48:24 GMT
ENV MEMCACHED_SHA1=face85ed6fad41432ad818445b24eca55bccdd78
# Wed, 14 Jun 2023 20:50:40 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 14 Jun 2023 20:50:40 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 14 Jun 2023 20:50:41 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 14 Jun 2023 20:50:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Jun 2023 20:50:41 GMT
USER memcache
# Wed, 14 Jun 2023 20:50:41 GMT
EXPOSE 11211
# Wed, 14 Jun 2023 20:50:41 GMT
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
	-	`sha256:96a3de0d22592d9a254814d5b77e3a84e73d2f055d162503fe811f731a320701`  
		Last Modified: Wed, 14 Jun 2023 20:53:34 GMT  
		Size: 7.2 MB (7169888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a38b201fb7fc8d917459453ee1c0218cf9845c96b885a02b02999f81b21c6bb`  
		Last Modified: Wed, 14 Jun 2023 20:53:33 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6f5720dc1980c886ee7e8d6067ed87e102bb31824e557a85fbd54273542debf`  
		Last Modified: Wed, 14 Jun 2023 20:53:33 GMT  
		Size: 120.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.20` - linux; arm variant v5

```console
$ docker pull memcached@sha256:bb4a530ed3dc36e702635724bf49a6703694d36a7bcfdeabb2b0d3ff6b101143
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.1 MB (35095204 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f00b0d176a0550d5b0d3f94dc00489066995ce4a1be3e688924144b9077256f`
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
# Wed, 14 Jun 2023 21:56:26 GMT
ENV MEMCACHED_VERSION=1.6.20
# Wed, 14 Jun 2023 21:56:27 GMT
ENV MEMCACHED_SHA1=face85ed6fad41432ad818445b24eca55bccdd78
# Wed, 14 Jun 2023 22:00:10 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 14 Jun 2023 22:00:10 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 14 Jun 2023 22:00:12 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 14 Jun 2023 22:00:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Jun 2023 22:00:12 GMT
USER memcache
# Wed, 14 Jun 2023 22:00:12 GMT
EXPOSE 11211
# Wed, 14 Jun 2023 22:00:13 GMT
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
	-	`sha256:feb8e13d6ab7efa5799bc12cdb4d8f410166028673257b803f31b6bc9d0eb70c`  
		Last Modified: Wed, 14 Jun 2023 22:00:42 GMT  
		Size: 5.8 MB (5829749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cf20cb3e5676ee2969940d8133531dcd0df55159ccb7dbd567cc83b2bc02384`  
		Last Modified: Wed, 14 Jun 2023 22:00:39 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04bc2d45321e126b2795ea784886ac10a0b3c5724ccf555f0d20f2c7ee4225f1`  
		Last Modified: Wed, 14 Jun 2023 22:00:39 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.20` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:3464bfccdfad0dc788e056949d59fc0b665ec165654b3a8502a2f4a3868a3dc7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.9 MB (37872888 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:20f33353745665e05e1722aa9af40e06b3f58778f8e758e786eaad30054de61f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 12 Jun 2023 23:40:13 GMT
ADD file:f75c3fe22fec548b35a86a9a5802fdc97497f5d253cf630d65f13282169d3f3f in / 
# Mon, 12 Jun 2023 23:40:14 GMT
CMD ["bash"]
# Wed, 14 Jun 2023 20:54:33 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 14 Jun 2023 20:54:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 14 Jun 2023 20:54:37 GMT
ENV MEMCACHED_VERSION=1.6.20
# Wed, 14 Jun 2023 20:54:37 GMT
ENV MEMCACHED_SHA1=face85ed6fad41432ad818445b24eca55bccdd78
# Wed, 14 Jun 2023 20:57:13 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 14 Jun 2023 20:57:13 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 14 Jun 2023 20:57:14 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 14 Jun 2023 20:57:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Jun 2023 20:57:14 GMT
USER memcache
# Wed, 14 Jun 2023 20:57:14 GMT
EXPOSE 11211
# Wed, 14 Jun 2023 20:57:14 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:95039a22a7cc3ae41d71f075e6e09e91e8da850fb5f80aba2f4a09f254520539`  
		Last Modified: Mon, 12 Jun 2023 23:44:08 GMT  
		Size: 29.2 MB (29152534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6da70104cc8ee465752315034f04011354e6149243e2bc69b9da49e6855df4b8`  
		Last Modified: Wed, 14 Jun 2023 21:00:29 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a7b40152f53e05b8cbcfe09be5b1598fcc05cf4f9ffad3b296eca43305450da`  
		Last Modified: Wed, 14 Jun 2023 21:00:30 GMT  
		Size: 2.5 MB (2539179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bf09d04f9c61af195486f42915b137b8612584f982737f5e465d02648a6dc8a`  
		Last Modified: Wed, 14 Jun 2023 21:00:30 GMT  
		Size: 6.2 MB (6179640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e71555e51295eeceeab1a9ab6bebb21108fbbe59e01349857c51932deea0f64`  
		Last Modified: Wed, 14 Jun 2023 21:00:29 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15cd3195dbfc5cedaf71b7c156002599dfb94219b51f85c966a1bee80bc37e65`  
		Last Modified: Wed, 14 Jun 2023 21:00:29 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.20` - linux; 386

```console
$ docker pull memcached@sha256:7c2fdc7c597b4f6efd737d9b8f1e78841cda31e4492a6ae32f3d6f1ab6911cb8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.5 MB (39457716 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a1e668084859e8f39e52c33d0d7a68506127f94d95c61ffb7f43f9441843fa3b`
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
# Wed, 14 Jun 2023 22:34:33 GMT
ENV MEMCACHED_VERSION=1.6.20
# Wed, 14 Jun 2023 22:34:33 GMT
ENV MEMCACHED_SHA1=face85ed6fad41432ad818445b24eca55bccdd78
# Wed, 14 Jun 2023 22:38:16 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 14 Jun 2023 22:38:17 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 14 Jun 2023 22:38:17 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 14 Jun 2023 22:38:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Jun 2023 22:38:17 GMT
USER memcache
# Wed, 14 Jun 2023 22:38:17 GMT
EXPOSE 11211
# Wed, 14 Jun 2023 22:38:18 GMT
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
	-	`sha256:2896f0aba2db45558c3b7f796cc22aa198f38d579fdc6ddf35893d5ea553c080`  
		Last Modified: Wed, 14 Jun 2023 22:42:10 GMT  
		Size: 6.6 MB (6630422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17e035509d03f0bd9a08582ab075babcb6e7dcbe048f9968c81ae996df72e6aa`  
		Last Modified: Wed, 14 Jun 2023 22:42:09 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc5b3164ed6a8d968b1da11795198c4d6ce05822ff371f41d2c7eb373d44141b`  
		Last Modified: Wed, 14 Jun 2023 22:42:09 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.20` - linux; mips64le

```console
$ docker pull memcached@sha256:d2855c4deb19365dd1c83b81c9e1fa36f7873cc8b3dd02f8f01de10200bf208e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.6 MB (37554221 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7068fffc8ee0a4607e1586297977a273786efb52e1782f11396ee5f7a5150c0f`
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
# Wed, 14 Jun 2023 18:38:39 GMT
ENV MEMCACHED_VERSION=1.6.20
# Wed, 14 Jun 2023 18:38:41 GMT
ENV MEMCACHED_SHA1=face85ed6fad41432ad818445b24eca55bccdd78
# Wed, 14 Jun 2023 18:45:20 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 14 Jun 2023 18:45:23 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 14 Jun 2023 18:45:27 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 14 Jun 2023 18:45:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Jun 2023 18:45:32 GMT
USER memcache
# Wed, 14 Jun 2023 18:45:35 GMT
EXPOSE 11211
# Wed, 14 Jun 2023 18:45:38 GMT
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
	-	`sha256:76d4e9cc234d41e69eba3bf411cb1d3ebe17e2fefbffb0c3458d613f2545337e`  
		Last Modified: Wed, 14 Jun 2023 18:46:09 GMT  
		Size: 6.5 MB (6499709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0988c34e4840378b9876eba362b50458e769389d0cc626698bef65e46c721458`  
		Last Modified: Wed, 14 Jun 2023 18:46:04 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db55745458426cdf0d23fd0589fd440e2d328e4d5ffb00a9ef6d2e0225cec8bf`  
		Last Modified: Wed, 14 Jun 2023 18:46:04 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.20` - linux; ppc64le

```console
$ docker pull memcached@sha256:0e023c41d9c6a8d04edad22ecea59cfcf424d0dc3895c442a9e7a4575961d53d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.2 MB (43193448 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a85a60b74a9575a203aba1a5f800dfe479b80cde8ff577ccd5e7e77bdaab64c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 12 Jun 2023 23:17:34 GMT
ADD file:3f8b9849acb625537f99921ef80190de7b03afdc287a5d1113a92cc41ae24be2 in / 
# Mon, 12 Jun 2023 23:17:36 GMT
CMD ["bash"]
# Wed, 14 Jun 2023 18:15:42 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 14 Jun 2023 18:15:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 14 Jun 2023 18:15:50 GMT
ENV MEMCACHED_VERSION=1.6.20
# Wed, 14 Jun 2023 18:15:51 GMT
ENV MEMCACHED_SHA1=face85ed6fad41432ad818445b24eca55bccdd78
# Wed, 14 Jun 2023 18:19:27 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 14 Jun 2023 18:19:28 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 14 Jun 2023 18:19:30 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 14 Jun 2023 18:19:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Jun 2023 18:19:31 GMT
USER memcache
# Wed, 14 Jun 2023 18:19:32 GMT
EXPOSE 11211
# Wed, 14 Jun 2023 18:19:32 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:9f041b53cef30007c43057f2520876c85ed6bee6be5aaee867dfb31a053d6cca`  
		Last Modified: Mon, 12 Jun 2023 23:24:09 GMT  
		Size: 33.1 MB (33116725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2a2d84b1fee81412bbd9bb301c77e6dfacfac70c2f1485de806658b49b06e08`  
		Last Modified: Wed, 14 Jun 2023 18:19:49 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca8bb5af043b48c9fe0e110ee13c139ceb715570346140fc86092d582d38b52b`  
		Last Modified: Wed, 14 Jun 2023 18:19:50 GMT  
		Size: 2.9 MB (2891306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e2d7805a151ec1618da95ad34cb2fdc6ae889b9f7908aaca6d063ca864f3e24`  
		Last Modified: Wed, 14 Jun 2023 18:19:52 GMT  
		Size: 7.2 MB (7183881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc5db4b315753422be0d08638f594b1ec64484c44f68942473f903387853b3bd`  
		Last Modified: Wed, 14 Jun 2023 18:19:49 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a8a9b2ed7c41d27d92f9db3c21beec2a2e288b0bc54a19aa1d3574b6085eaa6`  
		Last Modified: Wed, 14 Jun 2023 18:19:49 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.20` - linux; s390x

```console
$ docker pull memcached@sha256:7bbe5a63846bc51d11850be291c164685b55f4d65a48ea07e8a6df50e489b658
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.9 MB (35907698 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d7e906c7eff45be64cda148363028a1270de09239533ca7dfee428108e20a155`
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
# Thu, 15 Jun 2023 06:23:29 GMT
ENV MEMCACHED_VERSION=1.6.20
# Thu, 15 Jun 2023 06:23:29 GMT
ENV MEMCACHED_SHA1=face85ed6fad41432ad818445b24eca55bccdd78
# Thu, 15 Jun 2023 06:26:33 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 15 Jun 2023 06:26:33 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 15 Jun 2023 06:26:34 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 15 Jun 2023 06:26:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 15 Jun 2023 06:26:35 GMT
USER memcache
# Thu, 15 Jun 2023 06:26:35 GMT
EXPOSE 11211
# Thu, 15 Jun 2023 06:26:35 GMT
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
	-	`sha256:a7ba1840ae9bcaa91375ac3b538e9ad379ec203bf9c6616bff06ec2a9ca6616a`  
		Last Modified: Thu, 15 Jun 2023 06:35:18 GMT  
		Size: 6.1 MB (6072893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d4533d005f06d7358727f3d1a167ee982d65ec08c863bd2171511918dab48d4`  
		Last Modified: Thu, 15 Jun 2023 06:35:17 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:769590255adfb1d384255f87732ddc4f78483e8203987ffba90f56f4102080e7`  
		Last Modified: Thu, 15 Jun 2023 06:35:17 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:1.6.20-alpine`

```console
$ docker pull memcached@sha256:2943c39203d6df11309370bbd8e3896daddfac79f1a6414a9a9cc2381e70da81
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `memcached:1.6.20-alpine` - linux; amd64

```console
$ docker pull memcached@sha256:a7a04bc20ec122d9f024dff57494853d5dc9705fb97af9170cc31a1f531dcaa5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4462373 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:15429daa972e1d57884e75ecc7f784564ae7cf089c25671dd118a0025f806b6f`
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
# Wed, 14 Jun 2023 20:50:59 GMT
ENV MEMCACHED_VERSION=1.6.20
# Wed, 14 Jun 2023 20:50:59 GMT
ENV MEMCACHED_SHA1=face85ed6fad41432ad818445b24eca55bccdd78
# Wed, 14 Jun 2023 20:53:09 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Wed, 14 Jun 2023 20:53:09 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 14 Jun 2023 20:53:09 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 14 Jun 2023 20:53:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Jun 2023 20:53:09 GMT
USER memcache
# Wed, 14 Jun 2023 20:53:09 GMT
EXPOSE 11211
# Wed, 14 Jun 2023 20:53:09 GMT
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
	-	`sha256:bc06ea6ffc2a4279c91e26e37b450afb1e0f1007815b19a7146d52b016dddc61`  
		Last Modified: Wed, 14 Jun 2023 20:53:59 GMT  
		Size: 954.7 KB (954748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:098e9e56712cb64736718f40b476d8eeb9410130c28ce94fe1bc2d380d9083cf`  
		Last Modified: Wed, 14 Jun 2023 20:53:59 GMT  
		Size: 282.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5c14818f6fb630a615284b18f945c89c0563530c25f07af955d0f85504020e9`  
		Last Modified: Wed, 14 Jun 2023 20:53:58 GMT  
		Size: 118.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.20-alpine` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:e59934ff7bef6e6053b618f65923d2c1fa7235a008fb20f4fe9db13f8d6dc167
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.4 MB (4399194 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dab6918acf63bcf26d1a95d40666c44f281aa14f0d4e27884d4c2f4b227dd9b3`
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
# Wed, 14 Jun 2023 20:57:27 GMT
ENV MEMCACHED_VERSION=1.6.20
# Wed, 14 Jun 2023 20:57:27 GMT
ENV MEMCACHED_SHA1=face85ed6fad41432ad818445b24eca55bccdd78
# Wed, 14 Jun 2023 20:59:54 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Wed, 14 Jun 2023 20:59:54 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 14 Jun 2023 20:59:55 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 14 Jun 2023 20:59:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Jun 2023 20:59:55 GMT
USER memcache
# Wed, 14 Jun 2023 20:59:55 GMT
EXPOSE 11211
# Wed, 14 Jun 2023 20:59:55 GMT
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
	-	`sha256:eddee3cdc367d6f8265fe941f97020460db6cb5555711640b2ad62bd5c2a613c`  
		Last Modified: Wed, 14 Jun 2023 21:00:51 GMT  
		Size: 944.1 KB (944138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfec1ffcd9427d8fb06b908c1d3e0715a9db99c94c46f7896890a98b95c5f049`  
		Last Modified: Wed, 14 Jun 2023 21:00:51 GMT  
		Size: 280.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aea835bd4a5d779b88da37bc977813dd1ed9d228f5e78e3459edde4fa6f155e2`  
		Last Modified: Wed, 14 Jun 2023 21:00:51 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.20-alpine` - linux; 386

```console
$ docker pull memcached@sha256:a919915b23bf734458584f42947ebf9a743a84c8c93d2e2ea784e1bc230aaa59
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.3 MB (4282199 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2764bc1af6a7d65fbfe6ad34b4c7d1799646f8d940c1b23b550f5b577d86b8b9`
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
# Wed, 14 Jun 2023 22:38:22 GMT
ENV MEMCACHED_VERSION=1.6.20
# Wed, 14 Jun 2023 22:38:22 GMT
ENV MEMCACHED_SHA1=face85ed6fad41432ad818445b24eca55bccdd78
# Wed, 14 Jun 2023 22:41:49 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Wed, 14 Jun 2023 22:41:49 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 14 Jun 2023 22:41:50 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 14 Jun 2023 22:41:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Jun 2023 22:41:50 GMT
USER memcache
# Wed, 14 Jun 2023 22:41:50 GMT
EXPOSE 11211
# Wed, 14 Jun 2023 22:41:50 GMT
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
	-	`sha256:e6eae361cc7d0f997a631fbe78920dacf40cb6d4751c30ee1692dbeac08bc37f`  
		Last Modified: Wed, 14 Jun 2023 22:42:32 GMT  
		Size: 937.0 KB (937049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26d07209b7ab8b880d78464e8fda28a770a3be477f9566a419967691b487705f`  
		Last Modified: Wed, 14 Jun 2023 22:42:32 GMT  
		Size: 280.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af5afdbe7d4d8e1bd1297aa2dfcdc690485f3965c75a5eb520d5681c789048c5`  
		Last Modified: Wed, 14 Jun 2023 22:42:32 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.20-alpine` - linux; ppc64le

```console
$ docker pull memcached@sha256:4ac2ba7993ef774f28a06c635dfb14927d19a5d624e1d935a9d17231df0f153f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4453208 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d545989d562d3df14a6b1e5f35cfa997c5f02dcbe213a92d66f3aaad767c1feb`
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
# Thu, 15 Jun 2023 04:20:03 GMT
ENV MEMCACHED_VERSION=1.6.20
# Thu, 15 Jun 2023 04:20:03 GMT
ENV MEMCACHED_SHA1=face85ed6fad41432ad818445b24eca55bccdd78
# Thu, 15 Jun 2023 04:23:03 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Thu, 15 Jun 2023 04:23:04 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 15 Jun 2023 04:23:05 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 15 Jun 2023 04:23:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 15 Jun 2023 04:23:05 GMT
USER memcache
# Thu, 15 Jun 2023 04:23:06 GMT
EXPOSE 11211
# Thu, 15 Jun 2023 04:23:06 GMT
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
	-	`sha256:b035d841131485b85fca254bc1f51878eeb4efb089ca292b6912144e0744dcfa`  
		Last Modified: Thu, 15 Jun 2023 04:23:37 GMT  
		Size: 982.8 KB (982821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49b24d1f64de4f01a1b2c94bbd8b53bfd5d55c0d2c842418f679f2dc3122f93d`  
		Last Modified: Thu, 15 Jun 2023 04:23:37 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:400968138d2a427cec2d804e2fb8b52908236f9823f026c8d3f5f90f5fbbed0b`  
		Last Modified: Thu, 15 Jun 2023 04:23:36 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.20-alpine` - linux; s390x

```console
$ docker pull memcached@sha256:441c53da2edef09782ae8d67860d08a92c2c8c9e4abf7f0a48977db69a803953
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.3 MB (4278165 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1023dcfb4b4b8c4b0993be67253a28f023a74ff3b9eaa67976766f6d256f73a7`
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
# Thu, 15 Jun 2023 06:27:49 GMT
ENV MEMCACHED_VERSION=1.6.20
# Thu, 15 Jun 2023 06:27:50 GMT
ENV MEMCACHED_SHA1=face85ed6fad41432ad818445b24eca55bccdd78
# Thu, 15 Jun 2023 06:31:41 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Thu, 15 Jun 2023 06:31:42 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 15 Jun 2023 06:31:44 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 15 Jun 2023 06:31:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 15 Jun 2023 06:31:45 GMT
USER memcache
# Thu, 15 Jun 2023 06:31:45 GMT
EXPOSE 11211
# Thu, 15 Jun 2023 06:31:45 GMT
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
	-	`sha256:baa4da6084d6df86753b54ce48182165eb8c080ba843e13fa42fb2503ab59c27`  
		Last Modified: Thu, 15 Jun 2023 06:36:33 GMT  
		Size: 950.1 KB (950145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fc33101b6e87a2752ae5e82c32aa4480ef0000c174eb363eadfe98755991b38`  
		Last Modified: Thu, 15 Jun 2023 06:36:33 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c8630e5ca40a95cae4c251c954b07bae6331ac9d08eeff70d12d3263339dca0`  
		Last Modified: Thu, 15 Jun 2023 06:36:33 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:1.6.20-alpine3.18`

```console
$ docker pull memcached@sha256:2943c39203d6df11309370bbd8e3896daddfac79f1a6414a9a9cc2381e70da81
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `memcached:1.6.20-alpine3.18` - linux; amd64

```console
$ docker pull memcached@sha256:a7a04bc20ec122d9f024dff57494853d5dc9705fb97af9170cc31a1f531dcaa5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4462373 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:15429daa972e1d57884e75ecc7f784564ae7cf089c25671dd118a0025f806b6f`
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
# Wed, 14 Jun 2023 20:50:59 GMT
ENV MEMCACHED_VERSION=1.6.20
# Wed, 14 Jun 2023 20:50:59 GMT
ENV MEMCACHED_SHA1=face85ed6fad41432ad818445b24eca55bccdd78
# Wed, 14 Jun 2023 20:53:09 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Wed, 14 Jun 2023 20:53:09 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 14 Jun 2023 20:53:09 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 14 Jun 2023 20:53:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Jun 2023 20:53:09 GMT
USER memcache
# Wed, 14 Jun 2023 20:53:09 GMT
EXPOSE 11211
# Wed, 14 Jun 2023 20:53:09 GMT
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
	-	`sha256:bc06ea6ffc2a4279c91e26e37b450afb1e0f1007815b19a7146d52b016dddc61`  
		Last Modified: Wed, 14 Jun 2023 20:53:59 GMT  
		Size: 954.7 KB (954748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:098e9e56712cb64736718f40b476d8eeb9410130c28ce94fe1bc2d380d9083cf`  
		Last Modified: Wed, 14 Jun 2023 20:53:59 GMT  
		Size: 282.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5c14818f6fb630a615284b18f945c89c0563530c25f07af955d0f85504020e9`  
		Last Modified: Wed, 14 Jun 2023 20:53:58 GMT  
		Size: 118.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.20-alpine3.18` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:e59934ff7bef6e6053b618f65923d2c1fa7235a008fb20f4fe9db13f8d6dc167
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.4 MB (4399194 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dab6918acf63bcf26d1a95d40666c44f281aa14f0d4e27884d4c2f4b227dd9b3`
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
# Wed, 14 Jun 2023 20:57:27 GMT
ENV MEMCACHED_VERSION=1.6.20
# Wed, 14 Jun 2023 20:57:27 GMT
ENV MEMCACHED_SHA1=face85ed6fad41432ad818445b24eca55bccdd78
# Wed, 14 Jun 2023 20:59:54 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Wed, 14 Jun 2023 20:59:54 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 14 Jun 2023 20:59:55 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 14 Jun 2023 20:59:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Jun 2023 20:59:55 GMT
USER memcache
# Wed, 14 Jun 2023 20:59:55 GMT
EXPOSE 11211
# Wed, 14 Jun 2023 20:59:55 GMT
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
	-	`sha256:eddee3cdc367d6f8265fe941f97020460db6cb5555711640b2ad62bd5c2a613c`  
		Last Modified: Wed, 14 Jun 2023 21:00:51 GMT  
		Size: 944.1 KB (944138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfec1ffcd9427d8fb06b908c1d3e0715a9db99c94c46f7896890a98b95c5f049`  
		Last Modified: Wed, 14 Jun 2023 21:00:51 GMT  
		Size: 280.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aea835bd4a5d779b88da37bc977813dd1ed9d228f5e78e3459edde4fa6f155e2`  
		Last Modified: Wed, 14 Jun 2023 21:00:51 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.20-alpine3.18` - linux; 386

```console
$ docker pull memcached@sha256:a919915b23bf734458584f42947ebf9a743a84c8c93d2e2ea784e1bc230aaa59
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.3 MB (4282199 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2764bc1af6a7d65fbfe6ad34b4c7d1799646f8d940c1b23b550f5b577d86b8b9`
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
# Wed, 14 Jun 2023 22:38:22 GMT
ENV MEMCACHED_VERSION=1.6.20
# Wed, 14 Jun 2023 22:38:22 GMT
ENV MEMCACHED_SHA1=face85ed6fad41432ad818445b24eca55bccdd78
# Wed, 14 Jun 2023 22:41:49 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Wed, 14 Jun 2023 22:41:49 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 14 Jun 2023 22:41:50 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 14 Jun 2023 22:41:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Jun 2023 22:41:50 GMT
USER memcache
# Wed, 14 Jun 2023 22:41:50 GMT
EXPOSE 11211
# Wed, 14 Jun 2023 22:41:50 GMT
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
	-	`sha256:e6eae361cc7d0f997a631fbe78920dacf40cb6d4751c30ee1692dbeac08bc37f`  
		Last Modified: Wed, 14 Jun 2023 22:42:32 GMT  
		Size: 937.0 KB (937049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26d07209b7ab8b880d78464e8fda28a770a3be477f9566a419967691b487705f`  
		Last Modified: Wed, 14 Jun 2023 22:42:32 GMT  
		Size: 280.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af5afdbe7d4d8e1bd1297aa2dfcdc690485f3965c75a5eb520d5681c789048c5`  
		Last Modified: Wed, 14 Jun 2023 22:42:32 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.20-alpine3.18` - linux; ppc64le

```console
$ docker pull memcached@sha256:4ac2ba7993ef774f28a06c635dfb14927d19a5d624e1d935a9d17231df0f153f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4453208 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d545989d562d3df14a6b1e5f35cfa997c5f02dcbe213a92d66f3aaad767c1feb`
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
# Thu, 15 Jun 2023 04:20:03 GMT
ENV MEMCACHED_VERSION=1.6.20
# Thu, 15 Jun 2023 04:20:03 GMT
ENV MEMCACHED_SHA1=face85ed6fad41432ad818445b24eca55bccdd78
# Thu, 15 Jun 2023 04:23:03 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Thu, 15 Jun 2023 04:23:04 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 15 Jun 2023 04:23:05 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 15 Jun 2023 04:23:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 15 Jun 2023 04:23:05 GMT
USER memcache
# Thu, 15 Jun 2023 04:23:06 GMT
EXPOSE 11211
# Thu, 15 Jun 2023 04:23:06 GMT
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
	-	`sha256:b035d841131485b85fca254bc1f51878eeb4efb089ca292b6912144e0744dcfa`  
		Last Modified: Thu, 15 Jun 2023 04:23:37 GMT  
		Size: 982.8 KB (982821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49b24d1f64de4f01a1b2c94bbd8b53bfd5d55c0d2c842418f679f2dc3122f93d`  
		Last Modified: Thu, 15 Jun 2023 04:23:37 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:400968138d2a427cec2d804e2fb8b52908236f9823f026c8d3f5f90f5fbbed0b`  
		Last Modified: Thu, 15 Jun 2023 04:23:36 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.20-alpine3.18` - linux; s390x

```console
$ docker pull memcached@sha256:441c53da2edef09782ae8d67860d08a92c2c8c9e4abf7f0a48977db69a803953
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.3 MB (4278165 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1023dcfb4b4b8c4b0993be67253a28f023a74ff3b9eaa67976766f6d256f73a7`
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
# Thu, 15 Jun 2023 06:27:49 GMT
ENV MEMCACHED_VERSION=1.6.20
# Thu, 15 Jun 2023 06:27:50 GMT
ENV MEMCACHED_SHA1=face85ed6fad41432ad818445b24eca55bccdd78
# Thu, 15 Jun 2023 06:31:41 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Thu, 15 Jun 2023 06:31:42 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 15 Jun 2023 06:31:44 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 15 Jun 2023 06:31:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 15 Jun 2023 06:31:45 GMT
USER memcache
# Thu, 15 Jun 2023 06:31:45 GMT
EXPOSE 11211
# Thu, 15 Jun 2023 06:31:45 GMT
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
	-	`sha256:baa4da6084d6df86753b54ce48182165eb8c080ba843e13fa42fb2503ab59c27`  
		Last Modified: Thu, 15 Jun 2023 06:36:33 GMT  
		Size: 950.1 KB (950145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fc33101b6e87a2752ae5e82c32aa4480ef0000c174eb363eadfe98755991b38`  
		Last Modified: Thu, 15 Jun 2023 06:36:33 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c8630e5ca40a95cae4c251c954b07bae6331ac9d08eeff70d12d3263339dca0`  
		Last Modified: Thu, 15 Jun 2023 06:36:33 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:1.6.20-bookworm`

```console
$ docker pull memcached@sha256:8b7a3ce027c33dc2142b3826dae320dacdb9987fa86267c15505a80147f926b7
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

### `memcached:1.6.20-bookworm` - linux; amd64

```console
$ docker pull memcached@sha256:533c607824b2f5781b179e175fcdf055577a3f076fb0a0fdcd13487c7c92125f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.0 MB (38973406 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cbcfa8d0003c80b0bba4004f4b15b4a5600b9dd481ac2d887bc31e794f067464`
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
# Wed, 14 Jun 2023 20:48:24 GMT
ENV MEMCACHED_VERSION=1.6.20
# Wed, 14 Jun 2023 20:48:24 GMT
ENV MEMCACHED_SHA1=face85ed6fad41432ad818445b24eca55bccdd78
# Wed, 14 Jun 2023 20:50:40 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 14 Jun 2023 20:50:40 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 14 Jun 2023 20:50:41 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 14 Jun 2023 20:50:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Jun 2023 20:50:41 GMT
USER memcache
# Wed, 14 Jun 2023 20:50:41 GMT
EXPOSE 11211
# Wed, 14 Jun 2023 20:50:41 GMT
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
	-	`sha256:96a3de0d22592d9a254814d5b77e3a84e73d2f055d162503fe811f731a320701`  
		Last Modified: Wed, 14 Jun 2023 20:53:34 GMT  
		Size: 7.2 MB (7169888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a38b201fb7fc8d917459453ee1c0218cf9845c96b885a02b02999f81b21c6bb`  
		Last Modified: Wed, 14 Jun 2023 20:53:33 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6f5720dc1980c886ee7e8d6067ed87e102bb31824e557a85fbd54273542debf`  
		Last Modified: Wed, 14 Jun 2023 20:53:33 GMT  
		Size: 120.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.20-bookworm` - linux; arm variant v5

```console
$ docker pull memcached@sha256:bb4a530ed3dc36e702635724bf49a6703694d36a7bcfdeabb2b0d3ff6b101143
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.1 MB (35095204 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f00b0d176a0550d5b0d3f94dc00489066995ce4a1be3e688924144b9077256f`
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
# Wed, 14 Jun 2023 21:56:26 GMT
ENV MEMCACHED_VERSION=1.6.20
# Wed, 14 Jun 2023 21:56:27 GMT
ENV MEMCACHED_SHA1=face85ed6fad41432ad818445b24eca55bccdd78
# Wed, 14 Jun 2023 22:00:10 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 14 Jun 2023 22:00:10 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 14 Jun 2023 22:00:12 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 14 Jun 2023 22:00:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Jun 2023 22:00:12 GMT
USER memcache
# Wed, 14 Jun 2023 22:00:12 GMT
EXPOSE 11211
# Wed, 14 Jun 2023 22:00:13 GMT
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
	-	`sha256:feb8e13d6ab7efa5799bc12cdb4d8f410166028673257b803f31b6bc9d0eb70c`  
		Last Modified: Wed, 14 Jun 2023 22:00:42 GMT  
		Size: 5.8 MB (5829749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cf20cb3e5676ee2969940d8133531dcd0df55159ccb7dbd567cc83b2bc02384`  
		Last Modified: Wed, 14 Jun 2023 22:00:39 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04bc2d45321e126b2795ea784886ac10a0b3c5724ccf555f0d20f2c7ee4225f1`  
		Last Modified: Wed, 14 Jun 2023 22:00:39 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.20-bookworm` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:3464bfccdfad0dc788e056949d59fc0b665ec165654b3a8502a2f4a3868a3dc7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.9 MB (37872888 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:20f33353745665e05e1722aa9af40e06b3f58778f8e758e786eaad30054de61f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 12 Jun 2023 23:40:13 GMT
ADD file:f75c3fe22fec548b35a86a9a5802fdc97497f5d253cf630d65f13282169d3f3f in / 
# Mon, 12 Jun 2023 23:40:14 GMT
CMD ["bash"]
# Wed, 14 Jun 2023 20:54:33 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 14 Jun 2023 20:54:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 14 Jun 2023 20:54:37 GMT
ENV MEMCACHED_VERSION=1.6.20
# Wed, 14 Jun 2023 20:54:37 GMT
ENV MEMCACHED_SHA1=face85ed6fad41432ad818445b24eca55bccdd78
# Wed, 14 Jun 2023 20:57:13 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 14 Jun 2023 20:57:13 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 14 Jun 2023 20:57:14 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 14 Jun 2023 20:57:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Jun 2023 20:57:14 GMT
USER memcache
# Wed, 14 Jun 2023 20:57:14 GMT
EXPOSE 11211
# Wed, 14 Jun 2023 20:57:14 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:95039a22a7cc3ae41d71f075e6e09e91e8da850fb5f80aba2f4a09f254520539`  
		Last Modified: Mon, 12 Jun 2023 23:44:08 GMT  
		Size: 29.2 MB (29152534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6da70104cc8ee465752315034f04011354e6149243e2bc69b9da49e6855df4b8`  
		Last Modified: Wed, 14 Jun 2023 21:00:29 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a7b40152f53e05b8cbcfe09be5b1598fcc05cf4f9ffad3b296eca43305450da`  
		Last Modified: Wed, 14 Jun 2023 21:00:30 GMT  
		Size: 2.5 MB (2539179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bf09d04f9c61af195486f42915b137b8612584f982737f5e465d02648a6dc8a`  
		Last Modified: Wed, 14 Jun 2023 21:00:30 GMT  
		Size: 6.2 MB (6179640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e71555e51295eeceeab1a9ab6bebb21108fbbe59e01349857c51932deea0f64`  
		Last Modified: Wed, 14 Jun 2023 21:00:29 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15cd3195dbfc5cedaf71b7c156002599dfb94219b51f85c966a1bee80bc37e65`  
		Last Modified: Wed, 14 Jun 2023 21:00:29 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.20-bookworm` - linux; 386

```console
$ docker pull memcached@sha256:7c2fdc7c597b4f6efd737d9b8f1e78841cda31e4492a6ae32f3d6f1ab6911cb8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.5 MB (39457716 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a1e668084859e8f39e52c33d0d7a68506127f94d95c61ffb7f43f9441843fa3b`
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
# Wed, 14 Jun 2023 22:34:33 GMT
ENV MEMCACHED_VERSION=1.6.20
# Wed, 14 Jun 2023 22:34:33 GMT
ENV MEMCACHED_SHA1=face85ed6fad41432ad818445b24eca55bccdd78
# Wed, 14 Jun 2023 22:38:16 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 14 Jun 2023 22:38:17 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 14 Jun 2023 22:38:17 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 14 Jun 2023 22:38:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Jun 2023 22:38:17 GMT
USER memcache
# Wed, 14 Jun 2023 22:38:17 GMT
EXPOSE 11211
# Wed, 14 Jun 2023 22:38:18 GMT
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
	-	`sha256:2896f0aba2db45558c3b7f796cc22aa198f38d579fdc6ddf35893d5ea553c080`  
		Last Modified: Wed, 14 Jun 2023 22:42:10 GMT  
		Size: 6.6 MB (6630422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17e035509d03f0bd9a08582ab075babcb6e7dcbe048f9968c81ae996df72e6aa`  
		Last Modified: Wed, 14 Jun 2023 22:42:09 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc5b3164ed6a8d968b1da11795198c4d6ce05822ff371f41d2c7eb373d44141b`  
		Last Modified: Wed, 14 Jun 2023 22:42:09 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.20-bookworm` - linux; mips64le

```console
$ docker pull memcached@sha256:d2855c4deb19365dd1c83b81c9e1fa36f7873cc8b3dd02f8f01de10200bf208e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.6 MB (37554221 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7068fffc8ee0a4607e1586297977a273786efb52e1782f11396ee5f7a5150c0f`
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
# Wed, 14 Jun 2023 18:38:39 GMT
ENV MEMCACHED_VERSION=1.6.20
# Wed, 14 Jun 2023 18:38:41 GMT
ENV MEMCACHED_SHA1=face85ed6fad41432ad818445b24eca55bccdd78
# Wed, 14 Jun 2023 18:45:20 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 14 Jun 2023 18:45:23 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 14 Jun 2023 18:45:27 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 14 Jun 2023 18:45:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Jun 2023 18:45:32 GMT
USER memcache
# Wed, 14 Jun 2023 18:45:35 GMT
EXPOSE 11211
# Wed, 14 Jun 2023 18:45:38 GMT
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
	-	`sha256:76d4e9cc234d41e69eba3bf411cb1d3ebe17e2fefbffb0c3458d613f2545337e`  
		Last Modified: Wed, 14 Jun 2023 18:46:09 GMT  
		Size: 6.5 MB (6499709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0988c34e4840378b9876eba362b50458e769389d0cc626698bef65e46c721458`  
		Last Modified: Wed, 14 Jun 2023 18:46:04 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db55745458426cdf0d23fd0589fd440e2d328e4d5ffb00a9ef6d2e0225cec8bf`  
		Last Modified: Wed, 14 Jun 2023 18:46:04 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.20-bookworm` - linux; ppc64le

```console
$ docker pull memcached@sha256:0e023c41d9c6a8d04edad22ecea59cfcf424d0dc3895c442a9e7a4575961d53d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.2 MB (43193448 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a85a60b74a9575a203aba1a5f800dfe479b80cde8ff577ccd5e7e77bdaab64c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 12 Jun 2023 23:17:34 GMT
ADD file:3f8b9849acb625537f99921ef80190de7b03afdc287a5d1113a92cc41ae24be2 in / 
# Mon, 12 Jun 2023 23:17:36 GMT
CMD ["bash"]
# Wed, 14 Jun 2023 18:15:42 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 14 Jun 2023 18:15:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 14 Jun 2023 18:15:50 GMT
ENV MEMCACHED_VERSION=1.6.20
# Wed, 14 Jun 2023 18:15:51 GMT
ENV MEMCACHED_SHA1=face85ed6fad41432ad818445b24eca55bccdd78
# Wed, 14 Jun 2023 18:19:27 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 14 Jun 2023 18:19:28 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 14 Jun 2023 18:19:30 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 14 Jun 2023 18:19:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Jun 2023 18:19:31 GMT
USER memcache
# Wed, 14 Jun 2023 18:19:32 GMT
EXPOSE 11211
# Wed, 14 Jun 2023 18:19:32 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:9f041b53cef30007c43057f2520876c85ed6bee6be5aaee867dfb31a053d6cca`  
		Last Modified: Mon, 12 Jun 2023 23:24:09 GMT  
		Size: 33.1 MB (33116725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2a2d84b1fee81412bbd9bb301c77e6dfacfac70c2f1485de806658b49b06e08`  
		Last Modified: Wed, 14 Jun 2023 18:19:49 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca8bb5af043b48c9fe0e110ee13c139ceb715570346140fc86092d582d38b52b`  
		Last Modified: Wed, 14 Jun 2023 18:19:50 GMT  
		Size: 2.9 MB (2891306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e2d7805a151ec1618da95ad34cb2fdc6ae889b9f7908aaca6d063ca864f3e24`  
		Last Modified: Wed, 14 Jun 2023 18:19:52 GMT  
		Size: 7.2 MB (7183881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc5db4b315753422be0d08638f594b1ec64484c44f68942473f903387853b3bd`  
		Last Modified: Wed, 14 Jun 2023 18:19:49 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a8a9b2ed7c41d27d92f9db3c21beec2a2e288b0bc54a19aa1d3574b6085eaa6`  
		Last Modified: Wed, 14 Jun 2023 18:19:49 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.20-bookworm` - linux; s390x

```console
$ docker pull memcached@sha256:7bbe5a63846bc51d11850be291c164685b55f4d65a48ea07e8a6df50e489b658
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.9 MB (35907698 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d7e906c7eff45be64cda148363028a1270de09239533ca7dfee428108e20a155`
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
# Thu, 15 Jun 2023 06:23:29 GMT
ENV MEMCACHED_VERSION=1.6.20
# Thu, 15 Jun 2023 06:23:29 GMT
ENV MEMCACHED_SHA1=face85ed6fad41432ad818445b24eca55bccdd78
# Thu, 15 Jun 2023 06:26:33 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 15 Jun 2023 06:26:33 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 15 Jun 2023 06:26:34 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 15 Jun 2023 06:26:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 15 Jun 2023 06:26:35 GMT
USER memcache
# Thu, 15 Jun 2023 06:26:35 GMT
EXPOSE 11211
# Thu, 15 Jun 2023 06:26:35 GMT
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
	-	`sha256:a7ba1840ae9bcaa91375ac3b538e9ad379ec203bf9c6616bff06ec2a9ca6616a`  
		Last Modified: Thu, 15 Jun 2023 06:35:18 GMT  
		Size: 6.1 MB (6072893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d4533d005f06d7358727f3d1a167ee982d65ec08c863bd2171511918dab48d4`  
		Last Modified: Thu, 15 Jun 2023 06:35:17 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:769590255adfb1d384255f87732ddc4f78483e8203987ffba90f56f4102080e7`  
		Last Modified: Thu, 15 Jun 2023 06:35:17 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:alpine`

```console
$ docker pull memcached@sha256:bb867cdf4270f78a89270fab6532b2d27aa02dec52e62ba08d6cf02809ce37de
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
$ docker pull memcached@sha256:a7a04bc20ec122d9f024dff57494853d5dc9705fb97af9170cc31a1f531dcaa5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4462373 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:15429daa972e1d57884e75ecc7f784564ae7cf089c25671dd118a0025f806b6f`
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
# Wed, 14 Jun 2023 20:50:59 GMT
ENV MEMCACHED_VERSION=1.6.20
# Wed, 14 Jun 2023 20:50:59 GMT
ENV MEMCACHED_SHA1=face85ed6fad41432ad818445b24eca55bccdd78
# Wed, 14 Jun 2023 20:53:09 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Wed, 14 Jun 2023 20:53:09 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 14 Jun 2023 20:53:09 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 14 Jun 2023 20:53:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Jun 2023 20:53:09 GMT
USER memcache
# Wed, 14 Jun 2023 20:53:09 GMT
EXPOSE 11211
# Wed, 14 Jun 2023 20:53:09 GMT
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
	-	`sha256:bc06ea6ffc2a4279c91e26e37b450afb1e0f1007815b19a7146d52b016dddc61`  
		Last Modified: Wed, 14 Jun 2023 20:53:59 GMT  
		Size: 954.7 KB (954748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:098e9e56712cb64736718f40b476d8eeb9410130c28ce94fe1bc2d380d9083cf`  
		Last Modified: Wed, 14 Jun 2023 20:53:59 GMT  
		Size: 282.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5c14818f6fb630a615284b18f945c89c0563530c25f07af955d0f85504020e9`  
		Last Modified: Wed, 14 Jun 2023 20:53:58 GMT  
		Size: 118.0 B  
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
$ docker pull memcached@sha256:e59934ff7bef6e6053b618f65923d2c1fa7235a008fb20f4fe9db13f8d6dc167
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.4 MB (4399194 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dab6918acf63bcf26d1a95d40666c44f281aa14f0d4e27884d4c2f4b227dd9b3`
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
# Wed, 14 Jun 2023 20:57:27 GMT
ENV MEMCACHED_VERSION=1.6.20
# Wed, 14 Jun 2023 20:57:27 GMT
ENV MEMCACHED_SHA1=face85ed6fad41432ad818445b24eca55bccdd78
# Wed, 14 Jun 2023 20:59:54 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Wed, 14 Jun 2023 20:59:54 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 14 Jun 2023 20:59:55 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 14 Jun 2023 20:59:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Jun 2023 20:59:55 GMT
USER memcache
# Wed, 14 Jun 2023 20:59:55 GMT
EXPOSE 11211
# Wed, 14 Jun 2023 20:59:55 GMT
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
	-	`sha256:eddee3cdc367d6f8265fe941f97020460db6cb5555711640b2ad62bd5c2a613c`  
		Last Modified: Wed, 14 Jun 2023 21:00:51 GMT  
		Size: 944.1 KB (944138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfec1ffcd9427d8fb06b908c1d3e0715a9db99c94c46f7896890a98b95c5f049`  
		Last Modified: Wed, 14 Jun 2023 21:00:51 GMT  
		Size: 280.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aea835bd4a5d779b88da37bc977813dd1ed9d228f5e78e3459edde4fa6f155e2`  
		Last Modified: Wed, 14 Jun 2023 21:00:51 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:alpine` - linux; 386

```console
$ docker pull memcached@sha256:a919915b23bf734458584f42947ebf9a743a84c8c93d2e2ea784e1bc230aaa59
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.3 MB (4282199 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2764bc1af6a7d65fbfe6ad34b4c7d1799646f8d940c1b23b550f5b577d86b8b9`
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
# Wed, 14 Jun 2023 22:38:22 GMT
ENV MEMCACHED_VERSION=1.6.20
# Wed, 14 Jun 2023 22:38:22 GMT
ENV MEMCACHED_SHA1=face85ed6fad41432ad818445b24eca55bccdd78
# Wed, 14 Jun 2023 22:41:49 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Wed, 14 Jun 2023 22:41:49 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 14 Jun 2023 22:41:50 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 14 Jun 2023 22:41:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Jun 2023 22:41:50 GMT
USER memcache
# Wed, 14 Jun 2023 22:41:50 GMT
EXPOSE 11211
# Wed, 14 Jun 2023 22:41:50 GMT
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
	-	`sha256:e6eae361cc7d0f997a631fbe78920dacf40cb6d4751c30ee1692dbeac08bc37f`  
		Last Modified: Wed, 14 Jun 2023 22:42:32 GMT  
		Size: 937.0 KB (937049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26d07209b7ab8b880d78464e8fda28a770a3be477f9566a419967691b487705f`  
		Last Modified: Wed, 14 Jun 2023 22:42:32 GMT  
		Size: 280.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af5afdbe7d4d8e1bd1297aa2dfcdc690485f3965c75a5eb520d5681c789048c5`  
		Last Modified: Wed, 14 Jun 2023 22:42:32 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:alpine` - linux; ppc64le

```console
$ docker pull memcached@sha256:4ac2ba7993ef774f28a06c635dfb14927d19a5d624e1d935a9d17231df0f153f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4453208 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d545989d562d3df14a6b1e5f35cfa997c5f02dcbe213a92d66f3aaad767c1feb`
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
# Thu, 15 Jun 2023 04:20:03 GMT
ENV MEMCACHED_VERSION=1.6.20
# Thu, 15 Jun 2023 04:20:03 GMT
ENV MEMCACHED_SHA1=face85ed6fad41432ad818445b24eca55bccdd78
# Thu, 15 Jun 2023 04:23:03 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Thu, 15 Jun 2023 04:23:04 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 15 Jun 2023 04:23:05 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 15 Jun 2023 04:23:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 15 Jun 2023 04:23:05 GMT
USER memcache
# Thu, 15 Jun 2023 04:23:06 GMT
EXPOSE 11211
# Thu, 15 Jun 2023 04:23:06 GMT
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
	-	`sha256:b035d841131485b85fca254bc1f51878eeb4efb089ca292b6912144e0744dcfa`  
		Last Modified: Thu, 15 Jun 2023 04:23:37 GMT  
		Size: 982.8 KB (982821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49b24d1f64de4f01a1b2c94bbd8b53bfd5d55c0d2c842418f679f2dc3122f93d`  
		Last Modified: Thu, 15 Jun 2023 04:23:37 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:400968138d2a427cec2d804e2fb8b52908236f9823f026c8d3f5f90f5fbbed0b`  
		Last Modified: Thu, 15 Jun 2023 04:23:36 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:alpine` - linux; s390x

```console
$ docker pull memcached@sha256:441c53da2edef09782ae8d67860d08a92c2c8c9e4abf7f0a48977db69a803953
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.3 MB (4278165 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1023dcfb4b4b8c4b0993be67253a28f023a74ff3b9eaa67976766f6d256f73a7`
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
# Thu, 15 Jun 2023 06:27:49 GMT
ENV MEMCACHED_VERSION=1.6.20
# Thu, 15 Jun 2023 06:27:50 GMT
ENV MEMCACHED_SHA1=face85ed6fad41432ad818445b24eca55bccdd78
# Thu, 15 Jun 2023 06:31:41 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Thu, 15 Jun 2023 06:31:42 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 15 Jun 2023 06:31:44 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 15 Jun 2023 06:31:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 15 Jun 2023 06:31:45 GMT
USER memcache
# Thu, 15 Jun 2023 06:31:45 GMT
EXPOSE 11211
# Thu, 15 Jun 2023 06:31:45 GMT
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
	-	`sha256:baa4da6084d6df86753b54ce48182165eb8c080ba843e13fa42fb2503ab59c27`  
		Last Modified: Thu, 15 Jun 2023 06:36:33 GMT  
		Size: 950.1 KB (950145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fc33101b6e87a2752ae5e82c32aa4480ef0000c174eb363eadfe98755991b38`  
		Last Modified: Thu, 15 Jun 2023 06:36:33 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c8630e5ca40a95cae4c251c954b07bae6331ac9d08eeff70d12d3263339dca0`  
		Last Modified: Thu, 15 Jun 2023 06:36:33 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:alpine3.18`

```console
$ docker pull memcached@sha256:2943c39203d6df11309370bbd8e3896daddfac79f1a6414a9a9cc2381e70da81
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
$ docker pull memcached@sha256:a7a04bc20ec122d9f024dff57494853d5dc9705fb97af9170cc31a1f531dcaa5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4462373 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:15429daa972e1d57884e75ecc7f784564ae7cf089c25671dd118a0025f806b6f`
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
# Wed, 14 Jun 2023 20:50:59 GMT
ENV MEMCACHED_VERSION=1.6.20
# Wed, 14 Jun 2023 20:50:59 GMT
ENV MEMCACHED_SHA1=face85ed6fad41432ad818445b24eca55bccdd78
# Wed, 14 Jun 2023 20:53:09 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Wed, 14 Jun 2023 20:53:09 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 14 Jun 2023 20:53:09 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 14 Jun 2023 20:53:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Jun 2023 20:53:09 GMT
USER memcache
# Wed, 14 Jun 2023 20:53:09 GMT
EXPOSE 11211
# Wed, 14 Jun 2023 20:53:09 GMT
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
	-	`sha256:bc06ea6ffc2a4279c91e26e37b450afb1e0f1007815b19a7146d52b016dddc61`  
		Last Modified: Wed, 14 Jun 2023 20:53:59 GMT  
		Size: 954.7 KB (954748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:098e9e56712cb64736718f40b476d8eeb9410130c28ce94fe1bc2d380d9083cf`  
		Last Modified: Wed, 14 Jun 2023 20:53:59 GMT  
		Size: 282.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5c14818f6fb630a615284b18f945c89c0563530c25f07af955d0f85504020e9`  
		Last Modified: Wed, 14 Jun 2023 20:53:58 GMT  
		Size: 118.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:alpine3.18` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:e59934ff7bef6e6053b618f65923d2c1fa7235a008fb20f4fe9db13f8d6dc167
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.4 MB (4399194 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dab6918acf63bcf26d1a95d40666c44f281aa14f0d4e27884d4c2f4b227dd9b3`
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
# Wed, 14 Jun 2023 20:57:27 GMT
ENV MEMCACHED_VERSION=1.6.20
# Wed, 14 Jun 2023 20:57:27 GMT
ENV MEMCACHED_SHA1=face85ed6fad41432ad818445b24eca55bccdd78
# Wed, 14 Jun 2023 20:59:54 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Wed, 14 Jun 2023 20:59:54 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 14 Jun 2023 20:59:55 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 14 Jun 2023 20:59:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Jun 2023 20:59:55 GMT
USER memcache
# Wed, 14 Jun 2023 20:59:55 GMT
EXPOSE 11211
# Wed, 14 Jun 2023 20:59:55 GMT
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
	-	`sha256:eddee3cdc367d6f8265fe941f97020460db6cb5555711640b2ad62bd5c2a613c`  
		Last Modified: Wed, 14 Jun 2023 21:00:51 GMT  
		Size: 944.1 KB (944138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfec1ffcd9427d8fb06b908c1d3e0715a9db99c94c46f7896890a98b95c5f049`  
		Last Modified: Wed, 14 Jun 2023 21:00:51 GMT  
		Size: 280.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aea835bd4a5d779b88da37bc977813dd1ed9d228f5e78e3459edde4fa6f155e2`  
		Last Modified: Wed, 14 Jun 2023 21:00:51 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:alpine3.18` - linux; 386

```console
$ docker pull memcached@sha256:a919915b23bf734458584f42947ebf9a743a84c8c93d2e2ea784e1bc230aaa59
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.3 MB (4282199 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2764bc1af6a7d65fbfe6ad34b4c7d1799646f8d940c1b23b550f5b577d86b8b9`
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
# Wed, 14 Jun 2023 22:38:22 GMT
ENV MEMCACHED_VERSION=1.6.20
# Wed, 14 Jun 2023 22:38:22 GMT
ENV MEMCACHED_SHA1=face85ed6fad41432ad818445b24eca55bccdd78
# Wed, 14 Jun 2023 22:41:49 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Wed, 14 Jun 2023 22:41:49 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 14 Jun 2023 22:41:50 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 14 Jun 2023 22:41:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Jun 2023 22:41:50 GMT
USER memcache
# Wed, 14 Jun 2023 22:41:50 GMT
EXPOSE 11211
# Wed, 14 Jun 2023 22:41:50 GMT
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
	-	`sha256:e6eae361cc7d0f997a631fbe78920dacf40cb6d4751c30ee1692dbeac08bc37f`  
		Last Modified: Wed, 14 Jun 2023 22:42:32 GMT  
		Size: 937.0 KB (937049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26d07209b7ab8b880d78464e8fda28a770a3be477f9566a419967691b487705f`  
		Last Modified: Wed, 14 Jun 2023 22:42:32 GMT  
		Size: 280.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af5afdbe7d4d8e1bd1297aa2dfcdc690485f3965c75a5eb520d5681c789048c5`  
		Last Modified: Wed, 14 Jun 2023 22:42:32 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:alpine3.18` - linux; ppc64le

```console
$ docker pull memcached@sha256:4ac2ba7993ef774f28a06c635dfb14927d19a5d624e1d935a9d17231df0f153f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4453208 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d545989d562d3df14a6b1e5f35cfa997c5f02dcbe213a92d66f3aaad767c1feb`
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
# Thu, 15 Jun 2023 04:20:03 GMT
ENV MEMCACHED_VERSION=1.6.20
# Thu, 15 Jun 2023 04:20:03 GMT
ENV MEMCACHED_SHA1=face85ed6fad41432ad818445b24eca55bccdd78
# Thu, 15 Jun 2023 04:23:03 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Thu, 15 Jun 2023 04:23:04 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 15 Jun 2023 04:23:05 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 15 Jun 2023 04:23:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 15 Jun 2023 04:23:05 GMT
USER memcache
# Thu, 15 Jun 2023 04:23:06 GMT
EXPOSE 11211
# Thu, 15 Jun 2023 04:23:06 GMT
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
	-	`sha256:b035d841131485b85fca254bc1f51878eeb4efb089ca292b6912144e0744dcfa`  
		Last Modified: Thu, 15 Jun 2023 04:23:37 GMT  
		Size: 982.8 KB (982821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49b24d1f64de4f01a1b2c94bbd8b53bfd5d55c0d2c842418f679f2dc3122f93d`  
		Last Modified: Thu, 15 Jun 2023 04:23:37 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:400968138d2a427cec2d804e2fb8b52908236f9823f026c8d3f5f90f5fbbed0b`  
		Last Modified: Thu, 15 Jun 2023 04:23:36 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:alpine3.18` - linux; s390x

```console
$ docker pull memcached@sha256:441c53da2edef09782ae8d67860d08a92c2c8c9e4abf7f0a48977db69a803953
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.3 MB (4278165 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1023dcfb4b4b8c4b0993be67253a28f023a74ff3b9eaa67976766f6d256f73a7`
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
# Thu, 15 Jun 2023 06:27:49 GMT
ENV MEMCACHED_VERSION=1.6.20
# Thu, 15 Jun 2023 06:27:50 GMT
ENV MEMCACHED_SHA1=face85ed6fad41432ad818445b24eca55bccdd78
# Thu, 15 Jun 2023 06:31:41 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Thu, 15 Jun 2023 06:31:42 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 15 Jun 2023 06:31:44 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 15 Jun 2023 06:31:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 15 Jun 2023 06:31:45 GMT
USER memcache
# Thu, 15 Jun 2023 06:31:45 GMT
EXPOSE 11211
# Thu, 15 Jun 2023 06:31:45 GMT
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
	-	`sha256:baa4da6084d6df86753b54ce48182165eb8c080ba843e13fa42fb2503ab59c27`  
		Last Modified: Thu, 15 Jun 2023 06:36:33 GMT  
		Size: 950.1 KB (950145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fc33101b6e87a2752ae5e82c32aa4480ef0000c174eb363eadfe98755991b38`  
		Last Modified: Thu, 15 Jun 2023 06:36:33 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c8630e5ca40a95cae4c251c954b07bae6331ac9d08eeff70d12d3263339dca0`  
		Last Modified: Thu, 15 Jun 2023 06:36:33 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:bookworm`

```console
$ docker pull memcached@sha256:8b7a3ce027c33dc2142b3826dae320dacdb9987fa86267c15505a80147f926b7
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
$ docker pull memcached@sha256:533c607824b2f5781b179e175fcdf055577a3f076fb0a0fdcd13487c7c92125f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.0 MB (38973406 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cbcfa8d0003c80b0bba4004f4b15b4a5600b9dd481ac2d887bc31e794f067464`
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
# Wed, 14 Jun 2023 20:48:24 GMT
ENV MEMCACHED_VERSION=1.6.20
# Wed, 14 Jun 2023 20:48:24 GMT
ENV MEMCACHED_SHA1=face85ed6fad41432ad818445b24eca55bccdd78
# Wed, 14 Jun 2023 20:50:40 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 14 Jun 2023 20:50:40 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 14 Jun 2023 20:50:41 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 14 Jun 2023 20:50:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Jun 2023 20:50:41 GMT
USER memcache
# Wed, 14 Jun 2023 20:50:41 GMT
EXPOSE 11211
# Wed, 14 Jun 2023 20:50:41 GMT
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
	-	`sha256:96a3de0d22592d9a254814d5b77e3a84e73d2f055d162503fe811f731a320701`  
		Last Modified: Wed, 14 Jun 2023 20:53:34 GMT  
		Size: 7.2 MB (7169888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a38b201fb7fc8d917459453ee1c0218cf9845c96b885a02b02999f81b21c6bb`  
		Last Modified: Wed, 14 Jun 2023 20:53:33 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6f5720dc1980c886ee7e8d6067ed87e102bb31824e557a85fbd54273542debf`  
		Last Modified: Wed, 14 Jun 2023 20:53:33 GMT  
		Size: 120.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:bookworm` - linux; arm variant v5

```console
$ docker pull memcached@sha256:bb4a530ed3dc36e702635724bf49a6703694d36a7bcfdeabb2b0d3ff6b101143
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.1 MB (35095204 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f00b0d176a0550d5b0d3f94dc00489066995ce4a1be3e688924144b9077256f`
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
# Wed, 14 Jun 2023 21:56:26 GMT
ENV MEMCACHED_VERSION=1.6.20
# Wed, 14 Jun 2023 21:56:27 GMT
ENV MEMCACHED_SHA1=face85ed6fad41432ad818445b24eca55bccdd78
# Wed, 14 Jun 2023 22:00:10 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 14 Jun 2023 22:00:10 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 14 Jun 2023 22:00:12 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 14 Jun 2023 22:00:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Jun 2023 22:00:12 GMT
USER memcache
# Wed, 14 Jun 2023 22:00:12 GMT
EXPOSE 11211
# Wed, 14 Jun 2023 22:00:13 GMT
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
	-	`sha256:feb8e13d6ab7efa5799bc12cdb4d8f410166028673257b803f31b6bc9d0eb70c`  
		Last Modified: Wed, 14 Jun 2023 22:00:42 GMT  
		Size: 5.8 MB (5829749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cf20cb3e5676ee2969940d8133531dcd0df55159ccb7dbd567cc83b2bc02384`  
		Last Modified: Wed, 14 Jun 2023 22:00:39 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04bc2d45321e126b2795ea784886ac10a0b3c5724ccf555f0d20f2c7ee4225f1`  
		Last Modified: Wed, 14 Jun 2023 22:00:39 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:bookworm` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:3464bfccdfad0dc788e056949d59fc0b665ec165654b3a8502a2f4a3868a3dc7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.9 MB (37872888 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:20f33353745665e05e1722aa9af40e06b3f58778f8e758e786eaad30054de61f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 12 Jun 2023 23:40:13 GMT
ADD file:f75c3fe22fec548b35a86a9a5802fdc97497f5d253cf630d65f13282169d3f3f in / 
# Mon, 12 Jun 2023 23:40:14 GMT
CMD ["bash"]
# Wed, 14 Jun 2023 20:54:33 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 14 Jun 2023 20:54:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 14 Jun 2023 20:54:37 GMT
ENV MEMCACHED_VERSION=1.6.20
# Wed, 14 Jun 2023 20:54:37 GMT
ENV MEMCACHED_SHA1=face85ed6fad41432ad818445b24eca55bccdd78
# Wed, 14 Jun 2023 20:57:13 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 14 Jun 2023 20:57:13 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 14 Jun 2023 20:57:14 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 14 Jun 2023 20:57:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Jun 2023 20:57:14 GMT
USER memcache
# Wed, 14 Jun 2023 20:57:14 GMT
EXPOSE 11211
# Wed, 14 Jun 2023 20:57:14 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:95039a22a7cc3ae41d71f075e6e09e91e8da850fb5f80aba2f4a09f254520539`  
		Last Modified: Mon, 12 Jun 2023 23:44:08 GMT  
		Size: 29.2 MB (29152534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6da70104cc8ee465752315034f04011354e6149243e2bc69b9da49e6855df4b8`  
		Last Modified: Wed, 14 Jun 2023 21:00:29 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a7b40152f53e05b8cbcfe09be5b1598fcc05cf4f9ffad3b296eca43305450da`  
		Last Modified: Wed, 14 Jun 2023 21:00:30 GMT  
		Size: 2.5 MB (2539179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bf09d04f9c61af195486f42915b137b8612584f982737f5e465d02648a6dc8a`  
		Last Modified: Wed, 14 Jun 2023 21:00:30 GMT  
		Size: 6.2 MB (6179640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e71555e51295eeceeab1a9ab6bebb21108fbbe59e01349857c51932deea0f64`  
		Last Modified: Wed, 14 Jun 2023 21:00:29 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15cd3195dbfc5cedaf71b7c156002599dfb94219b51f85c966a1bee80bc37e65`  
		Last Modified: Wed, 14 Jun 2023 21:00:29 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:bookworm` - linux; 386

```console
$ docker pull memcached@sha256:7c2fdc7c597b4f6efd737d9b8f1e78841cda31e4492a6ae32f3d6f1ab6911cb8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.5 MB (39457716 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a1e668084859e8f39e52c33d0d7a68506127f94d95c61ffb7f43f9441843fa3b`
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
# Wed, 14 Jun 2023 22:34:33 GMT
ENV MEMCACHED_VERSION=1.6.20
# Wed, 14 Jun 2023 22:34:33 GMT
ENV MEMCACHED_SHA1=face85ed6fad41432ad818445b24eca55bccdd78
# Wed, 14 Jun 2023 22:38:16 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 14 Jun 2023 22:38:17 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 14 Jun 2023 22:38:17 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 14 Jun 2023 22:38:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Jun 2023 22:38:17 GMT
USER memcache
# Wed, 14 Jun 2023 22:38:17 GMT
EXPOSE 11211
# Wed, 14 Jun 2023 22:38:18 GMT
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
	-	`sha256:2896f0aba2db45558c3b7f796cc22aa198f38d579fdc6ddf35893d5ea553c080`  
		Last Modified: Wed, 14 Jun 2023 22:42:10 GMT  
		Size: 6.6 MB (6630422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17e035509d03f0bd9a08582ab075babcb6e7dcbe048f9968c81ae996df72e6aa`  
		Last Modified: Wed, 14 Jun 2023 22:42:09 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc5b3164ed6a8d968b1da11795198c4d6ce05822ff371f41d2c7eb373d44141b`  
		Last Modified: Wed, 14 Jun 2023 22:42:09 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:bookworm` - linux; mips64le

```console
$ docker pull memcached@sha256:d2855c4deb19365dd1c83b81c9e1fa36f7873cc8b3dd02f8f01de10200bf208e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.6 MB (37554221 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7068fffc8ee0a4607e1586297977a273786efb52e1782f11396ee5f7a5150c0f`
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
# Wed, 14 Jun 2023 18:38:39 GMT
ENV MEMCACHED_VERSION=1.6.20
# Wed, 14 Jun 2023 18:38:41 GMT
ENV MEMCACHED_SHA1=face85ed6fad41432ad818445b24eca55bccdd78
# Wed, 14 Jun 2023 18:45:20 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 14 Jun 2023 18:45:23 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 14 Jun 2023 18:45:27 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 14 Jun 2023 18:45:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Jun 2023 18:45:32 GMT
USER memcache
# Wed, 14 Jun 2023 18:45:35 GMT
EXPOSE 11211
# Wed, 14 Jun 2023 18:45:38 GMT
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
	-	`sha256:76d4e9cc234d41e69eba3bf411cb1d3ebe17e2fefbffb0c3458d613f2545337e`  
		Last Modified: Wed, 14 Jun 2023 18:46:09 GMT  
		Size: 6.5 MB (6499709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0988c34e4840378b9876eba362b50458e769389d0cc626698bef65e46c721458`  
		Last Modified: Wed, 14 Jun 2023 18:46:04 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db55745458426cdf0d23fd0589fd440e2d328e4d5ffb00a9ef6d2e0225cec8bf`  
		Last Modified: Wed, 14 Jun 2023 18:46:04 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:bookworm` - linux; ppc64le

```console
$ docker pull memcached@sha256:0e023c41d9c6a8d04edad22ecea59cfcf424d0dc3895c442a9e7a4575961d53d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.2 MB (43193448 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a85a60b74a9575a203aba1a5f800dfe479b80cde8ff577ccd5e7e77bdaab64c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 12 Jun 2023 23:17:34 GMT
ADD file:3f8b9849acb625537f99921ef80190de7b03afdc287a5d1113a92cc41ae24be2 in / 
# Mon, 12 Jun 2023 23:17:36 GMT
CMD ["bash"]
# Wed, 14 Jun 2023 18:15:42 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 14 Jun 2023 18:15:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 14 Jun 2023 18:15:50 GMT
ENV MEMCACHED_VERSION=1.6.20
# Wed, 14 Jun 2023 18:15:51 GMT
ENV MEMCACHED_SHA1=face85ed6fad41432ad818445b24eca55bccdd78
# Wed, 14 Jun 2023 18:19:27 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 14 Jun 2023 18:19:28 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 14 Jun 2023 18:19:30 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 14 Jun 2023 18:19:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Jun 2023 18:19:31 GMT
USER memcache
# Wed, 14 Jun 2023 18:19:32 GMT
EXPOSE 11211
# Wed, 14 Jun 2023 18:19:32 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:9f041b53cef30007c43057f2520876c85ed6bee6be5aaee867dfb31a053d6cca`  
		Last Modified: Mon, 12 Jun 2023 23:24:09 GMT  
		Size: 33.1 MB (33116725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2a2d84b1fee81412bbd9bb301c77e6dfacfac70c2f1485de806658b49b06e08`  
		Last Modified: Wed, 14 Jun 2023 18:19:49 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca8bb5af043b48c9fe0e110ee13c139ceb715570346140fc86092d582d38b52b`  
		Last Modified: Wed, 14 Jun 2023 18:19:50 GMT  
		Size: 2.9 MB (2891306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e2d7805a151ec1618da95ad34cb2fdc6ae889b9f7908aaca6d063ca864f3e24`  
		Last Modified: Wed, 14 Jun 2023 18:19:52 GMT  
		Size: 7.2 MB (7183881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc5db4b315753422be0d08638f594b1ec64484c44f68942473f903387853b3bd`  
		Last Modified: Wed, 14 Jun 2023 18:19:49 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a8a9b2ed7c41d27d92f9db3c21beec2a2e288b0bc54a19aa1d3574b6085eaa6`  
		Last Modified: Wed, 14 Jun 2023 18:19:49 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:bookworm` - linux; s390x

```console
$ docker pull memcached@sha256:7bbe5a63846bc51d11850be291c164685b55f4d65a48ea07e8a6df50e489b658
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.9 MB (35907698 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d7e906c7eff45be64cda148363028a1270de09239533ca7dfee428108e20a155`
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
# Thu, 15 Jun 2023 06:23:29 GMT
ENV MEMCACHED_VERSION=1.6.20
# Thu, 15 Jun 2023 06:23:29 GMT
ENV MEMCACHED_SHA1=face85ed6fad41432ad818445b24eca55bccdd78
# Thu, 15 Jun 2023 06:26:33 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 15 Jun 2023 06:26:33 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 15 Jun 2023 06:26:34 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 15 Jun 2023 06:26:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 15 Jun 2023 06:26:35 GMT
USER memcache
# Thu, 15 Jun 2023 06:26:35 GMT
EXPOSE 11211
# Thu, 15 Jun 2023 06:26:35 GMT
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
	-	`sha256:a7ba1840ae9bcaa91375ac3b538e9ad379ec203bf9c6616bff06ec2a9ca6616a`  
		Last Modified: Thu, 15 Jun 2023 06:35:18 GMT  
		Size: 6.1 MB (6072893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d4533d005f06d7358727f3d1a167ee982d65ec08c863bd2171511918dab48d4`  
		Last Modified: Thu, 15 Jun 2023 06:35:17 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:769590255adfb1d384255f87732ddc4f78483e8203987ffba90f56f4102080e7`  
		Last Modified: Thu, 15 Jun 2023 06:35:17 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:latest`

```console
$ docker pull memcached@sha256:791d3a3f4bed25f726ff2e0fea1bbc1038a5154dfadfc2d19cd2e8dd4c5a1a05
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
$ docker pull memcached@sha256:533c607824b2f5781b179e175fcdf055577a3f076fb0a0fdcd13487c7c92125f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.0 MB (38973406 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cbcfa8d0003c80b0bba4004f4b15b4a5600b9dd481ac2d887bc31e794f067464`
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
# Wed, 14 Jun 2023 20:48:24 GMT
ENV MEMCACHED_VERSION=1.6.20
# Wed, 14 Jun 2023 20:48:24 GMT
ENV MEMCACHED_SHA1=face85ed6fad41432ad818445b24eca55bccdd78
# Wed, 14 Jun 2023 20:50:40 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 14 Jun 2023 20:50:40 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 14 Jun 2023 20:50:41 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 14 Jun 2023 20:50:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Jun 2023 20:50:41 GMT
USER memcache
# Wed, 14 Jun 2023 20:50:41 GMT
EXPOSE 11211
# Wed, 14 Jun 2023 20:50:41 GMT
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
	-	`sha256:96a3de0d22592d9a254814d5b77e3a84e73d2f055d162503fe811f731a320701`  
		Last Modified: Wed, 14 Jun 2023 20:53:34 GMT  
		Size: 7.2 MB (7169888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a38b201fb7fc8d917459453ee1c0218cf9845c96b885a02b02999f81b21c6bb`  
		Last Modified: Wed, 14 Jun 2023 20:53:33 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6f5720dc1980c886ee7e8d6067ed87e102bb31824e557a85fbd54273542debf`  
		Last Modified: Wed, 14 Jun 2023 20:53:33 GMT  
		Size: 120.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:latest` - linux; arm variant v5

```console
$ docker pull memcached@sha256:bb4a530ed3dc36e702635724bf49a6703694d36a7bcfdeabb2b0d3ff6b101143
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.1 MB (35095204 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f00b0d176a0550d5b0d3f94dc00489066995ce4a1be3e688924144b9077256f`
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
# Wed, 14 Jun 2023 21:56:26 GMT
ENV MEMCACHED_VERSION=1.6.20
# Wed, 14 Jun 2023 21:56:27 GMT
ENV MEMCACHED_SHA1=face85ed6fad41432ad818445b24eca55bccdd78
# Wed, 14 Jun 2023 22:00:10 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 14 Jun 2023 22:00:10 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 14 Jun 2023 22:00:12 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 14 Jun 2023 22:00:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Jun 2023 22:00:12 GMT
USER memcache
# Wed, 14 Jun 2023 22:00:12 GMT
EXPOSE 11211
# Wed, 14 Jun 2023 22:00:13 GMT
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
	-	`sha256:feb8e13d6ab7efa5799bc12cdb4d8f410166028673257b803f31b6bc9d0eb70c`  
		Last Modified: Wed, 14 Jun 2023 22:00:42 GMT  
		Size: 5.8 MB (5829749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cf20cb3e5676ee2969940d8133531dcd0df55159ccb7dbd567cc83b2bc02384`  
		Last Modified: Wed, 14 Jun 2023 22:00:39 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04bc2d45321e126b2795ea784886ac10a0b3c5724ccf555f0d20f2c7ee4225f1`  
		Last Modified: Wed, 14 Jun 2023 22:00:39 GMT  
		Size: 121.0 B  
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
$ docker pull memcached@sha256:3464bfccdfad0dc788e056949d59fc0b665ec165654b3a8502a2f4a3868a3dc7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.9 MB (37872888 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:20f33353745665e05e1722aa9af40e06b3f58778f8e758e786eaad30054de61f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 12 Jun 2023 23:40:13 GMT
ADD file:f75c3fe22fec548b35a86a9a5802fdc97497f5d253cf630d65f13282169d3f3f in / 
# Mon, 12 Jun 2023 23:40:14 GMT
CMD ["bash"]
# Wed, 14 Jun 2023 20:54:33 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 14 Jun 2023 20:54:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 14 Jun 2023 20:54:37 GMT
ENV MEMCACHED_VERSION=1.6.20
# Wed, 14 Jun 2023 20:54:37 GMT
ENV MEMCACHED_SHA1=face85ed6fad41432ad818445b24eca55bccdd78
# Wed, 14 Jun 2023 20:57:13 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 14 Jun 2023 20:57:13 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 14 Jun 2023 20:57:14 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 14 Jun 2023 20:57:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Jun 2023 20:57:14 GMT
USER memcache
# Wed, 14 Jun 2023 20:57:14 GMT
EXPOSE 11211
# Wed, 14 Jun 2023 20:57:14 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:95039a22a7cc3ae41d71f075e6e09e91e8da850fb5f80aba2f4a09f254520539`  
		Last Modified: Mon, 12 Jun 2023 23:44:08 GMT  
		Size: 29.2 MB (29152534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6da70104cc8ee465752315034f04011354e6149243e2bc69b9da49e6855df4b8`  
		Last Modified: Wed, 14 Jun 2023 21:00:29 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a7b40152f53e05b8cbcfe09be5b1598fcc05cf4f9ffad3b296eca43305450da`  
		Last Modified: Wed, 14 Jun 2023 21:00:30 GMT  
		Size: 2.5 MB (2539179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bf09d04f9c61af195486f42915b137b8612584f982737f5e465d02648a6dc8a`  
		Last Modified: Wed, 14 Jun 2023 21:00:30 GMT  
		Size: 6.2 MB (6179640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e71555e51295eeceeab1a9ab6bebb21108fbbe59e01349857c51932deea0f64`  
		Last Modified: Wed, 14 Jun 2023 21:00:29 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15cd3195dbfc5cedaf71b7c156002599dfb94219b51f85c966a1bee80bc37e65`  
		Last Modified: Wed, 14 Jun 2023 21:00:29 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:latest` - linux; 386

```console
$ docker pull memcached@sha256:7c2fdc7c597b4f6efd737d9b8f1e78841cda31e4492a6ae32f3d6f1ab6911cb8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.5 MB (39457716 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a1e668084859e8f39e52c33d0d7a68506127f94d95c61ffb7f43f9441843fa3b`
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
# Wed, 14 Jun 2023 22:34:33 GMT
ENV MEMCACHED_VERSION=1.6.20
# Wed, 14 Jun 2023 22:34:33 GMT
ENV MEMCACHED_SHA1=face85ed6fad41432ad818445b24eca55bccdd78
# Wed, 14 Jun 2023 22:38:16 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 14 Jun 2023 22:38:17 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 14 Jun 2023 22:38:17 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 14 Jun 2023 22:38:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Jun 2023 22:38:17 GMT
USER memcache
# Wed, 14 Jun 2023 22:38:17 GMT
EXPOSE 11211
# Wed, 14 Jun 2023 22:38:18 GMT
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
	-	`sha256:2896f0aba2db45558c3b7f796cc22aa198f38d579fdc6ddf35893d5ea553c080`  
		Last Modified: Wed, 14 Jun 2023 22:42:10 GMT  
		Size: 6.6 MB (6630422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17e035509d03f0bd9a08582ab075babcb6e7dcbe048f9968c81ae996df72e6aa`  
		Last Modified: Wed, 14 Jun 2023 22:42:09 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc5b3164ed6a8d968b1da11795198c4d6ce05822ff371f41d2c7eb373d44141b`  
		Last Modified: Wed, 14 Jun 2023 22:42:09 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:latest` - linux; mips64le

```console
$ docker pull memcached@sha256:d2855c4deb19365dd1c83b81c9e1fa36f7873cc8b3dd02f8f01de10200bf208e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.6 MB (37554221 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7068fffc8ee0a4607e1586297977a273786efb52e1782f11396ee5f7a5150c0f`
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
# Wed, 14 Jun 2023 18:38:39 GMT
ENV MEMCACHED_VERSION=1.6.20
# Wed, 14 Jun 2023 18:38:41 GMT
ENV MEMCACHED_SHA1=face85ed6fad41432ad818445b24eca55bccdd78
# Wed, 14 Jun 2023 18:45:20 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 14 Jun 2023 18:45:23 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 14 Jun 2023 18:45:27 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 14 Jun 2023 18:45:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Jun 2023 18:45:32 GMT
USER memcache
# Wed, 14 Jun 2023 18:45:35 GMT
EXPOSE 11211
# Wed, 14 Jun 2023 18:45:38 GMT
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
	-	`sha256:76d4e9cc234d41e69eba3bf411cb1d3ebe17e2fefbffb0c3458d613f2545337e`  
		Last Modified: Wed, 14 Jun 2023 18:46:09 GMT  
		Size: 6.5 MB (6499709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0988c34e4840378b9876eba362b50458e769389d0cc626698bef65e46c721458`  
		Last Modified: Wed, 14 Jun 2023 18:46:04 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db55745458426cdf0d23fd0589fd440e2d328e4d5ffb00a9ef6d2e0225cec8bf`  
		Last Modified: Wed, 14 Jun 2023 18:46:04 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:latest` - linux; ppc64le

```console
$ docker pull memcached@sha256:0e023c41d9c6a8d04edad22ecea59cfcf424d0dc3895c442a9e7a4575961d53d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.2 MB (43193448 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a85a60b74a9575a203aba1a5f800dfe479b80cde8ff577ccd5e7e77bdaab64c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 12 Jun 2023 23:17:34 GMT
ADD file:3f8b9849acb625537f99921ef80190de7b03afdc287a5d1113a92cc41ae24be2 in / 
# Mon, 12 Jun 2023 23:17:36 GMT
CMD ["bash"]
# Wed, 14 Jun 2023 18:15:42 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 14 Jun 2023 18:15:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 14 Jun 2023 18:15:50 GMT
ENV MEMCACHED_VERSION=1.6.20
# Wed, 14 Jun 2023 18:15:51 GMT
ENV MEMCACHED_SHA1=face85ed6fad41432ad818445b24eca55bccdd78
# Wed, 14 Jun 2023 18:19:27 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 14 Jun 2023 18:19:28 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 14 Jun 2023 18:19:30 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 14 Jun 2023 18:19:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Jun 2023 18:19:31 GMT
USER memcache
# Wed, 14 Jun 2023 18:19:32 GMT
EXPOSE 11211
# Wed, 14 Jun 2023 18:19:32 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:9f041b53cef30007c43057f2520876c85ed6bee6be5aaee867dfb31a053d6cca`  
		Last Modified: Mon, 12 Jun 2023 23:24:09 GMT  
		Size: 33.1 MB (33116725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2a2d84b1fee81412bbd9bb301c77e6dfacfac70c2f1485de806658b49b06e08`  
		Last Modified: Wed, 14 Jun 2023 18:19:49 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca8bb5af043b48c9fe0e110ee13c139ceb715570346140fc86092d582d38b52b`  
		Last Modified: Wed, 14 Jun 2023 18:19:50 GMT  
		Size: 2.9 MB (2891306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e2d7805a151ec1618da95ad34cb2fdc6ae889b9f7908aaca6d063ca864f3e24`  
		Last Modified: Wed, 14 Jun 2023 18:19:52 GMT  
		Size: 7.2 MB (7183881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc5db4b315753422be0d08638f594b1ec64484c44f68942473f903387853b3bd`  
		Last Modified: Wed, 14 Jun 2023 18:19:49 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a8a9b2ed7c41d27d92f9db3c21beec2a2e288b0bc54a19aa1d3574b6085eaa6`  
		Last Modified: Wed, 14 Jun 2023 18:19:49 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:latest` - linux; s390x

```console
$ docker pull memcached@sha256:7bbe5a63846bc51d11850be291c164685b55f4d65a48ea07e8a6df50e489b658
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.9 MB (35907698 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d7e906c7eff45be64cda148363028a1270de09239533ca7dfee428108e20a155`
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
# Thu, 15 Jun 2023 06:23:29 GMT
ENV MEMCACHED_VERSION=1.6.20
# Thu, 15 Jun 2023 06:23:29 GMT
ENV MEMCACHED_SHA1=face85ed6fad41432ad818445b24eca55bccdd78
# Thu, 15 Jun 2023 06:26:33 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 15 Jun 2023 06:26:33 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 15 Jun 2023 06:26:34 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 15 Jun 2023 06:26:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 15 Jun 2023 06:26:35 GMT
USER memcache
# Thu, 15 Jun 2023 06:26:35 GMT
EXPOSE 11211
# Thu, 15 Jun 2023 06:26:35 GMT
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
	-	`sha256:a7ba1840ae9bcaa91375ac3b538e9ad379ec203bf9c6616bff06ec2a9ca6616a`  
		Last Modified: Thu, 15 Jun 2023 06:35:18 GMT  
		Size: 6.1 MB (6072893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d4533d005f06d7358727f3d1a167ee982d65ec08c863bd2171511918dab48d4`  
		Last Modified: Thu, 15 Jun 2023 06:35:17 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:769590255adfb1d384255f87732ddc4f78483e8203987ffba90f56f4102080e7`  
		Last Modified: Thu, 15 Jun 2023 06:35:17 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
