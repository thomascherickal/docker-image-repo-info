## `memcached:1-alpine3.15`

```console
$ docker pull memcached@sha256:193e15ea545f37aa25c7180a43b9ab71da62db81a45251359a018aafc6706754
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `memcached:1-alpine3.15` - linux; amd64

```console
$ docker pull memcached@sha256:7cb5b54e26c0f5f6dde5d79ff088e31f395411ceed4b03cb572de43505abd037
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3864339 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a6f5112bfdf77b998aa77fb83a7f2bce3d5af41510a936973eec924ec34cb39d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 29 Mar 2022 00:19:36 GMT
ADD file:3b5a33c96fd3c10d0c438d907ce172903f7b2bde0f4e5107831e135ddf111b19 in / 
# Tue, 29 Mar 2022 00:19:36 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 15:51:14 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 29 Mar 2022 15:51:15 GMT
RUN apk add --no-cache libsasl
# Tue, 29 Mar 2022 15:51:15 GMT
ENV MEMCACHED_VERSION=1.6.14
# Tue, 29 Mar 2022 15:51:16 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Tue, 29 Mar 2022 15:55:06 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 29 Mar 2022 15:55:07 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 29 Mar 2022 15:55:07 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 29 Mar 2022 15:55:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 29 Mar 2022 15:55:07 GMT
USER memcache
# Tue, 29 Mar 2022 15:55:07 GMT
EXPOSE 11211
# Tue, 29 Mar 2022 15:55:07 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:40e059520d199e1a1a259089077f2a0c879951c9a4540490bad3a0d7714c6ae7`  
		Last Modified: Mon, 28 Mar 2022 23:30:57 GMT  
		Size: 2.8 MB (2814512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27b0e2187473c5b3c9492eae115e2e4dacfdfc06f78ea00c2a0b3b1455c40cdf`  
		Last Modified: Tue, 29 Mar 2022 15:56:06 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b7814c37b63c095afd6c29f878f1462bdeb47b5c3d2bf115e29d63fc3a88c01`  
		Last Modified: Tue, 29 Mar 2022 15:56:06 GMT  
		Size: 109.2 KB (109177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99c527deaa62aff904bcd0684fcf406a73b892701f5b4e71886d890e0773f0e1`  
		Last Modified: Tue, 29 Mar 2022 15:56:06 GMT  
		Size: 939.0 KB (938982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:419557d66ea1c2ce1a4585b4b60075ee390bb987ab330529ea782e592d5052fe`  
		Last Modified: Tue, 29 Mar 2022 15:56:06 GMT  
		Size: 280.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7cd40dea95b2fe93f2258abdf49950bbceebda3dc2ca8b41fe38f703970195f`  
		Last Modified: Tue, 29 Mar 2022 15:56:05 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-alpine3.15` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:1879b7c4695f0e15fb3a6651c0baa1ad79909e2ddf146ab9acaef8e261649fb6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3756089 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:477772a96f8ed2eb73ed4cb43f26e0759fb78c58555dc6209d4cd3d5dc523184`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 29 Mar 2022 00:40:05 GMT
ADD file:24e8b04304ef91bbf949674909ccaf2c66e3dcd096c3c307a0510569eadf576f in / 
# Tue, 29 Mar 2022 00:40:05 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 12:15:46 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 29 Mar 2022 12:15:48 GMT
RUN apk add --no-cache libsasl
# Tue, 29 Mar 2022 12:15:49 GMT
ENV MEMCACHED_VERSION=1.6.14
# Tue, 29 Mar 2022 12:15:50 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Tue, 29 Mar 2022 12:18:49 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 29 Mar 2022 12:18:51 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 29 Mar 2022 12:18:51 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 29 Mar 2022 12:18:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 29 Mar 2022 12:18:53 GMT
USER memcache
# Tue, 29 Mar 2022 12:18:54 GMT
EXPOSE 11211
# Tue, 29 Mar 2022 12:18:55 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:80fa7f07ec7b717ec5f8e2717b91e3d659e129052ec3def2570a5674322688d9`  
		Last Modified: Tue, 29 Mar 2022 00:41:08 GMT  
		Size: 2.7 MB (2716347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f10b8b6cab642fcf434c73ffafd368a2957c1bcffc899eab76fc97b0dc0104df`  
		Last Modified: Tue, 29 Mar 2022 12:20:15 GMT  
		Size: 1.2 KB (1240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1ae26cb130c189f6c90ab2a00b9869cd303a8f015b22e8a8e7f323603ce189f`  
		Last Modified: Tue, 29 Mar 2022 12:20:15 GMT  
		Size: 110.5 KB (110504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad24a2012747b16e96884e25f084c2ae322f6eb1297c07c9b35b32fd788de3ad`  
		Last Modified: Tue, 29 Mar 2022 12:20:15 GMT  
		Size: 927.6 KB (927594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4d2de24d3ae001fe4e34957c61528d7f4c942ecbdbfeb2cc2ad3bbbedc0d821`  
		Last Modified: Tue, 29 Mar 2022 12:20:15 GMT  
		Size: 283.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea12d8f2572be56c778f320cf2cb4b9df90e59ff5b9271f6e0694bdf3a328ecf`  
		Last Modified: Tue, 29 Mar 2022 12:20:15 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-alpine3.15` - linux; 386

```console
$ docker pull memcached@sha256:3a57e189b8a05f3869fcffa07dafd6f113fba91152352cc3755e6a8caa8716d5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3888284 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f1c6da0099e853f69c7f11687b63af6550a0971b63bf67e766c48941b888a3a1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 29 Mar 2022 00:38:32 GMT
ADD file:8d3b249cd4cd9b2fb1888f3efcc06d39c2f56b4c25257ecee645c1be0146f7fd in / 
# Tue, 29 Mar 2022 00:38:33 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 05:55:14 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 29 Mar 2022 05:55:15 GMT
RUN apk add --no-cache libsasl
# Tue, 29 Mar 2022 05:55:16 GMT
ENV MEMCACHED_VERSION=1.6.14
# Tue, 29 Mar 2022 05:55:17 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Tue, 29 Mar 2022 05:58:08 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 29 Mar 2022 05:58:10 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 29 Mar 2022 05:58:10 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 29 Mar 2022 05:58:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 29 Mar 2022 05:58:12 GMT
USER memcache
# Tue, 29 Mar 2022 05:58:13 GMT
EXPOSE 11211
# Tue, 29 Mar 2022 05:58:14 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:134f45dc6b904419acf27b9807970f271117691bc67b963b86de8965db932175`  
		Last Modified: Tue, 29 Mar 2022 00:39:35 GMT  
		Size: 2.8 MB (2818926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b025aab6ef850f12e7930415ee8b8b862e6ae62d6ab9831ed1ba640c5c10ca4c`  
		Last Modified: Tue, 29 Mar 2022 05:59:30 GMT  
		Size: 1.2 KB (1239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e94bdf2743784dacdafc11884df742673dc7194f6d86423e3c118d9a6e6387ce`  
		Last Modified: Tue, 29 Mar 2022 05:59:30 GMT  
		Size: 120.9 KB (120870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4064b2cd0f143dff906d32e679520c1b9642eb7d4d3e1245fc331ec24c7046f`  
		Last Modified: Tue, 29 Mar 2022 05:59:31 GMT  
		Size: 946.8 KB (946849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:178107cfc4ce09821bac84c72ff339c470023f513394c2f1a8cdfed81cde1968`  
		Last Modified: Tue, 29 Mar 2022 05:59:31 GMT  
		Size: 282.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3474e1394263fa2a6fc98534e4496929fe5ebf3453bd2e8961c4e9c8f4a4b646`  
		Last Modified: Tue, 29 Mar 2022 05:59:30 GMT  
		Size: 118.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-alpine3.15` - linux; ppc64le

```console
$ docker pull memcached@sha256:ea9d9ea93474614a47062c28a534bcb28a4b34227ac9c832ee0b0793e5911a11
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3907382 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c0f07418708ef893842302c48b8fc06f951730795d82cfd7969e98409703740`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 23 Mar 2022 15:24:30 GMT
ADD file:3392b3547a6a1366b9a6ada72065830d8886708bbfc70472c607e742dfd07994 in / 
# Wed, 23 Mar 2022 15:24:32 GMT
CMD ["/bin/sh"]
# Wed, 23 Mar 2022 20:44:22 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Wed, 23 Mar 2022 20:44:33 GMT
RUN apk add --no-cache libsasl
# Wed, 23 Mar 2022 20:44:37 GMT
ENV MEMCACHED_VERSION=1.6.14
# Wed, 23 Mar 2022 20:44:40 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Wed, 23 Mar 2022 20:47:41 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Wed, 23 Mar 2022 20:47:44 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 23 Mar 2022 20:47:53 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 23 Mar 2022 20:47:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 23 Mar 2022 20:47:59 GMT
USER memcache
# Wed, 23 Mar 2022 20:48:02 GMT
EXPOSE 11211
# Wed, 23 Mar 2022 20:48:04 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:58323f60457d1c04dce77185ce8c0377ac10135b55fdf4506e87d24e67780d7d`  
		Last Modified: Wed, 23 Mar 2022 15:25:23 GMT  
		Size: 2.8 MB (2814037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49c21486966ee97b06bdcf6aa49bccd1b95c8d89b7678b5db920b549709b65dc`  
		Last Modified: Wed, 23 Mar 2022 20:48:57 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26831e4f705a05888236c65e02502584ff220e2875c0f8df1938b9c8f13d585d`  
		Last Modified: Wed, 23 Mar 2022 20:48:57 GMT  
		Size: 126.1 KB (126149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:202f0c5bc6581cdafd64cbc07da87c6c0e78f5c33a190ad78663107b8fe67cf9`  
		Last Modified: Wed, 23 Mar 2022 20:48:57 GMT  
		Size: 965.5 KB (965524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e324486d17bceda8e6ebc22ee6e07373f9e46ae73c7bc64f464dcc6e593de1a`  
		Last Modified: Wed, 23 Mar 2022 20:48:57 GMT  
		Size: 283.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c82c1ae2ba35483f92c1a0af509e4d4171b0be7426d2390c72d493c43fef9c4a`  
		Last Modified: Wed, 23 Mar 2022 20:48:57 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-alpine3.15` - linux; s390x

```console
$ docker pull memcached@sha256:22ba706f6470fcee976dc72a19885f1b404b8a4969aeaf308f3c2bd2a57a637e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.7 MB (3651059 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:01d985a687b90bb5ab52e8f5ea365f869cd1d1e8cc0cb96e162b4d413e912662`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 23 Mar 2022 15:41:27 GMT
ADD file:c6fe4c8affcc912e0de86d8691aecb959ac828259f09843a569ec4e5714d6c6f in / 
# Wed, 23 Mar 2022 15:41:27 GMT
CMD ["/bin/sh"]
# Wed, 23 Mar 2022 19:23:12 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Wed, 23 Mar 2022 19:23:13 GMT
RUN apk add --no-cache libsasl
# Wed, 23 Mar 2022 19:23:13 GMT
ENV MEMCACHED_VERSION=1.6.14
# Wed, 23 Mar 2022 19:23:13 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Wed, 23 Mar 2022 19:26:40 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Wed, 23 Mar 2022 19:26:40 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 23 Mar 2022 19:26:40 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 23 Mar 2022 19:26:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 23 Mar 2022 19:26:41 GMT
USER memcache
# Wed, 23 Mar 2022 19:26:41 GMT
EXPOSE 11211
# Wed, 23 Mar 2022 19:26:41 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:cf2f18c21a46b2d59a7a34a051c9c289710e89cdef47cc582fdb9d65a1e68e44`  
		Last Modified: Wed, 23 Mar 2022 15:42:18 GMT  
		Size: 2.6 MB (2601698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2e16ee8799723c65d4a3f828a44428422e20be991172621139b6d7e1c7018b7`  
		Last Modified: Wed, 23 Mar 2022 19:27:30 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65abab6efc031c671a8f2cdbb2a7643066ddf401e8767db082a36bce7cc111e1`  
		Last Modified: Wed, 23 Mar 2022 19:27:30 GMT  
		Size: 113.4 KB (113446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aae9b4754acb16c953a4a8e0d6b87c3f48d5a3a657040a9b9c5b0f4f3260539b`  
		Last Modified: Wed, 23 Mar 2022 19:27:30 GMT  
		Size: 934.2 KB (934243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:317006ee42846f1406454720d6a51cc3ffe807b5d9d104e64a569b216b78024d`  
		Last Modified: Wed, 23 Mar 2022 19:27:30 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f10b61971c858a9a937423d253e21b0d35165794e3a4c470e293bd1ef2588782`  
		Last Modified: Wed, 23 Mar 2022 19:27:30 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
