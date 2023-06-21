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
