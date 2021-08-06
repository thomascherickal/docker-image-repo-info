## `memcached:alpine3.14`

```console
$ docker pull memcached@sha256:799228a970ea96d394b1d8e1241c37e27b0fb84d5a89168a35553372269cc050
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `memcached:alpine3.14` - linux; amd64

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

### `memcached:alpine3.14` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:3d93273af96de43b51add0d01ffec6cb248a83a6b4adf02cc9e6051b3f96fbd8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3792018 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ca1be9ff405513cf815b965422761dd197bd3f72229bb2973ea006961381a309`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 06 Aug 2021 17:39:26 GMT
ADD file:1a8fd1066485e1261462e689c1a072f010c1d3be904b73ef2b84128fac652951 in / 
# Fri, 06 Aug 2021 17:39:27 GMT
CMD ["/bin/sh"]
# Fri, 06 Aug 2021 19:44:13 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Fri, 06 Aug 2021 19:44:14 GMT
RUN apk add --no-cache libsasl
# Fri, 06 Aug 2021 19:44:14 GMT
ENV MEMCACHED_VERSION=1.6.10
# Fri, 06 Aug 2021 19:44:15 GMT
ENV MEMCACHED_SHA1=cb5b9fe77a2a59cc6cc7103a415bc07df9ddc6ec
# Fri, 06 Aug 2021 19:48:06 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Fri, 06 Aug 2021 19:48:07 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 06 Aug 2021 19:48:07 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 06 Aug 2021 19:48:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 06 Aug 2021 19:48:08 GMT
USER memcache
# Fri, 06 Aug 2021 19:48:08 GMT
EXPOSE 11211
# Fri, 06 Aug 2021 19:48:08 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:fd3acdcea5682abced546ec19fb6ebee725c5184e5d91614c469c0a79e67f2d0`  
		Last Modified: Fri, 06 Aug 2021 17:40:12 GMT  
		Size: 2.7 MB (2710613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3e7ec193b32b8cfc53263af4e876a7055d4318058e76620bce0544f9120c6c7`  
		Last Modified: Fri, 06 Aug 2021 19:49:06 GMT  
		Size: 1.3 KB (1266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af2047017486a2b18ef6819325e63c7b73faa11404da5ac0addfeeaa66c34d35`  
		Last Modified: Fri, 06 Aug 2021 19:49:06 GMT  
		Size: 157.2 KB (157197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d96bbd7be8b6283902f7bac12c1e45e0cf356d8b8d1c57e298f2df6946aed0d`  
		Last Modified: Fri, 06 Aug 2021 19:49:07 GMT  
		Size: 922.5 KB (922540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7159339c1b34149bc53211472fa2171a492cfcac24ae0584d0e5b8743700edd7`  
		Last Modified: Fri, 06 Aug 2021 19:49:06 GMT  
		Size: 281.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fe1a76a68267bbc6ec790cb0ee914959f9afc0a827978dfc8e5b637dc7a76bc`  
		Last Modified: Fri, 06 Aug 2021 19:49:06 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:alpine3.14` - linux; 386

```console
$ docker pull memcached@sha256:5b703164d69411526a5b9b2c50e0919566ddefb848e2ab407ec1bc2a6d9a50d9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3937070 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f06fd71826f53b91e8eca0ddffb1a454f5fbe08b04c9af8057692edb69b655e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 06 Aug 2021 17:38:26 GMT
ADD file:bafaec4a54d6cef99b5f3660d074a3d2251e4d4bd09df9ea65f33e9bffb7d88d in / 
# Fri, 06 Aug 2021 17:38:26 GMT
CMD ["/bin/sh"]
# Fri, 06 Aug 2021 19:40:06 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Fri, 06 Aug 2021 19:40:08 GMT
RUN apk add --no-cache libsasl
# Fri, 06 Aug 2021 19:40:08 GMT
ENV MEMCACHED_VERSION=1.6.10
# Fri, 06 Aug 2021 19:40:08 GMT
ENV MEMCACHED_SHA1=cb5b9fe77a2a59cc6cc7103a415bc07df9ddc6ec
# Fri, 06 Aug 2021 19:44:28 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Fri, 06 Aug 2021 19:44:28 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 06 Aug 2021 19:44:29 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 06 Aug 2021 19:44:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 06 Aug 2021 19:44:30 GMT
USER memcache
# Fri, 06 Aug 2021 19:44:30 GMT
EXPOSE 11211
# Fri, 06 Aug 2021 19:44:30 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:935703e1179e32e201e4a36d5664d58299dc8e7bcac197b70c295c0a59216db1`  
		Last Modified: Fri, 06 Aug 2021 17:39:15 GMT  
		Size: 2.8 MB (2821910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3997dcd952980827296aa49e7efcada10bcba749dd861df25f203d3f6b5e29fb`  
		Last Modified: Fri, 06 Aug 2021 19:45:55 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:363458a9ace96b06a1c58f2e8eb904dcaafcf96d9fc83364e89c15a69e1b044b`  
		Last Modified: Fri, 06 Aug 2021 19:45:55 GMT  
		Size: 169.0 KB (169023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8c1e47e1d8dffc3bf1ae4f7c79d5beac21f9680f97019bbc558fc087fa2524b`  
		Last Modified: Fri, 06 Aug 2021 19:45:56 GMT  
		Size: 944.5 KB (944463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28fc4379aa8294cba65c62b90c0316b066f29409ea1107f0b1af7e054de7d542`  
		Last Modified: Fri, 06 Aug 2021 19:45:55 GMT  
		Size: 283.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:859cc9f0c06e5a29acc2998ff62c7683221186e0d5ffa10de0196ba8740652bd`  
		Last Modified: Fri, 06 Aug 2021 19:45:55 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:alpine3.14` - linux; ppc64le

```console
$ docker pull memcached@sha256:96d6eb0b597ee6f99ea017c544da3a3da8c438a65f24577d69d903a613b42eb9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.0 MB (3953046 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a5afddb48ca7c5d1fffa75e492f5c852b1f92154ac06b71e83b340175e286f2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 30 Jul 2021 17:24:32 GMT
ADD file:0075aad7a94f0496483442bb2d9fdaa13e9c23087b90638d014b4bc263aa3861 in / 
# Fri, 30 Jul 2021 17:24:37 GMT
CMD ["/bin/sh"]
# Sat, 31 Jul 2021 02:00:19 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Sat, 31 Jul 2021 02:00:38 GMT
RUN apk add --no-cache libsasl
# Sat, 31 Jul 2021 02:00:41 GMT
ENV MEMCACHED_VERSION=1.6.10
# Sat, 31 Jul 2021 02:00:44 GMT
ENV MEMCACHED_SHA1=cb5b9fe77a2a59cc6cc7103a415bc07df9ddc6ec
# Sat, 31 Jul 2021 02:04:12 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Sat, 31 Jul 2021 02:04:14 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Sat, 31 Jul 2021 02:04:20 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Sat, 31 Jul 2021 02:04:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 31 Jul 2021 02:04:26 GMT
USER memcache
# Sat, 31 Jul 2021 02:04:29 GMT
EXPOSE 11211
# Sat, 31 Jul 2021 02:04:31 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:baf144cfb66ebe9df1969f3b90f1c448beff98edc84de1ccb5d6346195a070d4`  
		Last Modified: Tue, 15 Jun 2021 22:27:38 GMT  
		Size: 2.8 MB (2810478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98f63b81da11ee9893297c678d45b878b88bf1613542a902a234af006646f033`  
		Last Modified: Sat, 31 Jul 2021 02:05:23 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d285b5d5ee57cf8c3a3c677ad0aa80efe93a17e29603777fe0304d4c0e475f1`  
		Last Modified: Sat, 31 Jul 2021 02:05:24 GMT  
		Size: 179.6 KB (179648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:434627f38141f3056915a216098010ea26b8daedb59bd319797171e91de52257`  
		Last Modified: Sat, 31 Jul 2021 02:05:24 GMT  
		Size: 961.2 KB (961246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f003eac5ed43a42f901cfc8315162dadfecfcadc770156a1937dc7b88ab4a5c0`  
		Last Modified: Sat, 31 Jul 2021 02:05:23 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:136b49658cb22ccfc99bc66faf440d902d8634cbacf7d64c81795f64cdc3b72c`  
		Last Modified: Sat, 31 Jul 2021 02:05:23 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
