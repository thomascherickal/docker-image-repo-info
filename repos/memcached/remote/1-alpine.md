## `memcached:1-alpine`

```console
$ docker pull memcached@sha256:32a6ff0c8679603a3977c810419511d6137db92c4f01d0d8282aa397e5cf71c6
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
$ docker pull memcached@sha256:e1928aafa8833a2470b47fcc89754c26403ba3cda2ecbb4c4266072279e22576
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4886255 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ff697670a954aa7c8407c1f4391c129aea5e6c94f3728513631fed5f7756e164`
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
# Tue, 24 Nov 2020 00:44:26 GMT
ENV MEMCACHED_VERSION=1.6.9
# Tue, 24 Nov 2020 00:44:26 GMT
ENV MEMCACHED_SHA1=42ae062094fdf083cfe7b21ff377c781011c2be1
# Tue, 24 Nov 2020 00:48:41 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		dpkg-dev dpkg 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		tar 		wget 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 24 Nov 2020 00:48:42 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 24 Nov 2020 00:48:43 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 24 Nov 2020 00:48:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 24 Nov 2020 00:48:43 GMT
USER memcache
# Tue, 24 Nov 2020 00:48:43 GMT
EXPOSE 11211
# Tue, 24 Nov 2020 00:48:44 GMT
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
	-	`sha256:3b822756c8bfaf1bc207adc2de3741e339a2693e9ee8e311a149808db14b5208`  
		Last Modified: Tue, 24 Nov 2020 00:49:13 GMT  
		Size: 2.1 MB (2072463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af2d6b4d764b9c213154f1680d12d1ccf7241e76e6064dda66d5d3c3031f0e2b`  
		Last Modified: Tue, 24 Nov 2020 00:49:13 GMT  
		Size: 281.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e55816799a4db3ab4e13a264038fa0de836f4301b050cca3324eb8290e423e62`  
		Last Modified: Tue, 24 Nov 2020 00:49:13 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-alpine` - linux; arm variant v6

```console
$ docker pull memcached@sha256:84a8ab8b2c2ae46bba6afd02619cb1d0a180fd46d11749f1cb624b952ab8c9f1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4647852 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9c1779891a9245caed80bbadedd3187997a4cd109651441cbf70107bc5045c55`
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
# Tue, 24 Nov 2020 00:04:10 GMT
ENV MEMCACHED_VERSION=1.6.9
# Tue, 24 Nov 2020 00:04:10 GMT
ENV MEMCACHED_SHA1=42ae062094fdf083cfe7b21ff377c781011c2be1
# Tue, 24 Nov 2020 00:07:15 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		dpkg-dev dpkg 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		tar 		wget 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 24 Nov 2020 00:07:16 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 24 Nov 2020 00:07:18 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 24 Nov 2020 00:07:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 24 Nov 2020 00:07:19 GMT
USER memcache
# Tue, 24 Nov 2020 00:07:19 GMT
EXPOSE 11211
# Tue, 24 Nov 2020 00:07:20 GMT
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
	-	`sha256:99d3cdccf3fbd7cd515e5b74a671cda38dd9df4bcbbd570db901bf84e5003914`  
		Last Modified: Tue, 24 Nov 2020 00:07:32 GMT  
		Size: 2.0 MB (2029372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27ab5b24072ce098cf121983637ecc7320b3b99a6596ee6f3233b82854182fe2`  
		Last Modified: Tue, 24 Nov 2020 00:07:31 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fec87d28784f49a987a725efbd26639511b95005578516f18eb091f70680a17`  
		Last Modified: Tue, 24 Nov 2020 00:07:32 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-alpine` - linux; arm variant v7

```console
$ docker pull memcached@sha256:bbdb2d34f35910a55efd127f93a3b084b4210359d3ba3e04d492a70beea0320e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.3 MB (4313145 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e7520fc1477e6051f5415fbdf6960a7f9c528353aeb867c7069aa259916176ad`
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
# Tue, 24 Nov 2020 00:26:09 GMT
ENV MEMCACHED_VERSION=1.6.9
# Tue, 24 Nov 2020 00:26:10 GMT
ENV MEMCACHED_SHA1=42ae062094fdf083cfe7b21ff377c781011c2be1
# Tue, 24 Nov 2020 00:29:05 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		dpkg-dev dpkg 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		tar 		wget 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 24 Nov 2020 00:29:06 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 24 Nov 2020 00:29:08 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 24 Nov 2020 00:29:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 24 Nov 2020 00:29:11 GMT
USER memcache
# Tue, 24 Nov 2020 00:29:13 GMT
EXPOSE 11211
# Tue, 24 Nov 2020 00:29:14 GMT
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
	-	`sha256:510b94932fc56e01e3a03af48c5bcaabec2bb336f8f787734bf846feb7de347f`  
		Last Modified: Tue, 24 Nov 2020 00:29:48 GMT  
		Size: 1.9 MB (1891978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88faa5219b31e7f196605b6c2b273fae85f47d56c7fb5d5b320dd544e35414ba`  
		Last Modified: Tue, 24 Nov 2020 00:29:47 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c92e34d046a66b160935550f49396501447c4ddb5001f0ec2c33e25b1c3c5059`  
		Last Modified: Tue, 24 Nov 2020 00:29:48 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-alpine` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:a869ac02f75f64470176cf16c595e4e58bae5d5d3f442227581808e68763ace4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.8 MB (4811465 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8fd84a91919653be4583fcf329fccb126128ca56a60319c8f9c28adc05682650`
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
# Tue, 24 Nov 2020 00:54:44 GMT
ENV MEMCACHED_VERSION=1.6.9
# Tue, 24 Nov 2020 00:54:45 GMT
ENV MEMCACHED_SHA1=42ae062094fdf083cfe7b21ff377c781011c2be1
# Tue, 24 Nov 2020 00:57:40 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		dpkg-dev dpkg 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		tar 		wget 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 24 Nov 2020 00:57:40 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 24 Nov 2020 00:57:43 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 24 Nov 2020 00:57:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 24 Nov 2020 00:57:45 GMT
USER memcache
# Tue, 24 Nov 2020 00:57:45 GMT
EXPOSE 11211
# Tue, 24 Nov 2020 00:57:46 GMT
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
	-	`sha256:aed9de8619e85f52cd0657870aadd42de21c84ce68ca3412f496fd6fcd4a22bd`  
		Last Modified: Tue, 24 Nov 2020 00:58:20 GMT  
		Size: 2.1 MB (2087563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1adb1280ccf1abb19444686be75fa42aaf40a41c2c1d972d78188844c921175`  
		Last Modified: Tue, 24 Nov 2020 00:58:21 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78dc9a71b866039ff5461d91fc16d477e864471680f8066f56f37ed996019d83`  
		Last Modified: Tue, 24 Nov 2020 00:58:20 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-alpine` - linux; 386

```console
$ docker pull memcached@sha256:8fe6ce4813127db9eda50ca3d2c739e1ee4e19e6b2604c42857a084f2cee7f20
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (4962966 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6fde562f92d407d755937a5fd62e36ad4e6c11e614f0b1efe15b3c365a5919be`
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
# Tue, 24 Nov 2020 00:42:56 GMT
ENV MEMCACHED_VERSION=1.6.9
# Tue, 24 Nov 2020 00:42:56 GMT
ENV MEMCACHED_SHA1=42ae062094fdf083cfe7b21ff377c781011c2be1
# Tue, 24 Nov 2020 00:47:29 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		dpkg-dev dpkg 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		tar 		wget 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 24 Nov 2020 00:47:30 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 24 Nov 2020 00:47:31 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 24 Nov 2020 00:47:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 24 Nov 2020 00:47:31 GMT
USER memcache
# Tue, 24 Nov 2020 00:47:31 GMT
EXPOSE 11211
# Tue, 24 Nov 2020 00:47:31 GMT
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
	-	`sha256:2a7eca4f7b1391c2d397e86710de5666847f1cb0acef37165d31b41883f22895`  
		Last Modified: Tue, 24 Nov 2020 00:47:58 GMT  
		Size: 2.2 MB (2153599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c9fe46f7c3454fca381ef88344cfa1726d58a48fd7ddcbe6677de774e70c4c3`  
		Last Modified: Tue, 24 Nov 2020 00:47:57 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c645f1cec0c95903a4212ca1390af1c4ff8c0a4219b7a7ac4bedd631da2d447`  
		Last Modified: Tue, 24 Nov 2020 00:47:57 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-alpine` - linux; ppc64le

```console
$ docker pull memcached@sha256:7d76bf4416ce1df4bd72710970fa497307b515895f95e2adc44fc0d927e2e3b8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4563787 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7de761a79ff461eb8e54e9cd0cc6ceda36e3be45699b7a128f2cbb2b396ff5ad`
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
# Fri, 30 Oct 2020 11:59:46 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		dpkg-dev dpkg 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		tar 		wget 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Fri, 30 Oct 2020 11:59:48 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 30 Oct 2020 11:59:53 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 30 Oct 2020 11:59:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 30 Oct 2020 11:59:56 GMT
USER memcache
# Fri, 30 Oct 2020 11:59:58 GMT
EXPOSE 11211
# Fri, 30 Oct 2020 12:00:00 GMT
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
	-	`sha256:603341c5c367a00c556b1cef2a45967f54bc3c608aeb15b041e6aaeaf5c278ef`  
		Last Modified: Fri, 30 Oct 2020 12:00:22 GMT  
		Size: 1.7 MB (1742583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc8baf174d0a545732e56f7b659d48b19270ad1bcab34fb578b58254810b8966`  
		Last Modified: Fri, 30 Oct 2020 12:00:23 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:def13b85f243d3c6d7c04b72d6ec6736627101e18a3f1d3bfff329fac514f188`  
		Last Modified: Fri, 30 Oct 2020 12:00:22 GMT  
		Size: 118.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-alpine` - linux; s390x

```console
$ docker pull memcached@sha256:a54e2e0ee91bb55a0d8521a4ab8f30649588d259e6b18320f292e51025dc35b8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4676494 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e05224f43fe277aeda8f17fc8ded12da4a0d81a153a08e34d8ddf961d5c2d7e`
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
# Tue, 24 Nov 2020 01:38:51 GMT
ENV MEMCACHED_VERSION=1.6.9
# Tue, 24 Nov 2020 01:38:52 GMT
ENV MEMCACHED_SHA1=42ae062094fdf083cfe7b21ff377c781011c2be1
# Tue, 24 Nov 2020 01:42:39 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		dpkg-dev dpkg 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		tar 		wget 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 24 Nov 2020 01:42:39 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 24 Nov 2020 01:42:41 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 24 Nov 2020 01:42:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 24 Nov 2020 01:42:43 GMT
USER memcache
# Tue, 24 Nov 2020 01:42:43 GMT
EXPOSE 11211
# Tue, 24 Nov 2020 01:42:44 GMT
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
	-	`sha256:18bd0358bc33c61ca0847dc0ae52053ab05c8491609929457c3e5195a035ce1b`  
		Last Modified: Tue, 24 Nov 2020 01:43:20 GMT  
		Size: 2.1 MB (2093430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2eea37208f09cfee5b7632f5f78f5cf51df5b2b248d14d585ba256baad4914f`  
		Last Modified: Tue, 24 Nov 2020 01:43:19 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09896b451609b7d0e69a6af517cff8a599cf66df743696a3b53b57bd13d89582`  
		Last Modified: Tue, 24 Nov 2020 01:43:19 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
