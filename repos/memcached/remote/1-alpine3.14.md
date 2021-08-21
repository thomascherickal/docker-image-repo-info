## `memcached:1-alpine3.14`

```console
$ docker pull memcached@sha256:1cbe051d122223f218652bc34076cdf7ecd1981776afd69ed039943a028d5bbe
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `memcached:1-alpine3.14` - linux; amd64

```console
$ docker pull memcached@sha256:34b1ab627355edd9cceaa422b7b91e57caf007ae9b1a22922c38a08660e81efb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3903170 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:def8a42f3e88882c2265cc9e3f62e9e7681e163fe20a5f403d6fef77e8fb2111`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 06 Aug 2021 17:19:45 GMT
ADD file:34eb5c40aa00028921a224d1764ae1b1f3ef710d191e4dfc7df55e0594aa7217 in / 
# Fri, 06 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Sat, 07 Aug 2021 00:14:12 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Sat, 07 Aug 2021 00:14:13 GMT
RUN apk add --no-cache libsasl
# Sat, 07 Aug 2021 00:14:13 GMT
ENV MEMCACHED_VERSION=1.6.10
# Sat, 07 Aug 2021 00:14:14 GMT
ENV MEMCACHED_SHA1=cb5b9fe77a2a59cc6cc7103a415bc07df9ddc6ec
# Sat, 07 Aug 2021 00:18:04 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Sat, 07 Aug 2021 00:18:04 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Sat, 07 Aug 2021 00:18:05 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Sat, 07 Aug 2021 00:18:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 07 Aug 2021 00:18:05 GMT
USER memcache
# Sat, 07 Aug 2021 00:18:06 GMT
EXPOSE 11211
# Sat, 07 Aug 2021 00:18:06 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:29291e31a76a7e560b9b7ad3cada56e8c18d50a96cca8a2573e4f4689d7aca77`  
		Last Modified: Thu, 05 Aug 2021 15:56:25 GMT  
		Size: 2.8 MB (2813006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2aeb0b192a3f1081390d942a614d2b614c78be8c6728490b30f3abd0ea9b95a`  
		Last Modified: Sat, 07 Aug 2021 00:18:44 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4abbd93452bbb7ca5339028c20945da9101602ba49f9f42965452a3db6a98d2`  
		Last Modified: Sat, 07 Aug 2021 00:18:43 GMT  
		Size: 155.5 KB (155516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c472ac5a156e0c1551a6f99d1b657a6d495496b0cff418dffc1bbd630bd36640`  
		Last Modified: Sat, 07 Aug 2021 00:18:44 GMT  
		Size: 933.0 KB (932979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f4d28fec27cb7828cc4877db15d8023b453fef8d557721a6dc2c9f721c801bb`  
		Last Modified: Sat, 07 Aug 2021 00:18:43 GMT  
		Size: 280.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef85351ee7d962d3acc985da8128513818c7604be17e847251f543dfddf68747`  
		Last Modified: Sat, 07 Aug 2021 00:18:44 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-alpine3.14` - linux; arm64 variant v8

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

### `memcached:1-alpine3.14` - linux; 386

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

### `memcached:1-alpine3.14` - linux; ppc64le

```console
$ docker pull memcached@sha256:5ceda0e184a63631c255d5e5ff48c4c33d99af475ea06afcea6870e37fe19d68
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.0 MB (3953753 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:22db1888d17d2d29920e6a8042ccce4c79e4869f8c5f9c0c23487d8020f9740c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 06 Aug 2021 18:28:28 GMT
ADD file:40f3b617d7ff269d92f0ffcf8aad561b5f2c0626ef519a7f584f1ba0182b3188 in / 
# Fri, 06 Aug 2021 18:28:35 GMT
CMD ["/bin/sh"]
# Fri, 06 Aug 2021 21:46:01 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Fri, 06 Aug 2021 21:46:10 GMT
RUN apk add --no-cache libsasl
# Fri, 06 Aug 2021 21:46:13 GMT
ENV MEMCACHED_VERSION=1.6.10
# Fri, 06 Aug 2021 21:46:14 GMT
ENV MEMCACHED_SHA1=cb5b9fe77a2a59cc6cc7103a415bc07df9ddc6ec
# Fri, 06 Aug 2021 21:49:36 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Fri, 06 Aug 2021 21:49:40 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 06 Aug 2021 21:49:54 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 06 Aug 2021 21:50:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 06 Aug 2021 21:50:05 GMT
USER memcache
# Fri, 06 Aug 2021 21:50:08 GMT
EXPOSE 11211
# Fri, 06 Aug 2021 21:50:13 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:0ff902055236f70c4694c806877243e1dd52c513825a2a3ecc7eba8f5202acc8`  
		Last Modified: Fri, 06 Aug 2021 18:29:33 GMT  
		Size: 2.8 MB (2811152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a27a0115207f739cf0dadef89d1d4fa84ff382340ab5cfdc1a8c1d53fd2a4e1f`  
		Last Modified: Fri, 06 Aug 2021 21:51:17 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4535061ab98aeabde3c8815eda6ca7c387deddf01744a07f971c91fdbd402077`  
		Last Modified: Fri, 06 Aug 2021 21:51:17 GMT  
		Size: 179.7 KB (179663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c3c6a8fbed47687965665fabcb41ff9687a30f7a7ca112954c97c1c6e16cfbe`  
		Last Modified: Fri, 06 Aug 2021 21:51:18 GMT  
		Size: 961.3 KB (961265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95052d9a1041312d1404b4b4497de4ed9bf2db25a9b753d19b1a4b6d6d4f15b0`  
		Last Modified: Fri, 06 Aug 2021 21:51:17 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a9a71b75e165be41def41b7731961647b9f9b195ecb92da1d88139d5cf77400`  
		Last Modified: Fri, 06 Aug 2021 21:51:17 GMT  
		Size: 119.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-alpine3.14` - linux; s390x

```console
$ docker pull memcached@sha256:2b8100b8d620d079cd998a89b76bea1a8d09c103c189a44d21fead37c0856e8d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.7 MB (3694498 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:34f48a34f12e89ff7fe55fc05dde87a7890b58907e59352babfca3c6cd0894e5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 06 Aug 2021 17:41:30 GMT
ADD file:bdf19d63e9f8600d2fbe02435279b8df06fbcb5105e6b8eea778d8ef928e219a in / 
# Fri, 06 Aug 2021 17:41:31 GMT
CMD ["/bin/sh"]
# Fri, 06 Aug 2021 18:37:51 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Fri, 06 Aug 2021 18:37:54 GMT
RUN apk add --no-cache libsasl
# Fri, 06 Aug 2021 18:37:54 GMT
ENV MEMCACHED_VERSION=1.6.10
# Fri, 06 Aug 2021 18:37:55 GMT
ENV MEMCACHED_SHA1=cb5b9fe77a2a59cc6cc7103a415bc07df9ddc6ec
# Sat, 21 Aug 2021 04:21:17 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Sat, 21 Aug 2021 04:21:17 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Sat, 21 Aug 2021 04:21:19 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Sat, 21 Aug 2021 04:21:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 21 Aug 2021 04:21:20 GMT
USER memcache
# Sat, 21 Aug 2021 04:21:21 GMT
EXPOSE 11211
# Sat, 21 Aug 2021 04:21:21 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:625f57562315453466f73bc9d8c96e678f8d4ea436b462d06c60fb217c6b3d38`  
		Last Modified: Fri, 06 Aug 2021 17:42:42 GMT  
		Size: 2.6 MB (2602036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8513cb540b3898142480b7e3f85e101504bedfab70d831bc480ae422c1c4cec`  
		Last Modified: Sat, 21 Aug 2021 04:22:19 GMT  
		Size: 1.3 KB (1273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20b8ec45ae3b80d748a851ee4c35837c0d45a769eae205c2f327f8d972ca1c51`  
		Last Modified: Sat, 21 Aug 2021 04:22:19 GMT  
		Size: 161.5 KB (161520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07f94c751b2bc6e37c5aa93aa9a3368e647b2615995a51839b0d07093f67a0a9`  
		Last Modified: Sat, 21 Aug 2021 04:22:19 GMT  
		Size: 929.3 KB (929267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2cdd1bd2136509036d1d793b3b78b3ce1a1bc88fb6ca809a063ab3fb97f266c`  
		Last Modified: Sat, 21 Aug 2021 04:22:19 GMT  
		Size: 282.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1fa99c20d4ebd3829f028f299ebac31184910b640fc0600af7bbaaba591d291`  
		Last Modified: Sat, 21 Aug 2021 04:22:19 GMT  
		Size: 120.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
