## `memcached:1-alpine`

```console
$ docker pull memcached@sha256:b9d478a65a9936c29d3dc92d79d1755869ffa412e64040ccc3f10f8c2f1f4436
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 11
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	unknown; unknown
	-	linux; 386
	-	unknown; unknown
	-	linux; ppc64le
	-	unknown; unknown
	-	linux; s390x
	-	unknown; unknown

### `memcached:1-alpine` - linux; amd64

```console
$ docker pull memcached@sha256:04d0d1df8b87df09639e1e9995971ad2ad8fe66c2d02e4987076a370a271a956
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4462859 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3012cf09bdc9226b392bd2af8f268f16f77c6fe65b3f72f558668e15047b8807`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 08 Dec 2023 01:20:49 GMT
ADD file:1f4eb46669b5b6275af19eb7471a6899a61c276aa7d925b8ae99310b14b75b92 in / 
# Fri, 08 Dec 2023 01:20:49 GMT
CMD ["/bin/sh"]
# Sat, 09 Dec 2023 01:54:10 GMT
RUN set -eux; 	addgroup -g 11211 memcache; 	adduser -D -u 11211 -G memcache memcache # buildkit
# Sat, 09 Dec 2023 01:54:10 GMT
RUN apk add --no-cache libsasl # buildkit
# Sat, 09 Dec 2023 01:54:10 GMT
ENV MEMCACHED_VERSION=1.6.22
# Sat, 09 Dec 2023 01:54:10 GMT
ENV MEMCACHED_URL=https://memcached.org/files/memcached-1.6.22.tar.gz
# Sat, 09 Dec 2023 01:54:10 GMT
ENV MEMCACHED_SHA1=7a691f390d59616dbebfc9e2e4942d499c39a338
# Sat, 09 Dec 2023 01:54:10 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		dpkg-dev dpkg 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 	; 		wget -O memcached.tar.gz "$MEMCACHED_URL"; 	echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c -; 	mkdir -p /usr/src/memcached; 	tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1; 	rm memcached.tar.gz; 		cd /usr/src/memcached; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	; 	nproc="$(nproc)"; 	make -j "$nproc"; 		make test PARALLEL="$nproc"; 		make install; 		cd /; 	rm -rf /usr/src/memcached; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .memcached-rundeps $runDeps; 	apk del --no-network .build-deps; 		memcached -V # buildkit
# Sat, 09 Dec 2023 01:54:10 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Sat, 09 Dec 2023 01:54:10 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Sat, 09 Dec 2023 01:54:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 09 Dec 2023 01:54:10 GMT
USER memcache
# Sat, 09 Dec 2023 01:54:10 GMT
EXPOSE map[11211/tcp:{}]
# Sat, 09 Dec 2023 01:54:10 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:661ff4d9561e3fd050929ee5097067c34bafc523ee60f5294a37fd08056a73ca`  
		Last Modified: Fri, 08 Dec 2023 01:21:10 GMT  
		Size: 3.4 MB (3408480 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ca103d2276212cc687cf236216a50e9bf98e0d696a8a63a573990e5b75e2a7e0`  
		Last Modified: Tue, 12 Dec 2023 20:52:46 GMT  
		Size: 1.2 KB (1242 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:cecbbbad4976dcd0f62489adc6ade439608ccbc5c8d64aa96df8578451559665`  
		Last Modified: Tue, 12 Dec 2023 20:52:46 GMT  
		Size: 104.2 KB (104203 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:64f63893492c8f6b29d157137f9062d5cc26157a9f530a15dbeed5864492734c`  
		Last Modified: Tue, 12 Dec 2023 20:52:46 GMT  
		Size: 948.5 KB (948535 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fe795c6bddfd42e13ac78f0081231f8e0e2ec695f3dfa99a77a26473eb160fc0`  
		Last Modified: Tue, 12 Dec 2023 20:52:46 GMT  
		Size: 277.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:81f873f0cd6918fb2224432d83c505b44e00227672661a3915574dd956e8194e`  
		Last Modified: Tue, 12 Dec 2023 20:52:47 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1-alpine` - unknown; unknown

```console
$ docker pull memcached@sha256:179681d2f3efc2f6d2f58a2255a3ee29c6bf92a37220b1d41ba0b8c80ade0b72
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **98.1 KB (98070 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3277e2ef6023c2abffb46b0362f3b8d7d758fe8b2c1216806c2b190517c70e9b`

```dockerfile
```

-	Layers:
	-	`sha256:9d49890946d1c8bd1ae77de744b5717210d885a7c59e657249b28c3f974e4c10`  
		Last Modified: Tue, 12 Dec 2023 20:52:46 GMT  
		Size: 78.6 KB (78603 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:2bff411886bbd4cfaeb87f474853596227a084233568074067a24f2e2b7bcf48`  
		Last Modified: Tue, 12 Dec 2023 20:52:46 GMT  
		Size: 19.5 KB (19467 bytes)  
		MIME: application/vnd.in-toto+json

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
$ docker pull memcached@sha256:e9673caac3d318f89edf7ca6eaba8910416292f12f0f0abbf3d862a8b5af88ae
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.4 MB (4406434 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a4e56736197b019e201b69449a358660e6806d076b61fd473dbcbb11caf5197`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 16 Oct 2023 06:54:12 GMT
ADD file:d8a30995bbcd627f084912c728fda5483b6ba486de25af588a0956069d0bd7ad in / 
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["/bin/sh"]
# Mon, 16 Oct 2023 06:54:12 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN apk add --no-cache libsasl # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_VERSION=1.6.22
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_SHA1=7a691f390d59616dbebfc9e2e4942d499c39a338
# Mon, 16 Oct 2023 06:54:12 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 16 Oct 2023 06:54:12 GMT
USER memcache
# Mon, 16 Oct 2023 06:54:12 GMT
EXPOSE map[11211/tcp:{}]
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:2c03dbb20264f09924f9eab176da44e5421e74a78b09531d3c63448a7baa7c59`  
		Last Modified: Thu, 30 Nov 2023 23:11:32 GMT  
		Size: 3.3 MB (3333033 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4962e560ef629491acb51e64b06a5ee52545098f8403705778786a404e81434b`  
		Last Modified: Fri, 01 Dec 2023 15:25:24 GMT  
		Size: 1.2 KB (1244 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d4b10238ba82be69f174742e8ae9cd6e4484f32dce6eeb40dcbe3c5a4e0a1480`  
		Last Modified: Fri, 01 Dec 2023 15:25:24 GMT  
		Size: 124.1 KB (124087 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:276ae0cb4d4371459c3116e0453691ac59cdd9a6d649cb27bb3d3a090ef10fbf`  
		Last Modified: Fri, 01 Dec 2023 15:25:24 GMT  
		Size: 947.7 KB (947670 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:315ab34d41c816b04b8d07e4b7db199c17340b3b882b52819a0564f6be31a04c`  
		Last Modified: Fri, 01 Dec 2023 15:25:24 GMT  
		Size: 278.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:024d99cdc8f15c63cc478d1850db680f8c0dfae1ea2a5bca55e41fb0db12d020`  
		Last Modified: Fri, 01 Dec 2023 15:25:25 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1-alpine` - unknown; unknown

```console
$ docker pull memcached@sha256:91dac18281e4a194ee9756cf2652c70b2fb0bd2ba9d26c5c86d44c762d111821
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **96.9 KB (96880 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3590bb02748f6b9e8a22ef90e7b41976bcb90189d98a78beae80f5aab1cd1cf4`

```dockerfile
```

-	Layers:
	-	`sha256:605a9d206d49d790bef9ce82c45179355571f37a91c5730ca6f59a03e13c0c76`  
		Last Modified: Fri, 01 Dec 2023 15:25:24 GMT  
		Size: 78.1 KB (78074 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:95803ef4905954256ae922386b3196bdafabd328ecd648b88ed7d8c13ec3b640`  
		Last Modified: Fri, 01 Dec 2023 15:25:24 GMT  
		Size: 18.8 KB (18806 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:1-alpine` - linux; 386

```console
$ docker pull memcached@sha256:c281c55fd61946d53161839c584fb2bab1e6701155ad4b32c816d6ab0dc21a08
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4692614 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c2fd98aa81c35c4a5fa9401b2f61ac48a2632d3b4b4baacc4b7982b10310097`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 28 Sep 2023 20:38:19 GMT
ADD file:8402753f294e403e92353bd65c86a6428c960be5116c0a15484b663a84f66fcd in / 
# Thu, 28 Sep 2023 20:38:20 GMT
CMD ["/bin/sh"]
# Mon, 16 Oct 2023 06:54:12 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN apk add --no-cache libsasl # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_VERSION=1.6.22
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_SHA1=7a691f390d59616dbebfc9e2e4942d499c39a338
# Mon, 16 Oct 2023 06:54:12 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 16 Oct 2023 06:54:12 GMT
USER memcache
# Mon, 16 Oct 2023 06:54:12 GMT
EXPOSE map[11211/tcp:{}]
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:dc95107ad2a031a015320bb397f73ec151d738127175b31ad643120697dc7e90`  
		Last Modified: Thu, 28 Sep 2023 20:39:32 GMT  
		Size: 3.2 MB (3235757 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4951068162aca253cfa98ba4876636d5f13870e8ae9df08734f097bb6291e163`  
		Last Modified: Wed, 18 Oct 2023 01:04:05 GMT  
		Size: 1.2 KB (1246 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:50e4c32dd77b7a60c60be859a9848c50b3da8b95360dea46acf070797f48ab2a`  
		Last Modified: Wed, 18 Oct 2023 01:04:05 GMT  
		Size: 109.5 KB (109458 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:77aecf5d85dda7360aa3010357b83f206e1873aa4df6de5692c0c39dbf083c2a`  
		Last Modified: Wed, 18 Oct 2023 01:04:06 GMT  
		Size: 1.3 MB (1345750 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:99e49c7a1306cd1125b7dbc332a0b1b47b2408c77e975df11b090c0ab5599be3`  
		Last Modified: Wed, 18 Oct 2023 01:04:06 GMT  
		Size: 281.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:68c5ecf5461e2d137f2c403e26fe6e0532a5ecf0eedcd77a5b18254c82b9a075`  
		Last Modified: Wed, 18 Oct 2023 01:04:07 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1-alpine` - unknown; unknown

```console
$ docker pull memcached@sha256:f0efd827c59fd288434c24a501d257456e82560b34d98f97cfe8b132454e28b4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.7 KB (18687 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ea78294aafd9f308a52d310f899433de63e91eaac550b4ace8c1b8647774c7b8`

```dockerfile
```

-	Layers:
	-	`sha256:8c15fbe468a3b1236cadb64627426b8e2cb8bb71fddd26e10cdc44abd3b3519c`  
		Last Modified: Wed, 18 Oct 2023 01:04:05 GMT  
		Size: 18.7 KB (18687 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:1-alpine` - linux; ppc64le

```console
$ docker pull memcached@sha256:bae49b5a412b4535ebab987425356a20af16fc1ce70c38e18f6aa6572cac522d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4460245 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b845ad70056a07d2adbebdc425879a4eb74152c886dae5d8e5496c6114cd3cda`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 16 Oct 2023 06:54:12 GMT
ADD file:3450a1687b552498a987f87cb844b7f597c7181d7c3d31943d7b3036d5300d5e in / 
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["/bin/sh"]
# Mon, 16 Oct 2023 06:54:12 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN apk add --no-cache libsasl # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_VERSION=1.6.22
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_SHA1=7a691f390d59616dbebfc9e2e4942d499c39a338
# Mon, 16 Oct 2023 06:54:12 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 16 Oct 2023 06:54:12 GMT
USER memcache
# Mon, 16 Oct 2023 06:54:12 GMT
EXPOSE map[11211/tcp:{}]
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:4e13780adf2776477b14ef9c0f4f563f820a2fde166d472218037b979e84d31a`  
		Last Modified: Thu, 30 Nov 2023 23:20:01 GMT  
		Size: 3.3 MB (3348322 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a33c280bf18f1bba1782f90d468941796634b74c44d9aae4c406162114520e9a`  
		Last Modified: Fri, 01 Dec 2023 12:01:06 GMT  
		Size: 1.2 KB (1247 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a54d91525051bf65bd807cac3c6f1a685ac2fc6ec7f763df97c18a3ca4b6dde0`  
		Last Modified: Fri, 01 Dec 2023 12:01:07 GMT  
		Size: 123.9 KB (123864 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:73f73a883ca0c1147533ae5085475dee29244e8ef06b0455c52afa6ab50c3023`  
		Last Modified: Fri, 01 Dec 2023 12:01:07 GMT  
		Size: 986.4 KB (986410 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:183bb794a2f98d5b2192b311c4b597c47ee4ee0bb405558f67827c8afaf0b8d3`  
		Last Modified: Fri, 01 Dec 2023 12:01:07 GMT  
		Size: 280.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:556988ad767ddefdfb131bbf239cceba01e60b197c0893287ee0f6274e54a0c8`  
		Last Modified: Fri, 01 Dec 2023 12:01:08 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1-alpine` - unknown; unknown

```console
$ docker pull memcached@sha256:df95592ada35b125fd73982e23f99a4fc3820ab083e12870f4edb179935ec44d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.3 KB (95332 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:67d44fe1dc00fdfaba957619ac6567e2ba40c2bad9a422ffb5287bb160b01fe7`

```dockerfile
```

-	Layers:
	-	`sha256:4a7a9ea74e3391f7a0e156b244eb474f674d42637b77983cfd9c92b23701d5ce`  
		Last Modified: Fri, 01 Dec 2023 12:01:06 GMT  
		Size: 76.5 KB (76477 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:671ec9ab176a20a138f0a3e238976e619a6f3011f598148b2cadd4c167721f81`  
		Last Modified: Fri, 01 Dec 2023 12:01:07 GMT  
		Size: 18.9 KB (18855 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:1-alpine` - linux; s390x

```console
$ docker pull memcached@sha256:53d0bdb491815057b9014ab30e95c68146d83accdc9d8d690e308e67e7f4eed5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.3 MB (4326665 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b078f3aede6257187e9488318eac328332ace90ac171c8a99d0ca495e1e9ad40`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 08 Dec 2023 01:41:50 GMT
ADD file:47e0982fc3ae485c06d46f3c0022afd39ed7ec95fe755c2391e6b0cfcae65dfc in / 
# Fri, 08 Dec 2023 01:41:51 GMT
CMD ["/bin/sh"]
# Sat, 09 Dec 2023 01:54:10 GMT
RUN set -eux; 	addgroup -g 11211 memcache; 	adduser -D -u 11211 -G memcache memcache # buildkit
# Sat, 09 Dec 2023 01:54:10 GMT
RUN apk add --no-cache libsasl # buildkit
# Sat, 09 Dec 2023 01:54:10 GMT
ENV MEMCACHED_VERSION=1.6.22
# Sat, 09 Dec 2023 01:54:10 GMT
ENV MEMCACHED_URL=https://memcached.org/files/memcached-1.6.22.tar.gz
# Sat, 09 Dec 2023 01:54:10 GMT
ENV MEMCACHED_SHA1=7a691f390d59616dbebfc9e2e4942d499c39a338
# Sat, 09 Dec 2023 01:54:10 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		dpkg-dev dpkg 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 	; 		wget -O memcached.tar.gz "$MEMCACHED_URL"; 	echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c -; 	mkdir -p /usr/src/memcached; 	tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1; 	rm memcached.tar.gz; 		cd /usr/src/memcached; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	; 	nproc="$(nproc)"; 	make -j "$nproc"; 		make test PARALLEL="$nproc"; 		make install; 		cd /; 	rm -rf /usr/src/memcached; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .memcached-rundeps $runDeps; 	apk del --no-network .build-deps; 		memcached -V # buildkit
# Sat, 09 Dec 2023 01:54:10 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Sat, 09 Dec 2023 01:54:10 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Sat, 09 Dec 2023 01:54:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 09 Dec 2023 01:54:10 GMT
USER memcache
# Sat, 09 Dec 2023 01:54:10 GMT
EXPOSE map[11211/tcp:{}]
# Sat, 09 Dec 2023 01:54:10 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:0fca3ee44ced87b7184bc23390283fdf10cfae0e844a25b785dd11c463815227`  
		Last Modified: Fri, 08 Dec 2023 01:42:30 GMT  
		Size: 3.2 MB (3242332 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ff601679be7ba19260a77b326cf587dcc37315b02c2e0b0effc7084da4684bd7`  
		Last Modified: Wed, 13 Dec 2023 00:39:43 GMT  
		Size: 1.2 KB (1242 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:15b2401b35befb0832d96cebfdee6215736b27c0e3d064d67da9917deca4c14c`  
		Last Modified: Wed, 13 Dec 2023 00:39:43 GMT  
		Size: 113.1 KB (113142 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d59b1e1447b7739e5338731014a96bea369258cbf54b2d152ef50bb06e308bad`  
		Last Modified: Wed, 13 Dec 2023 00:39:43 GMT  
		Size: 969.5 KB (969547 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:44c62bb151b09d73f2bc083bb91abedfb6660c5045d34f7d576415190ae4e09f`  
		Last Modified: Wed, 13 Dec 2023 00:39:43 GMT  
		Size: 280.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:eaaf7e6dbf7fbf661d0b3f6f5d38fbd888ab6707a76919a5f4a633194e895a2f`  
		Last Modified: Wed, 13 Dec 2023 00:39:43 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1-alpine` - unknown; unknown

```console
$ docker pull memcached@sha256:1c2ba4c72ac494072ca8249e1368c9974cec5e63ff363b9da79930b7a8fbb5cf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **96.3 KB (96269 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c33c986fa5bcf287e1c7594cc4bc4b13289d51ef15c3db591e513fcb7b653ce`

```dockerfile
```

-	Layers:
	-	`sha256:358b294b5bd4c90ab3ded38657baddb4cf8a5d594c5ea9c5683191efc2c70e05`  
		Last Modified: Wed, 13 Dec 2023 00:39:43 GMT  
		Size: 77.0 KB (76967 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:708c671c1199a85cfb58a91ad4f1c34c29d381f2905468f64a42c8fbb6341e30`  
		Last Modified: Wed, 13 Dec 2023 00:39:43 GMT  
		Size: 19.3 KB (19302 bytes)  
		MIME: application/vnd.in-toto+json
