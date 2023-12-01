## `memcached:1-alpine3.18`

```console
$ docker pull memcached@sha256:93a9ff5ab97a213a027913f59bf902a118fa9750f88dbd4d513ebd920428820e
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 10
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown
	-	linux; 386
	-	unknown; unknown
	-	linux; ppc64le
	-	unknown; unknown
	-	linux; s390x
	-	unknown; unknown

### `memcached:1-alpine3.18` - linux; amd64

```console
$ docker pull memcached@sha256:f85dfa7d8ec9dc1b785c37ccf6dfa62bca5fec355c32ddf7957116376863284a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4471146 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f687f33554b696db4e2422b52d11bd36b20649d152ca63d20848c83b0679237f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 16 Oct 2023 06:54:12 GMT
ADD file:fc714080c3bcbbce7ac746a10d7b4355ffa36293a8d435d62cd5359ea8eb8364 in / 
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
	-	`sha256:c926b61bad3b94ae7351bafd0c184c159ebf0643b085f7ef1d47ecdc7316833c`  
		Last Modified: Thu, 30 Nov 2023 23:23:28 GMT  
		Size: 3.4 MB (3402422 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ce5e53c5eb3023b585266ac7ee39c0b268a83b4e16556b72f52bd67e39f596be`  
		Last Modified: Fri, 01 Dec 2023 00:14:01 GMT  
		Size: 1.2 KB (1243 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e958dac8143e41701702904f092ab10b8682434d3d88e5af758dafaeb3317428`  
		Last Modified: Fri, 01 Dec 2023 00:14:01 GMT  
		Size: 108.0 KB (107998 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:61dfbf83553658c4ab4a5ae4477150c88a3f30da8309b9cfefdc185b3764e501`  
		Last Modified: Fri, 01 Dec 2023 00:14:01 GMT  
		Size: 959.1 KB (959085 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8b397213e2806c5c7c6aca6c20bc2f69362c9f6204c5d3947eaaf870176d9a36`  
		Last Modified: Fri, 01 Dec 2023 00:14:01 GMT  
		Size: 277.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8c404d1dff37be469e83d35363176296e0129304273844e38a69edbd6861f08c`  
		Last Modified: Fri, 01 Dec 2023 00:14:02 GMT  
		Size: 121.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1-alpine3.18` - unknown; unknown

```console
$ docker pull memcached@sha256:6a508d9bd488a6e6f8bbaae93d8ff14548111b267a7440f64edec96b04f8a3cb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.0 KB (97008 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1fdbf48b2b61dd467eec02ffd7b0e996989023a93d9ecbc7a655a0755362c38a`

```dockerfile
```

-	Layers:
	-	`sha256:5c3e16fb5448bac47fadf2a80df72f13e831b463525dc9823da6c85f1770bf69`  
		Last Modified: Fri, 01 Dec 2023 00:14:01 GMT  
		Size: 78.1 KB (78055 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:1d5f7cf7dffd0d16953251b75fd8b7224aae91e57357d5af853c41398d72a5f7`  
		Last Modified: Fri, 01 Dec 2023 00:14:01 GMT  
		Size: 19.0 KB (18953 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:1-alpine3.18` - linux; arm64 variant v8

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

### `memcached:1-alpine3.18` - unknown; unknown

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

### `memcached:1-alpine3.18` - linux; 386

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

### `memcached:1-alpine3.18` - unknown; unknown

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

### `memcached:1-alpine3.18` - linux; ppc64le

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

### `memcached:1-alpine3.18` - unknown; unknown

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

### `memcached:1-alpine3.18` - linux; s390x

```console
$ docker pull memcached@sha256:7af81a585082ce3ca180a3fac82a30bb37a43973123841b2dec30e5d096be8cb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.3 MB (4285472 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b785f0d9bb74e0e2b4f8772ce85a7b23cfc2e2f8dbb7ad428517b68cca17de38`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 16 Oct 2023 06:54:12 GMT
ADD file:50d6643abf7df167a927decd69d193b980557ff73cca48dce86d57e2ff25ad45 in / 
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
	-	`sha256:2ea477e1c0c3db3337ee1d7c659f8c465021a65c036998ed3fa3b667d4b30153`  
		Last Modified: Thu, 30 Nov 2023 22:42:52 GMT  
		Size: 3.2 MB (3217454 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a7b34c58047c2f1ded65320321066565e57ddd2ed65156bde99267b8e575bf63`  
		Last Modified: Fri, 01 Dec 2023 11:03:57 GMT  
		Size: 1.2 KB (1244 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:036bb49faad29b98ef9de81de4441efa5208c00e72ccea2b631c7b1c283f072d`  
		Last Modified: Fri, 01 Dec 2023 11:03:57 GMT  
		Size: 112.8 KB (112781 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c1da6195feb453292bec9ae13a8968a7fbc7b611793ac2bc13df3614b514db3f`  
		Last Modified: Fri, 01 Dec 2023 11:03:57 GMT  
		Size: 953.6 KB (953590 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a43896e685e7c2e1e51c75c1ed262d1c57940abdc2e68d74301201c9aa8ebdfe`  
		Last Modified: Fri, 01 Dec 2023 11:03:57 GMT  
		Size: 281.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:928e080b9c3b24e2e655bd62e483670acb3c5508648e5a2784a6bebb4d252367`  
		Last Modified: Fri, 01 Dec 2023 11:03:57 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1-alpine3.18` - unknown; unknown

```console
$ docker pull memcached@sha256:89eda6fd40656e7c2d5de572e4bdfbd821a333eb1067170caf9074dcbc141515
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.2 KB (95207 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0e34e69a75d4acd1221e6dd87a6f96bcf43e52e6ebaba333e1e4cc57d391f048`

```dockerfile
```

-	Layers:
	-	`sha256:c5dd02fe5ddfbc8ce715e0e666a98ae24e73371a2a8dee859d796538f4cf0618`  
		Last Modified: Fri, 01 Dec 2023 11:03:57 GMT  
		Size: 76.4 KB (76419 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:13692e9f247d60b0cd5d0d4c0ccb23a86437ea348414e8548639ba89b5e4b65a`  
		Last Modified: Fri, 01 Dec 2023 11:03:57 GMT  
		Size: 18.8 KB (18788 bytes)  
		MIME: application/vnd.in-toto+json
