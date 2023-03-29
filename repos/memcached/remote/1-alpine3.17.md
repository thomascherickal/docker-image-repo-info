## `memcached:1-alpine3.17`

```console
$ docker pull memcached@sha256:c74f34b9d8cb7fd8f97605c8a6422bfa5798a760be44f1d352d130e09c29f37e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `memcached:1-alpine3.17` - linux; amd64

```console
$ docker pull memcached@sha256:edbf7d9971836aec40a14e9df1c3ee0727a02c19a7a779adf17c0b113e96ca20
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.4 MB (4438028 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bfbfe4534dcb1c5334597ff0db1fbf9bd028042be924bd311dba424d645d579b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Sat, 11 Feb 2023 04:46:42 GMT
ADD file:40887ab7c06977737e63c215c9bd297c0c74de8d12d16ebdf1c3d40ac392f62d in / 
# Sat, 11 Feb 2023 04:46:42 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 09:58:30 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Sat, 11 Feb 2023 09:58:31 GMT
RUN apk add --no-cache libsasl
# Thu, 09 Mar 2023 23:22:40 GMT
ENV MEMCACHED_VERSION=1.6.19
# Thu, 09 Mar 2023 23:22:40 GMT
ENV MEMCACHED_SHA1=105e87e7fbf13fb826c5d81e4646c865c56f14d1
# Thu, 09 Mar 2023 23:25:12 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Thu, 09 Mar 2023 23:25:12 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 09 Mar 2023 23:25:13 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 09 Mar 2023 23:25:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 09 Mar 2023 23:25:13 GMT
USER memcache
# Thu, 09 Mar 2023 23:25:13 GMT
EXPOSE 11211
# Thu, 09 Mar 2023 23:25:13 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:63b65145d645c1250c391b2d16ebe53b3747c295ca8ba2fcb6b0cf064a4dc21c`  
		Last Modified: Fri, 10 Feb 2023 22:41:31 GMT  
		Size: 3.4 MB (3374446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c9d34df899bc98bf58070807c47869c3b9eab68834980e4dcf59b244b1988d6`  
		Last Modified: Sat, 11 Feb 2023 10:01:27 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:babd87796391ae4372d9c412d9783a94c6be3d0d472aff809b7e068872a2a4e0`  
		Last Modified: Sat, 11 Feb 2023 10:01:27 GMT  
		Size: 108.7 KB (108725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e3a7452ac3c31d9cc370dff48d9f19288a6f1d9fafab71432be5288b08e8ecb`  
		Last Modified: Thu, 09 Mar 2023 23:26:01 GMT  
		Size: 953.2 KB (953185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b1f27f97b2c50ab2b97259bc68deea8bb5a874b3576a0a6c00cdd57a214626f`  
		Last Modified: Thu, 09 Mar 2023 23:26:01 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:197d09636ae5c10ef87fb74137cc01f7ad8b18a70466910c77868618ec2cdbfd`  
		Last Modified: Thu, 09 Mar 2023 23:26:01 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-alpine3.17` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:a804066a8d2851e68eda59abcd6eecac45d53a053483653a658d3e512dbd1a2d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.3 MB (4327176 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91fb020a8f057e1b05f44242a9ef90a8a97bc12b14f5b728b188dae43cea22af`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:08 GMT
ADD file:9bd9ea42a9f3bdc769e80c6b8a4b117d65f73ae68e155a6172a1184e7ac8bcc1 in / 
# Fri, 10 Feb 2023 21:24:08 GMT
CMD ["/bin/sh"]
# Fri, 10 Feb 2023 23:02:57 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Fri, 10 Feb 2023 23:02:58 GMT
RUN apk add --no-cache libsasl
# Thu, 09 Mar 2023 22:42:31 GMT
ENV MEMCACHED_VERSION=1.6.19
# Thu, 09 Mar 2023 22:42:31 GMT
ENV MEMCACHED_SHA1=105e87e7fbf13fb826c5d81e4646c865c56f14d1
# Thu, 09 Mar 2023 22:45:28 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Thu, 09 Mar 2023 22:45:29 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 09 Mar 2023 22:45:29 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 09 Mar 2023 22:45:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 09 Mar 2023 22:45:29 GMT
USER memcache
# Thu, 09 Mar 2023 22:45:29 GMT
EXPOSE 11211
# Thu, 09 Mar 2023 22:45:29 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:af6eaf76a39c2d3e7e0b8a0420486e3df33c4027d696c076a99a3d0ac09026af`  
		Last Modified: Fri, 10 Feb 2023 21:24:39 GMT  
		Size: 3.3 MB (3261959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b800dc4bc77d97a32c77cc040cf8af17620cd05559e1ddc5b71e2ec4b9f74d1e`  
		Last Modified: Fri, 10 Feb 2023 23:06:11 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:962c33dd1aa58ccc5344306a91c3fcfbfe6b4ad91358a838b241bc4788603f12`  
		Last Modified: Fri, 10 Feb 2023 23:06:11 GMT  
		Size: 120.4 KB (120434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:553b274f6b67f0cf63eaeff174c431816d492a83c3851667bba01ff07a7521b4`  
		Last Modified: Thu, 09 Mar 2023 22:46:21 GMT  
		Size: 943.1 KB (943111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae2f475e9afc5eb121bbc63e408b67878599c15c76c6f5d484370d9d65bb2a31`  
		Last Modified: Thu, 09 Mar 2023 22:46:20 GMT  
		Size: 283.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0a95a9f823d01d54a201c1755fa8ed0fe5620c4ec73fd0f2bdce1047e565e0f`  
		Last Modified: Thu, 09 Mar 2023 22:46:20 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-alpine3.17` - linux; 386

```console
$ docker pull memcached@sha256:8fac0cb14b2a1294972b8dddd626a68eaef4c19c3227ee6f35fcfb9ffc217ed1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4501280 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e6420b0eb91ad6fce2add523afa96efcb325bc4cadd5614a0b99e6fa2ce074c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:23 GMT
ADD file:125f3514520a5cd29df2830a409aa026a2bc06a77a7a5d150133436404b33d41 in / 
# Fri, 10 Feb 2023 21:24:24 GMT
CMD ["/bin/sh"]
# Wed, 01 Mar 2023 03:01:23 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Wed, 01 Mar 2023 03:01:24 GMT
RUN apk add --no-cache libsasl
# Thu, 09 Mar 2023 22:44:45 GMT
ENV MEMCACHED_VERSION=1.6.19
# Thu, 09 Mar 2023 22:44:45 GMT
ENV MEMCACHED_SHA1=105e87e7fbf13fb826c5d81e4646c865c56f14d1
# Thu, 09 Mar 2023 22:48:51 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Thu, 09 Mar 2023 22:48:51 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 09 Mar 2023 22:48:51 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 09 Mar 2023 22:48:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 09 Mar 2023 22:48:52 GMT
USER memcache
# Thu, 09 Mar 2023 22:48:52 GMT
EXPOSE 11211
# Thu, 09 Mar 2023 22:48:52 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:b3e346c15c2377ec0e75cc9efa98baecd58b0e9bb92f0ec07eeda0bcc7e67fc7`  
		Last Modified: Fri, 10 Feb 2023 21:25:13 GMT  
		Size: 3.4 MB (3412353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50e0c8da1896350b7b35eb3d73de07e96683cae46c927206d4358c75861a5237`  
		Last Modified: Wed, 01 Mar 2023 03:06:35 GMT  
		Size: 1.3 KB (1266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e7953e5895402c2d68ff08541d4e2a542a70625f9201d71ce02e5ce89fe8cbd`  
		Last Modified: Wed, 01 Mar 2023 03:06:35 GMT  
		Size: 120.5 KB (120473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01f77f09ca6c0590c7ecf7a169fd6d8e2feaab85113cdc32311285529c8551b3`  
		Last Modified: Thu, 09 Mar 2023 22:50:13 GMT  
		Size: 966.8 KB (966782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddf3e3ea4fea6a4015aa833d5d58a03e9876c644a5bd71098343707a9f476fbd`  
		Last Modified: Thu, 09 Mar 2023 22:50:13 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80a71addae447425ffd6a049de1acb491c1e8c3ef55edfd8c6b00d7ed7356af2`  
		Last Modified: Thu, 09 Mar 2023 22:50:13 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-alpine3.17` - linux; ppc64le

```console
$ docker pull memcached@sha256:4d8d53001fdedbbe22ac1fb7e8246b82603aab72deb9466f8165c6320fbfe21c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4498846 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:29308dd54cca915f88cf1541ca3602a7507b8bb015bb9c82a3c6570ca40f5440`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 10 Feb 2023 21:20:36 GMT
ADD file:ec037a0d4b462d12963ac20d9ec49bb73b4bcaf84d4bc7b364ebf93667e585b0 in / 
# Fri, 10 Feb 2023 21:20:36 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 05:34:06 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Sat, 11 Feb 2023 05:34:09 GMT
RUN apk add --no-cache libsasl
# Thu, 09 Mar 2023 23:21:01 GMT
ENV MEMCACHED_VERSION=1.6.19
# Thu, 09 Mar 2023 23:21:01 GMT
ENV MEMCACHED_SHA1=105e87e7fbf13fb826c5d81e4646c865c56f14d1
# Thu, 09 Mar 2023 23:24:35 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Thu, 09 Mar 2023 23:24:35 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 09 Mar 2023 23:24:37 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 09 Mar 2023 23:24:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 09 Mar 2023 23:24:39 GMT
USER memcache
# Thu, 09 Mar 2023 23:24:39 GMT
EXPOSE 11211
# Thu, 09 Mar 2023 23:24:40 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:aa3c56f9c6f127b6c8f628c95db165741ca400d19bdaef2752d80f093e47451e`  
		Last Modified: Fri, 10 Feb 2023 21:21:37 GMT  
		Size: 3.4 MB (3390750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04d03a14bc153c819b47151bf115c150a0bd72f664a0a947a3080098f4155e7c`  
		Last Modified: Sat, 11 Feb 2023 05:38:28 GMT  
		Size: 1.3 KB (1266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c2a35bdf2a74cf476c396c1507730634e96580c56b436e3a5abbecd92fbd424`  
		Last Modified: Sat, 11 Feb 2023 05:38:28 GMT  
		Size: 125.3 KB (125328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52a9fe4af298ad054a9989bea90b5ec49d7b02bd188c18671dec534e010bd58d`  
		Last Modified: Thu, 09 Mar 2023 23:26:02 GMT  
		Size: 981.1 KB (981094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c24b2d29fddefd04e944a9b619123d8386ed2155b8cadc1da54bf52af45d336`  
		Last Modified: Thu, 09 Mar 2023 23:26:02 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a4e5abe10e88810dba0caed164da51c4f37ef590c11538f2b30fa72a4e5c5d7`  
		Last Modified: Thu, 09 Mar 2023 23:26:02 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-alpine3.17` - linux; s390x

```console
$ docker pull memcached@sha256:abb7fe9a70083c3e6dd78b9dca293a7ec060dcc6f76711279b49104756596a8c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4236344 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:32b2bd5047a38e78e421875a36a2a31d7b29909fe7eb8d075cf075ba30664661`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 29 Mar 2023 17:41:57 GMT
ADD file:675ad8acf4b076e34aeeba26dd482be7640df5912b1ec5e3183b7eb69c01e83e in / 
# Wed, 29 Mar 2023 17:41:57 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 18:48:17 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Wed, 29 Mar 2023 18:48:18 GMT
RUN apk add --no-cache libsasl
# Wed, 29 Mar 2023 18:48:18 GMT
ENV MEMCACHED_VERSION=1.6.19
# Wed, 29 Mar 2023 18:48:18 GMT
ENV MEMCACHED_SHA1=105e87e7fbf13fb826c5d81e4646c865c56f14d1
# Wed, 29 Mar 2023 18:51:55 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Wed, 29 Mar 2023 18:51:55 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 29 Mar 2023 18:51:56 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 29 Mar 2023 18:51:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 29 Mar 2023 18:51:56 GMT
USER memcache
# Wed, 29 Mar 2023 18:51:56 GMT
EXPOSE 11211
# Wed, 29 Mar 2023 18:51:56 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:a76f78d8854217635d8049ec8501edb806f961e72989cfff8503982e6ff2579d`  
		Last Modified: Wed, 29 Mar 2023 17:42:31 GMT  
		Size: 3.2 MB (3175187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fd08642be91a342be38d3bfe200cfd81beb88b99302a76f38b79c2e1a3eb9ee`  
		Last Modified: Wed, 29 Mar 2023 18:52:18 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:871e6692d297067c237b13c08321f584b70e4e1406f61ce2305386063470c707`  
		Last Modified: Wed, 29 Mar 2023 18:52:18 GMT  
		Size: 112.9 KB (112866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb6755bb5881de3899c6b93ba7388fb7ef3b65a28f77bfcf79ca68646317c508`  
		Last Modified: Wed, 29 Mar 2023 18:52:18 GMT  
		Size: 946.6 KB (946623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfe8924cd483e904ffcd4a125ad19bf66557488ba8e0c9a4ece41394f97e7048`  
		Last Modified: Wed, 29 Mar 2023 18:52:18 GMT  
		Size: 279.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26b805df42ae1f903d91a3e5ae420dba382a11a9ca77eb9523c7873db21e614d`  
		Last Modified: Wed, 29 Mar 2023 18:52:18 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
