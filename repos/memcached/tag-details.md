<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `memcached`

-	[`memcached:1`](#memcached1)
-	[`memcached:1-alpine`](#memcached1-alpine)
-	[`memcached:1-alpine3.16`](#memcached1-alpine316)
-	[`memcached:1-bullseye`](#memcached1-bullseye)
-	[`memcached:1.6`](#memcached16)
-	[`memcached:1.6-alpine`](#memcached16-alpine)
-	[`memcached:1.6-alpine3.16`](#memcached16-alpine316)
-	[`memcached:1.6-bullseye`](#memcached16-bullseye)
-	[`memcached:1.6.15`](#memcached1615)
-	[`memcached:1.6.15-alpine`](#memcached1615-alpine)
-	[`memcached:1.6.15-alpine3.16`](#memcached1615-alpine316)
-	[`memcached:1.6.15-bullseye`](#memcached1615-bullseye)
-	[`memcached:alpine`](#memcachedalpine)
-	[`memcached:alpine3.16`](#memcachedalpine316)
-	[`memcached:bullseye`](#memcachedbullseye)
-	[`memcached:latest`](#memcachedlatest)

## `memcached:1`

```console
$ docker pull memcached@sha256:b422bca20902101cd4a427ccda5ea9729a89bdc6cd8ab8a7d8cd09b1470af6b6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; s390x

### `memcached:1` - linux; amd64

```console
$ docker pull memcached@sha256:1be4a685ac5a327ffbd7d1c7240378e7156824f9406b1eeb5fe19eadc2e61c53
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.0 MB (32968544 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a23fd759590b790a7cae87582ba4d747378de71b47e581b9295c02ce34eb9ed0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 23 Jun 2022 00:20:27 GMT
ADD file:8adbbab04d6f84cd83b5f4205b89b0acb7ecbf27a1bb2dc181d0a629479039fe in / 
# Thu, 23 Jun 2022 00:20:27 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 04:18:20 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Thu, 23 Jun 2022 04:18:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 04:18:24 GMT
ENV MEMCACHED_VERSION=1.6.15
# Thu, 23 Jun 2022 04:18:24 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Thu, 23 Jun 2022 04:21:07 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 23 Jun 2022 04:21:07 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 23 Jun 2022 04:21:08 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 23 Jun 2022 04:21:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jun 2022 04:21:08 GMT
USER memcache
# Thu, 23 Jun 2022 04:21:08 GMT
EXPOSE 11211
# Thu, 23 Jun 2022 04:21:08 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:b85a868b505ffd0342a37e6a3b1c49f7c71878afe569a807e6238ef08252fcb7`  
		Last Modified: Thu, 23 Jun 2022 00:25:18 GMT  
		Size: 31.4 MB (31379408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f58bb523c8de07d0d72658b2e622e82f065a1adef45f6f90f11eb7c71b9d0c61`  
		Last Modified: Thu, 23 Jun 2022 04:21:33 GMT  
		Size: 5.0 KB (4979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a458d61c2cd35b8afffe3741b04321a87f86ba216e5e2a4f9429b83b32ceb35`  
		Last Modified: Thu, 23 Jun 2022 04:21:33 GMT  
		Size: 328.1 KB (328115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7eda168e1238eaa8f5c20b7240bb8bc84c9a3f7b4b8cdc0be18f58f27bff1692`  
		Last Modified: Thu, 23 Jun 2022 04:21:33 GMT  
		Size: 1.3 MB (1255633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f188c32090c0c66f2f209fedc0778269d3edf2ad9db239ac0d2e1e3b64b36fd4`  
		Last Modified: Thu, 23 Jun 2022 04:21:33 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f492776609f9ffcbe6d066f45223bc2da677c44beb7bb0cdc6dfa34271885b34`  
		Last Modified: Thu, 23 Jun 2022 04:21:33 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1` - linux; arm variant v5

```console
$ docker pull memcached@sha256:54ff97ee8133b4181bff0e30de243b68ffa4ad0a7ecc458e6648a24760c63213
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.5 MB (30470395 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:07faffc84c650af3ec2eb3326c593cd933cba137c34c87589a375371eee849f3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 23 Jun 2022 00:50:38 GMT
ADD file:839c0e211e2260f5d54f2633e53c817c1f59e2394ba4b12f60e01e46cee61011 in / 
# Thu, 23 Jun 2022 00:50:39 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 02:41:47 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Thu, 23 Jun 2022 02:41:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 02:41:58 GMT
ENV MEMCACHED_VERSION=1.6.15
# Thu, 23 Jun 2022 02:41:59 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Thu, 23 Jun 2022 02:46:28 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 23 Jun 2022 02:46:29 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 23 Jun 2022 02:46:31 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 23 Jun 2022 02:46:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jun 2022 02:46:32 GMT
USER memcache
# Thu, 23 Jun 2022 02:46:32 GMT
EXPOSE 11211
# Thu, 23 Jun 2022 02:46:33 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:bd2d3b4056bd1b0310082fc5d17c6d03348601456c4b9306d1a333f1cec561f9`  
		Last Modified: Thu, 23 Jun 2022 01:05:39 GMT  
		Size: 28.9 MB (28921550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f500bb51d193d56af19fbeb8ebc1919ec2e6d04cf9a7d1637ad79cc00397c1b`  
		Last Modified: Thu, 23 Jun 2022 02:47:27 GMT  
		Size: 4.9 KB (4894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c3dc6e5372afc0620e0eeae739b429bee70842f20a15ca8345787a674d5d3b8`  
		Last Modified: Thu, 23 Jun 2022 02:47:28 GMT  
		Size: 316.6 KB (316616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83d6f2e7e5c2a1d3566c4d9cd05fd132529535ba7eaecb00d312c0d0a6055a4c`  
		Last Modified: Thu, 23 Jun 2022 02:47:28 GMT  
		Size: 1.2 MB (1226926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:109349836a4d5f4431660fec9744df70f92475b22644182ae9d77c8c56c8960a`  
		Last Modified: Thu, 23 Jun 2022 02:47:27 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b87ddf1818c82326658f3ca6d444b01978e23d30a7232e4ef1e0f6f0ba4ab18`  
		Last Modified: Thu, 23 Jun 2022 02:47:27 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1` - linux; arm variant v7

```console
$ docker pull memcached@sha256:b3ddbe1e7ec04512ac9e20555b72ba4b2e7e9ee99138535fabe5e92cc92302b5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.1 MB (28092007 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cbbff85100ff53c710f4caa30445e0ee79ccd0fe61cc91a522821fc5415e6bcf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 23 Jun 2022 00:59:45 GMT
ADD file:925abfb9fc0e4a7cc0c979b12c9bd2607f5c493d37b05535ca010f81beb060a9 in / 
# Thu, 23 Jun 2022 00:59:46 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 22:08:47 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Thu, 23 Jun 2022 22:08:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 22:08:56 GMT
ENV MEMCACHED_VERSION=1.6.15
# Thu, 23 Jun 2022 22:08:56 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Thu, 23 Jun 2022 22:13:04 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 23 Jun 2022 22:13:05 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 23 Jun 2022 22:13:06 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 23 Jun 2022 22:13:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jun 2022 22:13:07 GMT
USER memcache
# Thu, 23 Jun 2022 22:13:08 GMT
EXPOSE 11211
# Thu, 23 Jun 2022 22:13:08 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:d2fd562560d8062a78064adfbfa204521167c301f00f5ab3c65b9c2a54083dba`  
		Last Modified: Thu, 23 Jun 2022 01:15:22 GMT  
		Size: 26.6 MB (26576105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8864d1bfbfd3f4b781316abd42de97a2967a6b20534ffdc4fea6a3de16c1d972`  
		Last Modified: Fri, 24 Jun 2022 01:14:10 GMT  
		Size: 4.9 KB (4897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fa7c6c177f3ba693baa86ed010daf821ca2addfe7f3b8a83c7f52fac209a6e8`  
		Last Modified: Fri, 24 Jun 2022 01:14:10 GMT  
		Size: 312.1 KB (312076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f802ee5fb123a2824f3e6f93144c74f9e1c88159fc819b46f7ed2913ec61281a`  
		Last Modified: Fri, 24 Jun 2022 01:14:11 GMT  
		Size: 1.2 MB (1198521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25b61f87cd4332b040dd59bae91f0701228904433b1955bb4f51b7377db17b00`  
		Last Modified: Fri, 24 Jun 2022 01:14:10 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:532462b4f12685e2093583f1e86c82d5c2c8069b92ccbc9bbcf8efad7dfd3252`  
		Last Modified: Fri, 24 Jun 2022 01:14:10 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:536f8192668e851874eec7d483055b0af220a7eb0be43010f2f9825e99ab0111
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.4 MB (31444932 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2ce58160065ec196d51dcdc756610352a57f6192b28345989be83b94b8300dec`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 23 Jun 2022 00:40:43 GMT
ADD file:134be48af13f80f3474bf1b080ca781feb7b972148d482849862e55eb2acd61c in / 
# Thu, 23 Jun 2022 00:40:44 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 03:53:19 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Thu, 23 Jun 2022 03:53:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 03:53:24 GMT
ENV MEMCACHED_VERSION=1.6.15
# Thu, 23 Jun 2022 03:53:25 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Thu, 23 Jun 2022 03:56:00 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 23 Jun 2022 03:56:02 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 23 Jun 2022 03:56:02 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 23 Jun 2022 03:56:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jun 2022 03:56:04 GMT
USER memcache
# Thu, 23 Jun 2022 03:56:05 GMT
EXPOSE 11211
# Thu, 23 Jun 2022 03:56:06 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:3b157c852f2736e12f09046f214fe5f6a0b1652bd860269b3988c92a197026e8`  
		Last Modified: Thu, 23 Jun 2022 00:47:22 GMT  
		Size: 30.1 MB (30065720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee776bb67ffbc00ca5100c88e1f7ae63b580bc131c046c3c7138b7fb796683a2`  
		Last Modified: Thu, 23 Jun 2022 03:56:51 GMT  
		Size: 4.9 KB (4904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85b234170a3d54e3ad2be2993a7e7b09550a4e00327804a183e07bc786d01bc8`  
		Last Modified: Thu, 23 Jun 2022 03:56:51 GMT  
		Size: 119.2 KB (119223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a61e7150a45b8305adc14ed47f7beb3e807a7f08223393e6f5382b043b120941`  
		Last Modified: Thu, 23 Jun 2022 03:56:51 GMT  
		Size: 1.3 MB (1254677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ed6ad1685f73da9293938d389b8c24ee8b8af4d04d4c8b502cb6082d58bf349`  
		Last Modified: Thu, 23 Jun 2022 03:56:51 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:276672cde8876c99c646defdc630e9be5ae5cfb33c192102b6387ce99d151179`  
		Last Modified: Thu, 23 Jun 2022 03:56:51 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1` - linux; 386

```console
$ docker pull memcached@sha256:651e5275f0623232ecfa476f864b6634de4e9ffc6671376c796ffd70e31c83b6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.8 MB (33778463 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31252c746c529da361fcb075711def9645866db716700e15d9e4ce92e96ed3a0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 23 Jun 2022 00:39:33 GMT
ADD file:9d46d3f8fb63833a6dbd8dd796ad541d556046a48342d22e1fd3bffa3fb8e504 in / 
# Thu, 23 Jun 2022 00:39:33 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 03:32:31 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Thu, 23 Jun 2022 03:32:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 03:32:36 GMT
ENV MEMCACHED_VERSION=1.6.15
# Thu, 23 Jun 2022 03:32:37 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Thu, 23 Jun 2022 03:35:28 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 23 Jun 2022 03:35:30 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 23 Jun 2022 03:35:30 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 23 Jun 2022 03:35:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jun 2022 03:35:32 GMT
USER memcache
# Thu, 23 Jun 2022 03:35:33 GMT
EXPOSE 11211
# Thu, 23 Jun 2022 03:35:34 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:4870b12e407743816673c11cfb39974d80c1569d876287bef61f8c585954822f`  
		Last Modified: Thu, 23 Jun 2022 00:46:40 GMT  
		Size: 32.4 MB (32390198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a67b6581e800ff3e02f41dd18cb78bc620a25becd83769f84d2c61aed5d01ea`  
		Last Modified: Thu, 23 Jun 2022 03:36:21 GMT  
		Size: 4.8 KB (4773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b70025d0ac3fc2b23b2e76f6d96c607c6a04b53c9850fe3f14fa855827b9d19d`  
		Last Modified: Thu, 23 Jun 2022 03:36:21 GMT  
		Size: 130.1 KB (130137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a383a40e44984d67c847d2a4bbc7d3525f3867ff39c81a5221970dc744ee822e`  
		Last Modified: Thu, 23 Jun 2022 03:36:21 GMT  
		Size: 1.3 MB (1252947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24f731218f56e8a5f3d250c9a4e15f841afbd92a0ee71f88761feb880aa937b3`  
		Last Modified: Thu, 23 Jun 2022 03:36:21 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15ab75a8041fc16fdde22888eb35315059264f2c153e8d05d7f132d1aa413e3a`  
		Last Modified: Thu, 23 Jun 2022 03:36:21 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1` - linux; mips64le

```console
$ docker pull memcached@sha256:71ebcf40d19139f8bab5733065ff1b2599e5d52359c6f6cbfad2104be2f1fe33
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.0 MB (31014756 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d95105805101f850723625215940d8b2be96a9b40f984174eee903985becb9e0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 23 Jun 2022 01:10:25 GMT
ADD file:fd1174cc47ac636f0cab382578a899d69ed489e4dee53ec838955e36066f526a in / 
# Thu, 23 Jun 2022 01:10:29 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 03:13:46 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Thu, 23 Jun 2022 03:14:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 03:14:06 GMT
ENV MEMCACHED_VERSION=1.6.15
# Thu, 23 Jun 2022 03:14:08 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Thu, 23 Jun 2022 03:21:07 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 23 Jun 2022 03:21:09 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 23 Jun 2022 03:21:15 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 23 Jun 2022 03:21:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jun 2022 03:21:20 GMT
USER memcache
# Thu, 23 Jun 2022 03:21:22 GMT
EXPOSE 11211
# Thu, 23 Jun 2022 03:21:25 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:9d199cb5e183b38c9edcc527cbaaa79bb56da73bd09ed449223842775ef4a244`  
		Last Modified: Thu, 23 Jun 2022 01:20:19 GMT  
		Size: 29.6 MB (29641027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d188c3e3bf643b15e2e70cc10dab71da1f4e871305c84cf6d927a2750209ee47`  
		Last Modified: Thu, 23 Jun 2022 03:21:53 GMT  
		Size: 4.9 KB (4863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8855d5fcd2d728913f5ae40b13f074576721a44abf081e6bd4e8f48e8deb8262`  
		Last Modified: Thu, 23 Jun 2022 03:21:54 GMT  
		Size: 117.2 KB (117169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:726be3b42973c4aa79e2ffcecb3633c1ec825f8099da6b5d952810bf4d1827cd`  
		Last Modified: Thu, 23 Jun 2022 03:21:54 GMT  
		Size: 1.3 MB (1251289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6176796787c17dc9b41c47c10e23979540bb32e2833c3eeceb1456f0b228166f`  
		Last Modified: Thu, 23 Jun 2022 03:21:54 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:926c03f02a771007ddd9b4fd2172ff2d89647400c4370fdedb4533a5c99e42b1`  
		Last Modified: Thu, 23 Jun 2022 03:21:53 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1` - linux; ppc64le

```console
$ docker pull memcached@sha256:0bfecd8ca43abc3e50d162ce07d6794beb5d9f98ce929e9371c2542065e6c785
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.0 MB (36972124 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ac53be686814de607770ae7fba96134fc9cd4e5afe7444779b08c02a0c92a6c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 23 Jun 2022 02:02:32 GMT
ADD file:e18c13649ea1f145047652c8e171c4824f9b6b0dbc92127a914c7fca910acf96 in / 
# Thu, 23 Jun 2022 02:02:34 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 08:15:12 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Thu, 23 Jun 2022 08:15:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 08:15:26 GMT
ENV MEMCACHED_VERSION=1.6.15
# Thu, 23 Jun 2022 08:15:30 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Thu, 23 Jun 2022 08:20:21 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 23 Jun 2022 08:20:23 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 23 Jun 2022 08:20:29 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 23 Jun 2022 08:20:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jun 2022 08:20:34 GMT
USER memcache
# Thu, 23 Jun 2022 08:20:36 GMT
EXPOSE 11211
# Thu, 23 Jun 2022 08:20:38 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:7716f0df7ba06b6f1937cd664805984e25e386a4165f2c6acc65356686e35221`  
		Last Modified: Thu, 23 Jun 2022 02:15:20 GMT  
		Size: 35.3 MB (35286823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54d7d03c3543d8cc9dbdea919601e8b8bdebdf5f54f23ee2a186edde48a4025c`  
		Last Modified: Thu, 23 Jun 2022 08:21:29 GMT  
		Size: 5.0 KB (4987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa5efdc63c420d0295d4932cc7467f1a9005b4724f592c4fba99b6c801f57810`  
		Last Modified: Thu, 23 Jun 2022 08:21:29 GMT  
		Size: 357.0 KB (356958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:329e40de463f01938ecac1d284adb38a29fde479486e279cb302d95abe9f4a16`  
		Last Modified: Thu, 23 Jun 2022 08:21:29 GMT  
		Size: 1.3 MB (1322949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d823793235eacc3363db343cea0db041905e9fde59ff5262e0fd8826e962f5a`  
		Last Modified: Thu, 23 Jun 2022 08:21:29 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2ae46dbc3324ea97ee7556a1bc8006b075f7a1492e3a2114aaf8dec7c579b76`  
		Last Modified: Thu, 23 Jun 2022 08:21:29 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1` - linux; s390x

```console
$ docker pull memcached@sha256:1e49c15efaf9999b31f526130902a04a53eeac416f40d1549e98b3fa1a872c04
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.2 MB (31226391 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b8090a3ed64f97313e1ddce878717e3bf8c1aace9d7bf247a1fa53418081f0c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 23 Jun 2022 00:43:10 GMT
ADD file:0b511e3efd87267fb27161eae56c4d08f0fed733697da6ffe6ea96a4cb68e938 in / 
# Thu, 23 Jun 2022 00:43:15 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 13:41:46 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Thu, 23 Jun 2022 13:41:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 13:41:49 GMT
ENV MEMCACHED_VERSION=1.6.15
# Thu, 23 Jun 2022 13:41:50 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Thu, 23 Jun 2022 13:45:09 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 23 Jun 2022 13:45:09 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 23 Jun 2022 13:45:10 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 23 Jun 2022 13:45:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jun 2022 13:45:10 GMT
USER memcache
# Thu, 23 Jun 2022 13:45:10 GMT
EXPOSE 11211
# Thu, 23 Jun 2022 13:45:10 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:c547f465e0c8708ad0c57cf09caa52f4c2b5b295bf10ab1ce71ca17ff81ea36a`  
		Last Modified: Thu, 23 Jun 2022 00:51:59 GMT  
		Size: 29.7 MB (29655262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04837776e7fbb579dda3720caca85ff9cb19eea15a8830ab0f23a160fa832205`  
		Last Modified: Thu, 23 Jun 2022 13:46:03 GMT  
		Size: 5.0 KB (5025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d844915fd9a66accf5106919c6a63121ed4fde412dcf958133bc1b1483b307b`  
		Last Modified: Thu, 23 Jun 2022 13:46:03 GMT  
		Size: 324.2 KB (324209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51abf5cd3f179d43b5845c7dc42a6f07ddfd6da706ca58f78d53641e3d62289f`  
		Last Modified: Thu, 23 Jun 2022 13:46:03 GMT  
		Size: 1.2 MB (1241485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31ea51fd993089ad7346961b0897d009e18b953416139bf4359ff089b9e9ada9`  
		Last Modified: Thu, 23 Jun 2022 13:46:04 GMT  
		Size: 289.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cda18e1b304fdde7d799586641bad45a035387c02b0c7e8d696e91221b046e28`  
		Last Modified: Thu, 23 Jun 2022 13:46:03 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:1-alpine`

```console
$ docker pull memcached@sha256:96af3fed9ef980101602ea90c3220679bb326bfe70474e4f06759f25db4591e2
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
$ docker pull memcached@sha256:bae66da0e8cdb7daa226cc0837e2562404a4007466044ffdfa88a8a0431d5c7a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3853361 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e3f5d6e8d61d2ec54ff3d21da1c6dbddca8f0018c8f1c1253287129fa3926d7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 23 May 2022 19:19:30 GMT
ADD file:8e81116368669ed3dd361bc898d61bff249f524139a239fdaf3ec46869a39921 in / 
# Mon, 23 May 2022 19:19:31 GMT
CMD ["/bin/sh"]
# Tue, 24 May 2022 19:24:21 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 24 May 2022 19:24:23 GMT
RUN apk add --no-cache libsasl
# Tue, 24 May 2022 19:24:23 GMT
ENV MEMCACHED_VERSION=1.6.15
# Tue, 24 May 2022 19:24:23 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Tue, 24 May 2022 19:27:18 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 24 May 2022 19:27:18 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 24 May 2022 19:27:19 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 24 May 2022 19:27:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 24 May 2022 19:27:19 GMT
USER memcache
# Tue, 24 May 2022 19:27:19 GMT
EXPOSE 11211
# Tue, 24 May 2022 19:27:19 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:2408cc74d12b6cd092bb8b516ba7d5e290f485d3eb9672efc00f0583730179e8`  
		Last Modified: Mon, 23 May 2022 19:09:38 GMT  
		Size: 2.8 MB (2798889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6da329a3b4330a0705bfb49b5e6ce2fb61bc108d0a32d41c2c0dad6d9dd6c8fa`  
		Last Modified: Tue, 24 May 2022 19:27:48 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f4ba002bd64c19ecd49e1afc372709c9bcfb3dbe2b9ee2b02d43dea8fddc3cc`  
		Last Modified: Tue, 24 May 2022 19:27:48 GMT  
		Size: 108.3 KB (108307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d664dde428a76ca57c1261382f6f9b758a3b5b0e12b51f6a5b1a38bef237456a`  
		Last Modified: Tue, 24 May 2022 19:27:48 GMT  
		Size: 944.5 KB (944489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef11efc606151d8228ae06848232d8d65ae50082bf0ad5c5104d06c27ce7c85d`  
		Last Modified: Tue, 24 May 2022 19:27:48 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f118f0edbe76d09a02e63a4712d1b9b3eb1ebce2a271c740baba58cc48df9f4e`  
		Last Modified: Tue, 24 May 2022 19:27:48 GMT  
		Size: 121.0 B  
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
$ docker pull memcached@sha256:8ec1f6a98e264e73e3c7b2feba04b272ce1522adc9d40118b9684721c41122b0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.7 MB (3737167 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f393a4888061e0456042ebb89fbc11cf72af15c189e0d0e4ee62b7fcfd44c683`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 23 May 2022 19:39:22 GMT
ADD file:3ae36c6c4a1fc43157692da97c6c4fa6c3d0189ba82e2bef7f5aaf4a5e083f18 in / 
# Mon, 23 May 2022 19:39:22 GMT
CMD ["/bin/sh"]
# Tue, 24 May 2022 20:08:53 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 24 May 2022 20:08:55 GMT
RUN apk add --no-cache libsasl
# Tue, 24 May 2022 20:08:56 GMT
ENV MEMCACHED_VERSION=1.6.15
# Tue, 24 May 2022 20:08:57 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Tue, 24 May 2022 20:12:06 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 24 May 2022 20:12:08 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 24 May 2022 20:12:08 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 24 May 2022 20:12:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 24 May 2022 20:12:10 GMT
USER memcache
# Tue, 24 May 2022 20:12:11 GMT
EXPOSE 11211
# Tue, 24 May 2022 20:12:12 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:b3c136eddcbf2003d3180787cef00f39d46b9fd9e4623178282ad6a8d63ad3b0`  
		Last Modified: Mon, 23 May 2022 19:08:34 GMT  
		Size: 2.7 MB (2694464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e87d2d7a8c9bc1317afe928c225caaafd86b3b73a2bc359f8037eb0f501b394c`  
		Last Modified: Tue, 24 May 2022 20:12:58 GMT  
		Size: 1.2 KB (1242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55dbcde2059d799697807a93b36d71cd601b20e2218abb7cb9261d22e8a7d67a`  
		Last Modified: Tue, 24 May 2022 20:12:58 GMT  
		Size: 109.6 KB (109557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4aa3db0ac20b8381c09df00576661af3c209195453eeeb892b8532059b932a39`  
		Last Modified: Tue, 24 May 2022 20:12:59 GMT  
		Size: 931.5 KB (931496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d999e908ec416e199da213e6fca67cdc82d3d440098a1bfbc5bc7c5a2f35636`  
		Last Modified: Tue, 24 May 2022 20:12:58 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8017baa48e45fa47c2fab6975dcd0ab8a560c64c0de05f7113831a537b385a3b`  
		Last Modified: Tue, 24 May 2022 20:12:58 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-alpine` - linux; 386

```console
$ docker pull memcached@sha256:3560af36f0aaeb7e4d2da47f0ad4a91bc675aa017423f34911490b09908230e8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3878370 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7d5a231eedb6e0b20291a77ac7a71c5a16aca1a9eb62893e285cefa1b95bdf5b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 23 May 2022 19:38:20 GMT
ADD file:1750ccfabfe93636015070d51a6e824cbd738056223421c69d8aaabc38041b18 in / 
# Mon, 23 May 2022 19:38:20 GMT
CMD ["/bin/sh"]
# Tue, 24 May 2022 19:46:24 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 24 May 2022 19:46:26 GMT
RUN apk add --no-cache libsasl
# Tue, 24 May 2022 19:46:26 GMT
ENV MEMCACHED_VERSION=1.6.15
# Tue, 24 May 2022 19:46:27 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Tue, 24 May 2022 19:49:17 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 24 May 2022 19:49:19 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 24 May 2022 19:49:19 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 24 May 2022 19:49:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 24 May 2022 19:49:21 GMT
USER memcache
# Tue, 24 May 2022 19:49:22 GMT
EXPOSE 11211
# Tue, 24 May 2022 19:49:23 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:bb638a3869eed698f88775c7a48f36f8e22e7c6bbaa98fa1d5678966b619b859`  
		Last Modified: Mon, 23 May 2022 19:09:25 GMT  
		Size: 2.8 MB (2801887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d301e0dbe5a2594f09f110ec3c1e79f4bd885af78b4992bf8af7a9f7b0507d5a`  
		Last Modified: Tue, 24 May 2022 19:50:14 GMT  
		Size: 1.2 KB (1242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:880ddc23b9c3165a8e86c64a648782c63c9a7271e84df6ac2f5a8c110d32258d`  
		Last Modified: Tue, 24 May 2022 19:50:14 GMT  
		Size: 119.8 KB (119821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c60884a7874466d1525bb0560fcbbbc226cfb4fb1507f1bd0d45d4f1b0e1307b`  
		Last Modified: Tue, 24 May 2022 19:50:15 GMT  
		Size: 955.0 KB (955017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89ad9c1959a10762028a884c1a33f06bb71bcb1a9ac372c889304f75f2a4b597`  
		Last Modified: Tue, 24 May 2022 19:50:14 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b267a8907abfcf28b9d96b17379ce57985989f17d34c06dfd238aee8ed0da61`  
		Last Modified: Tue, 24 May 2022 19:50:14 GMT  
		Size: 119.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-alpine` - linux; ppc64le

```console
$ docker pull memcached@sha256:edeccd4ca90cecc053bd78239bef1a1ccec0d2f189655d39e29e44216157fec4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3891798 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:348c555fa9d4bcfd44f2f7426151f1666fd08a28ce9fea73c503bc207229c503`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 23 May 2022 19:16:51 GMT
ADD file:6a5450c8a7cee3ceda59e7cb350c54df4139b0f7b7cf49c8b31bb9c01646c3cd in / 
# Mon, 23 May 2022 19:16:53 GMT
CMD ["/bin/sh"]
# Tue, 24 May 2022 19:29:15 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 24 May 2022 19:29:23 GMT
RUN apk add --no-cache libsasl
# Tue, 24 May 2022 19:29:30 GMT
ENV MEMCACHED_VERSION=1.6.15
# Tue, 24 May 2022 19:29:36 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Tue, 24 May 2022 19:33:02 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 24 May 2022 19:33:03 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 24 May 2022 19:33:08 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 24 May 2022 19:33:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 24 May 2022 19:33:14 GMT
USER memcache
# Tue, 24 May 2022 19:33:17 GMT
EXPOSE 11211
# Tue, 24 May 2022 19:33:19 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:d3deabf2a506ef6f5fa7c2a68bf27047574cef9908b30a97ff2d01ae539b089a`  
		Last Modified: Mon, 23 May 2022 19:09:13 GMT  
		Size: 2.8 MB (2789745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b479cfab13a2f2ffe6bfc643d96b2ca17a80380353869913b72735725a953596`  
		Last Modified: Tue, 24 May 2022 19:34:20 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9111d00ba5c4381f0f8b185e1703815ef94004e492b01b0d3c7a7fe53acc977`  
		Last Modified: Tue, 24 May 2022 19:34:21 GMT  
		Size: 126.0 KB (126043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1a992983a73a33de517b221e813f6ddddea412212564e886bba2a9a09f82735`  
		Last Modified: Tue, 24 May 2022 19:34:21 GMT  
		Size: 974.3 KB (974333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6de2f26a895426d80205ef485568a93b91456d9913ce062578d21db1d228ef7`  
		Last Modified: Tue, 24 May 2022 19:34:20 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27f443297da5126d218f0cfd07deeb374b4db49ce895657aed034e4eba40ce1c`  
		Last Modified: Tue, 24 May 2022 19:34:20 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-alpine` - linux; s390x

```console
$ docker pull memcached@sha256:79c15e8f5b25e585bc279ba8a2e990aaf1bcb0622e4b2cfe246b32381748232d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.6 MB (3629283 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3984c3293b24638ac012e61d1d83266b40194c43831d6d2f59fe1c01615baf07`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 23 May 2022 19:41:59 GMT
ADD file:e1852d8ef555a0d3ef6d0b74a898720c82bb9f491430b06a0dd0499497ce118e in / 
# Mon, 23 May 2022 19:42:10 GMT
CMD ["/bin/sh"]
# Tue, 24 May 2022 19:50:13 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 24 May 2022 19:50:14 GMT
RUN apk add --no-cache libsasl
# Tue, 24 May 2022 19:50:15 GMT
ENV MEMCACHED_VERSION=1.6.15
# Tue, 24 May 2022 19:50:15 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Tue, 24 May 2022 19:54:14 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 24 May 2022 19:54:15 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 24 May 2022 19:54:16 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 24 May 2022 19:54:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 24 May 2022 19:54:16 GMT
USER memcache
# Tue, 24 May 2022 19:54:16 GMT
EXPOSE 11211
# Tue, 24 May 2022 19:54:16 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:af1ac1a73384e058591d04d19bc05a06781cc32d52d4593b468d6cb95eda9858`  
		Last Modified: Mon, 23 May 2022 19:43:36 GMT  
		Size: 2.6 MB (2580494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0cdb25dad8a9e7c836addf0dfee4462f64217c81619f5c7519d620c59c68fff`  
		Last Modified: Tue, 24 May 2022 19:55:16 GMT  
		Size: 1.3 KB (1265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bfb96fb83213592db4a96cd8313433230d559f81caa115c56c8f9018d5e01f5`  
		Last Modified: Tue, 24 May 2022 19:55:16 GMT  
		Size: 112.5 KB (112500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fd8f0273e1af52c2d6bc2ea6e8f7c7b516ce039d78151fe854039d86e62db91`  
		Last Modified: Tue, 24 May 2022 19:55:17 GMT  
		Size: 934.6 KB (934620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a50bb84155cee8c93b5835daaee0a57b7c14397817ac75279b1ac51d2626f594`  
		Last Modified: Tue, 24 May 2022 19:55:16 GMT  
		Size: 283.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:196f82f950409b7b7c0e395502911ba3177047647ed8ac24e62c49dacf4eebf1`  
		Last Modified: Tue, 24 May 2022 19:55:17 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:1-alpine3.16`

```console
$ docker pull memcached@sha256:bab32a8a61543525190db12c2a518c3c2331656a4409185f0f4f33a506e3aae7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `memcached:1-alpine3.16` - linux; amd64

```console
$ docker pull memcached@sha256:bae66da0e8cdb7daa226cc0837e2562404a4007466044ffdfa88a8a0431d5c7a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3853361 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e3f5d6e8d61d2ec54ff3d21da1c6dbddca8f0018c8f1c1253287129fa3926d7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 23 May 2022 19:19:30 GMT
ADD file:8e81116368669ed3dd361bc898d61bff249f524139a239fdaf3ec46869a39921 in / 
# Mon, 23 May 2022 19:19:31 GMT
CMD ["/bin/sh"]
# Tue, 24 May 2022 19:24:21 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 24 May 2022 19:24:23 GMT
RUN apk add --no-cache libsasl
# Tue, 24 May 2022 19:24:23 GMT
ENV MEMCACHED_VERSION=1.6.15
# Tue, 24 May 2022 19:24:23 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Tue, 24 May 2022 19:27:18 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 24 May 2022 19:27:18 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 24 May 2022 19:27:19 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 24 May 2022 19:27:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 24 May 2022 19:27:19 GMT
USER memcache
# Tue, 24 May 2022 19:27:19 GMT
EXPOSE 11211
# Tue, 24 May 2022 19:27:19 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:2408cc74d12b6cd092bb8b516ba7d5e290f485d3eb9672efc00f0583730179e8`  
		Last Modified: Mon, 23 May 2022 19:09:38 GMT  
		Size: 2.8 MB (2798889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6da329a3b4330a0705bfb49b5e6ce2fb61bc108d0a32d41c2c0dad6d9dd6c8fa`  
		Last Modified: Tue, 24 May 2022 19:27:48 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f4ba002bd64c19ecd49e1afc372709c9bcfb3dbe2b9ee2b02d43dea8fddc3cc`  
		Last Modified: Tue, 24 May 2022 19:27:48 GMT  
		Size: 108.3 KB (108307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d664dde428a76ca57c1261382f6f9b758a3b5b0e12b51f6a5b1a38bef237456a`  
		Last Modified: Tue, 24 May 2022 19:27:48 GMT  
		Size: 944.5 KB (944489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef11efc606151d8228ae06848232d8d65ae50082bf0ad5c5104d06c27ce7c85d`  
		Last Modified: Tue, 24 May 2022 19:27:48 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f118f0edbe76d09a02e63a4712d1b9b3eb1ebce2a271c740baba58cc48df9f4e`  
		Last Modified: Tue, 24 May 2022 19:27:48 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-alpine3.16` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:8ec1f6a98e264e73e3c7b2feba04b272ce1522adc9d40118b9684721c41122b0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.7 MB (3737167 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f393a4888061e0456042ebb89fbc11cf72af15c189e0d0e4ee62b7fcfd44c683`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 23 May 2022 19:39:22 GMT
ADD file:3ae36c6c4a1fc43157692da97c6c4fa6c3d0189ba82e2bef7f5aaf4a5e083f18 in / 
# Mon, 23 May 2022 19:39:22 GMT
CMD ["/bin/sh"]
# Tue, 24 May 2022 20:08:53 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 24 May 2022 20:08:55 GMT
RUN apk add --no-cache libsasl
# Tue, 24 May 2022 20:08:56 GMT
ENV MEMCACHED_VERSION=1.6.15
# Tue, 24 May 2022 20:08:57 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Tue, 24 May 2022 20:12:06 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 24 May 2022 20:12:08 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 24 May 2022 20:12:08 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 24 May 2022 20:12:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 24 May 2022 20:12:10 GMT
USER memcache
# Tue, 24 May 2022 20:12:11 GMT
EXPOSE 11211
# Tue, 24 May 2022 20:12:12 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:b3c136eddcbf2003d3180787cef00f39d46b9fd9e4623178282ad6a8d63ad3b0`  
		Last Modified: Mon, 23 May 2022 19:08:34 GMT  
		Size: 2.7 MB (2694464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e87d2d7a8c9bc1317afe928c225caaafd86b3b73a2bc359f8037eb0f501b394c`  
		Last Modified: Tue, 24 May 2022 20:12:58 GMT  
		Size: 1.2 KB (1242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55dbcde2059d799697807a93b36d71cd601b20e2218abb7cb9261d22e8a7d67a`  
		Last Modified: Tue, 24 May 2022 20:12:58 GMT  
		Size: 109.6 KB (109557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4aa3db0ac20b8381c09df00576661af3c209195453eeeb892b8532059b932a39`  
		Last Modified: Tue, 24 May 2022 20:12:59 GMT  
		Size: 931.5 KB (931496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d999e908ec416e199da213e6fca67cdc82d3d440098a1bfbc5bc7c5a2f35636`  
		Last Modified: Tue, 24 May 2022 20:12:58 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8017baa48e45fa47c2fab6975dcd0ab8a560c64c0de05f7113831a537b385a3b`  
		Last Modified: Tue, 24 May 2022 20:12:58 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-alpine3.16` - linux; 386

```console
$ docker pull memcached@sha256:3560af36f0aaeb7e4d2da47f0ad4a91bc675aa017423f34911490b09908230e8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3878370 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7d5a231eedb6e0b20291a77ac7a71c5a16aca1a9eb62893e285cefa1b95bdf5b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 23 May 2022 19:38:20 GMT
ADD file:1750ccfabfe93636015070d51a6e824cbd738056223421c69d8aaabc38041b18 in / 
# Mon, 23 May 2022 19:38:20 GMT
CMD ["/bin/sh"]
# Tue, 24 May 2022 19:46:24 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 24 May 2022 19:46:26 GMT
RUN apk add --no-cache libsasl
# Tue, 24 May 2022 19:46:26 GMT
ENV MEMCACHED_VERSION=1.6.15
# Tue, 24 May 2022 19:46:27 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Tue, 24 May 2022 19:49:17 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 24 May 2022 19:49:19 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 24 May 2022 19:49:19 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 24 May 2022 19:49:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 24 May 2022 19:49:21 GMT
USER memcache
# Tue, 24 May 2022 19:49:22 GMT
EXPOSE 11211
# Tue, 24 May 2022 19:49:23 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:bb638a3869eed698f88775c7a48f36f8e22e7c6bbaa98fa1d5678966b619b859`  
		Last Modified: Mon, 23 May 2022 19:09:25 GMT  
		Size: 2.8 MB (2801887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d301e0dbe5a2594f09f110ec3c1e79f4bd885af78b4992bf8af7a9f7b0507d5a`  
		Last Modified: Tue, 24 May 2022 19:50:14 GMT  
		Size: 1.2 KB (1242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:880ddc23b9c3165a8e86c64a648782c63c9a7271e84df6ac2f5a8c110d32258d`  
		Last Modified: Tue, 24 May 2022 19:50:14 GMT  
		Size: 119.8 KB (119821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c60884a7874466d1525bb0560fcbbbc226cfb4fb1507f1bd0d45d4f1b0e1307b`  
		Last Modified: Tue, 24 May 2022 19:50:15 GMT  
		Size: 955.0 KB (955017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89ad9c1959a10762028a884c1a33f06bb71bcb1a9ac372c889304f75f2a4b597`  
		Last Modified: Tue, 24 May 2022 19:50:14 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b267a8907abfcf28b9d96b17379ce57985989f17d34c06dfd238aee8ed0da61`  
		Last Modified: Tue, 24 May 2022 19:50:14 GMT  
		Size: 119.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-alpine3.16` - linux; ppc64le

```console
$ docker pull memcached@sha256:edeccd4ca90cecc053bd78239bef1a1ccec0d2f189655d39e29e44216157fec4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3891798 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:348c555fa9d4bcfd44f2f7426151f1666fd08a28ce9fea73c503bc207229c503`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 23 May 2022 19:16:51 GMT
ADD file:6a5450c8a7cee3ceda59e7cb350c54df4139b0f7b7cf49c8b31bb9c01646c3cd in / 
# Mon, 23 May 2022 19:16:53 GMT
CMD ["/bin/sh"]
# Tue, 24 May 2022 19:29:15 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 24 May 2022 19:29:23 GMT
RUN apk add --no-cache libsasl
# Tue, 24 May 2022 19:29:30 GMT
ENV MEMCACHED_VERSION=1.6.15
# Tue, 24 May 2022 19:29:36 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Tue, 24 May 2022 19:33:02 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 24 May 2022 19:33:03 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 24 May 2022 19:33:08 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 24 May 2022 19:33:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 24 May 2022 19:33:14 GMT
USER memcache
# Tue, 24 May 2022 19:33:17 GMT
EXPOSE 11211
# Tue, 24 May 2022 19:33:19 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:d3deabf2a506ef6f5fa7c2a68bf27047574cef9908b30a97ff2d01ae539b089a`  
		Last Modified: Mon, 23 May 2022 19:09:13 GMT  
		Size: 2.8 MB (2789745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b479cfab13a2f2ffe6bfc643d96b2ca17a80380353869913b72735725a953596`  
		Last Modified: Tue, 24 May 2022 19:34:20 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9111d00ba5c4381f0f8b185e1703815ef94004e492b01b0d3c7a7fe53acc977`  
		Last Modified: Tue, 24 May 2022 19:34:21 GMT  
		Size: 126.0 KB (126043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1a992983a73a33de517b221e813f6ddddea412212564e886bba2a9a09f82735`  
		Last Modified: Tue, 24 May 2022 19:34:21 GMT  
		Size: 974.3 KB (974333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6de2f26a895426d80205ef485568a93b91456d9913ce062578d21db1d228ef7`  
		Last Modified: Tue, 24 May 2022 19:34:20 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27f443297da5126d218f0cfd07deeb374b4db49ce895657aed034e4eba40ce1c`  
		Last Modified: Tue, 24 May 2022 19:34:20 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-alpine3.16` - linux; s390x

```console
$ docker pull memcached@sha256:79c15e8f5b25e585bc279ba8a2e990aaf1bcb0622e4b2cfe246b32381748232d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.6 MB (3629283 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3984c3293b24638ac012e61d1d83266b40194c43831d6d2f59fe1c01615baf07`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 23 May 2022 19:41:59 GMT
ADD file:e1852d8ef555a0d3ef6d0b74a898720c82bb9f491430b06a0dd0499497ce118e in / 
# Mon, 23 May 2022 19:42:10 GMT
CMD ["/bin/sh"]
# Tue, 24 May 2022 19:50:13 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 24 May 2022 19:50:14 GMT
RUN apk add --no-cache libsasl
# Tue, 24 May 2022 19:50:15 GMT
ENV MEMCACHED_VERSION=1.6.15
# Tue, 24 May 2022 19:50:15 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Tue, 24 May 2022 19:54:14 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 24 May 2022 19:54:15 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 24 May 2022 19:54:16 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 24 May 2022 19:54:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 24 May 2022 19:54:16 GMT
USER memcache
# Tue, 24 May 2022 19:54:16 GMT
EXPOSE 11211
# Tue, 24 May 2022 19:54:16 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:af1ac1a73384e058591d04d19bc05a06781cc32d52d4593b468d6cb95eda9858`  
		Last Modified: Mon, 23 May 2022 19:43:36 GMT  
		Size: 2.6 MB (2580494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0cdb25dad8a9e7c836addf0dfee4462f64217c81619f5c7519d620c59c68fff`  
		Last Modified: Tue, 24 May 2022 19:55:16 GMT  
		Size: 1.3 KB (1265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bfb96fb83213592db4a96cd8313433230d559f81caa115c56c8f9018d5e01f5`  
		Last Modified: Tue, 24 May 2022 19:55:16 GMT  
		Size: 112.5 KB (112500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fd8f0273e1af52c2d6bc2ea6e8f7c7b516ce039d78151fe854039d86e62db91`  
		Last Modified: Tue, 24 May 2022 19:55:17 GMT  
		Size: 934.6 KB (934620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a50bb84155cee8c93b5835daaee0a57b7c14397817ac75279b1ac51d2626f594`  
		Last Modified: Tue, 24 May 2022 19:55:16 GMT  
		Size: 283.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:196f82f950409b7b7c0e395502911ba3177047647ed8ac24e62c49dacf4eebf1`  
		Last Modified: Tue, 24 May 2022 19:55:17 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:1-bullseye`

```console
$ docker pull memcached@sha256:b422bca20902101cd4a427ccda5ea9729a89bdc6cd8ab8a7d8cd09b1470af6b6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; s390x

### `memcached:1-bullseye` - linux; amd64

```console
$ docker pull memcached@sha256:1be4a685ac5a327ffbd7d1c7240378e7156824f9406b1eeb5fe19eadc2e61c53
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.0 MB (32968544 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a23fd759590b790a7cae87582ba4d747378de71b47e581b9295c02ce34eb9ed0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 23 Jun 2022 00:20:27 GMT
ADD file:8adbbab04d6f84cd83b5f4205b89b0acb7ecbf27a1bb2dc181d0a629479039fe in / 
# Thu, 23 Jun 2022 00:20:27 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 04:18:20 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Thu, 23 Jun 2022 04:18:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 04:18:24 GMT
ENV MEMCACHED_VERSION=1.6.15
# Thu, 23 Jun 2022 04:18:24 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Thu, 23 Jun 2022 04:21:07 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 23 Jun 2022 04:21:07 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 23 Jun 2022 04:21:08 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 23 Jun 2022 04:21:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jun 2022 04:21:08 GMT
USER memcache
# Thu, 23 Jun 2022 04:21:08 GMT
EXPOSE 11211
# Thu, 23 Jun 2022 04:21:08 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:b85a868b505ffd0342a37e6a3b1c49f7c71878afe569a807e6238ef08252fcb7`  
		Last Modified: Thu, 23 Jun 2022 00:25:18 GMT  
		Size: 31.4 MB (31379408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f58bb523c8de07d0d72658b2e622e82f065a1adef45f6f90f11eb7c71b9d0c61`  
		Last Modified: Thu, 23 Jun 2022 04:21:33 GMT  
		Size: 5.0 KB (4979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a458d61c2cd35b8afffe3741b04321a87f86ba216e5e2a4f9429b83b32ceb35`  
		Last Modified: Thu, 23 Jun 2022 04:21:33 GMT  
		Size: 328.1 KB (328115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7eda168e1238eaa8f5c20b7240bb8bc84c9a3f7b4b8cdc0be18f58f27bff1692`  
		Last Modified: Thu, 23 Jun 2022 04:21:33 GMT  
		Size: 1.3 MB (1255633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f188c32090c0c66f2f209fedc0778269d3edf2ad9db239ac0d2e1e3b64b36fd4`  
		Last Modified: Thu, 23 Jun 2022 04:21:33 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f492776609f9ffcbe6d066f45223bc2da677c44beb7bb0cdc6dfa34271885b34`  
		Last Modified: Thu, 23 Jun 2022 04:21:33 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-bullseye` - linux; arm variant v5

```console
$ docker pull memcached@sha256:54ff97ee8133b4181bff0e30de243b68ffa4ad0a7ecc458e6648a24760c63213
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.5 MB (30470395 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:07faffc84c650af3ec2eb3326c593cd933cba137c34c87589a375371eee849f3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 23 Jun 2022 00:50:38 GMT
ADD file:839c0e211e2260f5d54f2633e53c817c1f59e2394ba4b12f60e01e46cee61011 in / 
# Thu, 23 Jun 2022 00:50:39 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 02:41:47 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Thu, 23 Jun 2022 02:41:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 02:41:58 GMT
ENV MEMCACHED_VERSION=1.6.15
# Thu, 23 Jun 2022 02:41:59 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Thu, 23 Jun 2022 02:46:28 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 23 Jun 2022 02:46:29 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 23 Jun 2022 02:46:31 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 23 Jun 2022 02:46:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jun 2022 02:46:32 GMT
USER memcache
# Thu, 23 Jun 2022 02:46:32 GMT
EXPOSE 11211
# Thu, 23 Jun 2022 02:46:33 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:bd2d3b4056bd1b0310082fc5d17c6d03348601456c4b9306d1a333f1cec561f9`  
		Last Modified: Thu, 23 Jun 2022 01:05:39 GMT  
		Size: 28.9 MB (28921550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f500bb51d193d56af19fbeb8ebc1919ec2e6d04cf9a7d1637ad79cc00397c1b`  
		Last Modified: Thu, 23 Jun 2022 02:47:27 GMT  
		Size: 4.9 KB (4894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c3dc6e5372afc0620e0eeae739b429bee70842f20a15ca8345787a674d5d3b8`  
		Last Modified: Thu, 23 Jun 2022 02:47:28 GMT  
		Size: 316.6 KB (316616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83d6f2e7e5c2a1d3566c4d9cd05fd132529535ba7eaecb00d312c0d0a6055a4c`  
		Last Modified: Thu, 23 Jun 2022 02:47:28 GMT  
		Size: 1.2 MB (1226926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:109349836a4d5f4431660fec9744df70f92475b22644182ae9d77c8c56c8960a`  
		Last Modified: Thu, 23 Jun 2022 02:47:27 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b87ddf1818c82326658f3ca6d444b01978e23d30a7232e4ef1e0f6f0ba4ab18`  
		Last Modified: Thu, 23 Jun 2022 02:47:27 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-bullseye` - linux; arm variant v7

```console
$ docker pull memcached@sha256:b3ddbe1e7ec04512ac9e20555b72ba4b2e7e9ee99138535fabe5e92cc92302b5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.1 MB (28092007 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cbbff85100ff53c710f4caa30445e0ee79ccd0fe61cc91a522821fc5415e6bcf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 23 Jun 2022 00:59:45 GMT
ADD file:925abfb9fc0e4a7cc0c979b12c9bd2607f5c493d37b05535ca010f81beb060a9 in / 
# Thu, 23 Jun 2022 00:59:46 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 22:08:47 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Thu, 23 Jun 2022 22:08:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 22:08:56 GMT
ENV MEMCACHED_VERSION=1.6.15
# Thu, 23 Jun 2022 22:08:56 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Thu, 23 Jun 2022 22:13:04 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 23 Jun 2022 22:13:05 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 23 Jun 2022 22:13:06 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 23 Jun 2022 22:13:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jun 2022 22:13:07 GMT
USER memcache
# Thu, 23 Jun 2022 22:13:08 GMT
EXPOSE 11211
# Thu, 23 Jun 2022 22:13:08 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:d2fd562560d8062a78064adfbfa204521167c301f00f5ab3c65b9c2a54083dba`  
		Last Modified: Thu, 23 Jun 2022 01:15:22 GMT  
		Size: 26.6 MB (26576105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8864d1bfbfd3f4b781316abd42de97a2967a6b20534ffdc4fea6a3de16c1d972`  
		Last Modified: Fri, 24 Jun 2022 01:14:10 GMT  
		Size: 4.9 KB (4897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fa7c6c177f3ba693baa86ed010daf821ca2addfe7f3b8a83c7f52fac209a6e8`  
		Last Modified: Fri, 24 Jun 2022 01:14:10 GMT  
		Size: 312.1 KB (312076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f802ee5fb123a2824f3e6f93144c74f9e1c88159fc819b46f7ed2913ec61281a`  
		Last Modified: Fri, 24 Jun 2022 01:14:11 GMT  
		Size: 1.2 MB (1198521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25b61f87cd4332b040dd59bae91f0701228904433b1955bb4f51b7377db17b00`  
		Last Modified: Fri, 24 Jun 2022 01:14:10 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:532462b4f12685e2093583f1e86c82d5c2c8069b92ccbc9bbcf8efad7dfd3252`  
		Last Modified: Fri, 24 Jun 2022 01:14:10 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-bullseye` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:536f8192668e851874eec7d483055b0af220a7eb0be43010f2f9825e99ab0111
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.4 MB (31444932 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2ce58160065ec196d51dcdc756610352a57f6192b28345989be83b94b8300dec`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 23 Jun 2022 00:40:43 GMT
ADD file:134be48af13f80f3474bf1b080ca781feb7b972148d482849862e55eb2acd61c in / 
# Thu, 23 Jun 2022 00:40:44 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 03:53:19 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Thu, 23 Jun 2022 03:53:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 03:53:24 GMT
ENV MEMCACHED_VERSION=1.6.15
# Thu, 23 Jun 2022 03:53:25 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Thu, 23 Jun 2022 03:56:00 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 23 Jun 2022 03:56:02 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 23 Jun 2022 03:56:02 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 23 Jun 2022 03:56:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jun 2022 03:56:04 GMT
USER memcache
# Thu, 23 Jun 2022 03:56:05 GMT
EXPOSE 11211
# Thu, 23 Jun 2022 03:56:06 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:3b157c852f2736e12f09046f214fe5f6a0b1652bd860269b3988c92a197026e8`  
		Last Modified: Thu, 23 Jun 2022 00:47:22 GMT  
		Size: 30.1 MB (30065720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee776bb67ffbc00ca5100c88e1f7ae63b580bc131c046c3c7138b7fb796683a2`  
		Last Modified: Thu, 23 Jun 2022 03:56:51 GMT  
		Size: 4.9 KB (4904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85b234170a3d54e3ad2be2993a7e7b09550a4e00327804a183e07bc786d01bc8`  
		Last Modified: Thu, 23 Jun 2022 03:56:51 GMT  
		Size: 119.2 KB (119223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a61e7150a45b8305adc14ed47f7beb3e807a7f08223393e6f5382b043b120941`  
		Last Modified: Thu, 23 Jun 2022 03:56:51 GMT  
		Size: 1.3 MB (1254677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ed6ad1685f73da9293938d389b8c24ee8b8af4d04d4c8b502cb6082d58bf349`  
		Last Modified: Thu, 23 Jun 2022 03:56:51 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:276672cde8876c99c646defdc630e9be5ae5cfb33c192102b6387ce99d151179`  
		Last Modified: Thu, 23 Jun 2022 03:56:51 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-bullseye` - linux; 386

```console
$ docker pull memcached@sha256:651e5275f0623232ecfa476f864b6634de4e9ffc6671376c796ffd70e31c83b6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.8 MB (33778463 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31252c746c529da361fcb075711def9645866db716700e15d9e4ce92e96ed3a0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 23 Jun 2022 00:39:33 GMT
ADD file:9d46d3f8fb63833a6dbd8dd796ad541d556046a48342d22e1fd3bffa3fb8e504 in / 
# Thu, 23 Jun 2022 00:39:33 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 03:32:31 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Thu, 23 Jun 2022 03:32:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 03:32:36 GMT
ENV MEMCACHED_VERSION=1.6.15
# Thu, 23 Jun 2022 03:32:37 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Thu, 23 Jun 2022 03:35:28 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 23 Jun 2022 03:35:30 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 23 Jun 2022 03:35:30 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 23 Jun 2022 03:35:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jun 2022 03:35:32 GMT
USER memcache
# Thu, 23 Jun 2022 03:35:33 GMT
EXPOSE 11211
# Thu, 23 Jun 2022 03:35:34 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:4870b12e407743816673c11cfb39974d80c1569d876287bef61f8c585954822f`  
		Last Modified: Thu, 23 Jun 2022 00:46:40 GMT  
		Size: 32.4 MB (32390198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a67b6581e800ff3e02f41dd18cb78bc620a25becd83769f84d2c61aed5d01ea`  
		Last Modified: Thu, 23 Jun 2022 03:36:21 GMT  
		Size: 4.8 KB (4773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b70025d0ac3fc2b23b2e76f6d96c607c6a04b53c9850fe3f14fa855827b9d19d`  
		Last Modified: Thu, 23 Jun 2022 03:36:21 GMT  
		Size: 130.1 KB (130137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a383a40e44984d67c847d2a4bbc7d3525f3867ff39c81a5221970dc744ee822e`  
		Last Modified: Thu, 23 Jun 2022 03:36:21 GMT  
		Size: 1.3 MB (1252947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24f731218f56e8a5f3d250c9a4e15f841afbd92a0ee71f88761feb880aa937b3`  
		Last Modified: Thu, 23 Jun 2022 03:36:21 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15ab75a8041fc16fdde22888eb35315059264f2c153e8d05d7f132d1aa413e3a`  
		Last Modified: Thu, 23 Jun 2022 03:36:21 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-bullseye` - linux; mips64le

```console
$ docker pull memcached@sha256:71ebcf40d19139f8bab5733065ff1b2599e5d52359c6f6cbfad2104be2f1fe33
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.0 MB (31014756 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d95105805101f850723625215940d8b2be96a9b40f984174eee903985becb9e0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 23 Jun 2022 01:10:25 GMT
ADD file:fd1174cc47ac636f0cab382578a899d69ed489e4dee53ec838955e36066f526a in / 
# Thu, 23 Jun 2022 01:10:29 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 03:13:46 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Thu, 23 Jun 2022 03:14:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 03:14:06 GMT
ENV MEMCACHED_VERSION=1.6.15
# Thu, 23 Jun 2022 03:14:08 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Thu, 23 Jun 2022 03:21:07 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 23 Jun 2022 03:21:09 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 23 Jun 2022 03:21:15 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 23 Jun 2022 03:21:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jun 2022 03:21:20 GMT
USER memcache
# Thu, 23 Jun 2022 03:21:22 GMT
EXPOSE 11211
# Thu, 23 Jun 2022 03:21:25 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:9d199cb5e183b38c9edcc527cbaaa79bb56da73bd09ed449223842775ef4a244`  
		Last Modified: Thu, 23 Jun 2022 01:20:19 GMT  
		Size: 29.6 MB (29641027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d188c3e3bf643b15e2e70cc10dab71da1f4e871305c84cf6d927a2750209ee47`  
		Last Modified: Thu, 23 Jun 2022 03:21:53 GMT  
		Size: 4.9 KB (4863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8855d5fcd2d728913f5ae40b13f074576721a44abf081e6bd4e8f48e8deb8262`  
		Last Modified: Thu, 23 Jun 2022 03:21:54 GMT  
		Size: 117.2 KB (117169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:726be3b42973c4aa79e2ffcecb3633c1ec825f8099da6b5d952810bf4d1827cd`  
		Last Modified: Thu, 23 Jun 2022 03:21:54 GMT  
		Size: 1.3 MB (1251289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6176796787c17dc9b41c47c10e23979540bb32e2833c3eeceb1456f0b228166f`  
		Last Modified: Thu, 23 Jun 2022 03:21:54 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:926c03f02a771007ddd9b4fd2172ff2d89647400c4370fdedb4533a5c99e42b1`  
		Last Modified: Thu, 23 Jun 2022 03:21:53 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-bullseye` - linux; ppc64le

```console
$ docker pull memcached@sha256:0bfecd8ca43abc3e50d162ce07d6794beb5d9f98ce929e9371c2542065e6c785
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.0 MB (36972124 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ac53be686814de607770ae7fba96134fc9cd4e5afe7444779b08c02a0c92a6c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 23 Jun 2022 02:02:32 GMT
ADD file:e18c13649ea1f145047652c8e171c4824f9b6b0dbc92127a914c7fca910acf96 in / 
# Thu, 23 Jun 2022 02:02:34 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 08:15:12 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Thu, 23 Jun 2022 08:15:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 08:15:26 GMT
ENV MEMCACHED_VERSION=1.6.15
# Thu, 23 Jun 2022 08:15:30 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Thu, 23 Jun 2022 08:20:21 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 23 Jun 2022 08:20:23 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 23 Jun 2022 08:20:29 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 23 Jun 2022 08:20:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jun 2022 08:20:34 GMT
USER memcache
# Thu, 23 Jun 2022 08:20:36 GMT
EXPOSE 11211
# Thu, 23 Jun 2022 08:20:38 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:7716f0df7ba06b6f1937cd664805984e25e386a4165f2c6acc65356686e35221`  
		Last Modified: Thu, 23 Jun 2022 02:15:20 GMT  
		Size: 35.3 MB (35286823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54d7d03c3543d8cc9dbdea919601e8b8bdebdf5f54f23ee2a186edde48a4025c`  
		Last Modified: Thu, 23 Jun 2022 08:21:29 GMT  
		Size: 5.0 KB (4987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa5efdc63c420d0295d4932cc7467f1a9005b4724f592c4fba99b6c801f57810`  
		Last Modified: Thu, 23 Jun 2022 08:21:29 GMT  
		Size: 357.0 KB (356958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:329e40de463f01938ecac1d284adb38a29fde479486e279cb302d95abe9f4a16`  
		Last Modified: Thu, 23 Jun 2022 08:21:29 GMT  
		Size: 1.3 MB (1322949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d823793235eacc3363db343cea0db041905e9fde59ff5262e0fd8826e962f5a`  
		Last Modified: Thu, 23 Jun 2022 08:21:29 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2ae46dbc3324ea97ee7556a1bc8006b075f7a1492e3a2114aaf8dec7c579b76`  
		Last Modified: Thu, 23 Jun 2022 08:21:29 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-bullseye` - linux; s390x

```console
$ docker pull memcached@sha256:1e49c15efaf9999b31f526130902a04a53eeac416f40d1549e98b3fa1a872c04
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.2 MB (31226391 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b8090a3ed64f97313e1ddce878717e3bf8c1aace9d7bf247a1fa53418081f0c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 23 Jun 2022 00:43:10 GMT
ADD file:0b511e3efd87267fb27161eae56c4d08f0fed733697da6ffe6ea96a4cb68e938 in / 
# Thu, 23 Jun 2022 00:43:15 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 13:41:46 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Thu, 23 Jun 2022 13:41:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 13:41:49 GMT
ENV MEMCACHED_VERSION=1.6.15
# Thu, 23 Jun 2022 13:41:50 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Thu, 23 Jun 2022 13:45:09 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 23 Jun 2022 13:45:09 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 23 Jun 2022 13:45:10 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 23 Jun 2022 13:45:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jun 2022 13:45:10 GMT
USER memcache
# Thu, 23 Jun 2022 13:45:10 GMT
EXPOSE 11211
# Thu, 23 Jun 2022 13:45:10 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:c547f465e0c8708ad0c57cf09caa52f4c2b5b295bf10ab1ce71ca17ff81ea36a`  
		Last Modified: Thu, 23 Jun 2022 00:51:59 GMT  
		Size: 29.7 MB (29655262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04837776e7fbb579dda3720caca85ff9cb19eea15a8830ab0f23a160fa832205`  
		Last Modified: Thu, 23 Jun 2022 13:46:03 GMT  
		Size: 5.0 KB (5025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d844915fd9a66accf5106919c6a63121ed4fde412dcf958133bc1b1483b307b`  
		Last Modified: Thu, 23 Jun 2022 13:46:03 GMT  
		Size: 324.2 KB (324209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51abf5cd3f179d43b5845c7dc42a6f07ddfd6da706ca58f78d53641e3d62289f`  
		Last Modified: Thu, 23 Jun 2022 13:46:03 GMT  
		Size: 1.2 MB (1241485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31ea51fd993089ad7346961b0897d009e18b953416139bf4359ff089b9e9ada9`  
		Last Modified: Thu, 23 Jun 2022 13:46:04 GMT  
		Size: 289.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cda18e1b304fdde7d799586641bad45a035387c02b0c7e8d696e91221b046e28`  
		Last Modified: Thu, 23 Jun 2022 13:46:03 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:1.6`

```console
$ docker pull memcached@sha256:b422bca20902101cd4a427ccda5ea9729a89bdc6cd8ab8a7d8cd09b1470af6b6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; s390x

### `memcached:1.6` - linux; amd64

```console
$ docker pull memcached@sha256:1be4a685ac5a327ffbd7d1c7240378e7156824f9406b1eeb5fe19eadc2e61c53
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.0 MB (32968544 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a23fd759590b790a7cae87582ba4d747378de71b47e581b9295c02ce34eb9ed0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 23 Jun 2022 00:20:27 GMT
ADD file:8adbbab04d6f84cd83b5f4205b89b0acb7ecbf27a1bb2dc181d0a629479039fe in / 
# Thu, 23 Jun 2022 00:20:27 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 04:18:20 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Thu, 23 Jun 2022 04:18:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 04:18:24 GMT
ENV MEMCACHED_VERSION=1.6.15
# Thu, 23 Jun 2022 04:18:24 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Thu, 23 Jun 2022 04:21:07 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 23 Jun 2022 04:21:07 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 23 Jun 2022 04:21:08 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 23 Jun 2022 04:21:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jun 2022 04:21:08 GMT
USER memcache
# Thu, 23 Jun 2022 04:21:08 GMT
EXPOSE 11211
# Thu, 23 Jun 2022 04:21:08 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:b85a868b505ffd0342a37e6a3b1c49f7c71878afe569a807e6238ef08252fcb7`  
		Last Modified: Thu, 23 Jun 2022 00:25:18 GMT  
		Size: 31.4 MB (31379408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f58bb523c8de07d0d72658b2e622e82f065a1adef45f6f90f11eb7c71b9d0c61`  
		Last Modified: Thu, 23 Jun 2022 04:21:33 GMT  
		Size: 5.0 KB (4979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a458d61c2cd35b8afffe3741b04321a87f86ba216e5e2a4f9429b83b32ceb35`  
		Last Modified: Thu, 23 Jun 2022 04:21:33 GMT  
		Size: 328.1 KB (328115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7eda168e1238eaa8f5c20b7240bb8bc84c9a3f7b4b8cdc0be18f58f27bff1692`  
		Last Modified: Thu, 23 Jun 2022 04:21:33 GMT  
		Size: 1.3 MB (1255633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f188c32090c0c66f2f209fedc0778269d3edf2ad9db239ac0d2e1e3b64b36fd4`  
		Last Modified: Thu, 23 Jun 2022 04:21:33 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f492776609f9ffcbe6d066f45223bc2da677c44beb7bb0cdc6dfa34271885b34`  
		Last Modified: Thu, 23 Jun 2022 04:21:33 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6` - linux; arm variant v5

```console
$ docker pull memcached@sha256:54ff97ee8133b4181bff0e30de243b68ffa4ad0a7ecc458e6648a24760c63213
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.5 MB (30470395 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:07faffc84c650af3ec2eb3326c593cd933cba137c34c87589a375371eee849f3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 23 Jun 2022 00:50:38 GMT
ADD file:839c0e211e2260f5d54f2633e53c817c1f59e2394ba4b12f60e01e46cee61011 in / 
# Thu, 23 Jun 2022 00:50:39 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 02:41:47 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Thu, 23 Jun 2022 02:41:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 02:41:58 GMT
ENV MEMCACHED_VERSION=1.6.15
# Thu, 23 Jun 2022 02:41:59 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Thu, 23 Jun 2022 02:46:28 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 23 Jun 2022 02:46:29 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 23 Jun 2022 02:46:31 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 23 Jun 2022 02:46:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jun 2022 02:46:32 GMT
USER memcache
# Thu, 23 Jun 2022 02:46:32 GMT
EXPOSE 11211
# Thu, 23 Jun 2022 02:46:33 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:bd2d3b4056bd1b0310082fc5d17c6d03348601456c4b9306d1a333f1cec561f9`  
		Last Modified: Thu, 23 Jun 2022 01:05:39 GMT  
		Size: 28.9 MB (28921550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f500bb51d193d56af19fbeb8ebc1919ec2e6d04cf9a7d1637ad79cc00397c1b`  
		Last Modified: Thu, 23 Jun 2022 02:47:27 GMT  
		Size: 4.9 KB (4894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c3dc6e5372afc0620e0eeae739b429bee70842f20a15ca8345787a674d5d3b8`  
		Last Modified: Thu, 23 Jun 2022 02:47:28 GMT  
		Size: 316.6 KB (316616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83d6f2e7e5c2a1d3566c4d9cd05fd132529535ba7eaecb00d312c0d0a6055a4c`  
		Last Modified: Thu, 23 Jun 2022 02:47:28 GMT  
		Size: 1.2 MB (1226926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:109349836a4d5f4431660fec9744df70f92475b22644182ae9d77c8c56c8960a`  
		Last Modified: Thu, 23 Jun 2022 02:47:27 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b87ddf1818c82326658f3ca6d444b01978e23d30a7232e4ef1e0f6f0ba4ab18`  
		Last Modified: Thu, 23 Jun 2022 02:47:27 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6` - linux; arm variant v7

```console
$ docker pull memcached@sha256:b3ddbe1e7ec04512ac9e20555b72ba4b2e7e9ee99138535fabe5e92cc92302b5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.1 MB (28092007 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cbbff85100ff53c710f4caa30445e0ee79ccd0fe61cc91a522821fc5415e6bcf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 23 Jun 2022 00:59:45 GMT
ADD file:925abfb9fc0e4a7cc0c979b12c9bd2607f5c493d37b05535ca010f81beb060a9 in / 
# Thu, 23 Jun 2022 00:59:46 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 22:08:47 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Thu, 23 Jun 2022 22:08:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 22:08:56 GMT
ENV MEMCACHED_VERSION=1.6.15
# Thu, 23 Jun 2022 22:08:56 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Thu, 23 Jun 2022 22:13:04 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 23 Jun 2022 22:13:05 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 23 Jun 2022 22:13:06 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 23 Jun 2022 22:13:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jun 2022 22:13:07 GMT
USER memcache
# Thu, 23 Jun 2022 22:13:08 GMT
EXPOSE 11211
# Thu, 23 Jun 2022 22:13:08 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:d2fd562560d8062a78064adfbfa204521167c301f00f5ab3c65b9c2a54083dba`  
		Last Modified: Thu, 23 Jun 2022 01:15:22 GMT  
		Size: 26.6 MB (26576105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8864d1bfbfd3f4b781316abd42de97a2967a6b20534ffdc4fea6a3de16c1d972`  
		Last Modified: Fri, 24 Jun 2022 01:14:10 GMT  
		Size: 4.9 KB (4897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fa7c6c177f3ba693baa86ed010daf821ca2addfe7f3b8a83c7f52fac209a6e8`  
		Last Modified: Fri, 24 Jun 2022 01:14:10 GMT  
		Size: 312.1 KB (312076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f802ee5fb123a2824f3e6f93144c74f9e1c88159fc819b46f7ed2913ec61281a`  
		Last Modified: Fri, 24 Jun 2022 01:14:11 GMT  
		Size: 1.2 MB (1198521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25b61f87cd4332b040dd59bae91f0701228904433b1955bb4f51b7377db17b00`  
		Last Modified: Fri, 24 Jun 2022 01:14:10 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:532462b4f12685e2093583f1e86c82d5c2c8069b92ccbc9bbcf8efad7dfd3252`  
		Last Modified: Fri, 24 Jun 2022 01:14:10 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:536f8192668e851874eec7d483055b0af220a7eb0be43010f2f9825e99ab0111
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.4 MB (31444932 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2ce58160065ec196d51dcdc756610352a57f6192b28345989be83b94b8300dec`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 23 Jun 2022 00:40:43 GMT
ADD file:134be48af13f80f3474bf1b080ca781feb7b972148d482849862e55eb2acd61c in / 
# Thu, 23 Jun 2022 00:40:44 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 03:53:19 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Thu, 23 Jun 2022 03:53:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 03:53:24 GMT
ENV MEMCACHED_VERSION=1.6.15
# Thu, 23 Jun 2022 03:53:25 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Thu, 23 Jun 2022 03:56:00 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 23 Jun 2022 03:56:02 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 23 Jun 2022 03:56:02 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 23 Jun 2022 03:56:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jun 2022 03:56:04 GMT
USER memcache
# Thu, 23 Jun 2022 03:56:05 GMT
EXPOSE 11211
# Thu, 23 Jun 2022 03:56:06 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:3b157c852f2736e12f09046f214fe5f6a0b1652bd860269b3988c92a197026e8`  
		Last Modified: Thu, 23 Jun 2022 00:47:22 GMT  
		Size: 30.1 MB (30065720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee776bb67ffbc00ca5100c88e1f7ae63b580bc131c046c3c7138b7fb796683a2`  
		Last Modified: Thu, 23 Jun 2022 03:56:51 GMT  
		Size: 4.9 KB (4904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85b234170a3d54e3ad2be2993a7e7b09550a4e00327804a183e07bc786d01bc8`  
		Last Modified: Thu, 23 Jun 2022 03:56:51 GMT  
		Size: 119.2 KB (119223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a61e7150a45b8305adc14ed47f7beb3e807a7f08223393e6f5382b043b120941`  
		Last Modified: Thu, 23 Jun 2022 03:56:51 GMT  
		Size: 1.3 MB (1254677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ed6ad1685f73da9293938d389b8c24ee8b8af4d04d4c8b502cb6082d58bf349`  
		Last Modified: Thu, 23 Jun 2022 03:56:51 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:276672cde8876c99c646defdc630e9be5ae5cfb33c192102b6387ce99d151179`  
		Last Modified: Thu, 23 Jun 2022 03:56:51 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6` - linux; 386

```console
$ docker pull memcached@sha256:651e5275f0623232ecfa476f864b6634de4e9ffc6671376c796ffd70e31c83b6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.8 MB (33778463 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31252c746c529da361fcb075711def9645866db716700e15d9e4ce92e96ed3a0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 23 Jun 2022 00:39:33 GMT
ADD file:9d46d3f8fb63833a6dbd8dd796ad541d556046a48342d22e1fd3bffa3fb8e504 in / 
# Thu, 23 Jun 2022 00:39:33 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 03:32:31 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Thu, 23 Jun 2022 03:32:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 03:32:36 GMT
ENV MEMCACHED_VERSION=1.6.15
# Thu, 23 Jun 2022 03:32:37 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Thu, 23 Jun 2022 03:35:28 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 23 Jun 2022 03:35:30 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 23 Jun 2022 03:35:30 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 23 Jun 2022 03:35:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jun 2022 03:35:32 GMT
USER memcache
# Thu, 23 Jun 2022 03:35:33 GMT
EXPOSE 11211
# Thu, 23 Jun 2022 03:35:34 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:4870b12e407743816673c11cfb39974d80c1569d876287bef61f8c585954822f`  
		Last Modified: Thu, 23 Jun 2022 00:46:40 GMT  
		Size: 32.4 MB (32390198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a67b6581e800ff3e02f41dd18cb78bc620a25becd83769f84d2c61aed5d01ea`  
		Last Modified: Thu, 23 Jun 2022 03:36:21 GMT  
		Size: 4.8 KB (4773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b70025d0ac3fc2b23b2e76f6d96c607c6a04b53c9850fe3f14fa855827b9d19d`  
		Last Modified: Thu, 23 Jun 2022 03:36:21 GMT  
		Size: 130.1 KB (130137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a383a40e44984d67c847d2a4bbc7d3525f3867ff39c81a5221970dc744ee822e`  
		Last Modified: Thu, 23 Jun 2022 03:36:21 GMT  
		Size: 1.3 MB (1252947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24f731218f56e8a5f3d250c9a4e15f841afbd92a0ee71f88761feb880aa937b3`  
		Last Modified: Thu, 23 Jun 2022 03:36:21 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15ab75a8041fc16fdde22888eb35315059264f2c153e8d05d7f132d1aa413e3a`  
		Last Modified: Thu, 23 Jun 2022 03:36:21 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6` - linux; mips64le

```console
$ docker pull memcached@sha256:71ebcf40d19139f8bab5733065ff1b2599e5d52359c6f6cbfad2104be2f1fe33
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.0 MB (31014756 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d95105805101f850723625215940d8b2be96a9b40f984174eee903985becb9e0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 23 Jun 2022 01:10:25 GMT
ADD file:fd1174cc47ac636f0cab382578a899d69ed489e4dee53ec838955e36066f526a in / 
# Thu, 23 Jun 2022 01:10:29 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 03:13:46 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Thu, 23 Jun 2022 03:14:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 03:14:06 GMT
ENV MEMCACHED_VERSION=1.6.15
# Thu, 23 Jun 2022 03:14:08 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Thu, 23 Jun 2022 03:21:07 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 23 Jun 2022 03:21:09 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 23 Jun 2022 03:21:15 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 23 Jun 2022 03:21:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jun 2022 03:21:20 GMT
USER memcache
# Thu, 23 Jun 2022 03:21:22 GMT
EXPOSE 11211
# Thu, 23 Jun 2022 03:21:25 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:9d199cb5e183b38c9edcc527cbaaa79bb56da73bd09ed449223842775ef4a244`  
		Last Modified: Thu, 23 Jun 2022 01:20:19 GMT  
		Size: 29.6 MB (29641027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d188c3e3bf643b15e2e70cc10dab71da1f4e871305c84cf6d927a2750209ee47`  
		Last Modified: Thu, 23 Jun 2022 03:21:53 GMT  
		Size: 4.9 KB (4863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8855d5fcd2d728913f5ae40b13f074576721a44abf081e6bd4e8f48e8deb8262`  
		Last Modified: Thu, 23 Jun 2022 03:21:54 GMT  
		Size: 117.2 KB (117169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:726be3b42973c4aa79e2ffcecb3633c1ec825f8099da6b5d952810bf4d1827cd`  
		Last Modified: Thu, 23 Jun 2022 03:21:54 GMT  
		Size: 1.3 MB (1251289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6176796787c17dc9b41c47c10e23979540bb32e2833c3eeceb1456f0b228166f`  
		Last Modified: Thu, 23 Jun 2022 03:21:54 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:926c03f02a771007ddd9b4fd2172ff2d89647400c4370fdedb4533a5c99e42b1`  
		Last Modified: Thu, 23 Jun 2022 03:21:53 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6` - linux; ppc64le

```console
$ docker pull memcached@sha256:0bfecd8ca43abc3e50d162ce07d6794beb5d9f98ce929e9371c2542065e6c785
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.0 MB (36972124 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ac53be686814de607770ae7fba96134fc9cd4e5afe7444779b08c02a0c92a6c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 23 Jun 2022 02:02:32 GMT
ADD file:e18c13649ea1f145047652c8e171c4824f9b6b0dbc92127a914c7fca910acf96 in / 
# Thu, 23 Jun 2022 02:02:34 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 08:15:12 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Thu, 23 Jun 2022 08:15:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 08:15:26 GMT
ENV MEMCACHED_VERSION=1.6.15
# Thu, 23 Jun 2022 08:15:30 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Thu, 23 Jun 2022 08:20:21 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 23 Jun 2022 08:20:23 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 23 Jun 2022 08:20:29 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 23 Jun 2022 08:20:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jun 2022 08:20:34 GMT
USER memcache
# Thu, 23 Jun 2022 08:20:36 GMT
EXPOSE 11211
# Thu, 23 Jun 2022 08:20:38 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:7716f0df7ba06b6f1937cd664805984e25e386a4165f2c6acc65356686e35221`  
		Last Modified: Thu, 23 Jun 2022 02:15:20 GMT  
		Size: 35.3 MB (35286823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54d7d03c3543d8cc9dbdea919601e8b8bdebdf5f54f23ee2a186edde48a4025c`  
		Last Modified: Thu, 23 Jun 2022 08:21:29 GMT  
		Size: 5.0 KB (4987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa5efdc63c420d0295d4932cc7467f1a9005b4724f592c4fba99b6c801f57810`  
		Last Modified: Thu, 23 Jun 2022 08:21:29 GMT  
		Size: 357.0 KB (356958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:329e40de463f01938ecac1d284adb38a29fde479486e279cb302d95abe9f4a16`  
		Last Modified: Thu, 23 Jun 2022 08:21:29 GMT  
		Size: 1.3 MB (1322949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d823793235eacc3363db343cea0db041905e9fde59ff5262e0fd8826e962f5a`  
		Last Modified: Thu, 23 Jun 2022 08:21:29 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2ae46dbc3324ea97ee7556a1bc8006b075f7a1492e3a2114aaf8dec7c579b76`  
		Last Modified: Thu, 23 Jun 2022 08:21:29 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6` - linux; s390x

```console
$ docker pull memcached@sha256:1e49c15efaf9999b31f526130902a04a53eeac416f40d1549e98b3fa1a872c04
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.2 MB (31226391 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b8090a3ed64f97313e1ddce878717e3bf8c1aace9d7bf247a1fa53418081f0c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 23 Jun 2022 00:43:10 GMT
ADD file:0b511e3efd87267fb27161eae56c4d08f0fed733697da6ffe6ea96a4cb68e938 in / 
# Thu, 23 Jun 2022 00:43:15 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 13:41:46 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Thu, 23 Jun 2022 13:41:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 13:41:49 GMT
ENV MEMCACHED_VERSION=1.6.15
# Thu, 23 Jun 2022 13:41:50 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Thu, 23 Jun 2022 13:45:09 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 23 Jun 2022 13:45:09 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 23 Jun 2022 13:45:10 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 23 Jun 2022 13:45:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jun 2022 13:45:10 GMT
USER memcache
# Thu, 23 Jun 2022 13:45:10 GMT
EXPOSE 11211
# Thu, 23 Jun 2022 13:45:10 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:c547f465e0c8708ad0c57cf09caa52f4c2b5b295bf10ab1ce71ca17ff81ea36a`  
		Last Modified: Thu, 23 Jun 2022 00:51:59 GMT  
		Size: 29.7 MB (29655262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04837776e7fbb579dda3720caca85ff9cb19eea15a8830ab0f23a160fa832205`  
		Last Modified: Thu, 23 Jun 2022 13:46:03 GMT  
		Size: 5.0 KB (5025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d844915fd9a66accf5106919c6a63121ed4fde412dcf958133bc1b1483b307b`  
		Last Modified: Thu, 23 Jun 2022 13:46:03 GMT  
		Size: 324.2 KB (324209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51abf5cd3f179d43b5845c7dc42a6f07ddfd6da706ca58f78d53641e3d62289f`  
		Last Modified: Thu, 23 Jun 2022 13:46:03 GMT  
		Size: 1.2 MB (1241485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31ea51fd993089ad7346961b0897d009e18b953416139bf4359ff089b9e9ada9`  
		Last Modified: Thu, 23 Jun 2022 13:46:04 GMT  
		Size: 289.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cda18e1b304fdde7d799586641bad45a035387c02b0c7e8d696e91221b046e28`  
		Last Modified: Thu, 23 Jun 2022 13:46:03 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:1.6-alpine`

```console
$ docker pull memcached@sha256:96af3fed9ef980101602ea90c3220679bb326bfe70474e4f06759f25db4591e2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `memcached:1.6-alpine` - linux; amd64

```console
$ docker pull memcached@sha256:bae66da0e8cdb7daa226cc0837e2562404a4007466044ffdfa88a8a0431d5c7a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3853361 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e3f5d6e8d61d2ec54ff3d21da1c6dbddca8f0018c8f1c1253287129fa3926d7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 23 May 2022 19:19:30 GMT
ADD file:8e81116368669ed3dd361bc898d61bff249f524139a239fdaf3ec46869a39921 in / 
# Mon, 23 May 2022 19:19:31 GMT
CMD ["/bin/sh"]
# Tue, 24 May 2022 19:24:21 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 24 May 2022 19:24:23 GMT
RUN apk add --no-cache libsasl
# Tue, 24 May 2022 19:24:23 GMT
ENV MEMCACHED_VERSION=1.6.15
# Tue, 24 May 2022 19:24:23 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Tue, 24 May 2022 19:27:18 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 24 May 2022 19:27:18 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 24 May 2022 19:27:19 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 24 May 2022 19:27:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 24 May 2022 19:27:19 GMT
USER memcache
# Tue, 24 May 2022 19:27:19 GMT
EXPOSE 11211
# Tue, 24 May 2022 19:27:19 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:2408cc74d12b6cd092bb8b516ba7d5e290f485d3eb9672efc00f0583730179e8`  
		Last Modified: Mon, 23 May 2022 19:09:38 GMT  
		Size: 2.8 MB (2798889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6da329a3b4330a0705bfb49b5e6ce2fb61bc108d0a32d41c2c0dad6d9dd6c8fa`  
		Last Modified: Tue, 24 May 2022 19:27:48 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f4ba002bd64c19ecd49e1afc372709c9bcfb3dbe2b9ee2b02d43dea8fddc3cc`  
		Last Modified: Tue, 24 May 2022 19:27:48 GMT  
		Size: 108.3 KB (108307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d664dde428a76ca57c1261382f6f9b758a3b5b0e12b51f6a5b1a38bef237456a`  
		Last Modified: Tue, 24 May 2022 19:27:48 GMT  
		Size: 944.5 KB (944489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef11efc606151d8228ae06848232d8d65ae50082bf0ad5c5104d06c27ce7c85d`  
		Last Modified: Tue, 24 May 2022 19:27:48 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f118f0edbe76d09a02e63a4712d1b9b3eb1ebce2a271c740baba58cc48df9f4e`  
		Last Modified: Tue, 24 May 2022 19:27:48 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

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
$ docker pull memcached@sha256:8ec1f6a98e264e73e3c7b2feba04b272ce1522adc9d40118b9684721c41122b0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.7 MB (3737167 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f393a4888061e0456042ebb89fbc11cf72af15c189e0d0e4ee62b7fcfd44c683`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 23 May 2022 19:39:22 GMT
ADD file:3ae36c6c4a1fc43157692da97c6c4fa6c3d0189ba82e2bef7f5aaf4a5e083f18 in / 
# Mon, 23 May 2022 19:39:22 GMT
CMD ["/bin/sh"]
# Tue, 24 May 2022 20:08:53 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 24 May 2022 20:08:55 GMT
RUN apk add --no-cache libsasl
# Tue, 24 May 2022 20:08:56 GMT
ENV MEMCACHED_VERSION=1.6.15
# Tue, 24 May 2022 20:08:57 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Tue, 24 May 2022 20:12:06 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 24 May 2022 20:12:08 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 24 May 2022 20:12:08 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 24 May 2022 20:12:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 24 May 2022 20:12:10 GMT
USER memcache
# Tue, 24 May 2022 20:12:11 GMT
EXPOSE 11211
# Tue, 24 May 2022 20:12:12 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:b3c136eddcbf2003d3180787cef00f39d46b9fd9e4623178282ad6a8d63ad3b0`  
		Last Modified: Mon, 23 May 2022 19:08:34 GMT  
		Size: 2.7 MB (2694464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e87d2d7a8c9bc1317afe928c225caaafd86b3b73a2bc359f8037eb0f501b394c`  
		Last Modified: Tue, 24 May 2022 20:12:58 GMT  
		Size: 1.2 KB (1242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55dbcde2059d799697807a93b36d71cd601b20e2218abb7cb9261d22e8a7d67a`  
		Last Modified: Tue, 24 May 2022 20:12:58 GMT  
		Size: 109.6 KB (109557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4aa3db0ac20b8381c09df00576661af3c209195453eeeb892b8532059b932a39`  
		Last Modified: Tue, 24 May 2022 20:12:59 GMT  
		Size: 931.5 KB (931496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d999e908ec416e199da213e6fca67cdc82d3d440098a1bfbc5bc7c5a2f35636`  
		Last Modified: Tue, 24 May 2022 20:12:58 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8017baa48e45fa47c2fab6975dcd0ab8a560c64c0de05f7113831a537b385a3b`  
		Last Modified: Tue, 24 May 2022 20:12:58 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-alpine` - linux; 386

```console
$ docker pull memcached@sha256:3560af36f0aaeb7e4d2da47f0ad4a91bc675aa017423f34911490b09908230e8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3878370 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7d5a231eedb6e0b20291a77ac7a71c5a16aca1a9eb62893e285cefa1b95bdf5b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 23 May 2022 19:38:20 GMT
ADD file:1750ccfabfe93636015070d51a6e824cbd738056223421c69d8aaabc38041b18 in / 
# Mon, 23 May 2022 19:38:20 GMT
CMD ["/bin/sh"]
# Tue, 24 May 2022 19:46:24 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 24 May 2022 19:46:26 GMT
RUN apk add --no-cache libsasl
# Tue, 24 May 2022 19:46:26 GMT
ENV MEMCACHED_VERSION=1.6.15
# Tue, 24 May 2022 19:46:27 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Tue, 24 May 2022 19:49:17 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 24 May 2022 19:49:19 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 24 May 2022 19:49:19 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 24 May 2022 19:49:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 24 May 2022 19:49:21 GMT
USER memcache
# Tue, 24 May 2022 19:49:22 GMT
EXPOSE 11211
# Tue, 24 May 2022 19:49:23 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:bb638a3869eed698f88775c7a48f36f8e22e7c6bbaa98fa1d5678966b619b859`  
		Last Modified: Mon, 23 May 2022 19:09:25 GMT  
		Size: 2.8 MB (2801887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d301e0dbe5a2594f09f110ec3c1e79f4bd885af78b4992bf8af7a9f7b0507d5a`  
		Last Modified: Tue, 24 May 2022 19:50:14 GMT  
		Size: 1.2 KB (1242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:880ddc23b9c3165a8e86c64a648782c63c9a7271e84df6ac2f5a8c110d32258d`  
		Last Modified: Tue, 24 May 2022 19:50:14 GMT  
		Size: 119.8 KB (119821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c60884a7874466d1525bb0560fcbbbc226cfb4fb1507f1bd0d45d4f1b0e1307b`  
		Last Modified: Tue, 24 May 2022 19:50:15 GMT  
		Size: 955.0 KB (955017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89ad9c1959a10762028a884c1a33f06bb71bcb1a9ac372c889304f75f2a4b597`  
		Last Modified: Tue, 24 May 2022 19:50:14 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b267a8907abfcf28b9d96b17379ce57985989f17d34c06dfd238aee8ed0da61`  
		Last Modified: Tue, 24 May 2022 19:50:14 GMT  
		Size: 119.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-alpine` - linux; ppc64le

```console
$ docker pull memcached@sha256:edeccd4ca90cecc053bd78239bef1a1ccec0d2f189655d39e29e44216157fec4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3891798 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:348c555fa9d4bcfd44f2f7426151f1666fd08a28ce9fea73c503bc207229c503`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 23 May 2022 19:16:51 GMT
ADD file:6a5450c8a7cee3ceda59e7cb350c54df4139b0f7b7cf49c8b31bb9c01646c3cd in / 
# Mon, 23 May 2022 19:16:53 GMT
CMD ["/bin/sh"]
# Tue, 24 May 2022 19:29:15 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 24 May 2022 19:29:23 GMT
RUN apk add --no-cache libsasl
# Tue, 24 May 2022 19:29:30 GMT
ENV MEMCACHED_VERSION=1.6.15
# Tue, 24 May 2022 19:29:36 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Tue, 24 May 2022 19:33:02 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 24 May 2022 19:33:03 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 24 May 2022 19:33:08 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 24 May 2022 19:33:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 24 May 2022 19:33:14 GMT
USER memcache
# Tue, 24 May 2022 19:33:17 GMT
EXPOSE 11211
# Tue, 24 May 2022 19:33:19 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:d3deabf2a506ef6f5fa7c2a68bf27047574cef9908b30a97ff2d01ae539b089a`  
		Last Modified: Mon, 23 May 2022 19:09:13 GMT  
		Size: 2.8 MB (2789745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b479cfab13a2f2ffe6bfc643d96b2ca17a80380353869913b72735725a953596`  
		Last Modified: Tue, 24 May 2022 19:34:20 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9111d00ba5c4381f0f8b185e1703815ef94004e492b01b0d3c7a7fe53acc977`  
		Last Modified: Tue, 24 May 2022 19:34:21 GMT  
		Size: 126.0 KB (126043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1a992983a73a33de517b221e813f6ddddea412212564e886bba2a9a09f82735`  
		Last Modified: Tue, 24 May 2022 19:34:21 GMT  
		Size: 974.3 KB (974333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6de2f26a895426d80205ef485568a93b91456d9913ce062578d21db1d228ef7`  
		Last Modified: Tue, 24 May 2022 19:34:20 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27f443297da5126d218f0cfd07deeb374b4db49ce895657aed034e4eba40ce1c`  
		Last Modified: Tue, 24 May 2022 19:34:20 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-alpine` - linux; s390x

```console
$ docker pull memcached@sha256:79c15e8f5b25e585bc279ba8a2e990aaf1bcb0622e4b2cfe246b32381748232d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.6 MB (3629283 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3984c3293b24638ac012e61d1d83266b40194c43831d6d2f59fe1c01615baf07`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 23 May 2022 19:41:59 GMT
ADD file:e1852d8ef555a0d3ef6d0b74a898720c82bb9f491430b06a0dd0499497ce118e in / 
# Mon, 23 May 2022 19:42:10 GMT
CMD ["/bin/sh"]
# Tue, 24 May 2022 19:50:13 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 24 May 2022 19:50:14 GMT
RUN apk add --no-cache libsasl
# Tue, 24 May 2022 19:50:15 GMT
ENV MEMCACHED_VERSION=1.6.15
# Tue, 24 May 2022 19:50:15 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Tue, 24 May 2022 19:54:14 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 24 May 2022 19:54:15 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 24 May 2022 19:54:16 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 24 May 2022 19:54:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 24 May 2022 19:54:16 GMT
USER memcache
# Tue, 24 May 2022 19:54:16 GMT
EXPOSE 11211
# Tue, 24 May 2022 19:54:16 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:af1ac1a73384e058591d04d19bc05a06781cc32d52d4593b468d6cb95eda9858`  
		Last Modified: Mon, 23 May 2022 19:43:36 GMT  
		Size: 2.6 MB (2580494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0cdb25dad8a9e7c836addf0dfee4462f64217c81619f5c7519d620c59c68fff`  
		Last Modified: Tue, 24 May 2022 19:55:16 GMT  
		Size: 1.3 KB (1265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bfb96fb83213592db4a96cd8313433230d559f81caa115c56c8f9018d5e01f5`  
		Last Modified: Tue, 24 May 2022 19:55:16 GMT  
		Size: 112.5 KB (112500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fd8f0273e1af52c2d6bc2ea6e8f7c7b516ce039d78151fe854039d86e62db91`  
		Last Modified: Tue, 24 May 2022 19:55:17 GMT  
		Size: 934.6 KB (934620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a50bb84155cee8c93b5835daaee0a57b7c14397817ac75279b1ac51d2626f594`  
		Last Modified: Tue, 24 May 2022 19:55:16 GMT  
		Size: 283.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:196f82f950409b7b7c0e395502911ba3177047647ed8ac24e62c49dacf4eebf1`  
		Last Modified: Tue, 24 May 2022 19:55:17 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:1.6-alpine3.16`

```console
$ docker pull memcached@sha256:bab32a8a61543525190db12c2a518c3c2331656a4409185f0f4f33a506e3aae7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `memcached:1.6-alpine3.16` - linux; amd64

```console
$ docker pull memcached@sha256:bae66da0e8cdb7daa226cc0837e2562404a4007466044ffdfa88a8a0431d5c7a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3853361 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e3f5d6e8d61d2ec54ff3d21da1c6dbddca8f0018c8f1c1253287129fa3926d7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 23 May 2022 19:19:30 GMT
ADD file:8e81116368669ed3dd361bc898d61bff249f524139a239fdaf3ec46869a39921 in / 
# Mon, 23 May 2022 19:19:31 GMT
CMD ["/bin/sh"]
# Tue, 24 May 2022 19:24:21 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 24 May 2022 19:24:23 GMT
RUN apk add --no-cache libsasl
# Tue, 24 May 2022 19:24:23 GMT
ENV MEMCACHED_VERSION=1.6.15
# Tue, 24 May 2022 19:24:23 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Tue, 24 May 2022 19:27:18 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 24 May 2022 19:27:18 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 24 May 2022 19:27:19 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 24 May 2022 19:27:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 24 May 2022 19:27:19 GMT
USER memcache
# Tue, 24 May 2022 19:27:19 GMT
EXPOSE 11211
# Tue, 24 May 2022 19:27:19 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:2408cc74d12b6cd092bb8b516ba7d5e290f485d3eb9672efc00f0583730179e8`  
		Last Modified: Mon, 23 May 2022 19:09:38 GMT  
		Size: 2.8 MB (2798889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6da329a3b4330a0705bfb49b5e6ce2fb61bc108d0a32d41c2c0dad6d9dd6c8fa`  
		Last Modified: Tue, 24 May 2022 19:27:48 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f4ba002bd64c19ecd49e1afc372709c9bcfb3dbe2b9ee2b02d43dea8fddc3cc`  
		Last Modified: Tue, 24 May 2022 19:27:48 GMT  
		Size: 108.3 KB (108307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d664dde428a76ca57c1261382f6f9b758a3b5b0e12b51f6a5b1a38bef237456a`  
		Last Modified: Tue, 24 May 2022 19:27:48 GMT  
		Size: 944.5 KB (944489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef11efc606151d8228ae06848232d8d65ae50082bf0ad5c5104d06c27ce7c85d`  
		Last Modified: Tue, 24 May 2022 19:27:48 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f118f0edbe76d09a02e63a4712d1b9b3eb1ebce2a271c740baba58cc48df9f4e`  
		Last Modified: Tue, 24 May 2022 19:27:48 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-alpine3.16` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:8ec1f6a98e264e73e3c7b2feba04b272ce1522adc9d40118b9684721c41122b0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.7 MB (3737167 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f393a4888061e0456042ebb89fbc11cf72af15c189e0d0e4ee62b7fcfd44c683`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 23 May 2022 19:39:22 GMT
ADD file:3ae36c6c4a1fc43157692da97c6c4fa6c3d0189ba82e2bef7f5aaf4a5e083f18 in / 
# Mon, 23 May 2022 19:39:22 GMT
CMD ["/bin/sh"]
# Tue, 24 May 2022 20:08:53 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 24 May 2022 20:08:55 GMT
RUN apk add --no-cache libsasl
# Tue, 24 May 2022 20:08:56 GMT
ENV MEMCACHED_VERSION=1.6.15
# Tue, 24 May 2022 20:08:57 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Tue, 24 May 2022 20:12:06 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 24 May 2022 20:12:08 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 24 May 2022 20:12:08 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 24 May 2022 20:12:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 24 May 2022 20:12:10 GMT
USER memcache
# Tue, 24 May 2022 20:12:11 GMT
EXPOSE 11211
# Tue, 24 May 2022 20:12:12 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:b3c136eddcbf2003d3180787cef00f39d46b9fd9e4623178282ad6a8d63ad3b0`  
		Last Modified: Mon, 23 May 2022 19:08:34 GMT  
		Size: 2.7 MB (2694464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e87d2d7a8c9bc1317afe928c225caaafd86b3b73a2bc359f8037eb0f501b394c`  
		Last Modified: Tue, 24 May 2022 20:12:58 GMT  
		Size: 1.2 KB (1242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55dbcde2059d799697807a93b36d71cd601b20e2218abb7cb9261d22e8a7d67a`  
		Last Modified: Tue, 24 May 2022 20:12:58 GMT  
		Size: 109.6 KB (109557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4aa3db0ac20b8381c09df00576661af3c209195453eeeb892b8532059b932a39`  
		Last Modified: Tue, 24 May 2022 20:12:59 GMT  
		Size: 931.5 KB (931496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d999e908ec416e199da213e6fca67cdc82d3d440098a1bfbc5bc7c5a2f35636`  
		Last Modified: Tue, 24 May 2022 20:12:58 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8017baa48e45fa47c2fab6975dcd0ab8a560c64c0de05f7113831a537b385a3b`  
		Last Modified: Tue, 24 May 2022 20:12:58 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-alpine3.16` - linux; 386

```console
$ docker pull memcached@sha256:3560af36f0aaeb7e4d2da47f0ad4a91bc675aa017423f34911490b09908230e8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3878370 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7d5a231eedb6e0b20291a77ac7a71c5a16aca1a9eb62893e285cefa1b95bdf5b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 23 May 2022 19:38:20 GMT
ADD file:1750ccfabfe93636015070d51a6e824cbd738056223421c69d8aaabc38041b18 in / 
# Mon, 23 May 2022 19:38:20 GMT
CMD ["/bin/sh"]
# Tue, 24 May 2022 19:46:24 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 24 May 2022 19:46:26 GMT
RUN apk add --no-cache libsasl
# Tue, 24 May 2022 19:46:26 GMT
ENV MEMCACHED_VERSION=1.6.15
# Tue, 24 May 2022 19:46:27 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Tue, 24 May 2022 19:49:17 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 24 May 2022 19:49:19 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 24 May 2022 19:49:19 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 24 May 2022 19:49:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 24 May 2022 19:49:21 GMT
USER memcache
# Tue, 24 May 2022 19:49:22 GMT
EXPOSE 11211
# Tue, 24 May 2022 19:49:23 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:bb638a3869eed698f88775c7a48f36f8e22e7c6bbaa98fa1d5678966b619b859`  
		Last Modified: Mon, 23 May 2022 19:09:25 GMT  
		Size: 2.8 MB (2801887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d301e0dbe5a2594f09f110ec3c1e79f4bd885af78b4992bf8af7a9f7b0507d5a`  
		Last Modified: Tue, 24 May 2022 19:50:14 GMT  
		Size: 1.2 KB (1242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:880ddc23b9c3165a8e86c64a648782c63c9a7271e84df6ac2f5a8c110d32258d`  
		Last Modified: Tue, 24 May 2022 19:50:14 GMT  
		Size: 119.8 KB (119821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c60884a7874466d1525bb0560fcbbbc226cfb4fb1507f1bd0d45d4f1b0e1307b`  
		Last Modified: Tue, 24 May 2022 19:50:15 GMT  
		Size: 955.0 KB (955017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89ad9c1959a10762028a884c1a33f06bb71bcb1a9ac372c889304f75f2a4b597`  
		Last Modified: Tue, 24 May 2022 19:50:14 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b267a8907abfcf28b9d96b17379ce57985989f17d34c06dfd238aee8ed0da61`  
		Last Modified: Tue, 24 May 2022 19:50:14 GMT  
		Size: 119.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-alpine3.16` - linux; ppc64le

```console
$ docker pull memcached@sha256:edeccd4ca90cecc053bd78239bef1a1ccec0d2f189655d39e29e44216157fec4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3891798 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:348c555fa9d4bcfd44f2f7426151f1666fd08a28ce9fea73c503bc207229c503`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 23 May 2022 19:16:51 GMT
ADD file:6a5450c8a7cee3ceda59e7cb350c54df4139b0f7b7cf49c8b31bb9c01646c3cd in / 
# Mon, 23 May 2022 19:16:53 GMT
CMD ["/bin/sh"]
# Tue, 24 May 2022 19:29:15 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 24 May 2022 19:29:23 GMT
RUN apk add --no-cache libsasl
# Tue, 24 May 2022 19:29:30 GMT
ENV MEMCACHED_VERSION=1.6.15
# Tue, 24 May 2022 19:29:36 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Tue, 24 May 2022 19:33:02 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 24 May 2022 19:33:03 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 24 May 2022 19:33:08 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 24 May 2022 19:33:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 24 May 2022 19:33:14 GMT
USER memcache
# Tue, 24 May 2022 19:33:17 GMT
EXPOSE 11211
# Tue, 24 May 2022 19:33:19 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:d3deabf2a506ef6f5fa7c2a68bf27047574cef9908b30a97ff2d01ae539b089a`  
		Last Modified: Mon, 23 May 2022 19:09:13 GMT  
		Size: 2.8 MB (2789745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b479cfab13a2f2ffe6bfc643d96b2ca17a80380353869913b72735725a953596`  
		Last Modified: Tue, 24 May 2022 19:34:20 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9111d00ba5c4381f0f8b185e1703815ef94004e492b01b0d3c7a7fe53acc977`  
		Last Modified: Tue, 24 May 2022 19:34:21 GMT  
		Size: 126.0 KB (126043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1a992983a73a33de517b221e813f6ddddea412212564e886bba2a9a09f82735`  
		Last Modified: Tue, 24 May 2022 19:34:21 GMT  
		Size: 974.3 KB (974333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6de2f26a895426d80205ef485568a93b91456d9913ce062578d21db1d228ef7`  
		Last Modified: Tue, 24 May 2022 19:34:20 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27f443297da5126d218f0cfd07deeb374b4db49ce895657aed034e4eba40ce1c`  
		Last Modified: Tue, 24 May 2022 19:34:20 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-alpine3.16` - linux; s390x

```console
$ docker pull memcached@sha256:79c15e8f5b25e585bc279ba8a2e990aaf1bcb0622e4b2cfe246b32381748232d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.6 MB (3629283 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3984c3293b24638ac012e61d1d83266b40194c43831d6d2f59fe1c01615baf07`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 23 May 2022 19:41:59 GMT
ADD file:e1852d8ef555a0d3ef6d0b74a898720c82bb9f491430b06a0dd0499497ce118e in / 
# Mon, 23 May 2022 19:42:10 GMT
CMD ["/bin/sh"]
# Tue, 24 May 2022 19:50:13 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 24 May 2022 19:50:14 GMT
RUN apk add --no-cache libsasl
# Tue, 24 May 2022 19:50:15 GMT
ENV MEMCACHED_VERSION=1.6.15
# Tue, 24 May 2022 19:50:15 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Tue, 24 May 2022 19:54:14 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 24 May 2022 19:54:15 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 24 May 2022 19:54:16 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 24 May 2022 19:54:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 24 May 2022 19:54:16 GMT
USER memcache
# Tue, 24 May 2022 19:54:16 GMT
EXPOSE 11211
# Tue, 24 May 2022 19:54:16 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:af1ac1a73384e058591d04d19bc05a06781cc32d52d4593b468d6cb95eda9858`  
		Last Modified: Mon, 23 May 2022 19:43:36 GMT  
		Size: 2.6 MB (2580494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0cdb25dad8a9e7c836addf0dfee4462f64217c81619f5c7519d620c59c68fff`  
		Last Modified: Tue, 24 May 2022 19:55:16 GMT  
		Size: 1.3 KB (1265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bfb96fb83213592db4a96cd8313433230d559f81caa115c56c8f9018d5e01f5`  
		Last Modified: Tue, 24 May 2022 19:55:16 GMT  
		Size: 112.5 KB (112500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fd8f0273e1af52c2d6bc2ea6e8f7c7b516ce039d78151fe854039d86e62db91`  
		Last Modified: Tue, 24 May 2022 19:55:17 GMT  
		Size: 934.6 KB (934620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a50bb84155cee8c93b5835daaee0a57b7c14397817ac75279b1ac51d2626f594`  
		Last Modified: Tue, 24 May 2022 19:55:16 GMT  
		Size: 283.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:196f82f950409b7b7c0e395502911ba3177047647ed8ac24e62c49dacf4eebf1`  
		Last Modified: Tue, 24 May 2022 19:55:17 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:1.6-bullseye`

```console
$ docker pull memcached@sha256:b422bca20902101cd4a427ccda5ea9729a89bdc6cd8ab8a7d8cd09b1470af6b6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; s390x

### `memcached:1.6-bullseye` - linux; amd64

```console
$ docker pull memcached@sha256:1be4a685ac5a327ffbd7d1c7240378e7156824f9406b1eeb5fe19eadc2e61c53
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.0 MB (32968544 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a23fd759590b790a7cae87582ba4d747378de71b47e581b9295c02ce34eb9ed0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 23 Jun 2022 00:20:27 GMT
ADD file:8adbbab04d6f84cd83b5f4205b89b0acb7ecbf27a1bb2dc181d0a629479039fe in / 
# Thu, 23 Jun 2022 00:20:27 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 04:18:20 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Thu, 23 Jun 2022 04:18:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 04:18:24 GMT
ENV MEMCACHED_VERSION=1.6.15
# Thu, 23 Jun 2022 04:18:24 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Thu, 23 Jun 2022 04:21:07 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 23 Jun 2022 04:21:07 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 23 Jun 2022 04:21:08 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 23 Jun 2022 04:21:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jun 2022 04:21:08 GMT
USER memcache
# Thu, 23 Jun 2022 04:21:08 GMT
EXPOSE 11211
# Thu, 23 Jun 2022 04:21:08 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:b85a868b505ffd0342a37e6a3b1c49f7c71878afe569a807e6238ef08252fcb7`  
		Last Modified: Thu, 23 Jun 2022 00:25:18 GMT  
		Size: 31.4 MB (31379408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f58bb523c8de07d0d72658b2e622e82f065a1adef45f6f90f11eb7c71b9d0c61`  
		Last Modified: Thu, 23 Jun 2022 04:21:33 GMT  
		Size: 5.0 KB (4979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a458d61c2cd35b8afffe3741b04321a87f86ba216e5e2a4f9429b83b32ceb35`  
		Last Modified: Thu, 23 Jun 2022 04:21:33 GMT  
		Size: 328.1 KB (328115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7eda168e1238eaa8f5c20b7240bb8bc84c9a3f7b4b8cdc0be18f58f27bff1692`  
		Last Modified: Thu, 23 Jun 2022 04:21:33 GMT  
		Size: 1.3 MB (1255633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f188c32090c0c66f2f209fedc0778269d3edf2ad9db239ac0d2e1e3b64b36fd4`  
		Last Modified: Thu, 23 Jun 2022 04:21:33 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f492776609f9ffcbe6d066f45223bc2da677c44beb7bb0cdc6dfa34271885b34`  
		Last Modified: Thu, 23 Jun 2022 04:21:33 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-bullseye` - linux; arm variant v5

```console
$ docker pull memcached@sha256:54ff97ee8133b4181bff0e30de243b68ffa4ad0a7ecc458e6648a24760c63213
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.5 MB (30470395 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:07faffc84c650af3ec2eb3326c593cd933cba137c34c87589a375371eee849f3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 23 Jun 2022 00:50:38 GMT
ADD file:839c0e211e2260f5d54f2633e53c817c1f59e2394ba4b12f60e01e46cee61011 in / 
# Thu, 23 Jun 2022 00:50:39 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 02:41:47 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Thu, 23 Jun 2022 02:41:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 02:41:58 GMT
ENV MEMCACHED_VERSION=1.6.15
# Thu, 23 Jun 2022 02:41:59 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Thu, 23 Jun 2022 02:46:28 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 23 Jun 2022 02:46:29 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 23 Jun 2022 02:46:31 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 23 Jun 2022 02:46:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jun 2022 02:46:32 GMT
USER memcache
# Thu, 23 Jun 2022 02:46:32 GMT
EXPOSE 11211
# Thu, 23 Jun 2022 02:46:33 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:bd2d3b4056bd1b0310082fc5d17c6d03348601456c4b9306d1a333f1cec561f9`  
		Last Modified: Thu, 23 Jun 2022 01:05:39 GMT  
		Size: 28.9 MB (28921550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f500bb51d193d56af19fbeb8ebc1919ec2e6d04cf9a7d1637ad79cc00397c1b`  
		Last Modified: Thu, 23 Jun 2022 02:47:27 GMT  
		Size: 4.9 KB (4894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c3dc6e5372afc0620e0eeae739b429bee70842f20a15ca8345787a674d5d3b8`  
		Last Modified: Thu, 23 Jun 2022 02:47:28 GMT  
		Size: 316.6 KB (316616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83d6f2e7e5c2a1d3566c4d9cd05fd132529535ba7eaecb00d312c0d0a6055a4c`  
		Last Modified: Thu, 23 Jun 2022 02:47:28 GMT  
		Size: 1.2 MB (1226926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:109349836a4d5f4431660fec9744df70f92475b22644182ae9d77c8c56c8960a`  
		Last Modified: Thu, 23 Jun 2022 02:47:27 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b87ddf1818c82326658f3ca6d444b01978e23d30a7232e4ef1e0f6f0ba4ab18`  
		Last Modified: Thu, 23 Jun 2022 02:47:27 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-bullseye` - linux; arm variant v7

```console
$ docker pull memcached@sha256:b3ddbe1e7ec04512ac9e20555b72ba4b2e7e9ee99138535fabe5e92cc92302b5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.1 MB (28092007 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cbbff85100ff53c710f4caa30445e0ee79ccd0fe61cc91a522821fc5415e6bcf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 23 Jun 2022 00:59:45 GMT
ADD file:925abfb9fc0e4a7cc0c979b12c9bd2607f5c493d37b05535ca010f81beb060a9 in / 
# Thu, 23 Jun 2022 00:59:46 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 22:08:47 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Thu, 23 Jun 2022 22:08:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 22:08:56 GMT
ENV MEMCACHED_VERSION=1.6.15
# Thu, 23 Jun 2022 22:08:56 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Thu, 23 Jun 2022 22:13:04 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 23 Jun 2022 22:13:05 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 23 Jun 2022 22:13:06 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 23 Jun 2022 22:13:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jun 2022 22:13:07 GMT
USER memcache
# Thu, 23 Jun 2022 22:13:08 GMT
EXPOSE 11211
# Thu, 23 Jun 2022 22:13:08 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:d2fd562560d8062a78064adfbfa204521167c301f00f5ab3c65b9c2a54083dba`  
		Last Modified: Thu, 23 Jun 2022 01:15:22 GMT  
		Size: 26.6 MB (26576105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8864d1bfbfd3f4b781316abd42de97a2967a6b20534ffdc4fea6a3de16c1d972`  
		Last Modified: Fri, 24 Jun 2022 01:14:10 GMT  
		Size: 4.9 KB (4897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fa7c6c177f3ba693baa86ed010daf821ca2addfe7f3b8a83c7f52fac209a6e8`  
		Last Modified: Fri, 24 Jun 2022 01:14:10 GMT  
		Size: 312.1 KB (312076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f802ee5fb123a2824f3e6f93144c74f9e1c88159fc819b46f7ed2913ec61281a`  
		Last Modified: Fri, 24 Jun 2022 01:14:11 GMT  
		Size: 1.2 MB (1198521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25b61f87cd4332b040dd59bae91f0701228904433b1955bb4f51b7377db17b00`  
		Last Modified: Fri, 24 Jun 2022 01:14:10 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:532462b4f12685e2093583f1e86c82d5c2c8069b92ccbc9bbcf8efad7dfd3252`  
		Last Modified: Fri, 24 Jun 2022 01:14:10 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-bullseye` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:536f8192668e851874eec7d483055b0af220a7eb0be43010f2f9825e99ab0111
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.4 MB (31444932 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2ce58160065ec196d51dcdc756610352a57f6192b28345989be83b94b8300dec`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 23 Jun 2022 00:40:43 GMT
ADD file:134be48af13f80f3474bf1b080ca781feb7b972148d482849862e55eb2acd61c in / 
# Thu, 23 Jun 2022 00:40:44 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 03:53:19 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Thu, 23 Jun 2022 03:53:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 03:53:24 GMT
ENV MEMCACHED_VERSION=1.6.15
# Thu, 23 Jun 2022 03:53:25 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Thu, 23 Jun 2022 03:56:00 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 23 Jun 2022 03:56:02 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 23 Jun 2022 03:56:02 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 23 Jun 2022 03:56:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jun 2022 03:56:04 GMT
USER memcache
# Thu, 23 Jun 2022 03:56:05 GMT
EXPOSE 11211
# Thu, 23 Jun 2022 03:56:06 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:3b157c852f2736e12f09046f214fe5f6a0b1652bd860269b3988c92a197026e8`  
		Last Modified: Thu, 23 Jun 2022 00:47:22 GMT  
		Size: 30.1 MB (30065720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee776bb67ffbc00ca5100c88e1f7ae63b580bc131c046c3c7138b7fb796683a2`  
		Last Modified: Thu, 23 Jun 2022 03:56:51 GMT  
		Size: 4.9 KB (4904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85b234170a3d54e3ad2be2993a7e7b09550a4e00327804a183e07bc786d01bc8`  
		Last Modified: Thu, 23 Jun 2022 03:56:51 GMT  
		Size: 119.2 KB (119223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a61e7150a45b8305adc14ed47f7beb3e807a7f08223393e6f5382b043b120941`  
		Last Modified: Thu, 23 Jun 2022 03:56:51 GMT  
		Size: 1.3 MB (1254677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ed6ad1685f73da9293938d389b8c24ee8b8af4d04d4c8b502cb6082d58bf349`  
		Last Modified: Thu, 23 Jun 2022 03:56:51 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:276672cde8876c99c646defdc630e9be5ae5cfb33c192102b6387ce99d151179`  
		Last Modified: Thu, 23 Jun 2022 03:56:51 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-bullseye` - linux; 386

```console
$ docker pull memcached@sha256:651e5275f0623232ecfa476f864b6634de4e9ffc6671376c796ffd70e31c83b6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.8 MB (33778463 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31252c746c529da361fcb075711def9645866db716700e15d9e4ce92e96ed3a0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 23 Jun 2022 00:39:33 GMT
ADD file:9d46d3f8fb63833a6dbd8dd796ad541d556046a48342d22e1fd3bffa3fb8e504 in / 
# Thu, 23 Jun 2022 00:39:33 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 03:32:31 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Thu, 23 Jun 2022 03:32:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 03:32:36 GMT
ENV MEMCACHED_VERSION=1.6.15
# Thu, 23 Jun 2022 03:32:37 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Thu, 23 Jun 2022 03:35:28 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 23 Jun 2022 03:35:30 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 23 Jun 2022 03:35:30 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 23 Jun 2022 03:35:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jun 2022 03:35:32 GMT
USER memcache
# Thu, 23 Jun 2022 03:35:33 GMT
EXPOSE 11211
# Thu, 23 Jun 2022 03:35:34 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:4870b12e407743816673c11cfb39974d80c1569d876287bef61f8c585954822f`  
		Last Modified: Thu, 23 Jun 2022 00:46:40 GMT  
		Size: 32.4 MB (32390198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a67b6581e800ff3e02f41dd18cb78bc620a25becd83769f84d2c61aed5d01ea`  
		Last Modified: Thu, 23 Jun 2022 03:36:21 GMT  
		Size: 4.8 KB (4773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b70025d0ac3fc2b23b2e76f6d96c607c6a04b53c9850fe3f14fa855827b9d19d`  
		Last Modified: Thu, 23 Jun 2022 03:36:21 GMT  
		Size: 130.1 KB (130137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a383a40e44984d67c847d2a4bbc7d3525f3867ff39c81a5221970dc744ee822e`  
		Last Modified: Thu, 23 Jun 2022 03:36:21 GMT  
		Size: 1.3 MB (1252947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24f731218f56e8a5f3d250c9a4e15f841afbd92a0ee71f88761feb880aa937b3`  
		Last Modified: Thu, 23 Jun 2022 03:36:21 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15ab75a8041fc16fdde22888eb35315059264f2c153e8d05d7f132d1aa413e3a`  
		Last Modified: Thu, 23 Jun 2022 03:36:21 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-bullseye` - linux; mips64le

```console
$ docker pull memcached@sha256:71ebcf40d19139f8bab5733065ff1b2599e5d52359c6f6cbfad2104be2f1fe33
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.0 MB (31014756 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d95105805101f850723625215940d8b2be96a9b40f984174eee903985becb9e0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 23 Jun 2022 01:10:25 GMT
ADD file:fd1174cc47ac636f0cab382578a899d69ed489e4dee53ec838955e36066f526a in / 
# Thu, 23 Jun 2022 01:10:29 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 03:13:46 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Thu, 23 Jun 2022 03:14:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 03:14:06 GMT
ENV MEMCACHED_VERSION=1.6.15
# Thu, 23 Jun 2022 03:14:08 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Thu, 23 Jun 2022 03:21:07 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 23 Jun 2022 03:21:09 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 23 Jun 2022 03:21:15 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 23 Jun 2022 03:21:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jun 2022 03:21:20 GMT
USER memcache
# Thu, 23 Jun 2022 03:21:22 GMT
EXPOSE 11211
# Thu, 23 Jun 2022 03:21:25 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:9d199cb5e183b38c9edcc527cbaaa79bb56da73bd09ed449223842775ef4a244`  
		Last Modified: Thu, 23 Jun 2022 01:20:19 GMT  
		Size: 29.6 MB (29641027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d188c3e3bf643b15e2e70cc10dab71da1f4e871305c84cf6d927a2750209ee47`  
		Last Modified: Thu, 23 Jun 2022 03:21:53 GMT  
		Size: 4.9 KB (4863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8855d5fcd2d728913f5ae40b13f074576721a44abf081e6bd4e8f48e8deb8262`  
		Last Modified: Thu, 23 Jun 2022 03:21:54 GMT  
		Size: 117.2 KB (117169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:726be3b42973c4aa79e2ffcecb3633c1ec825f8099da6b5d952810bf4d1827cd`  
		Last Modified: Thu, 23 Jun 2022 03:21:54 GMT  
		Size: 1.3 MB (1251289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6176796787c17dc9b41c47c10e23979540bb32e2833c3eeceb1456f0b228166f`  
		Last Modified: Thu, 23 Jun 2022 03:21:54 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:926c03f02a771007ddd9b4fd2172ff2d89647400c4370fdedb4533a5c99e42b1`  
		Last Modified: Thu, 23 Jun 2022 03:21:53 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-bullseye` - linux; ppc64le

```console
$ docker pull memcached@sha256:0bfecd8ca43abc3e50d162ce07d6794beb5d9f98ce929e9371c2542065e6c785
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.0 MB (36972124 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ac53be686814de607770ae7fba96134fc9cd4e5afe7444779b08c02a0c92a6c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 23 Jun 2022 02:02:32 GMT
ADD file:e18c13649ea1f145047652c8e171c4824f9b6b0dbc92127a914c7fca910acf96 in / 
# Thu, 23 Jun 2022 02:02:34 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 08:15:12 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Thu, 23 Jun 2022 08:15:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 08:15:26 GMT
ENV MEMCACHED_VERSION=1.6.15
# Thu, 23 Jun 2022 08:15:30 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Thu, 23 Jun 2022 08:20:21 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 23 Jun 2022 08:20:23 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 23 Jun 2022 08:20:29 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 23 Jun 2022 08:20:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jun 2022 08:20:34 GMT
USER memcache
# Thu, 23 Jun 2022 08:20:36 GMT
EXPOSE 11211
# Thu, 23 Jun 2022 08:20:38 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:7716f0df7ba06b6f1937cd664805984e25e386a4165f2c6acc65356686e35221`  
		Last Modified: Thu, 23 Jun 2022 02:15:20 GMT  
		Size: 35.3 MB (35286823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54d7d03c3543d8cc9dbdea919601e8b8bdebdf5f54f23ee2a186edde48a4025c`  
		Last Modified: Thu, 23 Jun 2022 08:21:29 GMT  
		Size: 5.0 KB (4987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa5efdc63c420d0295d4932cc7467f1a9005b4724f592c4fba99b6c801f57810`  
		Last Modified: Thu, 23 Jun 2022 08:21:29 GMT  
		Size: 357.0 KB (356958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:329e40de463f01938ecac1d284adb38a29fde479486e279cb302d95abe9f4a16`  
		Last Modified: Thu, 23 Jun 2022 08:21:29 GMT  
		Size: 1.3 MB (1322949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d823793235eacc3363db343cea0db041905e9fde59ff5262e0fd8826e962f5a`  
		Last Modified: Thu, 23 Jun 2022 08:21:29 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2ae46dbc3324ea97ee7556a1bc8006b075f7a1492e3a2114aaf8dec7c579b76`  
		Last Modified: Thu, 23 Jun 2022 08:21:29 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-bullseye` - linux; s390x

```console
$ docker pull memcached@sha256:1e49c15efaf9999b31f526130902a04a53eeac416f40d1549e98b3fa1a872c04
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.2 MB (31226391 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b8090a3ed64f97313e1ddce878717e3bf8c1aace9d7bf247a1fa53418081f0c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 23 Jun 2022 00:43:10 GMT
ADD file:0b511e3efd87267fb27161eae56c4d08f0fed733697da6ffe6ea96a4cb68e938 in / 
# Thu, 23 Jun 2022 00:43:15 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 13:41:46 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Thu, 23 Jun 2022 13:41:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 13:41:49 GMT
ENV MEMCACHED_VERSION=1.6.15
# Thu, 23 Jun 2022 13:41:50 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Thu, 23 Jun 2022 13:45:09 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 23 Jun 2022 13:45:09 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 23 Jun 2022 13:45:10 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 23 Jun 2022 13:45:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jun 2022 13:45:10 GMT
USER memcache
# Thu, 23 Jun 2022 13:45:10 GMT
EXPOSE 11211
# Thu, 23 Jun 2022 13:45:10 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:c547f465e0c8708ad0c57cf09caa52f4c2b5b295bf10ab1ce71ca17ff81ea36a`  
		Last Modified: Thu, 23 Jun 2022 00:51:59 GMT  
		Size: 29.7 MB (29655262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04837776e7fbb579dda3720caca85ff9cb19eea15a8830ab0f23a160fa832205`  
		Last Modified: Thu, 23 Jun 2022 13:46:03 GMT  
		Size: 5.0 KB (5025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d844915fd9a66accf5106919c6a63121ed4fde412dcf958133bc1b1483b307b`  
		Last Modified: Thu, 23 Jun 2022 13:46:03 GMT  
		Size: 324.2 KB (324209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51abf5cd3f179d43b5845c7dc42a6f07ddfd6da706ca58f78d53641e3d62289f`  
		Last Modified: Thu, 23 Jun 2022 13:46:03 GMT  
		Size: 1.2 MB (1241485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31ea51fd993089ad7346961b0897d009e18b953416139bf4359ff089b9e9ada9`  
		Last Modified: Thu, 23 Jun 2022 13:46:04 GMT  
		Size: 289.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cda18e1b304fdde7d799586641bad45a035387c02b0c7e8d696e91221b046e28`  
		Last Modified: Thu, 23 Jun 2022 13:46:03 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:1.6.15`

```console
$ docker pull memcached@sha256:b422bca20902101cd4a427ccda5ea9729a89bdc6cd8ab8a7d8cd09b1470af6b6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; s390x

### `memcached:1.6.15` - linux; amd64

```console
$ docker pull memcached@sha256:1be4a685ac5a327ffbd7d1c7240378e7156824f9406b1eeb5fe19eadc2e61c53
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.0 MB (32968544 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a23fd759590b790a7cae87582ba4d747378de71b47e581b9295c02ce34eb9ed0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 23 Jun 2022 00:20:27 GMT
ADD file:8adbbab04d6f84cd83b5f4205b89b0acb7ecbf27a1bb2dc181d0a629479039fe in / 
# Thu, 23 Jun 2022 00:20:27 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 04:18:20 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Thu, 23 Jun 2022 04:18:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 04:18:24 GMT
ENV MEMCACHED_VERSION=1.6.15
# Thu, 23 Jun 2022 04:18:24 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Thu, 23 Jun 2022 04:21:07 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 23 Jun 2022 04:21:07 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 23 Jun 2022 04:21:08 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 23 Jun 2022 04:21:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jun 2022 04:21:08 GMT
USER memcache
# Thu, 23 Jun 2022 04:21:08 GMT
EXPOSE 11211
# Thu, 23 Jun 2022 04:21:08 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:b85a868b505ffd0342a37e6a3b1c49f7c71878afe569a807e6238ef08252fcb7`  
		Last Modified: Thu, 23 Jun 2022 00:25:18 GMT  
		Size: 31.4 MB (31379408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f58bb523c8de07d0d72658b2e622e82f065a1adef45f6f90f11eb7c71b9d0c61`  
		Last Modified: Thu, 23 Jun 2022 04:21:33 GMT  
		Size: 5.0 KB (4979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a458d61c2cd35b8afffe3741b04321a87f86ba216e5e2a4f9429b83b32ceb35`  
		Last Modified: Thu, 23 Jun 2022 04:21:33 GMT  
		Size: 328.1 KB (328115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7eda168e1238eaa8f5c20b7240bb8bc84c9a3f7b4b8cdc0be18f58f27bff1692`  
		Last Modified: Thu, 23 Jun 2022 04:21:33 GMT  
		Size: 1.3 MB (1255633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f188c32090c0c66f2f209fedc0778269d3edf2ad9db239ac0d2e1e3b64b36fd4`  
		Last Modified: Thu, 23 Jun 2022 04:21:33 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f492776609f9ffcbe6d066f45223bc2da677c44beb7bb0cdc6dfa34271885b34`  
		Last Modified: Thu, 23 Jun 2022 04:21:33 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.15` - linux; arm variant v5

```console
$ docker pull memcached@sha256:54ff97ee8133b4181bff0e30de243b68ffa4ad0a7ecc458e6648a24760c63213
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.5 MB (30470395 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:07faffc84c650af3ec2eb3326c593cd933cba137c34c87589a375371eee849f3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 23 Jun 2022 00:50:38 GMT
ADD file:839c0e211e2260f5d54f2633e53c817c1f59e2394ba4b12f60e01e46cee61011 in / 
# Thu, 23 Jun 2022 00:50:39 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 02:41:47 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Thu, 23 Jun 2022 02:41:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 02:41:58 GMT
ENV MEMCACHED_VERSION=1.6.15
# Thu, 23 Jun 2022 02:41:59 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Thu, 23 Jun 2022 02:46:28 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 23 Jun 2022 02:46:29 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 23 Jun 2022 02:46:31 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 23 Jun 2022 02:46:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jun 2022 02:46:32 GMT
USER memcache
# Thu, 23 Jun 2022 02:46:32 GMT
EXPOSE 11211
# Thu, 23 Jun 2022 02:46:33 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:bd2d3b4056bd1b0310082fc5d17c6d03348601456c4b9306d1a333f1cec561f9`  
		Last Modified: Thu, 23 Jun 2022 01:05:39 GMT  
		Size: 28.9 MB (28921550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f500bb51d193d56af19fbeb8ebc1919ec2e6d04cf9a7d1637ad79cc00397c1b`  
		Last Modified: Thu, 23 Jun 2022 02:47:27 GMT  
		Size: 4.9 KB (4894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c3dc6e5372afc0620e0eeae739b429bee70842f20a15ca8345787a674d5d3b8`  
		Last Modified: Thu, 23 Jun 2022 02:47:28 GMT  
		Size: 316.6 KB (316616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83d6f2e7e5c2a1d3566c4d9cd05fd132529535ba7eaecb00d312c0d0a6055a4c`  
		Last Modified: Thu, 23 Jun 2022 02:47:28 GMT  
		Size: 1.2 MB (1226926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:109349836a4d5f4431660fec9744df70f92475b22644182ae9d77c8c56c8960a`  
		Last Modified: Thu, 23 Jun 2022 02:47:27 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b87ddf1818c82326658f3ca6d444b01978e23d30a7232e4ef1e0f6f0ba4ab18`  
		Last Modified: Thu, 23 Jun 2022 02:47:27 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.15` - linux; arm variant v7

```console
$ docker pull memcached@sha256:b3ddbe1e7ec04512ac9e20555b72ba4b2e7e9ee99138535fabe5e92cc92302b5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.1 MB (28092007 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cbbff85100ff53c710f4caa30445e0ee79ccd0fe61cc91a522821fc5415e6bcf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 23 Jun 2022 00:59:45 GMT
ADD file:925abfb9fc0e4a7cc0c979b12c9bd2607f5c493d37b05535ca010f81beb060a9 in / 
# Thu, 23 Jun 2022 00:59:46 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 22:08:47 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Thu, 23 Jun 2022 22:08:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 22:08:56 GMT
ENV MEMCACHED_VERSION=1.6.15
# Thu, 23 Jun 2022 22:08:56 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Thu, 23 Jun 2022 22:13:04 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 23 Jun 2022 22:13:05 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 23 Jun 2022 22:13:06 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 23 Jun 2022 22:13:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jun 2022 22:13:07 GMT
USER memcache
# Thu, 23 Jun 2022 22:13:08 GMT
EXPOSE 11211
# Thu, 23 Jun 2022 22:13:08 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:d2fd562560d8062a78064adfbfa204521167c301f00f5ab3c65b9c2a54083dba`  
		Last Modified: Thu, 23 Jun 2022 01:15:22 GMT  
		Size: 26.6 MB (26576105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8864d1bfbfd3f4b781316abd42de97a2967a6b20534ffdc4fea6a3de16c1d972`  
		Last Modified: Fri, 24 Jun 2022 01:14:10 GMT  
		Size: 4.9 KB (4897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fa7c6c177f3ba693baa86ed010daf821ca2addfe7f3b8a83c7f52fac209a6e8`  
		Last Modified: Fri, 24 Jun 2022 01:14:10 GMT  
		Size: 312.1 KB (312076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f802ee5fb123a2824f3e6f93144c74f9e1c88159fc819b46f7ed2913ec61281a`  
		Last Modified: Fri, 24 Jun 2022 01:14:11 GMT  
		Size: 1.2 MB (1198521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25b61f87cd4332b040dd59bae91f0701228904433b1955bb4f51b7377db17b00`  
		Last Modified: Fri, 24 Jun 2022 01:14:10 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:532462b4f12685e2093583f1e86c82d5c2c8069b92ccbc9bbcf8efad7dfd3252`  
		Last Modified: Fri, 24 Jun 2022 01:14:10 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.15` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:536f8192668e851874eec7d483055b0af220a7eb0be43010f2f9825e99ab0111
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.4 MB (31444932 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2ce58160065ec196d51dcdc756610352a57f6192b28345989be83b94b8300dec`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 23 Jun 2022 00:40:43 GMT
ADD file:134be48af13f80f3474bf1b080ca781feb7b972148d482849862e55eb2acd61c in / 
# Thu, 23 Jun 2022 00:40:44 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 03:53:19 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Thu, 23 Jun 2022 03:53:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 03:53:24 GMT
ENV MEMCACHED_VERSION=1.6.15
# Thu, 23 Jun 2022 03:53:25 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Thu, 23 Jun 2022 03:56:00 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 23 Jun 2022 03:56:02 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 23 Jun 2022 03:56:02 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 23 Jun 2022 03:56:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jun 2022 03:56:04 GMT
USER memcache
# Thu, 23 Jun 2022 03:56:05 GMT
EXPOSE 11211
# Thu, 23 Jun 2022 03:56:06 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:3b157c852f2736e12f09046f214fe5f6a0b1652bd860269b3988c92a197026e8`  
		Last Modified: Thu, 23 Jun 2022 00:47:22 GMT  
		Size: 30.1 MB (30065720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee776bb67ffbc00ca5100c88e1f7ae63b580bc131c046c3c7138b7fb796683a2`  
		Last Modified: Thu, 23 Jun 2022 03:56:51 GMT  
		Size: 4.9 KB (4904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85b234170a3d54e3ad2be2993a7e7b09550a4e00327804a183e07bc786d01bc8`  
		Last Modified: Thu, 23 Jun 2022 03:56:51 GMT  
		Size: 119.2 KB (119223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a61e7150a45b8305adc14ed47f7beb3e807a7f08223393e6f5382b043b120941`  
		Last Modified: Thu, 23 Jun 2022 03:56:51 GMT  
		Size: 1.3 MB (1254677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ed6ad1685f73da9293938d389b8c24ee8b8af4d04d4c8b502cb6082d58bf349`  
		Last Modified: Thu, 23 Jun 2022 03:56:51 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:276672cde8876c99c646defdc630e9be5ae5cfb33c192102b6387ce99d151179`  
		Last Modified: Thu, 23 Jun 2022 03:56:51 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.15` - linux; 386

```console
$ docker pull memcached@sha256:651e5275f0623232ecfa476f864b6634de4e9ffc6671376c796ffd70e31c83b6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.8 MB (33778463 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31252c746c529da361fcb075711def9645866db716700e15d9e4ce92e96ed3a0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 23 Jun 2022 00:39:33 GMT
ADD file:9d46d3f8fb63833a6dbd8dd796ad541d556046a48342d22e1fd3bffa3fb8e504 in / 
# Thu, 23 Jun 2022 00:39:33 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 03:32:31 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Thu, 23 Jun 2022 03:32:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 03:32:36 GMT
ENV MEMCACHED_VERSION=1.6.15
# Thu, 23 Jun 2022 03:32:37 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Thu, 23 Jun 2022 03:35:28 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 23 Jun 2022 03:35:30 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 23 Jun 2022 03:35:30 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 23 Jun 2022 03:35:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jun 2022 03:35:32 GMT
USER memcache
# Thu, 23 Jun 2022 03:35:33 GMT
EXPOSE 11211
# Thu, 23 Jun 2022 03:35:34 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:4870b12e407743816673c11cfb39974d80c1569d876287bef61f8c585954822f`  
		Last Modified: Thu, 23 Jun 2022 00:46:40 GMT  
		Size: 32.4 MB (32390198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a67b6581e800ff3e02f41dd18cb78bc620a25becd83769f84d2c61aed5d01ea`  
		Last Modified: Thu, 23 Jun 2022 03:36:21 GMT  
		Size: 4.8 KB (4773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b70025d0ac3fc2b23b2e76f6d96c607c6a04b53c9850fe3f14fa855827b9d19d`  
		Last Modified: Thu, 23 Jun 2022 03:36:21 GMT  
		Size: 130.1 KB (130137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a383a40e44984d67c847d2a4bbc7d3525f3867ff39c81a5221970dc744ee822e`  
		Last Modified: Thu, 23 Jun 2022 03:36:21 GMT  
		Size: 1.3 MB (1252947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24f731218f56e8a5f3d250c9a4e15f841afbd92a0ee71f88761feb880aa937b3`  
		Last Modified: Thu, 23 Jun 2022 03:36:21 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15ab75a8041fc16fdde22888eb35315059264f2c153e8d05d7f132d1aa413e3a`  
		Last Modified: Thu, 23 Jun 2022 03:36:21 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.15` - linux; mips64le

```console
$ docker pull memcached@sha256:71ebcf40d19139f8bab5733065ff1b2599e5d52359c6f6cbfad2104be2f1fe33
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.0 MB (31014756 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d95105805101f850723625215940d8b2be96a9b40f984174eee903985becb9e0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 23 Jun 2022 01:10:25 GMT
ADD file:fd1174cc47ac636f0cab382578a899d69ed489e4dee53ec838955e36066f526a in / 
# Thu, 23 Jun 2022 01:10:29 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 03:13:46 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Thu, 23 Jun 2022 03:14:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 03:14:06 GMT
ENV MEMCACHED_VERSION=1.6.15
# Thu, 23 Jun 2022 03:14:08 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Thu, 23 Jun 2022 03:21:07 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 23 Jun 2022 03:21:09 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 23 Jun 2022 03:21:15 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 23 Jun 2022 03:21:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jun 2022 03:21:20 GMT
USER memcache
# Thu, 23 Jun 2022 03:21:22 GMT
EXPOSE 11211
# Thu, 23 Jun 2022 03:21:25 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:9d199cb5e183b38c9edcc527cbaaa79bb56da73bd09ed449223842775ef4a244`  
		Last Modified: Thu, 23 Jun 2022 01:20:19 GMT  
		Size: 29.6 MB (29641027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d188c3e3bf643b15e2e70cc10dab71da1f4e871305c84cf6d927a2750209ee47`  
		Last Modified: Thu, 23 Jun 2022 03:21:53 GMT  
		Size: 4.9 KB (4863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8855d5fcd2d728913f5ae40b13f074576721a44abf081e6bd4e8f48e8deb8262`  
		Last Modified: Thu, 23 Jun 2022 03:21:54 GMT  
		Size: 117.2 KB (117169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:726be3b42973c4aa79e2ffcecb3633c1ec825f8099da6b5d952810bf4d1827cd`  
		Last Modified: Thu, 23 Jun 2022 03:21:54 GMT  
		Size: 1.3 MB (1251289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6176796787c17dc9b41c47c10e23979540bb32e2833c3eeceb1456f0b228166f`  
		Last Modified: Thu, 23 Jun 2022 03:21:54 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:926c03f02a771007ddd9b4fd2172ff2d89647400c4370fdedb4533a5c99e42b1`  
		Last Modified: Thu, 23 Jun 2022 03:21:53 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.15` - linux; ppc64le

```console
$ docker pull memcached@sha256:0bfecd8ca43abc3e50d162ce07d6794beb5d9f98ce929e9371c2542065e6c785
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.0 MB (36972124 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ac53be686814de607770ae7fba96134fc9cd4e5afe7444779b08c02a0c92a6c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 23 Jun 2022 02:02:32 GMT
ADD file:e18c13649ea1f145047652c8e171c4824f9b6b0dbc92127a914c7fca910acf96 in / 
# Thu, 23 Jun 2022 02:02:34 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 08:15:12 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Thu, 23 Jun 2022 08:15:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 08:15:26 GMT
ENV MEMCACHED_VERSION=1.6.15
# Thu, 23 Jun 2022 08:15:30 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Thu, 23 Jun 2022 08:20:21 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 23 Jun 2022 08:20:23 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 23 Jun 2022 08:20:29 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 23 Jun 2022 08:20:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jun 2022 08:20:34 GMT
USER memcache
# Thu, 23 Jun 2022 08:20:36 GMT
EXPOSE 11211
# Thu, 23 Jun 2022 08:20:38 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:7716f0df7ba06b6f1937cd664805984e25e386a4165f2c6acc65356686e35221`  
		Last Modified: Thu, 23 Jun 2022 02:15:20 GMT  
		Size: 35.3 MB (35286823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54d7d03c3543d8cc9dbdea919601e8b8bdebdf5f54f23ee2a186edde48a4025c`  
		Last Modified: Thu, 23 Jun 2022 08:21:29 GMT  
		Size: 5.0 KB (4987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa5efdc63c420d0295d4932cc7467f1a9005b4724f592c4fba99b6c801f57810`  
		Last Modified: Thu, 23 Jun 2022 08:21:29 GMT  
		Size: 357.0 KB (356958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:329e40de463f01938ecac1d284adb38a29fde479486e279cb302d95abe9f4a16`  
		Last Modified: Thu, 23 Jun 2022 08:21:29 GMT  
		Size: 1.3 MB (1322949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d823793235eacc3363db343cea0db041905e9fde59ff5262e0fd8826e962f5a`  
		Last Modified: Thu, 23 Jun 2022 08:21:29 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2ae46dbc3324ea97ee7556a1bc8006b075f7a1492e3a2114aaf8dec7c579b76`  
		Last Modified: Thu, 23 Jun 2022 08:21:29 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.15` - linux; s390x

```console
$ docker pull memcached@sha256:1e49c15efaf9999b31f526130902a04a53eeac416f40d1549e98b3fa1a872c04
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.2 MB (31226391 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b8090a3ed64f97313e1ddce878717e3bf8c1aace9d7bf247a1fa53418081f0c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 23 Jun 2022 00:43:10 GMT
ADD file:0b511e3efd87267fb27161eae56c4d08f0fed733697da6ffe6ea96a4cb68e938 in / 
# Thu, 23 Jun 2022 00:43:15 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 13:41:46 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Thu, 23 Jun 2022 13:41:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 13:41:49 GMT
ENV MEMCACHED_VERSION=1.6.15
# Thu, 23 Jun 2022 13:41:50 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Thu, 23 Jun 2022 13:45:09 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 23 Jun 2022 13:45:09 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 23 Jun 2022 13:45:10 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 23 Jun 2022 13:45:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jun 2022 13:45:10 GMT
USER memcache
# Thu, 23 Jun 2022 13:45:10 GMT
EXPOSE 11211
# Thu, 23 Jun 2022 13:45:10 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:c547f465e0c8708ad0c57cf09caa52f4c2b5b295bf10ab1ce71ca17ff81ea36a`  
		Last Modified: Thu, 23 Jun 2022 00:51:59 GMT  
		Size: 29.7 MB (29655262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04837776e7fbb579dda3720caca85ff9cb19eea15a8830ab0f23a160fa832205`  
		Last Modified: Thu, 23 Jun 2022 13:46:03 GMT  
		Size: 5.0 KB (5025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d844915fd9a66accf5106919c6a63121ed4fde412dcf958133bc1b1483b307b`  
		Last Modified: Thu, 23 Jun 2022 13:46:03 GMT  
		Size: 324.2 KB (324209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51abf5cd3f179d43b5845c7dc42a6f07ddfd6da706ca58f78d53641e3d62289f`  
		Last Modified: Thu, 23 Jun 2022 13:46:03 GMT  
		Size: 1.2 MB (1241485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31ea51fd993089ad7346961b0897d009e18b953416139bf4359ff089b9e9ada9`  
		Last Modified: Thu, 23 Jun 2022 13:46:04 GMT  
		Size: 289.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cda18e1b304fdde7d799586641bad45a035387c02b0c7e8d696e91221b046e28`  
		Last Modified: Thu, 23 Jun 2022 13:46:03 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:1.6.15-alpine`

```console
$ docker pull memcached@sha256:bab32a8a61543525190db12c2a518c3c2331656a4409185f0f4f33a506e3aae7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `memcached:1.6.15-alpine` - linux; amd64

```console
$ docker pull memcached@sha256:bae66da0e8cdb7daa226cc0837e2562404a4007466044ffdfa88a8a0431d5c7a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3853361 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e3f5d6e8d61d2ec54ff3d21da1c6dbddca8f0018c8f1c1253287129fa3926d7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 23 May 2022 19:19:30 GMT
ADD file:8e81116368669ed3dd361bc898d61bff249f524139a239fdaf3ec46869a39921 in / 
# Mon, 23 May 2022 19:19:31 GMT
CMD ["/bin/sh"]
# Tue, 24 May 2022 19:24:21 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 24 May 2022 19:24:23 GMT
RUN apk add --no-cache libsasl
# Tue, 24 May 2022 19:24:23 GMT
ENV MEMCACHED_VERSION=1.6.15
# Tue, 24 May 2022 19:24:23 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Tue, 24 May 2022 19:27:18 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 24 May 2022 19:27:18 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 24 May 2022 19:27:19 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 24 May 2022 19:27:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 24 May 2022 19:27:19 GMT
USER memcache
# Tue, 24 May 2022 19:27:19 GMT
EXPOSE 11211
# Tue, 24 May 2022 19:27:19 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:2408cc74d12b6cd092bb8b516ba7d5e290f485d3eb9672efc00f0583730179e8`  
		Last Modified: Mon, 23 May 2022 19:09:38 GMT  
		Size: 2.8 MB (2798889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6da329a3b4330a0705bfb49b5e6ce2fb61bc108d0a32d41c2c0dad6d9dd6c8fa`  
		Last Modified: Tue, 24 May 2022 19:27:48 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f4ba002bd64c19ecd49e1afc372709c9bcfb3dbe2b9ee2b02d43dea8fddc3cc`  
		Last Modified: Tue, 24 May 2022 19:27:48 GMT  
		Size: 108.3 KB (108307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d664dde428a76ca57c1261382f6f9b758a3b5b0e12b51f6a5b1a38bef237456a`  
		Last Modified: Tue, 24 May 2022 19:27:48 GMT  
		Size: 944.5 KB (944489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef11efc606151d8228ae06848232d8d65ae50082bf0ad5c5104d06c27ce7c85d`  
		Last Modified: Tue, 24 May 2022 19:27:48 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f118f0edbe76d09a02e63a4712d1b9b3eb1ebce2a271c740baba58cc48df9f4e`  
		Last Modified: Tue, 24 May 2022 19:27:48 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.15-alpine` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:8ec1f6a98e264e73e3c7b2feba04b272ce1522adc9d40118b9684721c41122b0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.7 MB (3737167 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f393a4888061e0456042ebb89fbc11cf72af15c189e0d0e4ee62b7fcfd44c683`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 23 May 2022 19:39:22 GMT
ADD file:3ae36c6c4a1fc43157692da97c6c4fa6c3d0189ba82e2bef7f5aaf4a5e083f18 in / 
# Mon, 23 May 2022 19:39:22 GMT
CMD ["/bin/sh"]
# Tue, 24 May 2022 20:08:53 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 24 May 2022 20:08:55 GMT
RUN apk add --no-cache libsasl
# Tue, 24 May 2022 20:08:56 GMT
ENV MEMCACHED_VERSION=1.6.15
# Tue, 24 May 2022 20:08:57 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Tue, 24 May 2022 20:12:06 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 24 May 2022 20:12:08 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 24 May 2022 20:12:08 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 24 May 2022 20:12:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 24 May 2022 20:12:10 GMT
USER memcache
# Tue, 24 May 2022 20:12:11 GMT
EXPOSE 11211
# Tue, 24 May 2022 20:12:12 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:b3c136eddcbf2003d3180787cef00f39d46b9fd9e4623178282ad6a8d63ad3b0`  
		Last Modified: Mon, 23 May 2022 19:08:34 GMT  
		Size: 2.7 MB (2694464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e87d2d7a8c9bc1317afe928c225caaafd86b3b73a2bc359f8037eb0f501b394c`  
		Last Modified: Tue, 24 May 2022 20:12:58 GMT  
		Size: 1.2 KB (1242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55dbcde2059d799697807a93b36d71cd601b20e2218abb7cb9261d22e8a7d67a`  
		Last Modified: Tue, 24 May 2022 20:12:58 GMT  
		Size: 109.6 KB (109557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4aa3db0ac20b8381c09df00576661af3c209195453eeeb892b8532059b932a39`  
		Last Modified: Tue, 24 May 2022 20:12:59 GMT  
		Size: 931.5 KB (931496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d999e908ec416e199da213e6fca67cdc82d3d440098a1bfbc5bc7c5a2f35636`  
		Last Modified: Tue, 24 May 2022 20:12:58 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8017baa48e45fa47c2fab6975dcd0ab8a560c64c0de05f7113831a537b385a3b`  
		Last Modified: Tue, 24 May 2022 20:12:58 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.15-alpine` - linux; 386

```console
$ docker pull memcached@sha256:3560af36f0aaeb7e4d2da47f0ad4a91bc675aa017423f34911490b09908230e8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3878370 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7d5a231eedb6e0b20291a77ac7a71c5a16aca1a9eb62893e285cefa1b95bdf5b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 23 May 2022 19:38:20 GMT
ADD file:1750ccfabfe93636015070d51a6e824cbd738056223421c69d8aaabc38041b18 in / 
# Mon, 23 May 2022 19:38:20 GMT
CMD ["/bin/sh"]
# Tue, 24 May 2022 19:46:24 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 24 May 2022 19:46:26 GMT
RUN apk add --no-cache libsasl
# Tue, 24 May 2022 19:46:26 GMT
ENV MEMCACHED_VERSION=1.6.15
# Tue, 24 May 2022 19:46:27 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Tue, 24 May 2022 19:49:17 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 24 May 2022 19:49:19 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 24 May 2022 19:49:19 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 24 May 2022 19:49:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 24 May 2022 19:49:21 GMT
USER memcache
# Tue, 24 May 2022 19:49:22 GMT
EXPOSE 11211
# Tue, 24 May 2022 19:49:23 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:bb638a3869eed698f88775c7a48f36f8e22e7c6bbaa98fa1d5678966b619b859`  
		Last Modified: Mon, 23 May 2022 19:09:25 GMT  
		Size: 2.8 MB (2801887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d301e0dbe5a2594f09f110ec3c1e79f4bd885af78b4992bf8af7a9f7b0507d5a`  
		Last Modified: Tue, 24 May 2022 19:50:14 GMT  
		Size: 1.2 KB (1242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:880ddc23b9c3165a8e86c64a648782c63c9a7271e84df6ac2f5a8c110d32258d`  
		Last Modified: Tue, 24 May 2022 19:50:14 GMT  
		Size: 119.8 KB (119821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c60884a7874466d1525bb0560fcbbbc226cfb4fb1507f1bd0d45d4f1b0e1307b`  
		Last Modified: Tue, 24 May 2022 19:50:15 GMT  
		Size: 955.0 KB (955017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89ad9c1959a10762028a884c1a33f06bb71bcb1a9ac372c889304f75f2a4b597`  
		Last Modified: Tue, 24 May 2022 19:50:14 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b267a8907abfcf28b9d96b17379ce57985989f17d34c06dfd238aee8ed0da61`  
		Last Modified: Tue, 24 May 2022 19:50:14 GMT  
		Size: 119.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.15-alpine` - linux; ppc64le

```console
$ docker pull memcached@sha256:edeccd4ca90cecc053bd78239bef1a1ccec0d2f189655d39e29e44216157fec4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3891798 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:348c555fa9d4bcfd44f2f7426151f1666fd08a28ce9fea73c503bc207229c503`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 23 May 2022 19:16:51 GMT
ADD file:6a5450c8a7cee3ceda59e7cb350c54df4139b0f7b7cf49c8b31bb9c01646c3cd in / 
# Mon, 23 May 2022 19:16:53 GMT
CMD ["/bin/sh"]
# Tue, 24 May 2022 19:29:15 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 24 May 2022 19:29:23 GMT
RUN apk add --no-cache libsasl
# Tue, 24 May 2022 19:29:30 GMT
ENV MEMCACHED_VERSION=1.6.15
# Tue, 24 May 2022 19:29:36 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Tue, 24 May 2022 19:33:02 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 24 May 2022 19:33:03 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 24 May 2022 19:33:08 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 24 May 2022 19:33:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 24 May 2022 19:33:14 GMT
USER memcache
# Tue, 24 May 2022 19:33:17 GMT
EXPOSE 11211
# Tue, 24 May 2022 19:33:19 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:d3deabf2a506ef6f5fa7c2a68bf27047574cef9908b30a97ff2d01ae539b089a`  
		Last Modified: Mon, 23 May 2022 19:09:13 GMT  
		Size: 2.8 MB (2789745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b479cfab13a2f2ffe6bfc643d96b2ca17a80380353869913b72735725a953596`  
		Last Modified: Tue, 24 May 2022 19:34:20 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9111d00ba5c4381f0f8b185e1703815ef94004e492b01b0d3c7a7fe53acc977`  
		Last Modified: Tue, 24 May 2022 19:34:21 GMT  
		Size: 126.0 KB (126043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1a992983a73a33de517b221e813f6ddddea412212564e886bba2a9a09f82735`  
		Last Modified: Tue, 24 May 2022 19:34:21 GMT  
		Size: 974.3 KB (974333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6de2f26a895426d80205ef485568a93b91456d9913ce062578d21db1d228ef7`  
		Last Modified: Tue, 24 May 2022 19:34:20 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27f443297da5126d218f0cfd07deeb374b4db49ce895657aed034e4eba40ce1c`  
		Last Modified: Tue, 24 May 2022 19:34:20 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.15-alpine` - linux; s390x

```console
$ docker pull memcached@sha256:79c15e8f5b25e585bc279ba8a2e990aaf1bcb0622e4b2cfe246b32381748232d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.6 MB (3629283 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3984c3293b24638ac012e61d1d83266b40194c43831d6d2f59fe1c01615baf07`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 23 May 2022 19:41:59 GMT
ADD file:e1852d8ef555a0d3ef6d0b74a898720c82bb9f491430b06a0dd0499497ce118e in / 
# Mon, 23 May 2022 19:42:10 GMT
CMD ["/bin/sh"]
# Tue, 24 May 2022 19:50:13 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 24 May 2022 19:50:14 GMT
RUN apk add --no-cache libsasl
# Tue, 24 May 2022 19:50:15 GMT
ENV MEMCACHED_VERSION=1.6.15
# Tue, 24 May 2022 19:50:15 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Tue, 24 May 2022 19:54:14 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 24 May 2022 19:54:15 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 24 May 2022 19:54:16 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 24 May 2022 19:54:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 24 May 2022 19:54:16 GMT
USER memcache
# Tue, 24 May 2022 19:54:16 GMT
EXPOSE 11211
# Tue, 24 May 2022 19:54:16 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:af1ac1a73384e058591d04d19bc05a06781cc32d52d4593b468d6cb95eda9858`  
		Last Modified: Mon, 23 May 2022 19:43:36 GMT  
		Size: 2.6 MB (2580494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0cdb25dad8a9e7c836addf0dfee4462f64217c81619f5c7519d620c59c68fff`  
		Last Modified: Tue, 24 May 2022 19:55:16 GMT  
		Size: 1.3 KB (1265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bfb96fb83213592db4a96cd8313433230d559f81caa115c56c8f9018d5e01f5`  
		Last Modified: Tue, 24 May 2022 19:55:16 GMT  
		Size: 112.5 KB (112500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fd8f0273e1af52c2d6bc2ea6e8f7c7b516ce039d78151fe854039d86e62db91`  
		Last Modified: Tue, 24 May 2022 19:55:17 GMT  
		Size: 934.6 KB (934620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a50bb84155cee8c93b5835daaee0a57b7c14397817ac75279b1ac51d2626f594`  
		Last Modified: Tue, 24 May 2022 19:55:16 GMT  
		Size: 283.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:196f82f950409b7b7c0e395502911ba3177047647ed8ac24e62c49dacf4eebf1`  
		Last Modified: Tue, 24 May 2022 19:55:17 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:1.6.15-alpine3.16`

```console
$ docker pull memcached@sha256:bab32a8a61543525190db12c2a518c3c2331656a4409185f0f4f33a506e3aae7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `memcached:1.6.15-alpine3.16` - linux; amd64

```console
$ docker pull memcached@sha256:bae66da0e8cdb7daa226cc0837e2562404a4007466044ffdfa88a8a0431d5c7a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3853361 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e3f5d6e8d61d2ec54ff3d21da1c6dbddca8f0018c8f1c1253287129fa3926d7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 23 May 2022 19:19:30 GMT
ADD file:8e81116368669ed3dd361bc898d61bff249f524139a239fdaf3ec46869a39921 in / 
# Mon, 23 May 2022 19:19:31 GMT
CMD ["/bin/sh"]
# Tue, 24 May 2022 19:24:21 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 24 May 2022 19:24:23 GMT
RUN apk add --no-cache libsasl
# Tue, 24 May 2022 19:24:23 GMT
ENV MEMCACHED_VERSION=1.6.15
# Tue, 24 May 2022 19:24:23 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Tue, 24 May 2022 19:27:18 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 24 May 2022 19:27:18 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 24 May 2022 19:27:19 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 24 May 2022 19:27:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 24 May 2022 19:27:19 GMT
USER memcache
# Tue, 24 May 2022 19:27:19 GMT
EXPOSE 11211
# Tue, 24 May 2022 19:27:19 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:2408cc74d12b6cd092bb8b516ba7d5e290f485d3eb9672efc00f0583730179e8`  
		Last Modified: Mon, 23 May 2022 19:09:38 GMT  
		Size: 2.8 MB (2798889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6da329a3b4330a0705bfb49b5e6ce2fb61bc108d0a32d41c2c0dad6d9dd6c8fa`  
		Last Modified: Tue, 24 May 2022 19:27:48 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f4ba002bd64c19ecd49e1afc372709c9bcfb3dbe2b9ee2b02d43dea8fddc3cc`  
		Last Modified: Tue, 24 May 2022 19:27:48 GMT  
		Size: 108.3 KB (108307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d664dde428a76ca57c1261382f6f9b758a3b5b0e12b51f6a5b1a38bef237456a`  
		Last Modified: Tue, 24 May 2022 19:27:48 GMT  
		Size: 944.5 KB (944489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef11efc606151d8228ae06848232d8d65ae50082bf0ad5c5104d06c27ce7c85d`  
		Last Modified: Tue, 24 May 2022 19:27:48 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f118f0edbe76d09a02e63a4712d1b9b3eb1ebce2a271c740baba58cc48df9f4e`  
		Last Modified: Tue, 24 May 2022 19:27:48 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.15-alpine3.16` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:8ec1f6a98e264e73e3c7b2feba04b272ce1522adc9d40118b9684721c41122b0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.7 MB (3737167 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f393a4888061e0456042ebb89fbc11cf72af15c189e0d0e4ee62b7fcfd44c683`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 23 May 2022 19:39:22 GMT
ADD file:3ae36c6c4a1fc43157692da97c6c4fa6c3d0189ba82e2bef7f5aaf4a5e083f18 in / 
# Mon, 23 May 2022 19:39:22 GMT
CMD ["/bin/sh"]
# Tue, 24 May 2022 20:08:53 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 24 May 2022 20:08:55 GMT
RUN apk add --no-cache libsasl
# Tue, 24 May 2022 20:08:56 GMT
ENV MEMCACHED_VERSION=1.6.15
# Tue, 24 May 2022 20:08:57 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Tue, 24 May 2022 20:12:06 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 24 May 2022 20:12:08 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 24 May 2022 20:12:08 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 24 May 2022 20:12:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 24 May 2022 20:12:10 GMT
USER memcache
# Tue, 24 May 2022 20:12:11 GMT
EXPOSE 11211
# Tue, 24 May 2022 20:12:12 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:b3c136eddcbf2003d3180787cef00f39d46b9fd9e4623178282ad6a8d63ad3b0`  
		Last Modified: Mon, 23 May 2022 19:08:34 GMT  
		Size: 2.7 MB (2694464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e87d2d7a8c9bc1317afe928c225caaafd86b3b73a2bc359f8037eb0f501b394c`  
		Last Modified: Tue, 24 May 2022 20:12:58 GMT  
		Size: 1.2 KB (1242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55dbcde2059d799697807a93b36d71cd601b20e2218abb7cb9261d22e8a7d67a`  
		Last Modified: Tue, 24 May 2022 20:12:58 GMT  
		Size: 109.6 KB (109557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4aa3db0ac20b8381c09df00576661af3c209195453eeeb892b8532059b932a39`  
		Last Modified: Tue, 24 May 2022 20:12:59 GMT  
		Size: 931.5 KB (931496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d999e908ec416e199da213e6fca67cdc82d3d440098a1bfbc5bc7c5a2f35636`  
		Last Modified: Tue, 24 May 2022 20:12:58 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8017baa48e45fa47c2fab6975dcd0ab8a560c64c0de05f7113831a537b385a3b`  
		Last Modified: Tue, 24 May 2022 20:12:58 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.15-alpine3.16` - linux; 386

```console
$ docker pull memcached@sha256:3560af36f0aaeb7e4d2da47f0ad4a91bc675aa017423f34911490b09908230e8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3878370 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7d5a231eedb6e0b20291a77ac7a71c5a16aca1a9eb62893e285cefa1b95bdf5b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 23 May 2022 19:38:20 GMT
ADD file:1750ccfabfe93636015070d51a6e824cbd738056223421c69d8aaabc38041b18 in / 
# Mon, 23 May 2022 19:38:20 GMT
CMD ["/bin/sh"]
# Tue, 24 May 2022 19:46:24 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 24 May 2022 19:46:26 GMT
RUN apk add --no-cache libsasl
# Tue, 24 May 2022 19:46:26 GMT
ENV MEMCACHED_VERSION=1.6.15
# Tue, 24 May 2022 19:46:27 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Tue, 24 May 2022 19:49:17 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 24 May 2022 19:49:19 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 24 May 2022 19:49:19 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 24 May 2022 19:49:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 24 May 2022 19:49:21 GMT
USER memcache
# Tue, 24 May 2022 19:49:22 GMT
EXPOSE 11211
# Tue, 24 May 2022 19:49:23 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:bb638a3869eed698f88775c7a48f36f8e22e7c6bbaa98fa1d5678966b619b859`  
		Last Modified: Mon, 23 May 2022 19:09:25 GMT  
		Size: 2.8 MB (2801887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d301e0dbe5a2594f09f110ec3c1e79f4bd885af78b4992bf8af7a9f7b0507d5a`  
		Last Modified: Tue, 24 May 2022 19:50:14 GMT  
		Size: 1.2 KB (1242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:880ddc23b9c3165a8e86c64a648782c63c9a7271e84df6ac2f5a8c110d32258d`  
		Last Modified: Tue, 24 May 2022 19:50:14 GMT  
		Size: 119.8 KB (119821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c60884a7874466d1525bb0560fcbbbc226cfb4fb1507f1bd0d45d4f1b0e1307b`  
		Last Modified: Tue, 24 May 2022 19:50:15 GMT  
		Size: 955.0 KB (955017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89ad9c1959a10762028a884c1a33f06bb71bcb1a9ac372c889304f75f2a4b597`  
		Last Modified: Tue, 24 May 2022 19:50:14 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b267a8907abfcf28b9d96b17379ce57985989f17d34c06dfd238aee8ed0da61`  
		Last Modified: Tue, 24 May 2022 19:50:14 GMT  
		Size: 119.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.15-alpine3.16` - linux; ppc64le

```console
$ docker pull memcached@sha256:edeccd4ca90cecc053bd78239bef1a1ccec0d2f189655d39e29e44216157fec4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3891798 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:348c555fa9d4bcfd44f2f7426151f1666fd08a28ce9fea73c503bc207229c503`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 23 May 2022 19:16:51 GMT
ADD file:6a5450c8a7cee3ceda59e7cb350c54df4139b0f7b7cf49c8b31bb9c01646c3cd in / 
# Mon, 23 May 2022 19:16:53 GMT
CMD ["/bin/sh"]
# Tue, 24 May 2022 19:29:15 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 24 May 2022 19:29:23 GMT
RUN apk add --no-cache libsasl
# Tue, 24 May 2022 19:29:30 GMT
ENV MEMCACHED_VERSION=1.6.15
# Tue, 24 May 2022 19:29:36 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Tue, 24 May 2022 19:33:02 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 24 May 2022 19:33:03 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 24 May 2022 19:33:08 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 24 May 2022 19:33:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 24 May 2022 19:33:14 GMT
USER memcache
# Tue, 24 May 2022 19:33:17 GMT
EXPOSE 11211
# Tue, 24 May 2022 19:33:19 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:d3deabf2a506ef6f5fa7c2a68bf27047574cef9908b30a97ff2d01ae539b089a`  
		Last Modified: Mon, 23 May 2022 19:09:13 GMT  
		Size: 2.8 MB (2789745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b479cfab13a2f2ffe6bfc643d96b2ca17a80380353869913b72735725a953596`  
		Last Modified: Tue, 24 May 2022 19:34:20 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9111d00ba5c4381f0f8b185e1703815ef94004e492b01b0d3c7a7fe53acc977`  
		Last Modified: Tue, 24 May 2022 19:34:21 GMT  
		Size: 126.0 KB (126043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1a992983a73a33de517b221e813f6ddddea412212564e886bba2a9a09f82735`  
		Last Modified: Tue, 24 May 2022 19:34:21 GMT  
		Size: 974.3 KB (974333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6de2f26a895426d80205ef485568a93b91456d9913ce062578d21db1d228ef7`  
		Last Modified: Tue, 24 May 2022 19:34:20 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27f443297da5126d218f0cfd07deeb374b4db49ce895657aed034e4eba40ce1c`  
		Last Modified: Tue, 24 May 2022 19:34:20 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.15-alpine3.16` - linux; s390x

```console
$ docker pull memcached@sha256:79c15e8f5b25e585bc279ba8a2e990aaf1bcb0622e4b2cfe246b32381748232d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.6 MB (3629283 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3984c3293b24638ac012e61d1d83266b40194c43831d6d2f59fe1c01615baf07`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 23 May 2022 19:41:59 GMT
ADD file:e1852d8ef555a0d3ef6d0b74a898720c82bb9f491430b06a0dd0499497ce118e in / 
# Mon, 23 May 2022 19:42:10 GMT
CMD ["/bin/sh"]
# Tue, 24 May 2022 19:50:13 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 24 May 2022 19:50:14 GMT
RUN apk add --no-cache libsasl
# Tue, 24 May 2022 19:50:15 GMT
ENV MEMCACHED_VERSION=1.6.15
# Tue, 24 May 2022 19:50:15 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Tue, 24 May 2022 19:54:14 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 24 May 2022 19:54:15 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 24 May 2022 19:54:16 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 24 May 2022 19:54:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 24 May 2022 19:54:16 GMT
USER memcache
# Tue, 24 May 2022 19:54:16 GMT
EXPOSE 11211
# Tue, 24 May 2022 19:54:16 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:af1ac1a73384e058591d04d19bc05a06781cc32d52d4593b468d6cb95eda9858`  
		Last Modified: Mon, 23 May 2022 19:43:36 GMT  
		Size: 2.6 MB (2580494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0cdb25dad8a9e7c836addf0dfee4462f64217c81619f5c7519d620c59c68fff`  
		Last Modified: Tue, 24 May 2022 19:55:16 GMT  
		Size: 1.3 KB (1265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bfb96fb83213592db4a96cd8313433230d559f81caa115c56c8f9018d5e01f5`  
		Last Modified: Tue, 24 May 2022 19:55:16 GMT  
		Size: 112.5 KB (112500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fd8f0273e1af52c2d6bc2ea6e8f7c7b516ce039d78151fe854039d86e62db91`  
		Last Modified: Tue, 24 May 2022 19:55:17 GMT  
		Size: 934.6 KB (934620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a50bb84155cee8c93b5835daaee0a57b7c14397817ac75279b1ac51d2626f594`  
		Last Modified: Tue, 24 May 2022 19:55:16 GMT  
		Size: 283.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:196f82f950409b7b7c0e395502911ba3177047647ed8ac24e62c49dacf4eebf1`  
		Last Modified: Tue, 24 May 2022 19:55:17 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:1.6.15-bullseye`

```console
$ docker pull memcached@sha256:b422bca20902101cd4a427ccda5ea9729a89bdc6cd8ab8a7d8cd09b1470af6b6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; s390x

### `memcached:1.6.15-bullseye` - linux; amd64

```console
$ docker pull memcached@sha256:1be4a685ac5a327ffbd7d1c7240378e7156824f9406b1eeb5fe19eadc2e61c53
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.0 MB (32968544 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a23fd759590b790a7cae87582ba4d747378de71b47e581b9295c02ce34eb9ed0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 23 Jun 2022 00:20:27 GMT
ADD file:8adbbab04d6f84cd83b5f4205b89b0acb7ecbf27a1bb2dc181d0a629479039fe in / 
# Thu, 23 Jun 2022 00:20:27 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 04:18:20 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Thu, 23 Jun 2022 04:18:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 04:18:24 GMT
ENV MEMCACHED_VERSION=1.6.15
# Thu, 23 Jun 2022 04:18:24 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Thu, 23 Jun 2022 04:21:07 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 23 Jun 2022 04:21:07 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 23 Jun 2022 04:21:08 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 23 Jun 2022 04:21:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jun 2022 04:21:08 GMT
USER memcache
# Thu, 23 Jun 2022 04:21:08 GMT
EXPOSE 11211
# Thu, 23 Jun 2022 04:21:08 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:b85a868b505ffd0342a37e6a3b1c49f7c71878afe569a807e6238ef08252fcb7`  
		Last Modified: Thu, 23 Jun 2022 00:25:18 GMT  
		Size: 31.4 MB (31379408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f58bb523c8de07d0d72658b2e622e82f065a1adef45f6f90f11eb7c71b9d0c61`  
		Last Modified: Thu, 23 Jun 2022 04:21:33 GMT  
		Size: 5.0 KB (4979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a458d61c2cd35b8afffe3741b04321a87f86ba216e5e2a4f9429b83b32ceb35`  
		Last Modified: Thu, 23 Jun 2022 04:21:33 GMT  
		Size: 328.1 KB (328115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7eda168e1238eaa8f5c20b7240bb8bc84c9a3f7b4b8cdc0be18f58f27bff1692`  
		Last Modified: Thu, 23 Jun 2022 04:21:33 GMT  
		Size: 1.3 MB (1255633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f188c32090c0c66f2f209fedc0778269d3edf2ad9db239ac0d2e1e3b64b36fd4`  
		Last Modified: Thu, 23 Jun 2022 04:21:33 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f492776609f9ffcbe6d066f45223bc2da677c44beb7bb0cdc6dfa34271885b34`  
		Last Modified: Thu, 23 Jun 2022 04:21:33 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.15-bullseye` - linux; arm variant v5

```console
$ docker pull memcached@sha256:54ff97ee8133b4181bff0e30de243b68ffa4ad0a7ecc458e6648a24760c63213
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.5 MB (30470395 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:07faffc84c650af3ec2eb3326c593cd933cba137c34c87589a375371eee849f3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 23 Jun 2022 00:50:38 GMT
ADD file:839c0e211e2260f5d54f2633e53c817c1f59e2394ba4b12f60e01e46cee61011 in / 
# Thu, 23 Jun 2022 00:50:39 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 02:41:47 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Thu, 23 Jun 2022 02:41:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 02:41:58 GMT
ENV MEMCACHED_VERSION=1.6.15
# Thu, 23 Jun 2022 02:41:59 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Thu, 23 Jun 2022 02:46:28 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 23 Jun 2022 02:46:29 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 23 Jun 2022 02:46:31 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 23 Jun 2022 02:46:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jun 2022 02:46:32 GMT
USER memcache
# Thu, 23 Jun 2022 02:46:32 GMT
EXPOSE 11211
# Thu, 23 Jun 2022 02:46:33 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:bd2d3b4056bd1b0310082fc5d17c6d03348601456c4b9306d1a333f1cec561f9`  
		Last Modified: Thu, 23 Jun 2022 01:05:39 GMT  
		Size: 28.9 MB (28921550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f500bb51d193d56af19fbeb8ebc1919ec2e6d04cf9a7d1637ad79cc00397c1b`  
		Last Modified: Thu, 23 Jun 2022 02:47:27 GMT  
		Size: 4.9 KB (4894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c3dc6e5372afc0620e0eeae739b429bee70842f20a15ca8345787a674d5d3b8`  
		Last Modified: Thu, 23 Jun 2022 02:47:28 GMT  
		Size: 316.6 KB (316616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83d6f2e7e5c2a1d3566c4d9cd05fd132529535ba7eaecb00d312c0d0a6055a4c`  
		Last Modified: Thu, 23 Jun 2022 02:47:28 GMT  
		Size: 1.2 MB (1226926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:109349836a4d5f4431660fec9744df70f92475b22644182ae9d77c8c56c8960a`  
		Last Modified: Thu, 23 Jun 2022 02:47:27 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b87ddf1818c82326658f3ca6d444b01978e23d30a7232e4ef1e0f6f0ba4ab18`  
		Last Modified: Thu, 23 Jun 2022 02:47:27 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.15-bullseye` - linux; arm variant v7

```console
$ docker pull memcached@sha256:b3ddbe1e7ec04512ac9e20555b72ba4b2e7e9ee99138535fabe5e92cc92302b5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.1 MB (28092007 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cbbff85100ff53c710f4caa30445e0ee79ccd0fe61cc91a522821fc5415e6bcf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 23 Jun 2022 00:59:45 GMT
ADD file:925abfb9fc0e4a7cc0c979b12c9bd2607f5c493d37b05535ca010f81beb060a9 in / 
# Thu, 23 Jun 2022 00:59:46 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 22:08:47 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Thu, 23 Jun 2022 22:08:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 22:08:56 GMT
ENV MEMCACHED_VERSION=1.6.15
# Thu, 23 Jun 2022 22:08:56 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Thu, 23 Jun 2022 22:13:04 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 23 Jun 2022 22:13:05 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 23 Jun 2022 22:13:06 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 23 Jun 2022 22:13:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jun 2022 22:13:07 GMT
USER memcache
# Thu, 23 Jun 2022 22:13:08 GMT
EXPOSE 11211
# Thu, 23 Jun 2022 22:13:08 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:d2fd562560d8062a78064adfbfa204521167c301f00f5ab3c65b9c2a54083dba`  
		Last Modified: Thu, 23 Jun 2022 01:15:22 GMT  
		Size: 26.6 MB (26576105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8864d1bfbfd3f4b781316abd42de97a2967a6b20534ffdc4fea6a3de16c1d972`  
		Last Modified: Fri, 24 Jun 2022 01:14:10 GMT  
		Size: 4.9 KB (4897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fa7c6c177f3ba693baa86ed010daf821ca2addfe7f3b8a83c7f52fac209a6e8`  
		Last Modified: Fri, 24 Jun 2022 01:14:10 GMT  
		Size: 312.1 KB (312076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f802ee5fb123a2824f3e6f93144c74f9e1c88159fc819b46f7ed2913ec61281a`  
		Last Modified: Fri, 24 Jun 2022 01:14:11 GMT  
		Size: 1.2 MB (1198521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25b61f87cd4332b040dd59bae91f0701228904433b1955bb4f51b7377db17b00`  
		Last Modified: Fri, 24 Jun 2022 01:14:10 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:532462b4f12685e2093583f1e86c82d5c2c8069b92ccbc9bbcf8efad7dfd3252`  
		Last Modified: Fri, 24 Jun 2022 01:14:10 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.15-bullseye` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:536f8192668e851874eec7d483055b0af220a7eb0be43010f2f9825e99ab0111
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.4 MB (31444932 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2ce58160065ec196d51dcdc756610352a57f6192b28345989be83b94b8300dec`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 23 Jun 2022 00:40:43 GMT
ADD file:134be48af13f80f3474bf1b080ca781feb7b972148d482849862e55eb2acd61c in / 
# Thu, 23 Jun 2022 00:40:44 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 03:53:19 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Thu, 23 Jun 2022 03:53:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 03:53:24 GMT
ENV MEMCACHED_VERSION=1.6.15
# Thu, 23 Jun 2022 03:53:25 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Thu, 23 Jun 2022 03:56:00 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 23 Jun 2022 03:56:02 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 23 Jun 2022 03:56:02 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 23 Jun 2022 03:56:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jun 2022 03:56:04 GMT
USER memcache
# Thu, 23 Jun 2022 03:56:05 GMT
EXPOSE 11211
# Thu, 23 Jun 2022 03:56:06 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:3b157c852f2736e12f09046f214fe5f6a0b1652bd860269b3988c92a197026e8`  
		Last Modified: Thu, 23 Jun 2022 00:47:22 GMT  
		Size: 30.1 MB (30065720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee776bb67ffbc00ca5100c88e1f7ae63b580bc131c046c3c7138b7fb796683a2`  
		Last Modified: Thu, 23 Jun 2022 03:56:51 GMT  
		Size: 4.9 KB (4904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85b234170a3d54e3ad2be2993a7e7b09550a4e00327804a183e07bc786d01bc8`  
		Last Modified: Thu, 23 Jun 2022 03:56:51 GMT  
		Size: 119.2 KB (119223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a61e7150a45b8305adc14ed47f7beb3e807a7f08223393e6f5382b043b120941`  
		Last Modified: Thu, 23 Jun 2022 03:56:51 GMT  
		Size: 1.3 MB (1254677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ed6ad1685f73da9293938d389b8c24ee8b8af4d04d4c8b502cb6082d58bf349`  
		Last Modified: Thu, 23 Jun 2022 03:56:51 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:276672cde8876c99c646defdc630e9be5ae5cfb33c192102b6387ce99d151179`  
		Last Modified: Thu, 23 Jun 2022 03:56:51 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.15-bullseye` - linux; 386

```console
$ docker pull memcached@sha256:651e5275f0623232ecfa476f864b6634de4e9ffc6671376c796ffd70e31c83b6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.8 MB (33778463 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31252c746c529da361fcb075711def9645866db716700e15d9e4ce92e96ed3a0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 23 Jun 2022 00:39:33 GMT
ADD file:9d46d3f8fb63833a6dbd8dd796ad541d556046a48342d22e1fd3bffa3fb8e504 in / 
# Thu, 23 Jun 2022 00:39:33 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 03:32:31 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Thu, 23 Jun 2022 03:32:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 03:32:36 GMT
ENV MEMCACHED_VERSION=1.6.15
# Thu, 23 Jun 2022 03:32:37 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Thu, 23 Jun 2022 03:35:28 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 23 Jun 2022 03:35:30 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 23 Jun 2022 03:35:30 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 23 Jun 2022 03:35:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jun 2022 03:35:32 GMT
USER memcache
# Thu, 23 Jun 2022 03:35:33 GMT
EXPOSE 11211
# Thu, 23 Jun 2022 03:35:34 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:4870b12e407743816673c11cfb39974d80c1569d876287bef61f8c585954822f`  
		Last Modified: Thu, 23 Jun 2022 00:46:40 GMT  
		Size: 32.4 MB (32390198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a67b6581e800ff3e02f41dd18cb78bc620a25becd83769f84d2c61aed5d01ea`  
		Last Modified: Thu, 23 Jun 2022 03:36:21 GMT  
		Size: 4.8 KB (4773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b70025d0ac3fc2b23b2e76f6d96c607c6a04b53c9850fe3f14fa855827b9d19d`  
		Last Modified: Thu, 23 Jun 2022 03:36:21 GMT  
		Size: 130.1 KB (130137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a383a40e44984d67c847d2a4bbc7d3525f3867ff39c81a5221970dc744ee822e`  
		Last Modified: Thu, 23 Jun 2022 03:36:21 GMT  
		Size: 1.3 MB (1252947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24f731218f56e8a5f3d250c9a4e15f841afbd92a0ee71f88761feb880aa937b3`  
		Last Modified: Thu, 23 Jun 2022 03:36:21 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15ab75a8041fc16fdde22888eb35315059264f2c153e8d05d7f132d1aa413e3a`  
		Last Modified: Thu, 23 Jun 2022 03:36:21 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.15-bullseye` - linux; mips64le

```console
$ docker pull memcached@sha256:71ebcf40d19139f8bab5733065ff1b2599e5d52359c6f6cbfad2104be2f1fe33
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.0 MB (31014756 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d95105805101f850723625215940d8b2be96a9b40f984174eee903985becb9e0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 23 Jun 2022 01:10:25 GMT
ADD file:fd1174cc47ac636f0cab382578a899d69ed489e4dee53ec838955e36066f526a in / 
# Thu, 23 Jun 2022 01:10:29 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 03:13:46 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Thu, 23 Jun 2022 03:14:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 03:14:06 GMT
ENV MEMCACHED_VERSION=1.6.15
# Thu, 23 Jun 2022 03:14:08 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Thu, 23 Jun 2022 03:21:07 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 23 Jun 2022 03:21:09 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 23 Jun 2022 03:21:15 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 23 Jun 2022 03:21:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jun 2022 03:21:20 GMT
USER memcache
# Thu, 23 Jun 2022 03:21:22 GMT
EXPOSE 11211
# Thu, 23 Jun 2022 03:21:25 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:9d199cb5e183b38c9edcc527cbaaa79bb56da73bd09ed449223842775ef4a244`  
		Last Modified: Thu, 23 Jun 2022 01:20:19 GMT  
		Size: 29.6 MB (29641027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d188c3e3bf643b15e2e70cc10dab71da1f4e871305c84cf6d927a2750209ee47`  
		Last Modified: Thu, 23 Jun 2022 03:21:53 GMT  
		Size: 4.9 KB (4863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8855d5fcd2d728913f5ae40b13f074576721a44abf081e6bd4e8f48e8deb8262`  
		Last Modified: Thu, 23 Jun 2022 03:21:54 GMT  
		Size: 117.2 KB (117169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:726be3b42973c4aa79e2ffcecb3633c1ec825f8099da6b5d952810bf4d1827cd`  
		Last Modified: Thu, 23 Jun 2022 03:21:54 GMT  
		Size: 1.3 MB (1251289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6176796787c17dc9b41c47c10e23979540bb32e2833c3eeceb1456f0b228166f`  
		Last Modified: Thu, 23 Jun 2022 03:21:54 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:926c03f02a771007ddd9b4fd2172ff2d89647400c4370fdedb4533a5c99e42b1`  
		Last Modified: Thu, 23 Jun 2022 03:21:53 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.15-bullseye` - linux; ppc64le

```console
$ docker pull memcached@sha256:0bfecd8ca43abc3e50d162ce07d6794beb5d9f98ce929e9371c2542065e6c785
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.0 MB (36972124 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ac53be686814de607770ae7fba96134fc9cd4e5afe7444779b08c02a0c92a6c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 23 Jun 2022 02:02:32 GMT
ADD file:e18c13649ea1f145047652c8e171c4824f9b6b0dbc92127a914c7fca910acf96 in / 
# Thu, 23 Jun 2022 02:02:34 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 08:15:12 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Thu, 23 Jun 2022 08:15:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 08:15:26 GMT
ENV MEMCACHED_VERSION=1.6.15
# Thu, 23 Jun 2022 08:15:30 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Thu, 23 Jun 2022 08:20:21 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 23 Jun 2022 08:20:23 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 23 Jun 2022 08:20:29 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 23 Jun 2022 08:20:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jun 2022 08:20:34 GMT
USER memcache
# Thu, 23 Jun 2022 08:20:36 GMT
EXPOSE 11211
# Thu, 23 Jun 2022 08:20:38 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:7716f0df7ba06b6f1937cd664805984e25e386a4165f2c6acc65356686e35221`  
		Last Modified: Thu, 23 Jun 2022 02:15:20 GMT  
		Size: 35.3 MB (35286823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54d7d03c3543d8cc9dbdea919601e8b8bdebdf5f54f23ee2a186edde48a4025c`  
		Last Modified: Thu, 23 Jun 2022 08:21:29 GMT  
		Size: 5.0 KB (4987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa5efdc63c420d0295d4932cc7467f1a9005b4724f592c4fba99b6c801f57810`  
		Last Modified: Thu, 23 Jun 2022 08:21:29 GMT  
		Size: 357.0 KB (356958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:329e40de463f01938ecac1d284adb38a29fde479486e279cb302d95abe9f4a16`  
		Last Modified: Thu, 23 Jun 2022 08:21:29 GMT  
		Size: 1.3 MB (1322949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d823793235eacc3363db343cea0db041905e9fde59ff5262e0fd8826e962f5a`  
		Last Modified: Thu, 23 Jun 2022 08:21:29 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2ae46dbc3324ea97ee7556a1bc8006b075f7a1492e3a2114aaf8dec7c579b76`  
		Last Modified: Thu, 23 Jun 2022 08:21:29 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.15-bullseye` - linux; s390x

```console
$ docker pull memcached@sha256:1e49c15efaf9999b31f526130902a04a53eeac416f40d1549e98b3fa1a872c04
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.2 MB (31226391 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b8090a3ed64f97313e1ddce878717e3bf8c1aace9d7bf247a1fa53418081f0c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 23 Jun 2022 00:43:10 GMT
ADD file:0b511e3efd87267fb27161eae56c4d08f0fed733697da6ffe6ea96a4cb68e938 in / 
# Thu, 23 Jun 2022 00:43:15 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 13:41:46 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Thu, 23 Jun 2022 13:41:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 13:41:49 GMT
ENV MEMCACHED_VERSION=1.6.15
# Thu, 23 Jun 2022 13:41:50 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Thu, 23 Jun 2022 13:45:09 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 23 Jun 2022 13:45:09 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 23 Jun 2022 13:45:10 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 23 Jun 2022 13:45:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jun 2022 13:45:10 GMT
USER memcache
# Thu, 23 Jun 2022 13:45:10 GMT
EXPOSE 11211
# Thu, 23 Jun 2022 13:45:10 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:c547f465e0c8708ad0c57cf09caa52f4c2b5b295bf10ab1ce71ca17ff81ea36a`  
		Last Modified: Thu, 23 Jun 2022 00:51:59 GMT  
		Size: 29.7 MB (29655262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04837776e7fbb579dda3720caca85ff9cb19eea15a8830ab0f23a160fa832205`  
		Last Modified: Thu, 23 Jun 2022 13:46:03 GMT  
		Size: 5.0 KB (5025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d844915fd9a66accf5106919c6a63121ed4fde412dcf958133bc1b1483b307b`  
		Last Modified: Thu, 23 Jun 2022 13:46:03 GMT  
		Size: 324.2 KB (324209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51abf5cd3f179d43b5845c7dc42a6f07ddfd6da706ca58f78d53641e3d62289f`  
		Last Modified: Thu, 23 Jun 2022 13:46:03 GMT  
		Size: 1.2 MB (1241485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31ea51fd993089ad7346961b0897d009e18b953416139bf4359ff089b9e9ada9`  
		Last Modified: Thu, 23 Jun 2022 13:46:04 GMT  
		Size: 289.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cda18e1b304fdde7d799586641bad45a035387c02b0c7e8d696e91221b046e28`  
		Last Modified: Thu, 23 Jun 2022 13:46:03 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:alpine`

```console
$ docker pull memcached@sha256:96af3fed9ef980101602ea90c3220679bb326bfe70474e4f06759f25db4591e2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `memcached:alpine` - linux; amd64

```console
$ docker pull memcached@sha256:bae66da0e8cdb7daa226cc0837e2562404a4007466044ffdfa88a8a0431d5c7a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3853361 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e3f5d6e8d61d2ec54ff3d21da1c6dbddca8f0018c8f1c1253287129fa3926d7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 23 May 2022 19:19:30 GMT
ADD file:8e81116368669ed3dd361bc898d61bff249f524139a239fdaf3ec46869a39921 in / 
# Mon, 23 May 2022 19:19:31 GMT
CMD ["/bin/sh"]
# Tue, 24 May 2022 19:24:21 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 24 May 2022 19:24:23 GMT
RUN apk add --no-cache libsasl
# Tue, 24 May 2022 19:24:23 GMT
ENV MEMCACHED_VERSION=1.6.15
# Tue, 24 May 2022 19:24:23 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Tue, 24 May 2022 19:27:18 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 24 May 2022 19:27:18 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 24 May 2022 19:27:19 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 24 May 2022 19:27:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 24 May 2022 19:27:19 GMT
USER memcache
# Tue, 24 May 2022 19:27:19 GMT
EXPOSE 11211
# Tue, 24 May 2022 19:27:19 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:2408cc74d12b6cd092bb8b516ba7d5e290f485d3eb9672efc00f0583730179e8`  
		Last Modified: Mon, 23 May 2022 19:09:38 GMT  
		Size: 2.8 MB (2798889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6da329a3b4330a0705bfb49b5e6ce2fb61bc108d0a32d41c2c0dad6d9dd6c8fa`  
		Last Modified: Tue, 24 May 2022 19:27:48 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f4ba002bd64c19ecd49e1afc372709c9bcfb3dbe2b9ee2b02d43dea8fddc3cc`  
		Last Modified: Tue, 24 May 2022 19:27:48 GMT  
		Size: 108.3 KB (108307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d664dde428a76ca57c1261382f6f9b758a3b5b0e12b51f6a5b1a38bef237456a`  
		Last Modified: Tue, 24 May 2022 19:27:48 GMT  
		Size: 944.5 KB (944489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef11efc606151d8228ae06848232d8d65ae50082bf0ad5c5104d06c27ce7c85d`  
		Last Modified: Tue, 24 May 2022 19:27:48 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f118f0edbe76d09a02e63a4712d1b9b3eb1ebce2a271c740baba58cc48df9f4e`  
		Last Modified: Tue, 24 May 2022 19:27:48 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

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
$ docker pull memcached@sha256:8ec1f6a98e264e73e3c7b2feba04b272ce1522adc9d40118b9684721c41122b0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.7 MB (3737167 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f393a4888061e0456042ebb89fbc11cf72af15c189e0d0e4ee62b7fcfd44c683`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 23 May 2022 19:39:22 GMT
ADD file:3ae36c6c4a1fc43157692da97c6c4fa6c3d0189ba82e2bef7f5aaf4a5e083f18 in / 
# Mon, 23 May 2022 19:39:22 GMT
CMD ["/bin/sh"]
# Tue, 24 May 2022 20:08:53 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 24 May 2022 20:08:55 GMT
RUN apk add --no-cache libsasl
# Tue, 24 May 2022 20:08:56 GMT
ENV MEMCACHED_VERSION=1.6.15
# Tue, 24 May 2022 20:08:57 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Tue, 24 May 2022 20:12:06 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 24 May 2022 20:12:08 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 24 May 2022 20:12:08 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 24 May 2022 20:12:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 24 May 2022 20:12:10 GMT
USER memcache
# Tue, 24 May 2022 20:12:11 GMT
EXPOSE 11211
# Tue, 24 May 2022 20:12:12 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:b3c136eddcbf2003d3180787cef00f39d46b9fd9e4623178282ad6a8d63ad3b0`  
		Last Modified: Mon, 23 May 2022 19:08:34 GMT  
		Size: 2.7 MB (2694464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e87d2d7a8c9bc1317afe928c225caaafd86b3b73a2bc359f8037eb0f501b394c`  
		Last Modified: Tue, 24 May 2022 20:12:58 GMT  
		Size: 1.2 KB (1242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55dbcde2059d799697807a93b36d71cd601b20e2218abb7cb9261d22e8a7d67a`  
		Last Modified: Tue, 24 May 2022 20:12:58 GMT  
		Size: 109.6 KB (109557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4aa3db0ac20b8381c09df00576661af3c209195453eeeb892b8532059b932a39`  
		Last Modified: Tue, 24 May 2022 20:12:59 GMT  
		Size: 931.5 KB (931496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d999e908ec416e199da213e6fca67cdc82d3d440098a1bfbc5bc7c5a2f35636`  
		Last Modified: Tue, 24 May 2022 20:12:58 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8017baa48e45fa47c2fab6975dcd0ab8a560c64c0de05f7113831a537b385a3b`  
		Last Modified: Tue, 24 May 2022 20:12:58 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:alpine` - linux; 386

```console
$ docker pull memcached@sha256:3560af36f0aaeb7e4d2da47f0ad4a91bc675aa017423f34911490b09908230e8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3878370 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7d5a231eedb6e0b20291a77ac7a71c5a16aca1a9eb62893e285cefa1b95bdf5b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 23 May 2022 19:38:20 GMT
ADD file:1750ccfabfe93636015070d51a6e824cbd738056223421c69d8aaabc38041b18 in / 
# Mon, 23 May 2022 19:38:20 GMT
CMD ["/bin/sh"]
# Tue, 24 May 2022 19:46:24 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 24 May 2022 19:46:26 GMT
RUN apk add --no-cache libsasl
# Tue, 24 May 2022 19:46:26 GMT
ENV MEMCACHED_VERSION=1.6.15
# Tue, 24 May 2022 19:46:27 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Tue, 24 May 2022 19:49:17 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 24 May 2022 19:49:19 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 24 May 2022 19:49:19 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 24 May 2022 19:49:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 24 May 2022 19:49:21 GMT
USER memcache
# Tue, 24 May 2022 19:49:22 GMT
EXPOSE 11211
# Tue, 24 May 2022 19:49:23 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:bb638a3869eed698f88775c7a48f36f8e22e7c6bbaa98fa1d5678966b619b859`  
		Last Modified: Mon, 23 May 2022 19:09:25 GMT  
		Size: 2.8 MB (2801887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d301e0dbe5a2594f09f110ec3c1e79f4bd885af78b4992bf8af7a9f7b0507d5a`  
		Last Modified: Tue, 24 May 2022 19:50:14 GMT  
		Size: 1.2 KB (1242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:880ddc23b9c3165a8e86c64a648782c63c9a7271e84df6ac2f5a8c110d32258d`  
		Last Modified: Tue, 24 May 2022 19:50:14 GMT  
		Size: 119.8 KB (119821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c60884a7874466d1525bb0560fcbbbc226cfb4fb1507f1bd0d45d4f1b0e1307b`  
		Last Modified: Tue, 24 May 2022 19:50:15 GMT  
		Size: 955.0 KB (955017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89ad9c1959a10762028a884c1a33f06bb71bcb1a9ac372c889304f75f2a4b597`  
		Last Modified: Tue, 24 May 2022 19:50:14 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b267a8907abfcf28b9d96b17379ce57985989f17d34c06dfd238aee8ed0da61`  
		Last Modified: Tue, 24 May 2022 19:50:14 GMT  
		Size: 119.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:alpine` - linux; ppc64le

```console
$ docker pull memcached@sha256:edeccd4ca90cecc053bd78239bef1a1ccec0d2f189655d39e29e44216157fec4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3891798 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:348c555fa9d4bcfd44f2f7426151f1666fd08a28ce9fea73c503bc207229c503`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 23 May 2022 19:16:51 GMT
ADD file:6a5450c8a7cee3ceda59e7cb350c54df4139b0f7b7cf49c8b31bb9c01646c3cd in / 
# Mon, 23 May 2022 19:16:53 GMT
CMD ["/bin/sh"]
# Tue, 24 May 2022 19:29:15 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 24 May 2022 19:29:23 GMT
RUN apk add --no-cache libsasl
# Tue, 24 May 2022 19:29:30 GMT
ENV MEMCACHED_VERSION=1.6.15
# Tue, 24 May 2022 19:29:36 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Tue, 24 May 2022 19:33:02 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 24 May 2022 19:33:03 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 24 May 2022 19:33:08 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 24 May 2022 19:33:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 24 May 2022 19:33:14 GMT
USER memcache
# Tue, 24 May 2022 19:33:17 GMT
EXPOSE 11211
# Tue, 24 May 2022 19:33:19 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:d3deabf2a506ef6f5fa7c2a68bf27047574cef9908b30a97ff2d01ae539b089a`  
		Last Modified: Mon, 23 May 2022 19:09:13 GMT  
		Size: 2.8 MB (2789745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b479cfab13a2f2ffe6bfc643d96b2ca17a80380353869913b72735725a953596`  
		Last Modified: Tue, 24 May 2022 19:34:20 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9111d00ba5c4381f0f8b185e1703815ef94004e492b01b0d3c7a7fe53acc977`  
		Last Modified: Tue, 24 May 2022 19:34:21 GMT  
		Size: 126.0 KB (126043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1a992983a73a33de517b221e813f6ddddea412212564e886bba2a9a09f82735`  
		Last Modified: Tue, 24 May 2022 19:34:21 GMT  
		Size: 974.3 KB (974333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6de2f26a895426d80205ef485568a93b91456d9913ce062578d21db1d228ef7`  
		Last Modified: Tue, 24 May 2022 19:34:20 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27f443297da5126d218f0cfd07deeb374b4db49ce895657aed034e4eba40ce1c`  
		Last Modified: Tue, 24 May 2022 19:34:20 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:alpine` - linux; s390x

```console
$ docker pull memcached@sha256:79c15e8f5b25e585bc279ba8a2e990aaf1bcb0622e4b2cfe246b32381748232d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.6 MB (3629283 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3984c3293b24638ac012e61d1d83266b40194c43831d6d2f59fe1c01615baf07`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 23 May 2022 19:41:59 GMT
ADD file:e1852d8ef555a0d3ef6d0b74a898720c82bb9f491430b06a0dd0499497ce118e in / 
# Mon, 23 May 2022 19:42:10 GMT
CMD ["/bin/sh"]
# Tue, 24 May 2022 19:50:13 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 24 May 2022 19:50:14 GMT
RUN apk add --no-cache libsasl
# Tue, 24 May 2022 19:50:15 GMT
ENV MEMCACHED_VERSION=1.6.15
# Tue, 24 May 2022 19:50:15 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Tue, 24 May 2022 19:54:14 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 24 May 2022 19:54:15 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 24 May 2022 19:54:16 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 24 May 2022 19:54:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 24 May 2022 19:54:16 GMT
USER memcache
# Tue, 24 May 2022 19:54:16 GMT
EXPOSE 11211
# Tue, 24 May 2022 19:54:16 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:af1ac1a73384e058591d04d19bc05a06781cc32d52d4593b468d6cb95eda9858`  
		Last Modified: Mon, 23 May 2022 19:43:36 GMT  
		Size: 2.6 MB (2580494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0cdb25dad8a9e7c836addf0dfee4462f64217c81619f5c7519d620c59c68fff`  
		Last Modified: Tue, 24 May 2022 19:55:16 GMT  
		Size: 1.3 KB (1265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bfb96fb83213592db4a96cd8313433230d559f81caa115c56c8f9018d5e01f5`  
		Last Modified: Tue, 24 May 2022 19:55:16 GMT  
		Size: 112.5 KB (112500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fd8f0273e1af52c2d6bc2ea6e8f7c7b516ce039d78151fe854039d86e62db91`  
		Last Modified: Tue, 24 May 2022 19:55:17 GMT  
		Size: 934.6 KB (934620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a50bb84155cee8c93b5835daaee0a57b7c14397817ac75279b1ac51d2626f594`  
		Last Modified: Tue, 24 May 2022 19:55:16 GMT  
		Size: 283.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:196f82f950409b7b7c0e395502911ba3177047647ed8ac24e62c49dacf4eebf1`  
		Last Modified: Tue, 24 May 2022 19:55:17 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:alpine3.16`

```console
$ docker pull memcached@sha256:bab32a8a61543525190db12c2a518c3c2331656a4409185f0f4f33a506e3aae7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `memcached:alpine3.16` - linux; amd64

```console
$ docker pull memcached@sha256:bae66da0e8cdb7daa226cc0837e2562404a4007466044ffdfa88a8a0431d5c7a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3853361 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e3f5d6e8d61d2ec54ff3d21da1c6dbddca8f0018c8f1c1253287129fa3926d7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 23 May 2022 19:19:30 GMT
ADD file:8e81116368669ed3dd361bc898d61bff249f524139a239fdaf3ec46869a39921 in / 
# Mon, 23 May 2022 19:19:31 GMT
CMD ["/bin/sh"]
# Tue, 24 May 2022 19:24:21 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 24 May 2022 19:24:23 GMT
RUN apk add --no-cache libsasl
# Tue, 24 May 2022 19:24:23 GMT
ENV MEMCACHED_VERSION=1.6.15
# Tue, 24 May 2022 19:24:23 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Tue, 24 May 2022 19:27:18 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 24 May 2022 19:27:18 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 24 May 2022 19:27:19 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 24 May 2022 19:27:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 24 May 2022 19:27:19 GMT
USER memcache
# Tue, 24 May 2022 19:27:19 GMT
EXPOSE 11211
# Tue, 24 May 2022 19:27:19 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:2408cc74d12b6cd092bb8b516ba7d5e290f485d3eb9672efc00f0583730179e8`  
		Last Modified: Mon, 23 May 2022 19:09:38 GMT  
		Size: 2.8 MB (2798889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6da329a3b4330a0705bfb49b5e6ce2fb61bc108d0a32d41c2c0dad6d9dd6c8fa`  
		Last Modified: Tue, 24 May 2022 19:27:48 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f4ba002bd64c19ecd49e1afc372709c9bcfb3dbe2b9ee2b02d43dea8fddc3cc`  
		Last Modified: Tue, 24 May 2022 19:27:48 GMT  
		Size: 108.3 KB (108307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d664dde428a76ca57c1261382f6f9b758a3b5b0e12b51f6a5b1a38bef237456a`  
		Last Modified: Tue, 24 May 2022 19:27:48 GMT  
		Size: 944.5 KB (944489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef11efc606151d8228ae06848232d8d65ae50082bf0ad5c5104d06c27ce7c85d`  
		Last Modified: Tue, 24 May 2022 19:27:48 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f118f0edbe76d09a02e63a4712d1b9b3eb1ebce2a271c740baba58cc48df9f4e`  
		Last Modified: Tue, 24 May 2022 19:27:48 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:alpine3.16` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:8ec1f6a98e264e73e3c7b2feba04b272ce1522adc9d40118b9684721c41122b0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.7 MB (3737167 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f393a4888061e0456042ebb89fbc11cf72af15c189e0d0e4ee62b7fcfd44c683`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 23 May 2022 19:39:22 GMT
ADD file:3ae36c6c4a1fc43157692da97c6c4fa6c3d0189ba82e2bef7f5aaf4a5e083f18 in / 
# Mon, 23 May 2022 19:39:22 GMT
CMD ["/bin/sh"]
# Tue, 24 May 2022 20:08:53 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 24 May 2022 20:08:55 GMT
RUN apk add --no-cache libsasl
# Tue, 24 May 2022 20:08:56 GMT
ENV MEMCACHED_VERSION=1.6.15
# Tue, 24 May 2022 20:08:57 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Tue, 24 May 2022 20:12:06 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 24 May 2022 20:12:08 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 24 May 2022 20:12:08 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 24 May 2022 20:12:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 24 May 2022 20:12:10 GMT
USER memcache
# Tue, 24 May 2022 20:12:11 GMT
EXPOSE 11211
# Tue, 24 May 2022 20:12:12 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:b3c136eddcbf2003d3180787cef00f39d46b9fd9e4623178282ad6a8d63ad3b0`  
		Last Modified: Mon, 23 May 2022 19:08:34 GMT  
		Size: 2.7 MB (2694464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e87d2d7a8c9bc1317afe928c225caaafd86b3b73a2bc359f8037eb0f501b394c`  
		Last Modified: Tue, 24 May 2022 20:12:58 GMT  
		Size: 1.2 KB (1242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55dbcde2059d799697807a93b36d71cd601b20e2218abb7cb9261d22e8a7d67a`  
		Last Modified: Tue, 24 May 2022 20:12:58 GMT  
		Size: 109.6 KB (109557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4aa3db0ac20b8381c09df00576661af3c209195453eeeb892b8532059b932a39`  
		Last Modified: Tue, 24 May 2022 20:12:59 GMT  
		Size: 931.5 KB (931496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d999e908ec416e199da213e6fca67cdc82d3d440098a1bfbc5bc7c5a2f35636`  
		Last Modified: Tue, 24 May 2022 20:12:58 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8017baa48e45fa47c2fab6975dcd0ab8a560c64c0de05f7113831a537b385a3b`  
		Last Modified: Tue, 24 May 2022 20:12:58 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:alpine3.16` - linux; 386

```console
$ docker pull memcached@sha256:3560af36f0aaeb7e4d2da47f0ad4a91bc675aa017423f34911490b09908230e8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3878370 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7d5a231eedb6e0b20291a77ac7a71c5a16aca1a9eb62893e285cefa1b95bdf5b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 23 May 2022 19:38:20 GMT
ADD file:1750ccfabfe93636015070d51a6e824cbd738056223421c69d8aaabc38041b18 in / 
# Mon, 23 May 2022 19:38:20 GMT
CMD ["/bin/sh"]
# Tue, 24 May 2022 19:46:24 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 24 May 2022 19:46:26 GMT
RUN apk add --no-cache libsasl
# Tue, 24 May 2022 19:46:26 GMT
ENV MEMCACHED_VERSION=1.6.15
# Tue, 24 May 2022 19:46:27 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Tue, 24 May 2022 19:49:17 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 24 May 2022 19:49:19 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 24 May 2022 19:49:19 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 24 May 2022 19:49:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 24 May 2022 19:49:21 GMT
USER memcache
# Tue, 24 May 2022 19:49:22 GMT
EXPOSE 11211
# Tue, 24 May 2022 19:49:23 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:bb638a3869eed698f88775c7a48f36f8e22e7c6bbaa98fa1d5678966b619b859`  
		Last Modified: Mon, 23 May 2022 19:09:25 GMT  
		Size: 2.8 MB (2801887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d301e0dbe5a2594f09f110ec3c1e79f4bd885af78b4992bf8af7a9f7b0507d5a`  
		Last Modified: Tue, 24 May 2022 19:50:14 GMT  
		Size: 1.2 KB (1242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:880ddc23b9c3165a8e86c64a648782c63c9a7271e84df6ac2f5a8c110d32258d`  
		Last Modified: Tue, 24 May 2022 19:50:14 GMT  
		Size: 119.8 KB (119821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c60884a7874466d1525bb0560fcbbbc226cfb4fb1507f1bd0d45d4f1b0e1307b`  
		Last Modified: Tue, 24 May 2022 19:50:15 GMT  
		Size: 955.0 KB (955017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89ad9c1959a10762028a884c1a33f06bb71bcb1a9ac372c889304f75f2a4b597`  
		Last Modified: Tue, 24 May 2022 19:50:14 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b267a8907abfcf28b9d96b17379ce57985989f17d34c06dfd238aee8ed0da61`  
		Last Modified: Tue, 24 May 2022 19:50:14 GMT  
		Size: 119.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:alpine3.16` - linux; ppc64le

```console
$ docker pull memcached@sha256:edeccd4ca90cecc053bd78239bef1a1ccec0d2f189655d39e29e44216157fec4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3891798 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:348c555fa9d4bcfd44f2f7426151f1666fd08a28ce9fea73c503bc207229c503`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 23 May 2022 19:16:51 GMT
ADD file:6a5450c8a7cee3ceda59e7cb350c54df4139b0f7b7cf49c8b31bb9c01646c3cd in / 
# Mon, 23 May 2022 19:16:53 GMT
CMD ["/bin/sh"]
# Tue, 24 May 2022 19:29:15 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 24 May 2022 19:29:23 GMT
RUN apk add --no-cache libsasl
# Tue, 24 May 2022 19:29:30 GMT
ENV MEMCACHED_VERSION=1.6.15
# Tue, 24 May 2022 19:29:36 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Tue, 24 May 2022 19:33:02 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 24 May 2022 19:33:03 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 24 May 2022 19:33:08 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 24 May 2022 19:33:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 24 May 2022 19:33:14 GMT
USER memcache
# Tue, 24 May 2022 19:33:17 GMT
EXPOSE 11211
# Tue, 24 May 2022 19:33:19 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:d3deabf2a506ef6f5fa7c2a68bf27047574cef9908b30a97ff2d01ae539b089a`  
		Last Modified: Mon, 23 May 2022 19:09:13 GMT  
		Size: 2.8 MB (2789745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b479cfab13a2f2ffe6bfc643d96b2ca17a80380353869913b72735725a953596`  
		Last Modified: Tue, 24 May 2022 19:34:20 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9111d00ba5c4381f0f8b185e1703815ef94004e492b01b0d3c7a7fe53acc977`  
		Last Modified: Tue, 24 May 2022 19:34:21 GMT  
		Size: 126.0 KB (126043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1a992983a73a33de517b221e813f6ddddea412212564e886bba2a9a09f82735`  
		Last Modified: Tue, 24 May 2022 19:34:21 GMT  
		Size: 974.3 KB (974333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6de2f26a895426d80205ef485568a93b91456d9913ce062578d21db1d228ef7`  
		Last Modified: Tue, 24 May 2022 19:34:20 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27f443297da5126d218f0cfd07deeb374b4db49ce895657aed034e4eba40ce1c`  
		Last Modified: Tue, 24 May 2022 19:34:20 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:alpine3.16` - linux; s390x

```console
$ docker pull memcached@sha256:79c15e8f5b25e585bc279ba8a2e990aaf1bcb0622e4b2cfe246b32381748232d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.6 MB (3629283 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3984c3293b24638ac012e61d1d83266b40194c43831d6d2f59fe1c01615baf07`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 23 May 2022 19:41:59 GMT
ADD file:e1852d8ef555a0d3ef6d0b74a898720c82bb9f491430b06a0dd0499497ce118e in / 
# Mon, 23 May 2022 19:42:10 GMT
CMD ["/bin/sh"]
# Tue, 24 May 2022 19:50:13 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 24 May 2022 19:50:14 GMT
RUN apk add --no-cache libsasl
# Tue, 24 May 2022 19:50:15 GMT
ENV MEMCACHED_VERSION=1.6.15
# Tue, 24 May 2022 19:50:15 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Tue, 24 May 2022 19:54:14 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 24 May 2022 19:54:15 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 24 May 2022 19:54:16 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 24 May 2022 19:54:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 24 May 2022 19:54:16 GMT
USER memcache
# Tue, 24 May 2022 19:54:16 GMT
EXPOSE 11211
# Tue, 24 May 2022 19:54:16 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:af1ac1a73384e058591d04d19bc05a06781cc32d52d4593b468d6cb95eda9858`  
		Last Modified: Mon, 23 May 2022 19:43:36 GMT  
		Size: 2.6 MB (2580494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0cdb25dad8a9e7c836addf0dfee4462f64217c81619f5c7519d620c59c68fff`  
		Last Modified: Tue, 24 May 2022 19:55:16 GMT  
		Size: 1.3 KB (1265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bfb96fb83213592db4a96cd8313433230d559f81caa115c56c8f9018d5e01f5`  
		Last Modified: Tue, 24 May 2022 19:55:16 GMT  
		Size: 112.5 KB (112500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fd8f0273e1af52c2d6bc2ea6e8f7c7b516ce039d78151fe854039d86e62db91`  
		Last Modified: Tue, 24 May 2022 19:55:17 GMT  
		Size: 934.6 KB (934620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a50bb84155cee8c93b5835daaee0a57b7c14397817ac75279b1ac51d2626f594`  
		Last Modified: Tue, 24 May 2022 19:55:16 GMT  
		Size: 283.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:196f82f950409b7b7c0e395502911ba3177047647ed8ac24e62c49dacf4eebf1`  
		Last Modified: Tue, 24 May 2022 19:55:17 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:bullseye`

```console
$ docker pull memcached@sha256:b422bca20902101cd4a427ccda5ea9729a89bdc6cd8ab8a7d8cd09b1470af6b6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; s390x

### `memcached:bullseye` - linux; amd64

```console
$ docker pull memcached@sha256:1be4a685ac5a327ffbd7d1c7240378e7156824f9406b1eeb5fe19eadc2e61c53
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.0 MB (32968544 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a23fd759590b790a7cae87582ba4d747378de71b47e581b9295c02ce34eb9ed0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 23 Jun 2022 00:20:27 GMT
ADD file:8adbbab04d6f84cd83b5f4205b89b0acb7ecbf27a1bb2dc181d0a629479039fe in / 
# Thu, 23 Jun 2022 00:20:27 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 04:18:20 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Thu, 23 Jun 2022 04:18:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 04:18:24 GMT
ENV MEMCACHED_VERSION=1.6.15
# Thu, 23 Jun 2022 04:18:24 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Thu, 23 Jun 2022 04:21:07 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 23 Jun 2022 04:21:07 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 23 Jun 2022 04:21:08 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 23 Jun 2022 04:21:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jun 2022 04:21:08 GMT
USER memcache
# Thu, 23 Jun 2022 04:21:08 GMT
EXPOSE 11211
# Thu, 23 Jun 2022 04:21:08 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:b85a868b505ffd0342a37e6a3b1c49f7c71878afe569a807e6238ef08252fcb7`  
		Last Modified: Thu, 23 Jun 2022 00:25:18 GMT  
		Size: 31.4 MB (31379408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f58bb523c8de07d0d72658b2e622e82f065a1adef45f6f90f11eb7c71b9d0c61`  
		Last Modified: Thu, 23 Jun 2022 04:21:33 GMT  
		Size: 5.0 KB (4979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a458d61c2cd35b8afffe3741b04321a87f86ba216e5e2a4f9429b83b32ceb35`  
		Last Modified: Thu, 23 Jun 2022 04:21:33 GMT  
		Size: 328.1 KB (328115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7eda168e1238eaa8f5c20b7240bb8bc84c9a3f7b4b8cdc0be18f58f27bff1692`  
		Last Modified: Thu, 23 Jun 2022 04:21:33 GMT  
		Size: 1.3 MB (1255633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f188c32090c0c66f2f209fedc0778269d3edf2ad9db239ac0d2e1e3b64b36fd4`  
		Last Modified: Thu, 23 Jun 2022 04:21:33 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f492776609f9ffcbe6d066f45223bc2da677c44beb7bb0cdc6dfa34271885b34`  
		Last Modified: Thu, 23 Jun 2022 04:21:33 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:bullseye` - linux; arm variant v5

```console
$ docker pull memcached@sha256:54ff97ee8133b4181bff0e30de243b68ffa4ad0a7ecc458e6648a24760c63213
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.5 MB (30470395 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:07faffc84c650af3ec2eb3326c593cd933cba137c34c87589a375371eee849f3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 23 Jun 2022 00:50:38 GMT
ADD file:839c0e211e2260f5d54f2633e53c817c1f59e2394ba4b12f60e01e46cee61011 in / 
# Thu, 23 Jun 2022 00:50:39 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 02:41:47 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Thu, 23 Jun 2022 02:41:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 02:41:58 GMT
ENV MEMCACHED_VERSION=1.6.15
# Thu, 23 Jun 2022 02:41:59 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Thu, 23 Jun 2022 02:46:28 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 23 Jun 2022 02:46:29 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 23 Jun 2022 02:46:31 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 23 Jun 2022 02:46:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jun 2022 02:46:32 GMT
USER memcache
# Thu, 23 Jun 2022 02:46:32 GMT
EXPOSE 11211
# Thu, 23 Jun 2022 02:46:33 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:bd2d3b4056bd1b0310082fc5d17c6d03348601456c4b9306d1a333f1cec561f9`  
		Last Modified: Thu, 23 Jun 2022 01:05:39 GMT  
		Size: 28.9 MB (28921550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f500bb51d193d56af19fbeb8ebc1919ec2e6d04cf9a7d1637ad79cc00397c1b`  
		Last Modified: Thu, 23 Jun 2022 02:47:27 GMT  
		Size: 4.9 KB (4894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c3dc6e5372afc0620e0eeae739b429bee70842f20a15ca8345787a674d5d3b8`  
		Last Modified: Thu, 23 Jun 2022 02:47:28 GMT  
		Size: 316.6 KB (316616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83d6f2e7e5c2a1d3566c4d9cd05fd132529535ba7eaecb00d312c0d0a6055a4c`  
		Last Modified: Thu, 23 Jun 2022 02:47:28 GMT  
		Size: 1.2 MB (1226926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:109349836a4d5f4431660fec9744df70f92475b22644182ae9d77c8c56c8960a`  
		Last Modified: Thu, 23 Jun 2022 02:47:27 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b87ddf1818c82326658f3ca6d444b01978e23d30a7232e4ef1e0f6f0ba4ab18`  
		Last Modified: Thu, 23 Jun 2022 02:47:27 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:bullseye` - linux; arm variant v7

```console
$ docker pull memcached@sha256:b3ddbe1e7ec04512ac9e20555b72ba4b2e7e9ee99138535fabe5e92cc92302b5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.1 MB (28092007 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cbbff85100ff53c710f4caa30445e0ee79ccd0fe61cc91a522821fc5415e6bcf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 23 Jun 2022 00:59:45 GMT
ADD file:925abfb9fc0e4a7cc0c979b12c9bd2607f5c493d37b05535ca010f81beb060a9 in / 
# Thu, 23 Jun 2022 00:59:46 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 22:08:47 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Thu, 23 Jun 2022 22:08:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 22:08:56 GMT
ENV MEMCACHED_VERSION=1.6.15
# Thu, 23 Jun 2022 22:08:56 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Thu, 23 Jun 2022 22:13:04 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 23 Jun 2022 22:13:05 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 23 Jun 2022 22:13:06 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 23 Jun 2022 22:13:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jun 2022 22:13:07 GMT
USER memcache
# Thu, 23 Jun 2022 22:13:08 GMT
EXPOSE 11211
# Thu, 23 Jun 2022 22:13:08 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:d2fd562560d8062a78064adfbfa204521167c301f00f5ab3c65b9c2a54083dba`  
		Last Modified: Thu, 23 Jun 2022 01:15:22 GMT  
		Size: 26.6 MB (26576105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8864d1bfbfd3f4b781316abd42de97a2967a6b20534ffdc4fea6a3de16c1d972`  
		Last Modified: Fri, 24 Jun 2022 01:14:10 GMT  
		Size: 4.9 KB (4897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fa7c6c177f3ba693baa86ed010daf821ca2addfe7f3b8a83c7f52fac209a6e8`  
		Last Modified: Fri, 24 Jun 2022 01:14:10 GMT  
		Size: 312.1 KB (312076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f802ee5fb123a2824f3e6f93144c74f9e1c88159fc819b46f7ed2913ec61281a`  
		Last Modified: Fri, 24 Jun 2022 01:14:11 GMT  
		Size: 1.2 MB (1198521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25b61f87cd4332b040dd59bae91f0701228904433b1955bb4f51b7377db17b00`  
		Last Modified: Fri, 24 Jun 2022 01:14:10 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:532462b4f12685e2093583f1e86c82d5c2c8069b92ccbc9bbcf8efad7dfd3252`  
		Last Modified: Fri, 24 Jun 2022 01:14:10 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:bullseye` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:536f8192668e851874eec7d483055b0af220a7eb0be43010f2f9825e99ab0111
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.4 MB (31444932 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2ce58160065ec196d51dcdc756610352a57f6192b28345989be83b94b8300dec`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 23 Jun 2022 00:40:43 GMT
ADD file:134be48af13f80f3474bf1b080ca781feb7b972148d482849862e55eb2acd61c in / 
# Thu, 23 Jun 2022 00:40:44 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 03:53:19 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Thu, 23 Jun 2022 03:53:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 03:53:24 GMT
ENV MEMCACHED_VERSION=1.6.15
# Thu, 23 Jun 2022 03:53:25 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Thu, 23 Jun 2022 03:56:00 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 23 Jun 2022 03:56:02 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 23 Jun 2022 03:56:02 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 23 Jun 2022 03:56:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jun 2022 03:56:04 GMT
USER memcache
# Thu, 23 Jun 2022 03:56:05 GMT
EXPOSE 11211
# Thu, 23 Jun 2022 03:56:06 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:3b157c852f2736e12f09046f214fe5f6a0b1652bd860269b3988c92a197026e8`  
		Last Modified: Thu, 23 Jun 2022 00:47:22 GMT  
		Size: 30.1 MB (30065720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee776bb67ffbc00ca5100c88e1f7ae63b580bc131c046c3c7138b7fb796683a2`  
		Last Modified: Thu, 23 Jun 2022 03:56:51 GMT  
		Size: 4.9 KB (4904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85b234170a3d54e3ad2be2993a7e7b09550a4e00327804a183e07bc786d01bc8`  
		Last Modified: Thu, 23 Jun 2022 03:56:51 GMT  
		Size: 119.2 KB (119223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a61e7150a45b8305adc14ed47f7beb3e807a7f08223393e6f5382b043b120941`  
		Last Modified: Thu, 23 Jun 2022 03:56:51 GMT  
		Size: 1.3 MB (1254677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ed6ad1685f73da9293938d389b8c24ee8b8af4d04d4c8b502cb6082d58bf349`  
		Last Modified: Thu, 23 Jun 2022 03:56:51 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:276672cde8876c99c646defdc630e9be5ae5cfb33c192102b6387ce99d151179`  
		Last Modified: Thu, 23 Jun 2022 03:56:51 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:bullseye` - linux; 386

```console
$ docker pull memcached@sha256:651e5275f0623232ecfa476f864b6634de4e9ffc6671376c796ffd70e31c83b6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.8 MB (33778463 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31252c746c529da361fcb075711def9645866db716700e15d9e4ce92e96ed3a0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 23 Jun 2022 00:39:33 GMT
ADD file:9d46d3f8fb63833a6dbd8dd796ad541d556046a48342d22e1fd3bffa3fb8e504 in / 
# Thu, 23 Jun 2022 00:39:33 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 03:32:31 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Thu, 23 Jun 2022 03:32:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 03:32:36 GMT
ENV MEMCACHED_VERSION=1.6.15
# Thu, 23 Jun 2022 03:32:37 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Thu, 23 Jun 2022 03:35:28 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 23 Jun 2022 03:35:30 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 23 Jun 2022 03:35:30 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 23 Jun 2022 03:35:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jun 2022 03:35:32 GMT
USER memcache
# Thu, 23 Jun 2022 03:35:33 GMT
EXPOSE 11211
# Thu, 23 Jun 2022 03:35:34 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:4870b12e407743816673c11cfb39974d80c1569d876287bef61f8c585954822f`  
		Last Modified: Thu, 23 Jun 2022 00:46:40 GMT  
		Size: 32.4 MB (32390198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a67b6581e800ff3e02f41dd18cb78bc620a25becd83769f84d2c61aed5d01ea`  
		Last Modified: Thu, 23 Jun 2022 03:36:21 GMT  
		Size: 4.8 KB (4773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b70025d0ac3fc2b23b2e76f6d96c607c6a04b53c9850fe3f14fa855827b9d19d`  
		Last Modified: Thu, 23 Jun 2022 03:36:21 GMT  
		Size: 130.1 KB (130137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a383a40e44984d67c847d2a4bbc7d3525f3867ff39c81a5221970dc744ee822e`  
		Last Modified: Thu, 23 Jun 2022 03:36:21 GMT  
		Size: 1.3 MB (1252947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24f731218f56e8a5f3d250c9a4e15f841afbd92a0ee71f88761feb880aa937b3`  
		Last Modified: Thu, 23 Jun 2022 03:36:21 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15ab75a8041fc16fdde22888eb35315059264f2c153e8d05d7f132d1aa413e3a`  
		Last Modified: Thu, 23 Jun 2022 03:36:21 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:bullseye` - linux; mips64le

```console
$ docker pull memcached@sha256:71ebcf40d19139f8bab5733065ff1b2599e5d52359c6f6cbfad2104be2f1fe33
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.0 MB (31014756 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d95105805101f850723625215940d8b2be96a9b40f984174eee903985becb9e0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 23 Jun 2022 01:10:25 GMT
ADD file:fd1174cc47ac636f0cab382578a899d69ed489e4dee53ec838955e36066f526a in / 
# Thu, 23 Jun 2022 01:10:29 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 03:13:46 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Thu, 23 Jun 2022 03:14:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 03:14:06 GMT
ENV MEMCACHED_VERSION=1.6.15
# Thu, 23 Jun 2022 03:14:08 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Thu, 23 Jun 2022 03:21:07 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 23 Jun 2022 03:21:09 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 23 Jun 2022 03:21:15 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 23 Jun 2022 03:21:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jun 2022 03:21:20 GMT
USER memcache
# Thu, 23 Jun 2022 03:21:22 GMT
EXPOSE 11211
# Thu, 23 Jun 2022 03:21:25 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:9d199cb5e183b38c9edcc527cbaaa79bb56da73bd09ed449223842775ef4a244`  
		Last Modified: Thu, 23 Jun 2022 01:20:19 GMT  
		Size: 29.6 MB (29641027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d188c3e3bf643b15e2e70cc10dab71da1f4e871305c84cf6d927a2750209ee47`  
		Last Modified: Thu, 23 Jun 2022 03:21:53 GMT  
		Size: 4.9 KB (4863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8855d5fcd2d728913f5ae40b13f074576721a44abf081e6bd4e8f48e8deb8262`  
		Last Modified: Thu, 23 Jun 2022 03:21:54 GMT  
		Size: 117.2 KB (117169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:726be3b42973c4aa79e2ffcecb3633c1ec825f8099da6b5d952810bf4d1827cd`  
		Last Modified: Thu, 23 Jun 2022 03:21:54 GMT  
		Size: 1.3 MB (1251289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6176796787c17dc9b41c47c10e23979540bb32e2833c3eeceb1456f0b228166f`  
		Last Modified: Thu, 23 Jun 2022 03:21:54 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:926c03f02a771007ddd9b4fd2172ff2d89647400c4370fdedb4533a5c99e42b1`  
		Last Modified: Thu, 23 Jun 2022 03:21:53 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:bullseye` - linux; ppc64le

```console
$ docker pull memcached@sha256:0bfecd8ca43abc3e50d162ce07d6794beb5d9f98ce929e9371c2542065e6c785
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.0 MB (36972124 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ac53be686814de607770ae7fba96134fc9cd4e5afe7444779b08c02a0c92a6c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 23 Jun 2022 02:02:32 GMT
ADD file:e18c13649ea1f145047652c8e171c4824f9b6b0dbc92127a914c7fca910acf96 in / 
# Thu, 23 Jun 2022 02:02:34 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 08:15:12 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Thu, 23 Jun 2022 08:15:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 08:15:26 GMT
ENV MEMCACHED_VERSION=1.6.15
# Thu, 23 Jun 2022 08:15:30 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Thu, 23 Jun 2022 08:20:21 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 23 Jun 2022 08:20:23 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 23 Jun 2022 08:20:29 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 23 Jun 2022 08:20:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jun 2022 08:20:34 GMT
USER memcache
# Thu, 23 Jun 2022 08:20:36 GMT
EXPOSE 11211
# Thu, 23 Jun 2022 08:20:38 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:7716f0df7ba06b6f1937cd664805984e25e386a4165f2c6acc65356686e35221`  
		Last Modified: Thu, 23 Jun 2022 02:15:20 GMT  
		Size: 35.3 MB (35286823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54d7d03c3543d8cc9dbdea919601e8b8bdebdf5f54f23ee2a186edde48a4025c`  
		Last Modified: Thu, 23 Jun 2022 08:21:29 GMT  
		Size: 5.0 KB (4987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa5efdc63c420d0295d4932cc7467f1a9005b4724f592c4fba99b6c801f57810`  
		Last Modified: Thu, 23 Jun 2022 08:21:29 GMT  
		Size: 357.0 KB (356958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:329e40de463f01938ecac1d284adb38a29fde479486e279cb302d95abe9f4a16`  
		Last Modified: Thu, 23 Jun 2022 08:21:29 GMT  
		Size: 1.3 MB (1322949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d823793235eacc3363db343cea0db041905e9fde59ff5262e0fd8826e962f5a`  
		Last Modified: Thu, 23 Jun 2022 08:21:29 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2ae46dbc3324ea97ee7556a1bc8006b075f7a1492e3a2114aaf8dec7c579b76`  
		Last Modified: Thu, 23 Jun 2022 08:21:29 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:bullseye` - linux; s390x

```console
$ docker pull memcached@sha256:1e49c15efaf9999b31f526130902a04a53eeac416f40d1549e98b3fa1a872c04
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.2 MB (31226391 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b8090a3ed64f97313e1ddce878717e3bf8c1aace9d7bf247a1fa53418081f0c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 23 Jun 2022 00:43:10 GMT
ADD file:0b511e3efd87267fb27161eae56c4d08f0fed733697da6ffe6ea96a4cb68e938 in / 
# Thu, 23 Jun 2022 00:43:15 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 13:41:46 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Thu, 23 Jun 2022 13:41:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 13:41:49 GMT
ENV MEMCACHED_VERSION=1.6.15
# Thu, 23 Jun 2022 13:41:50 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Thu, 23 Jun 2022 13:45:09 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 23 Jun 2022 13:45:09 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 23 Jun 2022 13:45:10 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 23 Jun 2022 13:45:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jun 2022 13:45:10 GMT
USER memcache
# Thu, 23 Jun 2022 13:45:10 GMT
EXPOSE 11211
# Thu, 23 Jun 2022 13:45:10 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:c547f465e0c8708ad0c57cf09caa52f4c2b5b295bf10ab1ce71ca17ff81ea36a`  
		Last Modified: Thu, 23 Jun 2022 00:51:59 GMT  
		Size: 29.7 MB (29655262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04837776e7fbb579dda3720caca85ff9cb19eea15a8830ab0f23a160fa832205`  
		Last Modified: Thu, 23 Jun 2022 13:46:03 GMT  
		Size: 5.0 KB (5025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d844915fd9a66accf5106919c6a63121ed4fde412dcf958133bc1b1483b307b`  
		Last Modified: Thu, 23 Jun 2022 13:46:03 GMT  
		Size: 324.2 KB (324209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51abf5cd3f179d43b5845c7dc42a6f07ddfd6da706ca58f78d53641e3d62289f`  
		Last Modified: Thu, 23 Jun 2022 13:46:03 GMT  
		Size: 1.2 MB (1241485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31ea51fd993089ad7346961b0897d009e18b953416139bf4359ff089b9e9ada9`  
		Last Modified: Thu, 23 Jun 2022 13:46:04 GMT  
		Size: 289.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cda18e1b304fdde7d799586641bad45a035387c02b0c7e8d696e91221b046e28`  
		Last Modified: Thu, 23 Jun 2022 13:46:03 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:latest`

```console
$ docker pull memcached@sha256:b422bca20902101cd4a427ccda5ea9729a89bdc6cd8ab8a7d8cd09b1470af6b6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; s390x

### `memcached:latest` - linux; amd64

```console
$ docker pull memcached@sha256:1be4a685ac5a327ffbd7d1c7240378e7156824f9406b1eeb5fe19eadc2e61c53
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.0 MB (32968544 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a23fd759590b790a7cae87582ba4d747378de71b47e581b9295c02ce34eb9ed0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 23 Jun 2022 00:20:27 GMT
ADD file:8adbbab04d6f84cd83b5f4205b89b0acb7ecbf27a1bb2dc181d0a629479039fe in / 
# Thu, 23 Jun 2022 00:20:27 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 04:18:20 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Thu, 23 Jun 2022 04:18:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 04:18:24 GMT
ENV MEMCACHED_VERSION=1.6.15
# Thu, 23 Jun 2022 04:18:24 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Thu, 23 Jun 2022 04:21:07 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 23 Jun 2022 04:21:07 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 23 Jun 2022 04:21:08 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 23 Jun 2022 04:21:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jun 2022 04:21:08 GMT
USER memcache
# Thu, 23 Jun 2022 04:21:08 GMT
EXPOSE 11211
# Thu, 23 Jun 2022 04:21:08 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:b85a868b505ffd0342a37e6a3b1c49f7c71878afe569a807e6238ef08252fcb7`  
		Last Modified: Thu, 23 Jun 2022 00:25:18 GMT  
		Size: 31.4 MB (31379408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f58bb523c8de07d0d72658b2e622e82f065a1adef45f6f90f11eb7c71b9d0c61`  
		Last Modified: Thu, 23 Jun 2022 04:21:33 GMT  
		Size: 5.0 KB (4979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a458d61c2cd35b8afffe3741b04321a87f86ba216e5e2a4f9429b83b32ceb35`  
		Last Modified: Thu, 23 Jun 2022 04:21:33 GMT  
		Size: 328.1 KB (328115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7eda168e1238eaa8f5c20b7240bb8bc84c9a3f7b4b8cdc0be18f58f27bff1692`  
		Last Modified: Thu, 23 Jun 2022 04:21:33 GMT  
		Size: 1.3 MB (1255633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f188c32090c0c66f2f209fedc0778269d3edf2ad9db239ac0d2e1e3b64b36fd4`  
		Last Modified: Thu, 23 Jun 2022 04:21:33 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f492776609f9ffcbe6d066f45223bc2da677c44beb7bb0cdc6dfa34271885b34`  
		Last Modified: Thu, 23 Jun 2022 04:21:33 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:latest` - linux; arm variant v5

```console
$ docker pull memcached@sha256:54ff97ee8133b4181bff0e30de243b68ffa4ad0a7ecc458e6648a24760c63213
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.5 MB (30470395 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:07faffc84c650af3ec2eb3326c593cd933cba137c34c87589a375371eee849f3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 23 Jun 2022 00:50:38 GMT
ADD file:839c0e211e2260f5d54f2633e53c817c1f59e2394ba4b12f60e01e46cee61011 in / 
# Thu, 23 Jun 2022 00:50:39 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 02:41:47 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Thu, 23 Jun 2022 02:41:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 02:41:58 GMT
ENV MEMCACHED_VERSION=1.6.15
# Thu, 23 Jun 2022 02:41:59 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Thu, 23 Jun 2022 02:46:28 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 23 Jun 2022 02:46:29 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 23 Jun 2022 02:46:31 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 23 Jun 2022 02:46:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jun 2022 02:46:32 GMT
USER memcache
# Thu, 23 Jun 2022 02:46:32 GMT
EXPOSE 11211
# Thu, 23 Jun 2022 02:46:33 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:bd2d3b4056bd1b0310082fc5d17c6d03348601456c4b9306d1a333f1cec561f9`  
		Last Modified: Thu, 23 Jun 2022 01:05:39 GMT  
		Size: 28.9 MB (28921550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f500bb51d193d56af19fbeb8ebc1919ec2e6d04cf9a7d1637ad79cc00397c1b`  
		Last Modified: Thu, 23 Jun 2022 02:47:27 GMT  
		Size: 4.9 KB (4894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c3dc6e5372afc0620e0eeae739b429bee70842f20a15ca8345787a674d5d3b8`  
		Last Modified: Thu, 23 Jun 2022 02:47:28 GMT  
		Size: 316.6 KB (316616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83d6f2e7e5c2a1d3566c4d9cd05fd132529535ba7eaecb00d312c0d0a6055a4c`  
		Last Modified: Thu, 23 Jun 2022 02:47:28 GMT  
		Size: 1.2 MB (1226926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:109349836a4d5f4431660fec9744df70f92475b22644182ae9d77c8c56c8960a`  
		Last Modified: Thu, 23 Jun 2022 02:47:27 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b87ddf1818c82326658f3ca6d444b01978e23d30a7232e4ef1e0f6f0ba4ab18`  
		Last Modified: Thu, 23 Jun 2022 02:47:27 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:latest` - linux; arm variant v7

```console
$ docker pull memcached@sha256:b3ddbe1e7ec04512ac9e20555b72ba4b2e7e9ee99138535fabe5e92cc92302b5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.1 MB (28092007 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cbbff85100ff53c710f4caa30445e0ee79ccd0fe61cc91a522821fc5415e6bcf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 23 Jun 2022 00:59:45 GMT
ADD file:925abfb9fc0e4a7cc0c979b12c9bd2607f5c493d37b05535ca010f81beb060a9 in / 
# Thu, 23 Jun 2022 00:59:46 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 22:08:47 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Thu, 23 Jun 2022 22:08:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 22:08:56 GMT
ENV MEMCACHED_VERSION=1.6.15
# Thu, 23 Jun 2022 22:08:56 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Thu, 23 Jun 2022 22:13:04 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 23 Jun 2022 22:13:05 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 23 Jun 2022 22:13:06 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 23 Jun 2022 22:13:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jun 2022 22:13:07 GMT
USER memcache
# Thu, 23 Jun 2022 22:13:08 GMT
EXPOSE 11211
# Thu, 23 Jun 2022 22:13:08 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:d2fd562560d8062a78064adfbfa204521167c301f00f5ab3c65b9c2a54083dba`  
		Last Modified: Thu, 23 Jun 2022 01:15:22 GMT  
		Size: 26.6 MB (26576105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8864d1bfbfd3f4b781316abd42de97a2967a6b20534ffdc4fea6a3de16c1d972`  
		Last Modified: Fri, 24 Jun 2022 01:14:10 GMT  
		Size: 4.9 KB (4897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fa7c6c177f3ba693baa86ed010daf821ca2addfe7f3b8a83c7f52fac209a6e8`  
		Last Modified: Fri, 24 Jun 2022 01:14:10 GMT  
		Size: 312.1 KB (312076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f802ee5fb123a2824f3e6f93144c74f9e1c88159fc819b46f7ed2913ec61281a`  
		Last Modified: Fri, 24 Jun 2022 01:14:11 GMT  
		Size: 1.2 MB (1198521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25b61f87cd4332b040dd59bae91f0701228904433b1955bb4f51b7377db17b00`  
		Last Modified: Fri, 24 Jun 2022 01:14:10 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:532462b4f12685e2093583f1e86c82d5c2c8069b92ccbc9bbcf8efad7dfd3252`  
		Last Modified: Fri, 24 Jun 2022 01:14:10 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:latest` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:536f8192668e851874eec7d483055b0af220a7eb0be43010f2f9825e99ab0111
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.4 MB (31444932 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2ce58160065ec196d51dcdc756610352a57f6192b28345989be83b94b8300dec`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 23 Jun 2022 00:40:43 GMT
ADD file:134be48af13f80f3474bf1b080ca781feb7b972148d482849862e55eb2acd61c in / 
# Thu, 23 Jun 2022 00:40:44 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 03:53:19 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Thu, 23 Jun 2022 03:53:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 03:53:24 GMT
ENV MEMCACHED_VERSION=1.6.15
# Thu, 23 Jun 2022 03:53:25 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Thu, 23 Jun 2022 03:56:00 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 23 Jun 2022 03:56:02 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 23 Jun 2022 03:56:02 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 23 Jun 2022 03:56:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jun 2022 03:56:04 GMT
USER memcache
# Thu, 23 Jun 2022 03:56:05 GMT
EXPOSE 11211
# Thu, 23 Jun 2022 03:56:06 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:3b157c852f2736e12f09046f214fe5f6a0b1652bd860269b3988c92a197026e8`  
		Last Modified: Thu, 23 Jun 2022 00:47:22 GMT  
		Size: 30.1 MB (30065720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee776bb67ffbc00ca5100c88e1f7ae63b580bc131c046c3c7138b7fb796683a2`  
		Last Modified: Thu, 23 Jun 2022 03:56:51 GMT  
		Size: 4.9 KB (4904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85b234170a3d54e3ad2be2993a7e7b09550a4e00327804a183e07bc786d01bc8`  
		Last Modified: Thu, 23 Jun 2022 03:56:51 GMT  
		Size: 119.2 KB (119223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a61e7150a45b8305adc14ed47f7beb3e807a7f08223393e6f5382b043b120941`  
		Last Modified: Thu, 23 Jun 2022 03:56:51 GMT  
		Size: 1.3 MB (1254677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ed6ad1685f73da9293938d389b8c24ee8b8af4d04d4c8b502cb6082d58bf349`  
		Last Modified: Thu, 23 Jun 2022 03:56:51 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:276672cde8876c99c646defdc630e9be5ae5cfb33c192102b6387ce99d151179`  
		Last Modified: Thu, 23 Jun 2022 03:56:51 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:latest` - linux; 386

```console
$ docker pull memcached@sha256:651e5275f0623232ecfa476f864b6634de4e9ffc6671376c796ffd70e31c83b6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.8 MB (33778463 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31252c746c529da361fcb075711def9645866db716700e15d9e4ce92e96ed3a0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 23 Jun 2022 00:39:33 GMT
ADD file:9d46d3f8fb63833a6dbd8dd796ad541d556046a48342d22e1fd3bffa3fb8e504 in / 
# Thu, 23 Jun 2022 00:39:33 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 03:32:31 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Thu, 23 Jun 2022 03:32:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 03:32:36 GMT
ENV MEMCACHED_VERSION=1.6.15
# Thu, 23 Jun 2022 03:32:37 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Thu, 23 Jun 2022 03:35:28 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 23 Jun 2022 03:35:30 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 23 Jun 2022 03:35:30 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 23 Jun 2022 03:35:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jun 2022 03:35:32 GMT
USER memcache
# Thu, 23 Jun 2022 03:35:33 GMT
EXPOSE 11211
# Thu, 23 Jun 2022 03:35:34 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:4870b12e407743816673c11cfb39974d80c1569d876287bef61f8c585954822f`  
		Last Modified: Thu, 23 Jun 2022 00:46:40 GMT  
		Size: 32.4 MB (32390198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a67b6581e800ff3e02f41dd18cb78bc620a25becd83769f84d2c61aed5d01ea`  
		Last Modified: Thu, 23 Jun 2022 03:36:21 GMT  
		Size: 4.8 KB (4773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b70025d0ac3fc2b23b2e76f6d96c607c6a04b53c9850fe3f14fa855827b9d19d`  
		Last Modified: Thu, 23 Jun 2022 03:36:21 GMT  
		Size: 130.1 KB (130137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a383a40e44984d67c847d2a4bbc7d3525f3867ff39c81a5221970dc744ee822e`  
		Last Modified: Thu, 23 Jun 2022 03:36:21 GMT  
		Size: 1.3 MB (1252947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24f731218f56e8a5f3d250c9a4e15f841afbd92a0ee71f88761feb880aa937b3`  
		Last Modified: Thu, 23 Jun 2022 03:36:21 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15ab75a8041fc16fdde22888eb35315059264f2c153e8d05d7f132d1aa413e3a`  
		Last Modified: Thu, 23 Jun 2022 03:36:21 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:latest` - linux; mips64le

```console
$ docker pull memcached@sha256:71ebcf40d19139f8bab5733065ff1b2599e5d52359c6f6cbfad2104be2f1fe33
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.0 MB (31014756 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d95105805101f850723625215940d8b2be96a9b40f984174eee903985becb9e0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 23 Jun 2022 01:10:25 GMT
ADD file:fd1174cc47ac636f0cab382578a899d69ed489e4dee53ec838955e36066f526a in / 
# Thu, 23 Jun 2022 01:10:29 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 03:13:46 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Thu, 23 Jun 2022 03:14:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 03:14:06 GMT
ENV MEMCACHED_VERSION=1.6.15
# Thu, 23 Jun 2022 03:14:08 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Thu, 23 Jun 2022 03:21:07 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 23 Jun 2022 03:21:09 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 23 Jun 2022 03:21:15 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 23 Jun 2022 03:21:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jun 2022 03:21:20 GMT
USER memcache
# Thu, 23 Jun 2022 03:21:22 GMT
EXPOSE 11211
# Thu, 23 Jun 2022 03:21:25 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:9d199cb5e183b38c9edcc527cbaaa79bb56da73bd09ed449223842775ef4a244`  
		Last Modified: Thu, 23 Jun 2022 01:20:19 GMT  
		Size: 29.6 MB (29641027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d188c3e3bf643b15e2e70cc10dab71da1f4e871305c84cf6d927a2750209ee47`  
		Last Modified: Thu, 23 Jun 2022 03:21:53 GMT  
		Size: 4.9 KB (4863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8855d5fcd2d728913f5ae40b13f074576721a44abf081e6bd4e8f48e8deb8262`  
		Last Modified: Thu, 23 Jun 2022 03:21:54 GMT  
		Size: 117.2 KB (117169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:726be3b42973c4aa79e2ffcecb3633c1ec825f8099da6b5d952810bf4d1827cd`  
		Last Modified: Thu, 23 Jun 2022 03:21:54 GMT  
		Size: 1.3 MB (1251289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6176796787c17dc9b41c47c10e23979540bb32e2833c3eeceb1456f0b228166f`  
		Last Modified: Thu, 23 Jun 2022 03:21:54 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:926c03f02a771007ddd9b4fd2172ff2d89647400c4370fdedb4533a5c99e42b1`  
		Last Modified: Thu, 23 Jun 2022 03:21:53 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:latest` - linux; ppc64le

```console
$ docker pull memcached@sha256:0bfecd8ca43abc3e50d162ce07d6794beb5d9f98ce929e9371c2542065e6c785
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.0 MB (36972124 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ac53be686814de607770ae7fba96134fc9cd4e5afe7444779b08c02a0c92a6c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 23 Jun 2022 02:02:32 GMT
ADD file:e18c13649ea1f145047652c8e171c4824f9b6b0dbc92127a914c7fca910acf96 in / 
# Thu, 23 Jun 2022 02:02:34 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 08:15:12 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Thu, 23 Jun 2022 08:15:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 08:15:26 GMT
ENV MEMCACHED_VERSION=1.6.15
# Thu, 23 Jun 2022 08:15:30 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Thu, 23 Jun 2022 08:20:21 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 23 Jun 2022 08:20:23 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 23 Jun 2022 08:20:29 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 23 Jun 2022 08:20:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jun 2022 08:20:34 GMT
USER memcache
# Thu, 23 Jun 2022 08:20:36 GMT
EXPOSE 11211
# Thu, 23 Jun 2022 08:20:38 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:7716f0df7ba06b6f1937cd664805984e25e386a4165f2c6acc65356686e35221`  
		Last Modified: Thu, 23 Jun 2022 02:15:20 GMT  
		Size: 35.3 MB (35286823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54d7d03c3543d8cc9dbdea919601e8b8bdebdf5f54f23ee2a186edde48a4025c`  
		Last Modified: Thu, 23 Jun 2022 08:21:29 GMT  
		Size: 5.0 KB (4987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa5efdc63c420d0295d4932cc7467f1a9005b4724f592c4fba99b6c801f57810`  
		Last Modified: Thu, 23 Jun 2022 08:21:29 GMT  
		Size: 357.0 KB (356958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:329e40de463f01938ecac1d284adb38a29fde479486e279cb302d95abe9f4a16`  
		Last Modified: Thu, 23 Jun 2022 08:21:29 GMT  
		Size: 1.3 MB (1322949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d823793235eacc3363db343cea0db041905e9fde59ff5262e0fd8826e962f5a`  
		Last Modified: Thu, 23 Jun 2022 08:21:29 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2ae46dbc3324ea97ee7556a1bc8006b075f7a1492e3a2114aaf8dec7c579b76`  
		Last Modified: Thu, 23 Jun 2022 08:21:29 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:latest` - linux; s390x

```console
$ docker pull memcached@sha256:1e49c15efaf9999b31f526130902a04a53eeac416f40d1549e98b3fa1a872c04
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.2 MB (31226391 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b8090a3ed64f97313e1ddce878717e3bf8c1aace9d7bf247a1fa53418081f0c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 23 Jun 2022 00:43:10 GMT
ADD file:0b511e3efd87267fb27161eae56c4d08f0fed733697da6ffe6ea96a4cb68e938 in / 
# Thu, 23 Jun 2022 00:43:15 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 13:41:46 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Thu, 23 Jun 2022 13:41:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 13:41:49 GMT
ENV MEMCACHED_VERSION=1.6.15
# Thu, 23 Jun 2022 13:41:50 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Thu, 23 Jun 2022 13:45:09 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 23 Jun 2022 13:45:09 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 23 Jun 2022 13:45:10 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 23 Jun 2022 13:45:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jun 2022 13:45:10 GMT
USER memcache
# Thu, 23 Jun 2022 13:45:10 GMT
EXPOSE 11211
# Thu, 23 Jun 2022 13:45:10 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:c547f465e0c8708ad0c57cf09caa52f4c2b5b295bf10ab1ce71ca17ff81ea36a`  
		Last Modified: Thu, 23 Jun 2022 00:51:59 GMT  
		Size: 29.7 MB (29655262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04837776e7fbb579dda3720caca85ff9cb19eea15a8830ab0f23a160fa832205`  
		Last Modified: Thu, 23 Jun 2022 13:46:03 GMT  
		Size: 5.0 KB (5025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d844915fd9a66accf5106919c6a63121ed4fde412dcf958133bc1b1483b307b`  
		Last Modified: Thu, 23 Jun 2022 13:46:03 GMT  
		Size: 324.2 KB (324209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51abf5cd3f179d43b5845c7dc42a6f07ddfd6da706ca58f78d53641e3d62289f`  
		Last Modified: Thu, 23 Jun 2022 13:46:03 GMT  
		Size: 1.2 MB (1241485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31ea51fd993089ad7346961b0897d009e18b953416139bf4359ff089b9e9ada9`  
		Last Modified: Thu, 23 Jun 2022 13:46:04 GMT  
		Size: 289.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cda18e1b304fdde7d799586641bad45a035387c02b0c7e8d696e91221b046e28`  
		Last Modified: Thu, 23 Jun 2022 13:46:03 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
