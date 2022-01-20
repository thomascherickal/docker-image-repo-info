## `memcached:1-alpine3.15`

```console
$ docker pull memcached@sha256:0ea4e4c78dae5cb4bae40fb59b1678518fe7c08a79e86fe09d20976774ffe0ca
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
$ docker pull memcached@sha256:45aaea7e7e89c491a9f0fd713744cadbce7257ed338162a05895a058b28de082
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.3 MB (5344497 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:efe813961a6861b4b7a9ea7a113bc963417ffa1d218b3028aee164ce53c8900e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 24 Nov 2021 20:19:40 GMT
ADD file:9233f6f2237d79659a9521f7e390df217cec49f1a8aa3a12147bbca1956acdb9 in / 
# Wed, 24 Nov 2021 20:19:40 GMT
CMD ["/bin/sh"]
# Tue, 30 Nov 2021 02:35:59 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 30 Nov 2021 02:36:00 GMT
RUN apk add --no-cache libsasl
# Thu, 20 Jan 2022 04:27:13 GMT
ENV MEMCACHED_VERSION=1.6.13
# Thu, 20 Jan 2022 04:27:14 GMT
ENV MEMCACHED_SHA1=b9da57ba63ba8de8a980fe0fe2fedc8d59e1dfe3
# Thu, 20 Jan 2022 04:31:19 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Thu, 20 Jan 2022 04:31:20 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 20 Jan 2022 04:31:20 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 20 Jan 2022 04:31:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 20 Jan 2022 04:31:21 GMT
USER memcache
# Thu, 20 Jan 2022 04:31:21 GMT
EXPOSE 11211
# Thu, 20 Jan 2022 04:31:21 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:59bf1c3509f33515622619af21ed55bbe26d24913cedbca106468a5fb37a50c3`  
		Last Modified: Wed, 24 Nov 2021 20:20:05 GMT  
		Size: 2.8 MB (2818413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58e98a684550967ddcb81865eb41c76d2cb28ce000c8ab6b2fdc45ecd6d58e9f`  
		Last Modified: Tue, 30 Nov 2021 02:40:45 GMT  
		Size: 1.3 KB (1263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23d22b3cd5df08fb1f3c02ad4eb2e296a0d9d544f8be06beafcfc78f524cb6f3`  
		Last Modified: Tue, 30 Nov 2021 02:40:46 GMT  
		Size: 109.2 KB (109231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5520c8636fcd7f3b4f65e599f18fb0cd29608586f99d5ad5cfafb3e8d6c988b7`  
		Last Modified: Thu, 20 Jan 2022 04:32:24 GMT  
		Size: 2.4 MB (2415189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1d7ac8482db5779d15c4232deaf8cef6513f6c42b4f9f45d5acb357fb2f150a`  
		Last Modified: Thu, 20 Jan 2022 04:32:23 GMT  
		Size: 280.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:254eba4ea9838039a5f78de55b5b162c932fc48bd728e47f058cbd6fa329aec4`  
		Last Modified: Thu, 20 Jan 2022 04:32:23 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-alpine3.15` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:1da06e0f3e93367ec6144dd3df82063dec8c3be28cf0a781f662d7415edb8798
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.1 MB (5108941 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc0f0dc92b6ce6e0ff9ffbd598fc5ab0547d1a67a2b5af6cd95028ad95b629d8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 24 Nov 2021 20:39:20 GMT
ADD file:df53811312284306901fdaaff0a357a4bf40d631e662fe9ce6d342442e494b6c in / 
# Wed, 24 Nov 2021 20:39:20 GMT
CMD ["/bin/sh"]
# Mon, 29 Nov 2021 23:43:46 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Mon, 29 Nov 2021 23:43:48 GMT
RUN apk add --no-cache libsasl
# Thu, 20 Jan 2022 02:13:57 GMT
ENV MEMCACHED_VERSION=1.6.13
# Thu, 20 Jan 2022 02:13:58 GMT
ENV MEMCACHED_SHA1=b9da57ba63ba8de8a980fe0fe2fedc8d59e1dfe3
# Thu, 20 Jan 2022 02:16:47 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Thu, 20 Jan 2022 02:16:49 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 20 Jan 2022 02:16:49 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 20 Jan 2022 02:16:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 20 Jan 2022 02:16:51 GMT
USER memcache
# Thu, 20 Jan 2022 02:16:52 GMT
EXPOSE 11211
# Thu, 20 Jan 2022 02:16:53 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:9b3977197b4f2147bdd31e1271f811319dcd5c2fc595f14e81f5351ab6275b99`  
		Last Modified: Wed, 24 Nov 2021 20:39:59 GMT  
		Size: 2.7 MB (2715434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85437b97d6aa5e8fbe9de8abde12cee8d795ff43b8a977cb44ef934f12adb97a`  
		Last Modified: Mon, 29 Nov 2021 23:47:33 GMT  
		Size: 1.2 KB (1239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:610cb0458a378225900aedc80ffe5fdb3529e46116bdb6bcaf8705f436662614`  
		Last Modified: Mon, 29 Nov 2021 23:47:33 GMT  
		Size: 110.5 KB (110518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f016a88e51eea50eb2bdfc623d6fcf941d3abdc9f8f5ff5b20a38b053c376911`  
		Last Modified: Thu, 20 Jan 2022 02:18:12 GMT  
		Size: 2.3 MB (2281344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7b8c0b82c8858cced64ed4f9d57cc7d793c0ce43fe5833395af2539f31f66c3`  
		Last Modified: Thu, 20 Jan 2022 02:18:12 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:223c2c58a797660c53ddc3040d6e5b221ddb54696687666a4ad7f8f90a54d411`  
		Last Modified: Thu, 20 Jan 2022 02:18:12 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-alpine3.15` - linux; 386

```console
$ docker pull memcached@sha256:2111fc4dc862d2d5d910d439d898ef5e5584352b07a90d1886899b5fccea1289
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.4 MB (5368403 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8bdaabe15d79293fbb24ea5d2eecd5b4c3b8ab1c2e8982e752673014d31ebd96`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 24 Nov 2021 20:53:48 GMT
ADD file:b9a17131c440053f2f67e127b447645f25fd7de2d6caca42f569cafab6291855 in / 
# Wed, 24 Nov 2021 20:53:48 GMT
CMD ["/bin/sh"]
# Mon, 29 Nov 2021 23:40:53 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Mon, 29 Nov 2021 23:40:56 GMT
RUN apk add --no-cache libsasl
# Wed, 19 Jan 2022 23:52:54 GMT
ENV MEMCACHED_VERSION=1.6.13
# Wed, 19 Jan 2022 23:52:54 GMT
ENV MEMCACHED_SHA1=b9da57ba63ba8de8a980fe0fe2fedc8d59e1dfe3
# Wed, 19 Jan 2022 23:57:17 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Wed, 19 Jan 2022 23:57:17 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 19 Jan 2022 23:57:18 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 19 Jan 2022 23:57:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 19 Jan 2022 23:57:19 GMT
USER memcache
# Wed, 19 Jan 2022 23:57:19 GMT
EXPOSE 11211
# Wed, 19 Jan 2022 23:57:19 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:e6889e0d66307a4b916fc844f2dcbc03245c63bc4189dd3e88126d9dcf2f9231`  
		Last Modified: Wed, 24 Nov 2021 20:54:48 GMT  
		Size: 2.8 MB (2827117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45678c3b8c90609de31d42f56e0b57b28ef7324488a92a85ffff4c8b2ffff25e`  
		Last Modified: Mon, 29 Nov 2021 23:46:14 GMT  
		Size: 1.3 KB (1264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b3c44e17e0b014b04185b89fc721767e22e1b37dea6cef3913d63ca876865be`  
		Last Modified: Mon, 29 Nov 2021 23:46:14 GMT  
		Size: 121.1 KB (121141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8da32227c4153d82d37de7e8cd38a0ae6cacd65300ae108269757e9dde9a0f13`  
		Last Modified: Wed, 19 Jan 2022 23:58:56 GMT  
		Size: 2.4 MB (2418478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c56d2b3d8702bb2e9953ebba68609cb15b42de20175c38bae6646291ad1f1c3`  
		Last Modified: Wed, 19 Jan 2022 23:58:55 GMT  
		Size: 282.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed2c3956890b946d2b3ce4e5152a456bc69c0a83eec1716ac9c3a2e00542b99c`  
		Last Modified: Wed, 19 Jan 2022 23:58:55 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-alpine3.15` - linux; ppc64le

```console
$ docker pull memcached@sha256:e0aa1c9737e6cc0b0521e95cecccc9467287388982fa494ad384cfbde542d55b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.3 MB (5314928 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12bf7bfbf2b5a76c9af264c3f5c73d720861d34eac88319f87dcfe70b6e6c7a2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 24 Nov 2021 20:20:16 GMT
ADD file:57115dca2eb707f46b6301e75174e6aa316fb02ac28643b91429b75be51bd8c8 in / 
# Wed, 24 Nov 2021 20:20:20 GMT
CMD ["/bin/sh"]
# Tue, 30 Nov 2021 00:52:13 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 30 Nov 2021 00:52:18 GMT
RUN apk add --no-cache libsasl
# Thu, 20 Jan 2022 01:12:57 GMT
ENV MEMCACHED_VERSION=1.6.13
# Thu, 20 Jan 2022 01:13:05 GMT
ENV MEMCACHED_SHA1=b9da57ba63ba8de8a980fe0fe2fedc8d59e1dfe3
# Thu, 20 Jan 2022 01:16:38 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Thu, 20 Jan 2022 01:16:40 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 20 Jan 2022 01:16:50 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 20 Jan 2022 01:16:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 20 Jan 2022 01:16:56 GMT
USER memcache
# Thu, 20 Jan 2022 01:16:59 GMT
EXPOSE 11211
# Thu, 20 Jan 2022 01:17:04 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:159b5dcb1717c815c76ff5ea1db730e18e8609c9090238e43282856db9e71f47`  
		Last Modified: Wed, 24 Nov 2021 20:21:14 GMT  
		Size: 2.8 MB (2814780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f44bb0dc5dc6d3634512266fffaecf643a467ef890e0a60fa7daed8a8f379335`  
		Last Modified: Tue, 30 Nov 2021 00:57:03 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:242bba95e896195e2c48210499ed8dad5c07a25a93e0d6304a787f4d5f05bb79`  
		Last Modified: Tue, 30 Nov 2021 00:57:03 GMT  
		Size: 126.2 KB (126210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40fc4b1c6bde43100e34393169d99f7e2e598601a96871f99abbda0193b560dd`  
		Last Modified: Thu, 20 Jan 2022 01:18:29 GMT  
		Size: 2.4 MB (2372268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3067762ac635b679c1a61965f852adcf293e95653354186ae56376d3c77b8dd`  
		Last Modified: Thu, 20 Jan 2022 01:18:29 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81be8693a1f907306cef503933931cf196ef06ebd32c055331c3b772e4439913`  
		Last Modified: Thu, 20 Jan 2022 01:18:29 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-alpine3.15` - linux; s390x

```console
$ docker pull memcached@sha256:93a0f06460ab24fccef83d2089b94fcbe5887cff9ba19e47a3ade8cb281063a6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4868874 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a617b9325daba394b7421b0591b96e7ebfc2a11838ac90f09bb428bf7943298`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 24 Nov 2021 20:41:23 GMT
ADD file:cd24c711a2ef431b3ff94f9a02bfc42f159bc60de1d0eceecafea4e8af02441d in / 
# Wed, 24 Nov 2021 20:41:23 GMT
CMD ["/bin/sh"]
# Mon, 29 Nov 2021 23:44:15 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Mon, 29 Nov 2021 23:44:16 GMT
RUN apk add --no-cache libsasl
# Thu, 20 Jan 2022 00:22:10 GMT
ENV MEMCACHED_VERSION=1.6.13
# Thu, 20 Jan 2022 00:22:10 GMT
ENV MEMCACHED_SHA1=b9da57ba63ba8de8a980fe0fe2fedc8d59e1dfe3
# Thu, 20 Jan 2022 00:25:45 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Thu, 20 Jan 2022 00:25:46 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 20 Jan 2022 00:25:46 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 20 Jan 2022 00:25:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 20 Jan 2022 00:25:46 GMT
USER memcache
# Thu, 20 Jan 2022 00:25:47 GMT
EXPOSE 11211
# Thu, 20 Jan 2022 00:25:47 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:d6baca485f3d0f7c77221be60fbef5db014a5ef9d8f53db4a310c947c690d189`  
		Last Modified: Wed, 24 Nov 2021 20:42:15 GMT  
		Size: 2.6 MB (2605944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6edeb1ae5f198c40517796be434eacf51803993a767a2c0fe96428c6d089fad2`  
		Last Modified: Mon, 29 Nov 2021 23:48:55 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93f301719e66b550caefc1f2adbf776d1d20ad42c288f855d16644987f9614c4`  
		Last Modified: Mon, 29 Nov 2021 23:48:54 GMT  
		Size: 113.7 KB (113741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de0ea222c47103e23f5a2f03e32b6c37844e634ccba3146b4067bba06eee6a25`  
		Last Modified: Thu, 20 Jan 2022 00:27:03 GMT  
		Size: 2.1 MB (2147516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b2227f160ee33a3ac2d5341b3edb61d1804cbc64cc7cbad34d023f97adfcc05`  
		Last Modified: Thu, 20 Jan 2022 00:27:03 GMT  
		Size: 283.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9947b575a9f8a861c03adf146e508aa692c7a520cf6aafe3d98f1bde0db5904f`  
		Last Modified: Thu, 20 Jan 2022 00:27:03 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
