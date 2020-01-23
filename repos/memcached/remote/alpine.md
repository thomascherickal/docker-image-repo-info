## `memcached:alpine`

```console
$ docker pull memcached@sha256:a5937f7b44e7482c6119fe53e8b6ed62241e222f5ef92407a9085ca16742b396
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

### `memcached:alpine` - linux; amd64

```console
$ docker pull memcached@sha256:1dc4a9848a8ef2ce8bcda27195b4260842261851339133af9cfec4ce2f446b6a
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.3 MB (4312917 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:db5a019f09c89500e1c1178ba0c7bffc42eb3ea1cfdf241aa5eb80deae5e6e55`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:06 GMT
ADD file:d48cac34fac385cbc1de6adfdd88300f76f9bbe346cd17e64fd834d042a98326 in / 
# Thu, 23 Jan 2020 16:53:06 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 19:11:21 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Thu, 23 Jan 2020 19:11:23 GMT
RUN apk add --no-cache cyrus-sasl-plain
# Thu, 23 Jan 2020 19:11:23 GMT
ENV MEMCACHED_VERSION=1.5.20
# Thu, 23 Jan 2020 19:11:24 GMT
ENV MEMCACHED_SHA1=5d3b5af3ce0a1483d655017db7228bcaeff10d47
# Thu, 23 Jan 2020 19:18:40 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		dpkg-dev dpkg 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		perl 		perl-utils 		tar 		wget 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		$enableExtstore 	&& make -j "$(nproc)" 		&& make test 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Thu, 23 Jan 2020 19:18:40 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 23 Jan 2020 19:18:42 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 23 Jan 2020 19:18:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jan 2020 19:18:42 GMT
USER memcache
# Thu, 23 Jan 2020 19:18:42 GMT
EXPOSE 11211
# Thu, 23 Jan 2020 19:18:43 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:4167d3e149762ea326c26fc2fd4e36fdeb7d4e639408ad30f37b8f25ac285a98`  
		Last Modified: Thu, 23 Jan 2020 16:53:38 GMT  
		Size: 2.8 MB (2786962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d70e805cca1266f0102445b9abfb72281fd7c8511c737094dbbf1060dd9d3f37`  
		Last Modified: Thu, 23 Jan 2020 19:19:05 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80235597fc5084dad91b7ea206762a3615b13e218ca5f096a189b93defd5cf56`  
		Last Modified: Thu, 23 Jan 2020 19:19:04 GMT  
		Size: 14.9 KB (14882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10944b1d14c85ae2782c671b52e41901dcf6f4c964cd9288f1b8a634cf64d132`  
		Last Modified: Thu, 23 Jan 2020 19:19:05 GMT  
		Size: 1.5 MB (1509409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b783201c596796bf2b2ddc01898270fda609a7cd40a43a613b1733fbc07e0db`  
		Last Modified: Thu, 23 Jan 2020 19:19:05 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f07aedd291b20381acaf1b4c57f16e69b0b7974731e7942d3c92bfd66618723d`  
		Last Modified: Thu, 23 Jan 2020 19:19:05 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:alpine` - linux; arm variant v6

```console
$ docker pull memcached@sha256:4b7d6ae6affda2a8765f3d08012fbebb09056beb557816e1593074a2cee8ac39
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.0 MB (4038421 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b67b64a291e407fdc800f2d5f865f101c8b2a0edf8d9f03934be9d88def29e76`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:27 GMT
ADD file:2aa80d52585a6b34b2cc5811d46965a084e50cfb8cd183f1a88b2b1bc6556e1f in / 
# Thu, 23 Jan 2020 16:53:28 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 17:36:09 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Thu, 23 Jan 2020 17:36:13 GMT
RUN apk add --no-cache cyrus-sasl-plain
# Thu, 23 Jan 2020 17:36:14 GMT
ENV MEMCACHED_VERSION=1.5.20
# Thu, 23 Jan 2020 17:36:15 GMT
ENV MEMCACHED_SHA1=5d3b5af3ce0a1483d655017db7228bcaeff10d47
# Thu, 23 Jan 2020 17:43:23 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		dpkg-dev dpkg 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		perl 		perl-utils 		tar 		wget 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		$enableExtstore 	&& make -j "$(nproc)" 		&& make test 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Thu, 23 Jan 2020 17:43:23 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 23 Jan 2020 17:43:25 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 23 Jan 2020 17:43:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jan 2020 17:43:28 GMT
USER memcache
# Thu, 23 Jan 2020 17:43:30 GMT
EXPOSE 11211
# Thu, 23 Jan 2020 17:43:32 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:896868b7b9168cabb308702db96dc9769d10c23e20fc66f5f4abedf4c75d7642`  
		Last Modified: Thu, 23 Jan 2020 16:54:07 GMT  
		Size: 2.6 MB (2571407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0016ca6f71d72de8181825fafd5fc8c130297c9130e03a68d49ea87666023feb`  
		Last Modified: Thu, 23 Jan 2020 17:43:47 GMT  
		Size: 1.3 KB (1287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75a4c61e47c6f6c54760cc3bc80a3453f4a77a4894c00c24bc068c0362ff9571`  
		Last Modified: Thu, 23 Jan 2020 17:43:48 GMT  
		Size: 14.3 KB (14307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d142a799e3da288eeaf51b60fbe80636bf07f0e65490caf2e76cd0d897ce63b`  
		Last Modified: Thu, 23 Jan 2020 17:43:48 GMT  
		Size: 1.5 MB (1451013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1e4e919fc441eb10a50f635dfa518d156c09523b456ccfeed120af7a6ca8de8`  
		Last Modified: Thu, 23 Jan 2020 17:43:47 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14e662c928fd49ff098317bd949bed8a03767b788db382db30acf1ee80a464bb`  
		Last Modified: Thu, 23 Jan 2020 17:43:47 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:alpine` - linux; arm variant v7

```console
$ docker pull memcached@sha256:1f0f9606bbedde685a9bb3015a51730dab2c79d79acbaff889d2023f7211fbc0
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.7 MB (3727611 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6fe782d950cd9746d363389bf920998d54d3d0caec88cfbec9d4a58a3b249b9b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:31 GMT
ADD file:d05c9f9143d11d12045d4faef882e5985e6b38fabe52237dd8d8c0627a9620ab in / 
# Thu, 23 Jan 2020 16:53:32 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 18:23:23 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Thu, 23 Jan 2020 18:23:35 GMT
RUN apk add --no-cache cyrus-sasl-plain
# Thu, 23 Jan 2020 18:23:37 GMT
ENV MEMCACHED_VERSION=1.5.20
# Thu, 23 Jan 2020 18:23:38 GMT
ENV MEMCACHED_SHA1=5d3b5af3ce0a1483d655017db7228bcaeff10d47
# Thu, 23 Jan 2020 18:44:44 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		dpkg-dev dpkg 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		perl 		perl-utils 		tar 		wget 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		$enableExtstore 	&& make -j "$(nproc)" 		&& make test 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Thu, 23 Jan 2020 18:44:47 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 23 Jan 2020 18:44:57 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 23 Jan 2020 18:44:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jan 2020 18:45:01 GMT
USER memcache
# Thu, 23 Jan 2020 18:45:02 GMT
EXPOSE 11211
# Thu, 23 Jan 2020 18:45:04 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:4e972d957a606327b0b6c2e8aa4a6045c263b7496a536298aaebf690e9d85f1d`  
		Last Modified: Thu, 23 Jan 2020 16:53:59 GMT  
		Size: 2.4 MB (2378408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa6cfe185e17c674b07c4413b3af85fd1516f2a1b3741dc4f05d817df0cf37a5`  
		Last Modified: Thu, 23 Jan 2020 18:45:21 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aabcb51cee3a5ae8fab585c387282e5dac87d1d5698d7279cd51d6ddd10de89c`  
		Last Modified: Thu, 23 Jan 2020 18:45:22 GMT  
		Size: 13.3 KB (13283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6e11241e9ee34472d307ca81ed019f8482f22cf47bcdfb49fa9731649706123`  
		Last Modified: Thu, 23 Jan 2020 18:45:23 GMT  
		Size: 1.3 MB (1334226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ef609f9ccf15362253e69a47be20f3977a86321b71d23f72d1e24184cb6d408`  
		Last Modified: Thu, 23 Jan 2020 18:45:21 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1c40fa43125c972832cff52d6f8fadf7d3645df5ce687aa4ce4e58d34636414`  
		Last Modified: Thu, 23 Jan 2020 18:45:21 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:alpine` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:24a6f0728bf090a3d1d4f1f6b2a8da70897d63db0cfdeb44cdd86758d7285b4a
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.3 MB (4253972 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:62faabf32bbdb8dfc131820daeada2f150c8e0f5242574fdb2db8082994a8f6f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 23 Jan 2020 16:54:39 GMT
ADD file:bdfbd4b0dfb53eecc80bac65894d1e2fcfafb27dcf24ab019176e2c9f60b9a39 in / 
# Thu, 23 Jan 2020 16:54:40 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 18:39:04 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Thu, 23 Jan 2020 18:39:06 GMT
RUN apk add --no-cache cyrus-sasl-plain
# Thu, 23 Jan 2020 18:39:07 GMT
ENV MEMCACHED_VERSION=1.5.20
# Thu, 23 Jan 2020 18:39:08 GMT
ENV MEMCACHED_SHA1=5d3b5af3ce0a1483d655017db7228bcaeff10d47
# Thu, 23 Jan 2020 18:46:14 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		dpkg-dev dpkg 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		perl 		perl-utils 		tar 		wget 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		$enableExtstore 	&& make -j "$(nproc)" 		&& make test 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Thu, 23 Jan 2020 18:46:15 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 23 Jan 2020 18:46:17 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 23 Jan 2020 18:46:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jan 2020 18:46:19 GMT
USER memcache
# Thu, 23 Jan 2020 18:46:20 GMT
EXPOSE 11211
# Thu, 23 Jan 2020 18:46:21 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:f07e4bcf42b862c240f4c00f2f7ed362d7d93ca15151de547beda593f3b669e5`  
		Last Modified: Thu, 23 Jan 2020 16:55:24 GMT  
		Size: 2.7 MB (2717732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d61751473a1cb9d5e41c5e57aceda7327f2c87f8b814d1b23c2a12b6a2eb779`  
		Last Modified: Thu, 23 Jan 2020 18:46:45 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f96dcafabf06ed1c02437db55c35b57e18e62e408b41fe0c320f707ccc10c1e`  
		Last Modified: Thu, 23 Jan 2020 18:46:45 GMT  
		Size: 15.3 KB (15274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:427f16509575639fd99e3457b3f270294fb3a5a05cc3ca9c58d1e1d8138cb26c`  
		Last Modified: Thu, 23 Jan 2020 18:46:45 GMT  
		Size: 1.5 MB (1519273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe88beae8063f208af6846a03ae36e46c77b2aa72713837c62aa600b8ce4b91f`  
		Last Modified: Thu, 23 Jan 2020 18:46:45 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:944ca239de741aa6075ea4e9357f6fba7a66bc20c15bce9c785bf99e932ff9c2`  
		Last Modified: Thu, 23 Jan 2020 18:46:45 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:alpine` - linux; 386

```console
$ docker pull memcached@sha256:c5304b7332d3a2c29969b1311d020c0401d99b6468cd410ddee441335f6f9c56
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.4 MB (4402344 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ab510dfc97246e10896a8500449f831aa14e03c5c563f85c2ad6942511f26a0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 23 Jan 2020 16:52:57 GMT
ADD file:8c429ecc11f3cadcecc39922ce15df6b51a649929959b331fed8d1f42d722474 in / 
# Thu, 23 Jan 2020 16:52:57 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 22:18:25 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Thu, 23 Jan 2020 22:18:26 GMT
RUN apk add --no-cache cyrus-sasl-plain
# Thu, 23 Jan 2020 22:18:26 GMT
ENV MEMCACHED_VERSION=1.5.20
# Thu, 23 Jan 2020 22:18:26 GMT
ENV MEMCACHED_SHA1=5d3b5af3ce0a1483d655017db7228bcaeff10d47
# Thu, 23 Jan 2020 22:25:18 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		dpkg-dev dpkg 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		perl 		perl-utils 		tar 		wget 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		$enableExtstore 	&& make -j "$(nproc)" 		&& make test 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Thu, 23 Jan 2020 22:25:19 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 23 Jan 2020 22:25:19 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 23 Jan 2020 22:25:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jan 2020 22:25:20 GMT
USER memcache
# Thu, 23 Jan 2020 22:25:20 GMT
EXPOSE 11211
# Thu, 23 Jan 2020 22:25:20 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:8ad089020f8a1fd366fb13feb183e2f4c7410e2232c54b40f6a54fd56029fdf3`  
		Last Modified: Thu, 23 Jan 2020 16:53:22 GMT  
		Size: 2.8 MB (2785861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e131112a4c8c1a866269b2c02d546723b0ccf763704c3ee1450203982f70cbc`  
		Last Modified: Thu, 23 Jan 2020 22:25:33 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cab81fee01fb587f87b8c64ae2020375fc081ad036f3640c97891d9c20f5ba71`  
		Last Modified: Thu, 23 Jan 2020 22:25:34 GMT  
		Size: 15.8 KB (15813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddb0b89433f5851fd2f06cfe5153a638bb1f3814aa811d406145caa0bf57d444`  
		Last Modified: Thu, 23 Jan 2020 22:25:34 GMT  
		Size: 1.6 MB (1599003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ccb90b617bc0554f432a82fc027d807e6e66e591af106ac62dc0f197bbda365`  
		Last Modified: Thu, 23 Jan 2020 22:25:33 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8018f589bf367cf0fc7d8c6e0edf8f19822a99a3adc2a3ab82ce96befe324419`  
		Last Modified: Thu, 23 Jan 2020 22:25:33 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:alpine` - linux; ppc64le

```console
$ docker pull memcached@sha256:3ea2b35bdca9a73665201773bc7d230941ffbb925aa3ca70f66069bc7ec18a5b
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.4 MB (4400237 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b49c26609a3321fdae45e998bd06efd2494936758d0105ad918f996960d8ed68`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 21 Oct 2019 17:52:55 GMT
ADD file:11a2dd0058b1642e9ee52239d03223819a53ca346fd42826eead7729c50e1257 in / 
# Mon, 21 Oct 2019 17:53:00 GMT
CMD ["/bin/sh"]
# Mon, 21 Oct 2019 20:28:14 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Mon, 21 Oct 2019 20:28:19 GMT
RUN apk add --no-cache cyrus-sasl-plain
# Tue, 12 Nov 2019 02:21:07 GMT
ENV MEMCACHED_VERSION=1.5.20
# Tue, 12 Nov 2019 02:21:09 GMT
ENV MEMCACHED_SHA1=5d3b5af3ce0a1483d655017db7228bcaeff10d47
# Tue, 12 Nov 2019 02:27:51 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		dpkg-dev dpkg 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		perl 		perl-utils 		tar 		wget 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		$enableExtstore 	&& make -j "$(nproc)" 		&& make test 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 12 Nov 2019 02:27:53 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 12 Nov 2019 02:28:04 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 12 Nov 2019 02:28:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 12 Nov 2019 02:28:13 GMT
USER memcache
# Tue, 12 Nov 2019 02:28:16 GMT
EXPOSE 11211
# Tue, 12 Nov 2019 02:28:19 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:cd18d16ea896a0f0eb99be52a9722ffae9a5ac35cf28cb8b96f589352f8e71d6`  
		Last Modified: Mon, 21 Oct 2019 17:53:53 GMT  
		Size: 2.8 MB (2808504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7589e894157e5de27750310c1871a8c27ce249498629ae858f8df572066fd99e`  
		Last Modified: Mon, 21 Oct 2019 20:42:44 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da22c020bd7716dc80265f5fac6b0be6aede0348e0853f656d4c6be212809dc3`  
		Last Modified: Mon, 21 Oct 2019 20:42:44 GMT  
		Size: 15.9 KB (15940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b5d29d373cad33ef0fa7e90b8fac9fbdc7f057630d9baad8073182138523988`  
		Last Modified: Tue, 12 Nov 2019 02:28:59 GMT  
		Size: 1.6 MB (1574099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a36ec207c782863a2d376f70c24f3e65a6cd268512e965e949ba9c3b91c2e7b`  
		Last Modified: Tue, 12 Nov 2019 02:28:58 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ac6ea8950bc427c7159c0cff6d82068b020ee2bad76da606fb8c482a62e7f86`  
		Last Modified: Tue, 12 Nov 2019 02:28:58 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:alpine` - linux; s390x

```console
$ docker pull memcached@sha256:7295e677896a531ce8e2f171fde31f721618611720d4c911132736dbc45fa4d3
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.1 MB (4052728 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:04146b145e02520ac8848fd057a913852fd6ea8abc933fec317b7fc06010838d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 23 Jan 2020 16:52:43 GMT
ADD file:922e12714922ae035a33d6ceb8d2683ad3e454deca21ad02b699db908443342b in / 
# Thu, 23 Jan 2020 16:52:44 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 17:24:51 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Thu, 23 Jan 2020 17:24:52 GMT
RUN apk add --no-cache cyrus-sasl-plain
# Thu, 23 Jan 2020 17:24:52 GMT
ENV MEMCACHED_VERSION=1.5.20
# Thu, 23 Jan 2020 17:24:52 GMT
ENV MEMCACHED_SHA1=5d3b5af3ce0a1483d655017db7228bcaeff10d47
# Thu, 23 Jan 2020 17:28:28 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		dpkg-dev dpkg 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		perl 		perl-utils 		tar 		wget 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		$enableExtstore 	&& make -j "$(nproc)" 		&& make test 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Thu, 23 Jan 2020 17:28:28 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 23 Jan 2020 17:28:29 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 23 Jan 2020 17:28:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jan 2020 17:28:29 GMT
USER memcache
# Thu, 23 Jan 2020 17:28:29 GMT
EXPOSE 11211
# Thu, 23 Jan 2020 17:28:29 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:0449d076b2977b7e7ce4c35b0fe5199d86cabaf453e869da73b2efb66d6282dd`  
		Last Modified: Thu, 23 Jan 2020 16:53:07 GMT  
		Size: 2.6 MB (2573620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fe38d0bfb4cf690c35f5cad20f2b3852cf3e3feae187d049660d61066d34266`  
		Last Modified: Thu, 23 Jan 2020 17:28:43 GMT  
		Size: 1.3 KB (1263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e7b0be037aec2a267ac29fa65d5d2944abe8469008d0642de65630db833c613`  
		Last Modified: Thu, 23 Jan 2020 17:28:43 GMT  
		Size: 15.1 KB (15133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:721302a401eba2bc95563c39d70c6ceb2622f40852963b48a63b9436ac729b35`  
		Last Modified: Thu, 23 Jan 2020 17:28:43 GMT  
		Size: 1.5 MB (1462308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0a3a38346255281bbb2fe4efbc071d94d6322906bce537bbfb2c901d054f30d`  
		Last Modified: Thu, 23 Jan 2020 17:28:43 GMT  
		Size: 283.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb3309d80a3f4f5007acb79f3c9791f4d35a740e7d64bc8a859f0781987c9e51`  
		Last Modified: Thu, 23 Jan 2020 17:28:43 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
