<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `memcached`

-	[`memcached:1`](#memcached1)
-	[`memcached:1-alpine`](#memcached1-alpine)
-	[`memcached:1-alpine3.15`](#memcached1-alpine315)
-	[`memcached:1-bullseye`](#memcached1-bullseye)
-	[`memcached:1.6`](#memcached16)
-	[`memcached:1.6-alpine`](#memcached16-alpine)
-	[`memcached:1.6-alpine3.15`](#memcached16-alpine315)
-	[`memcached:1.6-bullseye`](#memcached16-bullseye)
-	[`memcached:1.6.13`](#memcached1613)
-	[`memcached:1.6.13-alpine`](#memcached1613-alpine)
-	[`memcached:1.6.13-alpine3.15`](#memcached1613-alpine315)
-	[`memcached:1.6.13-bullseye`](#memcached1613-bullseye)
-	[`memcached:alpine`](#memcachedalpine)
-	[`memcached:alpine3.15`](#memcachedalpine315)
-	[`memcached:bullseye`](#memcachedbullseye)
-	[`memcached:latest`](#memcachedlatest)

## `memcached:1`

```console
$ docker pull memcached@sha256:61a8c3887d91c23aa6ce62b145b6e77acb1bcf195e950b3971f4007f2a47fa12
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
$ docker pull memcached@sha256:c9756ec03bedf0411e142fa016cce653157ef46216102b2ad9012ba57a69e9b5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.9 MB (32945941 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c8b63b0eeb514dca60290d594b69ba36d42534eb7c4af27ceb25c4b900d862c8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 21 Dec 2021 01:22:43 GMT
ADD file:09675d11695f65c55efdc393ff0cd32f30194cd7d0fbef4631eebfed4414ac97 in / 
# Tue, 21 Dec 2021 01:22:43 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 18:34:30 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 21 Dec 2021 18:34:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 20 Jan 2022 04:23:06 GMT
ENV MEMCACHED_VERSION=1.6.13
# Thu, 20 Jan 2022 04:23:06 GMT
ENV MEMCACHED_SHA1=b9da57ba63ba8de8a980fe0fe2fedc8d59e1dfe3
# Thu, 20 Jan 2022 04:27:08 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 20 Jan 2022 04:27:08 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 20 Jan 2022 04:27:09 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 20 Jan 2022 04:27:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 20 Jan 2022 04:27:09 GMT
USER memcache
# Thu, 20 Jan 2022 04:27:10 GMT
EXPOSE 11211
# Thu, 20 Jan 2022 04:27:10 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:a2abf6c4d29d43a4bf9fbb769f524d0fb36a2edab49819c1bf3e76f409f953ea`  
		Last Modified: Tue, 21 Dec 2021 01:27:48 GMT  
		Size: 31.4 MB (31357624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aa5be68e24cfc338b0c9be41213371a3ed596d00487ad58df6494ed46626117`  
		Last Modified: Tue, 21 Dec 2021 18:39:12 GMT  
		Size: 5.0 KB (4978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:052b406b20ce6593c7a47bc0d4d4f8b45258c1aed8b86ab06c0fc75ab6b4ee40`  
		Last Modified: Tue, 21 Dec 2021 18:39:13 GMT  
		Size: 328.1 KB (328055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b89359883409361f4bb025aaae623b73503a2801842fa3ceda2711924cf71b5`  
		Last Modified: Thu, 20 Jan 2022 04:31:55 GMT  
		Size: 1.3 MB (1254875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f5e296124091603e6ac2227e0bb1a6cde6faafa7608b926488a5d003b20d987`  
		Last Modified: Thu, 20 Jan 2022 04:31:54 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d7a956a84f556974daee7c5e1010bfa31d093c5b8b5eaabffa21a4931fe48f7`  
		Last Modified: Thu, 20 Jan 2022 04:31:54 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1` - linux; arm variant v5

```console
$ docker pull memcached@sha256:d16a2790a88e4662d8340cb85a9660f7738b5abbe759bad21b8f676e0ca8312c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.4 MB (30447722 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7768dab3ed87264de0f4e8a613c070301197408077835da74c7faae6eb6f4bd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 21 Dec 2021 01:50:31 GMT
ADD file:a3023f71bd93966e7db1419adda3ccde4fcc5e2e8cf58e7b13c51036ed5ff796 in / 
# Tue, 21 Dec 2021 01:50:32 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 03:35:35 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 21 Dec 2021 03:35:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 19 Jan 2022 23:48:42 GMT
ENV MEMCACHED_VERSION=1.6.13
# Wed, 19 Jan 2022 23:48:43 GMT
ENV MEMCACHED_SHA1=b9da57ba63ba8de8a980fe0fe2fedc8d59e1dfe3
# Wed, 19 Jan 2022 23:54:08 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 19 Jan 2022 23:54:09 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 19 Jan 2022 23:54:13 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 19 Jan 2022 23:54:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 19 Jan 2022 23:54:14 GMT
USER memcache
# Wed, 19 Jan 2022 23:54:15 GMT
EXPOSE 11211
# Wed, 19 Jan 2022 23:54:16 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:054429d0cf4038fef39a3b5eb6ce52f600f9a2cbb71a4fb3e95ecf9b2da62581`  
		Last Modified: Tue, 21 Dec 2021 02:05:52 GMT  
		Size: 28.9 MB (28900253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb7fdf670368bfde88ac158623eeda4b36ce64bd838e78a9ffcd3d2622eea2e8`  
		Last Modified: Tue, 21 Dec 2021 03:41:18 GMT  
		Size: 4.9 KB (4893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21508b31a1593117f5747b299da29b6bec5fb36f008effcd821336ebafc8ad70`  
		Last Modified: Tue, 21 Dec 2021 03:41:18 GMT  
		Size: 316.6 KB (316576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6d782b9d573913a26c43aba467d4fed6b33af9b83f44cfb1e8f63a76f92ab3a`  
		Last Modified: Wed, 19 Jan 2022 23:55:13 GMT  
		Size: 1.2 MB (1225592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b184c6b4181672a28be507397bd5d2baad8db49549bba6940adb30ce28c3320`  
		Last Modified: Wed, 19 Jan 2022 23:55:12 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73e44f9f60691acb75f8287e5a5eaa0675e04ffbc1fa1e4abfe57733ca7aa595`  
		Last Modified: Wed, 19 Jan 2022 23:55:12 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1` - linux; arm variant v7

```console
$ docker pull memcached@sha256:7f4a3e4bd6d3845da89e6e1fa7ee377f050118bd20803a8716e7c8aab31670ee
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.1 MB (28078674 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d0493346f5301d1fac3c1ee8eb4df2a8f1791ec73c16d2425aa56be76aabae7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:08 GMT
ADD file:7f27f5b43b7cb04e509fe145266d9bdeacfcacb024cafac32e57ef1c831d5ea7 in / 
# Wed, 26 Jan 2022 01:42:09 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 08:54:44 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 26 Jan 2022 08:54:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 08:54:52 GMT
ENV MEMCACHED_VERSION=1.6.13
# Wed, 26 Jan 2022 08:54:52 GMT
ENV MEMCACHED_SHA1=b9da57ba63ba8de8a980fe0fe2fedc8d59e1dfe3
# Wed, 26 Jan 2022 08:59:15 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 26 Jan 2022 08:59:16 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 26 Jan 2022 08:59:18 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 26 Jan 2022 08:59:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Jan 2022 08:59:18 GMT
USER memcache
# Wed, 26 Jan 2022 08:59:19 GMT
EXPOSE 11211
# Wed, 26 Jan 2022 08:59:19 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:aaef1f1162ec03e01b5b955d41da400544ec2374093ae3dbc330ab2bb36df3e1`  
		Last Modified: Wed, 26 Jan 2022 01:57:59 GMT  
		Size: 26.6 MB (26564933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c9d3dbbb6d5b3a74ea3807c462c99fc02f7ef46831734a98ab085fbfd45d84c`  
		Last Modified: Wed, 26 Jan 2022 09:13:01 GMT  
		Size: 4.9 KB (4894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c553a44b8d98c757ba52201bd5897c9b84bed862d1f1a33b30eaee164faf002`  
		Last Modified: Wed, 26 Jan 2022 09:13:02 GMT  
		Size: 312.0 KB (312023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e05d6d11f4c98f66add6994ad62c7fe25432ba441f2618ba25e8d572c66fe89`  
		Last Modified: Wed, 26 Jan 2022 09:13:02 GMT  
		Size: 1.2 MB (1196416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:902b4740d93b1e9cdd39f484a29d2e022801b8f4612ddd6471c63d0d5aee77c7`  
		Last Modified: Wed, 26 Jan 2022 09:13:01 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0813f5460d7241e77461d216cec438321996a8a74a205fd5a63e3a6e7300ec08`  
		Last Modified: Wed, 26 Jan 2022 09:13:01 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:97cdec366a180179780e13eb6ab3b4839bd7ce753737ed9b69c45d5baf9d55e0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.4 MB (31434947 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9182bae18682935ee16f416121710ff59a5021e8148d558c7df06caa35e422c5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:31 GMT
ADD file:0ec6f47a8857bf8e6cef71ed8f864be7ce1790ff6ed04fd4201e7dbde4728d3a in / 
# Wed, 26 Jan 2022 01:42:31 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 04:50:24 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 26 Jan 2022 04:50:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 04:50:28 GMT
ENV MEMCACHED_VERSION=1.6.13
# Wed, 26 Jan 2022 04:50:29 GMT
ENV MEMCACHED_SHA1=b9da57ba63ba8de8a980fe0fe2fedc8d59e1dfe3
# Wed, 26 Jan 2022 04:53:09 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 26 Jan 2022 04:53:10 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 26 Jan 2022 04:53:10 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 26 Jan 2022 04:53:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Jan 2022 04:53:12 GMT
USER memcache
# Wed, 26 Jan 2022 04:53:13 GMT
EXPOSE 11211
# Wed, 26 Jan 2022 04:53:14 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:8998bd30e6a1204d13403045766edbe14f941b52087465f5d140ab63c8b113bf`  
		Last Modified: Wed, 26 Jan 2022 01:49:04 GMT  
		Size: 30.1 MB (30056774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a59fc24ed29770b5c2f4352a96e8a82fa286fa87df96964968e2fb2796e105ac`  
		Last Modified: Wed, 26 Jan 2022 04:53:58 GMT  
		Size: 4.9 KB (4900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54853adf97755cd00bf2b960a7a7458bfc9824d4847b0f97e7e5f41e86b6c351`  
		Last Modified: Wed, 26 Jan 2022 04:53:59 GMT  
		Size: 119.2 KB (119210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bc43135274188258180f193f3f9907dd72b6b09963f1886610f28977741356a`  
		Last Modified: Wed, 26 Jan 2022 04:53:59 GMT  
		Size: 1.3 MB (1253657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e306557d5e40e37e762e103bd520b6153919316e8d64e4ae3d21fa66d6420f3`  
		Last Modified: Wed, 26 Jan 2022 04:53:59 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86f1b169766c42ff4dabdf96ef26f2207f4f9fa4fdf13b53c3625a106c50ca12`  
		Last Modified: Wed, 26 Jan 2022 04:53:58 GMT  
		Size: 120.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1` - linux; 386

```console
$ docker pull memcached@sha256:caebaf527ba0576d76c6d7579c1c921d78dcd0522d3dbe11a11c5ebc1c05b37b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.0 MB (33971560 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f0d964750c0182cb6e1376d8eec8982b36ab1b3aa6f8ab59919f116da2625871`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 26 Jan 2022 01:39:55 GMT
ADD file:876ebf07c65841f4840842086c883af48e07386964fe6d643ba193895ec2a582 in / 
# Wed, 26 Jan 2022 01:39:56 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 08:45:04 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 26 Jan 2022 08:45:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 08:45:09 GMT
ENV MEMCACHED_VERSION=1.6.13
# Wed, 26 Jan 2022 08:45:09 GMT
ENV MEMCACHED_SHA1=b9da57ba63ba8de8a980fe0fe2fedc8d59e1dfe3
# Wed, 26 Jan 2022 08:49:29 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 26 Jan 2022 08:49:29 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 26 Jan 2022 08:49:30 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 26 Jan 2022 08:49:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Jan 2022 08:49:31 GMT
USER memcache
# Wed, 26 Jan 2022 08:49:31 GMT
EXPOSE 11211
# Wed, 26 Jan 2022 08:49:31 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:86933886b1754aba091548cf031a9bca88cdce9bb4fc1f28bb38b61594c2c2c7`  
		Last Modified: Wed, 26 Jan 2022 01:48:57 GMT  
		Size: 32.4 MB (32377406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84bd6e2dff27e256b3baec641bd7c64e8a138237c2c259a806d0f9a9fb1d2255`  
		Last Modified: Wed, 26 Jan 2022 08:50:25 GMT  
		Size: 4.9 KB (4896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d8c7dc83b8d6601d80421931237cbfcd968616d9910fad6f78ee1706ee8f1e3`  
		Last Modified: Wed, 26 Jan 2022 08:50:26 GMT  
		Size: 336.6 KB (336627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5e3e4cf9c8423bfa3e769914fdcf235f6b64837f5fb62f5ccc09a8d792a268c`  
		Last Modified: Wed, 26 Jan 2022 08:50:26 GMT  
		Size: 1.3 MB (1252223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6402d600344325d49706165f2b0feec85cd2421776889433e4c45230bc89b7ee`  
		Last Modified: Wed, 26 Jan 2022 08:50:25 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9fa9c73a03d6ce53a9ea22b31db2648aa6a02a1779ae0a5b19070fbbe806125`  
		Last Modified: Wed, 26 Jan 2022 08:50:25 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1` - linux; mips64le

```console
$ docker pull memcached@sha256:0848c96207329a581151eeefb1a2b5f1c13893e01667962c71ed108ba448ec8a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.2 MB (31212144 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5691adbb93dbe11492ece526682692fc23ae3869ddd09a5cc20fc92abe25fa68`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:45 GMT
ADD file:61767027a5ab46afbcd4079d200abe8d663326adc96fa28ca8c8955a06d9322e in / 
# Wed, 26 Jan 2022 01:42:46 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 04:16:54 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 26 Jan 2022 04:17:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 04:17:06 GMT
ENV MEMCACHED_VERSION=1.6.13
# Wed, 26 Jan 2022 04:17:07 GMT
ENV MEMCACHED_SHA1=b9da57ba63ba8de8a980fe0fe2fedc8d59e1dfe3
# Wed, 26 Jan 2022 04:23:00 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 26 Jan 2022 04:23:00 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 26 Jan 2022 04:23:02 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 26 Jan 2022 04:23:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Jan 2022 04:23:03 GMT
USER memcache
# Wed, 26 Jan 2022 04:23:03 GMT
EXPOSE 11211
# Wed, 26 Jan 2022 04:23:03 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:266e7d2b59483859eaa1711d2afeb25ea4458eeb36b3e909372930db1f834d7f`  
		Last Modified: Wed, 26 Jan 2022 01:51:23 GMT  
		Size: 29.6 MB (29632834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f2c23d84e18c59799194289c3354e30ed9e147411beb83fd8a53a6b0510244e`  
		Last Modified: Wed, 26 Jan 2022 04:23:22 GMT  
		Size: 5.0 KB (4977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e72e725e4f6fb1ddea7af05f25646fbd5f401583a994d00e98f8d9762bdeef1`  
		Last Modified: Wed, 26 Jan 2022 04:23:22 GMT  
		Size: 323.7 KB (323700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a64f2bbfc21569385827a44c22dc4d96a9004879a3db5a479ac796150f31a89`  
		Last Modified: Wed, 26 Jan 2022 04:23:23 GMT  
		Size: 1.3 MB (1250226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10ec607308395a4822bcdf6d4c2f8665284150145ceaee889026d63b5bbfc525`  
		Last Modified: Wed, 26 Jan 2022 04:23:22 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0544419df418d0761bfd4cee74e348f336fd813c7d70a2ba0f9c66dd4dcad99`  
		Last Modified: Wed, 26 Jan 2022 04:23:22 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1` - linux; ppc64le

```console
$ docker pull memcached@sha256:467baa60d3118dac94a8d1909db41ec8f8e0867581bba86e83d70d2843299d95
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.0 MB (36956955 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89c206a82af6419284433a55b65259fb3c41ae73d206fc37aa006d7c30d22d0e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 26 Jan 2022 01:46:51 GMT
ADD file:c03f34c221e57fa5cb625c166d1db9f72d6ba2fa17a3c41a5d04d6875d098949 in / 
# Wed, 26 Jan 2022 01:46:57 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 05:38:39 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 26 Jan 2022 05:38:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 05:38:55 GMT
ENV MEMCACHED_VERSION=1.6.13
# Wed, 26 Jan 2022 05:38:58 GMT
ENV MEMCACHED_SHA1=b9da57ba63ba8de8a980fe0fe2fedc8d59e1dfe3
# Wed, 26 Jan 2022 05:44:08 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 26 Jan 2022 05:44:10 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 26 Jan 2022 05:44:17 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 26 Jan 2022 05:44:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Jan 2022 05:44:24 GMT
USER memcache
# Wed, 26 Jan 2022 05:44:28 GMT
EXPOSE 11211
# Wed, 26 Jan 2022 05:44:32 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:3149ee4a73508a4c39107d64a3fdc1b021626a22a0ac95e62fa0cea49ab77fba`  
		Last Modified: Wed, 26 Jan 2022 01:57:01 GMT  
		Size: 35.3 MB (35273030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07bcb451658eb6d9eace467c2e989d96e53c409eb48347a369e9ad80aadcfe96`  
		Last Modified: Wed, 26 Jan 2022 05:45:22 GMT  
		Size: 5.0 KB (4980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8807782e060aa90873de57b2d3ec277632145f166e9c1e3801c57eea7e595cc`  
		Last Modified: Wed, 26 Jan 2022 05:45:22 GMT  
		Size: 356.9 KB (356905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9214a40cf25dcbbc1d21f60a5512d485bc08156423100a0bb814946e829e3a0e`  
		Last Modified: Wed, 26 Jan 2022 05:45:22 GMT  
		Size: 1.3 MB (1321633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90ee2e08d849858def804d36f370ce894ef499543f6e8a72b9aac42c9e1cc909`  
		Last Modified: Wed, 26 Jan 2022 05:45:22 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6635b7a8817986bc0e4c179ae7d01d924f3017618b34956074b196886d9aaa67`  
		Last Modified: Wed, 26 Jan 2022 05:45:22 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1` - linux; s390x

```console
$ docker pull memcached@sha256:0f830716b97909822e4fe0394e7907f03695936767866c5e3dde96f89f483b30
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.2 MB (31216717 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e41587da3718a95304af17c726b656832260d3107e24f7811d54a20c5bad539`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 26 Jan 2022 01:41:13 GMT
ADD file:03b224b82f458b08d3b5071e42b67915a3db309332c0fc9229db7cf1148bc1b5 in / 
# Wed, 26 Jan 2022 01:41:15 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 03:32:44 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 26 Jan 2022 03:32:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 03:32:47 GMT
ENV MEMCACHED_VERSION=1.6.13
# Wed, 26 Jan 2022 03:32:48 GMT
ENV MEMCACHED_SHA1=b9da57ba63ba8de8a980fe0fe2fedc8d59e1dfe3
# Wed, 26 Jan 2022 03:36:16 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 26 Jan 2022 03:36:16 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 26 Jan 2022 03:36:16 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 26 Jan 2022 03:36:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Jan 2022 03:36:17 GMT
USER memcache
# Wed, 26 Jan 2022 03:36:17 GMT
EXPOSE 11211
# Wed, 26 Jan 2022 03:36:17 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:70bed29526f8483937e4d2540d19256d30786007c7c321e717e00d2e74700380`  
		Last Modified: Wed, 26 Jan 2022 01:46:57 GMT  
		Size: 29.6 MB (29647071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:531e195eaaf208f50aadc4ec839bd3a8f8d4bb0a35dea07bb0e27335fcf6db05`  
		Last Modified: Wed, 26 Jan 2022 03:37:15 GMT  
		Size: 5.0 KB (5026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1072031f118cfb7a6e47244d0bc6a66ac9a2cd286044b62e34033f655f0166d`  
		Last Modified: Wed, 26 Jan 2022 03:37:16 GMT  
		Size: 324.1 KB (324144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3719ec4f04cc9c989d6e8fb755b61510a0e78a3d35107b06cfc6c109c5aac17d`  
		Last Modified: Wed, 26 Jan 2022 03:37:16 GMT  
		Size: 1.2 MB (1240067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c8553e94280409bcb797ba67589732c286468e57828ea58da8d393d5b25a881`  
		Last Modified: Wed, 26 Jan 2022 03:37:16 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de608eaa9aaa185e5049d6baf7896898fe3d2c6beef1fcac73855ec782e15eee`  
		Last Modified: Wed, 26 Jan 2022 03:37:16 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:1-alpine`

```console
$ docker pull memcached@sha256:4fd74bfdda3c109c25e7edfd6b77545c48963b938d6f75f4fb8c122c5cdae7cd
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

### `memcached:1-alpine` - linux; 386

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

### `memcached:1-alpine` - linux; ppc64le

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

### `memcached:1-alpine` - linux; s390x

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

## `memcached:1-bullseye`

```console
$ docker pull memcached@sha256:61a8c3887d91c23aa6ce62b145b6e77acb1bcf195e950b3971f4007f2a47fa12
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
$ docker pull memcached@sha256:c9756ec03bedf0411e142fa016cce653157ef46216102b2ad9012ba57a69e9b5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.9 MB (32945941 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c8b63b0eeb514dca60290d594b69ba36d42534eb7c4af27ceb25c4b900d862c8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 21 Dec 2021 01:22:43 GMT
ADD file:09675d11695f65c55efdc393ff0cd32f30194cd7d0fbef4631eebfed4414ac97 in / 
# Tue, 21 Dec 2021 01:22:43 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 18:34:30 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 21 Dec 2021 18:34:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 20 Jan 2022 04:23:06 GMT
ENV MEMCACHED_VERSION=1.6.13
# Thu, 20 Jan 2022 04:23:06 GMT
ENV MEMCACHED_SHA1=b9da57ba63ba8de8a980fe0fe2fedc8d59e1dfe3
# Thu, 20 Jan 2022 04:27:08 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 20 Jan 2022 04:27:08 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 20 Jan 2022 04:27:09 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 20 Jan 2022 04:27:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 20 Jan 2022 04:27:09 GMT
USER memcache
# Thu, 20 Jan 2022 04:27:10 GMT
EXPOSE 11211
# Thu, 20 Jan 2022 04:27:10 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:a2abf6c4d29d43a4bf9fbb769f524d0fb36a2edab49819c1bf3e76f409f953ea`  
		Last Modified: Tue, 21 Dec 2021 01:27:48 GMT  
		Size: 31.4 MB (31357624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aa5be68e24cfc338b0c9be41213371a3ed596d00487ad58df6494ed46626117`  
		Last Modified: Tue, 21 Dec 2021 18:39:12 GMT  
		Size: 5.0 KB (4978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:052b406b20ce6593c7a47bc0d4d4f8b45258c1aed8b86ab06c0fc75ab6b4ee40`  
		Last Modified: Tue, 21 Dec 2021 18:39:13 GMT  
		Size: 328.1 KB (328055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b89359883409361f4bb025aaae623b73503a2801842fa3ceda2711924cf71b5`  
		Last Modified: Thu, 20 Jan 2022 04:31:55 GMT  
		Size: 1.3 MB (1254875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f5e296124091603e6ac2227e0bb1a6cde6faafa7608b926488a5d003b20d987`  
		Last Modified: Thu, 20 Jan 2022 04:31:54 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d7a956a84f556974daee7c5e1010bfa31d093c5b8b5eaabffa21a4931fe48f7`  
		Last Modified: Thu, 20 Jan 2022 04:31:54 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-bullseye` - linux; arm variant v5

```console
$ docker pull memcached@sha256:d16a2790a88e4662d8340cb85a9660f7738b5abbe759bad21b8f676e0ca8312c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.4 MB (30447722 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7768dab3ed87264de0f4e8a613c070301197408077835da74c7faae6eb6f4bd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 21 Dec 2021 01:50:31 GMT
ADD file:a3023f71bd93966e7db1419adda3ccde4fcc5e2e8cf58e7b13c51036ed5ff796 in / 
# Tue, 21 Dec 2021 01:50:32 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 03:35:35 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 21 Dec 2021 03:35:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 19 Jan 2022 23:48:42 GMT
ENV MEMCACHED_VERSION=1.6.13
# Wed, 19 Jan 2022 23:48:43 GMT
ENV MEMCACHED_SHA1=b9da57ba63ba8de8a980fe0fe2fedc8d59e1dfe3
# Wed, 19 Jan 2022 23:54:08 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 19 Jan 2022 23:54:09 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 19 Jan 2022 23:54:13 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 19 Jan 2022 23:54:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 19 Jan 2022 23:54:14 GMT
USER memcache
# Wed, 19 Jan 2022 23:54:15 GMT
EXPOSE 11211
# Wed, 19 Jan 2022 23:54:16 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:054429d0cf4038fef39a3b5eb6ce52f600f9a2cbb71a4fb3e95ecf9b2da62581`  
		Last Modified: Tue, 21 Dec 2021 02:05:52 GMT  
		Size: 28.9 MB (28900253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb7fdf670368bfde88ac158623eeda4b36ce64bd838e78a9ffcd3d2622eea2e8`  
		Last Modified: Tue, 21 Dec 2021 03:41:18 GMT  
		Size: 4.9 KB (4893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21508b31a1593117f5747b299da29b6bec5fb36f008effcd821336ebafc8ad70`  
		Last Modified: Tue, 21 Dec 2021 03:41:18 GMT  
		Size: 316.6 KB (316576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6d782b9d573913a26c43aba467d4fed6b33af9b83f44cfb1e8f63a76f92ab3a`  
		Last Modified: Wed, 19 Jan 2022 23:55:13 GMT  
		Size: 1.2 MB (1225592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b184c6b4181672a28be507397bd5d2baad8db49549bba6940adb30ce28c3320`  
		Last Modified: Wed, 19 Jan 2022 23:55:12 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73e44f9f60691acb75f8287e5a5eaa0675e04ffbc1fa1e4abfe57733ca7aa595`  
		Last Modified: Wed, 19 Jan 2022 23:55:12 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-bullseye` - linux; arm variant v7

```console
$ docker pull memcached@sha256:7f4a3e4bd6d3845da89e6e1fa7ee377f050118bd20803a8716e7c8aab31670ee
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.1 MB (28078674 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d0493346f5301d1fac3c1ee8eb4df2a8f1791ec73c16d2425aa56be76aabae7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:08 GMT
ADD file:7f27f5b43b7cb04e509fe145266d9bdeacfcacb024cafac32e57ef1c831d5ea7 in / 
# Wed, 26 Jan 2022 01:42:09 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 08:54:44 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 26 Jan 2022 08:54:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 08:54:52 GMT
ENV MEMCACHED_VERSION=1.6.13
# Wed, 26 Jan 2022 08:54:52 GMT
ENV MEMCACHED_SHA1=b9da57ba63ba8de8a980fe0fe2fedc8d59e1dfe3
# Wed, 26 Jan 2022 08:59:15 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 26 Jan 2022 08:59:16 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 26 Jan 2022 08:59:18 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 26 Jan 2022 08:59:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Jan 2022 08:59:18 GMT
USER memcache
# Wed, 26 Jan 2022 08:59:19 GMT
EXPOSE 11211
# Wed, 26 Jan 2022 08:59:19 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:aaef1f1162ec03e01b5b955d41da400544ec2374093ae3dbc330ab2bb36df3e1`  
		Last Modified: Wed, 26 Jan 2022 01:57:59 GMT  
		Size: 26.6 MB (26564933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c9d3dbbb6d5b3a74ea3807c462c99fc02f7ef46831734a98ab085fbfd45d84c`  
		Last Modified: Wed, 26 Jan 2022 09:13:01 GMT  
		Size: 4.9 KB (4894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c553a44b8d98c757ba52201bd5897c9b84bed862d1f1a33b30eaee164faf002`  
		Last Modified: Wed, 26 Jan 2022 09:13:02 GMT  
		Size: 312.0 KB (312023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e05d6d11f4c98f66add6994ad62c7fe25432ba441f2618ba25e8d572c66fe89`  
		Last Modified: Wed, 26 Jan 2022 09:13:02 GMT  
		Size: 1.2 MB (1196416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:902b4740d93b1e9cdd39f484a29d2e022801b8f4612ddd6471c63d0d5aee77c7`  
		Last Modified: Wed, 26 Jan 2022 09:13:01 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0813f5460d7241e77461d216cec438321996a8a74a205fd5a63e3a6e7300ec08`  
		Last Modified: Wed, 26 Jan 2022 09:13:01 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-bullseye` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:97cdec366a180179780e13eb6ab3b4839bd7ce753737ed9b69c45d5baf9d55e0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.4 MB (31434947 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9182bae18682935ee16f416121710ff59a5021e8148d558c7df06caa35e422c5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:31 GMT
ADD file:0ec6f47a8857bf8e6cef71ed8f864be7ce1790ff6ed04fd4201e7dbde4728d3a in / 
# Wed, 26 Jan 2022 01:42:31 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 04:50:24 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 26 Jan 2022 04:50:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 04:50:28 GMT
ENV MEMCACHED_VERSION=1.6.13
# Wed, 26 Jan 2022 04:50:29 GMT
ENV MEMCACHED_SHA1=b9da57ba63ba8de8a980fe0fe2fedc8d59e1dfe3
# Wed, 26 Jan 2022 04:53:09 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 26 Jan 2022 04:53:10 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 26 Jan 2022 04:53:10 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 26 Jan 2022 04:53:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Jan 2022 04:53:12 GMT
USER memcache
# Wed, 26 Jan 2022 04:53:13 GMT
EXPOSE 11211
# Wed, 26 Jan 2022 04:53:14 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:8998bd30e6a1204d13403045766edbe14f941b52087465f5d140ab63c8b113bf`  
		Last Modified: Wed, 26 Jan 2022 01:49:04 GMT  
		Size: 30.1 MB (30056774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a59fc24ed29770b5c2f4352a96e8a82fa286fa87df96964968e2fb2796e105ac`  
		Last Modified: Wed, 26 Jan 2022 04:53:58 GMT  
		Size: 4.9 KB (4900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54853adf97755cd00bf2b960a7a7458bfc9824d4847b0f97e7e5f41e86b6c351`  
		Last Modified: Wed, 26 Jan 2022 04:53:59 GMT  
		Size: 119.2 KB (119210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bc43135274188258180f193f3f9907dd72b6b09963f1886610f28977741356a`  
		Last Modified: Wed, 26 Jan 2022 04:53:59 GMT  
		Size: 1.3 MB (1253657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e306557d5e40e37e762e103bd520b6153919316e8d64e4ae3d21fa66d6420f3`  
		Last Modified: Wed, 26 Jan 2022 04:53:59 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86f1b169766c42ff4dabdf96ef26f2207f4f9fa4fdf13b53c3625a106c50ca12`  
		Last Modified: Wed, 26 Jan 2022 04:53:58 GMT  
		Size: 120.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-bullseye` - linux; 386

```console
$ docker pull memcached@sha256:caebaf527ba0576d76c6d7579c1c921d78dcd0522d3dbe11a11c5ebc1c05b37b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.0 MB (33971560 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f0d964750c0182cb6e1376d8eec8982b36ab1b3aa6f8ab59919f116da2625871`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 26 Jan 2022 01:39:55 GMT
ADD file:876ebf07c65841f4840842086c883af48e07386964fe6d643ba193895ec2a582 in / 
# Wed, 26 Jan 2022 01:39:56 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 08:45:04 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 26 Jan 2022 08:45:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 08:45:09 GMT
ENV MEMCACHED_VERSION=1.6.13
# Wed, 26 Jan 2022 08:45:09 GMT
ENV MEMCACHED_SHA1=b9da57ba63ba8de8a980fe0fe2fedc8d59e1dfe3
# Wed, 26 Jan 2022 08:49:29 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 26 Jan 2022 08:49:29 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 26 Jan 2022 08:49:30 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 26 Jan 2022 08:49:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Jan 2022 08:49:31 GMT
USER memcache
# Wed, 26 Jan 2022 08:49:31 GMT
EXPOSE 11211
# Wed, 26 Jan 2022 08:49:31 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:86933886b1754aba091548cf031a9bca88cdce9bb4fc1f28bb38b61594c2c2c7`  
		Last Modified: Wed, 26 Jan 2022 01:48:57 GMT  
		Size: 32.4 MB (32377406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84bd6e2dff27e256b3baec641bd7c64e8a138237c2c259a806d0f9a9fb1d2255`  
		Last Modified: Wed, 26 Jan 2022 08:50:25 GMT  
		Size: 4.9 KB (4896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d8c7dc83b8d6601d80421931237cbfcd968616d9910fad6f78ee1706ee8f1e3`  
		Last Modified: Wed, 26 Jan 2022 08:50:26 GMT  
		Size: 336.6 KB (336627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5e3e4cf9c8423bfa3e769914fdcf235f6b64837f5fb62f5ccc09a8d792a268c`  
		Last Modified: Wed, 26 Jan 2022 08:50:26 GMT  
		Size: 1.3 MB (1252223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6402d600344325d49706165f2b0feec85cd2421776889433e4c45230bc89b7ee`  
		Last Modified: Wed, 26 Jan 2022 08:50:25 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9fa9c73a03d6ce53a9ea22b31db2648aa6a02a1779ae0a5b19070fbbe806125`  
		Last Modified: Wed, 26 Jan 2022 08:50:25 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-bullseye` - linux; mips64le

```console
$ docker pull memcached@sha256:0848c96207329a581151eeefb1a2b5f1c13893e01667962c71ed108ba448ec8a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.2 MB (31212144 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5691adbb93dbe11492ece526682692fc23ae3869ddd09a5cc20fc92abe25fa68`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:45 GMT
ADD file:61767027a5ab46afbcd4079d200abe8d663326adc96fa28ca8c8955a06d9322e in / 
# Wed, 26 Jan 2022 01:42:46 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 04:16:54 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 26 Jan 2022 04:17:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 04:17:06 GMT
ENV MEMCACHED_VERSION=1.6.13
# Wed, 26 Jan 2022 04:17:07 GMT
ENV MEMCACHED_SHA1=b9da57ba63ba8de8a980fe0fe2fedc8d59e1dfe3
# Wed, 26 Jan 2022 04:23:00 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 26 Jan 2022 04:23:00 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 26 Jan 2022 04:23:02 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 26 Jan 2022 04:23:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Jan 2022 04:23:03 GMT
USER memcache
# Wed, 26 Jan 2022 04:23:03 GMT
EXPOSE 11211
# Wed, 26 Jan 2022 04:23:03 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:266e7d2b59483859eaa1711d2afeb25ea4458eeb36b3e909372930db1f834d7f`  
		Last Modified: Wed, 26 Jan 2022 01:51:23 GMT  
		Size: 29.6 MB (29632834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f2c23d84e18c59799194289c3354e30ed9e147411beb83fd8a53a6b0510244e`  
		Last Modified: Wed, 26 Jan 2022 04:23:22 GMT  
		Size: 5.0 KB (4977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e72e725e4f6fb1ddea7af05f25646fbd5f401583a994d00e98f8d9762bdeef1`  
		Last Modified: Wed, 26 Jan 2022 04:23:22 GMT  
		Size: 323.7 KB (323700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a64f2bbfc21569385827a44c22dc4d96a9004879a3db5a479ac796150f31a89`  
		Last Modified: Wed, 26 Jan 2022 04:23:23 GMT  
		Size: 1.3 MB (1250226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10ec607308395a4822bcdf6d4c2f8665284150145ceaee889026d63b5bbfc525`  
		Last Modified: Wed, 26 Jan 2022 04:23:22 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0544419df418d0761bfd4cee74e348f336fd813c7d70a2ba0f9c66dd4dcad99`  
		Last Modified: Wed, 26 Jan 2022 04:23:22 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-bullseye` - linux; ppc64le

```console
$ docker pull memcached@sha256:467baa60d3118dac94a8d1909db41ec8f8e0867581bba86e83d70d2843299d95
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.0 MB (36956955 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89c206a82af6419284433a55b65259fb3c41ae73d206fc37aa006d7c30d22d0e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 26 Jan 2022 01:46:51 GMT
ADD file:c03f34c221e57fa5cb625c166d1db9f72d6ba2fa17a3c41a5d04d6875d098949 in / 
# Wed, 26 Jan 2022 01:46:57 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 05:38:39 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 26 Jan 2022 05:38:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 05:38:55 GMT
ENV MEMCACHED_VERSION=1.6.13
# Wed, 26 Jan 2022 05:38:58 GMT
ENV MEMCACHED_SHA1=b9da57ba63ba8de8a980fe0fe2fedc8d59e1dfe3
# Wed, 26 Jan 2022 05:44:08 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 26 Jan 2022 05:44:10 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 26 Jan 2022 05:44:17 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 26 Jan 2022 05:44:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Jan 2022 05:44:24 GMT
USER memcache
# Wed, 26 Jan 2022 05:44:28 GMT
EXPOSE 11211
# Wed, 26 Jan 2022 05:44:32 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:3149ee4a73508a4c39107d64a3fdc1b021626a22a0ac95e62fa0cea49ab77fba`  
		Last Modified: Wed, 26 Jan 2022 01:57:01 GMT  
		Size: 35.3 MB (35273030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07bcb451658eb6d9eace467c2e989d96e53c409eb48347a369e9ad80aadcfe96`  
		Last Modified: Wed, 26 Jan 2022 05:45:22 GMT  
		Size: 5.0 KB (4980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8807782e060aa90873de57b2d3ec277632145f166e9c1e3801c57eea7e595cc`  
		Last Modified: Wed, 26 Jan 2022 05:45:22 GMT  
		Size: 356.9 KB (356905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9214a40cf25dcbbc1d21f60a5512d485bc08156423100a0bb814946e829e3a0e`  
		Last Modified: Wed, 26 Jan 2022 05:45:22 GMT  
		Size: 1.3 MB (1321633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90ee2e08d849858def804d36f370ce894ef499543f6e8a72b9aac42c9e1cc909`  
		Last Modified: Wed, 26 Jan 2022 05:45:22 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6635b7a8817986bc0e4c179ae7d01d924f3017618b34956074b196886d9aaa67`  
		Last Modified: Wed, 26 Jan 2022 05:45:22 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-bullseye` - linux; s390x

```console
$ docker pull memcached@sha256:0f830716b97909822e4fe0394e7907f03695936767866c5e3dde96f89f483b30
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.2 MB (31216717 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e41587da3718a95304af17c726b656832260d3107e24f7811d54a20c5bad539`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 26 Jan 2022 01:41:13 GMT
ADD file:03b224b82f458b08d3b5071e42b67915a3db309332c0fc9229db7cf1148bc1b5 in / 
# Wed, 26 Jan 2022 01:41:15 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 03:32:44 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 26 Jan 2022 03:32:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 03:32:47 GMT
ENV MEMCACHED_VERSION=1.6.13
# Wed, 26 Jan 2022 03:32:48 GMT
ENV MEMCACHED_SHA1=b9da57ba63ba8de8a980fe0fe2fedc8d59e1dfe3
# Wed, 26 Jan 2022 03:36:16 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 26 Jan 2022 03:36:16 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 26 Jan 2022 03:36:16 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 26 Jan 2022 03:36:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Jan 2022 03:36:17 GMT
USER memcache
# Wed, 26 Jan 2022 03:36:17 GMT
EXPOSE 11211
# Wed, 26 Jan 2022 03:36:17 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:70bed29526f8483937e4d2540d19256d30786007c7c321e717e00d2e74700380`  
		Last Modified: Wed, 26 Jan 2022 01:46:57 GMT  
		Size: 29.6 MB (29647071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:531e195eaaf208f50aadc4ec839bd3a8f8d4bb0a35dea07bb0e27335fcf6db05`  
		Last Modified: Wed, 26 Jan 2022 03:37:15 GMT  
		Size: 5.0 KB (5026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1072031f118cfb7a6e47244d0bc6a66ac9a2cd286044b62e34033f655f0166d`  
		Last Modified: Wed, 26 Jan 2022 03:37:16 GMT  
		Size: 324.1 KB (324144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3719ec4f04cc9c989d6e8fb755b61510a0e78a3d35107b06cfc6c109c5aac17d`  
		Last Modified: Wed, 26 Jan 2022 03:37:16 GMT  
		Size: 1.2 MB (1240067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c8553e94280409bcb797ba67589732c286468e57828ea58da8d393d5b25a881`  
		Last Modified: Wed, 26 Jan 2022 03:37:16 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de608eaa9aaa185e5049d6baf7896898fe3d2c6beef1fcac73855ec782e15eee`  
		Last Modified: Wed, 26 Jan 2022 03:37:16 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:1.6`

```console
$ docker pull memcached@sha256:61a8c3887d91c23aa6ce62b145b6e77acb1bcf195e950b3971f4007f2a47fa12
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
$ docker pull memcached@sha256:c9756ec03bedf0411e142fa016cce653157ef46216102b2ad9012ba57a69e9b5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.9 MB (32945941 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c8b63b0eeb514dca60290d594b69ba36d42534eb7c4af27ceb25c4b900d862c8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 21 Dec 2021 01:22:43 GMT
ADD file:09675d11695f65c55efdc393ff0cd32f30194cd7d0fbef4631eebfed4414ac97 in / 
# Tue, 21 Dec 2021 01:22:43 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 18:34:30 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 21 Dec 2021 18:34:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 20 Jan 2022 04:23:06 GMT
ENV MEMCACHED_VERSION=1.6.13
# Thu, 20 Jan 2022 04:23:06 GMT
ENV MEMCACHED_SHA1=b9da57ba63ba8de8a980fe0fe2fedc8d59e1dfe3
# Thu, 20 Jan 2022 04:27:08 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 20 Jan 2022 04:27:08 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 20 Jan 2022 04:27:09 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 20 Jan 2022 04:27:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 20 Jan 2022 04:27:09 GMT
USER memcache
# Thu, 20 Jan 2022 04:27:10 GMT
EXPOSE 11211
# Thu, 20 Jan 2022 04:27:10 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:a2abf6c4d29d43a4bf9fbb769f524d0fb36a2edab49819c1bf3e76f409f953ea`  
		Last Modified: Tue, 21 Dec 2021 01:27:48 GMT  
		Size: 31.4 MB (31357624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aa5be68e24cfc338b0c9be41213371a3ed596d00487ad58df6494ed46626117`  
		Last Modified: Tue, 21 Dec 2021 18:39:12 GMT  
		Size: 5.0 KB (4978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:052b406b20ce6593c7a47bc0d4d4f8b45258c1aed8b86ab06c0fc75ab6b4ee40`  
		Last Modified: Tue, 21 Dec 2021 18:39:13 GMT  
		Size: 328.1 KB (328055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b89359883409361f4bb025aaae623b73503a2801842fa3ceda2711924cf71b5`  
		Last Modified: Thu, 20 Jan 2022 04:31:55 GMT  
		Size: 1.3 MB (1254875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f5e296124091603e6ac2227e0bb1a6cde6faafa7608b926488a5d003b20d987`  
		Last Modified: Thu, 20 Jan 2022 04:31:54 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d7a956a84f556974daee7c5e1010bfa31d093c5b8b5eaabffa21a4931fe48f7`  
		Last Modified: Thu, 20 Jan 2022 04:31:54 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6` - linux; arm variant v5

```console
$ docker pull memcached@sha256:d16a2790a88e4662d8340cb85a9660f7738b5abbe759bad21b8f676e0ca8312c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.4 MB (30447722 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7768dab3ed87264de0f4e8a613c070301197408077835da74c7faae6eb6f4bd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 21 Dec 2021 01:50:31 GMT
ADD file:a3023f71bd93966e7db1419adda3ccde4fcc5e2e8cf58e7b13c51036ed5ff796 in / 
# Tue, 21 Dec 2021 01:50:32 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 03:35:35 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 21 Dec 2021 03:35:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 19 Jan 2022 23:48:42 GMT
ENV MEMCACHED_VERSION=1.6.13
# Wed, 19 Jan 2022 23:48:43 GMT
ENV MEMCACHED_SHA1=b9da57ba63ba8de8a980fe0fe2fedc8d59e1dfe3
# Wed, 19 Jan 2022 23:54:08 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 19 Jan 2022 23:54:09 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 19 Jan 2022 23:54:13 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 19 Jan 2022 23:54:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 19 Jan 2022 23:54:14 GMT
USER memcache
# Wed, 19 Jan 2022 23:54:15 GMT
EXPOSE 11211
# Wed, 19 Jan 2022 23:54:16 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:054429d0cf4038fef39a3b5eb6ce52f600f9a2cbb71a4fb3e95ecf9b2da62581`  
		Last Modified: Tue, 21 Dec 2021 02:05:52 GMT  
		Size: 28.9 MB (28900253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb7fdf670368bfde88ac158623eeda4b36ce64bd838e78a9ffcd3d2622eea2e8`  
		Last Modified: Tue, 21 Dec 2021 03:41:18 GMT  
		Size: 4.9 KB (4893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21508b31a1593117f5747b299da29b6bec5fb36f008effcd821336ebafc8ad70`  
		Last Modified: Tue, 21 Dec 2021 03:41:18 GMT  
		Size: 316.6 KB (316576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6d782b9d573913a26c43aba467d4fed6b33af9b83f44cfb1e8f63a76f92ab3a`  
		Last Modified: Wed, 19 Jan 2022 23:55:13 GMT  
		Size: 1.2 MB (1225592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b184c6b4181672a28be507397bd5d2baad8db49549bba6940adb30ce28c3320`  
		Last Modified: Wed, 19 Jan 2022 23:55:12 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73e44f9f60691acb75f8287e5a5eaa0675e04ffbc1fa1e4abfe57733ca7aa595`  
		Last Modified: Wed, 19 Jan 2022 23:55:12 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6` - linux; arm variant v7

```console
$ docker pull memcached@sha256:7f4a3e4bd6d3845da89e6e1fa7ee377f050118bd20803a8716e7c8aab31670ee
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.1 MB (28078674 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d0493346f5301d1fac3c1ee8eb4df2a8f1791ec73c16d2425aa56be76aabae7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:08 GMT
ADD file:7f27f5b43b7cb04e509fe145266d9bdeacfcacb024cafac32e57ef1c831d5ea7 in / 
# Wed, 26 Jan 2022 01:42:09 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 08:54:44 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 26 Jan 2022 08:54:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 08:54:52 GMT
ENV MEMCACHED_VERSION=1.6.13
# Wed, 26 Jan 2022 08:54:52 GMT
ENV MEMCACHED_SHA1=b9da57ba63ba8de8a980fe0fe2fedc8d59e1dfe3
# Wed, 26 Jan 2022 08:59:15 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 26 Jan 2022 08:59:16 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 26 Jan 2022 08:59:18 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 26 Jan 2022 08:59:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Jan 2022 08:59:18 GMT
USER memcache
# Wed, 26 Jan 2022 08:59:19 GMT
EXPOSE 11211
# Wed, 26 Jan 2022 08:59:19 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:aaef1f1162ec03e01b5b955d41da400544ec2374093ae3dbc330ab2bb36df3e1`  
		Last Modified: Wed, 26 Jan 2022 01:57:59 GMT  
		Size: 26.6 MB (26564933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c9d3dbbb6d5b3a74ea3807c462c99fc02f7ef46831734a98ab085fbfd45d84c`  
		Last Modified: Wed, 26 Jan 2022 09:13:01 GMT  
		Size: 4.9 KB (4894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c553a44b8d98c757ba52201bd5897c9b84bed862d1f1a33b30eaee164faf002`  
		Last Modified: Wed, 26 Jan 2022 09:13:02 GMT  
		Size: 312.0 KB (312023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e05d6d11f4c98f66add6994ad62c7fe25432ba441f2618ba25e8d572c66fe89`  
		Last Modified: Wed, 26 Jan 2022 09:13:02 GMT  
		Size: 1.2 MB (1196416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:902b4740d93b1e9cdd39f484a29d2e022801b8f4612ddd6471c63d0d5aee77c7`  
		Last Modified: Wed, 26 Jan 2022 09:13:01 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0813f5460d7241e77461d216cec438321996a8a74a205fd5a63e3a6e7300ec08`  
		Last Modified: Wed, 26 Jan 2022 09:13:01 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:97cdec366a180179780e13eb6ab3b4839bd7ce753737ed9b69c45d5baf9d55e0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.4 MB (31434947 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9182bae18682935ee16f416121710ff59a5021e8148d558c7df06caa35e422c5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:31 GMT
ADD file:0ec6f47a8857bf8e6cef71ed8f864be7ce1790ff6ed04fd4201e7dbde4728d3a in / 
# Wed, 26 Jan 2022 01:42:31 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 04:50:24 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 26 Jan 2022 04:50:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 04:50:28 GMT
ENV MEMCACHED_VERSION=1.6.13
# Wed, 26 Jan 2022 04:50:29 GMT
ENV MEMCACHED_SHA1=b9da57ba63ba8de8a980fe0fe2fedc8d59e1dfe3
# Wed, 26 Jan 2022 04:53:09 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 26 Jan 2022 04:53:10 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 26 Jan 2022 04:53:10 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 26 Jan 2022 04:53:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Jan 2022 04:53:12 GMT
USER memcache
# Wed, 26 Jan 2022 04:53:13 GMT
EXPOSE 11211
# Wed, 26 Jan 2022 04:53:14 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:8998bd30e6a1204d13403045766edbe14f941b52087465f5d140ab63c8b113bf`  
		Last Modified: Wed, 26 Jan 2022 01:49:04 GMT  
		Size: 30.1 MB (30056774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a59fc24ed29770b5c2f4352a96e8a82fa286fa87df96964968e2fb2796e105ac`  
		Last Modified: Wed, 26 Jan 2022 04:53:58 GMT  
		Size: 4.9 KB (4900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54853adf97755cd00bf2b960a7a7458bfc9824d4847b0f97e7e5f41e86b6c351`  
		Last Modified: Wed, 26 Jan 2022 04:53:59 GMT  
		Size: 119.2 KB (119210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bc43135274188258180f193f3f9907dd72b6b09963f1886610f28977741356a`  
		Last Modified: Wed, 26 Jan 2022 04:53:59 GMT  
		Size: 1.3 MB (1253657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e306557d5e40e37e762e103bd520b6153919316e8d64e4ae3d21fa66d6420f3`  
		Last Modified: Wed, 26 Jan 2022 04:53:59 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86f1b169766c42ff4dabdf96ef26f2207f4f9fa4fdf13b53c3625a106c50ca12`  
		Last Modified: Wed, 26 Jan 2022 04:53:58 GMT  
		Size: 120.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6` - linux; 386

```console
$ docker pull memcached@sha256:caebaf527ba0576d76c6d7579c1c921d78dcd0522d3dbe11a11c5ebc1c05b37b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.0 MB (33971560 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f0d964750c0182cb6e1376d8eec8982b36ab1b3aa6f8ab59919f116da2625871`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 26 Jan 2022 01:39:55 GMT
ADD file:876ebf07c65841f4840842086c883af48e07386964fe6d643ba193895ec2a582 in / 
# Wed, 26 Jan 2022 01:39:56 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 08:45:04 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 26 Jan 2022 08:45:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 08:45:09 GMT
ENV MEMCACHED_VERSION=1.6.13
# Wed, 26 Jan 2022 08:45:09 GMT
ENV MEMCACHED_SHA1=b9da57ba63ba8de8a980fe0fe2fedc8d59e1dfe3
# Wed, 26 Jan 2022 08:49:29 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 26 Jan 2022 08:49:29 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 26 Jan 2022 08:49:30 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 26 Jan 2022 08:49:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Jan 2022 08:49:31 GMT
USER memcache
# Wed, 26 Jan 2022 08:49:31 GMT
EXPOSE 11211
# Wed, 26 Jan 2022 08:49:31 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:86933886b1754aba091548cf031a9bca88cdce9bb4fc1f28bb38b61594c2c2c7`  
		Last Modified: Wed, 26 Jan 2022 01:48:57 GMT  
		Size: 32.4 MB (32377406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84bd6e2dff27e256b3baec641bd7c64e8a138237c2c259a806d0f9a9fb1d2255`  
		Last Modified: Wed, 26 Jan 2022 08:50:25 GMT  
		Size: 4.9 KB (4896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d8c7dc83b8d6601d80421931237cbfcd968616d9910fad6f78ee1706ee8f1e3`  
		Last Modified: Wed, 26 Jan 2022 08:50:26 GMT  
		Size: 336.6 KB (336627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5e3e4cf9c8423bfa3e769914fdcf235f6b64837f5fb62f5ccc09a8d792a268c`  
		Last Modified: Wed, 26 Jan 2022 08:50:26 GMT  
		Size: 1.3 MB (1252223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6402d600344325d49706165f2b0feec85cd2421776889433e4c45230bc89b7ee`  
		Last Modified: Wed, 26 Jan 2022 08:50:25 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9fa9c73a03d6ce53a9ea22b31db2648aa6a02a1779ae0a5b19070fbbe806125`  
		Last Modified: Wed, 26 Jan 2022 08:50:25 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6` - linux; mips64le

```console
$ docker pull memcached@sha256:0848c96207329a581151eeefb1a2b5f1c13893e01667962c71ed108ba448ec8a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.2 MB (31212144 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5691adbb93dbe11492ece526682692fc23ae3869ddd09a5cc20fc92abe25fa68`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:45 GMT
ADD file:61767027a5ab46afbcd4079d200abe8d663326adc96fa28ca8c8955a06d9322e in / 
# Wed, 26 Jan 2022 01:42:46 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 04:16:54 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 26 Jan 2022 04:17:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 04:17:06 GMT
ENV MEMCACHED_VERSION=1.6.13
# Wed, 26 Jan 2022 04:17:07 GMT
ENV MEMCACHED_SHA1=b9da57ba63ba8de8a980fe0fe2fedc8d59e1dfe3
# Wed, 26 Jan 2022 04:23:00 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 26 Jan 2022 04:23:00 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 26 Jan 2022 04:23:02 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 26 Jan 2022 04:23:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Jan 2022 04:23:03 GMT
USER memcache
# Wed, 26 Jan 2022 04:23:03 GMT
EXPOSE 11211
# Wed, 26 Jan 2022 04:23:03 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:266e7d2b59483859eaa1711d2afeb25ea4458eeb36b3e909372930db1f834d7f`  
		Last Modified: Wed, 26 Jan 2022 01:51:23 GMT  
		Size: 29.6 MB (29632834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f2c23d84e18c59799194289c3354e30ed9e147411beb83fd8a53a6b0510244e`  
		Last Modified: Wed, 26 Jan 2022 04:23:22 GMT  
		Size: 5.0 KB (4977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e72e725e4f6fb1ddea7af05f25646fbd5f401583a994d00e98f8d9762bdeef1`  
		Last Modified: Wed, 26 Jan 2022 04:23:22 GMT  
		Size: 323.7 KB (323700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a64f2bbfc21569385827a44c22dc4d96a9004879a3db5a479ac796150f31a89`  
		Last Modified: Wed, 26 Jan 2022 04:23:23 GMT  
		Size: 1.3 MB (1250226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10ec607308395a4822bcdf6d4c2f8665284150145ceaee889026d63b5bbfc525`  
		Last Modified: Wed, 26 Jan 2022 04:23:22 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0544419df418d0761bfd4cee74e348f336fd813c7d70a2ba0f9c66dd4dcad99`  
		Last Modified: Wed, 26 Jan 2022 04:23:22 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6` - linux; ppc64le

```console
$ docker pull memcached@sha256:467baa60d3118dac94a8d1909db41ec8f8e0867581bba86e83d70d2843299d95
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.0 MB (36956955 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89c206a82af6419284433a55b65259fb3c41ae73d206fc37aa006d7c30d22d0e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 26 Jan 2022 01:46:51 GMT
ADD file:c03f34c221e57fa5cb625c166d1db9f72d6ba2fa17a3c41a5d04d6875d098949 in / 
# Wed, 26 Jan 2022 01:46:57 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 05:38:39 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 26 Jan 2022 05:38:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 05:38:55 GMT
ENV MEMCACHED_VERSION=1.6.13
# Wed, 26 Jan 2022 05:38:58 GMT
ENV MEMCACHED_SHA1=b9da57ba63ba8de8a980fe0fe2fedc8d59e1dfe3
# Wed, 26 Jan 2022 05:44:08 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 26 Jan 2022 05:44:10 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 26 Jan 2022 05:44:17 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 26 Jan 2022 05:44:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Jan 2022 05:44:24 GMT
USER memcache
# Wed, 26 Jan 2022 05:44:28 GMT
EXPOSE 11211
# Wed, 26 Jan 2022 05:44:32 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:3149ee4a73508a4c39107d64a3fdc1b021626a22a0ac95e62fa0cea49ab77fba`  
		Last Modified: Wed, 26 Jan 2022 01:57:01 GMT  
		Size: 35.3 MB (35273030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07bcb451658eb6d9eace467c2e989d96e53c409eb48347a369e9ad80aadcfe96`  
		Last Modified: Wed, 26 Jan 2022 05:45:22 GMT  
		Size: 5.0 KB (4980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8807782e060aa90873de57b2d3ec277632145f166e9c1e3801c57eea7e595cc`  
		Last Modified: Wed, 26 Jan 2022 05:45:22 GMT  
		Size: 356.9 KB (356905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9214a40cf25dcbbc1d21f60a5512d485bc08156423100a0bb814946e829e3a0e`  
		Last Modified: Wed, 26 Jan 2022 05:45:22 GMT  
		Size: 1.3 MB (1321633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90ee2e08d849858def804d36f370ce894ef499543f6e8a72b9aac42c9e1cc909`  
		Last Modified: Wed, 26 Jan 2022 05:45:22 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6635b7a8817986bc0e4c179ae7d01d924f3017618b34956074b196886d9aaa67`  
		Last Modified: Wed, 26 Jan 2022 05:45:22 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6` - linux; s390x

```console
$ docker pull memcached@sha256:0f830716b97909822e4fe0394e7907f03695936767866c5e3dde96f89f483b30
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.2 MB (31216717 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e41587da3718a95304af17c726b656832260d3107e24f7811d54a20c5bad539`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 26 Jan 2022 01:41:13 GMT
ADD file:03b224b82f458b08d3b5071e42b67915a3db309332c0fc9229db7cf1148bc1b5 in / 
# Wed, 26 Jan 2022 01:41:15 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 03:32:44 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 26 Jan 2022 03:32:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 03:32:47 GMT
ENV MEMCACHED_VERSION=1.6.13
# Wed, 26 Jan 2022 03:32:48 GMT
ENV MEMCACHED_SHA1=b9da57ba63ba8de8a980fe0fe2fedc8d59e1dfe3
# Wed, 26 Jan 2022 03:36:16 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 26 Jan 2022 03:36:16 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 26 Jan 2022 03:36:16 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 26 Jan 2022 03:36:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Jan 2022 03:36:17 GMT
USER memcache
# Wed, 26 Jan 2022 03:36:17 GMT
EXPOSE 11211
# Wed, 26 Jan 2022 03:36:17 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:70bed29526f8483937e4d2540d19256d30786007c7c321e717e00d2e74700380`  
		Last Modified: Wed, 26 Jan 2022 01:46:57 GMT  
		Size: 29.6 MB (29647071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:531e195eaaf208f50aadc4ec839bd3a8f8d4bb0a35dea07bb0e27335fcf6db05`  
		Last Modified: Wed, 26 Jan 2022 03:37:15 GMT  
		Size: 5.0 KB (5026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1072031f118cfb7a6e47244d0bc6a66ac9a2cd286044b62e34033f655f0166d`  
		Last Modified: Wed, 26 Jan 2022 03:37:16 GMT  
		Size: 324.1 KB (324144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3719ec4f04cc9c989d6e8fb755b61510a0e78a3d35107b06cfc6c109c5aac17d`  
		Last Modified: Wed, 26 Jan 2022 03:37:16 GMT  
		Size: 1.2 MB (1240067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c8553e94280409bcb797ba67589732c286468e57828ea58da8d393d5b25a881`  
		Last Modified: Wed, 26 Jan 2022 03:37:16 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de608eaa9aaa185e5049d6baf7896898fe3d2c6beef1fcac73855ec782e15eee`  
		Last Modified: Wed, 26 Jan 2022 03:37:16 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:1.6-alpine`

```console
$ docker pull memcached@sha256:4fd74bfdda3c109c25e7edfd6b77545c48963b938d6f75f4fb8c122c5cdae7cd
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

### `memcached:1.6-alpine` - linux; 386

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

### `memcached:1.6-alpine` - linux; ppc64le

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

### `memcached:1.6-alpine` - linux; s390x

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

## `memcached:1.6-alpine3.15`

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

### `memcached:1.6-alpine3.15` - linux; amd64

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

### `memcached:1.6-alpine3.15` - linux; arm64 variant v8

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

### `memcached:1.6-alpine3.15` - linux; 386

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

### `memcached:1.6-alpine3.15` - linux; ppc64le

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

### `memcached:1.6-alpine3.15` - linux; s390x

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

## `memcached:1.6-bullseye`

```console
$ docker pull memcached@sha256:61a8c3887d91c23aa6ce62b145b6e77acb1bcf195e950b3971f4007f2a47fa12
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
$ docker pull memcached@sha256:c9756ec03bedf0411e142fa016cce653157ef46216102b2ad9012ba57a69e9b5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.9 MB (32945941 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c8b63b0eeb514dca60290d594b69ba36d42534eb7c4af27ceb25c4b900d862c8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 21 Dec 2021 01:22:43 GMT
ADD file:09675d11695f65c55efdc393ff0cd32f30194cd7d0fbef4631eebfed4414ac97 in / 
# Tue, 21 Dec 2021 01:22:43 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 18:34:30 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 21 Dec 2021 18:34:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 20 Jan 2022 04:23:06 GMT
ENV MEMCACHED_VERSION=1.6.13
# Thu, 20 Jan 2022 04:23:06 GMT
ENV MEMCACHED_SHA1=b9da57ba63ba8de8a980fe0fe2fedc8d59e1dfe3
# Thu, 20 Jan 2022 04:27:08 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 20 Jan 2022 04:27:08 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 20 Jan 2022 04:27:09 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 20 Jan 2022 04:27:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 20 Jan 2022 04:27:09 GMT
USER memcache
# Thu, 20 Jan 2022 04:27:10 GMT
EXPOSE 11211
# Thu, 20 Jan 2022 04:27:10 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:a2abf6c4d29d43a4bf9fbb769f524d0fb36a2edab49819c1bf3e76f409f953ea`  
		Last Modified: Tue, 21 Dec 2021 01:27:48 GMT  
		Size: 31.4 MB (31357624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aa5be68e24cfc338b0c9be41213371a3ed596d00487ad58df6494ed46626117`  
		Last Modified: Tue, 21 Dec 2021 18:39:12 GMT  
		Size: 5.0 KB (4978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:052b406b20ce6593c7a47bc0d4d4f8b45258c1aed8b86ab06c0fc75ab6b4ee40`  
		Last Modified: Tue, 21 Dec 2021 18:39:13 GMT  
		Size: 328.1 KB (328055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b89359883409361f4bb025aaae623b73503a2801842fa3ceda2711924cf71b5`  
		Last Modified: Thu, 20 Jan 2022 04:31:55 GMT  
		Size: 1.3 MB (1254875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f5e296124091603e6ac2227e0bb1a6cde6faafa7608b926488a5d003b20d987`  
		Last Modified: Thu, 20 Jan 2022 04:31:54 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d7a956a84f556974daee7c5e1010bfa31d093c5b8b5eaabffa21a4931fe48f7`  
		Last Modified: Thu, 20 Jan 2022 04:31:54 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-bullseye` - linux; arm variant v5

```console
$ docker pull memcached@sha256:d16a2790a88e4662d8340cb85a9660f7738b5abbe759bad21b8f676e0ca8312c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.4 MB (30447722 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7768dab3ed87264de0f4e8a613c070301197408077835da74c7faae6eb6f4bd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 21 Dec 2021 01:50:31 GMT
ADD file:a3023f71bd93966e7db1419adda3ccde4fcc5e2e8cf58e7b13c51036ed5ff796 in / 
# Tue, 21 Dec 2021 01:50:32 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 03:35:35 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 21 Dec 2021 03:35:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 19 Jan 2022 23:48:42 GMT
ENV MEMCACHED_VERSION=1.6.13
# Wed, 19 Jan 2022 23:48:43 GMT
ENV MEMCACHED_SHA1=b9da57ba63ba8de8a980fe0fe2fedc8d59e1dfe3
# Wed, 19 Jan 2022 23:54:08 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 19 Jan 2022 23:54:09 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 19 Jan 2022 23:54:13 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 19 Jan 2022 23:54:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 19 Jan 2022 23:54:14 GMT
USER memcache
# Wed, 19 Jan 2022 23:54:15 GMT
EXPOSE 11211
# Wed, 19 Jan 2022 23:54:16 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:054429d0cf4038fef39a3b5eb6ce52f600f9a2cbb71a4fb3e95ecf9b2da62581`  
		Last Modified: Tue, 21 Dec 2021 02:05:52 GMT  
		Size: 28.9 MB (28900253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb7fdf670368bfde88ac158623eeda4b36ce64bd838e78a9ffcd3d2622eea2e8`  
		Last Modified: Tue, 21 Dec 2021 03:41:18 GMT  
		Size: 4.9 KB (4893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21508b31a1593117f5747b299da29b6bec5fb36f008effcd821336ebafc8ad70`  
		Last Modified: Tue, 21 Dec 2021 03:41:18 GMT  
		Size: 316.6 KB (316576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6d782b9d573913a26c43aba467d4fed6b33af9b83f44cfb1e8f63a76f92ab3a`  
		Last Modified: Wed, 19 Jan 2022 23:55:13 GMT  
		Size: 1.2 MB (1225592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b184c6b4181672a28be507397bd5d2baad8db49549bba6940adb30ce28c3320`  
		Last Modified: Wed, 19 Jan 2022 23:55:12 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73e44f9f60691acb75f8287e5a5eaa0675e04ffbc1fa1e4abfe57733ca7aa595`  
		Last Modified: Wed, 19 Jan 2022 23:55:12 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-bullseye` - linux; arm variant v7

```console
$ docker pull memcached@sha256:7f4a3e4bd6d3845da89e6e1fa7ee377f050118bd20803a8716e7c8aab31670ee
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.1 MB (28078674 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d0493346f5301d1fac3c1ee8eb4df2a8f1791ec73c16d2425aa56be76aabae7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:08 GMT
ADD file:7f27f5b43b7cb04e509fe145266d9bdeacfcacb024cafac32e57ef1c831d5ea7 in / 
# Wed, 26 Jan 2022 01:42:09 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 08:54:44 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 26 Jan 2022 08:54:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 08:54:52 GMT
ENV MEMCACHED_VERSION=1.6.13
# Wed, 26 Jan 2022 08:54:52 GMT
ENV MEMCACHED_SHA1=b9da57ba63ba8de8a980fe0fe2fedc8d59e1dfe3
# Wed, 26 Jan 2022 08:59:15 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 26 Jan 2022 08:59:16 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 26 Jan 2022 08:59:18 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 26 Jan 2022 08:59:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Jan 2022 08:59:18 GMT
USER memcache
# Wed, 26 Jan 2022 08:59:19 GMT
EXPOSE 11211
# Wed, 26 Jan 2022 08:59:19 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:aaef1f1162ec03e01b5b955d41da400544ec2374093ae3dbc330ab2bb36df3e1`  
		Last Modified: Wed, 26 Jan 2022 01:57:59 GMT  
		Size: 26.6 MB (26564933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c9d3dbbb6d5b3a74ea3807c462c99fc02f7ef46831734a98ab085fbfd45d84c`  
		Last Modified: Wed, 26 Jan 2022 09:13:01 GMT  
		Size: 4.9 KB (4894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c553a44b8d98c757ba52201bd5897c9b84bed862d1f1a33b30eaee164faf002`  
		Last Modified: Wed, 26 Jan 2022 09:13:02 GMT  
		Size: 312.0 KB (312023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e05d6d11f4c98f66add6994ad62c7fe25432ba441f2618ba25e8d572c66fe89`  
		Last Modified: Wed, 26 Jan 2022 09:13:02 GMT  
		Size: 1.2 MB (1196416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:902b4740d93b1e9cdd39f484a29d2e022801b8f4612ddd6471c63d0d5aee77c7`  
		Last Modified: Wed, 26 Jan 2022 09:13:01 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0813f5460d7241e77461d216cec438321996a8a74a205fd5a63e3a6e7300ec08`  
		Last Modified: Wed, 26 Jan 2022 09:13:01 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-bullseye` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:97cdec366a180179780e13eb6ab3b4839bd7ce753737ed9b69c45d5baf9d55e0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.4 MB (31434947 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9182bae18682935ee16f416121710ff59a5021e8148d558c7df06caa35e422c5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:31 GMT
ADD file:0ec6f47a8857bf8e6cef71ed8f864be7ce1790ff6ed04fd4201e7dbde4728d3a in / 
# Wed, 26 Jan 2022 01:42:31 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 04:50:24 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 26 Jan 2022 04:50:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 04:50:28 GMT
ENV MEMCACHED_VERSION=1.6.13
# Wed, 26 Jan 2022 04:50:29 GMT
ENV MEMCACHED_SHA1=b9da57ba63ba8de8a980fe0fe2fedc8d59e1dfe3
# Wed, 26 Jan 2022 04:53:09 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 26 Jan 2022 04:53:10 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 26 Jan 2022 04:53:10 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 26 Jan 2022 04:53:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Jan 2022 04:53:12 GMT
USER memcache
# Wed, 26 Jan 2022 04:53:13 GMT
EXPOSE 11211
# Wed, 26 Jan 2022 04:53:14 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:8998bd30e6a1204d13403045766edbe14f941b52087465f5d140ab63c8b113bf`  
		Last Modified: Wed, 26 Jan 2022 01:49:04 GMT  
		Size: 30.1 MB (30056774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a59fc24ed29770b5c2f4352a96e8a82fa286fa87df96964968e2fb2796e105ac`  
		Last Modified: Wed, 26 Jan 2022 04:53:58 GMT  
		Size: 4.9 KB (4900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54853adf97755cd00bf2b960a7a7458bfc9824d4847b0f97e7e5f41e86b6c351`  
		Last Modified: Wed, 26 Jan 2022 04:53:59 GMT  
		Size: 119.2 KB (119210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bc43135274188258180f193f3f9907dd72b6b09963f1886610f28977741356a`  
		Last Modified: Wed, 26 Jan 2022 04:53:59 GMT  
		Size: 1.3 MB (1253657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e306557d5e40e37e762e103bd520b6153919316e8d64e4ae3d21fa66d6420f3`  
		Last Modified: Wed, 26 Jan 2022 04:53:59 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86f1b169766c42ff4dabdf96ef26f2207f4f9fa4fdf13b53c3625a106c50ca12`  
		Last Modified: Wed, 26 Jan 2022 04:53:58 GMT  
		Size: 120.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-bullseye` - linux; 386

```console
$ docker pull memcached@sha256:caebaf527ba0576d76c6d7579c1c921d78dcd0522d3dbe11a11c5ebc1c05b37b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.0 MB (33971560 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f0d964750c0182cb6e1376d8eec8982b36ab1b3aa6f8ab59919f116da2625871`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 26 Jan 2022 01:39:55 GMT
ADD file:876ebf07c65841f4840842086c883af48e07386964fe6d643ba193895ec2a582 in / 
# Wed, 26 Jan 2022 01:39:56 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 08:45:04 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 26 Jan 2022 08:45:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 08:45:09 GMT
ENV MEMCACHED_VERSION=1.6.13
# Wed, 26 Jan 2022 08:45:09 GMT
ENV MEMCACHED_SHA1=b9da57ba63ba8de8a980fe0fe2fedc8d59e1dfe3
# Wed, 26 Jan 2022 08:49:29 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 26 Jan 2022 08:49:29 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 26 Jan 2022 08:49:30 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 26 Jan 2022 08:49:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Jan 2022 08:49:31 GMT
USER memcache
# Wed, 26 Jan 2022 08:49:31 GMT
EXPOSE 11211
# Wed, 26 Jan 2022 08:49:31 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:86933886b1754aba091548cf031a9bca88cdce9bb4fc1f28bb38b61594c2c2c7`  
		Last Modified: Wed, 26 Jan 2022 01:48:57 GMT  
		Size: 32.4 MB (32377406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84bd6e2dff27e256b3baec641bd7c64e8a138237c2c259a806d0f9a9fb1d2255`  
		Last Modified: Wed, 26 Jan 2022 08:50:25 GMT  
		Size: 4.9 KB (4896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d8c7dc83b8d6601d80421931237cbfcd968616d9910fad6f78ee1706ee8f1e3`  
		Last Modified: Wed, 26 Jan 2022 08:50:26 GMT  
		Size: 336.6 KB (336627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5e3e4cf9c8423bfa3e769914fdcf235f6b64837f5fb62f5ccc09a8d792a268c`  
		Last Modified: Wed, 26 Jan 2022 08:50:26 GMT  
		Size: 1.3 MB (1252223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6402d600344325d49706165f2b0feec85cd2421776889433e4c45230bc89b7ee`  
		Last Modified: Wed, 26 Jan 2022 08:50:25 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9fa9c73a03d6ce53a9ea22b31db2648aa6a02a1779ae0a5b19070fbbe806125`  
		Last Modified: Wed, 26 Jan 2022 08:50:25 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-bullseye` - linux; mips64le

```console
$ docker pull memcached@sha256:0848c96207329a581151eeefb1a2b5f1c13893e01667962c71ed108ba448ec8a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.2 MB (31212144 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5691adbb93dbe11492ece526682692fc23ae3869ddd09a5cc20fc92abe25fa68`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:45 GMT
ADD file:61767027a5ab46afbcd4079d200abe8d663326adc96fa28ca8c8955a06d9322e in / 
# Wed, 26 Jan 2022 01:42:46 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 04:16:54 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 26 Jan 2022 04:17:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 04:17:06 GMT
ENV MEMCACHED_VERSION=1.6.13
# Wed, 26 Jan 2022 04:17:07 GMT
ENV MEMCACHED_SHA1=b9da57ba63ba8de8a980fe0fe2fedc8d59e1dfe3
# Wed, 26 Jan 2022 04:23:00 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 26 Jan 2022 04:23:00 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 26 Jan 2022 04:23:02 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 26 Jan 2022 04:23:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Jan 2022 04:23:03 GMT
USER memcache
# Wed, 26 Jan 2022 04:23:03 GMT
EXPOSE 11211
# Wed, 26 Jan 2022 04:23:03 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:266e7d2b59483859eaa1711d2afeb25ea4458eeb36b3e909372930db1f834d7f`  
		Last Modified: Wed, 26 Jan 2022 01:51:23 GMT  
		Size: 29.6 MB (29632834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f2c23d84e18c59799194289c3354e30ed9e147411beb83fd8a53a6b0510244e`  
		Last Modified: Wed, 26 Jan 2022 04:23:22 GMT  
		Size: 5.0 KB (4977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e72e725e4f6fb1ddea7af05f25646fbd5f401583a994d00e98f8d9762bdeef1`  
		Last Modified: Wed, 26 Jan 2022 04:23:22 GMT  
		Size: 323.7 KB (323700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a64f2bbfc21569385827a44c22dc4d96a9004879a3db5a479ac796150f31a89`  
		Last Modified: Wed, 26 Jan 2022 04:23:23 GMT  
		Size: 1.3 MB (1250226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10ec607308395a4822bcdf6d4c2f8665284150145ceaee889026d63b5bbfc525`  
		Last Modified: Wed, 26 Jan 2022 04:23:22 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0544419df418d0761bfd4cee74e348f336fd813c7d70a2ba0f9c66dd4dcad99`  
		Last Modified: Wed, 26 Jan 2022 04:23:22 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-bullseye` - linux; ppc64le

```console
$ docker pull memcached@sha256:467baa60d3118dac94a8d1909db41ec8f8e0867581bba86e83d70d2843299d95
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.0 MB (36956955 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89c206a82af6419284433a55b65259fb3c41ae73d206fc37aa006d7c30d22d0e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 26 Jan 2022 01:46:51 GMT
ADD file:c03f34c221e57fa5cb625c166d1db9f72d6ba2fa17a3c41a5d04d6875d098949 in / 
# Wed, 26 Jan 2022 01:46:57 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 05:38:39 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 26 Jan 2022 05:38:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 05:38:55 GMT
ENV MEMCACHED_VERSION=1.6.13
# Wed, 26 Jan 2022 05:38:58 GMT
ENV MEMCACHED_SHA1=b9da57ba63ba8de8a980fe0fe2fedc8d59e1dfe3
# Wed, 26 Jan 2022 05:44:08 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 26 Jan 2022 05:44:10 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 26 Jan 2022 05:44:17 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 26 Jan 2022 05:44:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Jan 2022 05:44:24 GMT
USER memcache
# Wed, 26 Jan 2022 05:44:28 GMT
EXPOSE 11211
# Wed, 26 Jan 2022 05:44:32 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:3149ee4a73508a4c39107d64a3fdc1b021626a22a0ac95e62fa0cea49ab77fba`  
		Last Modified: Wed, 26 Jan 2022 01:57:01 GMT  
		Size: 35.3 MB (35273030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07bcb451658eb6d9eace467c2e989d96e53c409eb48347a369e9ad80aadcfe96`  
		Last Modified: Wed, 26 Jan 2022 05:45:22 GMT  
		Size: 5.0 KB (4980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8807782e060aa90873de57b2d3ec277632145f166e9c1e3801c57eea7e595cc`  
		Last Modified: Wed, 26 Jan 2022 05:45:22 GMT  
		Size: 356.9 KB (356905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9214a40cf25dcbbc1d21f60a5512d485bc08156423100a0bb814946e829e3a0e`  
		Last Modified: Wed, 26 Jan 2022 05:45:22 GMT  
		Size: 1.3 MB (1321633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90ee2e08d849858def804d36f370ce894ef499543f6e8a72b9aac42c9e1cc909`  
		Last Modified: Wed, 26 Jan 2022 05:45:22 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6635b7a8817986bc0e4c179ae7d01d924f3017618b34956074b196886d9aaa67`  
		Last Modified: Wed, 26 Jan 2022 05:45:22 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-bullseye` - linux; s390x

```console
$ docker pull memcached@sha256:0f830716b97909822e4fe0394e7907f03695936767866c5e3dde96f89f483b30
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.2 MB (31216717 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e41587da3718a95304af17c726b656832260d3107e24f7811d54a20c5bad539`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 26 Jan 2022 01:41:13 GMT
ADD file:03b224b82f458b08d3b5071e42b67915a3db309332c0fc9229db7cf1148bc1b5 in / 
# Wed, 26 Jan 2022 01:41:15 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 03:32:44 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 26 Jan 2022 03:32:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 03:32:47 GMT
ENV MEMCACHED_VERSION=1.6.13
# Wed, 26 Jan 2022 03:32:48 GMT
ENV MEMCACHED_SHA1=b9da57ba63ba8de8a980fe0fe2fedc8d59e1dfe3
# Wed, 26 Jan 2022 03:36:16 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 26 Jan 2022 03:36:16 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 26 Jan 2022 03:36:16 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 26 Jan 2022 03:36:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Jan 2022 03:36:17 GMT
USER memcache
# Wed, 26 Jan 2022 03:36:17 GMT
EXPOSE 11211
# Wed, 26 Jan 2022 03:36:17 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:70bed29526f8483937e4d2540d19256d30786007c7c321e717e00d2e74700380`  
		Last Modified: Wed, 26 Jan 2022 01:46:57 GMT  
		Size: 29.6 MB (29647071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:531e195eaaf208f50aadc4ec839bd3a8f8d4bb0a35dea07bb0e27335fcf6db05`  
		Last Modified: Wed, 26 Jan 2022 03:37:15 GMT  
		Size: 5.0 KB (5026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1072031f118cfb7a6e47244d0bc6a66ac9a2cd286044b62e34033f655f0166d`  
		Last Modified: Wed, 26 Jan 2022 03:37:16 GMT  
		Size: 324.1 KB (324144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3719ec4f04cc9c989d6e8fb755b61510a0e78a3d35107b06cfc6c109c5aac17d`  
		Last Modified: Wed, 26 Jan 2022 03:37:16 GMT  
		Size: 1.2 MB (1240067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c8553e94280409bcb797ba67589732c286468e57828ea58da8d393d5b25a881`  
		Last Modified: Wed, 26 Jan 2022 03:37:16 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de608eaa9aaa185e5049d6baf7896898fe3d2c6beef1fcac73855ec782e15eee`  
		Last Modified: Wed, 26 Jan 2022 03:37:16 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:1.6.13`

```console
$ docker pull memcached@sha256:61a8c3887d91c23aa6ce62b145b6e77acb1bcf195e950b3971f4007f2a47fa12
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

### `memcached:1.6.13` - linux; amd64

```console
$ docker pull memcached@sha256:c9756ec03bedf0411e142fa016cce653157ef46216102b2ad9012ba57a69e9b5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.9 MB (32945941 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c8b63b0eeb514dca60290d594b69ba36d42534eb7c4af27ceb25c4b900d862c8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 21 Dec 2021 01:22:43 GMT
ADD file:09675d11695f65c55efdc393ff0cd32f30194cd7d0fbef4631eebfed4414ac97 in / 
# Tue, 21 Dec 2021 01:22:43 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 18:34:30 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 21 Dec 2021 18:34:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 20 Jan 2022 04:23:06 GMT
ENV MEMCACHED_VERSION=1.6.13
# Thu, 20 Jan 2022 04:23:06 GMT
ENV MEMCACHED_SHA1=b9da57ba63ba8de8a980fe0fe2fedc8d59e1dfe3
# Thu, 20 Jan 2022 04:27:08 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 20 Jan 2022 04:27:08 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 20 Jan 2022 04:27:09 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 20 Jan 2022 04:27:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 20 Jan 2022 04:27:09 GMT
USER memcache
# Thu, 20 Jan 2022 04:27:10 GMT
EXPOSE 11211
# Thu, 20 Jan 2022 04:27:10 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:a2abf6c4d29d43a4bf9fbb769f524d0fb36a2edab49819c1bf3e76f409f953ea`  
		Last Modified: Tue, 21 Dec 2021 01:27:48 GMT  
		Size: 31.4 MB (31357624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aa5be68e24cfc338b0c9be41213371a3ed596d00487ad58df6494ed46626117`  
		Last Modified: Tue, 21 Dec 2021 18:39:12 GMT  
		Size: 5.0 KB (4978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:052b406b20ce6593c7a47bc0d4d4f8b45258c1aed8b86ab06c0fc75ab6b4ee40`  
		Last Modified: Tue, 21 Dec 2021 18:39:13 GMT  
		Size: 328.1 KB (328055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b89359883409361f4bb025aaae623b73503a2801842fa3ceda2711924cf71b5`  
		Last Modified: Thu, 20 Jan 2022 04:31:55 GMT  
		Size: 1.3 MB (1254875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f5e296124091603e6ac2227e0bb1a6cde6faafa7608b926488a5d003b20d987`  
		Last Modified: Thu, 20 Jan 2022 04:31:54 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d7a956a84f556974daee7c5e1010bfa31d093c5b8b5eaabffa21a4931fe48f7`  
		Last Modified: Thu, 20 Jan 2022 04:31:54 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.13` - linux; arm variant v5

```console
$ docker pull memcached@sha256:d16a2790a88e4662d8340cb85a9660f7738b5abbe759bad21b8f676e0ca8312c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.4 MB (30447722 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7768dab3ed87264de0f4e8a613c070301197408077835da74c7faae6eb6f4bd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 21 Dec 2021 01:50:31 GMT
ADD file:a3023f71bd93966e7db1419adda3ccde4fcc5e2e8cf58e7b13c51036ed5ff796 in / 
# Tue, 21 Dec 2021 01:50:32 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 03:35:35 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 21 Dec 2021 03:35:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 19 Jan 2022 23:48:42 GMT
ENV MEMCACHED_VERSION=1.6.13
# Wed, 19 Jan 2022 23:48:43 GMT
ENV MEMCACHED_SHA1=b9da57ba63ba8de8a980fe0fe2fedc8d59e1dfe3
# Wed, 19 Jan 2022 23:54:08 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 19 Jan 2022 23:54:09 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 19 Jan 2022 23:54:13 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 19 Jan 2022 23:54:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 19 Jan 2022 23:54:14 GMT
USER memcache
# Wed, 19 Jan 2022 23:54:15 GMT
EXPOSE 11211
# Wed, 19 Jan 2022 23:54:16 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:054429d0cf4038fef39a3b5eb6ce52f600f9a2cbb71a4fb3e95ecf9b2da62581`  
		Last Modified: Tue, 21 Dec 2021 02:05:52 GMT  
		Size: 28.9 MB (28900253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb7fdf670368bfde88ac158623eeda4b36ce64bd838e78a9ffcd3d2622eea2e8`  
		Last Modified: Tue, 21 Dec 2021 03:41:18 GMT  
		Size: 4.9 KB (4893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21508b31a1593117f5747b299da29b6bec5fb36f008effcd821336ebafc8ad70`  
		Last Modified: Tue, 21 Dec 2021 03:41:18 GMT  
		Size: 316.6 KB (316576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6d782b9d573913a26c43aba467d4fed6b33af9b83f44cfb1e8f63a76f92ab3a`  
		Last Modified: Wed, 19 Jan 2022 23:55:13 GMT  
		Size: 1.2 MB (1225592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b184c6b4181672a28be507397bd5d2baad8db49549bba6940adb30ce28c3320`  
		Last Modified: Wed, 19 Jan 2022 23:55:12 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73e44f9f60691acb75f8287e5a5eaa0675e04ffbc1fa1e4abfe57733ca7aa595`  
		Last Modified: Wed, 19 Jan 2022 23:55:12 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.13` - linux; arm variant v7

```console
$ docker pull memcached@sha256:7f4a3e4bd6d3845da89e6e1fa7ee377f050118bd20803a8716e7c8aab31670ee
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.1 MB (28078674 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d0493346f5301d1fac3c1ee8eb4df2a8f1791ec73c16d2425aa56be76aabae7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:08 GMT
ADD file:7f27f5b43b7cb04e509fe145266d9bdeacfcacb024cafac32e57ef1c831d5ea7 in / 
# Wed, 26 Jan 2022 01:42:09 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 08:54:44 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 26 Jan 2022 08:54:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 08:54:52 GMT
ENV MEMCACHED_VERSION=1.6.13
# Wed, 26 Jan 2022 08:54:52 GMT
ENV MEMCACHED_SHA1=b9da57ba63ba8de8a980fe0fe2fedc8d59e1dfe3
# Wed, 26 Jan 2022 08:59:15 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 26 Jan 2022 08:59:16 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 26 Jan 2022 08:59:18 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 26 Jan 2022 08:59:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Jan 2022 08:59:18 GMT
USER memcache
# Wed, 26 Jan 2022 08:59:19 GMT
EXPOSE 11211
# Wed, 26 Jan 2022 08:59:19 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:aaef1f1162ec03e01b5b955d41da400544ec2374093ae3dbc330ab2bb36df3e1`  
		Last Modified: Wed, 26 Jan 2022 01:57:59 GMT  
		Size: 26.6 MB (26564933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c9d3dbbb6d5b3a74ea3807c462c99fc02f7ef46831734a98ab085fbfd45d84c`  
		Last Modified: Wed, 26 Jan 2022 09:13:01 GMT  
		Size: 4.9 KB (4894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c553a44b8d98c757ba52201bd5897c9b84bed862d1f1a33b30eaee164faf002`  
		Last Modified: Wed, 26 Jan 2022 09:13:02 GMT  
		Size: 312.0 KB (312023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e05d6d11f4c98f66add6994ad62c7fe25432ba441f2618ba25e8d572c66fe89`  
		Last Modified: Wed, 26 Jan 2022 09:13:02 GMT  
		Size: 1.2 MB (1196416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:902b4740d93b1e9cdd39f484a29d2e022801b8f4612ddd6471c63d0d5aee77c7`  
		Last Modified: Wed, 26 Jan 2022 09:13:01 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0813f5460d7241e77461d216cec438321996a8a74a205fd5a63e3a6e7300ec08`  
		Last Modified: Wed, 26 Jan 2022 09:13:01 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.13` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:97cdec366a180179780e13eb6ab3b4839bd7ce753737ed9b69c45d5baf9d55e0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.4 MB (31434947 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9182bae18682935ee16f416121710ff59a5021e8148d558c7df06caa35e422c5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:31 GMT
ADD file:0ec6f47a8857bf8e6cef71ed8f864be7ce1790ff6ed04fd4201e7dbde4728d3a in / 
# Wed, 26 Jan 2022 01:42:31 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 04:50:24 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 26 Jan 2022 04:50:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 04:50:28 GMT
ENV MEMCACHED_VERSION=1.6.13
# Wed, 26 Jan 2022 04:50:29 GMT
ENV MEMCACHED_SHA1=b9da57ba63ba8de8a980fe0fe2fedc8d59e1dfe3
# Wed, 26 Jan 2022 04:53:09 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 26 Jan 2022 04:53:10 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 26 Jan 2022 04:53:10 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 26 Jan 2022 04:53:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Jan 2022 04:53:12 GMT
USER memcache
# Wed, 26 Jan 2022 04:53:13 GMT
EXPOSE 11211
# Wed, 26 Jan 2022 04:53:14 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:8998bd30e6a1204d13403045766edbe14f941b52087465f5d140ab63c8b113bf`  
		Last Modified: Wed, 26 Jan 2022 01:49:04 GMT  
		Size: 30.1 MB (30056774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a59fc24ed29770b5c2f4352a96e8a82fa286fa87df96964968e2fb2796e105ac`  
		Last Modified: Wed, 26 Jan 2022 04:53:58 GMT  
		Size: 4.9 KB (4900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54853adf97755cd00bf2b960a7a7458bfc9824d4847b0f97e7e5f41e86b6c351`  
		Last Modified: Wed, 26 Jan 2022 04:53:59 GMT  
		Size: 119.2 KB (119210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bc43135274188258180f193f3f9907dd72b6b09963f1886610f28977741356a`  
		Last Modified: Wed, 26 Jan 2022 04:53:59 GMT  
		Size: 1.3 MB (1253657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e306557d5e40e37e762e103bd520b6153919316e8d64e4ae3d21fa66d6420f3`  
		Last Modified: Wed, 26 Jan 2022 04:53:59 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86f1b169766c42ff4dabdf96ef26f2207f4f9fa4fdf13b53c3625a106c50ca12`  
		Last Modified: Wed, 26 Jan 2022 04:53:58 GMT  
		Size: 120.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.13` - linux; 386

```console
$ docker pull memcached@sha256:caebaf527ba0576d76c6d7579c1c921d78dcd0522d3dbe11a11c5ebc1c05b37b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.0 MB (33971560 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f0d964750c0182cb6e1376d8eec8982b36ab1b3aa6f8ab59919f116da2625871`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 26 Jan 2022 01:39:55 GMT
ADD file:876ebf07c65841f4840842086c883af48e07386964fe6d643ba193895ec2a582 in / 
# Wed, 26 Jan 2022 01:39:56 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 08:45:04 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 26 Jan 2022 08:45:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 08:45:09 GMT
ENV MEMCACHED_VERSION=1.6.13
# Wed, 26 Jan 2022 08:45:09 GMT
ENV MEMCACHED_SHA1=b9da57ba63ba8de8a980fe0fe2fedc8d59e1dfe3
# Wed, 26 Jan 2022 08:49:29 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 26 Jan 2022 08:49:29 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 26 Jan 2022 08:49:30 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 26 Jan 2022 08:49:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Jan 2022 08:49:31 GMT
USER memcache
# Wed, 26 Jan 2022 08:49:31 GMT
EXPOSE 11211
# Wed, 26 Jan 2022 08:49:31 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:86933886b1754aba091548cf031a9bca88cdce9bb4fc1f28bb38b61594c2c2c7`  
		Last Modified: Wed, 26 Jan 2022 01:48:57 GMT  
		Size: 32.4 MB (32377406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84bd6e2dff27e256b3baec641bd7c64e8a138237c2c259a806d0f9a9fb1d2255`  
		Last Modified: Wed, 26 Jan 2022 08:50:25 GMT  
		Size: 4.9 KB (4896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d8c7dc83b8d6601d80421931237cbfcd968616d9910fad6f78ee1706ee8f1e3`  
		Last Modified: Wed, 26 Jan 2022 08:50:26 GMT  
		Size: 336.6 KB (336627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5e3e4cf9c8423bfa3e769914fdcf235f6b64837f5fb62f5ccc09a8d792a268c`  
		Last Modified: Wed, 26 Jan 2022 08:50:26 GMT  
		Size: 1.3 MB (1252223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6402d600344325d49706165f2b0feec85cd2421776889433e4c45230bc89b7ee`  
		Last Modified: Wed, 26 Jan 2022 08:50:25 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9fa9c73a03d6ce53a9ea22b31db2648aa6a02a1779ae0a5b19070fbbe806125`  
		Last Modified: Wed, 26 Jan 2022 08:50:25 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.13` - linux; mips64le

```console
$ docker pull memcached@sha256:0848c96207329a581151eeefb1a2b5f1c13893e01667962c71ed108ba448ec8a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.2 MB (31212144 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5691adbb93dbe11492ece526682692fc23ae3869ddd09a5cc20fc92abe25fa68`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:45 GMT
ADD file:61767027a5ab46afbcd4079d200abe8d663326adc96fa28ca8c8955a06d9322e in / 
# Wed, 26 Jan 2022 01:42:46 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 04:16:54 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 26 Jan 2022 04:17:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 04:17:06 GMT
ENV MEMCACHED_VERSION=1.6.13
# Wed, 26 Jan 2022 04:17:07 GMT
ENV MEMCACHED_SHA1=b9da57ba63ba8de8a980fe0fe2fedc8d59e1dfe3
# Wed, 26 Jan 2022 04:23:00 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 26 Jan 2022 04:23:00 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 26 Jan 2022 04:23:02 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 26 Jan 2022 04:23:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Jan 2022 04:23:03 GMT
USER memcache
# Wed, 26 Jan 2022 04:23:03 GMT
EXPOSE 11211
# Wed, 26 Jan 2022 04:23:03 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:266e7d2b59483859eaa1711d2afeb25ea4458eeb36b3e909372930db1f834d7f`  
		Last Modified: Wed, 26 Jan 2022 01:51:23 GMT  
		Size: 29.6 MB (29632834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f2c23d84e18c59799194289c3354e30ed9e147411beb83fd8a53a6b0510244e`  
		Last Modified: Wed, 26 Jan 2022 04:23:22 GMT  
		Size: 5.0 KB (4977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e72e725e4f6fb1ddea7af05f25646fbd5f401583a994d00e98f8d9762bdeef1`  
		Last Modified: Wed, 26 Jan 2022 04:23:22 GMT  
		Size: 323.7 KB (323700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a64f2bbfc21569385827a44c22dc4d96a9004879a3db5a479ac796150f31a89`  
		Last Modified: Wed, 26 Jan 2022 04:23:23 GMT  
		Size: 1.3 MB (1250226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10ec607308395a4822bcdf6d4c2f8665284150145ceaee889026d63b5bbfc525`  
		Last Modified: Wed, 26 Jan 2022 04:23:22 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0544419df418d0761bfd4cee74e348f336fd813c7d70a2ba0f9c66dd4dcad99`  
		Last Modified: Wed, 26 Jan 2022 04:23:22 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.13` - linux; ppc64le

```console
$ docker pull memcached@sha256:467baa60d3118dac94a8d1909db41ec8f8e0867581bba86e83d70d2843299d95
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.0 MB (36956955 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89c206a82af6419284433a55b65259fb3c41ae73d206fc37aa006d7c30d22d0e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 26 Jan 2022 01:46:51 GMT
ADD file:c03f34c221e57fa5cb625c166d1db9f72d6ba2fa17a3c41a5d04d6875d098949 in / 
# Wed, 26 Jan 2022 01:46:57 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 05:38:39 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 26 Jan 2022 05:38:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 05:38:55 GMT
ENV MEMCACHED_VERSION=1.6.13
# Wed, 26 Jan 2022 05:38:58 GMT
ENV MEMCACHED_SHA1=b9da57ba63ba8de8a980fe0fe2fedc8d59e1dfe3
# Wed, 26 Jan 2022 05:44:08 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 26 Jan 2022 05:44:10 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 26 Jan 2022 05:44:17 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 26 Jan 2022 05:44:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Jan 2022 05:44:24 GMT
USER memcache
# Wed, 26 Jan 2022 05:44:28 GMT
EXPOSE 11211
# Wed, 26 Jan 2022 05:44:32 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:3149ee4a73508a4c39107d64a3fdc1b021626a22a0ac95e62fa0cea49ab77fba`  
		Last Modified: Wed, 26 Jan 2022 01:57:01 GMT  
		Size: 35.3 MB (35273030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07bcb451658eb6d9eace467c2e989d96e53c409eb48347a369e9ad80aadcfe96`  
		Last Modified: Wed, 26 Jan 2022 05:45:22 GMT  
		Size: 5.0 KB (4980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8807782e060aa90873de57b2d3ec277632145f166e9c1e3801c57eea7e595cc`  
		Last Modified: Wed, 26 Jan 2022 05:45:22 GMT  
		Size: 356.9 KB (356905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9214a40cf25dcbbc1d21f60a5512d485bc08156423100a0bb814946e829e3a0e`  
		Last Modified: Wed, 26 Jan 2022 05:45:22 GMT  
		Size: 1.3 MB (1321633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90ee2e08d849858def804d36f370ce894ef499543f6e8a72b9aac42c9e1cc909`  
		Last Modified: Wed, 26 Jan 2022 05:45:22 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6635b7a8817986bc0e4c179ae7d01d924f3017618b34956074b196886d9aaa67`  
		Last Modified: Wed, 26 Jan 2022 05:45:22 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.13` - linux; s390x

```console
$ docker pull memcached@sha256:0f830716b97909822e4fe0394e7907f03695936767866c5e3dde96f89f483b30
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.2 MB (31216717 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e41587da3718a95304af17c726b656832260d3107e24f7811d54a20c5bad539`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 26 Jan 2022 01:41:13 GMT
ADD file:03b224b82f458b08d3b5071e42b67915a3db309332c0fc9229db7cf1148bc1b5 in / 
# Wed, 26 Jan 2022 01:41:15 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 03:32:44 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 26 Jan 2022 03:32:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 03:32:47 GMT
ENV MEMCACHED_VERSION=1.6.13
# Wed, 26 Jan 2022 03:32:48 GMT
ENV MEMCACHED_SHA1=b9da57ba63ba8de8a980fe0fe2fedc8d59e1dfe3
# Wed, 26 Jan 2022 03:36:16 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 26 Jan 2022 03:36:16 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 26 Jan 2022 03:36:16 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 26 Jan 2022 03:36:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Jan 2022 03:36:17 GMT
USER memcache
# Wed, 26 Jan 2022 03:36:17 GMT
EXPOSE 11211
# Wed, 26 Jan 2022 03:36:17 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:70bed29526f8483937e4d2540d19256d30786007c7c321e717e00d2e74700380`  
		Last Modified: Wed, 26 Jan 2022 01:46:57 GMT  
		Size: 29.6 MB (29647071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:531e195eaaf208f50aadc4ec839bd3a8f8d4bb0a35dea07bb0e27335fcf6db05`  
		Last Modified: Wed, 26 Jan 2022 03:37:15 GMT  
		Size: 5.0 KB (5026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1072031f118cfb7a6e47244d0bc6a66ac9a2cd286044b62e34033f655f0166d`  
		Last Modified: Wed, 26 Jan 2022 03:37:16 GMT  
		Size: 324.1 KB (324144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3719ec4f04cc9c989d6e8fb755b61510a0e78a3d35107b06cfc6c109c5aac17d`  
		Last Modified: Wed, 26 Jan 2022 03:37:16 GMT  
		Size: 1.2 MB (1240067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c8553e94280409bcb797ba67589732c286468e57828ea58da8d393d5b25a881`  
		Last Modified: Wed, 26 Jan 2022 03:37:16 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de608eaa9aaa185e5049d6baf7896898fe3d2c6beef1fcac73855ec782e15eee`  
		Last Modified: Wed, 26 Jan 2022 03:37:16 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:1.6.13-alpine`

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

### `memcached:1.6.13-alpine` - linux; amd64

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

### `memcached:1.6.13-alpine` - linux; arm64 variant v8

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

### `memcached:1.6.13-alpine` - linux; 386

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

### `memcached:1.6.13-alpine` - linux; ppc64le

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

### `memcached:1.6.13-alpine` - linux; s390x

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

## `memcached:1.6.13-alpine3.15`

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

### `memcached:1.6.13-alpine3.15` - linux; amd64

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

### `memcached:1.6.13-alpine3.15` - linux; arm64 variant v8

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

### `memcached:1.6.13-alpine3.15` - linux; 386

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

### `memcached:1.6.13-alpine3.15` - linux; ppc64le

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

### `memcached:1.6.13-alpine3.15` - linux; s390x

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

## `memcached:1.6.13-bullseye`

```console
$ docker pull memcached@sha256:61a8c3887d91c23aa6ce62b145b6e77acb1bcf195e950b3971f4007f2a47fa12
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

### `memcached:1.6.13-bullseye` - linux; amd64

```console
$ docker pull memcached@sha256:c9756ec03bedf0411e142fa016cce653157ef46216102b2ad9012ba57a69e9b5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.9 MB (32945941 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c8b63b0eeb514dca60290d594b69ba36d42534eb7c4af27ceb25c4b900d862c8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 21 Dec 2021 01:22:43 GMT
ADD file:09675d11695f65c55efdc393ff0cd32f30194cd7d0fbef4631eebfed4414ac97 in / 
# Tue, 21 Dec 2021 01:22:43 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 18:34:30 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 21 Dec 2021 18:34:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 20 Jan 2022 04:23:06 GMT
ENV MEMCACHED_VERSION=1.6.13
# Thu, 20 Jan 2022 04:23:06 GMT
ENV MEMCACHED_SHA1=b9da57ba63ba8de8a980fe0fe2fedc8d59e1dfe3
# Thu, 20 Jan 2022 04:27:08 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 20 Jan 2022 04:27:08 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 20 Jan 2022 04:27:09 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 20 Jan 2022 04:27:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 20 Jan 2022 04:27:09 GMT
USER memcache
# Thu, 20 Jan 2022 04:27:10 GMT
EXPOSE 11211
# Thu, 20 Jan 2022 04:27:10 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:a2abf6c4d29d43a4bf9fbb769f524d0fb36a2edab49819c1bf3e76f409f953ea`  
		Last Modified: Tue, 21 Dec 2021 01:27:48 GMT  
		Size: 31.4 MB (31357624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aa5be68e24cfc338b0c9be41213371a3ed596d00487ad58df6494ed46626117`  
		Last Modified: Tue, 21 Dec 2021 18:39:12 GMT  
		Size: 5.0 KB (4978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:052b406b20ce6593c7a47bc0d4d4f8b45258c1aed8b86ab06c0fc75ab6b4ee40`  
		Last Modified: Tue, 21 Dec 2021 18:39:13 GMT  
		Size: 328.1 KB (328055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b89359883409361f4bb025aaae623b73503a2801842fa3ceda2711924cf71b5`  
		Last Modified: Thu, 20 Jan 2022 04:31:55 GMT  
		Size: 1.3 MB (1254875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f5e296124091603e6ac2227e0bb1a6cde6faafa7608b926488a5d003b20d987`  
		Last Modified: Thu, 20 Jan 2022 04:31:54 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d7a956a84f556974daee7c5e1010bfa31d093c5b8b5eaabffa21a4931fe48f7`  
		Last Modified: Thu, 20 Jan 2022 04:31:54 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.13-bullseye` - linux; arm variant v5

```console
$ docker pull memcached@sha256:d16a2790a88e4662d8340cb85a9660f7738b5abbe759bad21b8f676e0ca8312c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.4 MB (30447722 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7768dab3ed87264de0f4e8a613c070301197408077835da74c7faae6eb6f4bd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 21 Dec 2021 01:50:31 GMT
ADD file:a3023f71bd93966e7db1419adda3ccde4fcc5e2e8cf58e7b13c51036ed5ff796 in / 
# Tue, 21 Dec 2021 01:50:32 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 03:35:35 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 21 Dec 2021 03:35:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 19 Jan 2022 23:48:42 GMT
ENV MEMCACHED_VERSION=1.6.13
# Wed, 19 Jan 2022 23:48:43 GMT
ENV MEMCACHED_SHA1=b9da57ba63ba8de8a980fe0fe2fedc8d59e1dfe3
# Wed, 19 Jan 2022 23:54:08 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 19 Jan 2022 23:54:09 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 19 Jan 2022 23:54:13 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 19 Jan 2022 23:54:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 19 Jan 2022 23:54:14 GMT
USER memcache
# Wed, 19 Jan 2022 23:54:15 GMT
EXPOSE 11211
# Wed, 19 Jan 2022 23:54:16 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:054429d0cf4038fef39a3b5eb6ce52f600f9a2cbb71a4fb3e95ecf9b2da62581`  
		Last Modified: Tue, 21 Dec 2021 02:05:52 GMT  
		Size: 28.9 MB (28900253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb7fdf670368bfde88ac158623eeda4b36ce64bd838e78a9ffcd3d2622eea2e8`  
		Last Modified: Tue, 21 Dec 2021 03:41:18 GMT  
		Size: 4.9 KB (4893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21508b31a1593117f5747b299da29b6bec5fb36f008effcd821336ebafc8ad70`  
		Last Modified: Tue, 21 Dec 2021 03:41:18 GMT  
		Size: 316.6 KB (316576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6d782b9d573913a26c43aba467d4fed6b33af9b83f44cfb1e8f63a76f92ab3a`  
		Last Modified: Wed, 19 Jan 2022 23:55:13 GMT  
		Size: 1.2 MB (1225592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b184c6b4181672a28be507397bd5d2baad8db49549bba6940adb30ce28c3320`  
		Last Modified: Wed, 19 Jan 2022 23:55:12 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73e44f9f60691acb75f8287e5a5eaa0675e04ffbc1fa1e4abfe57733ca7aa595`  
		Last Modified: Wed, 19 Jan 2022 23:55:12 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.13-bullseye` - linux; arm variant v7

```console
$ docker pull memcached@sha256:7f4a3e4bd6d3845da89e6e1fa7ee377f050118bd20803a8716e7c8aab31670ee
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.1 MB (28078674 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d0493346f5301d1fac3c1ee8eb4df2a8f1791ec73c16d2425aa56be76aabae7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:08 GMT
ADD file:7f27f5b43b7cb04e509fe145266d9bdeacfcacb024cafac32e57ef1c831d5ea7 in / 
# Wed, 26 Jan 2022 01:42:09 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 08:54:44 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 26 Jan 2022 08:54:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 08:54:52 GMT
ENV MEMCACHED_VERSION=1.6.13
# Wed, 26 Jan 2022 08:54:52 GMT
ENV MEMCACHED_SHA1=b9da57ba63ba8de8a980fe0fe2fedc8d59e1dfe3
# Wed, 26 Jan 2022 08:59:15 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 26 Jan 2022 08:59:16 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 26 Jan 2022 08:59:18 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 26 Jan 2022 08:59:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Jan 2022 08:59:18 GMT
USER memcache
# Wed, 26 Jan 2022 08:59:19 GMT
EXPOSE 11211
# Wed, 26 Jan 2022 08:59:19 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:aaef1f1162ec03e01b5b955d41da400544ec2374093ae3dbc330ab2bb36df3e1`  
		Last Modified: Wed, 26 Jan 2022 01:57:59 GMT  
		Size: 26.6 MB (26564933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c9d3dbbb6d5b3a74ea3807c462c99fc02f7ef46831734a98ab085fbfd45d84c`  
		Last Modified: Wed, 26 Jan 2022 09:13:01 GMT  
		Size: 4.9 KB (4894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c553a44b8d98c757ba52201bd5897c9b84bed862d1f1a33b30eaee164faf002`  
		Last Modified: Wed, 26 Jan 2022 09:13:02 GMT  
		Size: 312.0 KB (312023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e05d6d11f4c98f66add6994ad62c7fe25432ba441f2618ba25e8d572c66fe89`  
		Last Modified: Wed, 26 Jan 2022 09:13:02 GMT  
		Size: 1.2 MB (1196416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:902b4740d93b1e9cdd39f484a29d2e022801b8f4612ddd6471c63d0d5aee77c7`  
		Last Modified: Wed, 26 Jan 2022 09:13:01 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0813f5460d7241e77461d216cec438321996a8a74a205fd5a63e3a6e7300ec08`  
		Last Modified: Wed, 26 Jan 2022 09:13:01 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.13-bullseye` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:97cdec366a180179780e13eb6ab3b4839bd7ce753737ed9b69c45d5baf9d55e0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.4 MB (31434947 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9182bae18682935ee16f416121710ff59a5021e8148d558c7df06caa35e422c5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:31 GMT
ADD file:0ec6f47a8857bf8e6cef71ed8f864be7ce1790ff6ed04fd4201e7dbde4728d3a in / 
# Wed, 26 Jan 2022 01:42:31 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 04:50:24 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 26 Jan 2022 04:50:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 04:50:28 GMT
ENV MEMCACHED_VERSION=1.6.13
# Wed, 26 Jan 2022 04:50:29 GMT
ENV MEMCACHED_SHA1=b9da57ba63ba8de8a980fe0fe2fedc8d59e1dfe3
# Wed, 26 Jan 2022 04:53:09 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 26 Jan 2022 04:53:10 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 26 Jan 2022 04:53:10 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 26 Jan 2022 04:53:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Jan 2022 04:53:12 GMT
USER memcache
# Wed, 26 Jan 2022 04:53:13 GMT
EXPOSE 11211
# Wed, 26 Jan 2022 04:53:14 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:8998bd30e6a1204d13403045766edbe14f941b52087465f5d140ab63c8b113bf`  
		Last Modified: Wed, 26 Jan 2022 01:49:04 GMT  
		Size: 30.1 MB (30056774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a59fc24ed29770b5c2f4352a96e8a82fa286fa87df96964968e2fb2796e105ac`  
		Last Modified: Wed, 26 Jan 2022 04:53:58 GMT  
		Size: 4.9 KB (4900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54853adf97755cd00bf2b960a7a7458bfc9824d4847b0f97e7e5f41e86b6c351`  
		Last Modified: Wed, 26 Jan 2022 04:53:59 GMT  
		Size: 119.2 KB (119210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bc43135274188258180f193f3f9907dd72b6b09963f1886610f28977741356a`  
		Last Modified: Wed, 26 Jan 2022 04:53:59 GMT  
		Size: 1.3 MB (1253657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e306557d5e40e37e762e103bd520b6153919316e8d64e4ae3d21fa66d6420f3`  
		Last Modified: Wed, 26 Jan 2022 04:53:59 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86f1b169766c42ff4dabdf96ef26f2207f4f9fa4fdf13b53c3625a106c50ca12`  
		Last Modified: Wed, 26 Jan 2022 04:53:58 GMT  
		Size: 120.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.13-bullseye` - linux; 386

```console
$ docker pull memcached@sha256:caebaf527ba0576d76c6d7579c1c921d78dcd0522d3dbe11a11c5ebc1c05b37b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.0 MB (33971560 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f0d964750c0182cb6e1376d8eec8982b36ab1b3aa6f8ab59919f116da2625871`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 26 Jan 2022 01:39:55 GMT
ADD file:876ebf07c65841f4840842086c883af48e07386964fe6d643ba193895ec2a582 in / 
# Wed, 26 Jan 2022 01:39:56 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 08:45:04 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 26 Jan 2022 08:45:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 08:45:09 GMT
ENV MEMCACHED_VERSION=1.6.13
# Wed, 26 Jan 2022 08:45:09 GMT
ENV MEMCACHED_SHA1=b9da57ba63ba8de8a980fe0fe2fedc8d59e1dfe3
# Wed, 26 Jan 2022 08:49:29 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 26 Jan 2022 08:49:29 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 26 Jan 2022 08:49:30 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 26 Jan 2022 08:49:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Jan 2022 08:49:31 GMT
USER memcache
# Wed, 26 Jan 2022 08:49:31 GMT
EXPOSE 11211
# Wed, 26 Jan 2022 08:49:31 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:86933886b1754aba091548cf031a9bca88cdce9bb4fc1f28bb38b61594c2c2c7`  
		Last Modified: Wed, 26 Jan 2022 01:48:57 GMT  
		Size: 32.4 MB (32377406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84bd6e2dff27e256b3baec641bd7c64e8a138237c2c259a806d0f9a9fb1d2255`  
		Last Modified: Wed, 26 Jan 2022 08:50:25 GMT  
		Size: 4.9 KB (4896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d8c7dc83b8d6601d80421931237cbfcd968616d9910fad6f78ee1706ee8f1e3`  
		Last Modified: Wed, 26 Jan 2022 08:50:26 GMT  
		Size: 336.6 KB (336627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5e3e4cf9c8423bfa3e769914fdcf235f6b64837f5fb62f5ccc09a8d792a268c`  
		Last Modified: Wed, 26 Jan 2022 08:50:26 GMT  
		Size: 1.3 MB (1252223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6402d600344325d49706165f2b0feec85cd2421776889433e4c45230bc89b7ee`  
		Last Modified: Wed, 26 Jan 2022 08:50:25 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9fa9c73a03d6ce53a9ea22b31db2648aa6a02a1779ae0a5b19070fbbe806125`  
		Last Modified: Wed, 26 Jan 2022 08:50:25 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.13-bullseye` - linux; mips64le

```console
$ docker pull memcached@sha256:0848c96207329a581151eeefb1a2b5f1c13893e01667962c71ed108ba448ec8a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.2 MB (31212144 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5691adbb93dbe11492ece526682692fc23ae3869ddd09a5cc20fc92abe25fa68`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:45 GMT
ADD file:61767027a5ab46afbcd4079d200abe8d663326adc96fa28ca8c8955a06d9322e in / 
# Wed, 26 Jan 2022 01:42:46 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 04:16:54 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 26 Jan 2022 04:17:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 04:17:06 GMT
ENV MEMCACHED_VERSION=1.6.13
# Wed, 26 Jan 2022 04:17:07 GMT
ENV MEMCACHED_SHA1=b9da57ba63ba8de8a980fe0fe2fedc8d59e1dfe3
# Wed, 26 Jan 2022 04:23:00 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 26 Jan 2022 04:23:00 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 26 Jan 2022 04:23:02 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 26 Jan 2022 04:23:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Jan 2022 04:23:03 GMT
USER memcache
# Wed, 26 Jan 2022 04:23:03 GMT
EXPOSE 11211
# Wed, 26 Jan 2022 04:23:03 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:266e7d2b59483859eaa1711d2afeb25ea4458eeb36b3e909372930db1f834d7f`  
		Last Modified: Wed, 26 Jan 2022 01:51:23 GMT  
		Size: 29.6 MB (29632834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f2c23d84e18c59799194289c3354e30ed9e147411beb83fd8a53a6b0510244e`  
		Last Modified: Wed, 26 Jan 2022 04:23:22 GMT  
		Size: 5.0 KB (4977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e72e725e4f6fb1ddea7af05f25646fbd5f401583a994d00e98f8d9762bdeef1`  
		Last Modified: Wed, 26 Jan 2022 04:23:22 GMT  
		Size: 323.7 KB (323700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a64f2bbfc21569385827a44c22dc4d96a9004879a3db5a479ac796150f31a89`  
		Last Modified: Wed, 26 Jan 2022 04:23:23 GMT  
		Size: 1.3 MB (1250226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10ec607308395a4822bcdf6d4c2f8665284150145ceaee889026d63b5bbfc525`  
		Last Modified: Wed, 26 Jan 2022 04:23:22 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0544419df418d0761bfd4cee74e348f336fd813c7d70a2ba0f9c66dd4dcad99`  
		Last Modified: Wed, 26 Jan 2022 04:23:22 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.13-bullseye` - linux; ppc64le

```console
$ docker pull memcached@sha256:467baa60d3118dac94a8d1909db41ec8f8e0867581bba86e83d70d2843299d95
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.0 MB (36956955 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89c206a82af6419284433a55b65259fb3c41ae73d206fc37aa006d7c30d22d0e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 26 Jan 2022 01:46:51 GMT
ADD file:c03f34c221e57fa5cb625c166d1db9f72d6ba2fa17a3c41a5d04d6875d098949 in / 
# Wed, 26 Jan 2022 01:46:57 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 05:38:39 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 26 Jan 2022 05:38:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 05:38:55 GMT
ENV MEMCACHED_VERSION=1.6.13
# Wed, 26 Jan 2022 05:38:58 GMT
ENV MEMCACHED_SHA1=b9da57ba63ba8de8a980fe0fe2fedc8d59e1dfe3
# Wed, 26 Jan 2022 05:44:08 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 26 Jan 2022 05:44:10 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 26 Jan 2022 05:44:17 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 26 Jan 2022 05:44:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Jan 2022 05:44:24 GMT
USER memcache
# Wed, 26 Jan 2022 05:44:28 GMT
EXPOSE 11211
# Wed, 26 Jan 2022 05:44:32 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:3149ee4a73508a4c39107d64a3fdc1b021626a22a0ac95e62fa0cea49ab77fba`  
		Last Modified: Wed, 26 Jan 2022 01:57:01 GMT  
		Size: 35.3 MB (35273030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07bcb451658eb6d9eace467c2e989d96e53c409eb48347a369e9ad80aadcfe96`  
		Last Modified: Wed, 26 Jan 2022 05:45:22 GMT  
		Size: 5.0 KB (4980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8807782e060aa90873de57b2d3ec277632145f166e9c1e3801c57eea7e595cc`  
		Last Modified: Wed, 26 Jan 2022 05:45:22 GMT  
		Size: 356.9 KB (356905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9214a40cf25dcbbc1d21f60a5512d485bc08156423100a0bb814946e829e3a0e`  
		Last Modified: Wed, 26 Jan 2022 05:45:22 GMT  
		Size: 1.3 MB (1321633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90ee2e08d849858def804d36f370ce894ef499543f6e8a72b9aac42c9e1cc909`  
		Last Modified: Wed, 26 Jan 2022 05:45:22 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6635b7a8817986bc0e4c179ae7d01d924f3017618b34956074b196886d9aaa67`  
		Last Modified: Wed, 26 Jan 2022 05:45:22 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.13-bullseye` - linux; s390x

```console
$ docker pull memcached@sha256:0f830716b97909822e4fe0394e7907f03695936767866c5e3dde96f89f483b30
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.2 MB (31216717 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e41587da3718a95304af17c726b656832260d3107e24f7811d54a20c5bad539`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 26 Jan 2022 01:41:13 GMT
ADD file:03b224b82f458b08d3b5071e42b67915a3db309332c0fc9229db7cf1148bc1b5 in / 
# Wed, 26 Jan 2022 01:41:15 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 03:32:44 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 26 Jan 2022 03:32:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 03:32:47 GMT
ENV MEMCACHED_VERSION=1.6.13
# Wed, 26 Jan 2022 03:32:48 GMT
ENV MEMCACHED_SHA1=b9da57ba63ba8de8a980fe0fe2fedc8d59e1dfe3
# Wed, 26 Jan 2022 03:36:16 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 26 Jan 2022 03:36:16 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 26 Jan 2022 03:36:16 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 26 Jan 2022 03:36:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Jan 2022 03:36:17 GMT
USER memcache
# Wed, 26 Jan 2022 03:36:17 GMT
EXPOSE 11211
# Wed, 26 Jan 2022 03:36:17 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:70bed29526f8483937e4d2540d19256d30786007c7c321e717e00d2e74700380`  
		Last Modified: Wed, 26 Jan 2022 01:46:57 GMT  
		Size: 29.6 MB (29647071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:531e195eaaf208f50aadc4ec839bd3a8f8d4bb0a35dea07bb0e27335fcf6db05`  
		Last Modified: Wed, 26 Jan 2022 03:37:15 GMT  
		Size: 5.0 KB (5026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1072031f118cfb7a6e47244d0bc6a66ac9a2cd286044b62e34033f655f0166d`  
		Last Modified: Wed, 26 Jan 2022 03:37:16 GMT  
		Size: 324.1 KB (324144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3719ec4f04cc9c989d6e8fb755b61510a0e78a3d35107b06cfc6c109c5aac17d`  
		Last Modified: Wed, 26 Jan 2022 03:37:16 GMT  
		Size: 1.2 MB (1240067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c8553e94280409bcb797ba67589732c286468e57828ea58da8d393d5b25a881`  
		Last Modified: Wed, 26 Jan 2022 03:37:16 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de608eaa9aaa185e5049d6baf7896898fe3d2c6beef1fcac73855ec782e15eee`  
		Last Modified: Wed, 26 Jan 2022 03:37:16 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:alpine`

```console
$ docker pull memcached@sha256:4fd74bfdda3c109c25e7edfd6b77545c48963b938d6f75f4fb8c122c5cdae7cd
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

### `memcached:alpine` - linux; 386

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

### `memcached:alpine` - linux; ppc64le

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

### `memcached:alpine` - linux; s390x

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

## `memcached:alpine3.15`

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

### `memcached:alpine3.15` - linux; amd64

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

### `memcached:alpine3.15` - linux; arm64 variant v8

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

### `memcached:alpine3.15` - linux; 386

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

### `memcached:alpine3.15` - linux; ppc64le

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

### `memcached:alpine3.15` - linux; s390x

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

## `memcached:bullseye`

```console
$ docker pull memcached@sha256:61a8c3887d91c23aa6ce62b145b6e77acb1bcf195e950b3971f4007f2a47fa12
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
$ docker pull memcached@sha256:c9756ec03bedf0411e142fa016cce653157ef46216102b2ad9012ba57a69e9b5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.9 MB (32945941 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c8b63b0eeb514dca60290d594b69ba36d42534eb7c4af27ceb25c4b900d862c8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 21 Dec 2021 01:22:43 GMT
ADD file:09675d11695f65c55efdc393ff0cd32f30194cd7d0fbef4631eebfed4414ac97 in / 
# Tue, 21 Dec 2021 01:22:43 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 18:34:30 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 21 Dec 2021 18:34:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 20 Jan 2022 04:23:06 GMT
ENV MEMCACHED_VERSION=1.6.13
# Thu, 20 Jan 2022 04:23:06 GMT
ENV MEMCACHED_SHA1=b9da57ba63ba8de8a980fe0fe2fedc8d59e1dfe3
# Thu, 20 Jan 2022 04:27:08 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 20 Jan 2022 04:27:08 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 20 Jan 2022 04:27:09 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 20 Jan 2022 04:27:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 20 Jan 2022 04:27:09 GMT
USER memcache
# Thu, 20 Jan 2022 04:27:10 GMT
EXPOSE 11211
# Thu, 20 Jan 2022 04:27:10 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:a2abf6c4d29d43a4bf9fbb769f524d0fb36a2edab49819c1bf3e76f409f953ea`  
		Last Modified: Tue, 21 Dec 2021 01:27:48 GMT  
		Size: 31.4 MB (31357624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aa5be68e24cfc338b0c9be41213371a3ed596d00487ad58df6494ed46626117`  
		Last Modified: Tue, 21 Dec 2021 18:39:12 GMT  
		Size: 5.0 KB (4978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:052b406b20ce6593c7a47bc0d4d4f8b45258c1aed8b86ab06c0fc75ab6b4ee40`  
		Last Modified: Tue, 21 Dec 2021 18:39:13 GMT  
		Size: 328.1 KB (328055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b89359883409361f4bb025aaae623b73503a2801842fa3ceda2711924cf71b5`  
		Last Modified: Thu, 20 Jan 2022 04:31:55 GMT  
		Size: 1.3 MB (1254875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f5e296124091603e6ac2227e0bb1a6cde6faafa7608b926488a5d003b20d987`  
		Last Modified: Thu, 20 Jan 2022 04:31:54 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d7a956a84f556974daee7c5e1010bfa31d093c5b8b5eaabffa21a4931fe48f7`  
		Last Modified: Thu, 20 Jan 2022 04:31:54 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:bullseye` - linux; arm variant v5

```console
$ docker pull memcached@sha256:d16a2790a88e4662d8340cb85a9660f7738b5abbe759bad21b8f676e0ca8312c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.4 MB (30447722 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7768dab3ed87264de0f4e8a613c070301197408077835da74c7faae6eb6f4bd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 21 Dec 2021 01:50:31 GMT
ADD file:a3023f71bd93966e7db1419adda3ccde4fcc5e2e8cf58e7b13c51036ed5ff796 in / 
# Tue, 21 Dec 2021 01:50:32 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 03:35:35 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 21 Dec 2021 03:35:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 19 Jan 2022 23:48:42 GMT
ENV MEMCACHED_VERSION=1.6.13
# Wed, 19 Jan 2022 23:48:43 GMT
ENV MEMCACHED_SHA1=b9da57ba63ba8de8a980fe0fe2fedc8d59e1dfe3
# Wed, 19 Jan 2022 23:54:08 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 19 Jan 2022 23:54:09 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 19 Jan 2022 23:54:13 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 19 Jan 2022 23:54:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 19 Jan 2022 23:54:14 GMT
USER memcache
# Wed, 19 Jan 2022 23:54:15 GMT
EXPOSE 11211
# Wed, 19 Jan 2022 23:54:16 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:054429d0cf4038fef39a3b5eb6ce52f600f9a2cbb71a4fb3e95ecf9b2da62581`  
		Last Modified: Tue, 21 Dec 2021 02:05:52 GMT  
		Size: 28.9 MB (28900253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb7fdf670368bfde88ac158623eeda4b36ce64bd838e78a9ffcd3d2622eea2e8`  
		Last Modified: Tue, 21 Dec 2021 03:41:18 GMT  
		Size: 4.9 KB (4893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21508b31a1593117f5747b299da29b6bec5fb36f008effcd821336ebafc8ad70`  
		Last Modified: Tue, 21 Dec 2021 03:41:18 GMT  
		Size: 316.6 KB (316576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6d782b9d573913a26c43aba467d4fed6b33af9b83f44cfb1e8f63a76f92ab3a`  
		Last Modified: Wed, 19 Jan 2022 23:55:13 GMT  
		Size: 1.2 MB (1225592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b184c6b4181672a28be507397bd5d2baad8db49549bba6940adb30ce28c3320`  
		Last Modified: Wed, 19 Jan 2022 23:55:12 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73e44f9f60691acb75f8287e5a5eaa0675e04ffbc1fa1e4abfe57733ca7aa595`  
		Last Modified: Wed, 19 Jan 2022 23:55:12 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:bullseye` - linux; arm variant v7

```console
$ docker pull memcached@sha256:7f4a3e4bd6d3845da89e6e1fa7ee377f050118bd20803a8716e7c8aab31670ee
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.1 MB (28078674 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d0493346f5301d1fac3c1ee8eb4df2a8f1791ec73c16d2425aa56be76aabae7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:08 GMT
ADD file:7f27f5b43b7cb04e509fe145266d9bdeacfcacb024cafac32e57ef1c831d5ea7 in / 
# Wed, 26 Jan 2022 01:42:09 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 08:54:44 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 26 Jan 2022 08:54:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 08:54:52 GMT
ENV MEMCACHED_VERSION=1.6.13
# Wed, 26 Jan 2022 08:54:52 GMT
ENV MEMCACHED_SHA1=b9da57ba63ba8de8a980fe0fe2fedc8d59e1dfe3
# Wed, 26 Jan 2022 08:59:15 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 26 Jan 2022 08:59:16 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 26 Jan 2022 08:59:18 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 26 Jan 2022 08:59:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Jan 2022 08:59:18 GMT
USER memcache
# Wed, 26 Jan 2022 08:59:19 GMT
EXPOSE 11211
# Wed, 26 Jan 2022 08:59:19 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:aaef1f1162ec03e01b5b955d41da400544ec2374093ae3dbc330ab2bb36df3e1`  
		Last Modified: Wed, 26 Jan 2022 01:57:59 GMT  
		Size: 26.6 MB (26564933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c9d3dbbb6d5b3a74ea3807c462c99fc02f7ef46831734a98ab085fbfd45d84c`  
		Last Modified: Wed, 26 Jan 2022 09:13:01 GMT  
		Size: 4.9 KB (4894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c553a44b8d98c757ba52201bd5897c9b84bed862d1f1a33b30eaee164faf002`  
		Last Modified: Wed, 26 Jan 2022 09:13:02 GMT  
		Size: 312.0 KB (312023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e05d6d11f4c98f66add6994ad62c7fe25432ba441f2618ba25e8d572c66fe89`  
		Last Modified: Wed, 26 Jan 2022 09:13:02 GMT  
		Size: 1.2 MB (1196416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:902b4740d93b1e9cdd39f484a29d2e022801b8f4612ddd6471c63d0d5aee77c7`  
		Last Modified: Wed, 26 Jan 2022 09:13:01 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0813f5460d7241e77461d216cec438321996a8a74a205fd5a63e3a6e7300ec08`  
		Last Modified: Wed, 26 Jan 2022 09:13:01 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:bullseye` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:97cdec366a180179780e13eb6ab3b4839bd7ce753737ed9b69c45d5baf9d55e0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.4 MB (31434947 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9182bae18682935ee16f416121710ff59a5021e8148d558c7df06caa35e422c5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:31 GMT
ADD file:0ec6f47a8857bf8e6cef71ed8f864be7ce1790ff6ed04fd4201e7dbde4728d3a in / 
# Wed, 26 Jan 2022 01:42:31 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 04:50:24 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 26 Jan 2022 04:50:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 04:50:28 GMT
ENV MEMCACHED_VERSION=1.6.13
# Wed, 26 Jan 2022 04:50:29 GMT
ENV MEMCACHED_SHA1=b9da57ba63ba8de8a980fe0fe2fedc8d59e1dfe3
# Wed, 26 Jan 2022 04:53:09 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 26 Jan 2022 04:53:10 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 26 Jan 2022 04:53:10 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 26 Jan 2022 04:53:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Jan 2022 04:53:12 GMT
USER memcache
# Wed, 26 Jan 2022 04:53:13 GMT
EXPOSE 11211
# Wed, 26 Jan 2022 04:53:14 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:8998bd30e6a1204d13403045766edbe14f941b52087465f5d140ab63c8b113bf`  
		Last Modified: Wed, 26 Jan 2022 01:49:04 GMT  
		Size: 30.1 MB (30056774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a59fc24ed29770b5c2f4352a96e8a82fa286fa87df96964968e2fb2796e105ac`  
		Last Modified: Wed, 26 Jan 2022 04:53:58 GMT  
		Size: 4.9 KB (4900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54853adf97755cd00bf2b960a7a7458bfc9824d4847b0f97e7e5f41e86b6c351`  
		Last Modified: Wed, 26 Jan 2022 04:53:59 GMT  
		Size: 119.2 KB (119210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bc43135274188258180f193f3f9907dd72b6b09963f1886610f28977741356a`  
		Last Modified: Wed, 26 Jan 2022 04:53:59 GMT  
		Size: 1.3 MB (1253657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e306557d5e40e37e762e103bd520b6153919316e8d64e4ae3d21fa66d6420f3`  
		Last Modified: Wed, 26 Jan 2022 04:53:59 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86f1b169766c42ff4dabdf96ef26f2207f4f9fa4fdf13b53c3625a106c50ca12`  
		Last Modified: Wed, 26 Jan 2022 04:53:58 GMT  
		Size: 120.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:bullseye` - linux; 386

```console
$ docker pull memcached@sha256:caebaf527ba0576d76c6d7579c1c921d78dcd0522d3dbe11a11c5ebc1c05b37b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.0 MB (33971560 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f0d964750c0182cb6e1376d8eec8982b36ab1b3aa6f8ab59919f116da2625871`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 26 Jan 2022 01:39:55 GMT
ADD file:876ebf07c65841f4840842086c883af48e07386964fe6d643ba193895ec2a582 in / 
# Wed, 26 Jan 2022 01:39:56 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 08:45:04 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 26 Jan 2022 08:45:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 08:45:09 GMT
ENV MEMCACHED_VERSION=1.6.13
# Wed, 26 Jan 2022 08:45:09 GMT
ENV MEMCACHED_SHA1=b9da57ba63ba8de8a980fe0fe2fedc8d59e1dfe3
# Wed, 26 Jan 2022 08:49:29 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 26 Jan 2022 08:49:29 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 26 Jan 2022 08:49:30 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 26 Jan 2022 08:49:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Jan 2022 08:49:31 GMT
USER memcache
# Wed, 26 Jan 2022 08:49:31 GMT
EXPOSE 11211
# Wed, 26 Jan 2022 08:49:31 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:86933886b1754aba091548cf031a9bca88cdce9bb4fc1f28bb38b61594c2c2c7`  
		Last Modified: Wed, 26 Jan 2022 01:48:57 GMT  
		Size: 32.4 MB (32377406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84bd6e2dff27e256b3baec641bd7c64e8a138237c2c259a806d0f9a9fb1d2255`  
		Last Modified: Wed, 26 Jan 2022 08:50:25 GMT  
		Size: 4.9 KB (4896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d8c7dc83b8d6601d80421931237cbfcd968616d9910fad6f78ee1706ee8f1e3`  
		Last Modified: Wed, 26 Jan 2022 08:50:26 GMT  
		Size: 336.6 KB (336627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5e3e4cf9c8423bfa3e769914fdcf235f6b64837f5fb62f5ccc09a8d792a268c`  
		Last Modified: Wed, 26 Jan 2022 08:50:26 GMT  
		Size: 1.3 MB (1252223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6402d600344325d49706165f2b0feec85cd2421776889433e4c45230bc89b7ee`  
		Last Modified: Wed, 26 Jan 2022 08:50:25 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9fa9c73a03d6ce53a9ea22b31db2648aa6a02a1779ae0a5b19070fbbe806125`  
		Last Modified: Wed, 26 Jan 2022 08:50:25 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:bullseye` - linux; mips64le

```console
$ docker pull memcached@sha256:0848c96207329a581151eeefb1a2b5f1c13893e01667962c71ed108ba448ec8a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.2 MB (31212144 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5691adbb93dbe11492ece526682692fc23ae3869ddd09a5cc20fc92abe25fa68`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:45 GMT
ADD file:61767027a5ab46afbcd4079d200abe8d663326adc96fa28ca8c8955a06d9322e in / 
# Wed, 26 Jan 2022 01:42:46 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 04:16:54 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 26 Jan 2022 04:17:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 04:17:06 GMT
ENV MEMCACHED_VERSION=1.6.13
# Wed, 26 Jan 2022 04:17:07 GMT
ENV MEMCACHED_SHA1=b9da57ba63ba8de8a980fe0fe2fedc8d59e1dfe3
# Wed, 26 Jan 2022 04:23:00 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 26 Jan 2022 04:23:00 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 26 Jan 2022 04:23:02 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 26 Jan 2022 04:23:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Jan 2022 04:23:03 GMT
USER memcache
# Wed, 26 Jan 2022 04:23:03 GMT
EXPOSE 11211
# Wed, 26 Jan 2022 04:23:03 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:266e7d2b59483859eaa1711d2afeb25ea4458eeb36b3e909372930db1f834d7f`  
		Last Modified: Wed, 26 Jan 2022 01:51:23 GMT  
		Size: 29.6 MB (29632834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f2c23d84e18c59799194289c3354e30ed9e147411beb83fd8a53a6b0510244e`  
		Last Modified: Wed, 26 Jan 2022 04:23:22 GMT  
		Size: 5.0 KB (4977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e72e725e4f6fb1ddea7af05f25646fbd5f401583a994d00e98f8d9762bdeef1`  
		Last Modified: Wed, 26 Jan 2022 04:23:22 GMT  
		Size: 323.7 KB (323700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a64f2bbfc21569385827a44c22dc4d96a9004879a3db5a479ac796150f31a89`  
		Last Modified: Wed, 26 Jan 2022 04:23:23 GMT  
		Size: 1.3 MB (1250226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10ec607308395a4822bcdf6d4c2f8665284150145ceaee889026d63b5bbfc525`  
		Last Modified: Wed, 26 Jan 2022 04:23:22 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0544419df418d0761bfd4cee74e348f336fd813c7d70a2ba0f9c66dd4dcad99`  
		Last Modified: Wed, 26 Jan 2022 04:23:22 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:bullseye` - linux; ppc64le

```console
$ docker pull memcached@sha256:467baa60d3118dac94a8d1909db41ec8f8e0867581bba86e83d70d2843299d95
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.0 MB (36956955 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89c206a82af6419284433a55b65259fb3c41ae73d206fc37aa006d7c30d22d0e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 26 Jan 2022 01:46:51 GMT
ADD file:c03f34c221e57fa5cb625c166d1db9f72d6ba2fa17a3c41a5d04d6875d098949 in / 
# Wed, 26 Jan 2022 01:46:57 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 05:38:39 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 26 Jan 2022 05:38:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 05:38:55 GMT
ENV MEMCACHED_VERSION=1.6.13
# Wed, 26 Jan 2022 05:38:58 GMT
ENV MEMCACHED_SHA1=b9da57ba63ba8de8a980fe0fe2fedc8d59e1dfe3
# Wed, 26 Jan 2022 05:44:08 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 26 Jan 2022 05:44:10 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 26 Jan 2022 05:44:17 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 26 Jan 2022 05:44:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Jan 2022 05:44:24 GMT
USER memcache
# Wed, 26 Jan 2022 05:44:28 GMT
EXPOSE 11211
# Wed, 26 Jan 2022 05:44:32 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:3149ee4a73508a4c39107d64a3fdc1b021626a22a0ac95e62fa0cea49ab77fba`  
		Last Modified: Wed, 26 Jan 2022 01:57:01 GMT  
		Size: 35.3 MB (35273030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07bcb451658eb6d9eace467c2e989d96e53c409eb48347a369e9ad80aadcfe96`  
		Last Modified: Wed, 26 Jan 2022 05:45:22 GMT  
		Size: 5.0 KB (4980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8807782e060aa90873de57b2d3ec277632145f166e9c1e3801c57eea7e595cc`  
		Last Modified: Wed, 26 Jan 2022 05:45:22 GMT  
		Size: 356.9 KB (356905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9214a40cf25dcbbc1d21f60a5512d485bc08156423100a0bb814946e829e3a0e`  
		Last Modified: Wed, 26 Jan 2022 05:45:22 GMT  
		Size: 1.3 MB (1321633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90ee2e08d849858def804d36f370ce894ef499543f6e8a72b9aac42c9e1cc909`  
		Last Modified: Wed, 26 Jan 2022 05:45:22 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6635b7a8817986bc0e4c179ae7d01d924f3017618b34956074b196886d9aaa67`  
		Last Modified: Wed, 26 Jan 2022 05:45:22 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:bullseye` - linux; s390x

```console
$ docker pull memcached@sha256:0f830716b97909822e4fe0394e7907f03695936767866c5e3dde96f89f483b30
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.2 MB (31216717 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e41587da3718a95304af17c726b656832260d3107e24f7811d54a20c5bad539`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 26 Jan 2022 01:41:13 GMT
ADD file:03b224b82f458b08d3b5071e42b67915a3db309332c0fc9229db7cf1148bc1b5 in / 
# Wed, 26 Jan 2022 01:41:15 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 03:32:44 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 26 Jan 2022 03:32:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 03:32:47 GMT
ENV MEMCACHED_VERSION=1.6.13
# Wed, 26 Jan 2022 03:32:48 GMT
ENV MEMCACHED_SHA1=b9da57ba63ba8de8a980fe0fe2fedc8d59e1dfe3
# Wed, 26 Jan 2022 03:36:16 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 26 Jan 2022 03:36:16 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 26 Jan 2022 03:36:16 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 26 Jan 2022 03:36:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Jan 2022 03:36:17 GMT
USER memcache
# Wed, 26 Jan 2022 03:36:17 GMT
EXPOSE 11211
# Wed, 26 Jan 2022 03:36:17 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:70bed29526f8483937e4d2540d19256d30786007c7c321e717e00d2e74700380`  
		Last Modified: Wed, 26 Jan 2022 01:46:57 GMT  
		Size: 29.6 MB (29647071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:531e195eaaf208f50aadc4ec839bd3a8f8d4bb0a35dea07bb0e27335fcf6db05`  
		Last Modified: Wed, 26 Jan 2022 03:37:15 GMT  
		Size: 5.0 KB (5026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1072031f118cfb7a6e47244d0bc6a66ac9a2cd286044b62e34033f655f0166d`  
		Last Modified: Wed, 26 Jan 2022 03:37:16 GMT  
		Size: 324.1 KB (324144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3719ec4f04cc9c989d6e8fb755b61510a0e78a3d35107b06cfc6c109c5aac17d`  
		Last Modified: Wed, 26 Jan 2022 03:37:16 GMT  
		Size: 1.2 MB (1240067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c8553e94280409bcb797ba67589732c286468e57828ea58da8d393d5b25a881`  
		Last Modified: Wed, 26 Jan 2022 03:37:16 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de608eaa9aaa185e5049d6baf7896898fe3d2c6beef1fcac73855ec782e15eee`  
		Last Modified: Wed, 26 Jan 2022 03:37:16 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:latest`

```console
$ docker pull memcached@sha256:61a8c3887d91c23aa6ce62b145b6e77acb1bcf195e950b3971f4007f2a47fa12
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
$ docker pull memcached@sha256:c9756ec03bedf0411e142fa016cce653157ef46216102b2ad9012ba57a69e9b5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.9 MB (32945941 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c8b63b0eeb514dca60290d594b69ba36d42534eb7c4af27ceb25c4b900d862c8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 21 Dec 2021 01:22:43 GMT
ADD file:09675d11695f65c55efdc393ff0cd32f30194cd7d0fbef4631eebfed4414ac97 in / 
# Tue, 21 Dec 2021 01:22:43 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 18:34:30 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 21 Dec 2021 18:34:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 20 Jan 2022 04:23:06 GMT
ENV MEMCACHED_VERSION=1.6.13
# Thu, 20 Jan 2022 04:23:06 GMT
ENV MEMCACHED_SHA1=b9da57ba63ba8de8a980fe0fe2fedc8d59e1dfe3
# Thu, 20 Jan 2022 04:27:08 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 20 Jan 2022 04:27:08 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 20 Jan 2022 04:27:09 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 20 Jan 2022 04:27:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 20 Jan 2022 04:27:09 GMT
USER memcache
# Thu, 20 Jan 2022 04:27:10 GMT
EXPOSE 11211
# Thu, 20 Jan 2022 04:27:10 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:a2abf6c4d29d43a4bf9fbb769f524d0fb36a2edab49819c1bf3e76f409f953ea`  
		Last Modified: Tue, 21 Dec 2021 01:27:48 GMT  
		Size: 31.4 MB (31357624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aa5be68e24cfc338b0c9be41213371a3ed596d00487ad58df6494ed46626117`  
		Last Modified: Tue, 21 Dec 2021 18:39:12 GMT  
		Size: 5.0 KB (4978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:052b406b20ce6593c7a47bc0d4d4f8b45258c1aed8b86ab06c0fc75ab6b4ee40`  
		Last Modified: Tue, 21 Dec 2021 18:39:13 GMT  
		Size: 328.1 KB (328055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b89359883409361f4bb025aaae623b73503a2801842fa3ceda2711924cf71b5`  
		Last Modified: Thu, 20 Jan 2022 04:31:55 GMT  
		Size: 1.3 MB (1254875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f5e296124091603e6ac2227e0bb1a6cde6faafa7608b926488a5d003b20d987`  
		Last Modified: Thu, 20 Jan 2022 04:31:54 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d7a956a84f556974daee7c5e1010bfa31d093c5b8b5eaabffa21a4931fe48f7`  
		Last Modified: Thu, 20 Jan 2022 04:31:54 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:latest` - linux; arm variant v5

```console
$ docker pull memcached@sha256:d16a2790a88e4662d8340cb85a9660f7738b5abbe759bad21b8f676e0ca8312c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.4 MB (30447722 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7768dab3ed87264de0f4e8a613c070301197408077835da74c7faae6eb6f4bd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 21 Dec 2021 01:50:31 GMT
ADD file:a3023f71bd93966e7db1419adda3ccde4fcc5e2e8cf58e7b13c51036ed5ff796 in / 
# Tue, 21 Dec 2021 01:50:32 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 03:35:35 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 21 Dec 2021 03:35:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 19 Jan 2022 23:48:42 GMT
ENV MEMCACHED_VERSION=1.6.13
# Wed, 19 Jan 2022 23:48:43 GMT
ENV MEMCACHED_SHA1=b9da57ba63ba8de8a980fe0fe2fedc8d59e1dfe3
# Wed, 19 Jan 2022 23:54:08 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 19 Jan 2022 23:54:09 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 19 Jan 2022 23:54:13 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 19 Jan 2022 23:54:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 19 Jan 2022 23:54:14 GMT
USER memcache
# Wed, 19 Jan 2022 23:54:15 GMT
EXPOSE 11211
# Wed, 19 Jan 2022 23:54:16 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:054429d0cf4038fef39a3b5eb6ce52f600f9a2cbb71a4fb3e95ecf9b2da62581`  
		Last Modified: Tue, 21 Dec 2021 02:05:52 GMT  
		Size: 28.9 MB (28900253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb7fdf670368bfde88ac158623eeda4b36ce64bd838e78a9ffcd3d2622eea2e8`  
		Last Modified: Tue, 21 Dec 2021 03:41:18 GMT  
		Size: 4.9 KB (4893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21508b31a1593117f5747b299da29b6bec5fb36f008effcd821336ebafc8ad70`  
		Last Modified: Tue, 21 Dec 2021 03:41:18 GMT  
		Size: 316.6 KB (316576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6d782b9d573913a26c43aba467d4fed6b33af9b83f44cfb1e8f63a76f92ab3a`  
		Last Modified: Wed, 19 Jan 2022 23:55:13 GMT  
		Size: 1.2 MB (1225592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b184c6b4181672a28be507397bd5d2baad8db49549bba6940adb30ce28c3320`  
		Last Modified: Wed, 19 Jan 2022 23:55:12 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73e44f9f60691acb75f8287e5a5eaa0675e04ffbc1fa1e4abfe57733ca7aa595`  
		Last Modified: Wed, 19 Jan 2022 23:55:12 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:latest` - linux; arm variant v7

```console
$ docker pull memcached@sha256:7f4a3e4bd6d3845da89e6e1fa7ee377f050118bd20803a8716e7c8aab31670ee
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.1 MB (28078674 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d0493346f5301d1fac3c1ee8eb4df2a8f1791ec73c16d2425aa56be76aabae7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:08 GMT
ADD file:7f27f5b43b7cb04e509fe145266d9bdeacfcacb024cafac32e57ef1c831d5ea7 in / 
# Wed, 26 Jan 2022 01:42:09 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 08:54:44 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 26 Jan 2022 08:54:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 08:54:52 GMT
ENV MEMCACHED_VERSION=1.6.13
# Wed, 26 Jan 2022 08:54:52 GMT
ENV MEMCACHED_SHA1=b9da57ba63ba8de8a980fe0fe2fedc8d59e1dfe3
# Wed, 26 Jan 2022 08:59:15 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 26 Jan 2022 08:59:16 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 26 Jan 2022 08:59:18 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 26 Jan 2022 08:59:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Jan 2022 08:59:18 GMT
USER memcache
# Wed, 26 Jan 2022 08:59:19 GMT
EXPOSE 11211
# Wed, 26 Jan 2022 08:59:19 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:aaef1f1162ec03e01b5b955d41da400544ec2374093ae3dbc330ab2bb36df3e1`  
		Last Modified: Wed, 26 Jan 2022 01:57:59 GMT  
		Size: 26.6 MB (26564933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c9d3dbbb6d5b3a74ea3807c462c99fc02f7ef46831734a98ab085fbfd45d84c`  
		Last Modified: Wed, 26 Jan 2022 09:13:01 GMT  
		Size: 4.9 KB (4894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c553a44b8d98c757ba52201bd5897c9b84bed862d1f1a33b30eaee164faf002`  
		Last Modified: Wed, 26 Jan 2022 09:13:02 GMT  
		Size: 312.0 KB (312023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e05d6d11f4c98f66add6994ad62c7fe25432ba441f2618ba25e8d572c66fe89`  
		Last Modified: Wed, 26 Jan 2022 09:13:02 GMT  
		Size: 1.2 MB (1196416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:902b4740d93b1e9cdd39f484a29d2e022801b8f4612ddd6471c63d0d5aee77c7`  
		Last Modified: Wed, 26 Jan 2022 09:13:01 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0813f5460d7241e77461d216cec438321996a8a74a205fd5a63e3a6e7300ec08`  
		Last Modified: Wed, 26 Jan 2022 09:13:01 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:latest` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:97cdec366a180179780e13eb6ab3b4839bd7ce753737ed9b69c45d5baf9d55e0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.4 MB (31434947 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9182bae18682935ee16f416121710ff59a5021e8148d558c7df06caa35e422c5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:31 GMT
ADD file:0ec6f47a8857bf8e6cef71ed8f864be7ce1790ff6ed04fd4201e7dbde4728d3a in / 
# Wed, 26 Jan 2022 01:42:31 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 04:50:24 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 26 Jan 2022 04:50:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 04:50:28 GMT
ENV MEMCACHED_VERSION=1.6.13
# Wed, 26 Jan 2022 04:50:29 GMT
ENV MEMCACHED_SHA1=b9da57ba63ba8de8a980fe0fe2fedc8d59e1dfe3
# Wed, 26 Jan 2022 04:53:09 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 26 Jan 2022 04:53:10 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 26 Jan 2022 04:53:10 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 26 Jan 2022 04:53:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Jan 2022 04:53:12 GMT
USER memcache
# Wed, 26 Jan 2022 04:53:13 GMT
EXPOSE 11211
# Wed, 26 Jan 2022 04:53:14 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:8998bd30e6a1204d13403045766edbe14f941b52087465f5d140ab63c8b113bf`  
		Last Modified: Wed, 26 Jan 2022 01:49:04 GMT  
		Size: 30.1 MB (30056774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a59fc24ed29770b5c2f4352a96e8a82fa286fa87df96964968e2fb2796e105ac`  
		Last Modified: Wed, 26 Jan 2022 04:53:58 GMT  
		Size: 4.9 KB (4900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54853adf97755cd00bf2b960a7a7458bfc9824d4847b0f97e7e5f41e86b6c351`  
		Last Modified: Wed, 26 Jan 2022 04:53:59 GMT  
		Size: 119.2 KB (119210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bc43135274188258180f193f3f9907dd72b6b09963f1886610f28977741356a`  
		Last Modified: Wed, 26 Jan 2022 04:53:59 GMT  
		Size: 1.3 MB (1253657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e306557d5e40e37e762e103bd520b6153919316e8d64e4ae3d21fa66d6420f3`  
		Last Modified: Wed, 26 Jan 2022 04:53:59 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86f1b169766c42ff4dabdf96ef26f2207f4f9fa4fdf13b53c3625a106c50ca12`  
		Last Modified: Wed, 26 Jan 2022 04:53:58 GMT  
		Size: 120.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:latest` - linux; 386

```console
$ docker pull memcached@sha256:caebaf527ba0576d76c6d7579c1c921d78dcd0522d3dbe11a11c5ebc1c05b37b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.0 MB (33971560 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f0d964750c0182cb6e1376d8eec8982b36ab1b3aa6f8ab59919f116da2625871`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 26 Jan 2022 01:39:55 GMT
ADD file:876ebf07c65841f4840842086c883af48e07386964fe6d643ba193895ec2a582 in / 
# Wed, 26 Jan 2022 01:39:56 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 08:45:04 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 26 Jan 2022 08:45:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 08:45:09 GMT
ENV MEMCACHED_VERSION=1.6.13
# Wed, 26 Jan 2022 08:45:09 GMT
ENV MEMCACHED_SHA1=b9da57ba63ba8de8a980fe0fe2fedc8d59e1dfe3
# Wed, 26 Jan 2022 08:49:29 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 26 Jan 2022 08:49:29 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 26 Jan 2022 08:49:30 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 26 Jan 2022 08:49:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Jan 2022 08:49:31 GMT
USER memcache
# Wed, 26 Jan 2022 08:49:31 GMT
EXPOSE 11211
# Wed, 26 Jan 2022 08:49:31 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:86933886b1754aba091548cf031a9bca88cdce9bb4fc1f28bb38b61594c2c2c7`  
		Last Modified: Wed, 26 Jan 2022 01:48:57 GMT  
		Size: 32.4 MB (32377406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84bd6e2dff27e256b3baec641bd7c64e8a138237c2c259a806d0f9a9fb1d2255`  
		Last Modified: Wed, 26 Jan 2022 08:50:25 GMT  
		Size: 4.9 KB (4896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d8c7dc83b8d6601d80421931237cbfcd968616d9910fad6f78ee1706ee8f1e3`  
		Last Modified: Wed, 26 Jan 2022 08:50:26 GMT  
		Size: 336.6 KB (336627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5e3e4cf9c8423bfa3e769914fdcf235f6b64837f5fb62f5ccc09a8d792a268c`  
		Last Modified: Wed, 26 Jan 2022 08:50:26 GMT  
		Size: 1.3 MB (1252223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6402d600344325d49706165f2b0feec85cd2421776889433e4c45230bc89b7ee`  
		Last Modified: Wed, 26 Jan 2022 08:50:25 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9fa9c73a03d6ce53a9ea22b31db2648aa6a02a1779ae0a5b19070fbbe806125`  
		Last Modified: Wed, 26 Jan 2022 08:50:25 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:latest` - linux; mips64le

```console
$ docker pull memcached@sha256:0848c96207329a581151eeefb1a2b5f1c13893e01667962c71ed108ba448ec8a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.2 MB (31212144 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5691adbb93dbe11492ece526682692fc23ae3869ddd09a5cc20fc92abe25fa68`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:45 GMT
ADD file:61767027a5ab46afbcd4079d200abe8d663326adc96fa28ca8c8955a06d9322e in / 
# Wed, 26 Jan 2022 01:42:46 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 04:16:54 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 26 Jan 2022 04:17:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 04:17:06 GMT
ENV MEMCACHED_VERSION=1.6.13
# Wed, 26 Jan 2022 04:17:07 GMT
ENV MEMCACHED_SHA1=b9da57ba63ba8de8a980fe0fe2fedc8d59e1dfe3
# Wed, 26 Jan 2022 04:23:00 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 26 Jan 2022 04:23:00 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 26 Jan 2022 04:23:02 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 26 Jan 2022 04:23:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Jan 2022 04:23:03 GMT
USER memcache
# Wed, 26 Jan 2022 04:23:03 GMT
EXPOSE 11211
# Wed, 26 Jan 2022 04:23:03 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:266e7d2b59483859eaa1711d2afeb25ea4458eeb36b3e909372930db1f834d7f`  
		Last Modified: Wed, 26 Jan 2022 01:51:23 GMT  
		Size: 29.6 MB (29632834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f2c23d84e18c59799194289c3354e30ed9e147411beb83fd8a53a6b0510244e`  
		Last Modified: Wed, 26 Jan 2022 04:23:22 GMT  
		Size: 5.0 KB (4977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e72e725e4f6fb1ddea7af05f25646fbd5f401583a994d00e98f8d9762bdeef1`  
		Last Modified: Wed, 26 Jan 2022 04:23:22 GMT  
		Size: 323.7 KB (323700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a64f2bbfc21569385827a44c22dc4d96a9004879a3db5a479ac796150f31a89`  
		Last Modified: Wed, 26 Jan 2022 04:23:23 GMT  
		Size: 1.3 MB (1250226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10ec607308395a4822bcdf6d4c2f8665284150145ceaee889026d63b5bbfc525`  
		Last Modified: Wed, 26 Jan 2022 04:23:22 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0544419df418d0761bfd4cee74e348f336fd813c7d70a2ba0f9c66dd4dcad99`  
		Last Modified: Wed, 26 Jan 2022 04:23:22 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:latest` - linux; ppc64le

```console
$ docker pull memcached@sha256:467baa60d3118dac94a8d1909db41ec8f8e0867581bba86e83d70d2843299d95
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.0 MB (36956955 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89c206a82af6419284433a55b65259fb3c41ae73d206fc37aa006d7c30d22d0e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 26 Jan 2022 01:46:51 GMT
ADD file:c03f34c221e57fa5cb625c166d1db9f72d6ba2fa17a3c41a5d04d6875d098949 in / 
# Wed, 26 Jan 2022 01:46:57 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 05:38:39 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 26 Jan 2022 05:38:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 05:38:55 GMT
ENV MEMCACHED_VERSION=1.6.13
# Wed, 26 Jan 2022 05:38:58 GMT
ENV MEMCACHED_SHA1=b9da57ba63ba8de8a980fe0fe2fedc8d59e1dfe3
# Wed, 26 Jan 2022 05:44:08 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 26 Jan 2022 05:44:10 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 26 Jan 2022 05:44:17 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 26 Jan 2022 05:44:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Jan 2022 05:44:24 GMT
USER memcache
# Wed, 26 Jan 2022 05:44:28 GMT
EXPOSE 11211
# Wed, 26 Jan 2022 05:44:32 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:3149ee4a73508a4c39107d64a3fdc1b021626a22a0ac95e62fa0cea49ab77fba`  
		Last Modified: Wed, 26 Jan 2022 01:57:01 GMT  
		Size: 35.3 MB (35273030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07bcb451658eb6d9eace467c2e989d96e53c409eb48347a369e9ad80aadcfe96`  
		Last Modified: Wed, 26 Jan 2022 05:45:22 GMT  
		Size: 5.0 KB (4980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8807782e060aa90873de57b2d3ec277632145f166e9c1e3801c57eea7e595cc`  
		Last Modified: Wed, 26 Jan 2022 05:45:22 GMT  
		Size: 356.9 KB (356905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9214a40cf25dcbbc1d21f60a5512d485bc08156423100a0bb814946e829e3a0e`  
		Last Modified: Wed, 26 Jan 2022 05:45:22 GMT  
		Size: 1.3 MB (1321633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90ee2e08d849858def804d36f370ce894ef499543f6e8a72b9aac42c9e1cc909`  
		Last Modified: Wed, 26 Jan 2022 05:45:22 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6635b7a8817986bc0e4c179ae7d01d924f3017618b34956074b196886d9aaa67`  
		Last Modified: Wed, 26 Jan 2022 05:45:22 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:latest` - linux; s390x

```console
$ docker pull memcached@sha256:0f830716b97909822e4fe0394e7907f03695936767866c5e3dde96f89f483b30
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.2 MB (31216717 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e41587da3718a95304af17c726b656832260d3107e24f7811d54a20c5bad539`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 26 Jan 2022 01:41:13 GMT
ADD file:03b224b82f458b08d3b5071e42b67915a3db309332c0fc9229db7cf1148bc1b5 in / 
# Wed, 26 Jan 2022 01:41:15 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 03:32:44 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 26 Jan 2022 03:32:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 03:32:47 GMT
ENV MEMCACHED_VERSION=1.6.13
# Wed, 26 Jan 2022 03:32:48 GMT
ENV MEMCACHED_SHA1=b9da57ba63ba8de8a980fe0fe2fedc8d59e1dfe3
# Wed, 26 Jan 2022 03:36:16 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 26 Jan 2022 03:36:16 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 26 Jan 2022 03:36:16 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 26 Jan 2022 03:36:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Jan 2022 03:36:17 GMT
USER memcache
# Wed, 26 Jan 2022 03:36:17 GMT
EXPOSE 11211
# Wed, 26 Jan 2022 03:36:17 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:70bed29526f8483937e4d2540d19256d30786007c7c321e717e00d2e74700380`  
		Last Modified: Wed, 26 Jan 2022 01:46:57 GMT  
		Size: 29.6 MB (29647071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:531e195eaaf208f50aadc4ec839bd3a8f8d4bb0a35dea07bb0e27335fcf6db05`  
		Last Modified: Wed, 26 Jan 2022 03:37:15 GMT  
		Size: 5.0 KB (5026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1072031f118cfb7a6e47244d0bc6a66ac9a2cd286044b62e34033f655f0166d`  
		Last Modified: Wed, 26 Jan 2022 03:37:16 GMT  
		Size: 324.1 KB (324144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3719ec4f04cc9c989d6e8fb755b61510a0e78a3d35107b06cfc6c109c5aac17d`  
		Last Modified: Wed, 26 Jan 2022 03:37:16 GMT  
		Size: 1.2 MB (1240067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c8553e94280409bcb797ba67589732c286468e57828ea58da8d393d5b25a881`  
		Last Modified: Wed, 26 Jan 2022 03:37:16 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de608eaa9aaa185e5049d6baf7896898fe3d2c6beef1fcac73855ec782e15eee`  
		Last Modified: Wed, 26 Jan 2022 03:37:16 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
