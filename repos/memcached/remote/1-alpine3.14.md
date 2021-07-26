## `memcached:1-alpine3.14`

```console
$ docker pull memcached@sha256:3abd00ee0f0dbc313fb0fa6d249a1952f91ba6de6ec4eb080f251c2d26657e1e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `memcached:1-alpine3.14` - linux; amd64

```console
$ docker pull memcached@sha256:7963ca0c5d0a949ba3fa43678833e6900f77c270ac891b569223df1216132801
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3901638 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec60b19e2b4daab74b7257390561703247fd3af20418fb7391c60abdca7aa9f5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 15 Jun 2021 22:19:37 GMT
ADD file:f278386b0cef68136129f5f58c52445590a417b624d62bca158d4dc926c340df in / 
# Tue, 15 Jun 2021 22:19:37 GMT
CMD ["/bin/sh"]
# Wed, 16 Jun 2021 23:30:54 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Wed, 16 Jun 2021 23:30:55 GMT
RUN apk add --no-cache libsasl
# Mon, 26 Jul 2021 19:27:36 GMT
ENV MEMCACHED_VERSION=1.6.10
# Mon, 26 Jul 2021 19:27:36 GMT
ENV MEMCACHED_SHA1=cb5b9fe77a2a59cc6cc7103a415bc07df9ddc6ec
# Mon, 26 Jul 2021 19:31:27 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Mon, 26 Jul 2021 19:31:28 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Mon, 26 Jul 2021 19:31:28 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Mon, 26 Jul 2021 19:31:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 26 Jul 2021 19:31:29 GMT
USER memcache
# Mon, 26 Jul 2021 19:31:29 GMT
EXPOSE 11211
# Mon, 26 Jul 2021 19:31:29 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:5843afab387455b37944e709ee8c78d7520df80f8d01cf7f861aae63beeddb6b`  
		Last Modified: Tue, 15 Jun 2021 22:20:04 GMT  
		Size: 2.8 MB (2811478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:736825e042c2579687aee758fbc5a2cfd5d10c6a3f03e74ae5810f6fa85a55f4`  
		Last Modified: Fri, 25 Jun 2021 22:00:17 GMT  
		Size: 1.3 KB (1265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a87d7e8d001446546a89575a4132658d264062ef45659a22de547010377eced1`  
		Last Modified: Fri, 25 Jun 2021 22:00:17 GMT  
		Size: 155.5 KB (155517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b855c3423ec921f0c144ccdc1493e88e71620c3df17a0dc6c325fd16c7a77ce4`  
		Last Modified: Mon, 26 Jul 2021 19:32:18 GMT  
		Size: 933.0 KB (932976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f54bc5bfc189381d8b68884c69c3434f006bb9613fa5a340f02e6bd06f76ea5c`  
		Last Modified: Mon, 26 Jul 2021 19:32:17 GMT  
		Size: 282.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:622aaa105078ae6ceda0c459837865b61c2f59952c4961870b1558f54512f750`  
		Last Modified: Mon, 26 Jul 2021 19:32:17 GMT  
		Size: 120.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-alpine3.14` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:5c106cbec14dc8780b3dc50e3594b43dc8f2d2f92a7c0ecdac41854a323e1308
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3791023 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:329ff8a3e4705214fb434073636cc31465a442c74a672a7c80ca12c01818ac63`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 15 Jun 2021 21:44:56 GMT
ADD file:6797caacbfe41bfe44000b39ed017016c6fcc492b3d6557cdaba88536df6c876 in / 
# Tue, 15 Jun 2021 21:44:56 GMT
CMD ["/bin/sh"]
# Wed, 16 Jun 2021 22:40:03 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Wed, 16 Jun 2021 22:40:04 GMT
RUN apk add --no-cache libsasl
# Mon, 26 Jul 2021 19:55:29 GMT
ENV MEMCACHED_VERSION=1.6.10
# Mon, 26 Jul 2021 19:55:29 GMT
ENV MEMCACHED_SHA1=cb5b9fe77a2a59cc6cc7103a415bc07df9ddc6ec
# Mon, 26 Jul 2021 19:59:23 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Mon, 26 Jul 2021 19:59:23 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Mon, 26 Jul 2021 19:59:24 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Mon, 26 Jul 2021 19:59:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 26 Jul 2021 19:59:24 GMT
USER memcache
# Mon, 26 Jul 2021 19:59:24 GMT
EXPOSE 11211
# Mon, 26 Jul 2021 19:59:24 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:58ab47519297212468320b23b8100fc1b2b96e8d342040806ae509a778a0a07a`  
		Last Modified: Tue, 15 Jun 2021 21:46:03 GMT  
		Size: 2.7 MB (2709626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a56af4dd3838844501a4534d1509f989d1535cb7f10b5a9ecfc9d8e56b1fdf6`  
		Last Modified: Fri, 25 Jun 2021 21:00:15 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:431ad5c56ca4b8ed610161f86dcaeafd33a32c23ab42fbe384e74039a85b37f3`  
		Last Modified: Fri, 25 Jun 2021 21:00:15 GMT  
		Size: 157.2 KB (157186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5dcc1cf978d46dcc8d269173df67e6066a6ac6924dd91483b75081801cd3aae`  
		Last Modified: Mon, 26 Jul 2021 20:01:00 GMT  
		Size: 922.5 KB (922537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:156901a97efd26b4a1ecac0bc4b7e92b72c551f0702385bb2a10a20a43b77951`  
		Last Modified: Mon, 26 Jul 2021 20:01:00 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e07dd7f3a66c6ea62a7f0e0077fb4d40096c11bf23575a463c376c3a3780880f`  
		Last Modified: Mon, 26 Jul 2021 20:00:59 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-alpine3.14` - linux; 386

```console
$ docker pull memcached@sha256:6f5f564475417887b4f60a879268c1cfae556188bda4c782ffefb3795a018137
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3935844 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:507623fc701464de300cfc2326545fc8e67a819a9fe8fe4b4b6cf030e1b3bbdf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 15 Jun 2021 21:38:30 GMT
ADD file:3b0fe1454491bb05e218b090fd461f2fd39546aa4a53eb3f953ee8eae149ac57 in / 
# Tue, 15 Jun 2021 21:38:30 GMT
CMD ["/bin/sh"]
# Wed, 16 Jun 2021 22:39:59 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Wed, 16 Jun 2021 22:40:00 GMT
RUN apk add --no-cache libsasl
# Mon, 26 Jul 2021 19:43:09 GMT
ENV MEMCACHED_VERSION=1.6.10
# Mon, 26 Jul 2021 19:43:10 GMT
ENV MEMCACHED_SHA1=cb5b9fe77a2a59cc6cc7103a415bc07df9ddc6ec
# Mon, 26 Jul 2021 19:47:16 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Mon, 26 Jul 2021 19:47:17 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Mon, 26 Jul 2021 19:47:17 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Mon, 26 Jul 2021 19:47:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 26 Jul 2021 19:47:18 GMT
USER memcache
# Mon, 26 Jul 2021 19:47:18 GMT
EXPOSE 11211
# Mon, 26 Jul 2021 19:47:18 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:be21df321efb39c5daf3151073ebff7688e15ea6cd5158878bc9559a5db76ac6`  
		Last Modified: Tue, 15 Jun 2021 21:39:16 GMT  
		Size: 2.8 MB (2820718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5e63afd3c51d53ab14ff3659f0465573d2b623fed420a40c62679368c3323fe`  
		Last Modified: Fri, 25 Jun 2021 21:55:20 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ed220e7655afd3c4a874ccf1c7cd8940cdbe930e32ee0dcd31a87cec11ced1f`  
		Last Modified: Fri, 25 Jun 2021 21:55:21 GMT  
		Size: 169.0 KB (169017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13619be276174ed900bb993aa654f86927a89e531e1be3691c062bd8aac895c0`  
		Last Modified: Mon, 26 Jul 2021 19:48:48 GMT  
		Size: 944.4 KB (944442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e41b7f0976da4bba64639a8d694de3868ac7dc4c81e37ef6d32dfc5b1c3f037e`  
		Last Modified: Mon, 26 Jul 2021 19:48:48 GMT  
		Size: 280.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9debce64e1b3f15ec71f6478cc89d1ee74479e1e6c30ecdb11e281cd022439b`  
		Last Modified: Mon, 26 Jul 2021 19:48:48 GMT  
		Size: 120.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-alpine3.14` - linux; ppc64le

```console
$ docker pull memcached@sha256:009cabefb8f849ddf50c65ab372f727b550e07c773ef7c540ca81a1af2bb6d33
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.0 MB (3953055 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ac1b3c128317206c80e87e76aa1d3e56bb1eb04caab61a1f35e0dcf9fda80b02`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 15 Jun 2021 22:27:00 GMT
ADD file:0075aad7a94f0496483442bb2d9fdaa13e9c23087b90638d014b4bc263aa3861 in / 
# Tue, 15 Jun 2021 22:27:03 GMT
CMD ["/bin/sh"]
# Thu, 15 Jul 2021 21:17:14 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Thu, 15 Jul 2021 21:17:41 GMT
RUN apk add --no-cache libsasl
# Mon, 26 Jul 2021 20:26:11 GMT
ENV MEMCACHED_VERSION=1.6.10
# Mon, 26 Jul 2021 20:26:13 GMT
ENV MEMCACHED_SHA1=cb5b9fe77a2a59cc6cc7103a415bc07df9ddc6ec
# Mon, 26 Jul 2021 20:29:39 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Mon, 26 Jul 2021 20:29:43 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Mon, 26 Jul 2021 20:29:58 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Mon, 26 Jul 2021 20:30:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 26 Jul 2021 20:30:15 GMT
USER memcache
# Mon, 26 Jul 2021 20:30:22 GMT
EXPOSE 11211
# Mon, 26 Jul 2021 20:30:25 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:baf144cfb66ebe9df1969f3b90f1c448beff98edc84de1ccb5d6346195a070d4`  
		Last Modified: Tue, 15 Jun 2021 22:27:38 GMT  
		Size: 2.8 MB (2810478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:031d07891c778c1d35d939c520c056d259e4333f504d806b9aad087150f51568`  
		Last Modified: Thu, 22 Jul 2021 08:16:02 GMT  
		Size: 1.3 KB (1276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e785b429baa06f8ed8fc94be5fea3e63da83198785705745f45eac9ad09c4e0`  
		Last Modified: Thu, 22 Jul 2021 08:16:02 GMT  
		Size: 179.6 KB (179646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbaf179ebeadb0207bcd0e2f5807a58fa39e2130bf77d61306ae0ead5d5ee521`  
		Last Modified: Mon, 26 Jul 2021 20:31:55 GMT  
		Size: 961.3 KB (961254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:629cf46fc8b6c8f7c62f0c0b00556a9588e9da327aea5aae9b54cbde821ec70d`  
		Last Modified: Mon, 26 Jul 2021 20:31:55 GMT  
		Size: 283.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbfd660306d6b8953251347905b548bedaaa20ce1f6f5b028231259ac443c91b`  
		Last Modified: Mon, 26 Jul 2021 20:31:55 GMT  
		Size: 118.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
