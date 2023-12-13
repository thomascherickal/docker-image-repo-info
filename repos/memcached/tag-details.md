<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `memcached`

-	[`memcached:1`](#memcached1)
-	[`memcached:1-alpine`](#memcached1-alpine)
-	[`memcached:1-alpine3.19`](#memcached1-alpine319)
-	[`memcached:1-bookworm`](#memcached1-bookworm)
-	[`memcached:1.6`](#memcached16)
-	[`memcached:1.6-alpine`](#memcached16-alpine)
-	[`memcached:1.6-alpine3.19`](#memcached16-alpine319)
-	[`memcached:1.6-bookworm`](#memcached16-bookworm)
-	[`memcached:1.6.22`](#memcached1622)
-	[`memcached:1.6.22-alpine`](#memcached1622-alpine)
-	[`memcached:1.6.22-alpine3.19`](#memcached1622-alpine319)
-	[`memcached:1.6.22-bookworm`](#memcached1622-bookworm)
-	[`memcached:alpine`](#memcachedalpine)
-	[`memcached:alpine3.19`](#memcachedalpine319)
-	[`memcached:bookworm`](#memcachedbookworm)
-	[`memcached:latest`](#memcachedlatest)

## `memcached:1`

```console
$ docker pull memcached@sha256:c0aa354cc777aa9bdbaf3789db81b1b1802be11940498801dbe1562999d5671e
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 15
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm variant v5
	-	unknown; unknown
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	unknown; unknown
	-	linux; 386
	-	unknown; unknown
	-	linux; mips64le
	-	unknown; unknown
	-	linux; ppc64le
	-	unknown; unknown
	-	linux; s390x
	-	unknown; unknown

### `memcached:1` - linux; amd64

```console
$ docker pull memcached@sha256:0d358fa0198562aa3d1e1c3e9386e1835256875517d8a4786f3dd50a1f65f1de
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.1 MB (41125606 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:03bad2c21b5df5c82f8c581ebec403482a3e00c0f35697ca669c46a7d000a13d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 21 Nov 2023 05:21:37 GMT
ADD file:d261a6f6921593f1e0b3f472ab1b1822e2c6deb0b369200f0b3370556bfad017 in / 
# Tue, 21 Nov 2023 05:21:37 GMT
CMD ["bash"]
# Mon, 04 Dec 2023 18:08:47 GMT
RUN set -eux; 	groupadd --system --gid 11211 memcache; 	useradd --system --gid memcache --uid 11211 memcache # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
ENV MEMCACHED_VERSION=1.6.22
# Mon, 04 Dec 2023 18:08:47 GMT
ENV MEMCACHED_URL=https://memcached.org/files/memcached-1.6.22.tar.gz
# Mon, 04 Dec 2023 18:08:47 GMT
ENV MEMCACHED_SHA1=7a691f390d59616dbebfc9e2e4942d499c39a338
# Mon, 04 Dec 2023 18:08:47 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O memcached.tar.gz "$MEMCACHED_URL"; 	echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c -; 	mkdir -p /usr/src/memcached; 	tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1; 	rm memcached.tar.gz; 		cd /usr/src/memcached; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	; 	nproc="$(nproc)"; 	make -j "$nproc"; 		sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf; 	make test PARALLEL="$nproc"; 	mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf; 		make install; 		cd /; 	rm -rf /usr/src/memcached; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		memcached -V # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 04 Dec 2023 18:08:47 GMT
USER memcache
# Mon, 04 Dec 2023 18:08:47 GMT
EXPOSE map[11211/tcp:{}]
# Mon, 04 Dec 2023 18:08:47 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:1f7ce2fa46ab3942feabee654933948821303a5a821789dddab2d8c3df59e227`  
		Last Modified: Tue, 21 Nov 2023 05:25:58 GMT  
		Size: 29.1 MB (29149908 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:21ac6fd160890cbc46a76542eb3f68654f3e3fb043b1b28a18155ec6863d60bc`  
		Last Modified: Tue, 12 Dec 2023 20:52:57 GMT  
		Size: 1.1 KB (1112 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6330fc82e1304befcc27a7598cd1a85152985d06426f94966788bf5a1583dcc6`  
		Last Modified: Tue, 12 Dec 2023 20:52:57 GMT  
		Size: 2.5 MB (2488284 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4047c827380f04698fbc51155441d719f93b84c1a092d633260c704f286296dd`  
		Last Modified: Tue, 12 Dec 2023 20:52:57 GMT  
		Size: 9.5 MB (9485895 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:401b5de2a4f8d9f588888754fa8347b67590c776363770f46ef67688116a4a0c`  
		Last Modified: Tue, 12 Dec 2023 20:52:57 GMT  
		Size: 285.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ee899f9aed95096580ea4a2325fd4824518ff1621f433f393fa253b52b7294b5`  
		Last Modified: Tue, 12 Dec 2023 20:52:58 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1` - unknown; unknown

```console
$ docker pull memcached@sha256:5ccb88c1a86bd6524b6d5c9383254cdd79314d656a0c982658ecd35d9716431b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 MB (3077929 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:238ef9023561adc9c09faf875c5370cb2711a83cc7327dcc49ae7f8255c23794`

```dockerfile
```

-	Layers:
	-	`sha256:f84a6f3d0bdab8613be68ff091a6a78bedf8f697d4df55ff90ac7b745337e72c`  
		Last Modified: Tue, 12 Dec 2023 20:52:57 GMT  
		Size: 3.1 MB (3056812 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:8d7aee053ab87a86e42ba3d14810d3f1918c6e66d4d3ef02bc9c741f3948b83e`  
		Last Modified: Tue, 12 Dec 2023 20:52:57 GMT  
		Size: 21.1 KB (21117 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:1` - linux; arm variant v5

```console
$ docker pull memcached@sha256:cb9426984b18b2d3df1c5fbb2bb7e2e9ebe08325d4adce6d0cd7a9207c413476
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.1 MB (37113170 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a8f2fb6119b629983f190d8b73208a156991d8cb65c47579a68125c339e9c75`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 21 Nov 2023 05:00:51 GMT
ADD file:1ae8e5ac45b11d01083680b765e1fcfef9f7938f89d6f424572126fa946d8cdf in / 
# Tue, 21 Nov 2023 05:00:52 GMT
CMD ["bash"]
# Mon, 04 Dec 2023 18:08:47 GMT
RUN set -eux; 	groupadd --system --gid 11211 memcache; 	useradd --system --gid memcache --uid 11211 memcache # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
ENV MEMCACHED_VERSION=1.6.22
# Mon, 04 Dec 2023 18:08:47 GMT
ENV MEMCACHED_URL=https://memcached.org/files/memcached-1.6.22.tar.gz
# Mon, 04 Dec 2023 18:08:47 GMT
ENV MEMCACHED_SHA1=7a691f390d59616dbebfc9e2e4942d499c39a338
# Mon, 04 Dec 2023 18:08:47 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O memcached.tar.gz "$MEMCACHED_URL"; 	echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c -; 	mkdir -p /usr/src/memcached; 	tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1; 	rm memcached.tar.gz; 		cd /usr/src/memcached; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	; 	nproc="$(nproc)"; 	make -j "$nproc"; 		sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf; 	make test PARALLEL="$nproc"; 	mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf; 		make install; 		cd /; 	rm -rf /usr/src/memcached; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		memcached -V # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 04 Dec 2023 18:08:47 GMT
USER memcache
# Mon, 04 Dec 2023 18:08:47 GMT
EXPOSE map[11211/tcp:{}]
# Mon, 04 Dec 2023 18:08:47 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:f476aef5b6e1122850e68c81ef06fc2df17e968961b060483b4d2fb33018aae3`  
		Last Modified: Tue, 21 Nov 2023 05:03:55 GMT  
		Size: 26.9 MB (26922153 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:89367ca16d2c3104d44514e1b9b94b0ac4070ea0f6f04523c72dda62795f3a17`  
		Last Modified: Tue, 12 Dec 2023 21:47:13 GMT  
		Size: 1.1 KB (1110 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5ecbc6577cf78c09bd4136f78a57a904ae1ab705fce8595e8d1187d800158e6f`  
		Last Modified: Tue, 12 Dec 2023 21:47:14 GMT  
		Size: 2.1 MB (2089289 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:12f8a270079b04e1372c73cc16ff2ae33e6f6ee0dcc7e8ed57843fca20b3d038`  
		Last Modified: Tue, 12 Dec 2023 21:47:14 GMT  
		Size: 8.1 MB (8100211 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5f592556023f9ba6125ecf6b89156ba61c05526ad324708c3d2a09600ee5e7e4`  
		Last Modified: Tue, 12 Dec 2023 21:47:14 GMT  
		Size: 285.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fa757a09f6a7a23114a13869f15b229384628cf108567d395dc0d4730c685409`  
		Last Modified: Tue, 12 Dec 2023 21:47:14 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1` - unknown; unknown

```console
$ docker pull memcached@sha256:0c93e2660a508733f1c7d5236af77ef81fbcd0b27e4ac55c81d83334c8794891
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.0 KB (21043 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:538fbf714aa2f8a4175400dd43b0715e416f73fe598fc50d3f763afa144595da`

```dockerfile
```

-	Layers:
	-	`sha256:f65b3a9a0f6936cae3c1e411ecdd846d754a1978d851fdacf4b25526cb9ff4cc`  
		Last Modified: Tue, 12 Dec 2023 21:47:14 GMT  
		Size: 21.0 KB (21043 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:1` - linux; arm variant v7

```console
$ docker pull memcached@sha256:2841be0a36134563966c09a6ed68b21053d20342ec8736cf92763c28077ead43
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.1 MB (28094215 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6cf74ffa940dd93988fc0beb6698c5796563c82a40b7dd668153969f64d2e6ca`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 09 Feb 2023 06:12:09 GMT
ADD file:5f1a343224e8486690bd90dd1e50c8d84b3d770c51bb6829544e5cf650c0419c in / 
# Thu, 09 Feb 2023 06:12:10 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 07:52:31 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Thu, 09 Feb 2023 07:52:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 07:52:35 GMT
ENV MEMCACHED_VERSION=1.6.18
# Thu, 09 Feb 2023 07:52:35 GMT
ENV MEMCACHED_SHA1=be16909bb75ab972ee5fe438312501de01c4725a
# Thu, 09 Feb 2023 07:55:44 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 09 Feb 2023 07:55:44 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 09 Feb 2023 07:55:44 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 09 Feb 2023 07:55:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 09 Feb 2023 07:55:44 GMT
USER memcache
# Thu, 09 Feb 2023 07:55:45 GMT
EXPOSE 11211
# Thu, 09 Feb 2023 07:55:45 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:e7318f6106ad75d7d482ae9dddf4d927b0872ef3ddb6e1330aa691fc8d17279e`  
		Last Modified: Thu, 09 Feb 2023 06:19:19 GMT  
		Size: 26.6 MB (26577666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de49d9d72daf1680b5f1b9532dd2eb0162829f36c8db9669935462636fbf99d9`  
		Last Modified: Thu, 09 Feb 2023 08:06:11 GMT  
		Size: 4.9 KB (4895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0beac9d5bcac946f8c54c72b8a9c136914b1aa7a5fe2b8c3df4c7d8858ea6559`  
		Last Modified: Thu, 09 Feb 2023 08:06:11 GMT  
		Size: 312.1 KB (312088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4c9e5a265394e4c0f357779e6195a4e82d767a3691a0e77d427e56651c3e54a`  
		Last Modified: Thu, 09 Feb 2023 08:06:11 GMT  
		Size: 1.2 MB (1199163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5ea82ad892fe1ae8623d84e32c8c027087cda8aa49e40d4546ed6942e471c60`  
		Last Modified: Thu, 09 Feb 2023 08:06:11 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa2ae3bcdc0d114ba49a67df022b6f7215fc87f1f50e64939fcfbbec4eaadee5`  
		Last Modified: Thu, 09 Feb 2023 08:06:11 GMT  
		Size: 118.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:c5adc5a4207d95c96a36131c2d39085b082f0e22f4595b935e72bcb463c10383
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.0 MB (39979924 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf26c17403ed5a4db96ddd8b41aeb2fd45483f897882a57972c994c95a44c5dd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 21 Nov 2023 06:27:06 GMT
ADD file:869c7d0747a17c53715581a2e862992eb8516c7f45f167821dfa80966a4870d1 in / 
# Tue, 21 Nov 2023 06:27:06 GMT
CMD ["bash"]
# Mon, 04 Dec 2023 18:08:47 GMT
RUN set -eux; 	groupadd --system --gid 11211 memcache; 	useradd --system --gid memcache --uid 11211 memcache # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
ENV MEMCACHED_VERSION=1.6.22
# Mon, 04 Dec 2023 18:08:47 GMT
ENV MEMCACHED_URL=https://memcached.org/files/memcached-1.6.22.tar.gz
# Mon, 04 Dec 2023 18:08:47 GMT
ENV MEMCACHED_SHA1=7a691f390d59616dbebfc9e2e4942d499c39a338
# Mon, 04 Dec 2023 18:08:47 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O memcached.tar.gz "$MEMCACHED_URL"; 	echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c -; 	mkdir -p /usr/src/memcached; 	tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1; 	rm memcached.tar.gz; 		cd /usr/src/memcached; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	; 	nproc="$(nproc)"; 	make -j "$nproc"; 		sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf; 	make test PARALLEL="$nproc"; 	mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf; 		make install; 		cd /; 	rm -rf /usr/src/memcached; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		memcached -V # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 04 Dec 2023 18:08:47 GMT
USER memcache
# Mon, 04 Dec 2023 18:08:47 GMT
EXPOSE map[11211/tcp:{}]
# Mon, 04 Dec 2023 18:08:47 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:2c6d21737d8318aa15c4cc838475029a5efc36c0429e3d8da80d97d0b96d9aaf`  
		Last Modified: Tue, 21 Nov 2023 06:30:30 GMT  
		Size: 29.2 MB (29179277 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1a39d6fec0d552a8078ab223bafd58bc9a0c8c27c26600a5b95c6a521bb97f3d`  
		Last Modified: Tue, 12 Dec 2023 23:43:17 GMT  
		Size: 1.1 KB (1112 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9d1ceea69964553dd3aaf853e0d7b753495cab4623b9377c69096be0bdf88146`  
		Last Modified: Tue, 12 Dec 2023 23:43:17 GMT  
		Size: 2.3 MB (2345975 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:52063b8e37cbc1e5e6e3af0f54b834ae3f6a53d023349ae819c9607e5fc98aec`  
		Last Modified: Tue, 12 Dec 2023 23:43:17 GMT  
		Size: 8.5 MB (8453155 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5b99d0095a64f8110efee1f5e91754cc923294d50c9e2927e515354746a3f465`  
		Last Modified: Tue, 12 Dec 2023 23:43:17 GMT  
		Size: 284.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:913c9e21eaa9c49c99b1b39e5cda0ef12356220075c869ea4776dca36fe83b75`  
		Last Modified: Tue, 12 Dec 2023 23:43:18 GMT  
		Size: 121.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1` - unknown; unknown

```console
$ docker pull memcached@sha256:3d519a2eb9e00b43e6bc7584f6962b12ba032c4487a6e4ef7fd2b00b667bc90d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 MB (3053138 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9cc25288d58197dcc1309ea4a8128d0b120b92ad2d877f226095cd4847696474`

```dockerfile
```

-	Layers:
	-	`sha256:c5edc5ba98b4e6a438caa0d4541784c5c1e8b23d6020bc0b2a5b9910d0725400`  
		Last Modified: Tue, 12 Dec 2023 23:43:17 GMT  
		Size: 3.0 MB (3032003 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:b15e35765293b6f1da0e628c94108f229423c5a6379b8b5c47a41415f377b6d8`  
		Last Modified: Tue, 12 Dec 2023 23:43:17 GMT  
		Size: 21.1 KB (21135 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:1` - linux; 386

```console
$ docker pull memcached@sha256:fa9dba8086765d68f2feecfc2ac08fb29c019597d09943bb480227e6cba87666
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.3 MB (39294993 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:93047050e75b6d4d64adb8a7c8f68cb118bad27ca9dc772120e251b174752cf9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 16 Oct 2023 06:54:12 GMT
ADD file:0c94521fdd9c0a4fdeeb9aad23e68cd053fba0dcd7c3af550aefa79377816e31 in / 
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["bash"]
# Mon, 16 Oct 2023 06:54:12 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_VERSION=1.6.22
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_SHA1=7a691f390d59616dbebfc9e2e4942d499c39a338
# Mon, 16 Oct 2023 06:54:12 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V # buildkit
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
	-	`sha256:98bdfce9af831c2a0d0bfcca812d0039cd1666986550f552b4b4c625bd5aa31c`  
		Last Modified: Wed, 01 Nov 2023 00:43:26 GMT  
		Size: 30.2 MB (30164042 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1b647d4b10cf20ac5807101c7d0380701be684aa82f5c01ec41f674b5ef23d42`  
		Last Modified: Wed, 01 Nov 2023 01:06:49 GMT  
		Size: 1.1 KB (1109 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b61c058003459de4911c2901b2d799b03de754a1b9e64ffbe21a04992e962e62`  
		Last Modified: Wed, 01 Nov 2023 01:06:49 GMT  
		Size: 2.5 MB (2492501 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:810b6db64df2fcc8f76941cdac75093cf35bd72ac3cd1fa5eb664e74c1f67cd8`  
		Last Modified: Wed, 01 Nov 2023 01:06:50 GMT  
		Size: 6.6 MB (6636937 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:dbb899942df4149bd5fae8bac6e295285ec80f82d621f2b29c931ee348491cfb`  
		Last Modified: Wed, 01 Nov 2023 01:06:49 GMT  
		Size: 282.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4a8530160ab232c37c0ddcbf5e3a731d835d378d1382843957f6c2a73b2b5be6`  
		Last Modified: Wed, 01 Nov 2023 01:06:50 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1` - unknown; unknown

```console
$ docker pull memcached@sha256:dd7ce9519c31365127142232df2ed0b285e9acc03cd77c23c838bf932165def8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.5 KB (21498 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eef82c92e07c11a92c337806d01cfb1c6cdc7a16608dcf304a38de34d2ef1dbb`

```dockerfile
```

-	Layers:
	-	`sha256:c0d9dd22513f8d3e791e1796d7ef1906e57c798c92dd35d0be9cf2eaecec5954`  
		Last Modified: Wed, 01 Nov 2023 01:06:49 GMT  
		Size: 21.5 KB (21498 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:1` - linux; mips64le

```console
$ docker pull memcached@sha256:9f7696d5078cf83e8b152cb00a3615576fd3c50d10be9253b9c188e16bfd8087
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.9 MB (39863164 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:685886644cfb343923260c15c66eb8c8d8bf7b84b6b1e855732aec2359b6ae29`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 21 Nov 2023 04:09:50 GMT
ADD file:e093749192323dc72b60a8440ddba26c415586f618b5e107fa264ba5eb2ca7ba in / 
# Tue, 21 Nov 2023 04:09:54 GMT
CMD ["bash"]
# Mon, 04 Dec 2023 18:08:47 GMT
RUN set -eux; 	groupadd --system --gid 11211 memcache; 	useradd --system --gid memcache --uid 11211 memcache # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
ENV MEMCACHED_VERSION=1.6.22
# Mon, 04 Dec 2023 18:08:47 GMT
ENV MEMCACHED_URL=https://memcached.org/files/memcached-1.6.22.tar.gz
# Mon, 04 Dec 2023 18:08:47 GMT
ENV MEMCACHED_SHA1=7a691f390d59616dbebfc9e2e4942d499c39a338
# Mon, 04 Dec 2023 18:08:47 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O memcached.tar.gz "$MEMCACHED_URL"; 	echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c -; 	mkdir -p /usr/src/memcached; 	tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1; 	rm memcached.tar.gz; 		cd /usr/src/memcached; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	; 	nproc="$(nproc)"; 	make -j "$nproc"; 		sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf; 	make test PARALLEL="$nproc"; 	mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf; 		make install; 		cd /; 	rm -rf /usr/src/memcached; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		memcached -V # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 04 Dec 2023 18:08:47 GMT
USER memcache
# Mon, 04 Dec 2023 18:08:47 GMT
EXPOSE map[11211/tcp:{}]
# Mon, 04 Dec 2023 18:08:47 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:ebdff2138fee4a3ec27560ab1353dc51c12c2608ff721f5db3d24104872b702a`  
		Last Modified: Tue, 21 Nov 2023 04:20:35 GMT  
		Size: 29.1 MB (29141984 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ee63ae82c6a87dc28cedafb91fbd6eaccd22add5b00a9cceb208472b30427b5d`  
		Last Modified: Tue, 12 Dec 2023 23:10:03 GMT  
		Size: 1.1 KB (1114 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3d430991f88102b07bcf8bf22f07667e49c9dfedb134b0ac36ddbb99d1e79db2`  
		Last Modified: Tue, 12 Dec 2023 23:10:04 GMT  
		Size: 1.9 MB (1937475 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ebe1140b392e915b8757b8d0a4b83f0aaf2103734e9f83c318821f641207b6b4`  
		Last Modified: Tue, 12 Dec 2023 23:10:04 GMT  
		Size: 8.8 MB (8782185 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:aedf1130e49a6aa7d9b74b9fd00914b171966fcf8beba71095787811fa3a0284`  
		Last Modified: Tue, 12 Dec 2023 23:10:03 GMT  
		Size: 284.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:457e2691e0499a1a1d26e6da85567f20a8dc396bde9d9952ce75fdcfe6cbafd8`  
		Last Modified: Tue, 12 Dec 2023 23:10:05 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1` - unknown; unknown

```console
$ docker pull memcached@sha256:d48752667ff111ef73342ae5c16218a373275e8b65c7696eff231ff49ca7b8e5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.0 KB (21004 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9138b1207d88c6ca6b32a2616d3c25b1f5d3280b7650ac4bfa7120518f6a8ad7`

```dockerfile
```

-	Layers:
	-	`sha256:2b1c5f3190ac8dfdff54a51d9421ad623af991deba1a46ba943cf88442079207`  
		Last Modified: Tue, 12 Dec 2023 23:10:03 GMT  
		Size: 21.0 KB (21004 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:1` - linux; ppc64le

```console
$ docker pull memcached@sha256:813f2ed7d8d4d2c4e6f4a19816964b0c95cc56d038d95d059571d51e115ab109
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.5 MB (45508655 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:73c79988c4d09a9ac9cb01aa05096b344821e8034c3cba04afb9cb78fe25db05`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 21 Nov 2023 04:24:14 GMT
ADD file:8b22a531b6611a1e63dfc20e4e2931592e2d821bd4b64c4b2810bb9a36640c02 in / 
# Tue, 21 Nov 2023 04:24:16 GMT
CMD ["bash"]
# Mon, 04 Dec 2023 18:08:47 GMT
RUN set -eux; 	groupadd --system --gid 11211 memcache; 	useradd --system --gid memcache --uid 11211 memcache # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
ENV MEMCACHED_VERSION=1.6.22
# Mon, 04 Dec 2023 18:08:47 GMT
ENV MEMCACHED_URL=https://memcached.org/files/memcached-1.6.22.tar.gz
# Mon, 04 Dec 2023 18:08:47 GMT
ENV MEMCACHED_SHA1=7a691f390d59616dbebfc9e2e4942d499c39a338
# Mon, 04 Dec 2023 18:08:47 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O memcached.tar.gz "$MEMCACHED_URL"; 	echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c -; 	mkdir -p /usr/src/memcached; 	tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1; 	rm memcached.tar.gz; 		cd /usr/src/memcached; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	; 	nproc="$(nproc)"; 	make -j "$nproc"; 		sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf; 	make test PARALLEL="$nproc"; 	mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf; 		make install; 		cd /; 	rm -rf /usr/src/memcached; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		memcached -V # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 04 Dec 2023 18:08:47 GMT
USER memcache
# Mon, 04 Dec 2023 18:08:47 GMT
EXPOSE map[11211/tcp:{}]
# Mon, 04 Dec 2023 18:08:47 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:c570d04e61d8e35a3c8f12179d048d701451f97f9cf2099ea3e3738512dbf062`  
		Last Modified: Tue, 21 Nov 2023 04:28:58 GMT  
		Size: 33.1 MB (33141607 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b53469d03d0156e89526c2b744f6850b65cfb9b509a6fda4c523764f7a9f9072`  
		Last Modified: Tue, 12 Dec 2023 23:08:09 GMT  
		Size: 1.1 KB (1111 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:12b61a5974195d80345022ed47cb4546f6fec60527b3932b2ce74d605db750e0`  
		Last Modified: Tue, 12 Dec 2023 23:08:09 GMT  
		Size: 2.7 MB (2698202 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:108f5df7a0010e4f69929c6ce4ff2e0e53877c6bbe11bd86acbbb0e7b608dca7`  
		Last Modified: Tue, 12 Dec 2023 23:08:09 GMT  
		Size: 9.7 MB (9667330 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:aa53d1e0a6b1123a31838e581de8d738ccaf05c9be569ec50b8d37cbc54a99bd`  
		Last Modified: Tue, 12 Dec 2023 23:08:08 GMT  
		Size: 283.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2cf8ef0b438a2029bfc9b928364eb71966baa4990e2ac4a9b1648cbd44271dc4`  
		Last Modified: Tue, 12 Dec 2023 23:08:10 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1` - unknown; unknown

```console
$ docker pull memcached@sha256:d75efc7b8726fbfade0b41c14205058def09ee997a7befb495808c2752a56a54
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 MB (3066416 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ca8bb0be2316bb58a60c953382dd1963eb7e265d0602de370e02152e1ac84d7`

```dockerfile
```

-	Layers:
	-	`sha256:34203b346608565cdbcd7cf9a56efb8ec2255b1a8f30267d6b2749d6a0bd2d6b`  
		Last Modified: Tue, 12 Dec 2023 23:08:09 GMT  
		Size: 3.0 MB (3045398 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:4da4f2a55f1773bfac75983e2e733c609b970884e935de987ec5b3ec5c92eb85`  
		Last Modified: Tue, 12 Dec 2023 23:08:08 GMT  
		Size: 21.0 KB (21018 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:1` - linux; s390x

```console
$ docker pull memcached@sha256:05084fffc798db32442e2cde93eac5815ffd909e9bf65692ac08c9b5ab79e677
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.0 MB (38041790 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eac80baab625f3daf940cdb3053e2e709bd61d78d7eae50b7db4d71f87bcd149`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 21 Nov 2023 05:04:35 GMT
ADD file:c33fa9fdde73983850798b6eb1cd062e0398109d1d773e6a937fead7475c8efc in / 
# Tue, 21 Nov 2023 05:04:41 GMT
CMD ["bash"]
# Mon, 04 Dec 2023 18:08:47 GMT
RUN set -eux; 	groupadd --system --gid 11211 memcache; 	useradd --system --gid memcache --uid 11211 memcache # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
ENV MEMCACHED_VERSION=1.6.22
# Mon, 04 Dec 2023 18:08:47 GMT
ENV MEMCACHED_URL=https://memcached.org/files/memcached-1.6.22.tar.gz
# Mon, 04 Dec 2023 18:08:47 GMT
ENV MEMCACHED_SHA1=7a691f390d59616dbebfc9e2e4942d499c39a338
# Mon, 04 Dec 2023 18:08:47 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O memcached.tar.gz "$MEMCACHED_URL"; 	echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c -; 	mkdir -p /usr/src/memcached; 	tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1; 	rm memcached.tar.gz; 		cd /usr/src/memcached; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	; 	nproc="$(nproc)"; 	make -j "$nproc"; 		sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf; 	make test PARALLEL="$nproc"; 	mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf; 		make install; 		cd /; 	rm -rf /usr/src/memcached; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		memcached -V # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 04 Dec 2023 18:08:47 GMT
USER memcache
# Mon, 04 Dec 2023 18:08:47 GMT
EXPOSE map[11211/tcp:{}]
# Mon, 04 Dec 2023 18:08:47 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:6daa625e5a040476e253e7acd0befa74254a4865ec836d6334a544d82a21d4be`  
		Last Modified: Tue, 21 Nov 2023 05:10:21 GMT  
		Size: 27.5 MB (27512885 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b19a3143cbec7ddc9a646dbbe779b0b5ec67662cf70e280db146f6ace54ccd61`  
		Last Modified: Wed, 13 Dec 2023 00:26:35 GMT  
		Size: 1.1 KB (1111 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b8af028b1fa76aa55f540dd5be5eaf89eea3fec23e09e9a88550aac36e9ee843`  
		Last Modified: Wed, 13 Dec 2023 00:26:35 GMT  
		Size: 2.2 MB (2152508 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9a774943469875a0902c53fccdd95cad9c18234b759bcdcc5816bd563deb7f14`  
		Last Modified: Wed, 13 Dec 2023 00:26:35 GMT  
		Size: 8.4 MB (8374880 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:266b4bf499a815da6f7ddcf68e1e61f8418c8ec655a2083e174aaa385de74d76`  
		Last Modified: Wed, 13 Dec 2023 00:26:35 GMT  
		Size: 284.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0da709e3482cc552b0a7b69eb05aaa21af1e74baaf4e3bccc34e95e478943630`  
		Last Modified: Wed, 13 Dec 2023 00:26:36 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1` - unknown; unknown

```console
$ docker pull memcached@sha256:525abad348ba03c5b9444f23409d647581284c1642d30539e2c9943405266f12
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 MB (3067303 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e3b551ec9122d039520bbd13bced5b1f5b0d5b1fd9e32c09a1d4536f7af1226`

```dockerfile
```

-	Layers:
	-	`sha256:5cc0958f61715f0746d9fa2a8a5c06f31608bb5d1cf32d606c46fc8e11b35984`  
		Last Modified: Wed, 13 Dec 2023 00:26:35 GMT  
		Size: 3.0 MB (3046353 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:3d2fed99d3355e42a820c1975105411eb7584cffb111d7e1fd541603f7721f1c`  
		Last Modified: Wed, 13 Dec 2023 00:26:35 GMT  
		Size: 20.9 KB (20950 bytes)  
		MIME: application/vnd.in-toto+json

## `memcached:1-alpine`

```console
$ docker pull memcached@sha256:9587ad270892c531bf1ac66f195312c2f0f374192e5ac79cf2dfc5dd7cd1555e
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
$ docker pull memcached@sha256:286df72d3172b8ed7793e7058f9327823d65bdac8a226a06a00d292c087ad9c2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.4 MB (4419383 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d682c07630240a305e61d9fe0b12e4dc6f338f6a6b2c95b0941b54b2b8509b75`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 08 Dec 2023 01:39:30 GMT
ADD file:8182c73f869a899cf624a59c400acb8226776d15e4d3a0d240a94e65340540d0 in / 
# Fri, 08 Dec 2023 01:39:30 GMT
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
	-	`sha256:c303524923177661067f7eb378c3dd5277088c2676ebd1cd78e68397bb80fdbf`  
		Last Modified: Fri, 08 Dec 2023 01:39:48 GMT  
		Size: 3.3 MB (3347794 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:dfede01b081f27465377bdafbbdb6b694c6fab18026972b2c380535dcef103b8`  
		Last Modified: Wed, 13 Dec 2023 01:35:47 GMT  
		Size: 1.2 KB (1246 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b6d7b6f4ad45bf3aee58c5a7e8083286bd79dc004840903fd5997929772bfb4c`  
		Last Modified: Wed, 13 Dec 2023 01:35:47 GMT  
		Size: 120.9 KB (120897 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:64a4d385fe9c52ce74fd893218a806a70ac60ff0c57a80c1b3e43096c1f9ebc0`  
		Last Modified: Wed, 13 Dec 2023 01:35:48 GMT  
		Size: 949.0 KB (949044 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fd5239ae2cadceed6ddca34da081735d9a9d40ec7e5bdded8b5faca81fb0a070`  
		Last Modified: Wed, 13 Dec 2023 01:35:48 GMT  
		Size: 282.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4ab0568624eca639b58ae572fcf8e82d6fb6cb3d9f6ca5d7df2b7329747dedd4`  
		Last Modified: Wed, 13 Dec 2023 01:35:49 GMT  
		Size: 120.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1-alpine` - unknown; unknown

```console
$ docker pull memcached@sha256:6f8a1e61dcc0fd492cbafc5fd2b4c22d6154464b462857003e8e48a48305823a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **98.1 KB (98108 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ffc7ff6f7a07bd49a0241faf0b1957add37ce71b17cbdf2c878e4fc78cdc7bc4`

```dockerfile
```

-	Layers:
	-	`sha256:a9702aa1523d9e76bf98e50205b92ccf5d5bee944388fa4b376abeae8048c7d5`  
		Last Modified: Wed, 13 Dec 2023 01:35:48 GMT  
		Size: 78.6 KB (78622 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:3a49d198124cd7443d92b69a3737a232e2d6e7c626eb726c2902193c31acd5bd`  
		Last Modified: Wed, 13 Dec 2023 01:35:47 GMT  
		Size: 19.5 KB (19486 bytes)  
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
$ docker pull memcached@sha256:06711fbe2ddda329f14ab4a0825494b32336140e6a0e3b6c4d879adc475857c3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4468374 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09b1d12275d18bb3dac772e05585652308aa081f1aeae540381aea1c9ed321bd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 08 Dec 2023 01:22:51 GMT
ADD file:052421189f8d269382daaaa8beb63c687e4d8ca908c421abdce53bcc627a40b4 in / 
# Fri, 08 Dec 2023 01:22:51 GMT
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
	-	`sha256:243ac51c334a47917a84be93e972ee6378987e9b3b917a5a8df29025e161c1f3`  
		Last Modified: Fri, 08 Dec 2023 01:23:14 GMT  
		Size: 3.4 MB (3358233 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:add73e7dbebd6c86078686bb046ef57017b090fe917f656feb83ec0ef971b5f3`  
		Last Modified: Tue, 12 Dec 2023 23:20:17 GMT  
		Size: 1.2 KB (1243 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d64bed657a7e728633e13f2021b35954e98be9ecae77096d30cdaa1d9260d61e`  
		Last Modified: Tue, 12 Dec 2023 23:20:17 GMT  
		Size: 123.4 KB (123403 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1b7a39c0f73f39f740b607f200570edf13046db40879e4aebbdca9e2fd273b0f`  
		Last Modified: Tue, 12 Dec 2023 23:20:17 GMT  
		Size: 985.1 KB (985092 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ad6306836cf70172b90d6b82bffc8546c005c16cda9b7d58dc5dbd386b7ee7d8`  
		Last Modified: Tue, 12 Dec 2023 23:20:17 GMT  
		Size: 281.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:71e3eb1fb10d08825521650c7c7ddedf3cfce2f976e93c18ab11aace23c38be5`  
		Last Modified: Tue, 12 Dec 2023 23:20:18 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1-alpine` - unknown; unknown

```console
$ docker pull memcached@sha256:65ba466bf93c49f07fd340ced359d51a13a74b069cca4de2d034d12f42b92ea4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **96.4 KB (96395 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0e68093b9e036b2a9ff696038b0fd906f66504c0a0cd70dda18954ebb93d4bd1`

```dockerfile
```

-	Layers:
	-	`sha256:b64631288cf2d05d3a1d99eb8cb41f077724b027aaf136bb327f88055e4ceaf4`  
		Last Modified: Tue, 12 Dec 2023 23:20:17 GMT  
		Size: 77.0 KB (77025 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:8ac9ea640f8ca624c147fd0dcc40f859a6284e5f50c4396e0b1e962a4b732813`  
		Last Modified: Tue, 12 Dec 2023 23:20:17 GMT  
		Size: 19.4 KB (19370 bytes)  
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

## `memcached:1-alpine3.19`

```console
$ docker pull memcached@sha256:fc05162ae59e353d64bc065f589df156b875b48ac0d9c6bab788e9a2a2e400ca
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 8
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown
	-	linux; ppc64le
	-	unknown; unknown
	-	linux; s390x
	-	unknown; unknown

### `memcached:1-alpine3.19` - linux; amd64

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

### `memcached:1-alpine3.19` - unknown; unknown

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

### `memcached:1-alpine3.19` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:286df72d3172b8ed7793e7058f9327823d65bdac8a226a06a00d292c087ad9c2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.4 MB (4419383 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d682c07630240a305e61d9fe0b12e4dc6f338f6a6b2c95b0941b54b2b8509b75`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 08 Dec 2023 01:39:30 GMT
ADD file:8182c73f869a899cf624a59c400acb8226776d15e4d3a0d240a94e65340540d0 in / 
# Fri, 08 Dec 2023 01:39:30 GMT
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
	-	`sha256:c303524923177661067f7eb378c3dd5277088c2676ebd1cd78e68397bb80fdbf`  
		Last Modified: Fri, 08 Dec 2023 01:39:48 GMT  
		Size: 3.3 MB (3347794 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:dfede01b081f27465377bdafbbdb6b694c6fab18026972b2c380535dcef103b8`  
		Last Modified: Wed, 13 Dec 2023 01:35:47 GMT  
		Size: 1.2 KB (1246 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b6d7b6f4ad45bf3aee58c5a7e8083286bd79dc004840903fd5997929772bfb4c`  
		Last Modified: Wed, 13 Dec 2023 01:35:47 GMT  
		Size: 120.9 KB (120897 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:64a4d385fe9c52ce74fd893218a806a70ac60ff0c57a80c1b3e43096c1f9ebc0`  
		Last Modified: Wed, 13 Dec 2023 01:35:48 GMT  
		Size: 949.0 KB (949044 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fd5239ae2cadceed6ddca34da081735d9a9d40ec7e5bdded8b5faca81fb0a070`  
		Last Modified: Wed, 13 Dec 2023 01:35:48 GMT  
		Size: 282.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4ab0568624eca639b58ae572fcf8e82d6fb6cb3d9f6ca5d7df2b7329747dedd4`  
		Last Modified: Wed, 13 Dec 2023 01:35:49 GMT  
		Size: 120.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1-alpine3.19` - unknown; unknown

```console
$ docker pull memcached@sha256:6f8a1e61dcc0fd492cbafc5fd2b4c22d6154464b462857003e8e48a48305823a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **98.1 KB (98108 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ffc7ff6f7a07bd49a0241faf0b1957add37ce71b17cbdf2c878e4fc78cdc7bc4`

```dockerfile
```

-	Layers:
	-	`sha256:a9702aa1523d9e76bf98e50205b92ccf5d5bee944388fa4b376abeae8048c7d5`  
		Last Modified: Wed, 13 Dec 2023 01:35:48 GMT  
		Size: 78.6 KB (78622 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:3a49d198124cd7443d92b69a3737a232e2d6e7c626eb726c2902193c31acd5bd`  
		Last Modified: Wed, 13 Dec 2023 01:35:47 GMT  
		Size: 19.5 KB (19486 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:1-alpine3.19` - linux; ppc64le

```console
$ docker pull memcached@sha256:06711fbe2ddda329f14ab4a0825494b32336140e6a0e3b6c4d879adc475857c3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4468374 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09b1d12275d18bb3dac772e05585652308aa081f1aeae540381aea1c9ed321bd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 08 Dec 2023 01:22:51 GMT
ADD file:052421189f8d269382daaaa8beb63c687e4d8ca908c421abdce53bcc627a40b4 in / 
# Fri, 08 Dec 2023 01:22:51 GMT
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
	-	`sha256:243ac51c334a47917a84be93e972ee6378987e9b3b917a5a8df29025e161c1f3`  
		Last Modified: Fri, 08 Dec 2023 01:23:14 GMT  
		Size: 3.4 MB (3358233 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:add73e7dbebd6c86078686bb046ef57017b090fe917f656feb83ec0ef971b5f3`  
		Last Modified: Tue, 12 Dec 2023 23:20:17 GMT  
		Size: 1.2 KB (1243 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d64bed657a7e728633e13f2021b35954e98be9ecae77096d30cdaa1d9260d61e`  
		Last Modified: Tue, 12 Dec 2023 23:20:17 GMT  
		Size: 123.4 KB (123403 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1b7a39c0f73f39f740b607f200570edf13046db40879e4aebbdca9e2fd273b0f`  
		Last Modified: Tue, 12 Dec 2023 23:20:17 GMT  
		Size: 985.1 KB (985092 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ad6306836cf70172b90d6b82bffc8546c005c16cda9b7d58dc5dbd386b7ee7d8`  
		Last Modified: Tue, 12 Dec 2023 23:20:17 GMT  
		Size: 281.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:71e3eb1fb10d08825521650c7c7ddedf3cfce2f976e93c18ab11aace23c38be5`  
		Last Modified: Tue, 12 Dec 2023 23:20:18 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1-alpine3.19` - unknown; unknown

```console
$ docker pull memcached@sha256:65ba466bf93c49f07fd340ced359d51a13a74b069cca4de2d034d12f42b92ea4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **96.4 KB (96395 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0e68093b9e036b2a9ff696038b0fd906f66504c0a0cd70dda18954ebb93d4bd1`

```dockerfile
```

-	Layers:
	-	`sha256:b64631288cf2d05d3a1d99eb8cb41f077724b027aaf136bb327f88055e4ceaf4`  
		Last Modified: Tue, 12 Dec 2023 23:20:17 GMT  
		Size: 77.0 KB (77025 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:8ac9ea640f8ca624c147fd0dcc40f859a6284e5f50c4396e0b1e962a4b732813`  
		Last Modified: Tue, 12 Dec 2023 23:20:17 GMT  
		Size: 19.4 KB (19370 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:1-alpine3.19` - linux; s390x

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

### `memcached:1-alpine3.19` - unknown; unknown

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

## `memcached:1-bookworm`

```console
$ docker pull memcached@sha256:5006d1a9ea8a2cedd728d75c2e85cb26c96489f6a039d14ba2c44f99ea310d1c
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 14
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm variant v5
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown
	-	linux; 386
	-	unknown; unknown
	-	linux; mips64le
	-	unknown; unknown
	-	linux; ppc64le
	-	unknown; unknown
	-	linux; s390x
	-	unknown; unknown

### `memcached:1-bookworm` - linux; amd64

```console
$ docker pull memcached@sha256:0d358fa0198562aa3d1e1c3e9386e1835256875517d8a4786f3dd50a1f65f1de
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.1 MB (41125606 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:03bad2c21b5df5c82f8c581ebec403482a3e00c0f35697ca669c46a7d000a13d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 21 Nov 2023 05:21:37 GMT
ADD file:d261a6f6921593f1e0b3f472ab1b1822e2c6deb0b369200f0b3370556bfad017 in / 
# Tue, 21 Nov 2023 05:21:37 GMT
CMD ["bash"]
# Mon, 04 Dec 2023 18:08:47 GMT
RUN set -eux; 	groupadd --system --gid 11211 memcache; 	useradd --system --gid memcache --uid 11211 memcache # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
ENV MEMCACHED_VERSION=1.6.22
# Mon, 04 Dec 2023 18:08:47 GMT
ENV MEMCACHED_URL=https://memcached.org/files/memcached-1.6.22.tar.gz
# Mon, 04 Dec 2023 18:08:47 GMT
ENV MEMCACHED_SHA1=7a691f390d59616dbebfc9e2e4942d499c39a338
# Mon, 04 Dec 2023 18:08:47 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O memcached.tar.gz "$MEMCACHED_URL"; 	echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c -; 	mkdir -p /usr/src/memcached; 	tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1; 	rm memcached.tar.gz; 		cd /usr/src/memcached; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	; 	nproc="$(nproc)"; 	make -j "$nproc"; 		sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf; 	make test PARALLEL="$nproc"; 	mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf; 		make install; 		cd /; 	rm -rf /usr/src/memcached; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		memcached -V # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 04 Dec 2023 18:08:47 GMT
USER memcache
# Mon, 04 Dec 2023 18:08:47 GMT
EXPOSE map[11211/tcp:{}]
# Mon, 04 Dec 2023 18:08:47 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:1f7ce2fa46ab3942feabee654933948821303a5a821789dddab2d8c3df59e227`  
		Last Modified: Tue, 21 Nov 2023 05:25:58 GMT  
		Size: 29.1 MB (29149908 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:21ac6fd160890cbc46a76542eb3f68654f3e3fb043b1b28a18155ec6863d60bc`  
		Last Modified: Tue, 12 Dec 2023 20:52:57 GMT  
		Size: 1.1 KB (1112 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6330fc82e1304befcc27a7598cd1a85152985d06426f94966788bf5a1583dcc6`  
		Last Modified: Tue, 12 Dec 2023 20:52:57 GMT  
		Size: 2.5 MB (2488284 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4047c827380f04698fbc51155441d719f93b84c1a092d633260c704f286296dd`  
		Last Modified: Tue, 12 Dec 2023 20:52:57 GMT  
		Size: 9.5 MB (9485895 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:401b5de2a4f8d9f588888754fa8347b67590c776363770f46ef67688116a4a0c`  
		Last Modified: Tue, 12 Dec 2023 20:52:57 GMT  
		Size: 285.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ee899f9aed95096580ea4a2325fd4824518ff1621f433f393fa253b52b7294b5`  
		Last Modified: Tue, 12 Dec 2023 20:52:58 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1-bookworm` - unknown; unknown

```console
$ docker pull memcached@sha256:5ccb88c1a86bd6524b6d5c9383254cdd79314d656a0c982658ecd35d9716431b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 MB (3077929 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:238ef9023561adc9c09faf875c5370cb2711a83cc7327dcc49ae7f8255c23794`

```dockerfile
```

-	Layers:
	-	`sha256:f84a6f3d0bdab8613be68ff091a6a78bedf8f697d4df55ff90ac7b745337e72c`  
		Last Modified: Tue, 12 Dec 2023 20:52:57 GMT  
		Size: 3.1 MB (3056812 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:8d7aee053ab87a86e42ba3d14810d3f1918c6e66d4d3ef02bc9c741f3948b83e`  
		Last Modified: Tue, 12 Dec 2023 20:52:57 GMT  
		Size: 21.1 KB (21117 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:1-bookworm` - linux; arm variant v5

```console
$ docker pull memcached@sha256:cb9426984b18b2d3df1c5fbb2bb7e2e9ebe08325d4adce6d0cd7a9207c413476
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.1 MB (37113170 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a8f2fb6119b629983f190d8b73208a156991d8cb65c47579a68125c339e9c75`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 21 Nov 2023 05:00:51 GMT
ADD file:1ae8e5ac45b11d01083680b765e1fcfef9f7938f89d6f424572126fa946d8cdf in / 
# Tue, 21 Nov 2023 05:00:52 GMT
CMD ["bash"]
# Mon, 04 Dec 2023 18:08:47 GMT
RUN set -eux; 	groupadd --system --gid 11211 memcache; 	useradd --system --gid memcache --uid 11211 memcache # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
ENV MEMCACHED_VERSION=1.6.22
# Mon, 04 Dec 2023 18:08:47 GMT
ENV MEMCACHED_URL=https://memcached.org/files/memcached-1.6.22.tar.gz
# Mon, 04 Dec 2023 18:08:47 GMT
ENV MEMCACHED_SHA1=7a691f390d59616dbebfc9e2e4942d499c39a338
# Mon, 04 Dec 2023 18:08:47 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O memcached.tar.gz "$MEMCACHED_URL"; 	echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c -; 	mkdir -p /usr/src/memcached; 	tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1; 	rm memcached.tar.gz; 		cd /usr/src/memcached; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	; 	nproc="$(nproc)"; 	make -j "$nproc"; 		sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf; 	make test PARALLEL="$nproc"; 	mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf; 		make install; 		cd /; 	rm -rf /usr/src/memcached; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		memcached -V # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 04 Dec 2023 18:08:47 GMT
USER memcache
# Mon, 04 Dec 2023 18:08:47 GMT
EXPOSE map[11211/tcp:{}]
# Mon, 04 Dec 2023 18:08:47 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:f476aef5b6e1122850e68c81ef06fc2df17e968961b060483b4d2fb33018aae3`  
		Last Modified: Tue, 21 Nov 2023 05:03:55 GMT  
		Size: 26.9 MB (26922153 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:89367ca16d2c3104d44514e1b9b94b0ac4070ea0f6f04523c72dda62795f3a17`  
		Last Modified: Tue, 12 Dec 2023 21:47:13 GMT  
		Size: 1.1 KB (1110 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5ecbc6577cf78c09bd4136f78a57a904ae1ab705fce8595e8d1187d800158e6f`  
		Last Modified: Tue, 12 Dec 2023 21:47:14 GMT  
		Size: 2.1 MB (2089289 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:12f8a270079b04e1372c73cc16ff2ae33e6f6ee0dcc7e8ed57843fca20b3d038`  
		Last Modified: Tue, 12 Dec 2023 21:47:14 GMT  
		Size: 8.1 MB (8100211 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5f592556023f9ba6125ecf6b89156ba61c05526ad324708c3d2a09600ee5e7e4`  
		Last Modified: Tue, 12 Dec 2023 21:47:14 GMT  
		Size: 285.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fa757a09f6a7a23114a13869f15b229384628cf108567d395dc0d4730c685409`  
		Last Modified: Tue, 12 Dec 2023 21:47:14 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1-bookworm` - unknown; unknown

```console
$ docker pull memcached@sha256:0c93e2660a508733f1c7d5236af77ef81fbcd0b27e4ac55c81d83334c8794891
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.0 KB (21043 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:538fbf714aa2f8a4175400dd43b0715e416f73fe598fc50d3f763afa144595da`

```dockerfile
```

-	Layers:
	-	`sha256:f65b3a9a0f6936cae3c1e411ecdd846d754a1978d851fdacf4b25526cb9ff4cc`  
		Last Modified: Tue, 12 Dec 2023 21:47:14 GMT  
		Size: 21.0 KB (21043 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:1-bookworm` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:c5adc5a4207d95c96a36131c2d39085b082f0e22f4595b935e72bcb463c10383
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.0 MB (39979924 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf26c17403ed5a4db96ddd8b41aeb2fd45483f897882a57972c994c95a44c5dd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 21 Nov 2023 06:27:06 GMT
ADD file:869c7d0747a17c53715581a2e862992eb8516c7f45f167821dfa80966a4870d1 in / 
# Tue, 21 Nov 2023 06:27:06 GMT
CMD ["bash"]
# Mon, 04 Dec 2023 18:08:47 GMT
RUN set -eux; 	groupadd --system --gid 11211 memcache; 	useradd --system --gid memcache --uid 11211 memcache # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
ENV MEMCACHED_VERSION=1.6.22
# Mon, 04 Dec 2023 18:08:47 GMT
ENV MEMCACHED_URL=https://memcached.org/files/memcached-1.6.22.tar.gz
# Mon, 04 Dec 2023 18:08:47 GMT
ENV MEMCACHED_SHA1=7a691f390d59616dbebfc9e2e4942d499c39a338
# Mon, 04 Dec 2023 18:08:47 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O memcached.tar.gz "$MEMCACHED_URL"; 	echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c -; 	mkdir -p /usr/src/memcached; 	tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1; 	rm memcached.tar.gz; 		cd /usr/src/memcached; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	; 	nproc="$(nproc)"; 	make -j "$nproc"; 		sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf; 	make test PARALLEL="$nproc"; 	mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf; 		make install; 		cd /; 	rm -rf /usr/src/memcached; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		memcached -V # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 04 Dec 2023 18:08:47 GMT
USER memcache
# Mon, 04 Dec 2023 18:08:47 GMT
EXPOSE map[11211/tcp:{}]
# Mon, 04 Dec 2023 18:08:47 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:2c6d21737d8318aa15c4cc838475029a5efc36c0429e3d8da80d97d0b96d9aaf`  
		Last Modified: Tue, 21 Nov 2023 06:30:30 GMT  
		Size: 29.2 MB (29179277 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1a39d6fec0d552a8078ab223bafd58bc9a0c8c27c26600a5b95c6a521bb97f3d`  
		Last Modified: Tue, 12 Dec 2023 23:43:17 GMT  
		Size: 1.1 KB (1112 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9d1ceea69964553dd3aaf853e0d7b753495cab4623b9377c69096be0bdf88146`  
		Last Modified: Tue, 12 Dec 2023 23:43:17 GMT  
		Size: 2.3 MB (2345975 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:52063b8e37cbc1e5e6e3af0f54b834ae3f6a53d023349ae819c9607e5fc98aec`  
		Last Modified: Tue, 12 Dec 2023 23:43:17 GMT  
		Size: 8.5 MB (8453155 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5b99d0095a64f8110efee1f5e91754cc923294d50c9e2927e515354746a3f465`  
		Last Modified: Tue, 12 Dec 2023 23:43:17 GMT  
		Size: 284.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:913c9e21eaa9c49c99b1b39e5cda0ef12356220075c869ea4776dca36fe83b75`  
		Last Modified: Tue, 12 Dec 2023 23:43:18 GMT  
		Size: 121.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1-bookworm` - unknown; unknown

```console
$ docker pull memcached@sha256:3d519a2eb9e00b43e6bc7584f6962b12ba032c4487a6e4ef7fd2b00b667bc90d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 MB (3053138 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9cc25288d58197dcc1309ea4a8128d0b120b92ad2d877f226095cd4847696474`

```dockerfile
```

-	Layers:
	-	`sha256:c5edc5ba98b4e6a438caa0d4541784c5c1e8b23d6020bc0b2a5b9910d0725400`  
		Last Modified: Tue, 12 Dec 2023 23:43:17 GMT  
		Size: 3.0 MB (3032003 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:b15e35765293b6f1da0e628c94108f229423c5a6379b8b5c47a41415f377b6d8`  
		Last Modified: Tue, 12 Dec 2023 23:43:17 GMT  
		Size: 21.1 KB (21135 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:1-bookworm` - linux; 386

```console
$ docker pull memcached@sha256:fa9dba8086765d68f2feecfc2ac08fb29c019597d09943bb480227e6cba87666
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.3 MB (39294993 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:93047050e75b6d4d64adb8a7c8f68cb118bad27ca9dc772120e251b174752cf9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 16 Oct 2023 06:54:12 GMT
ADD file:0c94521fdd9c0a4fdeeb9aad23e68cd053fba0dcd7c3af550aefa79377816e31 in / 
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["bash"]
# Mon, 16 Oct 2023 06:54:12 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_VERSION=1.6.22
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_SHA1=7a691f390d59616dbebfc9e2e4942d499c39a338
# Mon, 16 Oct 2023 06:54:12 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V # buildkit
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
	-	`sha256:98bdfce9af831c2a0d0bfcca812d0039cd1666986550f552b4b4c625bd5aa31c`  
		Last Modified: Wed, 01 Nov 2023 00:43:26 GMT  
		Size: 30.2 MB (30164042 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1b647d4b10cf20ac5807101c7d0380701be684aa82f5c01ec41f674b5ef23d42`  
		Last Modified: Wed, 01 Nov 2023 01:06:49 GMT  
		Size: 1.1 KB (1109 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b61c058003459de4911c2901b2d799b03de754a1b9e64ffbe21a04992e962e62`  
		Last Modified: Wed, 01 Nov 2023 01:06:49 GMT  
		Size: 2.5 MB (2492501 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:810b6db64df2fcc8f76941cdac75093cf35bd72ac3cd1fa5eb664e74c1f67cd8`  
		Last Modified: Wed, 01 Nov 2023 01:06:50 GMT  
		Size: 6.6 MB (6636937 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:dbb899942df4149bd5fae8bac6e295285ec80f82d621f2b29c931ee348491cfb`  
		Last Modified: Wed, 01 Nov 2023 01:06:49 GMT  
		Size: 282.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4a8530160ab232c37c0ddcbf5e3a731d835d378d1382843957f6c2a73b2b5be6`  
		Last Modified: Wed, 01 Nov 2023 01:06:50 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1-bookworm` - unknown; unknown

```console
$ docker pull memcached@sha256:dd7ce9519c31365127142232df2ed0b285e9acc03cd77c23c838bf932165def8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.5 KB (21498 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eef82c92e07c11a92c337806d01cfb1c6cdc7a16608dcf304a38de34d2ef1dbb`

```dockerfile
```

-	Layers:
	-	`sha256:c0d9dd22513f8d3e791e1796d7ef1906e57c798c92dd35d0be9cf2eaecec5954`  
		Last Modified: Wed, 01 Nov 2023 01:06:49 GMT  
		Size: 21.5 KB (21498 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:1-bookworm` - linux; mips64le

```console
$ docker pull memcached@sha256:9f7696d5078cf83e8b152cb00a3615576fd3c50d10be9253b9c188e16bfd8087
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.9 MB (39863164 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:685886644cfb343923260c15c66eb8c8d8bf7b84b6b1e855732aec2359b6ae29`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 21 Nov 2023 04:09:50 GMT
ADD file:e093749192323dc72b60a8440ddba26c415586f618b5e107fa264ba5eb2ca7ba in / 
# Tue, 21 Nov 2023 04:09:54 GMT
CMD ["bash"]
# Mon, 04 Dec 2023 18:08:47 GMT
RUN set -eux; 	groupadd --system --gid 11211 memcache; 	useradd --system --gid memcache --uid 11211 memcache # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
ENV MEMCACHED_VERSION=1.6.22
# Mon, 04 Dec 2023 18:08:47 GMT
ENV MEMCACHED_URL=https://memcached.org/files/memcached-1.6.22.tar.gz
# Mon, 04 Dec 2023 18:08:47 GMT
ENV MEMCACHED_SHA1=7a691f390d59616dbebfc9e2e4942d499c39a338
# Mon, 04 Dec 2023 18:08:47 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O memcached.tar.gz "$MEMCACHED_URL"; 	echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c -; 	mkdir -p /usr/src/memcached; 	tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1; 	rm memcached.tar.gz; 		cd /usr/src/memcached; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	; 	nproc="$(nproc)"; 	make -j "$nproc"; 		sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf; 	make test PARALLEL="$nproc"; 	mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf; 		make install; 		cd /; 	rm -rf /usr/src/memcached; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		memcached -V # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 04 Dec 2023 18:08:47 GMT
USER memcache
# Mon, 04 Dec 2023 18:08:47 GMT
EXPOSE map[11211/tcp:{}]
# Mon, 04 Dec 2023 18:08:47 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:ebdff2138fee4a3ec27560ab1353dc51c12c2608ff721f5db3d24104872b702a`  
		Last Modified: Tue, 21 Nov 2023 04:20:35 GMT  
		Size: 29.1 MB (29141984 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ee63ae82c6a87dc28cedafb91fbd6eaccd22add5b00a9cceb208472b30427b5d`  
		Last Modified: Tue, 12 Dec 2023 23:10:03 GMT  
		Size: 1.1 KB (1114 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3d430991f88102b07bcf8bf22f07667e49c9dfedb134b0ac36ddbb99d1e79db2`  
		Last Modified: Tue, 12 Dec 2023 23:10:04 GMT  
		Size: 1.9 MB (1937475 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ebe1140b392e915b8757b8d0a4b83f0aaf2103734e9f83c318821f641207b6b4`  
		Last Modified: Tue, 12 Dec 2023 23:10:04 GMT  
		Size: 8.8 MB (8782185 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:aedf1130e49a6aa7d9b74b9fd00914b171966fcf8beba71095787811fa3a0284`  
		Last Modified: Tue, 12 Dec 2023 23:10:03 GMT  
		Size: 284.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:457e2691e0499a1a1d26e6da85567f20a8dc396bde9d9952ce75fdcfe6cbafd8`  
		Last Modified: Tue, 12 Dec 2023 23:10:05 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1-bookworm` - unknown; unknown

```console
$ docker pull memcached@sha256:d48752667ff111ef73342ae5c16218a373275e8b65c7696eff231ff49ca7b8e5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.0 KB (21004 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9138b1207d88c6ca6b32a2616d3c25b1f5d3280b7650ac4bfa7120518f6a8ad7`

```dockerfile
```

-	Layers:
	-	`sha256:2b1c5f3190ac8dfdff54a51d9421ad623af991deba1a46ba943cf88442079207`  
		Last Modified: Tue, 12 Dec 2023 23:10:03 GMT  
		Size: 21.0 KB (21004 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:1-bookworm` - linux; ppc64le

```console
$ docker pull memcached@sha256:813f2ed7d8d4d2c4e6f4a19816964b0c95cc56d038d95d059571d51e115ab109
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.5 MB (45508655 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:73c79988c4d09a9ac9cb01aa05096b344821e8034c3cba04afb9cb78fe25db05`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 21 Nov 2023 04:24:14 GMT
ADD file:8b22a531b6611a1e63dfc20e4e2931592e2d821bd4b64c4b2810bb9a36640c02 in / 
# Tue, 21 Nov 2023 04:24:16 GMT
CMD ["bash"]
# Mon, 04 Dec 2023 18:08:47 GMT
RUN set -eux; 	groupadd --system --gid 11211 memcache; 	useradd --system --gid memcache --uid 11211 memcache # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
ENV MEMCACHED_VERSION=1.6.22
# Mon, 04 Dec 2023 18:08:47 GMT
ENV MEMCACHED_URL=https://memcached.org/files/memcached-1.6.22.tar.gz
# Mon, 04 Dec 2023 18:08:47 GMT
ENV MEMCACHED_SHA1=7a691f390d59616dbebfc9e2e4942d499c39a338
# Mon, 04 Dec 2023 18:08:47 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O memcached.tar.gz "$MEMCACHED_URL"; 	echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c -; 	mkdir -p /usr/src/memcached; 	tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1; 	rm memcached.tar.gz; 		cd /usr/src/memcached; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	; 	nproc="$(nproc)"; 	make -j "$nproc"; 		sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf; 	make test PARALLEL="$nproc"; 	mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf; 		make install; 		cd /; 	rm -rf /usr/src/memcached; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		memcached -V # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 04 Dec 2023 18:08:47 GMT
USER memcache
# Mon, 04 Dec 2023 18:08:47 GMT
EXPOSE map[11211/tcp:{}]
# Mon, 04 Dec 2023 18:08:47 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:c570d04e61d8e35a3c8f12179d048d701451f97f9cf2099ea3e3738512dbf062`  
		Last Modified: Tue, 21 Nov 2023 04:28:58 GMT  
		Size: 33.1 MB (33141607 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b53469d03d0156e89526c2b744f6850b65cfb9b509a6fda4c523764f7a9f9072`  
		Last Modified: Tue, 12 Dec 2023 23:08:09 GMT  
		Size: 1.1 KB (1111 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:12b61a5974195d80345022ed47cb4546f6fec60527b3932b2ce74d605db750e0`  
		Last Modified: Tue, 12 Dec 2023 23:08:09 GMT  
		Size: 2.7 MB (2698202 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:108f5df7a0010e4f69929c6ce4ff2e0e53877c6bbe11bd86acbbb0e7b608dca7`  
		Last Modified: Tue, 12 Dec 2023 23:08:09 GMT  
		Size: 9.7 MB (9667330 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:aa53d1e0a6b1123a31838e581de8d738ccaf05c9be569ec50b8d37cbc54a99bd`  
		Last Modified: Tue, 12 Dec 2023 23:08:08 GMT  
		Size: 283.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2cf8ef0b438a2029bfc9b928364eb71966baa4990e2ac4a9b1648cbd44271dc4`  
		Last Modified: Tue, 12 Dec 2023 23:08:10 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1-bookworm` - unknown; unknown

```console
$ docker pull memcached@sha256:d75efc7b8726fbfade0b41c14205058def09ee997a7befb495808c2752a56a54
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 MB (3066416 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ca8bb0be2316bb58a60c953382dd1963eb7e265d0602de370e02152e1ac84d7`

```dockerfile
```

-	Layers:
	-	`sha256:34203b346608565cdbcd7cf9a56efb8ec2255b1a8f30267d6b2749d6a0bd2d6b`  
		Last Modified: Tue, 12 Dec 2023 23:08:09 GMT  
		Size: 3.0 MB (3045398 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:4da4f2a55f1773bfac75983e2e733c609b970884e935de987ec5b3ec5c92eb85`  
		Last Modified: Tue, 12 Dec 2023 23:08:08 GMT  
		Size: 21.0 KB (21018 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:1-bookworm` - linux; s390x

```console
$ docker pull memcached@sha256:05084fffc798db32442e2cde93eac5815ffd909e9bf65692ac08c9b5ab79e677
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.0 MB (38041790 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eac80baab625f3daf940cdb3053e2e709bd61d78d7eae50b7db4d71f87bcd149`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 21 Nov 2023 05:04:35 GMT
ADD file:c33fa9fdde73983850798b6eb1cd062e0398109d1d773e6a937fead7475c8efc in / 
# Tue, 21 Nov 2023 05:04:41 GMT
CMD ["bash"]
# Mon, 04 Dec 2023 18:08:47 GMT
RUN set -eux; 	groupadd --system --gid 11211 memcache; 	useradd --system --gid memcache --uid 11211 memcache # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
ENV MEMCACHED_VERSION=1.6.22
# Mon, 04 Dec 2023 18:08:47 GMT
ENV MEMCACHED_URL=https://memcached.org/files/memcached-1.6.22.tar.gz
# Mon, 04 Dec 2023 18:08:47 GMT
ENV MEMCACHED_SHA1=7a691f390d59616dbebfc9e2e4942d499c39a338
# Mon, 04 Dec 2023 18:08:47 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O memcached.tar.gz "$MEMCACHED_URL"; 	echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c -; 	mkdir -p /usr/src/memcached; 	tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1; 	rm memcached.tar.gz; 		cd /usr/src/memcached; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	; 	nproc="$(nproc)"; 	make -j "$nproc"; 		sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf; 	make test PARALLEL="$nproc"; 	mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf; 		make install; 		cd /; 	rm -rf /usr/src/memcached; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		memcached -V # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 04 Dec 2023 18:08:47 GMT
USER memcache
# Mon, 04 Dec 2023 18:08:47 GMT
EXPOSE map[11211/tcp:{}]
# Mon, 04 Dec 2023 18:08:47 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:6daa625e5a040476e253e7acd0befa74254a4865ec836d6334a544d82a21d4be`  
		Last Modified: Tue, 21 Nov 2023 05:10:21 GMT  
		Size: 27.5 MB (27512885 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b19a3143cbec7ddc9a646dbbe779b0b5ec67662cf70e280db146f6ace54ccd61`  
		Last Modified: Wed, 13 Dec 2023 00:26:35 GMT  
		Size: 1.1 KB (1111 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b8af028b1fa76aa55f540dd5be5eaf89eea3fec23e09e9a88550aac36e9ee843`  
		Last Modified: Wed, 13 Dec 2023 00:26:35 GMT  
		Size: 2.2 MB (2152508 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9a774943469875a0902c53fccdd95cad9c18234b759bcdcc5816bd563deb7f14`  
		Last Modified: Wed, 13 Dec 2023 00:26:35 GMT  
		Size: 8.4 MB (8374880 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:266b4bf499a815da6f7ddcf68e1e61f8418c8ec655a2083e174aaa385de74d76`  
		Last Modified: Wed, 13 Dec 2023 00:26:35 GMT  
		Size: 284.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0da709e3482cc552b0a7b69eb05aaa21af1e74baaf4e3bccc34e95e478943630`  
		Last Modified: Wed, 13 Dec 2023 00:26:36 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1-bookworm` - unknown; unknown

```console
$ docker pull memcached@sha256:525abad348ba03c5b9444f23409d647581284c1642d30539e2c9943405266f12
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 MB (3067303 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e3b551ec9122d039520bbd13bced5b1f5b0d5b1fd9e32c09a1d4536f7af1226`

```dockerfile
```

-	Layers:
	-	`sha256:5cc0958f61715f0746d9fa2a8a5c06f31608bb5d1cf32d606c46fc8e11b35984`  
		Last Modified: Wed, 13 Dec 2023 00:26:35 GMT  
		Size: 3.0 MB (3046353 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:3d2fed99d3355e42a820c1975105411eb7584cffb111d7e1fd541603f7721f1c`  
		Last Modified: Wed, 13 Dec 2023 00:26:35 GMT  
		Size: 20.9 KB (20950 bytes)  
		MIME: application/vnd.in-toto+json

## `memcached:1.6`

```console
$ docker pull memcached@sha256:c0aa354cc777aa9bdbaf3789db81b1b1802be11940498801dbe1562999d5671e
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 15
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm variant v5
	-	unknown; unknown
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	unknown; unknown
	-	linux; 386
	-	unknown; unknown
	-	linux; mips64le
	-	unknown; unknown
	-	linux; ppc64le
	-	unknown; unknown
	-	linux; s390x
	-	unknown; unknown

### `memcached:1.6` - linux; amd64

```console
$ docker pull memcached@sha256:0d358fa0198562aa3d1e1c3e9386e1835256875517d8a4786f3dd50a1f65f1de
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.1 MB (41125606 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:03bad2c21b5df5c82f8c581ebec403482a3e00c0f35697ca669c46a7d000a13d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 21 Nov 2023 05:21:37 GMT
ADD file:d261a6f6921593f1e0b3f472ab1b1822e2c6deb0b369200f0b3370556bfad017 in / 
# Tue, 21 Nov 2023 05:21:37 GMT
CMD ["bash"]
# Mon, 04 Dec 2023 18:08:47 GMT
RUN set -eux; 	groupadd --system --gid 11211 memcache; 	useradd --system --gid memcache --uid 11211 memcache # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
ENV MEMCACHED_VERSION=1.6.22
# Mon, 04 Dec 2023 18:08:47 GMT
ENV MEMCACHED_URL=https://memcached.org/files/memcached-1.6.22.tar.gz
# Mon, 04 Dec 2023 18:08:47 GMT
ENV MEMCACHED_SHA1=7a691f390d59616dbebfc9e2e4942d499c39a338
# Mon, 04 Dec 2023 18:08:47 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O memcached.tar.gz "$MEMCACHED_URL"; 	echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c -; 	mkdir -p /usr/src/memcached; 	tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1; 	rm memcached.tar.gz; 		cd /usr/src/memcached; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	; 	nproc="$(nproc)"; 	make -j "$nproc"; 		sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf; 	make test PARALLEL="$nproc"; 	mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf; 		make install; 		cd /; 	rm -rf /usr/src/memcached; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		memcached -V # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 04 Dec 2023 18:08:47 GMT
USER memcache
# Mon, 04 Dec 2023 18:08:47 GMT
EXPOSE map[11211/tcp:{}]
# Mon, 04 Dec 2023 18:08:47 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:1f7ce2fa46ab3942feabee654933948821303a5a821789dddab2d8c3df59e227`  
		Last Modified: Tue, 21 Nov 2023 05:25:58 GMT  
		Size: 29.1 MB (29149908 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:21ac6fd160890cbc46a76542eb3f68654f3e3fb043b1b28a18155ec6863d60bc`  
		Last Modified: Tue, 12 Dec 2023 20:52:57 GMT  
		Size: 1.1 KB (1112 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6330fc82e1304befcc27a7598cd1a85152985d06426f94966788bf5a1583dcc6`  
		Last Modified: Tue, 12 Dec 2023 20:52:57 GMT  
		Size: 2.5 MB (2488284 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4047c827380f04698fbc51155441d719f93b84c1a092d633260c704f286296dd`  
		Last Modified: Tue, 12 Dec 2023 20:52:57 GMT  
		Size: 9.5 MB (9485895 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:401b5de2a4f8d9f588888754fa8347b67590c776363770f46ef67688116a4a0c`  
		Last Modified: Tue, 12 Dec 2023 20:52:57 GMT  
		Size: 285.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ee899f9aed95096580ea4a2325fd4824518ff1621f433f393fa253b52b7294b5`  
		Last Modified: Tue, 12 Dec 2023 20:52:58 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1.6` - unknown; unknown

```console
$ docker pull memcached@sha256:5ccb88c1a86bd6524b6d5c9383254cdd79314d656a0c982658ecd35d9716431b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 MB (3077929 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:238ef9023561adc9c09faf875c5370cb2711a83cc7327dcc49ae7f8255c23794`

```dockerfile
```

-	Layers:
	-	`sha256:f84a6f3d0bdab8613be68ff091a6a78bedf8f697d4df55ff90ac7b745337e72c`  
		Last Modified: Tue, 12 Dec 2023 20:52:57 GMT  
		Size: 3.1 MB (3056812 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:8d7aee053ab87a86e42ba3d14810d3f1918c6e66d4d3ef02bc9c741f3948b83e`  
		Last Modified: Tue, 12 Dec 2023 20:52:57 GMT  
		Size: 21.1 KB (21117 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:1.6` - linux; arm variant v5

```console
$ docker pull memcached@sha256:cb9426984b18b2d3df1c5fbb2bb7e2e9ebe08325d4adce6d0cd7a9207c413476
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.1 MB (37113170 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a8f2fb6119b629983f190d8b73208a156991d8cb65c47579a68125c339e9c75`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 21 Nov 2023 05:00:51 GMT
ADD file:1ae8e5ac45b11d01083680b765e1fcfef9f7938f89d6f424572126fa946d8cdf in / 
# Tue, 21 Nov 2023 05:00:52 GMT
CMD ["bash"]
# Mon, 04 Dec 2023 18:08:47 GMT
RUN set -eux; 	groupadd --system --gid 11211 memcache; 	useradd --system --gid memcache --uid 11211 memcache # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
ENV MEMCACHED_VERSION=1.6.22
# Mon, 04 Dec 2023 18:08:47 GMT
ENV MEMCACHED_URL=https://memcached.org/files/memcached-1.6.22.tar.gz
# Mon, 04 Dec 2023 18:08:47 GMT
ENV MEMCACHED_SHA1=7a691f390d59616dbebfc9e2e4942d499c39a338
# Mon, 04 Dec 2023 18:08:47 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O memcached.tar.gz "$MEMCACHED_URL"; 	echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c -; 	mkdir -p /usr/src/memcached; 	tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1; 	rm memcached.tar.gz; 		cd /usr/src/memcached; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	; 	nproc="$(nproc)"; 	make -j "$nproc"; 		sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf; 	make test PARALLEL="$nproc"; 	mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf; 		make install; 		cd /; 	rm -rf /usr/src/memcached; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		memcached -V # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 04 Dec 2023 18:08:47 GMT
USER memcache
# Mon, 04 Dec 2023 18:08:47 GMT
EXPOSE map[11211/tcp:{}]
# Mon, 04 Dec 2023 18:08:47 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:f476aef5b6e1122850e68c81ef06fc2df17e968961b060483b4d2fb33018aae3`  
		Last Modified: Tue, 21 Nov 2023 05:03:55 GMT  
		Size: 26.9 MB (26922153 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:89367ca16d2c3104d44514e1b9b94b0ac4070ea0f6f04523c72dda62795f3a17`  
		Last Modified: Tue, 12 Dec 2023 21:47:13 GMT  
		Size: 1.1 KB (1110 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5ecbc6577cf78c09bd4136f78a57a904ae1ab705fce8595e8d1187d800158e6f`  
		Last Modified: Tue, 12 Dec 2023 21:47:14 GMT  
		Size: 2.1 MB (2089289 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:12f8a270079b04e1372c73cc16ff2ae33e6f6ee0dcc7e8ed57843fca20b3d038`  
		Last Modified: Tue, 12 Dec 2023 21:47:14 GMT  
		Size: 8.1 MB (8100211 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5f592556023f9ba6125ecf6b89156ba61c05526ad324708c3d2a09600ee5e7e4`  
		Last Modified: Tue, 12 Dec 2023 21:47:14 GMT  
		Size: 285.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fa757a09f6a7a23114a13869f15b229384628cf108567d395dc0d4730c685409`  
		Last Modified: Tue, 12 Dec 2023 21:47:14 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1.6` - unknown; unknown

```console
$ docker pull memcached@sha256:0c93e2660a508733f1c7d5236af77ef81fbcd0b27e4ac55c81d83334c8794891
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.0 KB (21043 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:538fbf714aa2f8a4175400dd43b0715e416f73fe598fc50d3f763afa144595da`

```dockerfile
```

-	Layers:
	-	`sha256:f65b3a9a0f6936cae3c1e411ecdd846d754a1978d851fdacf4b25526cb9ff4cc`  
		Last Modified: Tue, 12 Dec 2023 21:47:14 GMT  
		Size: 21.0 KB (21043 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:1.6` - linux; arm variant v7

```console
$ docker pull memcached@sha256:2841be0a36134563966c09a6ed68b21053d20342ec8736cf92763c28077ead43
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.1 MB (28094215 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6cf74ffa940dd93988fc0beb6698c5796563c82a40b7dd668153969f64d2e6ca`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 09 Feb 2023 06:12:09 GMT
ADD file:5f1a343224e8486690bd90dd1e50c8d84b3d770c51bb6829544e5cf650c0419c in / 
# Thu, 09 Feb 2023 06:12:10 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 07:52:31 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Thu, 09 Feb 2023 07:52:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 07:52:35 GMT
ENV MEMCACHED_VERSION=1.6.18
# Thu, 09 Feb 2023 07:52:35 GMT
ENV MEMCACHED_SHA1=be16909bb75ab972ee5fe438312501de01c4725a
# Thu, 09 Feb 2023 07:55:44 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 09 Feb 2023 07:55:44 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 09 Feb 2023 07:55:44 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 09 Feb 2023 07:55:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 09 Feb 2023 07:55:44 GMT
USER memcache
# Thu, 09 Feb 2023 07:55:45 GMT
EXPOSE 11211
# Thu, 09 Feb 2023 07:55:45 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:e7318f6106ad75d7d482ae9dddf4d927b0872ef3ddb6e1330aa691fc8d17279e`  
		Last Modified: Thu, 09 Feb 2023 06:19:19 GMT  
		Size: 26.6 MB (26577666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de49d9d72daf1680b5f1b9532dd2eb0162829f36c8db9669935462636fbf99d9`  
		Last Modified: Thu, 09 Feb 2023 08:06:11 GMT  
		Size: 4.9 KB (4895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0beac9d5bcac946f8c54c72b8a9c136914b1aa7a5fe2b8c3df4c7d8858ea6559`  
		Last Modified: Thu, 09 Feb 2023 08:06:11 GMT  
		Size: 312.1 KB (312088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4c9e5a265394e4c0f357779e6195a4e82d767a3691a0e77d427e56651c3e54a`  
		Last Modified: Thu, 09 Feb 2023 08:06:11 GMT  
		Size: 1.2 MB (1199163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5ea82ad892fe1ae8623d84e32c8c027087cda8aa49e40d4546ed6942e471c60`  
		Last Modified: Thu, 09 Feb 2023 08:06:11 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa2ae3bcdc0d114ba49a67df022b6f7215fc87f1f50e64939fcfbbec4eaadee5`  
		Last Modified: Thu, 09 Feb 2023 08:06:11 GMT  
		Size: 118.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:c5adc5a4207d95c96a36131c2d39085b082f0e22f4595b935e72bcb463c10383
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.0 MB (39979924 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf26c17403ed5a4db96ddd8b41aeb2fd45483f897882a57972c994c95a44c5dd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 21 Nov 2023 06:27:06 GMT
ADD file:869c7d0747a17c53715581a2e862992eb8516c7f45f167821dfa80966a4870d1 in / 
# Tue, 21 Nov 2023 06:27:06 GMT
CMD ["bash"]
# Mon, 04 Dec 2023 18:08:47 GMT
RUN set -eux; 	groupadd --system --gid 11211 memcache; 	useradd --system --gid memcache --uid 11211 memcache # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
ENV MEMCACHED_VERSION=1.6.22
# Mon, 04 Dec 2023 18:08:47 GMT
ENV MEMCACHED_URL=https://memcached.org/files/memcached-1.6.22.tar.gz
# Mon, 04 Dec 2023 18:08:47 GMT
ENV MEMCACHED_SHA1=7a691f390d59616dbebfc9e2e4942d499c39a338
# Mon, 04 Dec 2023 18:08:47 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O memcached.tar.gz "$MEMCACHED_URL"; 	echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c -; 	mkdir -p /usr/src/memcached; 	tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1; 	rm memcached.tar.gz; 		cd /usr/src/memcached; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	; 	nproc="$(nproc)"; 	make -j "$nproc"; 		sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf; 	make test PARALLEL="$nproc"; 	mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf; 		make install; 		cd /; 	rm -rf /usr/src/memcached; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		memcached -V # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 04 Dec 2023 18:08:47 GMT
USER memcache
# Mon, 04 Dec 2023 18:08:47 GMT
EXPOSE map[11211/tcp:{}]
# Mon, 04 Dec 2023 18:08:47 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:2c6d21737d8318aa15c4cc838475029a5efc36c0429e3d8da80d97d0b96d9aaf`  
		Last Modified: Tue, 21 Nov 2023 06:30:30 GMT  
		Size: 29.2 MB (29179277 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1a39d6fec0d552a8078ab223bafd58bc9a0c8c27c26600a5b95c6a521bb97f3d`  
		Last Modified: Tue, 12 Dec 2023 23:43:17 GMT  
		Size: 1.1 KB (1112 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9d1ceea69964553dd3aaf853e0d7b753495cab4623b9377c69096be0bdf88146`  
		Last Modified: Tue, 12 Dec 2023 23:43:17 GMT  
		Size: 2.3 MB (2345975 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:52063b8e37cbc1e5e6e3af0f54b834ae3f6a53d023349ae819c9607e5fc98aec`  
		Last Modified: Tue, 12 Dec 2023 23:43:17 GMT  
		Size: 8.5 MB (8453155 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5b99d0095a64f8110efee1f5e91754cc923294d50c9e2927e515354746a3f465`  
		Last Modified: Tue, 12 Dec 2023 23:43:17 GMT  
		Size: 284.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:913c9e21eaa9c49c99b1b39e5cda0ef12356220075c869ea4776dca36fe83b75`  
		Last Modified: Tue, 12 Dec 2023 23:43:18 GMT  
		Size: 121.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1.6` - unknown; unknown

```console
$ docker pull memcached@sha256:3d519a2eb9e00b43e6bc7584f6962b12ba032c4487a6e4ef7fd2b00b667bc90d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 MB (3053138 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9cc25288d58197dcc1309ea4a8128d0b120b92ad2d877f226095cd4847696474`

```dockerfile
```

-	Layers:
	-	`sha256:c5edc5ba98b4e6a438caa0d4541784c5c1e8b23d6020bc0b2a5b9910d0725400`  
		Last Modified: Tue, 12 Dec 2023 23:43:17 GMT  
		Size: 3.0 MB (3032003 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:b15e35765293b6f1da0e628c94108f229423c5a6379b8b5c47a41415f377b6d8`  
		Last Modified: Tue, 12 Dec 2023 23:43:17 GMT  
		Size: 21.1 KB (21135 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:1.6` - linux; 386

```console
$ docker pull memcached@sha256:fa9dba8086765d68f2feecfc2ac08fb29c019597d09943bb480227e6cba87666
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.3 MB (39294993 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:93047050e75b6d4d64adb8a7c8f68cb118bad27ca9dc772120e251b174752cf9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 16 Oct 2023 06:54:12 GMT
ADD file:0c94521fdd9c0a4fdeeb9aad23e68cd053fba0dcd7c3af550aefa79377816e31 in / 
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["bash"]
# Mon, 16 Oct 2023 06:54:12 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_VERSION=1.6.22
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_SHA1=7a691f390d59616dbebfc9e2e4942d499c39a338
# Mon, 16 Oct 2023 06:54:12 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V # buildkit
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
	-	`sha256:98bdfce9af831c2a0d0bfcca812d0039cd1666986550f552b4b4c625bd5aa31c`  
		Last Modified: Wed, 01 Nov 2023 00:43:26 GMT  
		Size: 30.2 MB (30164042 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1b647d4b10cf20ac5807101c7d0380701be684aa82f5c01ec41f674b5ef23d42`  
		Last Modified: Wed, 01 Nov 2023 01:06:49 GMT  
		Size: 1.1 KB (1109 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b61c058003459de4911c2901b2d799b03de754a1b9e64ffbe21a04992e962e62`  
		Last Modified: Wed, 01 Nov 2023 01:06:49 GMT  
		Size: 2.5 MB (2492501 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:810b6db64df2fcc8f76941cdac75093cf35bd72ac3cd1fa5eb664e74c1f67cd8`  
		Last Modified: Wed, 01 Nov 2023 01:06:50 GMT  
		Size: 6.6 MB (6636937 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:dbb899942df4149bd5fae8bac6e295285ec80f82d621f2b29c931ee348491cfb`  
		Last Modified: Wed, 01 Nov 2023 01:06:49 GMT  
		Size: 282.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4a8530160ab232c37c0ddcbf5e3a731d835d378d1382843957f6c2a73b2b5be6`  
		Last Modified: Wed, 01 Nov 2023 01:06:50 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1.6` - unknown; unknown

```console
$ docker pull memcached@sha256:dd7ce9519c31365127142232df2ed0b285e9acc03cd77c23c838bf932165def8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.5 KB (21498 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eef82c92e07c11a92c337806d01cfb1c6cdc7a16608dcf304a38de34d2ef1dbb`

```dockerfile
```

-	Layers:
	-	`sha256:c0d9dd22513f8d3e791e1796d7ef1906e57c798c92dd35d0be9cf2eaecec5954`  
		Last Modified: Wed, 01 Nov 2023 01:06:49 GMT  
		Size: 21.5 KB (21498 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:1.6` - linux; mips64le

```console
$ docker pull memcached@sha256:9f7696d5078cf83e8b152cb00a3615576fd3c50d10be9253b9c188e16bfd8087
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.9 MB (39863164 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:685886644cfb343923260c15c66eb8c8d8bf7b84b6b1e855732aec2359b6ae29`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 21 Nov 2023 04:09:50 GMT
ADD file:e093749192323dc72b60a8440ddba26c415586f618b5e107fa264ba5eb2ca7ba in / 
# Tue, 21 Nov 2023 04:09:54 GMT
CMD ["bash"]
# Mon, 04 Dec 2023 18:08:47 GMT
RUN set -eux; 	groupadd --system --gid 11211 memcache; 	useradd --system --gid memcache --uid 11211 memcache # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
ENV MEMCACHED_VERSION=1.6.22
# Mon, 04 Dec 2023 18:08:47 GMT
ENV MEMCACHED_URL=https://memcached.org/files/memcached-1.6.22.tar.gz
# Mon, 04 Dec 2023 18:08:47 GMT
ENV MEMCACHED_SHA1=7a691f390d59616dbebfc9e2e4942d499c39a338
# Mon, 04 Dec 2023 18:08:47 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O memcached.tar.gz "$MEMCACHED_URL"; 	echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c -; 	mkdir -p /usr/src/memcached; 	tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1; 	rm memcached.tar.gz; 		cd /usr/src/memcached; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	; 	nproc="$(nproc)"; 	make -j "$nproc"; 		sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf; 	make test PARALLEL="$nproc"; 	mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf; 		make install; 		cd /; 	rm -rf /usr/src/memcached; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		memcached -V # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 04 Dec 2023 18:08:47 GMT
USER memcache
# Mon, 04 Dec 2023 18:08:47 GMT
EXPOSE map[11211/tcp:{}]
# Mon, 04 Dec 2023 18:08:47 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:ebdff2138fee4a3ec27560ab1353dc51c12c2608ff721f5db3d24104872b702a`  
		Last Modified: Tue, 21 Nov 2023 04:20:35 GMT  
		Size: 29.1 MB (29141984 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ee63ae82c6a87dc28cedafb91fbd6eaccd22add5b00a9cceb208472b30427b5d`  
		Last Modified: Tue, 12 Dec 2023 23:10:03 GMT  
		Size: 1.1 KB (1114 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3d430991f88102b07bcf8bf22f07667e49c9dfedb134b0ac36ddbb99d1e79db2`  
		Last Modified: Tue, 12 Dec 2023 23:10:04 GMT  
		Size: 1.9 MB (1937475 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ebe1140b392e915b8757b8d0a4b83f0aaf2103734e9f83c318821f641207b6b4`  
		Last Modified: Tue, 12 Dec 2023 23:10:04 GMT  
		Size: 8.8 MB (8782185 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:aedf1130e49a6aa7d9b74b9fd00914b171966fcf8beba71095787811fa3a0284`  
		Last Modified: Tue, 12 Dec 2023 23:10:03 GMT  
		Size: 284.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:457e2691e0499a1a1d26e6da85567f20a8dc396bde9d9952ce75fdcfe6cbafd8`  
		Last Modified: Tue, 12 Dec 2023 23:10:05 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1.6` - unknown; unknown

```console
$ docker pull memcached@sha256:d48752667ff111ef73342ae5c16218a373275e8b65c7696eff231ff49ca7b8e5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.0 KB (21004 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9138b1207d88c6ca6b32a2616d3c25b1f5d3280b7650ac4bfa7120518f6a8ad7`

```dockerfile
```

-	Layers:
	-	`sha256:2b1c5f3190ac8dfdff54a51d9421ad623af991deba1a46ba943cf88442079207`  
		Last Modified: Tue, 12 Dec 2023 23:10:03 GMT  
		Size: 21.0 KB (21004 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:1.6` - linux; ppc64le

```console
$ docker pull memcached@sha256:813f2ed7d8d4d2c4e6f4a19816964b0c95cc56d038d95d059571d51e115ab109
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.5 MB (45508655 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:73c79988c4d09a9ac9cb01aa05096b344821e8034c3cba04afb9cb78fe25db05`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 21 Nov 2023 04:24:14 GMT
ADD file:8b22a531b6611a1e63dfc20e4e2931592e2d821bd4b64c4b2810bb9a36640c02 in / 
# Tue, 21 Nov 2023 04:24:16 GMT
CMD ["bash"]
# Mon, 04 Dec 2023 18:08:47 GMT
RUN set -eux; 	groupadd --system --gid 11211 memcache; 	useradd --system --gid memcache --uid 11211 memcache # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
ENV MEMCACHED_VERSION=1.6.22
# Mon, 04 Dec 2023 18:08:47 GMT
ENV MEMCACHED_URL=https://memcached.org/files/memcached-1.6.22.tar.gz
# Mon, 04 Dec 2023 18:08:47 GMT
ENV MEMCACHED_SHA1=7a691f390d59616dbebfc9e2e4942d499c39a338
# Mon, 04 Dec 2023 18:08:47 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O memcached.tar.gz "$MEMCACHED_URL"; 	echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c -; 	mkdir -p /usr/src/memcached; 	tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1; 	rm memcached.tar.gz; 		cd /usr/src/memcached; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	; 	nproc="$(nproc)"; 	make -j "$nproc"; 		sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf; 	make test PARALLEL="$nproc"; 	mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf; 		make install; 		cd /; 	rm -rf /usr/src/memcached; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		memcached -V # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 04 Dec 2023 18:08:47 GMT
USER memcache
# Mon, 04 Dec 2023 18:08:47 GMT
EXPOSE map[11211/tcp:{}]
# Mon, 04 Dec 2023 18:08:47 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:c570d04e61d8e35a3c8f12179d048d701451f97f9cf2099ea3e3738512dbf062`  
		Last Modified: Tue, 21 Nov 2023 04:28:58 GMT  
		Size: 33.1 MB (33141607 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b53469d03d0156e89526c2b744f6850b65cfb9b509a6fda4c523764f7a9f9072`  
		Last Modified: Tue, 12 Dec 2023 23:08:09 GMT  
		Size: 1.1 KB (1111 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:12b61a5974195d80345022ed47cb4546f6fec60527b3932b2ce74d605db750e0`  
		Last Modified: Tue, 12 Dec 2023 23:08:09 GMT  
		Size: 2.7 MB (2698202 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:108f5df7a0010e4f69929c6ce4ff2e0e53877c6bbe11bd86acbbb0e7b608dca7`  
		Last Modified: Tue, 12 Dec 2023 23:08:09 GMT  
		Size: 9.7 MB (9667330 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:aa53d1e0a6b1123a31838e581de8d738ccaf05c9be569ec50b8d37cbc54a99bd`  
		Last Modified: Tue, 12 Dec 2023 23:08:08 GMT  
		Size: 283.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2cf8ef0b438a2029bfc9b928364eb71966baa4990e2ac4a9b1648cbd44271dc4`  
		Last Modified: Tue, 12 Dec 2023 23:08:10 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1.6` - unknown; unknown

```console
$ docker pull memcached@sha256:d75efc7b8726fbfade0b41c14205058def09ee997a7befb495808c2752a56a54
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 MB (3066416 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ca8bb0be2316bb58a60c953382dd1963eb7e265d0602de370e02152e1ac84d7`

```dockerfile
```

-	Layers:
	-	`sha256:34203b346608565cdbcd7cf9a56efb8ec2255b1a8f30267d6b2749d6a0bd2d6b`  
		Last Modified: Tue, 12 Dec 2023 23:08:09 GMT  
		Size: 3.0 MB (3045398 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:4da4f2a55f1773bfac75983e2e733c609b970884e935de987ec5b3ec5c92eb85`  
		Last Modified: Tue, 12 Dec 2023 23:08:08 GMT  
		Size: 21.0 KB (21018 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:1.6` - linux; s390x

```console
$ docker pull memcached@sha256:05084fffc798db32442e2cde93eac5815ffd909e9bf65692ac08c9b5ab79e677
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.0 MB (38041790 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eac80baab625f3daf940cdb3053e2e709bd61d78d7eae50b7db4d71f87bcd149`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 21 Nov 2023 05:04:35 GMT
ADD file:c33fa9fdde73983850798b6eb1cd062e0398109d1d773e6a937fead7475c8efc in / 
# Tue, 21 Nov 2023 05:04:41 GMT
CMD ["bash"]
# Mon, 04 Dec 2023 18:08:47 GMT
RUN set -eux; 	groupadd --system --gid 11211 memcache; 	useradd --system --gid memcache --uid 11211 memcache # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
ENV MEMCACHED_VERSION=1.6.22
# Mon, 04 Dec 2023 18:08:47 GMT
ENV MEMCACHED_URL=https://memcached.org/files/memcached-1.6.22.tar.gz
# Mon, 04 Dec 2023 18:08:47 GMT
ENV MEMCACHED_SHA1=7a691f390d59616dbebfc9e2e4942d499c39a338
# Mon, 04 Dec 2023 18:08:47 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O memcached.tar.gz "$MEMCACHED_URL"; 	echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c -; 	mkdir -p /usr/src/memcached; 	tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1; 	rm memcached.tar.gz; 		cd /usr/src/memcached; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	; 	nproc="$(nproc)"; 	make -j "$nproc"; 		sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf; 	make test PARALLEL="$nproc"; 	mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf; 		make install; 		cd /; 	rm -rf /usr/src/memcached; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		memcached -V # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 04 Dec 2023 18:08:47 GMT
USER memcache
# Mon, 04 Dec 2023 18:08:47 GMT
EXPOSE map[11211/tcp:{}]
# Mon, 04 Dec 2023 18:08:47 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:6daa625e5a040476e253e7acd0befa74254a4865ec836d6334a544d82a21d4be`  
		Last Modified: Tue, 21 Nov 2023 05:10:21 GMT  
		Size: 27.5 MB (27512885 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b19a3143cbec7ddc9a646dbbe779b0b5ec67662cf70e280db146f6ace54ccd61`  
		Last Modified: Wed, 13 Dec 2023 00:26:35 GMT  
		Size: 1.1 KB (1111 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b8af028b1fa76aa55f540dd5be5eaf89eea3fec23e09e9a88550aac36e9ee843`  
		Last Modified: Wed, 13 Dec 2023 00:26:35 GMT  
		Size: 2.2 MB (2152508 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9a774943469875a0902c53fccdd95cad9c18234b759bcdcc5816bd563deb7f14`  
		Last Modified: Wed, 13 Dec 2023 00:26:35 GMT  
		Size: 8.4 MB (8374880 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:266b4bf499a815da6f7ddcf68e1e61f8418c8ec655a2083e174aaa385de74d76`  
		Last Modified: Wed, 13 Dec 2023 00:26:35 GMT  
		Size: 284.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0da709e3482cc552b0a7b69eb05aaa21af1e74baaf4e3bccc34e95e478943630`  
		Last Modified: Wed, 13 Dec 2023 00:26:36 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1.6` - unknown; unknown

```console
$ docker pull memcached@sha256:525abad348ba03c5b9444f23409d647581284c1642d30539e2c9943405266f12
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 MB (3067303 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e3b551ec9122d039520bbd13bced5b1f5b0d5b1fd9e32c09a1d4536f7af1226`

```dockerfile
```

-	Layers:
	-	`sha256:5cc0958f61715f0746d9fa2a8a5c06f31608bb5d1cf32d606c46fc8e11b35984`  
		Last Modified: Wed, 13 Dec 2023 00:26:35 GMT  
		Size: 3.0 MB (3046353 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:3d2fed99d3355e42a820c1975105411eb7584cffb111d7e1fd541603f7721f1c`  
		Last Modified: Wed, 13 Dec 2023 00:26:35 GMT  
		Size: 20.9 KB (20950 bytes)  
		MIME: application/vnd.in-toto+json

## `memcached:1.6-alpine`

```console
$ docker pull memcached@sha256:9587ad270892c531bf1ac66f195312c2f0f374192e5ac79cf2dfc5dd7cd1555e
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

### `memcached:1.6-alpine` - linux; amd64

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

### `memcached:1.6-alpine` - unknown; unknown

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

### `memcached:1.6-alpine` - linux; arm variant v7

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

### `memcached:1.6-alpine` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:286df72d3172b8ed7793e7058f9327823d65bdac8a226a06a00d292c087ad9c2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.4 MB (4419383 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d682c07630240a305e61d9fe0b12e4dc6f338f6a6b2c95b0941b54b2b8509b75`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 08 Dec 2023 01:39:30 GMT
ADD file:8182c73f869a899cf624a59c400acb8226776d15e4d3a0d240a94e65340540d0 in / 
# Fri, 08 Dec 2023 01:39:30 GMT
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
	-	`sha256:c303524923177661067f7eb378c3dd5277088c2676ebd1cd78e68397bb80fdbf`  
		Last Modified: Fri, 08 Dec 2023 01:39:48 GMT  
		Size: 3.3 MB (3347794 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:dfede01b081f27465377bdafbbdb6b694c6fab18026972b2c380535dcef103b8`  
		Last Modified: Wed, 13 Dec 2023 01:35:47 GMT  
		Size: 1.2 KB (1246 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b6d7b6f4ad45bf3aee58c5a7e8083286bd79dc004840903fd5997929772bfb4c`  
		Last Modified: Wed, 13 Dec 2023 01:35:47 GMT  
		Size: 120.9 KB (120897 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:64a4d385fe9c52ce74fd893218a806a70ac60ff0c57a80c1b3e43096c1f9ebc0`  
		Last Modified: Wed, 13 Dec 2023 01:35:48 GMT  
		Size: 949.0 KB (949044 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fd5239ae2cadceed6ddca34da081735d9a9d40ec7e5bdded8b5faca81fb0a070`  
		Last Modified: Wed, 13 Dec 2023 01:35:48 GMT  
		Size: 282.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4ab0568624eca639b58ae572fcf8e82d6fb6cb3d9f6ca5d7df2b7329747dedd4`  
		Last Modified: Wed, 13 Dec 2023 01:35:49 GMT  
		Size: 120.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1.6-alpine` - unknown; unknown

```console
$ docker pull memcached@sha256:6f8a1e61dcc0fd492cbafc5fd2b4c22d6154464b462857003e8e48a48305823a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **98.1 KB (98108 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ffc7ff6f7a07bd49a0241faf0b1957add37ce71b17cbdf2c878e4fc78cdc7bc4`

```dockerfile
```

-	Layers:
	-	`sha256:a9702aa1523d9e76bf98e50205b92ccf5d5bee944388fa4b376abeae8048c7d5`  
		Last Modified: Wed, 13 Dec 2023 01:35:48 GMT  
		Size: 78.6 KB (78622 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:3a49d198124cd7443d92b69a3737a232e2d6e7c626eb726c2902193c31acd5bd`  
		Last Modified: Wed, 13 Dec 2023 01:35:47 GMT  
		Size: 19.5 KB (19486 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:1.6-alpine` - linux; 386

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

### `memcached:1.6-alpine` - unknown; unknown

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

### `memcached:1.6-alpine` - linux; ppc64le

```console
$ docker pull memcached@sha256:06711fbe2ddda329f14ab4a0825494b32336140e6a0e3b6c4d879adc475857c3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4468374 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09b1d12275d18bb3dac772e05585652308aa081f1aeae540381aea1c9ed321bd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 08 Dec 2023 01:22:51 GMT
ADD file:052421189f8d269382daaaa8beb63c687e4d8ca908c421abdce53bcc627a40b4 in / 
# Fri, 08 Dec 2023 01:22:51 GMT
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
	-	`sha256:243ac51c334a47917a84be93e972ee6378987e9b3b917a5a8df29025e161c1f3`  
		Last Modified: Fri, 08 Dec 2023 01:23:14 GMT  
		Size: 3.4 MB (3358233 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:add73e7dbebd6c86078686bb046ef57017b090fe917f656feb83ec0ef971b5f3`  
		Last Modified: Tue, 12 Dec 2023 23:20:17 GMT  
		Size: 1.2 KB (1243 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d64bed657a7e728633e13f2021b35954e98be9ecae77096d30cdaa1d9260d61e`  
		Last Modified: Tue, 12 Dec 2023 23:20:17 GMT  
		Size: 123.4 KB (123403 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1b7a39c0f73f39f740b607f200570edf13046db40879e4aebbdca9e2fd273b0f`  
		Last Modified: Tue, 12 Dec 2023 23:20:17 GMT  
		Size: 985.1 KB (985092 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ad6306836cf70172b90d6b82bffc8546c005c16cda9b7d58dc5dbd386b7ee7d8`  
		Last Modified: Tue, 12 Dec 2023 23:20:17 GMT  
		Size: 281.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:71e3eb1fb10d08825521650c7c7ddedf3cfce2f976e93c18ab11aace23c38be5`  
		Last Modified: Tue, 12 Dec 2023 23:20:18 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1.6-alpine` - unknown; unknown

```console
$ docker pull memcached@sha256:65ba466bf93c49f07fd340ced359d51a13a74b069cca4de2d034d12f42b92ea4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **96.4 KB (96395 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0e68093b9e036b2a9ff696038b0fd906f66504c0a0cd70dda18954ebb93d4bd1`

```dockerfile
```

-	Layers:
	-	`sha256:b64631288cf2d05d3a1d99eb8cb41f077724b027aaf136bb327f88055e4ceaf4`  
		Last Modified: Tue, 12 Dec 2023 23:20:17 GMT  
		Size: 77.0 KB (77025 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:8ac9ea640f8ca624c147fd0dcc40f859a6284e5f50c4396e0b1e962a4b732813`  
		Last Modified: Tue, 12 Dec 2023 23:20:17 GMT  
		Size: 19.4 KB (19370 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:1.6-alpine` - linux; s390x

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

### `memcached:1.6-alpine` - unknown; unknown

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

## `memcached:1.6-alpine3.19`

```console
$ docker pull memcached@sha256:fc05162ae59e353d64bc065f589df156b875b48ac0d9c6bab788e9a2a2e400ca
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 8
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown
	-	linux; ppc64le
	-	unknown; unknown
	-	linux; s390x
	-	unknown; unknown

### `memcached:1.6-alpine3.19` - linux; amd64

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

### `memcached:1.6-alpine3.19` - unknown; unknown

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

### `memcached:1.6-alpine3.19` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:286df72d3172b8ed7793e7058f9327823d65bdac8a226a06a00d292c087ad9c2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.4 MB (4419383 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d682c07630240a305e61d9fe0b12e4dc6f338f6a6b2c95b0941b54b2b8509b75`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 08 Dec 2023 01:39:30 GMT
ADD file:8182c73f869a899cf624a59c400acb8226776d15e4d3a0d240a94e65340540d0 in / 
# Fri, 08 Dec 2023 01:39:30 GMT
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
	-	`sha256:c303524923177661067f7eb378c3dd5277088c2676ebd1cd78e68397bb80fdbf`  
		Last Modified: Fri, 08 Dec 2023 01:39:48 GMT  
		Size: 3.3 MB (3347794 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:dfede01b081f27465377bdafbbdb6b694c6fab18026972b2c380535dcef103b8`  
		Last Modified: Wed, 13 Dec 2023 01:35:47 GMT  
		Size: 1.2 KB (1246 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b6d7b6f4ad45bf3aee58c5a7e8083286bd79dc004840903fd5997929772bfb4c`  
		Last Modified: Wed, 13 Dec 2023 01:35:47 GMT  
		Size: 120.9 KB (120897 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:64a4d385fe9c52ce74fd893218a806a70ac60ff0c57a80c1b3e43096c1f9ebc0`  
		Last Modified: Wed, 13 Dec 2023 01:35:48 GMT  
		Size: 949.0 KB (949044 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fd5239ae2cadceed6ddca34da081735d9a9d40ec7e5bdded8b5faca81fb0a070`  
		Last Modified: Wed, 13 Dec 2023 01:35:48 GMT  
		Size: 282.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4ab0568624eca639b58ae572fcf8e82d6fb6cb3d9f6ca5d7df2b7329747dedd4`  
		Last Modified: Wed, 13 Dec 2023 01:35:49 GMT  
		Size: 120.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1.6-alpine3.19` - unknown; unknown

```console
$ docker pull memcached@sha256:6f8a1e61dcc0fd492cbafc5fd2b4c22d6154464b462857003e8e48a48305823a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **98.1 KB (98108 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ffc7ff6f7a07bd49a0241faf0b1957add37ce71b17cbdf2c878e4fc78cdc7bc4`

```dockerfile
```

-	Layers:
	-	`sha256:a9702aa1523d9e76bf98e50205b92ccf5d5bee944388fa4b376abeae8048c7d5`  
		Last Modified: Wed, 13 Dec 2023 01:35:48 GMT  
		Size: 78.6 KB (78622 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:3a49d198124cd7443d92b69a3737a232e2d6e7c626eb726c2902193c31acd5bd`  
		Last Modified: Wed, 13 Dec 2023 01:35:47 GMT  
		Size: 19.5 KB (19486 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:1.6-alpine3.19` - linux; ppc64le

```console
$ docker pull memcached@sha256:06711fbe2ddda329f14ab4a0825494b32336140e6a0e3b6c4d879adc475857c3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4468374 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09b1d12275d18bb3dac772e05585652308aa081f1aeae540381aea1c9ed321bd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 08 Dec 2023 01:22:51 GMT
ADD file:052421189f8d269382daaaa8beb63c687e4d8ca908c421abdce53bcc627a40b4 in / 
# Fri, 08 Dec 2023 01:22:51 GMT
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
	-	`sha256:243ac51c334a47917a84be93e972ee6378987e9b3b917a5a8df29025e161c1f3`  
		Last Modified: Fri, 08 Dec 2023 01:23:14 GMT  
		Size: 3.4 MB (3358233 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:add73e7dbebd6c86078686bb046ef57017b090fe917f656feb83ec0ef971b5f3`  
		Last Modified: Tue, 12 Dec 2023 23:20:17 GMT  
		Size: 1.2 KB (1243 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d64bed657a7e728633e13f2021b35954e98be9ecae77096d30cdaa1d9260d61e`  
		Last Modified: Tue, 12 Dec 2023 23:20:17 GMT  
		Size: 123.4 KB (123403 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1b7a39c0f73f39f740b607f200570edf13046db40879e4aebbdca9e2fd273b0f`  
		Last Modified: Tue, 12 Dec 2023 23:20:17 GMT  
		Size: 985.1 KB (985092 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ad6306836cf70172b90d6b82bffc8546c005c16cda9b7d58dc5dbd386b7ee7d8`  
		Last Modified: Tue, 12 Dec 2023 23:20:17 GMT  
		Size: 281.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:71e3eb1fb10d08825521650c7c7ddedf3cfce2f976e93c18ab11aace23c38be5`  
		Last Modified: Tue, 12 Dec 2023 23:20:18 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1.6-alpine3.19` - unknown; unknown

```console
$ docker pull memcached@sha256:65ba466bf93c49f07fd340ced359d51a13a74b069cca4de2d034d12f42b92ea4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **96.4 KB (96395 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0e68093b9e036b2a9ff696038b0fd906f66504c0a0cd70dda18954ebb93d4bd1`

```dockerfile
```

-	Layers:
	-	`sha256:b64631288cf2d05d3a1d99eb8cb41f077724b027aaf136bb327f88055e4ceaf4`  
		Last Modified: Tue, 12 Dec 2023 23:20:17 GMT  
		Size: 77.0 KB (77025 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:8ac9ea640f8ca624c147fd0dcc40f859a6284e5f50c4396e0b1e962a4b732813`  
		Last Modified: Tue, 12 Dec 2023 23:20:17 GMT  
		Size: 19.4 KB (19370 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:1.6-alpine3.19` - linux; s390x

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

### `memcached:1.6-alpine3.19` - unknown; unknown

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

## `memcached:1.6-bookworm`

```console
$ docker pull memcached@sha256:5006d1a9ea8a2cedd728d75c2e85cb26c96489f6a039d14ba2c44f99ea310d1c
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 14
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm variant v5
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown
	-	linux; 386
	-	unknown; unknown
	-	linux; mips64le
	-	unknown; unknown
	-	linux; ppc64le
	-	unknown; unknown
	-	linux; s390x
	-	unknown; unknown

### `memcached:1.6-bookworm` - linux; amd64

```console
$ docker pull memcached@sha256:0d358fa0198562aa3d1e1c3e9386e1835256875517d8a4786f3dd50a1f65f1de
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.1 MB (41125606 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:03bad2c21b5df5c82f8c581ebec403482a3e00c0f35697ca669c46a7d000a13d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 21 Nov 2023 05:21:37 GMT
ADD file:d261a6f6921593f1e0b3f472ab1b1822e2c6deb0b369200f0b3370556bfad017 in / 
# Tue, 21 Nov 2023 05:21:37 GMT
CMD ["bash"]
# Mon, 04 Dec 2023 18:08:47 GMT
RUN set -eux; 	groupadd --system --gid 11211 memcache; 	useradd --system --gid memcache --uid 11211 memcache # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
ENV MEMCACHED_VERSION=1.6.22
# Mon, 04 Dec 2023 18:08:47 GMT
ENV MEMCACHED_URL=https://memcached.org/files/memcached-1.6.22.tar.gz
# Mon, 04 Dec 2023 18:08:47 GMT
ENV MEMCACHED_SHA1=7a691f390d59616dbebfc9e2e4942d499c39a338
# Mon, 04 Dec 2023 18:08:47 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O memcached.tar.gz "$MEMCACHED_URL"; 	echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c -; 	mkdir -p /usr/src/memcached; 	tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1; 	rm memcached.tar.gz; 		cd /usr/src/memcached; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	; 	nproc="$(nproc)"; 	make -j "$nproc"; 		sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf; 	make test PARALLEL="$nproc"; 	mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf; 		make install; 		cd /; 	rm -rf /usr/src/memcached; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		memcached -V # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 04 Dec 2023 18:08:47 GMT
USER memcache
# Mon, 04 Dec 2023 18:08:47 GMT
EXPOSE map[11211/tcp:{}]
# Mon, 04 Dec 2023 18:08:47 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:1f7ce2fa46ab3942feabee654933948821303a5a821789dddab2d8c3df59e227`  
		Last Modified: Tue, 21 Nov 2023 05:25:58 GMT  
		Size: 29.1 MB (29149908 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:21ac6fd160890cbc46a76542eb3f68654f3e3fb043b1b28a18155ec6863d60bc`  
		Last Modified: Tue, 12 Dec 2023 20:52:57 GMT  
		Size: 1.1 KB (1112 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6330fc82e1304befcc27a7598cd1a85152985d06426f94966788bf5a1583dcc6`  
		Last Modified: Tue, 12 Dec 2023 20:52:57 GMT  
		Size: 2.5 MB (2488284 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4047c827380f04698fbc51155441d719f93b84c1a092d633260c704f286296dd`  
		Last Modified: Tue, 12 Dec 2023 20:52:57 GMT  
		Size: 9.5 MB (9485895 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:401b5de2a4f8d9f588888754fa8347b67590c776363770f46ef67688116a4a0c`  
		Last Modified: Tue, 12 Dec 2023 20:52:57 GMT  
		Size: 285.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ee899f9aed95096580ea4a2325fd4824518ff1621f433f393fa253b52b7294b5`  
		Last Modified: Tue, 12 Dec 2023 20:52:58 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1.6-bookworm` - unknown; unknown

```console
$ docker pull memcached@sha256:5ccb88c1a86bd6524b6d5c9383254cdd79314d656a0c982658ecd35d9716431b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 MB (3077929 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:238ef9023561adc9c09faf875c5370cb2711a83cc7327dcc49ae7f8255c23794`

```dockerfile
```

-	Layers:
	-	`sha256:f84a6f3d0bdab8613be68ff091a6a78bedf8f697d4df55ff90ac7b745337e72c`  
		Last Modified: Tue, 12 Dec 2023 20:52:57 GMT  
		Size: 3.1 MB (3056812 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:8d7aee053ab87a86e42ba3d14810d3f1918c6e66d4d3ef02bc9c741f3948b83e`  
		Last Modified: Tue, 12 Dec 2023 20:52:57 GMT  
		Size: 21.1 KB (21117 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:1.6-bookworm` - linux; arm variant v5

```console
$ docker pull memcached@sha256:cb9426984b18b2d3df1c5fbb2bb7e2e9ebe08325d4adce6d0cd7a9207c413476
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.1 MB (37113170 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a8f2fb6119b629983f190d8b73208a156991d8cb65c47579a68125c339e9c75`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 21 Nov 2023 05:00:51 GMT
ADD file:1ae8e5ac45b11d01083680b765e1fcfef9f7938f89d6f424572126fa946d8cdf in / 
# Tue, 21 Nov 2023 05:00:52 GMT
CMD ["bash"]
# Mon, 04 Dec 2023 18:08:47 GMT
RUN set -eux; 	groupadd --system --gid 11211 memcache; 	useradd --system --gid memcache --uid 11211 memcache # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
ENV MEMCACHED_VERSION=1.6.22
# Mon, 04 Dec 2023 18:08:47 GMT
ENV MEMCACHED_URL=https://memcached.org/files/memcached-1.6.22.tar.gz
# Mon, 04 Dec 2023 18:08:47 GMT
ENV MEMCACHED_SHA1=7a691f390d59616dbebfc9e2e4942d499c39a338
# Mon, 04 Dec 2023 18:08:47 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O memcached.tar.gz "$MEMCACHED_URL"; 	echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c -; 	mkdir -p /usr/src/memcached; 	tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1; 	rm memcached.tar.gz; 		cd /usr/src/memcached; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	; 	nproc="$(nproc)"; 	make -j "$nproc"; 		sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf; 	make test PARALLEL="$nproc"; 	mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf; 		make install; 		cd /; 	rm -rf /usr/src/memcached; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		memcached -V # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 04 Dec 2023 18:08:47 GMT
USER memcache
# Mon, 04 Dec 2023 18:08:47 GMT
EXPOSE map[11211/tcp:{}]
# Mon, 04 Dec 2023 18:08:47 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:f476aef5b6e1122850e68c81ef06fc2df17e968961b060483b4d2fb33018aae3`  
		Last Modified: Tue, 21 Nov 2023 05:03:55 GMT  
		Size: 26.9 MB (26922153 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:89367ca16d2c3104d44514e1b9b94b0ac4070ea0f6f04523c72dda62795f3a17`  
		Last Modified: Tue, 12 Dec 2023 21:47:13 GMT  
		Size: 1.1 KB (1110 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5ecbc6577cf78c09bd4136f78a57a904ae1ab705fce8595e8d1187d800158e6f`  
		Last Modified: Tue, 12 Dec 2023 21:47:14 GMT  
		Size: 2.1 MB (2089289 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:12f8a270079b04e1372c73cc16ff2ae33e6f6ee0dcc7e8ed57843fca20b3d038`  
		Last Modified: Tue, 12 Dec 2023 21:47:14 GMT  
		Size: 8.1 MB (8100211 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5f592556023f9ba6125ecf6b89156ba61c05526ad324708c3d2a09600ee5e7e4`  
		Last Modified: Tue, 12 Dec 2023 21:47:14 GMT  
		Size: 285.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fa757a09f6a7a23114a13869f15b229384628cf108567d395dc0d4730c685409`  
		Last Modified: Tue, 12 Dec 2023 21:47:14 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1.6-bookworm` - unknown; unknown

```console
$ docker pull memcached@sha256:0c93e2660a508733f1c7d5236af77ef81fbcd0b27e4ac55c81d83334c8794891
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.0 KB (21043 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:538fbf714aa2f8a4175400dd43b0715e416f73fe598fc50d3f763afa144595da`

```dockerfile
```

-	Layers:
	-	`sha256:f65b3a9a0f6936cae3c1e411ecdd846d754a1978d851fdacf4b25526cb9ff4cc`  
		Last Modified: Tue, 12 Dec 2023 21:47:14 GMT  
		Size: 21.0 KB (21043 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:1.6-bookworm` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:c5adc5a4207d95c96a36131c2d39085b082f0e22f4595b935e72bcb463c10383
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.0 MB (39979924 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf26c17403ed5a4db96ddd8b41aeb2fd45483f897882a57972c994c95a44c5dd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 21 Nov 2023 06:27:06 GMT
ADD file:869c7d0747a17c53715581a2e862992eb8516c7f45f167821dfa80966a4870d1 in / 
# Tue, 21 Nov 2023 06:27:06 GMT
CMD ["bash"]
# Mon, 04 Dec 2023 18:08:47 GMT
RUN set -eux; 	groupadd --system --gid 11211 memcache; 	useradd --system --gid memcache --uid 11211 memcache # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
ENV MEMCACHED_VERSION=1.6.22
# Mon, 04 Dec 2023 18:08:47 GMT
ENV MEMCACHED_URL=https://memcached.org/files/memcached-1.6.22.tar.gz
# Mon, 04 Dec 2023 18:08:47 GMT
ENV MEMCACHED_SHA1=7a691f390d59616dbebfc9e2e4942d499c39a338
# Mon, 04 Dec 2023 18:08:47 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O memcached.tar.gz "$MEMCACHED_URL"; 	echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c -; 	mkdir -p /usr/src/memcached; 	tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1; 	rm memcached.tar.gz; 		cd /usr/src/memcached; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	; 	nproc="$(nproc)"; 	make -j "$nproc"; 		sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf; 	make test PARALLEL="$nproc"; 	mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf; 		make install; 		cd /; 	rm -rf /usr/src/memcached; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		memcached -V # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 04 Dec 2023 18:08:47 GMT
USER memcache
# Mon, 04 Dec 2023 18:08:47 GMT
EXPOSE map[11211/tcp:{}]
# Mon, 04 Dec 2023 18:08:47 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:2c6d21737d8318aa15c4cc838475029a5efc36c0429e3d8da80d97d0b96d9aaf`  
		Last Modified: Tue, 21 Nov 2023 06:30:30 GMT  
		Size: 29.2 MB (29179277 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1a39d6fec0d552a8078ab223bafd58bc9a0c8c27c26600a5b95c6a521bb97f3d`  
		Last Modified: Tue, 12 Dec 2023 23:43:17 GMT  
		Size: 1.1 KB (1112 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9d1ceea69964553dd3aaf853e0d7b753495cab4623b9377c69096be0bdf88146`  
		Last Modified: Tue, 12 Dec 2023 23:43:17 GMT  
		Size: 2.3 MB (2345975 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:52063b8e37cbc1e5e6e3af0f54b834ae3f6a53d023349ae819c9607e5fc98aec`  
		Last Modified: Tue, 12 Dec 2023 23:43:17 GMT  
		Size: 8.5 MB (8453155 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5b99d0095a64f8110efee1f5e91754cc923294d50c9e2927e515354746a3f465`  
		Last Modified: Tue, 12 Dec 2023 23:43:17 GMT  
		Size: 284.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:913c9e21eaa9c49c99b1b39e5cda0ef12356220075c869ea4776dca36fe83b75`  
		Last Modified: Tue, 12 Dec 2023 23:43:18 GMT  
		Size: 121.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1.6-bookworm` - unknown; unknown

```console
$ docker pull memcached@sha256:3d519a2eb9e00b43e6bc7584f6962b12ba032c4487a6e4ef7fd2b00b667bc90d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 MB (3053138 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9cc25288d58197dcc1309ea4a8128d0b120b92ad2d877f226095cd4847696474`

```dockerfile
```

-	Layers:
	-	`sha256:c5edc5ba98b4e6a438caa0d4541784c5c1e8b23d6020bc0b2a5b9910d0725400`  
		Last Modified: Tue, 12 Dec 2023 23:43:17 GMT  
		Size: 3.0 MB (3032003 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:b15e35765293b6f1da0e628c94108f229423c5a6379b8b5c47a41415f377b6d8`  
		Last Modified: Tue, 12 Dec 2023 23:43:17 GMT  
		Size: 21.1 KB (21135 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:1.6-bookworm` - linux; 386

```console
$ docker pull memcached@sha256:fa9dba8086765d68f2feecfc2ac08fb29c019597d09943bb480227e6cba87666
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.3 MB (39294993 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:93047050e75b6d4d64adb8a7c8f68cb118bad27ca9dc772120e251b174752cf9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 16 Oct 2023 06:54:12 GMT
ADD file:0c94521fdd9c0a4fdeeb9aad23e68cd053fba0dcd7c3af550aefa79377816e31 in / 
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["bash"]
# Mon, 16 Oct 2023 06:54:12 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_VERSION=1.6.22
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_SHA1=7a691f390d59616dbebfc9e2e4942d499c39a338
# Mon, 16 Oct 2023 06:54:12 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V # buildkit
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
	-	`sha256:98bdfce9af831c2a0d0bfcca812d0039cd1666986550f552b4b4c625bd5aa31c`  
		Last Modified: Wed, 01 Nov 2023 00:43:26 GMT  
		Size: 30.2 MB (30164042 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1b647d4b10cf20ac5807101c7d0380701be684aa82f5c01ec41f674b5ef23d42`  
		Last Modified: Wed, 01 Nov 2023 01:06:49 GMT  
		Size: 1.1 KB (1109 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b61c058003459de4911c2901b2d799b03de754a1b9e64ffbe21a04992e962e62`  
		Last Modified: Wed, 01 Nov 2023 01:06:49 GMT  
		Size: 2.5 MB (2492501 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:810b6db64df2fcc8f76941cdac75093cf35bd72ac3cd1fa5eb664e74c1f67cd8`  
		Last Modified: Wed, 01 Nov 2023 01:06:50 GMT  
		Size: 6.6 MB (6636937 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:dbb899942df4149bd5fae8bac6e295285ec80f82d621f2b29c931ee348491cfb`  
		Last Modified: Wed, 01 Nov 2023 01:06:49 GMT  
		Size: 282.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4a8530160ab232c37c0ddcbf5e3a731d835d378d1382843957f6c2a73b2b5be6`  
		Last Modified: Wed, 01 Nov 2023 01:06:50 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1.6-bookworm` - unknown; unknown

```console
$ docker pull memcached@sha256:dd7ce9519c31365127142232df2ed0b285e9acc03cd77c23c838bf932165def8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.5 KB (21498 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eef82c92e07c11a92c337806d01cfb1c6cdc7a16608dcf304a38de34d2ef1dbb`

```dockerfile
```

-	Layers:
	-	`sha256:c0d9dd22513f8d3e791e1796d7ef1906e57c798c92dd35d0be9cf2eaecec5954`  
		Last Modified: Wed, 01 Nov 2023 01:06:49 GMT  
		Size: 21.5 KB (21498 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:1.6-bookworm` - linux; mips64le

```console
$ docker pull memcached@sha256:9f7696d5078cf83e8b152cb00a3615576fd3c50d10be9253b9c188e16bfd8087
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.9 MB (39863164 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:685886644cfb343923260c15c66eb8c8d8bf7b84b6b1e855732aec2359b6ae29`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 21 Nov 2023 04:09:50 GMT
ADD file:e093749192323dc72b60a8440ddba26c415586f618b5e107fa264ba5eb2ca7ba in / 
# Tue, 21 Nov 2023 04:09:54 GMT
CMD ["bash"]
# Mon, 04 Dec 2023 18:08:47 GMT
RUN set -eux; 	groupadd --system --gid 11211 memcache; 	useradd --system --gid memcache --uid 11211 memcache # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
ENV MEMCACHED_VERSION=1.6.22
# Mon, 04 Dec 2023 18:08:47 GMT
ENV MEMCACHED_URL=https://memcached.org/files/memcached-1.6.22.tar.gz
# Mon, 04 Dec 2023 18:08:47 GMT
ENV MEMCACHED_SHA1=7a691f390d59616dbebfc9e2e4942d499c39a338
# Mon, 04 Dec 2023 18:08:47 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O memcached.tar.gz "$MEMCACHED_URL"; 	echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c -; 	mkdir -p /usr/src/memcached; 	tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1; 	rm memcached.tar.gz; 		cd /usr/src/memcached; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	; 	nproc="$(nproc)"; 	make -j "$nproc"; 		sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf; 	make test PARALLEL="$nproc"; 	mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf; 		make install; 		cd /; 	rm -rf /usr/src/memcached; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		memcached -V # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 04 Dec 2023 18:08:47 GMT
USER memcache
# Mon, 04 Dec 2023 18:08:47 GMT
EXPOSE map[11211/tcp:{}]
# Mon, 04 Dec 2023 18:08:47 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:ebdff2138fee4a3ec27560ab1353dc51c12c2608ff721f5db3d24104872b702a`  
		Last Modified: Tue, 21 Nov 2023 04:20:35 GMT  
		Size: 29.1 MB (29141984 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ee63ae82c6a87dc28cedafb91fbd6eaccd22add5b00a9cceb208472b30427b5d`  
		Last Modified: Tue, 12 Dec 2023 23:10:03 GMT  
		Size: 1.1 KB (1114 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3d430991f88102b07bcf8bf22f07667e49c9dfedb134b0ac36ddbb99d1e79db2`  
		Last Modified: Tue, 12 Dec 2023 23:10:04 GMT  
		Size: 1.9 MB (1937475 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ebe1140b392e915b8757b8d0a4b83f0aaf2103734e9f83c318821f641207b6b4`  
		Last Modified: Tue, 12 Dec 2023 23:10:04 GMT  
		Size: 8.8 MB (8782185 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:aedf1130e49a6aa7d9b74b9fd00914b171966fcf8beba71095787811fa3a0284`  
		Last Modified: Tue, 12 Dec 2023 23:10:03 GMT  
		Size: 284.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:457e2691e0499a1a1d26e6da85567f20a8dc396bde9d9952ce75fdcfe6cbafd8`  
		Last Modified: Tue, 12 Dec 2023 23:10:05 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1.6-bookworm` - unknown; unknown

```console
$ docker pull memcached@sha256:d48752667ff111ef73342ae5c16218a373275e8b65c7696eff231ff49ca7b8e5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.0 KB (21004 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9138b1207d88c6ca6b32a2616d3c25b1f5d3280b7650ac4bfa7120518f6a8ad7`

```dockerfile
```

-	Layers:
	-	`sha256:2b1c5f3190ac8dfdff54a51d9421ad623af991deba1a46ba943cf88442079207`  
		Last Modified: Tue, 12 Dec 2023 23:10:03 GMT  
		Size: 21.0 KB (21004 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:1.6-bookworm` - linux; ppc64le

```console
$ docker pull memcached@sha256:813f2ed7d8d4d2c4e6f4a19816964b0c95cc56d038d95d059571d51e115ab109
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.5 MB (45508655 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:73c79988c4d09a9ac9cb01aa05096b344821e8034c3cba04afb9cb78fe25db05`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 21 Nov 2023 04:24:14 GMT
ADD file:8b22a531b6611a1e63dfc20e4e2931592e2d821bd4b64c4b2810bb9a36640c02 in / 
# Tue, 21 Nov 2023 04:24:16 GMT
CMD ["bash"]
# Mon, 04 Dec 2023 18:08:47 GMT
RUN set -eux; 	groupadd --system --gid 11211 memcache; 	useradd --system --gid memcache --uid 11211 memcache # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
ENV MEMCACHED_VERSION=1.6.22
# Mon, 04 Dec 2023 18:08:47 GMT
ENV MEMCACHED_URL=https://memcached.org/files/memcached-1.6.22.tar.gz
# Mon, 04 Dec 2023 18:08:47 GMT
ENV MEMCACHED_SHA1=7a691f390d59616dbebfc9e2e4942d499c39a338
# Mon, 04 Dec 2023 18:08:47 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O memcached.tar.gz "$MEMCACHED_URL"; 	echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c -; 	mkdir -p /usr/src/memcached; 	tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1; 	rm memcached.tar.gz; 		cd /usr/src/memcached; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	; 	nproc="$(nproc)"; 	make -j "$nproc"; 		sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf; 	make test PARALLEL="$nproc"; 	mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf; 		make install; 		cd /; 	rm -rf /usr/src/memcached; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		memcached -V # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 04 Dec 2023 18:08:47 GMT
USER memcache
# Mon, 04 Dec 2023 18:08:47 GMT
EXPOSE map[11211/tcp:{}]
# Mon, 04 Dec 2023 18:08:47 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:c570d04e61d8e35a3c8f12179d048d701451f97f9cf2099ea3e3738512dbf062`  
		Last Modified: Tue, 21 Nov 2023 04:28:58 GMT  
		Size: 33.1 MB (33141607 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b53469d03d0156e89526c2b744f6850b65cfb9b509a6fda4c523764f7a9f9072`  
		Last Modified: Tue, 12 Dec 2023 23:08:09 GMT  
		Size: 1.1 KB (1111 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:12b61a5974195d80345022ed47cb4546f6fec60527b3932b2ce74d605db750e0`  
		Last Modified: Tue, 12 Dec 2023 23:08:09 GMT  
		Size: 2.7 MB (2698202 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:108f5df7a0010e4f69929c6ce4ff2e0e53877c6bbe11bd86acbbb0e7b608dca7`  
		Last Modified: Tue, 12 Dec 2023 23:08:09 GMT  
		Size: 9.7 MB (9667330 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:aa53d1e0a6b1123a31838e581de8d738ccaf05c9be569ec50b8d37cbc54a99bd`  
		Last Modified: Tue, 12 Dec 2023 23:08:08 GMT  
		Size: 283.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2cf8ef0b438a2029bfc9b928364eb71966baa4990e2ac4a9b1648cbd44271dc4`  
		Last Modified: Tue, 12 Dec 2023 23:08:10 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1.6-bookworm` - unknown; unknown

```console
$ docker pull memcached@sha256:d75efc7b8726fbfade0b41c14205058def09ee997a7befb495808c2752a56a54
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 MB (3066416 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ca8bb0be2316bb58a60c953382dd1963eb7e265d0602de370e02152e1ac84d7`

```dockerfile
```

-	Layers:
	-	`sha256:34203b346608565cdbcd7cf9a56efb8ec2255b1a8f30267d6b2749d6a0bd2d6b`  
		Last Modified: Tue, 12 Dec 2023 23:08:09 GMT  
		Size: 3.0 MB (3045398 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:4da4f2a55f1773bfac75983e2e733c609b970884e935de987ec5b3ec5c92eb85`  
		Last Modified: Tue, 12 Dec 2023 23:08:08 GMT  
		Size: 21.0 KB (21018 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:1.6-bookworm` - linux; s390x

```console
$ docker pull memcached@sha256:05084fffc798db32442e2cde93eac5815ffd909e9bf65692ac08c9b5ab79e677
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.0 MB (38041790 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eac80baab625f3daf940cdb3053e2e709bd61d78d7eae50b7db4d71f87bcd149`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 21 Nov 2023 05:04:35 GMT
ADD file:c33fa9fdde73983850798b6eb1cd062e0398109d1d773e6a937fead7475c8efc in / 
# Tue, 21 Nov 2023 05:04:41 GMT
CMD ["bash"]
# Mon, 04 Dec 2023 18:08:47 GMT
RUN set -eux; 	groupadd --system --gid 11211 memcache; 	useradd --system --gid memcache --uid 11211 memcache # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
ENV MEMCACHED_VERSION=1.6.22
# Mon, 04 Dec 2023 18:08:47 GMT
ENV MEMCACHED_URL=https://memcached.org/files/memcached-1.6.22.tar.gz
# Mon, 04 Dec 2023 18:08:47 GMT
ENV MEMCACHED_SHA1=7a691f390d59616dbebfc9e2e4942d499c39a338
# Mon, 04 Dec 2023 18:08:47 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O memcached.tar.gz "$MEMCACHED_URL"; 	echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c -; 	mkdir -p /usr/src/memcached; 	tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1; 	rm memcached.tar.gz; 		cd /usr/src/memcached; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	; 	nproc="$(nproc)"; 	make -j "$nproc"; 		sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf; 	make test PARALLEL="$nproc"; 	mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf; 		make install; 		cd /; 	rm -rf /usr/src/memcached; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		memcached -V # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 04 Dec 2023 18:08:47 GMT
USER memcache
# Mon, 04 Dec 2023 18:08:47 GMT
EXPOSE map[11211/tcp:{}]
# Mon, 04 Dec 2023 18:08:47 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:6daa625e5a040476e253e7acd0befa74254a4865ec836d6334a544d82a21d4be`  
		Last Modified: Tue, 21 Nov 2023 05:10:21 GMT  
		Size: 27.5 MB (27512885 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b19a3143cbec7ddc9a646dbbe779b0b5ec67662cf70e280db146f6ace54ccd61`  
		Last Modified: Wed, 13 Dec 2023 00:26:35 GMT  
		Size: 1.1 KB (1111 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b8af028b1fa76aa55f540dd5be5eaf89eea3fec23e09e9a88550aac36e9ee843`  
		Last Modified: Wed, 13 Dec 2023 00:26:35 GMT  
		Size: 2.2 MB (2152508 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9a774943469875a0902c53fccdd95cad9c18234b759bcdcc5816bd563deb7f14`  
		Last Modified: Wed, 13 Dec 2023 00:26:35 GMT  
		Size: 8.4 MB (8374880 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:266b4bf499a815da6f7ddcf68e1e61f8418c8ec655a2083e174aaa385de74d76`  
		Last Modified: Wed, 13 Dec 2023 00:26:35 GMT  
		Size: 284.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0da709e3482cc552b0a7b69eb05aaa21af1e74baaf4e3bccc34e95e478943630`  
		Last Modified: Wed, 13 Dec 2023 00:26:36 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1.6-bookworm` - unknown; unknown

```console
$ docker pull memcached@sha256:525abad348ba03c5b9444f23409d647581284c1642d30539e2c9943405266f12
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 MB (3067303 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e3b551ec9122d039520bbd13bced5b1f5b0d5b1fd9e32c09a1d4536f7af1226`

```dockerfile
```

-	Layers:
	-	`sha256:5cc0958f61715f0746d9fa2a8a5c06f31608bb5d1cf32d606c46fc8e11b35984`  
		Last Modified: Wed, 13 Dec 2023 00:26:35 GMT  
		Size: 3.0 MB (3046353 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:3d2fed99d3355e42a820c1975105411eb7584cffb111d7e1fd541603f7721f1c`  
		Last Modified: Wed, 13 Dec 2023 00:26:35 GMT  
		Size: 20.9 KB (20950 bytes)  
		MIME: application/vnd.in-toto+json

## `memcached:1.6.22`

```console
$ docker pull memcached@sha256:5006d1a9ea8a2cedd728d75c2e85cb26c96489f6a039d14ba2c44f99ea310d1c
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 14
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm variant v5
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown
	-	linux; 386
	-	unknown; unknown
	-	linux; mips64le
	-	unknown; unknown
	-	linux; ppc64le
	-	unknown; unknown
	-	linux; s390x
	-	unknown; unknown

### `memcached:1.6.22` - linux; amd64

```console
$ docker pull memcached@sha256:0d358fa0198562aa3d1e1c3e9386e1835256875517d8a4786f3dd50a1f65f1de
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.1 MB (41125606 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:03bad2c21b5df5c82f8c581ebec403482a3e00c0f35697ca669c46a7d000a13d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 21 Nov 2023 05:21:37 GMT
ADD file:d261a6f6921593f1e0b3f472ab1b1822e2c6deb0b369200f0b3370556bfad017 in / 
# Tue, 21 Nov 2023 05:21:37 GMT
CMD ["bash"]
# Mon, 04 Dec 2023 18:08:47 GMT
RUN set -eux; 	groupadd --system --gid 11211 memcache; 	useradd --system --gid memcache --uid 11211 memcache # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
ENV MEMCACHED_VERSION=1.6.22
# Mon, 04 Dec 2023 18:08:47 GMT
ENV MEMCACHED_URL=https://memcached.org/files/memcached-1.6.22.tar.gz
# Mon, 04 Dec 2023 18:08:47 GMT
ENV MEMCACHED_SHA1=7a691f390d59616dbebfc9e2e4942d499c39a338
# Mon, 04 Dec 2023 18:08:47 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O memcached.tar.gz "$MEMCACHED_URL"; 	echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c -; 	mkdir -p /usr/src/memcached; 	tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1; 	rm memcached.tar.gz; 		cd /usr/src/memcached; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	; 	nproc="$(nproc)"; 	make -j "$nproc"; 		sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf; 	make test PARALLEL="$nproc"; 	mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf; 		make install; 		cd /; 	rm -rf /usr/src/memcached; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		memcached -V # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 04 Dec 2023 18:08:47 GMT
USER memcache
# Mon, 04 Dec 2023 18:08:47 GMT
EXPOSE map[11211/tcp:{}]
# Mon, 04 Dec 2023 18:08:47 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:1f7ce2fa46ab3942feabee654933948821303a5a821789dddab2d8c3df59e227`  
		Last Modified: Tue, 21 Nov 2023 05:25:58 GMT  
		Size: 29.1 MB (29149908 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:21ac6fd160890cbc46a76542eb3f68654f3e3fb043b1b28a18155ec6863d60bc`  
		Last Modified: Tue, 12 Dec 2023 20:52:57 GMT  
		Size: 1.1 KB (1112 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6330fc82e1304befcc27a7598cd1a85152985d06426f94966788bf5a1583dcc6`  
		Last Modified: Tue, 12 Dec 2023 20:52:57 GMT  
		Size: 2.5 MB (2488284 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4047c827380f04698fbc51155441d719f93b84c1a092d633260c704f286296dd`  
		Last Modified: Tue, 12 Dec 2023 20:52:57 GMT  
		Size: 9.5 MB (9485895 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:401b5de2a4f8d9f588888754fa8347b67590c776363770f46ef67688116a4a0c`  
		Last Modified: Tue, 12 Dec 2023 20:52:57 GMT  
		Size: 285.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ee899f9aed95096580ea4a2325fd4824518ff1621f433f393fa253b52b7294b5`  
		Last Modified: Tue, 12 Dec 2023 20:52:58 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1.6.22` - unknown; unknown

```console
$ docker pull memcached@sha256:5ccb88c1a86bd6524b6d5c9383254cdd79314d656a0c982658ecd35d9716431b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 MB (3077929 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:238ef9023561adc9c09faf875c5370cb2711a83cc7327dcc49ae7f8255c23794`

```dockerfile
```

-	Layers:
	-	`sha256:f84a6f3d0bdab8613be68ff091a6a78bedf8f697d4df55ff90ac7b745337e72c`  
		Last Modified: Tue, 12 Dec 2023 20:52:57 GMT  
		Size: 3.1 MB (3056812 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:8d7aee053ab87a86e42ba3d14810d3f1918c6e66d4d3ef02bc9c741f3948b83e`  
		Last Modified: Tue, 12 Dec 2023 20:52:57 GMT  
		Size: 21.1 KB (21117 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:1.6.22` - linux; arm variant v5

```console
$ docker pull memcached@sha256:cb9426984b18b2d3df1c5fbb2bb7e2e9ebe08325d4adce6d0cd7a9207c413476
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.1 MB (37113170 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a8f2fb6119b629983f190d8b73208a156991d8cb65c47579a68125c339e9c75`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 21 Nov 2023 05:00:51 GMT
ADD file:1ae8e5ac45b11d01083680b765e1fcfef9f7938f89d6f424572126fa946d8cdf in / 
# Tue, 21 Nov 2023 05:00:52 GMT
CMD ["bash"]
# Mon, 04 Dec 2023 18:08:47 GMT
RUN set -eux; 	groupadd --system --gid 11211 memcache; 	useradd --system --gid memcache --uid 11211 memcache # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
ENV MEMCACHED_VERSION=1.6.22
# Mon, 04 Dec 2023 18:08:47 GMT
ENV MEMCACHED_URL=https://memcached.org/files/memcached-1.6.22.tar.gz
# Mon, 04 Dec 2023 18:08:47 GMT
ENV MEMCACHED_SHA1=7a691f390d59616dbebfc9e2e4942d499c39a338
# Mon, 04 Dec 2023 18:08:47 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O memcached.tar.gz "$MEMCACHED_URL"; 	echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c -; 	mkdir -p /usr/src/memcached; 	tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1; 	rm memcached.tar.gz; 		cd /usr/src/memcached; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	; 	nproc="$(nproc)"; 	make -j "$nproc"; 		sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf; 	make test PARALLEL="$nproc"; 	mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf; 		make install; 		cd /; 	rm -rf /usr/src/memcached; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		memcached -V # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 04 Dec 2023 18:08:47 GMT
USER memcache
# Mon, 04 Dec 2023 18:08:47 GMT
EXPOSE map[11211/tcp:{}]
# Mon, 04 Dec 2023 18:08:47 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:f476aef5b6e1122850e68c81ef06fc2df17e968961b060483b4d2fb33018aae3`  
		Last Modified: Tue, 21 Nov 2023 05:03:55 GMT  
		Size: 26.9 MB (26922153 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:89367ca16d2c3104d44514e1b9b94b0ac4070ea0f6f04523c72dda62795f3a17`  
		Last Modified: Tue, 12 Dec 2023 21:47:13 GMT  
		Size: 1.1 KB (1110 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5ecbc6577cf78c09bd4136f78a57a904ae1ab705fce8595e8d1187d800158e6f`  
		Last Modified: Tue, 12 Dec 2023 21:47:14 GMT  
		Size: 2.1 MB (2089289 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:12f8a270079b04e1372c73cc16ff2ae33e6f6ee0dcc7e8ed57843fca20b3d038`  
		Last Modified: Tue, 12 Dec 2023 21:47:14 GMT  
		Size: 8.1 MB (8100211 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5f592556023f9ba6125ecf6b89156ba61c05526ad324708c3d2a09600ee5e7e4`  
		Last Modified: Tue, 12 Dec 2023 21:47:14 GMT  
		Size: 285.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fa757a09f6a7a23114a13869f15b229384628cf108567d395dc0d4730c685409`  
		Last Modified: Tue, 12 Dec 2023 21:47:14 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1.6.22` - unknown; unknown

```console
$ docker pull memcached@sha256:0c93e2660a508733f1c7d5236af77ef81fbcd0b27e4ac55c81d83334c8794891
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.0 KB (21043 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:538fbf714aa2f8a4175400dd43b0715e416f73fe598fc50d3f763afa144595da`

```dockerfile
```

-	Layers:
	-	`sha256:f65b3a9a0f6936cae3c1e411ecdd846d754a1978d851fdacf4b25526cb9ff4cc`  
		Last Modified: Tue, 12 Dec 2023 21:47:14 GMT  
		Size: 21.0 KB (21043 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:1.6.22` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:c5adc5a4207d95c96a36131c2d39085b082f0e22f4595b935e72bcb463c10383
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.0 MB (39979924 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf26c17403ed5a4db96ddd8b41aeb2fd45483f897882a57972c994c95a44c5dd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 21 Nov 2023 06:27:06 GMT
ADD file:869c7d0747a17c53715581a2e862992eb8516c7f45f167821dfa80966a4870d1 in / 
# Tue, 21 Nov 2023 06:27:06 GMT
CMD ["bash"]
# Mon, 04 Dec 2023 18:08:47 GMT
RUN set -eux; 	groupadd --system --gid 11211 memcache; 	useradd --system --gid memcache --uid 11211 memcache # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
ENV MEMCACHED_VERSION=1.6.22
# Mon, 04 Dec 2023 18:08:47 GMT
ENV MEMCACHED_URL=https://memcached.org/files/memcached-1.6.22.tar.gz
# Mon, 04 Dec 2023 18:08:47 GMT
ENV MEMCACHED_SHA1=7a691f390d59616dbebfc9e2e4942d499c39a338
# Mon, 04 Dec 2023 18:08:47 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O memcached.tar.gz "$MEMCACHED_URL"; 	echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c -; 	mkdir -p /usr/src/memcached; 	tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1; 	rm memcached.tar.gz; 		cd /usr/src/memcached; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	; 	nproc="$(nproc)"; 	make -j "$nproc"; 		sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf; 	make test PARALLEL="$nproc"; 	mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf; 		make install; 		cd /; 	rm -rf /usr/src/memcached; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		memcached -V # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 04 Dec 2023 18:08:47 GMT
USER memcache
# Mon, 04 Dec 2023 18:08:47 GMT
EXPOSE map[11211/tcp:{}]
# Mon, 04 Dec 2023 18:08:47 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:2c6d21737d8318aa15c4cc838475029a5efc36c0429e3d8da80d97d0b96d9aaf`  
		Last Modified: Tue, 21 Nov 2023 06:30:30 GMT  
		Size: 29.2 MB (29179277 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1a39d6fec0d552a8078ab223bafd58bc9a0c8c27c26600a5b95c6a521bb97f3d`  
		Last Modified: Tue, 12 Dec 2023 23:43:17 GMT  
		Size: 1.1 KB (1112 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9d1ceea69964553dd3aaf853e0d7b753495cab4623b9377c69096be0bdf88146`  
		Last Modified: Tue, 12 Dec 2023 23:43:17 GMT  
		Size: 2.3 MB (2345975 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:52063b8e37cbc1e5e6e3af0f54b834ae3f6a53d023349ae819c9607e5fc98aec`  
		Last Modified: Tue, 12 Dec 2023 23:43:17 GMT  
		Size: 8.5 MB (8453155 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5b99d0095a64f8110efee1f5e91754cc923294d50c9e2927e515354746a3f465`  
		Last Modified: Tue, 12 Dec 2023 23:43:17 GMT  
		Size: 284.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:913c9e21eaa9c49c99b1b39e5cda0ef12356220075c869ea4776dca36fe83b75`  
		Last Modified: Tue, 12 Dec 2023 23:43:18 GMT  
		Size: 121.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1.6.22` - unknown; unknown

```console
$ docker pull memcached@sha256:3d519a2eb9e00b43e6bc7584f6962b12ba032c4487a6e4ef7fd2b00b667bc90d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 MB (3053138 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9cc25288d58197dcc1309ea4a8128d0b120b92ad2d877f226095cd4847696474`

```dockerfile
```

-	Layers:
	-	`sha256:c5edc5ba98b4e6a438caa0d4541784c5c1e8b23d6020bc0b2a5b9910d0725400`  
		Last Modified: Tue, 12 Dec 2023 23:43:17 GMT  
		Size: 3.0 MB (3032003 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:b15e35765293b6f1da0e628c94108f229423c5a6379b8b5c47a41415f377b6d8`  
		Last Modified: Tue, 12 Dec 2023 23:43:17 GMT  
		Size: 21.1 KB (21135 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:1.6.22` - linux; 386

```console
$ docker pull memcached@sha256:fa9dba8086765d68f2feecfc2ac08fb29c019597d09943bb480227e6cba87666
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.3 MB (39294993 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:93047050e75b6d4d64adb8a7c8f68cb118bad27ca9dc772120e251b174752cf9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 16 Oct 2023 06:54:12 GMT
ADD file:0c94521fdd9c0a4fdeeb9aad23e68cd053fba0dcd7c3af550aefa79377816e31 in / 
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["bash"]
# Mon, 16 Oct 2023 06:54:12 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_VERSION=1.6.22
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_SHA1=7a691f390d59616dbebfc9e2e4942d499c39a338
# Mon, 16 Oct 2023 06:54:12 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V # buildkit
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
	-	`sha256:98bdfce9af831c2a0d0bfcca812d0039cd1666986550f552b4b4c625bd5aa31c`  
		Last Modified: Wed, 01 Nov 2023 00:43:26 GMT  
		Size: 30.2 MB (30164042 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1b647d4b10cf20ac5807101c7d0380701be684aa82f5c01ec41f674b5ef23d42`  
		Last Modified: Wed, 01 Nov 2023 01:06:49 GMT  
		Size: 1.1 KB (1109 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b61c058003459de4911c2901b2d799b03de754a1b9e64ffbe21a04992e962e62`  
		Last Modified: Wed, 01 Nov 2023 01:06:49 GMT  
		Size: 2.5 MB (2492501 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:810b6db64df2fcc8f76941cdac75093cf35bd72ac3cd1fa5eb664e74c1f67cd8`  
		Last Modified: Wed, 01 Nov 2023 01:06:50 GMT  
		Size: 6.6 MB (6636937 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:dbb899942df4149bd5fae8bac6e295285ec80f82d621f2b29c931ee348491cfb`  
		Last Modified: Wed, 01 Nov 2023 01:06:49 GMT  
		Size: 282.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4a8530160ab232c37c0ddcbf5e3a731d835d378d1382843957f6c2a73b2b5be6`  
		Last Modified: Wed, 01 Nov 2023 01:06:50 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1.6.22` - unknown; unknown

```console
$ docker pull memcached@sha256:dd7ce9519c31365127142232df2ed0b285e9acc03cd77c23c838bf932165def8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.5 KB (21498 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eef82c92e07c11a92c337806d01cfb1c6cdc7a16608dcf304a38de34d2ef1dbb`

```dockerfile
```

-	Layers:
	-	`sha256:c0d9dd22513f8d3e791e1796d7ef1906e57c798c92dd35d0be9cf2eaecec5954`  
		Last Modified: Wed, 01 Nov 2023 01:06:49 GMT  
		Size: 21.5 KB (21498 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:1.6.22` - linux; mips64le

```console
$ docker pull memcached@sha256:9f7696d5078cf83e8b152cb00a3615576fd3c50d10be9253b9c188e16bfd8087
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.9 MB (39863164 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:685886644cfb343923260c15c66eb8c8d8bf7b84b6b1e855732aec2359b6ae29`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 21 Nov 2023 04:09:50 GMT
ADD file:e093749192323dc72b60a8440ddba26c415586f618b5e107fa264ba5eb2ca7ba in / 
# Tue, 21 Nov 2023 04:09:54 GMT
CMD ["bash"]
# Mon, 04 Dec 2023 18:08:47 GMT
RUN set -eux; 	groupadd --system --gid 11211 memcache; 	useradd --system --gid memcache --uid 11211 memcache # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
ENV MEMCACHED_VERSION=1.6.22
# Mon, 04 Dec 2023 18:08:47 GMT
ENV MEMCACHED_URL=https://memcached.org/files/memcached-1.6.22.tar.gz
# Mon, 04 Dec 2023 18:08:47 GMT
ENV MEMCACHED_SHA1=7a691f390d59616dbebfc9e2e4942d499c39a338
# Mon, 04 Dec 2023 18:08:47 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O memcached.tar.gz "$MEMCACHED_URL"; 	echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c -; 	mkdir -p /usr/src/memcached; 	tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1; 	rm memcached.tar.gz; 		cd /usr/src/memcached; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	; 	nproc="$(nproc)"; 	make -j "$nproc"; 		sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf; 	make test PARALLEL="$nproc"; 	mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf; 		make install; 		cd /; 	rm -rf /usr/src/memcached; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		memcached -V # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 04 Dec 2023 18:08:47 GMT
USER memcache
# Mon, 04 Dec 2023 18:08:47 GMT
EXPOSE map[11211/tcp:{}]
# Mon, 04 Dec 2023 18:08:47 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:ebdff2138fee4a3ec27560ab1353dc51c12c2608ff721f5db3d24104872b702a`  
		Last Modified: Tue, 21 Nov 2023 04:20:35 GMT  
		Size: 29.1 MB (29141984 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ee63ae82c6a87dc28cedafb91fbd6eaccd22add5b00a9cceb208472b30427b5d`  
		Last Modified: Tue, 12 Dec 2023 23:10:03 GMT  
		Size: 1.1 KB (1114 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3d430991f88102b07bcf8bf22f07667e49c9dfedb134b0ac36ddbb99d1e79db2`  
		Last Modified: Tue, 12 Dec 2023 23:10:04 GMT  
		Size: 1.9 MB (1937475 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ebe1140b392e915b8757b8d0a4b83f0aaf2103734e9f83c318821f641207b6b4`  
		Last Modified: Tue, 12 Dec 2023 23:10:04 GMT  
		Size: 8.8 MB (8782185 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:aedf1130e49a6aa7d9b74b9fd00914b171966fcf8beba71095787811fa3a0284`  
		Last Modified: Tue, 12 Dec 2023 23:10:03 GMT  
		Size: 284.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:457e2691e0499a1a1d26e6da85567f20a8dc396bde9d9952ce75fdcfe6cbafd8`  
		Last Modified: Tue, 12 Dec 2023 23:10:05 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1.6.22` - unknown; unknown

```console
$ docker pull memcached@sha256:d48752667ff111ef73342ae5c16218a373275e8b65c7696eff231ff49ca7b8e5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.0 KB (21004 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9138b1207d88c6ca6b32a2616d3c25b1f5d3280b7650ac4bfa7120518f6a8ad7`

```dockerfile
```

-	Layers:
	-	`sha256:2b1c5f3190ac8dfdff54a51d9421ad623af991deba1a46ba943cf88442079207`  
		Last Modified: Tue, 12 Dec 2023 23:10:03 GMT  
		Size: 21.0 KB (21004 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:1.6.22` - linux; ppc64le

```console
$ docker pull memcached@sha256:813f2ed7d8d4d2c4e6f4a19816964b0c95cc56d038d95d059571d51e115ab109
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.5 MB (45508655 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:73c79988c4d09a9ac9cb01aa05096b344821e8034c3cba04afb9cb78fe25db05`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 21 Nov 2023 04:24:14 GMT
ADD file:8b22a531b6611a1e63dfc20e4e2931592e2d821bd4b64c4b2810bb9a36640c02 in / 
# Tue, 21 Nov 2023 04:24:16 GMT
CMD ["bash"]
# Mon, 04 Dec 2023 18:08:47 GMT
RUN set -eux; 	groupadd --system --gid 11211 memcache; 	useradd --system --gid memcache --uid 11211 memcache # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
ENV MEMCACHED_VERSION=1.6.22
# Mon, 04 Dec 2023 18:08:47 GMT
ENV MEMCACHED_URL=https://memcached.org/files/memcached-1.6.22.tar.gz
# Mon, 04 Dec 2023 18:08:47 GMT
ENV MEMCACHED_SHA1=7a691f390d59616dbebfc9e2e4942d499c39a338
# Mon, 04 Dec 2023 18:08:47 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O memcached.tar.gz "$MEMCACHED_URL"; 	echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c -; 	mkdir -p /usr/src/memcached; 	tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1; 	rm memcached.tar.gz; 		cd /usr/src/memcached; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	; 	nproc="$(nproc)"; 	make -j "$nproc"; 		sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf; 	make test PARALLEL="$nproc"; 	mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf; 		make install; 		cd /; 	rm -rf /usr/src/memcached; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		memcached -V # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 04 Dec 2023 18:08:47 GMT
USER memcache
# Mon, 04 Dec 2023 18:08:47 GMT
EXPOSE map[11211/tcp:{}]
# Mon, 04 Dec 2023 18:08:47 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:c570d04e61d8e35a3c8f12179d048d701451f97f9cf2099ea3e3738512dbf062`  
		Last Modified: Tue, 21 Nov 2023 04:28:58 GMT  
		Size: 33.1 MB (33141607 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b53469d03d0156e89526c2b744f6850b65cfb9b509a6fda4c523764f7a9f9072`  
		Last Modified: Tue, 12 Dec 2023 23:08:09 GMT  
		Size: 1.1 KB (1111 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:12b61a5974195d80345022ed47cb4546f6fec60527b3932b2ce74d605db750e0`  
		Last Modified: Tue, 12 Dec 2023 23:08:09 GMT  
		Size: 2.7 MB (2698202 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:108f5df7a0010e4f69929c6ce4ff2e0e53877c6bbe11bd86acbbb0e7b608dca7`  
		Last Modified: Tue, 12 Dec 2023 23:08:09 GMT  
		Size: 9.7 MB (9667330 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:aa53d1e0a6b1123a31838e581de8d738ccaf05c9be569ec50b8d37cbc54a99bd`  
		Last Modified: Tue, 12 Dec 2023 23:08:08 GMT  
		Size: 283.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2cf8ef0b438a2029bfc9b928364eb71966baa4990e2ac4a9b1648cbd44271dc4`  
		Last Modified: Tue, 12 Dec 2023 23:08:10 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1.6.22` - unknown; unknown

```console
$ docker pull memcached@sha256:d75efc7b8726fbfade0b41c14205058def09ee997a7befb495808c2752a56a54
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 MB (3066416 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ca8bb0be2316bb58a60c953382dd1963eb7e265d0602de370e02152e1ac84d7`

```dockerfile
```

-	Layers:
	-	`sha256:34203b346608565cdbcd7cf9a56efb8ec2255b1a8f30267d6b2749d6a0bd2d6b`  
		Last Modified: Tue, 12 Dec 2023 23:08:09 GMT  
		Size: 3.0 MB (3045398 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:4da4f2a55f1773bfac75983e2e733c609b970884e935de987ec5b3ec5c92eb85`  
		Last Modified: Tue, 12 Dec 2023 23:08:08 GMT  
		Size: 21.0 KB (21018 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:1.6.22` - linux; s390x

```console
$ docker pull memcached@sha256:05084fffc798db32442e2cde93eac5815ffd909e9bf65692ac08c9b5ab79e677
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.0 MB (38041790 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eac80baab625f3daf940cdb3053e2e709bd61d78d7eae50b7db4d71f87bcd149`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 21 Nov 2023 05:04:35 GMT
ADD file:c33fa9fdde73983850798b6eb1cd062e0398109d1d773e6a937fead7475c8efc in / 
# Tue, 21 Nov 2023 05:04:41 GMT
CMD ["bash"]
# Mon, 04 Dec 2023 18:08:47 GMT
RUN set -eux; 	groupadd --system --gid 11211 memcache; 	useradd --system --gid memcache --uid 11211 memcache # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
ENV MEMCACHED_VERSION=1.6.22
# Mon, 04 Dec 2023 18:08:47 GMT
ENV MEMCACHED_URL=https://memcached.org/files/memcached-1.6.22.tar.gz
# Mon, 04 Dec 2023 18:08:47 GMT
ENV MEMCACHED_SHA1=7a691f390d59616dbebfc9e2e4942d499c39a338
# Mon, 04 Dec 2023 18:08:47 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O memcached.tar.gz "$MEMCACHED_URL"; 	echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c -; 	mkdir -p /usr/src/memcached; 	tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1; 	rm memcached.tar.gz; 		cd /usr/src/memcached; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	; 	nproc="$(nproc)"; 	make -j "$nproc"; 		sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf; 	make test PARALLEL="$nproc"; 	mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf; 		make install; 		cd /; 	rm -rf /usr/src/memcached; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		memcached -V # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 04 Dec 2023 18:08:47 GMT
USER memcache
# Mon, 04 Dec 2023 18:08:47 GMT
EXPOSE map[11211/tcp:{}]
# Mon, 04 Dec 2023 18:08:47 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:6daa625e5a040476e253e7acd0befa74254a4865ec836d6334a544d82a21d4be`  
		Last Modified: Tue, 21 Nov 2023 05:10:21 GMT  
		Size: 27.5 MB (27512885 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b19a3143cbec7ddc9a646dbbe779b0b5ec67662cf70e280db146f6ace54ccd61`  
		Last Modified: Wed, 13 Dec 2023 00:26:35 GMT  
		Size: 1.1 KB (1111 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b8af028b1fa76aa55f540dd5be5eaf89eea3fec23e09e9a88550aac36e9ee843`  
		Last Modified: Wed, 13 Dec 2023 00:26:35 GMT  
		Size: 2.2 MB (2152508 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9a774943469875a0902c53fccdd95cad9c18234b759bcdcc5816bd563deb7f14`  
		Last Modified: Wed, 13 Dec 2023 00:26:35 GMT  
		Size: 8.4 MB (8374880 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:266b4bf499a815da6f7ddcf68e1e61f8418c8ec655a2083e174aaa385de74d76`  
		Last Modified: Wed, 13 Dec 2023 00:26:35 GMT  
		Size: 284.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0da709e3482cc552b0a7b69eb05aaa21af1e74baaf4e3bccc34e95e478943630`  
		Last Modified: Wed, 13 Dec 2023 00:26:36 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1.6.22` - unknown; unknown

```console
$ docker pull memcached@sha256:525abad348ba03c5b9444f23409d647581284c1642d30539e2c9943405266f12
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 MB (3067303 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e3b551ec9122d039520bbd13bced5b1f5b0d5b1fd9e32c09a1d4536f7af1226`

```dockerfile
```

-	Layers:
	-	`sha256:5cc0958f61715f0746d9fa2a8a5c06f31608bb5d1cf32d606c46fc8e11b35984`  
		Last Modified: Wed, 13 Dec 2023 00:26:35 GMT  
		Size: 3.0 MB (3046353 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:3d2fed99d3355e42a820c1975105411eb7584cffb111d7e1fd541603f7721f1c`  
		Last Modified: Wed, 13 Dec 2023 00:26:35 GMT  
		Size: 20.9 KB (20950 bytes)  
		MIME: application/vnd.in-toto+json

## `memcached:1.6.22-alpine`

```console
$ docker pull memcached@sha256:ae831daf80781a01c783ce07bf4517a65e3e25b4ee9b6fb9e576a01aaaa47ffc
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

### `memcached:1.6.22-alpine` - linux; amd64

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

### `memcached:1.6.22-alpine` - unknown; unknown

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

### `memcached:1.6.22-alpine` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:286df72d3172b8ed7793e7058f9327823d65bdac8a226a06a00d292c087ad9c2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.4 MB (4419383 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d682c07630240a305e61d9fe0b12e4dc6f338f6a6b2c95b0941b54b2b8509b75`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 08 Dec 2023 01:39:30 GMT
ADD file:8182c73f869a899cf624a59c400acb8226776d15e4d3a0d240a94e65340540d0 in / 
# Fri, 08 Dec 2023 01:39:30 GMT
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
	-	`sha256:c303524923177661067f7eb378c3dd5277088c2676ebd1cd78e68397bb80fdbf`  
		Last Modified: Fri, 08 Dec 2023 01:39:48 GMT  
		Size: 3.3 MB (3347794 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:dfede01b081f27465377bdafbbdb6b694c6fab18026972b2c380535dcef103b8`  
		Last Modified: Wed, 13 Dec 2023 01:35:47 GMT  
		Size: 1.2 KB (1246 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b6d7b6f4ad45bf3aee58c5a7e8083286bd79dc004840903fd5997929772bfb4c`  
		Last Modified: Wed, 13 Dec 2023 01:35:47 GMT  
		Size: 120.9 KB (120897 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:64a4d385fe9c52ce74fd893218a806a70ac60ff0c57a80c1b3e43096c1f9ebc0`  
		Last Modified: Wed, 13 Dec 2023 01:35:48 GMT  
		Size: 949.0 KB (949044 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fd5239ae2cadceed6ddca34da081735d9a9d40ec7e5bdded8b5faca81fb0a070`  
		Last Modified: Wed, 13 Dec 2023 01:35:48 GMT  
		Size: 282.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4ab0568624eca639b58ae572fcf8e82d6fb6cb3d9f6ca5d7df2b7329747dedd4`  
		Last Modified: Wed, 13 Dec 2023 01:35:49 GMT  
		Size: 120.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1.6.22-alpine` - unknown; unknown

```console
$ docker pull memcached@sha256:6f8a1e61dcc0fd492cbafc5fd2b4c22d6154464b462857003e8e48a48305823a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **98.1 KB (98108 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ffc7ff6f7a07bd49a0241faf0b1957add37ce71b17cbdf2c878e4fc78cdc7bc4`

```dockerfile
```

-	Layers:
	-	`sha256:a9702aa1523d9e76bf98e50205b92ccf5d5bee944388fa4b376abeae8048c7d5`  
		Last Modified: Wed, 13 Dec 2023 01:35:48 GMT  
		Size: 78.6 KB (78622 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:3a49d198124cd7443d92b69a3737a232e2d6e7c626eb726c2902193c31acd5bd`  
		Last Modified: Wed, 13 Dec 2023 01:35:47 GMT  
		Size: 19.5 KB (19486 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:1.6.22-alpine` - linux; 386

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

### `memcached:1.6.22-alpine` - unknown; unknown

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

### `memcached:1.6.22-alpine` - linux; ppc64le

```console
$ docker pull memcached@sha256:06711fbe2ddda329f14ab4a0825494b32336140e6a0e3b6c4d879adc475857c3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4468374 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09b1d12275d18bb3dac772e05585652308aa081f1aeae540381aea1c9ed321bd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 08 Dec 2023 01:22:51 GMT
ADD file:052421189f8d269382daaaa8beb63c687e4d8ca908c421abdce53bcc627a40b4 in / 
# Fri, 08 Dec 2023 01:22:51 GMT
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
	-	`sha256:243ac51c334a47917a84be93e972ee6378987e9b3b917a5a8df29025e161c1f3`  
		Last Modified: Fri, 08 Dec 2023 01:23:14 GMT  
		Size: 3.4 MB (3358233 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:add73e7dbebd6c86078686bb046ef57017b090fe917f656feb83ec0ef971b5f3`  
		Last Modified: Tue, 12 Dec 2023 23:20:17 GMT  
		Size: 1.2 KB (1243 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d64bed657a7e728633e13f2021b35954e98be9ecae77096d30cdaa1d9260d61e`  
		Last Modified: Tue, 12 Dec 2023 23:20:17 GMT  
		Size: 123.4 KB (123403 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1b7a39c0f73f39f740b607f200570edf13046db40879e4aebbdca9e2fd273b0f`  
		Last Modified: Tue, 12 Dec 2023 23:20:17 GMT  
		Size: 985.1 KB (985092 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ad6306836cf70172b90d6b82bffc8546c005c16cda9b7d58dc5dbd386b7ee7d8`  
		Last Modified: Tue, 12 Dec 2023 23:20:17 GMT  
		Size: 281.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:71e3eb1fb10d08825521650c7c7ddedf3cfce2f976e93c18ab11aace23c38be5`  
		Last Modified: Tue, 12 Dec 2023 23:20:18 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1.6.22-alpine` - unknown; unknown

```console
$ docker pull memcached@sha256:65ba466bf93c49f07fd340ced359d51a13a74b069cca4de2d034d12f42b92ea4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **96.4 KB (96395 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0e68093b9e036b2a9ff696038b0fd906f66504c0a0cd70dda18954ebb93d4bd1`

```dockerfile
```

-	Layers:
	-	`sha256:b64631288cf2d05d3a1d99eb8cb41f077724b027aaf136bb327f88055e4ceaf4`  
		Last Modified: Tue, 12 Dec 2023 23:20:17 GMT  
		Size: 77.0 KB (77025 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:8ac9ea640f8ca624c147fd0dcc40f859a6284e5f50c4396e0b1e962a4b732813`  
		Last Modified: Tue, 12 Dec 2023 23:20:17 GMT  
		Size: 19.4 KB (19370 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:1.6.22-alpine` - linux; s390x

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

### `memcached:1.6.22-alpine` - unknown; unknown

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

## `memcached:1.6.22-alpine3.19`

```console
$ docker pull memcached@sha256:fc05162ae59e353d64bc065f589df156b875b48ac0d9c6bab788e9a2a2e400ca
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 8
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown
	-	linux; ppc64le
	-	unknown; unknown
	-	linux; s390x
	-	unknown; unknown

### `memcached:1.6.22-alpine3.19` - linux; amd64

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

### `memcached:1.6.22-alpine3.19` - unknown; unknown

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

### `memcached:1.6.22-alpine3.19` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:286df72d3172b8ed7793e7058f9327823d65bdac8a226a06a00d292c087ad9c2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.4 MB (4419383 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d682c07630240a305e61d9fe0b12e4dc6f338f6a6b2c95b0941b54b2b8509b75`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 08 Dec 2023 01:39:30 GMT
ADD file:8182c73f869a899cf624a59c400acb8226776d15e4d3a0d240a94e65340540d0 in / 
# Fri, 08 Dec 2023 01:39:30 GMT
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
	-	`sha256:c303524923177661067f7eb378c3dd5277088c2676ebd1cd78e68397bb80fdbf`  
		Last Modified: Fri, 08 Dec 2023 01:39:48 GMT  
		Size: 3.3 MB (3347794 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:dfede01b081f27465377bdafbbdb6b694c6fab18026972b2c380535dcef103b8`  
		Last Modified: Wed, 13 Dec 2023 01:35:47 GMT  
		Size: 1.2 KB (1246 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b6d7b6f4ad45bf3aee58c5a7e8083286bd79dc004840903fd5997929772bfb4c`  
		Last Modified: Wed, 13 Dec 2023 01:35:47 GMT  
		Size: 120.9 KB (120897 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:64a4d385fe9c52ce74fd893218a806a70ac60ff0c57a80c1b3e43096c1f9ebc0`  
		Last Modified: Wed, 13 Dec 2023 01:35:48 GMT  
		Size: 949.0 KB (949044 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fd5239ae2cadceed6ddca34da081735d9a9d40ec7e5bdded8b5faca81fb0a070`  
		Last Modified: Wed, 13 Dec 2023 01:35:48 GMT  
		Size: 282.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4ab0568624eca639b58ae572fcf8e82d6fb6cb3d9f6ca5d7df2b7329747dedd4`  
		Last Modified: Wed, 13 Dec 2023 01:35:49 GMT  
		Size: 120.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1.6.22-alpine3.19` - unknown; unknown

```console
$ docker pull memcached@sha256:6f8a1e61dcc0fd492cbafc5fd2b4c22d6154464b462857003e8e48a48305823a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **98.1 KB (98108 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ffc7ff6f7a07bd49a0241faf0b1957add37ce71b17cbdf2c878e4fc78cdc7bc4`

```dockerfile
```

-	Layers:
	-	`sha256:a9702aa1523d9e76bf98e50205b92ccf5d5bee944388fa4b376abeae8048c7d5`  
		Last Modified: Wed, 13 Dec 2023 01:35:48 GMT  
		Size: 78.6 KB (78622 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:3a49d198124cd7443d92b69a3737a232e2d6e7c626eb726c2902193c31acd5bd`  
		Last Modified: Wed, 13 Dec 2023 01:35:47 GMT  
		Size: 19.5 KB (19486 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:1.6.22-alpine3.19` - linux; ppc64le

```console
$ docker pull memcached@sha256:06711fbe2ddda329f14ab4a0825494b32336140e6a0e3b6c4d879adc475857c3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4468374 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09b1d12275d18bb3dac772e05585652308aa081f1aeae540381aea1c9ed321bd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 08 Dec 2023 01:22:51 GMT
ADD file:052421189f8d269382daaaa8beb63c687e4d8ca908c421abdce53bcc627a40b4 in / 
# Fri, 08 Dec 2023 01:22:51 GMT
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
	-	`sha256:243ac51c334a47917a84be93e972ee6378987e9b3b917a5a8df29025e161c1f3`  
		Last Modified: Fri, 08 Dec 2023 01:23:14 GMT  
		Size: 3.4 MB (3358233 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:add73e7dbebd6c86078686bb046ef57017b090fe917f656feb83ec0ef971b5f3`  
		Last Modified: Tue, 12 Dec 2023 23:20:17 GMT  
		Size: 1.2 KB (1243 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d64bed657a7e728633e13f2021b35954e98be9ecae77096d30cdaa1d9260d61e`  
		Last Modified: Tue, 12 Dec 2023 23:20:17 GMT  
		Size: 123.4 KB (123403 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1b7a39c0f73f39f740b607f200570edf13046db40879e4aebbdca9e2fd273b0f`  
		Last Modified: Tue, 12 Dec 2023 23:20:17 GMT  
		Size: 985.1 KB (985092 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ad6306836cf70172b90d6b82bffc8546c005c16cda9b7d58dc5dbd386b7ee7d8`  
		Last Modified: Tue, 12 Dec 2023 23:20:17 GMT  
		Size: 281.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:71e3eb1fb10d08825521650c7c7ddedf3cfce2f976e93c18ab11aace23c38be5`  
		Last Modified: Tue, 12 Dec 2023 23:20:18 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1.6.22-alpine3.19` - unknown; unknown

```console
$ docker pull memcached@sha256:65ba466bf93c49f07fd340ced359d51a13a74b069cca4de2d034d12f42b92ea4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **96.4 KB (96395 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0e68093b9e036b2a9ff696038b0fd906f66504c0a0cd70dda18954ebb93d4bd1`

```dockerfile
```

-	Layers:
	-	`sha256:b64631288cf2d05d3a1d99eb8cb41f077724b027aaf136bb327f88055e4ceaf4`  
		Last Modified: Tue, 12 Dec 2023 23:20:17 GMT  
		Size: 77.0 KB (77025 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:8ac9ea640f8ca624c147fd0dcc40f859a6284e5f50c4396e0b1e962a4b732813`  
		Last Modified: Tue, 12 Dec 2023 23:20:17 GMT  
		Size: 19.4 KB (19370 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:1.6.22-alpine3.19` - linux; s390x

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

### `memcached:1.6.22-alpine3.19` - unknown; unknown

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

## `memcached:1.6.22-bookworm`

```console
$ docker pull memcached@sha256:5006d1a9ea8a2cedd728d75c2e85cb26c96489f6a039d14ba2c44f99ea310d1c
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 14
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm variant v5
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown
	-	linux; 386
	-	unknown; unknown
	-	linux; mips64le
	-	unknown; unknown
	-	linux; ppc64le
	-	unknown; unknown
	-	linux; s390x
	-	unknown; unknown

### `memcached:1.6.22-bookworm` - linux; amd64

```console
$ docker pull memcached@sha256:0d358fa0198562aa3d1e1c3e9386e1835256875517d8a4786f3dd50a1f65f1de
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.1 MB (41125606 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:03bad2c21b5df5c82f8c581ebec403482a3e00c0f35697ca669c46a7d000a13d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 21 Nov 2023 05:21:37 GMT
ADD file:d261a6f6921593f1e0b3f472ab1b1822e2c6deb0b369200f0b3370556bfad017 in / 
# Tue, 21 Nov 2023 05:21:37 GMT
CMD ["bash"]
# Mon, 04 Dec 2023 18:08:47 GMT
RUN set -eux; 	groupadd --system --gid 11211 memcache; 	useradd --system --gid memcache --uid 11211 memcache # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
ENV MEMCACHED_VERSION=1.6.22
# Mon, 04 Dec 2023 18:08:47 GMT
ENV MEMCACHED_URL=https://memcached.org/files/memcached-1.6.22.tar.gz
# Mon, 04 Dec 2023 18:08:47 GMT
ENV MEMCACHED_SHA1=7a691f390d59616dbebfc9e2e4942d499c39a338
# Mon, 04 Dec 2023 18:08:47 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O memcached.tar.gz "$MEMCACHED_URL"; 	echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c -; 	mkdir -p /usr/src/memcached; 	tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1; 	rm memcached.tar.gz; 		cd /usr/src/memcached; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	; 	nproc="$(nproc)"; 	make -j "$nproc"; 		sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf; 	make test PARALLEL="$nproc"; 	mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf; 		make install; 		cd /; 	rm -rf /usr/src/memcached; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		memcached -V # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 04 Dec 2023 18:08:47 GMT
USER memcache
# Mon, 04 Dec 2023 18:08:47 GMT
EXPOSE map[11211/tcp:{}]
# Mon, 04 Dec 2023 18:08:47 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:1f7ce2fa46ab3942feabee654933948821303a5a821789dddab2d8c3df59e227`  
		Last Modified: Tue, 21 Nov 2023 05:25:58 GMT  
		Size: 29.1 MB (29149908 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:21ac6fd160890cbc46a76542eb3f68654f3e3fb043b1b28a18155ec6863d60bc`  
		Last Modified: Tue, 12 Dec 2023 20:52:57 GMT  
		Size: 1.1 KB (1112 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6330fc82e1304befcc27a7598cd1a85152985d06426f94966788bf5a1583dcc6`  
		Last Modified: Tue, 12 Dec 2023 20:52:57 GMT  
		Size: 2.5 MB (2488284 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4047c827380f04698fbc51155441d719f93b84c1a092d633260c704f286296dd`  
		Last Modified: Tue, 12 Dec 2023 20:52:57 GMT  
		Size: 9.5 MB (9485895 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:401b5de2a4f8d9f588888754fa8347b67590c776363770f46ef67688116a4a0c`  
		Last Modified: Tue, 12 Dec 2023 20:52:57 GMT  
		Size: 285.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ee899f9aed95096580ea4a2325fd4824518ff1621f433f393fa253b52b7294b5`  
		Last Modified: Tue, 12 Dec 2023 20:52:58 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1.6.22-bookworm` - unknown; unknown

```console
$ docker pull memcached@sha256:5ccb88c1a86bd6524b6d5c9383254cdd79314d656a0c982658ecd35d9716431b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 MB (3077929 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:238ef9023561adc9c09faf875c5370cb2711a83cc7327dcc49ae7f8255c23794`

```dockerfile
```

-	Layers:
	-	`sha256:f84a6f3d0bdab8613be68ff091a6a78bedf8f697d4df55ff90ac7b745337e72c`  
		Last Modified: Tue, 12 Dec 2023 20:52:57 GMT  
		Size: 3.1 MB (3056812 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:8d7aee053ab87a86e42ba3d14810d3f1918c6e66d4d3ef02bc9c741f3948b83e`  
		Last Modified: Tue, 12 Dec 2023 20:52:57 GMT  
		Size: 21.1 KB (21117 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:1.6.22-bookworm` - linux; arm variant v5

```console
$ docker pull memcached@sha256:cb9426984b18b2d3df1c5fbb2bb7e2e9ebe08325d4adce6d0cd7a9207c413476
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.1 MB (37113170 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a8f2fb6119b629983f190d8b73208a156991d8cb65c47579a68125c339e9c75`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 21 Nov 2023 05:00:51 GMT
ADD file:1ae8e5ac45b11d01083680b765e1fcfef9f7938f89d6f424572126fa946d8cdf in / 
# Tue, 21 Nov 2023 05:00:52 GMT
CMD ["bash"]
# Mon, 04 Dec 2023 18:08:47 GMT
RUN set -eux; 	groupadd --system --gid 11211 memcache; 	useradd --system --gid memcache --uid 11211 memcache # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
ENV MEMCACHED_VERSION=1.6.22
# Mon, 04 Dec 2023 18:08:47 GMT
ENV MEMCACHED_URL=https://memcached.org/files/memcached-1.6.22.tar.gz
# Mon, 04 Dec 2023 18:08:47 GMT
ENV MEMCACHED_SHA1=7a691f390d59616dbebfc9e2e4942d499c39a338
# Mon, 04 Dec 2023 18:08:47 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O memcached.tar.gz "$MEMCACHED_URL"; 	echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c -; 	mkdir -p /usr/src/memcached; 	tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1; 	rm memcached.tar.gz; 		cd /usr/src/memcached; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	; 	nproc="$(nproc)"; 	make -j "$nproc"; 		sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf; 	make test PARALLEL="$nproc"; 	mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf; 		make install; 		cd /; 	rm -rf /usr/src/memcached; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		memcached -V # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 04 Dec 2023 18:08:47 GMT
USER memcache
# Mon, 04 Dec 2023 18:08:47 GMT
EXPOSE map[11211/tcp:{}]
# Mon, 04 Dec 2023 18:08:47 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:f476aef5b6e1122850e68c81ef06fc2df17e968961b060483b4d2fb33018aae3`  
		Last Modified: Tue, 21 Nov 2023 05:03:55 GMT  
		Size: 26.9 MB (26922153 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:89367ca16d2c3104d44514e1b9b94b0ac4070ea0f6f04523c72dda62795f3a17`  
		Last Modified: Tue, 12 Dec 2023 21:47:13 GMT  
		Size: 1.1 KB (1110 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5ecbc6577cf78c09bd4136f78a57a904ae1ab705fce8595e8d1187d800158e6f`  
		Last Modified: Tue, 12 Dec 2023 21:47:14 GMT  
		Size: 2.1 MB (2089289 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:12f8a270079b04e1372c73cc16ff2ae33e6f6ee0dcc7e8ed57843fca20b3d038`  
		Last Modified: Tue, 12 Dec 2023 21:47:14 GMT  
		Size: 8.1 MB (8100211 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5f592556023f9ba6125ecf6b89156ba61c05526ad324708c3d2a09600ee5e7e4`  
		Last Modified: Tue, 12 Dec 2023 21:47:14 GMT  
		Size: 285.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fa757a09f6a7a23114a13869f15b229384628cf108567d395dc0d4730c685409`  
		Last Modified: Tue, 12 Dec 2023 21:47:14 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1.6.22-bookworm` - unknown; unknown

```console
$ docker pull memcached@sha256:0c93e2660a508733f1c7d5236af77ef81fbcd0b27e4ac55c81d83334c8794891
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.0 KB (21043 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:538fbf714aa2f8a4175400dd43b0715e416f73fe598fc50d3f763afa144595da`

```dockerfile
```

-	Layers:
	-	`sha256:f65b3a9a0f6936cae3c1e411ecdd846d754a1978d851fdacf4b25526cb9ff4cc`  
		Last Modified: Tue, 12 Dec 2023 21:47:14 GMT  
		Size: 21.0 KB (21043 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:1.6.22-bookworm` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:c5adc5a4207d95c96a36131c2d39085b082f0e22f4595b935e72bcb463c10383
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.0 MB (39979924 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf26c17403ed5a4db96ddd8b41aeb2fd45483f897882a57972c994c95a44c5dd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 21 Nov 2023 06:27:06 GMT
ADD file:869c7d0747a17c53715581a2e862992eb8516c7f45f167821dfa80966a4870d1 in / 
# Tue, 21 Nov 2023 06:27:06 GMT
CMD ["bash"]
# Mon, 04 Dec 2023 18:08:47 GMT
RUN set -eux; 	groupadd --system --gid 11211 memcache; 	useradd --system --gid memcache --uid 11211 memcache # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
ENV MEMCACHED_VERSION=1.6.22
# Mon, 04 Dec 2023 18:08:47 GMT
ENV MEMCACHED_URL=https://memcached.org/files/memcached-1.6.22.tar.gz
# Mon, 04 Dec 2023 18:08:47 GMT
ENV MEMCACHED_SHA1=7a691f390d59616dbebfc9e2e4942d499c39a338
# Mon, 04 Dec 2023 18:08:47 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O memcached.tar.gz "$MEMCACHED_URL"; 	echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c -; 	mkdir -p /usr/src/memcached; 	tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1; 	rm memcached.tar.gz; 		cd /usr/src/memcached; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	; 	nproc="$(nproc)"; 	make -j "$nproc"; 		sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf; 	make test PARALLEL="$nproc"; 	mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf; 		make install; 		cd /; 	rm -rf /usr/src/memcached; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		memcached -V # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 04 Dec 2023 18:08:47 GMT
USER memcache
# Mon, 04 Dec 2023 18:08:47 GMT
EXPOSE map[11211/tcp:{}]
# Mon, 04 Dec 2023 18:08:47 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:2c6d21737d8318aa15c4cc838475029a5efc36c0429e3d8da80d97d0b96d9aaf`  
		Last Modified: Tue, 21 Nov 2023 06:30:30 GMT  
		Size: 29.2 MB (29179277 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1a39d6fec0d552a8078ab223bafd58bc9a0c8c27c26600a5b95c6a521bb97f3d`  
		Last Modified: Tue, 12 Dec 2023 23:43:17 GMT  
		Size: 1.1 KB (1112 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9d1ceea69964553dd3aaf853e0d7b753495cab4623b9377c69096be0bdf88146`  
		Last Modified: Tue, 12 Dec 2023 23:43:17 GMT  
		Size: 2.3 MB (2345975 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:52063b8e37cbc1e5e6e3af0f54b834ae3f6a53d023349ae819c9607e5fc98aec`  
		Last Modified: Tue, 12 Dec 2023 23:43:17 GMT  
		Size: 8.5 MB (8453155 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5b99d0095a64f8110efee1f5e91754cc923294d50c9e2927e515354746a3f465`  
		Last Modified: Tue, 12 Dec 2023 23:43:17 GMT  
		Size: 284.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:913c9e21eaa9c49c99b1b39e5cda0ef12356220075c869ea4776dca36fe83b75`  
		Last Modified: Tue, 12 Dec 2023 23:43:18 GMT  
		Size: 121.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1.6.22-bookworm` - unknown; unknown

```console
$ docker pull memcached@sha256:3d519a2eb9e00b43e6bc7584f6962b12ba032c4487a6e4ef7fd2b00b667bc90d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 MB (3053138 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9cc25288d58197dcc1309ea4a8128d0b120b92ad2d877f226095cd4847696474`

```dockerfile
```

-	Layers:
	-	`sha256:c5edc5ba98b4e6a438caa0d4541784c5c1e8b23d6020bc0b2a5b9910d0725400`  
		Last Modified: Tue, 12 Dec 2023 23:43:17 GMT  
		Size: 3.0 MB (3032003 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:b15e35765293b6f1da0e628c94108f229423c5a6379b8b5c47a41415f377b6d8`  
		Last Modified: Tue, 12 Dec 2023 23:43:17 GMT  
		Size: 21.1 KB (21135 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:1.6.22-bookworm` - linux; 386

```console
$ docker pull memcached@sha256:fa9dba8086765d68f2feecfc2ac08fb29c019597d09943bb480227e6cba87666
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.3 MB (39294993 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:93047050e75b6d4d64adb8a7c8f68cb118bad27ca9dc772120e251b174752cf9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 16 Oct 2023 06:54:12 GMT
ADD file:0c94521fdd9c0a4fdeeb9aad23e68cd053fba0dcd7c3af550aefa79377816e31 in / 
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["bash"]
# Mon, 16 Oct 2023 06:54:12 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_VERSION=1.6.22
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_SHA1=7a691f390d59616dbebfc9e2e4942d499c39a338
# Mon, 16 Oct 2023 06:54:12 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V # buildkit
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
	-	`sha256:98bdfce9af831c2a0d0bfcca812d0039cd1666986550f552b4b4c625bd5aa31c`  
		Last Modified: Wed, 01 Nov 2023 00:43:26 GMT  
		Size: 30.2 MB (30164042 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1b647d4b10cf20ac5807101c7d0380701be684aa82f5c01ec41f674b5ef23d42`  
		Last Modified: Wed, 01 Nov 2023 01:06:49 GMT  
		Size: 1.1 KB (1109 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b61c058003459de4911c2901b2d799b03de754a1b9e64ffbe21a04992e962e62`  
		Last Modified: Wed, 01 Nov 2023 01:06:49 GMT  
		Size: 2.5 MB (2492501 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:810b6db64df2fcc8f76941cdac75093cf35bd72ac3cd1fa5eb664e74c1f67cd8`  
		Last Modified: Wed, 01 Nov 2023 01:06:50 GMT  
		Size: 6.6 MB (6636937 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:dbb899942df4149bd5fae8bac6e295285ec80f82d621f2b29c931ee348491cfb`  
		Last Modified: Wed, 01 Nov 2023 01:06:49 GMT  
		Size: 282.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4a8530160ab232c37c0ddcbf5e3a731d835d378d1382843957f6c2a73b2b5be6`  
		Last Modified: Wed, 01 Nov 2023 01:06:50 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1.6.22-bookworm` - unknown; unknown

```console
$ docker pull memcached@sha256:dd7ce9519c31365127142232df2ed0b285e9acc03cd77c23c838bf932165def8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.5 KB (21498 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eef82c92e07c11a92c337806d01cfb1c6cdc7a16608dcf304a38de34d2ef1dbb`

```dockerfile
```

-	Layers:
	-	`sha256:c0d9dd22513f8d3e791e1796d7ef1906e57c798c92dd35d0be9cf2eaecec5954`  
		Last Modified: Wed, 01 Nov 2023 01:06:49 GMT  
		Size: 21.5 KB (21498 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:1.6.22-bookworm` - linux; mips64le

```console
$ docker pull memcached@sha256:9f7696d5078cf83e8b152cb00a3615576fd3c50d10be9253b9c188e16bfd8087
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.9 MB (39863164 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:685886644cfb343923260c15c66eb8c8d8bf7b84b6b1e855732aec2359b6ae29`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 21 Nov 2023 04:09:50 GMT
ADD file:e093749192323dc72b60a8440ddba26c415586f618b5e107fa264ba5eb2ca7ba in / 
# Tue, 21 Nov 2023 04:09:54 GMT
CMD ["bash"]
# Mon, 04 Dec 2023 18:08:47 GMT
RUN set -eux; 	groupadd --system --gid 11211 memcache; 	useradd --system --gid memcache --uid 11211 memcache # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
ENV MEMCACHED_VERSION=1.6.22
# Mon, 04 Dec 2023 18:08:47 GMT
ENV MEMCACHED_URL=https://memcached.org/files/memcached-1.6.22.tar.gz
# Mon, 04 Dec 2023 18:08:47 GMT
ENV MEMCACHED_SHA1=7a691f390d59616dbebfc9e2e4942d499c39a338
# Mon, 04 Dec 2023 18:08:47 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O memcached.tar.gz "$MEMCACHED_URL"; 	echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c -; 	mkdir -p /usr/src/memcached; 	tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1; 	rm memcached.tar.gz; 		cd /usr/src/memcached; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	; 	nproc="$(nproc)"; 	make -j "$nproc"; 		sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf; 	make test PARALLEL="$nproc"; 	mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf; 		make install; 		cd /; 	rm -rf /usr/src/memcached; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		memcached -V # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 04 Dec 2023 18:08:47 GMT
USER memcache
# Mon, 04 Dec 2023 18:08:47 GMT
EXPOSE map[11211/tcp:{}]
# Mon, 04 Dec 2023 18:08:47 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:ebdff2138fee4a3ec27560ab1353dc51c12c2608ff721f5db3d24104872b702a`  
		Last Modified: Tue, 21 Nov 2023 04:20:35 GMT  
		Size: 29.1 MB (29141984 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ee63ae82c6a87dc28cedafb91fbd6eaccd22add5b00a9cceb208472b30427b5d`  
		Last Modified: Tue, 12 Dec 2023 23:10:03 GMT  
		Size: 1.1 KB (1114 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3d430991f88102b07bcf8bf22f07667e49c9dfedb134b0ac36ddbb99d1e79db2`  
		Last Modified: Tue, 12 Dec 2023 23:10:04 GMT  
		Size: 1.9 MB (1937475 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ebe1140b392e915b8757b8d0a4b83f0aaf2103734e9f83c318821f641207b6b4`  
		Last Modified: Tue, 12 Dec 2023 23:10:04 GMT  
		Size: 8.8 MB (8782185 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:aedf1130e49a6aa7d9b74b9fd00914b171966fcf8beba71095787811fa3a0284`  
		Last Modified: Tue, 12 Dec 2023 23:10:03 GMT  
		Size: 284.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:457e2691e0499a1a1d26e6da85567f20a8dc396bde9d9952ce75fdcfe6cbafd8`  
		Last Modified: Tue, 12 Dec 2023 23:10:05 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1.6.22-bookworm` - unknown; unknown

```console
$ docker pull memcached@sha256:d48752667ff111ef73342ae5c16218a373275e8b65c7696eff231ff49ca7b8e5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.0 KB (21004 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9138b1207d88c6ca6b32a2616d3c25b1f5d3280b7650ac4bfa7120518f6a8ad7`

```dockerfile
```

-	Layers:
	-	`sha256:2b1c5f3190ac8dfdff54a51d9421ad623af991deba1a46ba943cf88442079207`  
		Last Modified: Tue, 12 Dec 2023 23:10:03 GMT  
		Size: 21.0 KB (21004 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:1.6.22-bookworm` - linux; ppc64le

```console
$ docker pull memcached@sha256:813f2ed7d8d4d2c4e6f4a19816964b0c95cc56d038d95d059571d51e115ab109
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.5 MB (45508655 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:73c79988c4d09a9ac9cb01aa05096b344821e8034c3cba04afb9cb78fe25db05`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 21 Nov 2023 04:24:14 GMT
ADD file:8b22a531b6611a1e63dfc20e4e2931592e2d821bd4b64c4b2810bb9a36640c02 in / 
# Tue, 21 Nov 2023 04:24:16 GMT
CMD ["bash"]
# Mon, 04 Dec 2023 18:08:47 GMT
RUN set -eux; 	groupadd --system --gid 11211 memcache; 	useradd --system --gid memcache --uid 11211 memcache # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
ENV MEMCACHED_VERSION=1.6.22
# Mon, 04 Dec 2023 18:08:47 GMT
ENV MEMCACHED_URL=https://memcached.org/files/memcached-1.6.22.tar.gz
# Mon, 04 Dec 2023 18:08:47 GMT
ENV MEMCACHED_SHA1=7a691f390d59616dbebfc9e2e4942d499c39a338
# Mon, 04 Dec 2023 18:08:47 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O memcached.tar.gz "$MEMCACHED_URL"; 	echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c -; 	mkdir -p /usr/src/memcached; 	tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1; 	rm memcached.tar.gz; 		cd /usr/src/memcached; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	; 	nproc="$(nproc)"; 	make -j "$nproc"; 		sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf; 	make test PARALLEL="$nproc"; 	mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf; 		make install; 		cd /; 	rm -rf /usr/src/memcached; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		memcached -V # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 04 Dec 2023 18:08:47 GMT
USER memcache
# Mon, 04 Dec 2023 18:08:47 GMT
EXPOSE map[11211/tcp:{}]
# Mon, 04 Dec 2023 18:08:47 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:c570d04e61d8e35a3c8f12179d048d701451f97f9cf2099ea3e3738512dbf062`  
		Last Modified: Tue, 21 Nov 2023 04:28:58 GMT  
		Size: 33.1 MB (33141607 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b53469d03d0156e89526c2b744f6850b65cfb9b509a6fda4c523764f7a9f9072`  
		Last Modified: Tue, 12 Dec 2023 23:08:09 GMT  
		Size: 1.1 KB (1111 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:12b61a5974195d80345022ed47cb4546f6fec60527b3932b2ce74d605db750e0`  
		Last Modified: Tue, 12 Dec 2023 23:08:09 GMT  
		Size: 2.7 MB (2698202 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:108f5df7a0010e4f69929c6ce4ff2e0e53877c6bbe11bd86acbbb0e7b608dca7`  
		Last Modified: Tue, 12 Dec 2023 23:08:09 GMT  
		Size: 9.7 MB (9667330 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:aa53d1e0a6b1123a31838e581de8d738ccaf05c9be569ec50b8d37cbc54a99bd`  
		Last Modified: Tue, 12 Dec 2023 23:08:08 GMT  
		Size: 283.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2cf8ef0b438a2029bfc9b928364eb71966baa4990e2ac4a9b1648cbd44271dc4`  
		Last Modified: Tue, 12 Dec 2023 23:08:10 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1.6.22-bookworm` - unknown; unknown

```console
$ docker pull memcached@sha256:d75efc7b8726fbfade0b41c14205058def09ee997a7befb495808c2752a56a54
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 MB (3066416 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ca8bb0be2316bb58a60c953382dd1963eb7e265d0602de370e02152e1ac84d7`

```dockerfile
```

-	Layers:
	-	`sha256:34203b346608565cdbcd7cf9a56efb8ec2255b1a8f30267d6b2749d6a0bd2d6b`  
		Last Modified: Tue, 12 Dec 2023 23:08:09 GMT  
		Size: 3.0 MB (3045398 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:4da4f2a55f1773bfac75983e2e733c609b970884e935de987ec5b3ec5c92eb85`  
		Last Modified: Tue, 12 Dec 2023 23:08:08 GMT  
		Size: 21.0 KB (21018 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:1.6.22-bookworm` - linux; s390x

```console
$ docker pull memcached@sha256:05084fffc798db32442e2cde93eac5815ffd909e9bf65692ac08c9b5ab79e677
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.0 MB (38041790 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eac80baab625f3daf940cdb3053e2e709bd61d78d7eae50b7db4d71f87bcd149`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 21 Nov 2023 05:04:35 GMT
ADD file:c33fa9fdde73983850798b6eb1cd062e0398109d1d773e6a937fead7475c8efc in / 
# Tue, 21 Nov 2023 05:04:41 GMT
CMD ["bash"]
# Mon, 04 Dec 2023 18:08:47 GMT
RUN set -eux; 	groupadd --system --gid 11211 memcache; 	useradd --system --gid memcache --uid 11211 memcache # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
ENV MEMCACHED_VERSION=1.6.22
# Mon, 04 Dec 2023 18:08:47 GMT
ENV MEMCACHED_URL=https://memcached.org/files/memcached-1.6.22.tar.gz
# Mon, 04 Dec 2023 18:08:47 GMT
ENV MEMCACHED_SHA1=7a691f390d59616dbebfc9e2e4942d499c39a338
# Mon, 04 Dec 2023 18:08:47 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O memcached.tar.gz "$MEMCACHED_URL"; 	echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c -; 	mkdir -p /usr/src/memcached; 	tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1; 	rm memcached.tar.gz; 		cd /usr/src/memcached; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	; 	nproc="$(nproc)"; 	make -j "$nproc"; 		sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf; 	make test PARALLEL="$nproc"; 	mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf; 		make install; 		cd /; 	rm -rf /usr/src/memcached; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		memcached -V # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 04 Dec 2023 18:08:47 GMT
USER memcache
# Mon, 04 Dec 2023 18:08:47 GMT
EXPOSE map[11211/tcp:{}]
# Mon, 04 Dec 2023 18:08:47 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:6daa625e5a040476e253e7acd0befa74254a4865ec836d6334a544d82a21d4be`  
		Last Modified: Tue, 21 Nov 2023 05:10:21 GMT  
		Size: 27.5 MB (27512885 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b19a3143cbec7ddc9a646dbbe779b0b5ec67662cf70e280db146f6ace54ccd61`  
		Last Modified: Wed, 13 Dec 2023 00:26:35 GMT  
		Size: 1.1 KB (1111 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b8af028b1fa76aa55f540dd5be5eaf89eea3fec23e09e9a88550aac36e9ee843`  
		Last Modified: Wed, 13 Dec 2023 00:26:35 GMT  
		Size: 2.2 MB (2152508 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9a774943469875a0902c53fccdd95cad9c18234b759bcdcc5816bd563deb7f14`  
		Last Modified: Wed, 13 Dec 2023 00:26:35 GMT  
		Size: 8.4 MB (8374880 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:266b4bf499a815da6f7ddcf68e1e61f8418c8ec655a2083e174aaa385de74d76`  
		Last Modified: Wed, 13 Dec 2023 00:26:35 GMT  
		Size: 284.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0da709e3482cc552b0a7b69eb05aaa21af1e74baaf4e3bccc34e95e478943630`  
		Last Modified: Wed, 13 Dec 2023 00:26:36 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1.6.22-bookworm` - unknown; unknown

```console
$ docker pull memcached@sha256:525abad348ba03c5b9444f23409d647581284c1642d30539e2c9943405266f12
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 MB (3067303 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e3b551ec9122d039520bbd13bced5b1f5b0d5b1fd9e32c09a1d4536f7af1226`

```dockerfile
```

-	Layers:
	-	`sha256:5cc0958f61715f0746d9fa2a8a5c06f31608bb5d1cf32d606c46fc8e11b35984`  
		Last Modified: Wed, 13 Dec 2023 00:26:35 GMT  
		Size: 3.0 MB (3046353 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:3d2fed99d3355e42a820c1975105411eb7584cffb111d7e1fd541603f7721f1c`  
		Last Modified: Wed, 13 Dec 2023 00:26:35 GMT  
		Size: 20.9 KB (20950 bytes)  
		MIME: application/vnd.in-toto+json

## `memcached:alpine`

```console
$ docker pull memcached@sha256:9587ad270892c531bf1ac66f195312c2f0f374192e5ac79cf2dfc5dd7cd1555e
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

### `memcached:alpine` - linux; amd64

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

### `memcached:alpine` - unknown; unknown

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

### `memcached:alpine` - linux; arm variant v7

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

### `memcached:alpine` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:286df72d3172b8ed7793e7058f9327823d65bdac8a226a06a00d292c087ad9c2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.4 MB (4419383 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d682c07630240a305e61d9fe0b12e4dc6f338f6a6b2c95b0941b54b2b8509b75`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 08 Dec 2023 01:39:30 GMT
ADD file:8182c73f869a899cf624a59c400acb8226776d15e4d3a0d240a94e65340540d0 in / 
# Fri, 08 Dec 2023 01:39:30 GMT
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
	-	`sha256:c303524923177661067f7eb378c3dd5277088c2676ebd1cd78e68397bb80fdbf`  
		Last Modified: Fri, 08 Dec 2023 01:39:48 GMT  
		Size: 3.3 MB (3347794 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:dfede01b081f27465377bdafbbdb6b694c6fab18026972b2c380535dcef103b8`  
		Last Modified: Wed, 13 Dec 2023 01:35:47 GMT  
		Size: 1.2 KB (1246 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b6d7b6f4ad45bf3aee58c5a7e8083286bd79dc004840903fd5997929772bfb4c`  
		Last Modified: Wed, 13 Dec 2023 01:35:47 GMT  
		Size: 120.9 KB (120897 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:64a4d385fe9c52ce74fd893218a806a70ac60ff0c57a80c1b3e43096c1f9ebc0`  
		Last Modified: Wed, 13 Dec 2023 01:35:48 GMT  
		Size: 949.0 KB (949044 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fd5239ae2cadceed6ddca34da081735d9a9d40ec7e5bdded8b5faca81fb0a070`  
		Last Modified: Wed, 13 Dec 2023 01:35:48 GMT  
		Size: 282.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4ab0568624eca639b58ae572fcf8e82d6fb6cb3d9f6ca5d7df2b7329747dedd4`  
		Last Modified: Wed, 13 Dec 2023 01:35:49 GMT  
		Size: 120.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:alpine` - unknown; unknown

```console
$ docker pull memcached@sha256:6f8a1e61dcc0fd492cbafc5fd2b4c22d6154464b462857003e8e48a48305823a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **98.1 KB (98108 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ffc7ff6f7a07bd49a0241faf0b1957add37ce71b17cbdf2c878e4fc78cdc7bc4`

```dockerfile
```

-	Layers:
	-	`sha256:a9702aa1523d9e76bf98e50205b92ccf5d5bee944388fa4b376abeae8048c7d5`  
		Last Modified: Wed, 13 Dec 2023 01:35:48 GMT  
		Size: 78.6 KB (78622 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:3a49d198124cd7443d92b69a3737a232e2d6e7c626eb726c2902193c31acd5bd`  
		Last Modified: Wed, 13 Dec 2023 01:35:47 GMT  
		Size: 19.5 KB (19486 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:alpine` - linux; 386

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

### `memcached:alpine` - unknown; unknown

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

### `memcached:alpine` - linux; ppc64le

```console
$ docker pull memcached@sha256:06711fbe2ddda329f14ab4a0825494b32336140e6a0e3b6c4d879adc475857c3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4468374 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09b1d12275d18bb3dac772e05585652308aa081f1aeae540381aea1c9ed321bd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 08 Dec 2023 01:22:51 GMT
ADD file:052421189f8d269382daaaa8beb63c687e4d8ca908c421abdce53bcc627a40b4 in / 
# Fri, 08 Dec 2023 01:22:51 GMT
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
	-	`sha256:243ac51c334a47917a84be93e972ee6378987e9b3b917a5a8df29025e161c1f3`  
		Last Modified: Fri, 08 Dec 2023 01:23:14 GMT  
		Size: 3.4 MB (3358233 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:add73e7dbebd6c86078686bb046ef57017b090fe917f656feb83ec0ef971b5f3`  
		Last Modified: Tue, 12 Dec 2023 23:20:17 GMT  
		Size: 1.2 KB (1243 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d64bed657a7e728633e13f2021b35954e98be9ecae77096d30cdaa1d9260d61e`  
		Last Modified: Tue, 12 Dec 2023 23:20:17 GMT  
		Size: 123.4 KB (123403 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1b7a39c0f73f39f740b607f200570edf13046db40879e4aebbdca9e2fd273b0f`  
		Last Modified: Tue, 12 Dec 2023 23:20:17 GMT  
		Size: 985.1 KB (985092 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ad6306836cf70172b90d6b82bffc8546c005c16cda9b7d58dc5dbd386b7ee7d8`  
		Last Modified: Tue, 12 Dec 2023 23:20:17 GMT  
		Size: 281.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:71e3eb1fb10d08825521650c7c7ddedf3cfce2f976e93c18ab11aace23c38be5`  
		Last Modified: Tue, 12 Dec 2023 23:20:18 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:alpine` - unknown; unknown

```console
$ docker pull memcached@sha256:65ba466bf93c49f07fd340ced359d51a13a74b069cca4de2d034d12f42b92ea4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **96.4 KB (96395 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0e68093b9e036b2a9ff696038b0fd906f66504c0a0cd70dda18954ebb93d4bd1`

```dockerfile
```

-	Layers:
	-	`sha256:b64631288cf2d05d3a1d99eb8cb41f077724b027aaf136bb327f88055e4ceaf4`  
		Last Modified: Tue, 12 Dec 2023 23:20:17 GMT  
		Size: 77.0 KB (77025 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:8ac9ea640f8ca624c147fd0dcc40f859a6284e5f50c4396e0b1e962a4b732813`  
		Last Modified: Tue, 12 Dec 2023 23:20:17 GMT  
		Size: 19.4 KB (19370 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:alpine` - linux; s390x

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

### `memcached:alpine` - unknown; unknown

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

## `memcached:alpine3.19`

```console
$ docker pull memcached@sha256:fc05162ae59e353d64bc065f589df156b875b48ac0d9c6bab788e9a2a2e400ca
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 8
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown
	-	linux; ppc64le
	-	unknown; unknown
	-	linux; s390x
	-	unknown; unknown

### `memcached:alpine3.19` - linux; amd64

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

### `memcached:alpine3.19` - unknown; unknown

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

### `memcached:alpine3.19` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:286df72d3172b8ed7793e7058f9327823d65bdac8a226a06a00d292c087ad9c2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.4 MB (4419383 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d682c07630240a305e61d9fe0b12e4dc6f338f6a6b2c95b0941b54b2b8509b75`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 08 Dec 2023 01:39:30 GMT
ADD file:8182c73f869a899cf624a59c400acb8226776d15e4d3a0d240a94e65340540d0 in / 
# Fri, 08 Dec 2023 01:39:30 GMT
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
	-	`sha256:c303524923177661067f7eb378c3dd5277088c2676ebd1cd78e68397bb80fdbf`  
		Last Modified: Fri, 08 Dec 2023 01:39:48 GMT  
		Size: 3.3 MB (3347794 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:dfede01b081f27465377bdafbbdb6b694c6fab18026972b2c380535dcef103b8`  
		Last Modified: Wed, 13 Dec 2023 01:35:47 GMT  
		Size: 1.2 KB (1246 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b6d7b6f4ad45bf3aee58c5a7e8083286bd79dc004840903fd5997929772bfb4c`  
		Last Modified: Wed, 13 Dec 2023 01:35:47 GMT  
		Size: 120.9 KB (120897 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:64a4d385fe9c52ce74fd893218a806a70ac60ff0c57a80c1b3e43096c1f9ebc0`  
		Last Modified: Wed, 13 Dec 2023 01:35:48 GMT  
		Size: 949.0 KB (949044 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fd5239ae2cadceed6ddca34da081735d9a9d40ec7e5bdded8b5faca81fb0a070`  
		Last Modified: Wed, 13 Dec 2023 01:35:48 GMT  
		Size: 282.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4ab0568624eca639b58ae572fcf8e82d6fb6cb3d9f6ca5d7df2b7329747dedd4`  
		Last Modified: Wed, 13 Dec 2023 01:35:49 GMT  
		Size: 120.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:alpine3.19` - unknown; unknown

```console
$ docker pull memcached@sha256:6f8a1e61dcc0fd492cbafc5fd2b4c22d6154464b462857003e8e48a48305823a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **98.1 KB (98108 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ffc7ff6f7a07bd49a0241faf0b1957add37ce71b17cbdf2c878e4fc78cdc7bc4`

```dockerfile
```

-	Layers:
	-	`sha256:a9702aa1523d9e76bf98e50205b92ccf5d5bee944388fa4b376abeae8048c7d5`  
		Last Modified: Wed, 13 Dec 2023 01:35:48 GMT  
		Size: 78.6 KB (78622 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:3a49d198124cd7443d92b69a3737a232e2d6e7c626eb726c2902193c31acd5bd`  
		Last Modified: Wed, 13 Dec 2023 01:35:47 GMT  
		Size: 19.5 KB (19486 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:alpine3.19` - linux; ppc64le

```console
$ docker pull memcached@sha256:06711fbe2ddda329f14ab4a0825494b32336140e6a0e3b6c4d879adc475857c3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4468374 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09b1d12275d18bb3dac772e05585652308aa081f1aeae540381aea1c9ed321bd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 08 Dec 2023 01:22:51 GMT
ADD file:052421189f8d269382daaaa8beb63c687e4d8ca908c421abdce53bcc627a40b4 in / 
# Fri, 08 Dec 2023 01:22:51 GMT
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
	-	`sha256:243ac51c334a47917a84be93e972ee6378987e9b3b917a5a8df29025e161c1f3`  
		Last Modified: Fri, 08 Dec 2023 01:23:14 GMT  
		Size: 3.4 MB (3358233 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:add73e7dbebd6c86078686bb046ef57017b090fe917f656feb83ec0ef971b5f3`  
		Last Modified: Tue, 12 Dec 2023 23:20:17 GMT  
		Size: 1.2 KB (1243 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d64bed657a7e728633e13f2021b35954e98be9ecae77096d30cdaa1d9260d61e`  
		Last Modified: Tue, 12 Dec 2023 23:20:17 GMT  
		Size: 123.4 KB (123403 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1b7a39c0f73f39f740b607f200570edf13046db40879e4aebbdca9e2fd273b0f`  
		Last Modified: Tue, 12 Dec 2023 23:20:17 GMT  
		Size: 985.1 KB (985092 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ad6306836cf70172b90d6b82bffc8546c005c16cda9b7d58dc5dbd386b7ee7d8`  
		Last Modified: Tue, 12 Dec 2023 23:20:17 GMT  
		Size: 281.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:71e3eb1fb10d08825521650c7c7ddedf3cfce2f976e93c18ab11aace23c38be5`  
		Last Modified: Tue, 12 Dec 2023 23:20:18 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:alpine3.19` - unknown; unknown

```console
$ docker pull memcached@sha256:65ba466bf93c49f07fd340ced359d51a13a74b069cca4de2d034d12f42b92ea4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **96.4 KB (96395 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0e68093b9e036b2a9ff696038b0fd906f66504c0a0cd70dda18954ebb93d4bd1`

```dockerfile
```

-	Layers:
	-	`sha256:b64631288cf2d05d3a1d99eb8cb41f077724b027aaf136bb327f88055e4ceaf4`  
		Last Modified: Tue, 12 Dec 2023 23:20:17 GMT  
		Size: 77.0 KB (77025 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:8ac9ea640f8ca624c147fd0dcc40f859a6284e5f50c4396e0b1e962a4b732813`  
		Last Modified: Tue, 12 Dec 2023 23:20:17 GMT  
		Size: 19.4 KB (19370 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:alpine3.19` - linux; s390x

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

### `memcached:alpine3.19` - unknown; unknown

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

## `memcached:bookworm`

```console
$ docker pull memcached@sha256:5006d1a9ea8a2cedd728d75c2e85cb26c96489f6a039d14ba2c44f99ea310d1c
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 14
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm variant v5
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown
	-	linux; 386
	-	unknown; unknown
	-	linux; mips64le
	-	unknown; unknown
	-	linux; ppc64le
	-	unknown; unknown
	-	linux; s390x
	-	unknown; unknown

### `memcached:bookworm` - linux; amd64

```console
$ docker pull memcached@sha256:0d358fa0198562aa3d1e1c3e9386e1835256875517d8a4786f3dd50a1f65f1de
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.1 MB (41125606 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:03bad2c21b5df5c82f8c581ebec403482a3e00c0f35697ca669c46a7d000a13d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 21 Nov 2023 05:21:37 GMT
ADD file:d261a6f6921593f1e0b3f472ab1b1822e2c6deb0b369200f0b3370556bfad017 in / 
# Tue, 21 Nov 2023 05:21:37 GMT
CMD ["bash"]
# Mon, 04 Dec 2023 18:08:47 GMT
RUN set -eux; 	groupadd --system --gid 11211 memcache; 	useradd --system --gid memcache --uid 11211 memcache # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
ENV MEMCACHED_VERSION=1.6.22
# Mon, 04 Dec 2023 18:08:47 GMT
ENV MEMCACHED_URL=https://memcached.org/files/memcached-1.6.22.tar.gz
# Mon, 04 Dec 2023 18:08:47 GMT
ENV MEMCACHED_SHA1=7a691f390d59616dbebfc9e2e4942d499c39a338
# Mon, 04 Dec 2023 18:08:47 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O memcached.tar.gz "$MEMCACHED_URL"; 	echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c -; 	mkdir -p /usr/src/memcached; 	tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1; 	rm memcached.tar.gz; 		cd /usr/src/memcached; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	; 	nproc="$(nproc)"; 	make -j "$nproc"; 		sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf; 	make test PARALLEL="$nproc"; 	mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf; 		make install; 		cd /; 	rm -rf /usr/src/memcached; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		memcached -V # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 04 Dec 2023 18:08:47 GMT
USER memcache
# Mon, 04 Dec 2023 18:08:47 GMT
EXPOSE map[11211/tcp:{}]
# Mon, 04 Dec 2023 18:08:47 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:1f7ce2fa46ab3942feabee654933948821303a5a821789dddab2d8c3df59e227`  
		Last Modified: Tue, 21 Nov 2023 05:25:58 GMT  
		Size: 29.1 MB (29149908 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:21ac6fd160890cbc46a76542eb3f68654f3e3fb043b1b28a18155ec6863d60bc`  
		Last Modified: Tue, 12 Dec 2023 20:52:57 GMT  
		Size: 1.1 KB (1112 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6330fc82e1304befcc27a7598cd1a85152985d06426f94966788bf5a1583dcc6`  
		Last Modified: Tue, 12 Dec 2023 20:52:57 GMT  
		Size: 2.5 MB (2488284 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4047c827380f04698fbc51155441d719f93b84c1a092d633260c704f286296dd`  
		Last Modified: Tue, 12 Dec 2023 20:52:57 GMT  
		Size: 9.5 MB (9485895 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:401b5de2a4f8d9f588888754fa8347b67590c776363770f46ef67688116a4a0c`  
		Last Modified: Tue, 12 Dec 2023 20:52:57 GMT  
		Size: 285.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ee899f9aed95096580ea4a2325fd4824518ff1621f433f393fa253b52b7294b5`  
		Last Modified: Tue, 12 Dec 2023 20:52:58 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:bookworm` - unknown; unknown

```console
$ docker pull memcached@sha256:5ccb88c1a86bd6524b6d5c9383254cdd79314d656a0c982658ecd35d9716431b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 MB (3077929 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:238ef9023561adc9c09faf875c5370cb2711a83cc7327dcc49ae7f8255c23794`

```dockerfile
```

-	Layers:
	-	`sha256:f84a6f3d0bdab8613be68ff091a6a78bedf8f697d4df55ff90ac7b745337e72c`  
		Last Modified: Tue, 12 Dec 2023 20:52:57 GMT  
		Size: 3.1 MB (3056812 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:8d7aee053ab87a86e42ba3d14810d3f1918c6e66d4d3ef02bc9c741f3948b83e`  
		Last Modified: Tue, 12 Dec 2023 20:52:57 GMT  
		Size: 21.1 KB (21117 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:bookworm` - linux; arm variant v5

```console
$ docker pull memcached@sha256:cb9426984b18b2d3df1c5fbb2bb7e2e9ebe08325d4adce6d0cd7a9207c413476
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.1 MB (37113170 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a8f2fb6119b629983f190d8b73208a156991d8cb65c47579a68125c339e9c75`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 21 Nov 2023 05:00:51 GMT
ADD file:1ae8e5ac45b11d01083680b765e1fcfef9f7938f89d6f424572126fa946d8cdf in / 
# Tue, 21 Nov 2023 05:00:52 GMT
CMD ["bash"]
# Mon, 04 Dec 2023 18:08:47 GMT
RUN set -eux; 	groupadd --system --gid 11211 memcache; 	useradd --system --gid memcache --uid 11211 memcache # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
ENV MEMCACHED_VERSION=1.6.22
# Mon, 04 Dec 2023 18:08:47 GMT
ENV MEMCACHED_URL=https://memcached.org/files/memcached-1.6.22.tar.gz
# Mon, 04 Dec 2023 18:08:47 GMT
ENV MEMCACHED_SHA1=7a691f390d59616dbebfc9e2e4942d499c39a338
# Mon, 04 Dec 2023 18:08:47 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O memcached.tar.gz "$MEMCACHED_URL"; 	echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c -; 	mkdir -p /usr/src/memcached; 	tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1; 	rm memcached.tar.gz; 		cd /usr/src/memcached; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	; 	nproc="$(nproc)"; 	make -j "$nproc"; 		sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf; 	make test PARALLEL="$nproc"; 	mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf; 		make install; 		cd /; 	rm -rf /usr/src/memcached; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		memcached -V # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 04 Dec 2023 18:08:47 GMT
USER memcache
# Mon, 04 Dec 2023 18:08:47 GMT
EXPOSE map[11211/tcp:{}]
# Mon, 04 Dec 2023 18:08:47 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:f476aef5b6e1122850e68c81ef06fc2df17e968961b060483b4d2fb33018aae3`  
		Last Modified: Tue, 21 Nov 2023 05:03:55 GMT  
		Size: 26.9 MB (26922153 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:89367ca16d2c3104d44514e1b9b94b0ac4070ea0f6f04523c72dda62795f3a17`  
		Last Modified: Tue, 12 Dec 2023 21:47:13 GMT  
		Size: 1.1 KB (1110 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5ecbc6577cf78c09bd4136f78a57a904ae1ab705fce8595e8d1187d800158e6f`  
		Last Modified: Tue, 12 Dec 2023 21:47:14 GMT  
		Size: 2.1 MB (2089289 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:12f8a270079b04e1372c73cc16ff2ae33e6f6ee0dcc7e8ed57843fca20b3d038`  
		Last Modified: Tue, 12 Dec 2023 21:47:14 GMT  
		Size: 8.1 MB (8100211 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5f592556023f9ba6125ecf6b89156ba61c05526ad324708c3d2a09600ee5e7e4`  
		Last Modified: Tue, 12 Dec 2023 21:47:14 GMT  
		Size: 285.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fa757a09f6a7a23114a13869f15b229384628cf108567d395dc0d4730c685409`  
		Last Modified: Tue, 12 Dec 2023 21:47:14 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:bookworm` - unknown; unknown

```console
$ docker pull memcached@sha256:0c93e2660a508733f1c7d5236af77ef81fbcd0b27e4ac55c81d83334c8794891
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.0 KB (21043 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:538fbf714aa2f8a4175400dd43b0715e416f73fe598fc50d3f763afa144595da`

```dockerfile
```

-	Layers:
	-	`sha256:f65b3a9a0f6936cae3c1e411ecdd846d754a1978d851fdacf4b25526cb9ff4cc`  
		Last Modified: Tue, 12 Dec 2023 21:47:14 GMT  
		Size: 21.0 KB (21043 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:bookworm` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:c5adc5a4207d95c96a36131c2d39085b082f0e22f4595b935e72bcb463c10383
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.0 MB (39979924 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf26c17403ed5a4db96ddd8b41aeb2fd45483f897882a57972c994c95a44c5dd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 21 Nov 2023 06:27:06 GMT
ADD file:869c7d0747a17c53715581a2e862992eb8516c7f45f167821dfa80966a4870d1 in / 
# Tue, 21 Nov 2023 06:27:06 GMT
CMD ["bash"]
# Mon, 04 Dec 2023 18:08:47 GMT
RUN set -eux; 	groupadd --system --gid 11211 memcache; 	useradd --system --gid memcache --uid 11211 memcache # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
ENV MEMCACHED_VERSION=1.6.22
# Mon, 04 Dec 2023 18:08:47 GMT
ENV MEMCACHED_URL=https://memcached.org/files/memcached-1.6.22.tar.gz
# Mon, 04 Dec 2023 18:08:47 GMT
ENV MEMCACHED_SHA1=7a691f390d59616dbebfc9e2e4942d499c39a338
# Mon, 04 Dec 2023 18:08:47 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O memcached.tar.gz "$MEMCACHED_URL"; 	echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c -; 	mkdir -p /usr/src/memcached; 	tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1; 	rm memcached.tar.gz; 		cd /usr/src/memcached; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	; 	nproc="$(nproc)"; 	make -j "$nproc"; 		sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf; 	make test PARALLEL="$nproc"; 	mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf; 		make install; 		cd /; 	rm -rf /usr/src/memcached; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		memcached -V # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 04 Dec 2023 18:08:47 GMT
USER memcache
# Mon, 04 Dec 2023 18:08:47 GMT
EXPOSE map[11211/tcp:{}]
# Mon, 04 Dec 2023 18:08:47 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:2c6d21737d8318aa15c4cc838475029a5efc36c0429e3d8da80d97d0b96d9aaf`  
		Last Modified: Tue, 21 Nov 2023 06:30:30 GMT  
		Size: 29.2 MB (29179277 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1a39d6fec0d552a8078ab223bafd58bc9a0c8c27c26600a5b95c6a521bb97f3d`  
		Last Modified: Tue, 12 Dec 2023 23:43:17 GMT  
		Size: 1.1 KB (1112 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9d1ceea69964553dd3aaf853e0d7b753495cab4623b9377c69096be0bdf88146`  
		Last Modified: Tue, 12 Dec 2023 23:43:17 GMT  
		Size: 2.3 MB (2345975 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:52063b8e37cbc1e5e6e3af0f54b834ae3f6a53d023349ae819c9607e5fc98aec`  
		Last Modified: Tue, 12 Dec 2023 23:43:17 GMT  
		Size: 8.5 MB (8453155 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5b99d0095a64f8110efee1f5e91754cc923294d50c9e2927e515354746a3f465`  
		Last Modified: Tue, 12 Dec 2023 23:43:17 GMT  
		Size: 284.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:913c9e21eaa9c49c99b1b39e5cda0ef12356220075c869ea4776dca36fe83b75`  
		Last Modified: Tue, 12 Dec 2023 23:43:18 GMT  
		Size: 121.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:bookworm` - unknown; unknown

```console
$ docker pull memcached@sha256:3d519a2eb9e00b43e6bc7584f6962b12ba032c4487a6e4ef7fd2b00b667bc90d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 MB (3053138 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9cc25288d58197dcc1309ea4a8128d0b120b92ad2d877f226095cd4847696474`

```dockerfile
```

-	Layers:
	-	`sha256:c5edc5ba98b4e6a438caa0d4541784c5c1e8b23d6020bc0b2a5b9910d0725400`  
		Last Modified: Tue, 12 Dec 2023 23:43:17 GMT  
		Size: 3.0 MB (3032003 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:b15e35765293b6f1da0e628c94108f229423c5a6379b8b5c47a41415f377b6d8`  
		Last Modified: Tue, 12 Dec 2023 23:43:17 GMT  
		Size: 21.1 KB (21135 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:bookworm` - linux; 386

```console
$ docker pull memcached@sha256:fa9dba8086765d68f2feecfc2ac08fb29c019597d09943bb480227e6cba87666
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.3 MB (39294993 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:93047050e75b6d4d64adb8a7c8f68cb118bad27ca9dc772120e251b174752cf9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 16 Oct 2023 06:54:12 GMT
ADD file:0c94521fdd9c0a4fdeeb9aad23e68cd053fba0dcd7c3af550aefa79377816e31 in / 
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["bash"]
# Mon, 16 Oct 2023 06:54:12 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_VERSION=1.6.22
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_SHA1=7a691f390d59616dbebfc9e2e4942d499c39a338
# Mon, 16 Oct 2023 06:54:12 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V # buildkit
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
	-	`sha256:98bdfce9af831c2a0d0bfcca812d0039cd1666986550f552b4b4c625bd5aa31c`  
		Last Modified: Wed, 01 Nov 2023 00:43:26 GMT  
		Size: 30.2 MB (30164042 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1b647d4b10cf20ac5807101c7d0380701be684aa82f5c01ec41f674b5ef23d42`  
		Last Modified: Wed, 01 Nov 2023 01:06:49 GMT  
		Size: 1.1 KB (1109 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b61c058003459de4911c2901b2d799b03de754a1b9e64ffbe21a04992e962e62`  
		Last Modified: Wed, 01 Nov 2023 01:06:49 GMT  
		Size: 2.5 MB (2492501 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:810b6db64df2fcc8f76941cdac75093cf35bd72ac3cd1fa5eb664e74c1f67cd8`  
		Last Modified: Wed, 01 Nov 2023 01:06:50 GMT  
		Size: 6.6 MB (6636937 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:dbb899942df4149bd5fae8bac6e295285ec80f82d621f2b29c931ee348491cfb`  
		Last Modified: Wed, 01 Nov 2023 01:06:49 GMT  
		Size: 282.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4a8530160ab232c37c0ddcbf5e3a731d835d378d1382843957f6c2a73b2b5be6`  
		Last Modified: Wed, 01 Nov 2023 01:06:50 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:bookworm` - unknown; unknown

```console
$ docker pull memcached@sha256:dd7ce9519c31365127142232df2ed0b285e9acc03cd77c23c838bf932165def8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.5 KB (21498 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eef82c92e07c11a92c337806d01cfb1c6cdc7a16608dcf304a38de34d2ef1dbb`

```dockerfile
```

-	Layers:
	-	`sha256:c0d9dd22513f8d3e791e1796d7ef1906e57c798c92dd35d0be9cf2eaecec5954`  
		Last Modified: Wed, 01 Nov 2023 01:06:49 GMT  
		Size: 21.5 KB (21498 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:bookworm` - linux; mips64le

```console
$ docker pull memcached@sha256:9f7696d5078cf83e8b152cb00a3615576fd3c50d10be9253b9c188e16bfd8087
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.9 MB (39863164 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:685886644cfb343923260c15c66eb8c8d8bf7b84b6b1e855732aec2359b6ae29`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 21 Nov 2023 04:09:50 GMT
ADD file:e093749192323dc72b60a8440ddba26c415586f618b5e107fa264ba5eb2ca7ba in / 
# Tue, 21 Nov 2023 04:09:54 GMT
CMD ["bash"]
# Mon, 04 Dec 2023 18:08:47 GMT
RUN set -eux; 	groupadd --system --gid 11211 memcache; 	useradd --system --gid memcache --uid 11211 memcache # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
ENV MEMCACHED_VERSION=1.6.22
# Mon, 04 Dec 2023 18:08:47 GMT
ENV MEMCACHED_URL=https://memcached.org/files/memcached-1.6.22.tar.gz
# Mon, 04 Dec 2023 18:08:47 GMT
ENV MEMCACHED_SHA1=7a691f390d59616dbebfc9e2e4942d499c39a338
# Mon, 04 Dec 2023 18:08:47 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O memcached.tar.gz "$MEMCACHED_URL"; 	echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c -; 	mkdir -p /usr/src/memcached; 	tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1; 	rm memcached.tar.gz; 		cd /usr/src/memcached; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	; 	nproc="$(nproc)"; 	make -j "$nproc"; 		sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf; 	make test PARALLEL="$nproc"; 	mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf; 		make install; 		cd /; 	rm -rf /usr/src/memcached; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		memcached -V # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 04 Dec 2023 18:08:47 GMT
USER memcache
# Mon, 04 Dec 2023 18:08:47 GMT
EXPOSE map[11211/tcp:{}]
# Mon, 04 Dec 2023 18:08:47 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:ebdff2138fee4a3ec27560ab1353dc51c12c2608ff721f5db3d24104872b702a`  
		Last Modified: Tue, 21 Nov 2023 04:20:35 GMT  
		Size: 29.1 MB (29141984 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ee63ae82c6a87dc28cedafb91fbd6eaccd22add5b00a9cceb208472b30427b5d`  
		Last Modified: Tue, 12 Dec 2023 23:10:03 GMT  
		Size: 1.1 KB (1114 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3d430991f88102b07bcf8bf22f07667e49c9dfedb134b0ac36ddbb99d1e79db2`  
		Last Modified: Tue, 12 Dec 2023 23:10:04 GMT  
		Size: 1.9 MB (1937475 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ebe1140b392e915b8757b8d0a4b83f0aaf2103734e9f83c318821f641207b6b4`  
		Last Modified: Tue, 12 Dec 2023 23:10:04 GMT  
		Size: 8.8 MB (8782185 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:aedf1130e49a6aa7d9b74b9fd00914b171966fcf8beba71095787811fa3a0284`  
		Last Modified: Tue, 12 Dec 2023 23:10:03 GMT  
		Size: 284.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:457e2691e0499a1a1d26e6da85567f20a8dc396bde9d9952ce75fdcfe6cbafd8`  
		Last Modified: Tue, 12 Dec 2023 23:10:05 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:bookworm` - unknown; unknown

```console
$ docker pull memcached@sha256:d48752667ff111ef73342ae5c16218a373275e8b65c7696eff231ff49ca7b8e5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.0 KB (21004 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9138b1207d88c6ca6b32a2616d3c25b1f5d3280b7650ac4bfa7120518f6a8ad7`

```dockerfile
```

-	Layers:
	-	`sha256:2b1c5f3190ac8dfdff54a51d9421ad623af991deba1a46ba943cf88442079207`  
		Last Modified: Tue, 12 Dec 2023 23:10:03 GMT  
		Size: 21.0 KB (21004 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:bookworm` - linux; ppc64le

```console
$ docker pull memcached@sha256:813f2ed7d8d4d2c4e6f4a19816964b0c95cc56d038d95d059571d51e115ab109
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.5 MB (45508655 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:73c79988c4d09a9ac9cb01aa05096b344821e8034c3cba04afb9cb78fe25db05`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 21 Nov 2023 04:24:14 GMT
ADD file:8b22a531b6611a1e63dfc20e4e2931592e2d821bd4b64c4b2810bb9a36640c02 in / 
# Tue, 21 Nov 2023 04:24:16 GMT
CMD ["bash"]
# Mon, 04 Dec 2023 18:08:47 GMT
RUN set -eux; 	groupadd --system --gid 11211 memcache; 	useradd --system --gid memcache --uid 11211 memcache # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
ENV MEMCACHED_VERSION=1.6.22
# Mon, 04 Dec 2023 18:08:47 GMT
ENV MEMCACHED_URL=https://memcached.org/files/memcached-1.6.22.tar.gz
# Mon, 04 Dec 2023 18:08:47 GMT
ENV MEMCACHED_SHA1=7a691f390d59616dbebfc9e2e4942d499c39a338
# Mon, 04 Dec 2023 18:08:47 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O memcached.tar.gz "$MEMCACHED_URL"; 	echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c -; 	mkdir -p /usr/src/memcached; 	tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1; 	rm memcached.tar.gz; 		cd /usr/src/memcached; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	; 	nproc="$(nproc)"; 	make -j "$nproc"; 		sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf; 	make test PARALLEL="$nproc"; 	mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf; 		make install; 		cd /; 	rm -rf /usr/src/memcached; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		memcached -V # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 04 Dec 2023 18:08:47 GMT
USER memcache
# Mon, 04 Dec 2023 18:08:47 GMT
EXPOSE map[11211/tcp:{}]
# Mon, 04 Dec 2023 18:08:47 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:c570d04e61d8e35a3c8f12179d048d701451f97f9cf2099ea3e3738512dbf062`  
		Last Modified: Tue, 21 Nov 2023 04:28:58 GMT  
		Size: 33.1 MB (33141607 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b53469d03d0156e89526c2b744f6850b65cfb9b509a6fda4c523764f7a9f9072`  
		Last Modified: Tue, 12 Dec 2023 23:08:09 GMT  
		Size: 1.1 KB (1111 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:12b61a5974195d80345022ed47cb4546f6fec60527b3932b2ce74d605db750e0`  
		Last Modified: Tue, 12 Dec 2023 23:08:09 GMT  
		Size: 2.7 MB (2698202 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:108f5df7a0010e4f69929c6ce4ff2e0e53877c6bbe11bd86acbbb0e7b608dca7`  
		Last Modified: Tue, 12 Dec 2023 23:08:09 GMT  
		Size: 9.7 MB (9667330 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:aa53d1e0a6b1123a31838e581de8d738ccaf05c9be569ec50b8d37cbc54a99bd`  
		Last Modified: Tue, 12 Dec 2023 23:08:08 GMT  
		Size: 283.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2cf8ef0b438a2029bfc9b928364eb71966baa4990e2ac4a9b1648cbd44271dc4`  
		Last Modified: Tue, 12 Dec 2023 23:08:10 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:bookworm` - unknown; unknown

```console
$ docker pull memcached@sha256:d75efc7b8726fbfade0b41c14205058def09ee997a7befb495808c2752a56a54
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 MB (3066416 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ca8bb0be2316bb58a60c953382dd1963eb7e265d0602de370e02152e1ac84d7`

```dockerfile
```

-	Layers:
	-	`sha256:34203b346608565cdbcd7cf9a56efb8ec2255b1a8f30267d6b2749d6a0bd2d6b`  
		Last Modified: Tue, 12 Dec 2023 23:08:09 GMT  
		Size: 3.0 MB (3045398 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:4da4f2a55f1773bfac75983e2e733c609b970884e935de987ec5b3ec5c92eb85`  
		Last Modified: Tue, 12 Dec 2023 23:08:08 GMT  
		Size: 21.0 KB (21018 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:bookworm` - linux; s390x

```console
$ docker pull memcached@sha256:05084fffc798db32442e2cde93eac5815ffd909e9bf65692ac08c9b5ab79e677
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.0 MB (38041790 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eac80baab625f3daf940cdb3053e2e709bd61d78d7eae50b7db4d71f87bcd149`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 21 Nov 2023 05:04:35 GMT
ADD file:c33fa9fdde73983850798b6eb1cd062e0398109d1d773e6a937fead7475c8efc in / 
# Tue, 21 Nov 2023 05:04:41 GMT
CMD ["bash"]
# Mon, 04 Dec 2023 18:08:47 GMT
RUN set -eux; 	groupadd --system --gid 11211 memcache; 	useradd --system --gid memcache --uid 11211 memcache # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
ENV MEMCACHED_VERSION=1.6.22
# Mon, 04 Dec 2023 18:08:47 GMT
ENV MEMCACHED_URL=https://memcached.org/files/memcached-1.6.22.tar.gz
# Mon, 04 Dec 2023 18:08:47 GMT
ENV MEMCACHED_SHA1=7a691f390d59616dbebfc9e2e4942d499c39a338
# Mon, 04 Dec 2023 18:08:47 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O memcached.tar.gz "$MEMCACHED_URL"; 	echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c -; 	mkdir -p /usr/src/memcached; 	tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1; 	rm memcached.tar.gz; 		cd /usr/src/memcached; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	; 	nproc="$(nproc)"; 	make -j "$nproc"; 		sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf; 	make test PARALLEL="$nproc"; 	mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf; 		make install; 		cd /; 	rm -rf /usr/src/memcached; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		memcached -V # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 04 Dec 2023 18:08:47 GMT
USER memcache
# Mon, 04 Dec 2023 18:08:47 GMT
EXPOSE map[11211/tcp:{}]
# Mon, 04 Dec 2023 18:08:47 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:6daa625e5a040476e253e7acd0befa74254a4865ec836d6334a544d82a21d4be`  
		Last Modified: Tue, 21 Nov 2023 05:10:21 GMT  
		Size: 27.5 MB (27512885 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b19a3143cbec7ddc9a646dbbe779b0b5ec67662cf70e280db146f6ace54ccd61`  
		Last Modified: Wed, 13 Dec 2023 00:26:35 GMT  
		Size: 1.1 KB (1111 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b8af028b1fa76aa55f540dd5be5eaf89eea3fec23e09e9a88550aac36e9ee843`  
		Last Modified: Wed, 13 Dec 2023 00:26:35 GMT  
		Size: 2.2 MB (2152508 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9a774943469875a0902c53fccdd95cad9c18234b759bcdcc5816bd563deb7f14`  
		Last Modified: Wed, 13 Dec 2023 00:26:35 GMT  
		Size: 8.4 MB (8374880 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:266b4bf499a815da6f7ddcf68e1e61f8418c8ec655a2083e174aaa385de74d76`  
		Last Modified: Wed, 13 Dec 2023 00:26:35 GMT  
		Size: 284.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0da709e3482cc552b0a7b69eb05aaa21af1e74baaf4e3bccc34e95e478943630`  
		Last Modified: Wed, 13 Dec 2023 00:26:36 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:bookworm` - unknown; unknown

```console
$ docker pull memcached@sha256:525abad348ba03c5b9444f23409d647581284c1642d30539e2c9943405266f12
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 MB (3067303 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e3b551ec9122d039520bbd13bced5b1f5b0d5b1fd9e32c09a1d4536f7af1226`

```dockerfile
```

-	Layers:
	-	`sha256:5cc0958f61715f0746d9fa2a8a5c06f31608bb5d1cf32d606c46fc8e11b35984`  
		Last Modified: Wed, 13 Dec 2023 00:26:35 GMT  
		Size: 3.0 MB (3046353 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:3d2fed99d3355e42a820c1975105411eb7584cffb111d7e1fd541603f7721f1c`  
		Last Modified: Wed, 13 Dec 2023 00:26:35 GMT  
		Size: 20.9 KB (20950 bytes)  
		MIME: application/vnd.in-toto+json

## `memcached:latest`

```console
$ docker pull memcached@sha256:c0aa354cc777aa9bdbaf3789db81b1b1802be11940498801dbe1562999d5671e
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 15
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm variant v5
	-	unknown; unknown
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	unknown; unknown
	-	linux; 386
	-	unknown; unknown
	-	linux; mips64le
	-	unknown; unknown
	-	linux; ppc64le
	-	unknown; unknown
	-	linux; s390x
	-	unknown; unknown

### `memcached:latest` - linux; amd64

```console
$ docker pull memcached@sha256:0d358fa0198562aa3d1e1c3e9386e1835256875517d8a4786f3dd50a1f65f1de
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.1 MB (41125606 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:03bad2c21b5df5c82f8c581ebec403482a3e00c0f35697ca669c46a7d000a13d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 21 Nov 2023 05:21:37 GMT
ADD file:d261a6f6921593f1e0b3f472ab1b1822e2c6deb0b369200f0b3370556bfad017 in / 
# Tue, 21 Nov 2023 05:21:37 GMT
CMD ["bash"]
# Mon, 04 Dec 2023 18:08:47 GMT
RUN set -eux; 	groupadd --system --gid 11211 memcache; 	useradd --system --gid memcache --uid 11211 memcache # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
ENV MEMCACHED_VERSION=1.6.22
# Mon, 04 Dec 2023 18:08:47 GMT
ENV MEMCACHED_URL=https://memcached.org/files/memcached-1.6.22.tar.gz
# Mon, 04 Dec 2023 18:08:47 GMT
ENV MEMCACHED_SHA1=7a691f390d59616dbebfc9e2e4942d499c39a338
# Mon, 04 Dec 2023 18:08:47 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O memcached.tar.gz "$MEMCACHED_URL"; 	echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c -; 	mkdir -p /usr/src/memcached; 	tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1; 	rm memcached.tar.gz; 		cd /usr/src/memcached; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	; 	nproc="$(nproc)"; 	make -j "$nproc"; 		sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf; 	make test PARALLEL="$nproc"; 	mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf; 		make install; 		cd /; 	rm -rf /usr/src/memcached; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		memcached -V # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 04 Dec 2023 18:08:47 GMT
USER memcache
# Mon, 04 Dec 2023 18:08:47 GMT
EXPOSE map[11211/tcp:{}]
# Mon, 04 Dec 2023 18:08:47 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:1f7ce2fa46ab3942feabee654933948821303a5a821789dddab2d8c3df59e227`  
		Last Modified: Tue, 21 Nov 2023 05:25:58 GMT  
		Size: 29.1 MB (29149908 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:21ac6fd160890cbc46a76542eb3f68654f3e3fb043b1b28a18155ec6863d60bc`  
		Last Modified: Tue, 12 Dec 2023 20:52:57 GMT  
		Size: 1.1 KB (1112 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6330fc82e1304befcc27a7598cd1a85152985d06426f94966788bf5a1583dcc6`  
		Last Modified: Tue, 12 Dec 2023 20:52:57 GMT  
		Size: 2.5 MB (2488284 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4047c827380f04698fbc51155441d719f93b84c1a092d633260c704f286296dd`  
		Last Modified: Tue, 12 Dec 2023 20:52:57 GMT  
		Size: 9.5 MB (9485895 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:401b5de2a4f8d9f588888754fa8347b67590c776363770f46ef67688116a4a0c`  
		Last Modified: Tue, 12 Dec 2023 20:52:57 GMT  
		Size: 285.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ee899f9aed95096580ea4a2325fd4824518ff1621f433f393fa253b52b7294b5`  
		Last Modified: Tue, 12 Dec 2023 20:52:58 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:latest` - unknown; unknown

```console
$ docker pull memcached@sha256:5ccb88c1a86bd6524b6d5c9383254cdd79314d656a0c982658ecd35d9716431b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 MB (3077929 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:238ef9023561adc9c09faf875c5370cb2711a83cc7327dcc49ae7f8255c23794`

```dockerfile
```

-	Layers:
	-	`sha256:f84a6f3d0bdab8613be68ff091a6a78bedf8f697d4df55ff90ac7b745337e72c`  
		Last Modified: Tue, 12 Dec 2023 20:52:57 GMT  
		Size: 3.1 MB (3056812 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:8d7aee053ab87a86e42ba3d14810d3f1918c6e66d4d3ef02bc9c741f3948b83e`  
		Last Modified: Tue, 12 Dec 2023 20:52:57 GMT  
		Size: 21.1 KB (21117 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:latest` - linux; arm variant v5

```console
$ docker pull memcached@sha256:cb9426984b18b2d3df1c5fbb2bb7e2e9ebe08325d4adce6d0cd7a9207c413476
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.1 MB (37113170 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a8f2fb6119b629983f190d8b73208a156991d8cb65c47579a68125c339e9c75`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 21 Nov 2023 05:00:51 GMT
ADD file:1ae8e5ac45b11d01083680b765e1fcfef9f7938f89d6f424572126fa946d8cdf in / 
# Tue, 21 Nov 2023 05:00:52 GMT
CMD ["bash"]
# Mon, 04 Dec 2023 18:08:47 GMT
RUN set -eux; 	groupadd --system --gid 11211 memcache; 	useradd --system --gid memcache --uid 11211 memcache # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
ENV MEMCACHED_VERSION=1.6.22
# Mon, 04 Dec 2023 18:08:47 GMT
ENV MEMCACHED_URL=https://memcached.org/files/memcached-1.6.22.tar.gz
# Mon, 04 Dec 2023 18:08:47 GMT
ENV MEMCACHED_SHA1=7a691f390d59616dbebfc9e2e4942d499c39a338
# Mon, 04 Dec 2023 18:08:47 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O memcached.tar.gz "$MEMCACHED_URL"; 	echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c -; 	mkdir -p /usr/src/memcached; 	tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1; 	rm memcached.tar.gz; 		cd /usr/src/memcached; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	; 	nproc="$(nproc)"; 	make -j "$nproc"; 		sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf; 	make test PARALLEL="$nproc"; 	mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf; 		make install; 		cd /; 	rm -rf /usr/src/memcached; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		memcached -V # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 04 Dec 2023 18:08:47 GMT
USER memcache
# Mon, 04 Dec 2023 18:08:47 GMT
EXPOSE map[11211/tcp:{}]
# Mon, 04 Dec 2023 18:08:47 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:f476aef5b6e1122850e68c81ef06fc2df17e968961b060483b4d2fb33018aae3`  
		Last Modified: Tue, 21 Nov 2023 05:03:55 GMT  
		Size: 26.9 MB (26922153 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:89367ca16d2c3104d44514e1b9b94b0ac4070ea0f6f04523c72dda62795f3a17`  
		Last Modified: Tue, 12 Dec 2023 21:47:13 GMT  
		Size: 1.1 KB (1110 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5ecbc6577cf78c09bd4136f78a57a904ae1ab705fce8595e8d1187d800158e6f`  
		Last Modified: Tue, 12 Dec 2023 21:47:14 GMT  
		Size: 2.1 MB (2089289 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:12f8a270079b04e1372c73cc16ff2ae33e6f6ee0dcc7e8ed57843fca20b3d038`  
		Last Modified: Tue, 12 Dec 2023 21:47:14 GMT  
		Size: 8.1 MB (8100211 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5f592556023f9ba6125ecf6b89156ba61c05526ad324708c3d2a09600ee5e7e4`  
		Last Modified: Tue, 12 Dec 2023 21:47:14 GMT  
		Size: 285.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fa757a09f6a7a23114a13869f15b229384628cf108567d395dc0d4730c685409`  
		Last Modified: Tue, 12 Dec 2023 21:47:14 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:latest` - unknown; unknown

```console
$ docker pull memcached@sha256:0c93e2660a508733f1c7d5236af77ef81fbcd0b27e4ac55c81d83334c8794891
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.0 KB (21043 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:538fbf714aa2f8a4175400dd43b0715e416f73fe598fc50d3f763afa144595da`

```dockerfile
```

-	Layers:
	-	`sha256:f65b3a9a0f6936cae3c1e411ecdd846d754a1978d851fdacf4b25526cb9ff4cc`  
		Last Modified: Tue, 12 Dec 2023 21:47:14 GMT  
		Size: 21.0 KB (21043 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:latest` - linux; arm variant v7

```console
$ docker pull memcached@sha256:2841be0a36134563966c09a6ed68b21053d20342ec8736cf92763c28077ead43
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.1 MB (28094215 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6cf74ffa940dd93988fc0beb6698c5796563c82a40b7dd668153969f64d2e6ca`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 09 Feb 2023 06:12:09 GMT
ADD file:5f1a343224e8486690bd90dd1e50c8d84b3d770c51bb6829544e5cf650c0419c in / 
# Thu, 09 Feb 2023 06:12:10 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 07:52:31 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Thu, 09 Feb 2023 07:52:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 07:52:35 GMT
ENV MEMCACHED_VERSION=1.6.18
# Thu, 09 Feb 2023 07:52:35 GMT
ENV MEMCACHED_SHA1=be16909bb75ab972ee5fe438312501de01c4725a
# Thu, 09 Feb 2023 07:55:44 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 09 Feb 2023 07:55:44 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 09 Feb 2023 07:55:44 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 09 Feb 2023 07:55:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 09 Feb 2023 07:55:44 GMT
USER memcache
# Thu, 09 Feb 2023 07:55:45 GMT
EXPOSE 11211
# Thu, 09 Feb 2023 07:55:45 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:e7318f6106ad75d7d482ae9dddf4d927b0872ef3ddb6e1330aa691fc8d17279e`  
		Last Modified: Thu, 09 Feb 2023 06:19:19 GMT  
		Size: 26.6 MB (26577666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de49d9d72daf1680b5f1b9532dd2eb0162829f36c8db9669935462636fbf99d9`  
		Last Modified: Thu, 09 Feb 2023 08:06:11 GMT  
		Size: 4.9 KB (4895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0beac9d5bcac946f8c54c72b8a9c136914b1aa7a5fe2b8c3df4c7d8858ea6559`  
		Last Modified: Thu, 09 Feb 2023 08:06:11 GMT  
		Size: 312.1 KB (312088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4c9e5a265394e4c0f357779e6195a4e82d767a3691a0e77d427e56651c3e54a`  
		Last Modified: Thu, 09 Feb 2023 08:06:11 GMT  
		Size: 1.2 MB (1199163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5ea82ad892fe1ae8623d84e32c8c027087cda8aa49e40d4546ed6942e471c60`  
		Last Modified: Thu, 09 Feb 2023 08:06:11 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa2ae3bcdc0d114ba49a67df022b6f7215fc87f1f50e64939fcfbbec4eaadee5`  
		Last Modified: Thu, 09 Feb 2023 08:06:11 GMT  
		Size: 118.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:latest` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:c5adc5a4207d95c96a36131c2d39085b082f0e22f4595b935e72bcb463c10383
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.0 MB (39979924 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf26c17403ed5a4db96ddd8b41aeb2fd45483f897882a57972c994c95a44c5dd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 21 Nov 2023 06:27:06 GMT
ADD file:869c7d0747a17c53715581a2e862992eb8516c7f45f167821dfa80966a4870d1 in / 
# Tue, 21 Nov 2023 06:27:06 GMT
CMD ["bash"]
# Mon, 04 Dec 2023 18:08:47 GMT
RUN set -eux; 	groupadd --system --gid 11211 memcache; 	useradd --system --gid memcache --uid 11211 memcache # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
ENV MEMCACHED_VERSION=1.6.22
# Mon, 04 Dec 2023 18:08:47 GMT
ENV MEMCACHED_URL=https://memcached.org/files/memcached-1.6.22.tar.gz
# Mon, 04 Dec 2023 18:08:47 GMT
ENV MEMCACHED_SHA1=7a691f390d59616dbebfc9e2e4942d499c39a338
# Mon, 04 Dec 2023 18:08:47 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O memcached.tar.gz "$MEMCACHED_URL"; 	echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c -; 	mkdir -p /usr/src/memcached; 	tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1; 	rm memcached.tar.gz; 		cd /usr/src/memcached; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	; 	nproc="$(nproc)"; 	make -j "$nproc"; 		sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf; 	make test PARALLEL="$nproc"; 	mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf; 		make install; 		cd /; 	rm -rf /usr/src/memcached; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		memcached -V # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 04 Dec 2023 18:08:47 GMT
USER memcache
# Mon, 04 Dec 2023 18:08:47 GMT
EXPOSE map[11211/tcp:{}]
# Mon, 04 Dec 2023 18:08:47 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:2c6d21737d8318aa15c4cc838475029a5efc36c0429e3d8da80d97d0b96d9aaf`  
		Last Modified: Tue, 21 Nov 2023 06:30:30 GMT  
		Size: 29.2 MB (29179277 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1a39d6fec0d552a8078ab223bafd58bc9a0c8c27c26600a5b95c6a521bb97f3d`  
		Last Modified: Tue, 12 Dec 2023 23:43:17 GMT  
		Size: 1.1 KB (1112 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9d1ceea69964553dd3aaf853e0d7b753495cab4623b9377c69096be0bdf88146`  
		Last Modified: Tue, 12 Dec 2023 23:43:17 GMT  
		Size: 2.3 MB (2345975 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:52063b8e37cbc1e5e6e3af0f54b834ae3f6a53d023349ae819c9607e5fc98aec`  
		Last Modified: Tue, 12 Dec 2023 23:43:17 GMT  
		Size: 8.5 MB (8453155 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5b99d0095a64f8110efee1f5e91754cc923294d50c9e2927e515354746a3f465`  
		Last Modified: Tue, 12 Dec 2023 23:43:17 GMT  
		Size: 284.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:913c9e21eaa9c49c99b1b39e5cda0ef12356220075c869ea4776dca36fe83b75`  
		Last Modified: Tue, 12 Dec 2023 23:43:18 GMT  
		Size: 121.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:latest` - unknown; unknown

```console
$ docker pull memcached@sha256:3d519a2eb9e00b43e6bc7584f6962b12ba032c4487a6e4ef7fd2b00b667bc90d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 MB (3053138 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9cc25288d58197dcc1309ea4a8128d0b120b92ad2d877f226095cd4847696474`

```dockerfile
```

-	Layers:
	-	`sha256:c5edc5ba98b4e6a438caa0d4541784c5c1e8b23d6020bc0b2a5b9910d0725400`  
		Last Modified: Tue, 12 Dec 2023 23:43:17 GMT  
		Size: 3.0 MB (3032003 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:b15e35765293b6f1da0e628c94108f229423c5a6379b8b5c47a41415f377b6d8`  
		Last Modified: Tue, 12 Dec 2023 23:43:17 GMT  
		Size: 21.1 KB (21135 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:latest` - linux; 386

```console
$ docker pull memcached@sha256:fa9dba8086765d68f2feecfc2ac08fb29c019597d09943bb480227e6cba87666
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.3 MB (39294993 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:93047050e75b6d4d64adb8a7c8f68cb118bad27ca9dc772120e251b174752cf9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 16 Oct 2023 06:54:12 GMT
ADD file:0c94521fdd9c0a4fdeeb9aad23e68cd053fba0dcd7c3af550aefa79377816e31 in / 
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["bash"]
# Mon, 16 Oct 2023 06:54:12 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_VERSION=1.6.22
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_SHA1=7a691f390d59616dbebfc9e2e4942d499c39a338
# Mon, 16 Oct 2023 06:54:12 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V # buildkit
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
	-	`sha256:98bdfce9af831c2a0d0bfcca812d0039cd1666986550f552b4b4c625bd5aa31c`  
		Last Modified: Wed, 01 Nov 2023 00:43:26 GMT  
		Size: 30.2 MB (30164042 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1b647d4b10cf20ac5807101c7d0380701be684aa82f5c01ec41f674b5ef23d42`  
		Last Modified: Wed, 01 Nov 2023 01:06:49 GMT  
		Size: 1.1 KB (1109 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b61c058003459de4911c2901b2d799b03de754a1b9e64ffbe21a04992e962e62`  
		Last Modified: Wed, 01 Nov 2023 01:06:49 GMT  
		Size: 2.5 MB (2492501 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:810b6db64df2fcc8f76941cdac75093cf35bd72ac3cd1fa5eb664e74c1f67cd8`  
		Last Modified: Wed, 01 Nov 2023 01:06:50 GMT  
		Size: 6.6 MB (6636937 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:dbb899942df4149bd5fae8bac6e295285ec80f82d621f2b29c931ee348491cfb`  
		Last Modified: Wed, 01 Nov 2023 01:06:49 GMT  
		Size: 282.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4a8530160ab232c37c0ddcbf5e3a731d835d378d1382843957f6c2a73b2b5be6`  
		Last Modified: Wed, 01 Nov 2023 01:06:50 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:latest` - unknown; unknown

```console
$ docker pull memcached@sha256:dd7ce9519c31365127142232df2ed0b285e9acc03cd77c23c838bf932165def8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.5 KB (21498 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eef82c92e07c11a92c337806d01cfb1c6cdc7a16608dcf304a38de34d2ef1dbb`

```dockerfile
```

-	Layers:
	-	`sha256:c0d9dd22513f8d3e791e1796d7ef1906e57c798c92dd35d0be9cf2eaecec5954`  
		Last Modified: Wed, 01 Nov 2023 01:06:49 GMT  
		Size: 21.5 KB (21498 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:latest` - linux; mips64le

```console
$ docker pull memcached@sha256:9f7696d5078cf83e8b152cb00a3615576fd3c50d10be9253b9c188e16bfd8087
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.9 MB (39863164 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:685886644cfb343923260c15c66eb8c8d8bf7b84b6b1e855732aec2359b6ae29`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 21 Nov 2023 04:09:50 GMT
ADD file:e093749192323dc72b60a8440ddba26c415586f618b5e107fa264ba5eb2ca7ba in / 
# Tue, 21 Nov 2023 04:09:54 GMT
CMD ["bash"]
# Mon, 04 Dec 2023 18:08:47 GMT
RUN set -eux; 	groupadd --system --gid 11211 memcache; 	useradd --system --gid memcache --uid 11211 memcache # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
ENV MEMCACHED_VERSION=1.6.22
# Mon, 04 Dec 2023 18:08:47 GMT
ENV MEMCACHED_URL=https://memcached.org/files/memcached-1.6.22.tar.gz
# Mon, 04 Dec 2023 18:08:47 GMT
ENV MEMCACHED_SHA1=7a691f390d59616dbebfc9e2e4942d499c39a338
# Mon, 04 Dec 2023 18:08:47 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O memcached.tar.gz "$MEMCACHED_URL"; 	echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c -; 	mkdir -p /usr/src/memcached; 	tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1; 	rm memcached.tar.gz; 		cd /usr/src/memcached; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	; 	nproc="$(nproc)"; 	make -j "$nproc"; 		sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf; 	make test PARALLEL="$nproc"; 	mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf; 		make install; 		cd /; 	rm -rf /usr/src/memcached; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		memcached -V # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 04 Dec 2023 18:08:47 GMT
USER memcache
# Mon, 04 Dec 2023 18:08:47 GMT
EXPOSE map[11211/tcp:{}]
# Mon, 04 Dec 2023 18:08:47 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:ebdff2138fee4a3ec27560ab1353dc51c12c2608ff721f5db3d24104872b702a`  
		Last Modified: Tue, 21 Nov 2023 04:20:35 GMT  
		Size: 29.1 MB (29141984 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ee63ae82c6a87dc28cedafb91fbd6eaccd22add5b00a9cceb208472b30427b5d`  
		Last Modified: Tue, 12 Dec 2023 23:10:03 GMT  
		Size: 1.1 KB (1114 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3d430991f88102b07bcf8bf22f07667e49c9dfedb134b0ac36ddbb99d1e79db2`  
		Last Modified: Tue, 12 Dec 2023 23:10:04 GMT  
		Size: 1.9 MB (1937475 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ebe1140b392e915b8757b8d0a4b83f0aaf2103734e9f83c318821f641207b6b4`  
		Last Modified: Tue, 12 Dec 2023 23:10:04 GMT  
		Size: 8.8 MB (8782185 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:aedf1130e49a6aa7d9b74b9fd00914b171966fcf8beba71095787811fa3a0284`  
		Last Modified: Tue, 12 Dec 2023 23:10:03 GMT  
		Size: 284.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:457e2691e0499a1a1d26e6da85567f20a8dc396bde9d9952ce75fdcfe6cbafd8`  
		Last Modified: Tue, 12 Dec 2023 23:10:05 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:latest` - unknown; unknown

```console
$ docker pull memcached@sha256:d48752667ff111ef73342ae5c16218a373275e8b65c7696eff231ff49ca7b8e5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.0 KB (21004 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9138b1207d88c6ca6b32a2616d3c25b1f5d3280b7650ac4bfa7120518f6a8ad7`

```dockerfile
```

-	Layers:
	-	`sha256:2b1c5f3190ac8dfdff54a51d9421ad623af991deba1a46ba943cf88442079207`  
		Last Modified: Tue, 12 Dec 2023 23:10:03 GMT  
		Size: 21.0 KB (21004 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:latest` - linux; ppc64le

```console
$ docker pull memcached@sha256:813f2ed7d8d4d2c4e6f4a19816964b0c95cc56d038d95d059571d51e115ab109
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.5 MB (45508655 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:73c79988c4d09a9ac9cb01aa05096b344821e8034c3cba04afb9cb78fe25db05`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 21 Nov 2023 04:24:14 GMT
ADD file:8b22a531b6611a1e63dfc20e4e2931592e2d821bd4b64c4b2810bb9a36640c02 in / 
# Tue, 21 Nov 2023 04:24:16 GMT
CMD ["bash"]
# Mon, 04 Dec 2023 18:08:47 GMT
RUN set -eux; 	groupadd --system --gid 11211 memcache; 	useradd --system --gid memcache --uid 11211 memcache # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
ENV MEMCACHED_VERSION=1.6.22
# Mon, 04 Dec 2023 18:08:47 GMT
ENV MEMCACHED_URL=https://memcached.org/files/memcached-1.6.22.tar.gz
# Mon, 04 Dec 2023 18:08:47 GMT
ENV MEMCACHED_SHA1=7a691f390d59616dbebfc9e2e4942d499c39a338
# Mon, 04 Dec 2023 18:08:47 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O memcached.tar.gz "$MEMCACHED_URL"; 	echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c -; 	mkdir -p /usr/src/memcached; 	tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1; 	rm memcached.tar.gz; 		cd /usr/src/memcached; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	; 	nproc="$(nproc)"; 	make -j "$nproc"; 		sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf; 	make test PARALLEL="$nproc"; 	mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf; 		make install; 		cd /; 	rm -rf /usr/src/memcached; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		memcached -V # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 04 Dec 2023 18:08:47 GMT
USER memcache
# Mon, 04 Dec 2023 18:08:47 GMT
EXPOSE map[11211/tcp:{}]
# Mon, 04 Dec 2023 18:08:47 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:c570d04e61d8e35a3c8f12179d048d701451f97f9cf2099ea3e3738512dbf062`  
		Last Modified: Tue, 21 Nov 2023 04:28:58 GMT  
		Size: 33.1 MB (33141607 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b53469d03d0156e89526c2b744f6850b65cfb9b509a6fda4c523764f7a9f9072`  
		Last Modified: Tue, 12 Dec 2023 23:08:09 GMT  
		Size: 1.1 KB (1111 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:12b61a5974195d80345022ed47cb4546f6fec60527b3932b2ce74d605db750e0`  
		Last Modified: Tue, 12 Dec 2023 23:08:09 GMT  
		Size: 2.7 MB (2698202 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:108f5df7a0010e4f69929c6ce4ff2e0e53877c6bbe11bd86acbbb0e7b608dca7`  
		Last Modified: Tue, 12 Dec 2023 23:08:09 GMT  
		Size: 9.7 MB (9667330 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:aa53d1e0a6b1123a31838e581de8d738ccaf05c9be569ec50b8d37cbc54a99bd`  
		Last Modified: Tue, 12 Dec 2023 23:08:08 GMT  
		Size: 283.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2cf8ef0b438a2029bfc9b928364eb71966baa4990e2ac4a9b1648cbd44271dc4`  
		Last Modified: Tue, 12 Dec 2023 23:08:10 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:latest` - unknown; unknown

```console
$ docker pull memcached@sha256:d75efc7b8726fbfade0b41c14205058def09ee997a7befb495808c2752a56a54
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 MB (3066416 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ca8bb0be2316bb58a60c953382dd1963eb7e265d0602de370e02152e1ac84d7`

```dockerfile
```

-	Layers:
	-	`sha256:34203b346608565cdbcd7cf9a56efb8ec2255b1a8f30267d6b2749d6a0bd2d6b`  
		Last Modified: Tue, 12 Dec 2023 23:08:09 GMT  
		Size: 3.0 MB (3045398 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:4da4f2a55f1773bfac75983e2e733c609b970884e935de987ec5b3ec5c92eb85`  
		Last Modified: Tue, 12 Dec 2023 23:08:08 GMT  
		Size: 21.0 KB (21018 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:latest` - linux; s390x

```console
$ docker pull memcached@sha256:05084fffc798db32442e2cde93eac5815ffd909e9bf65692ac08c9b5ab79e677
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.0 MB (38041790 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eac80baab625f3daf940cdb3053e2e709bd61d78d7eae50b7db4d71f87bcd149`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 21 Nov 2023 05:04:35 GMT
ADD file:c33fa9fdde73983850798b6eb1cd062e0398109d1d773e6a937fead7475c8efc in / 
# Tue, 21 Nov 2023 05:04:41 GMT
CMD ["bash"]
# Mon, 04 Dec 2023 18:08:47 GMT
RUN set -eux; 	groupadd --system --gid 11211 memcache; 	useradd --system --gid memcache --uid 11211 memcache # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
ENV MEMCACHED_VERSION=1.6.22
# Mon, 04 Dec 2023 18:08:47 GMT
ENV MEMCACHED_URL=https://memcached.org/files/memcached-1.6.22.tar.gz
# Mon, 04 Dec 2023 18:08:47 GMT
ENV MEMCACHED_SHA1=7a691f390d59616dbebfc9e2e4942d499c39a338
# Mon, 04 Dec 2023 18:08:47 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O memcached.tar.gz "$MEMCACHED_URL"; 	echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c -; 	mkdir -p /usr/src/memcached; 	tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1; 	rm memcached.tar.gz; 		cd /usr/src/memcached; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	; 	nproc="$(nproc)"; 	make -j "$nproc"; 		sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf; 	make test PARALLEL="$nproc"; 	mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf; 		make install; 		cd /; 	rm -rf /usr/src/memcached; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		memcached -V # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 04 Dec 2023 18:08:47 GMT
USER memcache
# Mon, 04 Dec 2023 18:08:47 GMT
EXPOSE map[11211/tcp:{}]
# Mon, 04 Dec 2023 18:08:47 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:6daa625e5a040476e253e7acd0befa74254a4865ec836d6334a544d82a21d4be`  
		Last Modified: Tue, 21 Nov 2023 05:10:21 GMT  
		Size: 27.5 MB (27512885 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b19a3143cbec7ddc9a646dbbe779b0b5ec67662cf70e280db146f6ace54ccd61`  
		Last Modified: Wed, 13 Dec 2023 00:26:35 GMT  
		Size: 1.1 KB (1111 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b8af028b1fa76aa55f540dd5be5eaf89eea3fec23e09e9a88550aac36e9ee843`  
		Last Modified: Wed, 13 Dec 2023 00:26:35 GMT  
		Size: 2.2 MB (2152508 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9a774943469875a0902c53fccdd95cad9c18234b759bcdcc5816bd563deb7f14`  
		Last Modified: Wed, 13 Dec 2023 00:26:35 GMT  
		Size: 8.4 MB (8374880 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:266b4bf499a815da6f7ddcf68e1e61f8418c8ec655a2083e174aaa385de74d76`  
		Last Modified: Wed, 13 Dec 2023 00:26:35 GMT  
		Size: 284.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0da709e3482cc552b0a7b69eb05aaa21af1e74baaf4e3bccc34e95e478943630`  
		Last Modified: Wed, 13 Dec 2023 00:26:36 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:latest` - unknown; unknown

```console
$ docker pull memcached@sha256:525abad348ba03c5b9444f23409d647581284c1642d30539e2c9943405266f12
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 MB (3067303 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e3b551ec9122d039520bbd13bced5b1f5b0d5b1fd9e32c09a1d4536f7af1226`

```dockerfile
```

-	Layers:
	-	`sha256:5cc0958f61715f0746d9fa2a8a5c06f31608bb5d1cf32d606c46fc8e11b35984`  
		Last Modified: Wed, 13 Dec 2023 00:26:35 GMT  
		Size: 3.0 MB (3046353 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:3d2fed99d3355e42a820c1975105411eb7584cffb111d7e1fd541603f7721f1c`  
		Last Modified: Wed, 13 Dec 2023 00:26:35 GMT  
		Size: 20.9 KB (20950 bytes)  
		MIME: application/vnd.in-toto+json
