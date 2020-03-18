<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `memcached`

-	[`memcached:1`](#memcached1)
-	[`memcached:1.6`](#memcached16)
-	[`memcached:1.6.1`](#memcached161)
-	[`memcached:1.6.1-alpine`](#memcached161-alpine)
-	[`memcached:1.6-alpine`](#memcached16-alpine)
-	[`memcached:1-alpine`](#memcached1-alpine)
-	[`memcached:alpine`](#memcachedalpine)
-	[`memcached:latest`](#memcachedlatest)

## `memcached:1`

```console
$ docker pull memcached@sha256:4cf938dddf9daf5228194a84e27bba4f82a934fa8a2c7c57f0114a15aa1de834
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `memcached:1` - linux; amd64

```console
$ docker pull memcached@sha256:f01d94f9c4adae3a566151be2b41e9e0ab5410ef3fcb4e69e92226173c7f7259
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.5 MB (30483498 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:20188fe150aa349793b646f31dde86a97c2a60989b76bf01df11ec97e79f6a3f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 26 Feb 2020 00:37:39 GMT
ADD file:e5a364615e0f6961626089c7d658adbf8c8d95b3ae95a390a8bb33875317d434 in / 
# Wed, 26 Feb 2020 00:37:39 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 18:07:47 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 26 Feb 2020 18:07:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Mar 2020 23:22:04 GMT
ENV MEMCACHED_VERSION=1.6.1
# Tue, 17 Mar 2020 23:22:04 GMT
ENV MEMCACHED_SHA1=6e337924dbf953bfabda512405d710d9757c97c1
# Tue, 17 Mar 2020 23:30:13 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 17 Mar 2020 23:30:13 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 17 Mar 2020 23:30:14 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 17 Mar 2020 23:30:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 17 Mar 2020 23:30:14 GMT
USER memcache
# Tue, 17 Mar 2020 23:30:14 GMT
EXPOSE 11211
# Tue, 17 Mar 2020 23:30:14 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:68ced04f60ab5c7a5f1d0b0b4e7572c5a4c8cce44866513d30d9df1a15277d6b`  
		Last Modified: Wed, 26 Feb 2020 00:44:23 GMT  
		Size: 27.1 MB (27091819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7233c6ae94c59c690ba7007d1f0e360f97b515b3df0a5adc0a8e0c71e48dc836`  
		Last Modified: Wed, 26 Feb 2020 18:16:20 GMT  
		Size: 5.0 KB (4980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3945a4bf251bce21f9517716e4ed007325a8e8b279e52a09bc15fffa2f65b16d`  
		Last Modified: Wed, 26 Feb 2020 18:16:20 GMT  
		Size: 2.2 MB (2196514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9e46f4b34ecc2434e857dccae8dcefac20010d02aa70739107749e36164a43f`  
		Last Modified: Tue, 17 Mar 2020 23:38:46 GMT  
		Size: 1.2 MB (1189776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca1999a38cda2f5a4349e8b795ff37d1d1ba865a56a18defdaffac68af7800ce`  
		Last Modified: Tue, 17 Mar 2020 23:38:45 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4f797df323b4285de392809bad17d92950319a7753be796ab8b1a86d1666a85`  
		Last Modified: Tue, 17 Mar 2020 23:38:46 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1` - linux; arm variant v5

```console
$ docker pull memcached@sha256:d32bdb11fd734410cd1be1ae96fa977048cd809329b1a9cae28f4ec2f8b8fb8c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.9 MB (27888005 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1aec9eb200e1be46e4a6da6e72866613bd30e78e8865abd3dfdcb42b7877cca2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 26 Feb 2020 00:47:49 GMT
ADD file:745d3236976c8213b805ca6d14f150561816cd2eeec5aa7e1aaea44d9d5675e9 in / 
# Wed, 26 Feb 2020 00:47:53 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 01:21:35 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 26 Feb 2020 01:23:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Mar 2020 20:48:50 GMT
ENV MEMCACHED_VERSION=1.6.1
# Tue, 17 Mar 2020 20:48:52 GMT
ENV MEMCACHED_SHA1=6e337924dbf953bfabda512405d710d9757c97c1
# Tue, 17 Mar 2020 22:19:10 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 17 Mar 2020 22:19:13 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 17 Mar 2020 22:19:24 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 17 Mar 2020 22:19:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 17 Mar 2020 22:19:28 GMT
USER memcache
# Tue, 17 Mar 2020 22:19:29 GMT
EXPOSE 11211
# Tue, 17 Mar 2020 22:19:31 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:d9f9009f908455fa93c5b3e0d3230df44ea75299b2de375ab35b74193f679076`  
		Last Modified: Wed, 26 Feb 2020 00:59:18 GMT  
		Size: 24.8 MB (24830277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f028832400faf7f954f74987eff7a1e300690055f9df70085c778e354351f5d8`  
		Last Modified: Tue, 10 Mar 2020 13:06:25 GMT  
		Size: 4.9 KB (4895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dee056e35538c22bed8fa9de89eaa5b3ce1bfbce6a93be0b7ce527c378f23cf4`  
		Last Modified: Tue, 10 Mar 2020 13:06:33 GMT  
		Size: 1.9 MB (1896817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4def82d8eadc3db4d32a027dc0072359c4a3133a6bfca570381eed5e782302be`  
		Last Modified: Tue, 17 Mar 2020 22:19:53 GMT  
		Size: 1.2 MB (1155608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82fdc512c93448bbc2be492053f7303bef1efa0a68d7f8f5bbaa64ce758b250e`  
		Last Modified: Tue, 17 Mar 2020 22:19:56 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8003ad16648f331b96907ecf19d95da34b2b68aedf312ca29f1fc6e34ede22ab`  
		Last Modified: Tue, 17 Mar 2020 22:20:07 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1` - linux; arm variant v7

```console
$ docker pull memcached@sha256:cdf939e755f1f26e266767e417109b3ba044b51d444eff026e83bd1c7195fa9a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.6 MB (25644199 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b99a8df834c831b0c96ac194f07f1df3b4b1b22ac94731bc8ddd6f4f1df4419b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 26 Feb 2020 00:52:11 GMT
ADD file:2488038744e2e15217e67dd7f4bec5dcc7e9abe8a1010fe720a5ba7cbe7ab0eb in / 
# Wed, 26 Feb 2020 00:52:13 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 03:03:14 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 26 Feb 2020 03:05:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Mar 2020 22:23:13 GMT
ENV MEMCACHED_VERSION=1.6.1
# Tue, 17 Mar 2020 22:23:15 GMT
ENV MEMCACHED_SHA1=6e337924dbf953bfabda512405d710d9757c97c1
# Tue, 17 Mar 2020 22:51:58 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 17 Mar 2020 22:52:01 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 17 Mar 2020 22:52:11 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 17 Mar 2020 22:52:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 17 Mar 2020 22:52:15 GMT
USER memcache
# Tue, 17 Mar 2020 22:52:17 GMT
EXPOSE 11211
# Tue, 17 Mar 2020 22:52:19 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:fff3167bf8c79dc08baf67eb607823aadcbee2033f9620cc502e2c49423f605b`  
		Last Modified: Wed, 26 Feb 2020 01:07:32 GMT  
		Size: 22.7 MB (22699783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd762b0d48bc41e6bdfdb354ae48b55c2cbe60e2a0ad9cd60a9396304fb48660`  
		Last Modified: Wed, 26 Feb 2020 03:35:50 GMT  
		Size: 4.9 KB (4896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34dccc10f85111d1e9ad7f9118fc95ec338f9510a4fb1d7d847c500212185bf7`  
		Last Modified: Wed, 26 Feb 2020 03:35:57 GMT  
		Size: 1.8 MB (1811579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1aba4da49d87f5f9ee5f89839430139620889df5129d8f26fb948dd6e0738e1`  
		Last Modified: Wed, 18 Mar 2020 00:18:02 GMT  
		Size: 1.1 MB (1127532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:756d789cadf0cc90e8d82cad7000c52c7ad4c5d7984984c58b274a318c70c47c`  
		Last Modified: Wed, 18 Mar 2020 00:18:06 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d3d88a2570cc19347b319b789f0a3aafc02b99ac6c369e1343ba2315994bdb1`  
		Last Modified: Wed, 18 Mar 2020 00:18:17 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:89a48b7232e353e9d13fc62962805abcd59e6f69bfd363c03b0b47c0fba0534a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.1 MB (29091968 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a3d7d5d254344a16e0d4d3a008c5108f77c7e872f7f7649fa3ac50ce1aad6ed1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 26 Feb 2020 00:46:51 GMT
ADD file:a93818b0ffcb2823807811dffd78092a3e3f4981aabf48c3cb75f2fa319ac055 in / 
# Wed, 26 Feb 2020 00:46:55 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 13:34:13 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 26 Feb 2020 13:34:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Mar 2020 20:41:15 GMT
ENV MEMCACHED_VERSION=1.6.1
# Tue, 17 Mar 2020 20:41:16 GMT
ENV MEMCACHED_SHA1=6e337924dbf953bfabda512405d710d9757c97c1
# Tue, 17 Mar 2020 20:50:18 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 17 Mar 2020 20:50:18 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 17 Mar 2020 20:50:20 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 17 Mar 2020 20:50:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 17 Mar 2020 20:50:21 GMT
USER memcache
# Tue, 17 Mar 2020 20:50:22 GMT
EXPOSE 11211
# Tue, 17 Mar 2020 20:50:22 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:f338bc35613f66cfaad272234de7b77a91d6c5422855bf6239f2b0ff9d73f0a4`  
		Last Modified: Wed, 26 Feb 2020 00:56:15 GMT  
		Size: 25.9 MB (25851563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4d7ac360be705ceb72083cd1a2c07b2fd7f572f0cd8de06e6733c8f217739a2`  
		Last Modified: Wed, 26 Feb 2020 14:00:56 GMT  
		Size: 5.0 KB (5029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bd27757fe5a945d701f8f5bd7534c41588270d8f2b934ca8085e0a649cbbf91`  
		Last Modified: Wed, 26 Feb 2020 14:00:56 GMT  
		Size: 2.1 MB (2074945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc7a620a01855a969584241d573d1e6acf55dee0e7e6c4f8d4c821b6b0064637`  
		Last Modified: Tue, 17 Mar 2020 20:59:55 GMT  
		Size: 1.2 MB (1160025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04bcc8eff174cea809be4c1a00052dce74463a60ea51cfb0c0da09ec1e0d8b42`  
		Last Modified: Tue, 17 Mar 2020 20:59:55 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15d59c8d4a0e2a02d465e919de1d0adb45841bbbeb21e78c588a3251cb9f2740`  
		Last Modified: Tue, 17 Mar 2020 20:59:55 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1` - linux; 386

```console
$ docker pull memcached@sha256:c34541b96410e9129064d823a4e89051fd9001f132c51841ca9d6f2fee21078c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.2 MB (31155198 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c89fc4282ec39b4634a263a8481002f3d90d3be4ece62cc10f9cf40d7608f85`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 26 Feb 2020 00:32:17 GMT
ADD file:08977fa54555a1ed2ae44a3aec04df157092a6c1c1b70ce0407cc2dc2f8bcd76 in / 
# Wed, 26 Feb 2020 00:32:17 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 10:57:50 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 26 Feb 2020 10:57:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Mar 2020 21:56:16 GMT
ENV MEMCACHED_VERSION=1.6.1
# Tue, 17 Mar 2020 21:56:17 GMT
ENV MEMCACHED_SHA1=6e337924dbf953bfabda512405d710d9757c97c1
# Tue, 17 Mar 2020 22:05:32 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 17 Mar 2020 22:05:33 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 17 Mar 2020 22:05:34 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 17 Mar 2020 22:05:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 17 Mar 2020 22:05:35 GMT
USER memcache
# Tue, 17 Mar 2020 22:05:35 GMT
EXPOSE 11211
# Tue, 17 Mar 2020 22:05:35 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:1de10f1ae2a5bfd5f34f19421ebd282580e443321e4947cdf5f943875782b018`  
		Last Modified: Wed, 26 Feb 2020 00:38:34 GMT  
		Size: 27.7 MB (27747667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40f6886cf964eb4f4025c8157f9756ae21437cdf1a57f5fe279849787aff082b`  
		Last Modified: Wed, 26 Feb 2020 11:06:50 GMT  
		Size: 4.9 KB (4893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d843b4e4e2bb25c8a0fb82174c608d57f8eb0ac3e8f3773c31c988a34857030`  
		Last Modified: Wed, 26 Feb 2020 11:06:50 GMT  
		Size: 2.2 MB (2208102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28a0ed0844b264f9c1207229402186f1fff548292e028cb9a1c254402763364c`  
		Last Modified: Tue, 17 Mar 2020 22:14:44 GMT  
		Size: 1.2 MB (1194128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c2889f61fb8cb96b3ec44d3036bda0cef5e06e7703a4df8876adf9792462aa8`  
		Last Modified: Tue, 17 Mar 2020 22:14:44 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7d9bc4abf0879c8f9c4cb3d9d4551d03033f7e3356fd9df07c8c69ee60ff63f`  
		Last Modified: Tue, 17 Mar 2020 22:14:44 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1` - linux; ppc64le

```console
$ docker pull memcached@sha256:010267e365a1b82e10d694473d416094c5a196dc8d778a8c2d383ac2558c6a50
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.1 MB (34061620 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dbb12046217f66e43361864882561c2b935d472dc219f6d90d6824a6cab4cad1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 26 Feb 2020 01:31:23 GMT
ADD file:430f1f769b86c60db1b8d2f96ed26c24837b3ff5730264be42a9c0cd8e43df7f in / 
# Wed, 26 Feb 2020 01:31:29 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 08:58:42 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 26 Feb 2020 08:59:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Mar 2020 22:07:27 GMT
ENV MEMCACHED_VERSION=1.6.1
# Tue, 17 Mar 2020 22:07:29 GMT
ENV MEMCACHED_SHA1=6e337924dbf953bfabda512405d710d9757c97c1
# Tue, 17 Mar 2020 22:17:35 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 17 Mar 2020 22:17:37 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 17 Mar 2020 22:17:43 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 17 Mar 2020 22:17:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 17 Mar 2020 22:17:47 GMT
USER memcache
# Tue, 17 Mar 2020 22:17:49 GMT
EXPOSE 11211
# Tue, 17 Mar 2020 22:17:52 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:975241fcd2057cc8f4cb8f066d68ed18877152b88da11e682911ccc3bc3da7c4`  
		Last Modified: Wed, 26 Feb 2020 01:52:57 GMT  
		Size: 30.5 MB (30518427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c4567bf2efa314a53153932738e79b856d675d83e768d2e2ce3ab5b45930ace`  
		Last Modified: Wed, 26 Feb 2020 09:10:20 GMT  
		Size: 5.0 KB (4985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63966b4eb4cf356b52b220fc08251ec17ddb06f1425096935b9dbe79c39e5bb5`  
		Last Modified: Wed, 26 Feb 2020 09:10:20 GMT  
		Size: 2.3 MB (2322659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f210835730fc44353def79514fb093d60f6442f97c0fffaa7dc0962a6ba887a`  
		Last Modified: Tue, 17 Mar 2020 22:27:10 GMT  
		Size: 1.2 MB (1215142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fde09d96ef673b71efb6670819cea32e1454fe672a42f7377f396277e48c40b7`  
		Last Modified: Tue, 17 Mar 2020 22:27:09 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efca2b06ccc0d3c5720838c60727aad27be7400487ab096e48113b6a2be2e5ae`  
		Last Modified: Tue, 17 Mar 2020 22:27:09 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1` - linux; s390x

```console
$ docker pull memcached@sha256:057b9567b3c01a5b0dbf1c7dba5b89d88df721093c01da5c6a1425c1f8ad6265
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.7 MB (28694839 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe2378496a97259729a8423d4b14be0ea1db6e01b3f9aa9e34431ef824d655e6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Sat, 28 Dec 2019 04:42:03 GMT
ADD file:eec6c56f8680753860198c3af0d94aabb87018ca30f6f6e346621a6bffe0e4b8 in / 
# Sat, 28 Dec 2019 04:42:04 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 09:52:58 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Sat, 28 Dec 2019 09:53:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 09:53:02 GMT
ENV MEMCACHED_VERSION=1.5.20
# Sat, 28 Dec 2019 09:53:02 GMT
ENV MEMCACHED_SHA1=5d3b5af3ce0a1483d655017db7228bcaeff10d47
# Sat, 28 Dec 2019 09:57:41 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Sat, 28 Dec 2019 09:57:41 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Sat, 28 Dec 2019 09:57:42 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Sat, 28 Dec 2019 09:57:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 28 Dec 2019 09:57:42 GMT
USER memcache
# Sat, 28 Dec 2019 09:57:42 GMT
EXPOSE 11211
# Sat, 28 Dec 2019 09:57:42 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:f7542f43e95fb32a870ee38d7f0e7bb23267ac8dcf709e3944311b0a30d7a479`  
		Last Modified: Sat, 28 Dec 2019 04:45:08 GMT  
		Size: 25.7 MB (25705315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10233ccd3a1a569a8ec38365e560732bbd6adbbe1646b79cee3569d59f7cef73`  
		Last Modified: Sat, 28 Dec 2019 09:57:55 GMT  
		Size: 5.0 KB (5022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f3e3dfd06ace4d055f1539e38c0fb68e4d1866043a1ba372c8c2f0fec48315d`  
		Last Modified: Sat, 28 Dec 2019 09:57:55 GMT  
		Size: 1.9 MB (1885865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47cce4b30798653a4fcf3fd9160a90374e103d5c1e877e69645d033c0f916e67`  
		Last Modified: Sat, 28 Dec 2019 09:57:55 GMT  
		Size: 1.1 MB (1098229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:982ba8604e516e190f19469aa238d4197aa0000182cbc54d57345a029b765600`  
		Last Modified: Sat, 28 Dec 2019 09:57:55 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aabfe12e62b1d54d9dce449f2dc85f703ade5574f14eadfa54a601a86cc96e54`  
		Last Modified: Sat, 28 Dec 2019 09:57:55 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:1.6`

```console
$ docker pull memcached@sha256:96fa7f208b93c7f62f1febf8b5c38f8fd45230a708207b3e7eda98b4cff93bfc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `memcached:1.6` - linux; amd64

```console
$ docker pull memcached@sha256:f01d94f9c4adae3a566151be2b41e9e0ab5410ef3fcb4e69e92226173c7f7259
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.5 MB (30483498 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:20188fe150aa349793b646f31dde86a97c2a60989b76bf01df11ec97e79f6a3f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 26 Feb 2020 00:37:39 GMT
ADD file:e5a364615e0f6961626089c7d658adbf8c8d95b3ae95a390a8bb33875317d434 in / 
# Wed, 26 Feb 2020 00:37:39 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 18:07:47 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 26 Feb 2020 18:07:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Mar 2020 23:22:04 GMT
ENV MEMCACHED_VERSION=1.6.1
# Tue, 17 Mar 2020 23:22:04 GMT
ENV MEMCACHED_SHA1=6e337924dbf953bfabda512405d710d9757c97c1
# Tue, 17 Mar 2020 23:30:13 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 17 Mar 2020 23:30:13 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 17 Mar 2020 23:30:14 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 17 Mar 2020 23:30:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 17 Mar 2020 23:30:14 GMT
USER memcache
# Tue, 17 Mar 2020 23:30:14 GMT
EXPOSE 11211
# Tue, 17 Mar 2020 23:30:14 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:68ced04f60ab5c7a5f1d0b0b4e7572c5a4c8cce44866513d30d9df1a15277d6b`  
		Last Modified: Wed, 26 Feb 2020 00:44:23 GMT  
		Size: 27.1 MB (27091819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7233c6ae94c59c690ba7007d1f0e360f97b515b3df0a5adc0a8e0c71e48dc836`  
		Last Modified: Wed, 26 Feb 2020 18:16:20 GMT  
		Size: 5.0 KB (4980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3945a4bf251bce21f9517716e4ed007325a8e8b279e52a09bc15fffa2f65b16d`  
		Last Modified: Wed, 26 Feb 2020 18:16:20 GMT  
		Size: 2.2 MB (2196514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9e46f4b34ecc2434e857dccae8dcefac20010d02aa70739107749e36164a43f`  
		Last Modified: Tue, 17 Mar 2020 23:38:46 GMT  
		Size: 1.2 MB (1189776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca1999a38cda2f5a4349e8b795ff37d1d1ba865a56a18defdaffac68af7800ce`  
		Last Modified: Tue, 17 Mar 2020 23:38:45 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4f797df323b4285de392809bad17d92950319a7753be796ab8b1a86d1666a85`  
		Last Modified: Tue, 17 Mar 2020 23:38:46 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6` - linux; arm variant v5

```console
$ docker pull memcached@sha256:d32bdb11fd734410cd1be1ae96fa977048cd809329b1a9cae28f4ec2f8b8fb8c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.9 MB (27888005 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1aec9eb200e1be46e4a6da6e72866613bd30e78e8865abd3dfdcb42b7877cca2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 26 Feb 2020 00:47:49 GMT
ADD file:745d3236976c8213b805ca6d14f150561816cd2eeec5aa7e1aaea44d9d5675e9 in / 
# Wed, 26 Feb 2020 00:47:53 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 01:21:35 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 26 Feb 2020 01:23:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Mar 2020 20:48:50 GMT
ENV MEMCACHED_VERSION=1.6.1
# Tue, 17 Mar 2020 20:48:52 GMT
ENV MEMCACHED_SHA1=6e337924dbf953bfabda512405d710d9757c97c1
# Tue, 17 Mar 2020 22:19:10 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 17 Mar 2020 22:19:13 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 17 Mar 2020 22:19:24 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 17 Mar 2020 22:19:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 17 Mar 2020 22:19:28 GMT
USER memcache
# Tue, 17 Mar 2020 22:19:29 GMT
EXPOSE 11211
# Tue, 17 Mar 2020 22:19:31 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:d9f9009f908455fa93c5b3e0d3230df44ea75299b2de375ab35b74193f679076`  
		Last Modified: Wed, 26 Feb 2020 00:59:18 GMT  
		Size: 24.8 MB (24830277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f028832400faf7f954f74987eff7a1e300690055f9df70085c778e354351f5d8`  
		Last Modified: Tue, 10 Mar 2020 13:06:25 GMT  
		Size: 4.9 KB (4895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dee056e35538c22bed8fa9de89eaa5b3ce1bfbce6a93be0b7ce527c378f23cf4`  
		Last Modified: Tue, 10 Mar 2020 13:06:33 GMT  
		Size: 1.9 MB (1896817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4def82d8eadc3db4d32a027dc0072359c4a3133a6bfca570381eed5e782302be`  
		Last Modified: Tue, 17 Mar 2020 22:19:53 GMT  
		Size: 1.2 MB (1155608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82fdc512c93448bbc2be492053f7303bef1efa0a68d7f8f5bbaa64ce758b250e`  
		Last Modified: Tue, 17 Mar 2020 22:19:56 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8003ad16648f331b96907ecf19d95da34b2b68aedf312ca29f1fc6e34ede22ab`  
		Last Modified: Tue, 17 Mar 2020 22:20:07 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6` - linux; arm variant v7

```console
$ docker pull memcached@sha256:cdf939e755f1f26e266767e417109b3ba044b51d444eff026e83bd1c7195fa9a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.6 MB (25644199 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b99a8df834c831b0c96ac194f07f1df3b4b1b22ac94731bc8ddd6f4f1df4419b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 26 Feb 2020 00:52:11 GMT
ADD file:2488038744e2e15217e67dd7f4bec5dcc7e9abe8a1010fe720a5ba7cbe7ab0eb in / 
# Wed, 26 Feb 2020 00:52:13 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 03:03:14 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 26 Feb 2020 03:05:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Mar 2020 22:23:13 GMT
ENV MEMCACHED_VERSION=1.6.1
# Tue, 17 Mar 2020 22:23:15 GMT
ENV MEMCACHED_SHA1=6e337924dbf953bfabda512405d710d9757c97c1
# Tue, 17 Mar 2020 22:51:58 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 17 Mar 2020 22:52:01 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 17 Mar 2020 22:52:11 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 17 Mar 2020 22:52:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 17 Mar 2020 22:52:15 GMT
USER memcache
# Tue, 17 Mar 2020 22:52:17 GMT
EXPOSE 11211
# Tue, 17 Mar 2020 22:52:19 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:fff3167bf8c79dc08baf67eb607823aadcbee2033f9620cc502e2c49423f605b`  
		Last Modified: Wed, 26 Feb 2020 01:07:32 GMT  
		Size: 22.7 MB (22699783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd762b0d48bc41e6bdfdb354ae48b55c2cbe60e2a0ad9cd60a9396304fb48660`  
		Last Modified: Wed, 26 Feb 2020 03:35:50 GMT  
		Size: 4.9 KB (4896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34dccc10f85111d1e9ad7f9118fc95ec338f9510a4fb1d7d847c500212185bf7`  
		Last Modified: Wed, 26 Feb 2020 03:35:57 GMT  
		Size: 1.8 MB (1811579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1aba4da49d87f5f9ee5f89839430139620889df5129d8f26fb948dd6e0738e1`  
		Last Modified: Wed, 18 Mar 2020 00:18:02 GMT  
		Size: 1.1 MB (1127532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:756d789cadf0cc90e8d82cad7000c52c7ad4c5d7984984c58b274a318c70c47c`  
		Last Modified: Wed, 18 Mar 2020 00:18:06 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d3d88a2570cc19347b319b789f0a3aafc02b99ac6c369e1343ba2315994bdb1`  
		Last Modified: Wed, 18 Mar 2020 00:18:17 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:89a48b7232e353e9d13fc62962805abcd59e6f69bfd363c03b0b47c0fba0534a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.1 MB (29091968 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a3d7d5d254344a16e0d4d3a008c5108f77c7e872f7f7649fa3ac50ce1aad6ed1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 26 Feb 2020 00:46:51 GMT
ADD file:a93818b0ffcb2823807811dffd78092a3e3f4981aabf48c3cb75f2fa319ac055 in / 
# Wed, 26 Feb 2020 00:46:55 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 13:34:13 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 26 Feb 2020 13:34:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Mar 2020 20:41:15 GMT
ENV MEMCACHED_VERSION=1.6.1
# Tue, 17 Mar 2020 20:41:16 GMT
ENV MEMCACHED_SHA1=6e337924dbf953bfabda512405d710d9757c97c1
# Tue, 17 Mar 2020 20:50:18 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 17 Mar 2020 20:50:18 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 17 Mar 2020 20:50:20 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 17 Mar 2020 20:50:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 17 Mar 2020 20:50:21 GMT
USER memcache
# Tue, 17 Mar 2020 20:50:22 GMT
EXPOSE 11211
# Tue, 17 Mar 2020 20:50:22 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:f338bc35613f66cfaad272234de7b77a91d6c5422855bf6239f2b0ff9d73f0a4`  
		Last Modified: Wed, 26 Feb 2020 00:56:15 GMT  
		Size: 25.9 MB (25851563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4d7ac360be705ceb72083cd1a2c07b2fd7f572f0cd8de06e6733c8f217739a2`  
		Last Modified: Wed, 26 Feb 2020 14:00:56 GMT  
		Size: 5.0 KB (5029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bd27757fe5a945d701f8f5bd7534c41588270d8f2b934ca8085e0a649cbbf91`  
		Last Modified: Wed, 26 Feb 2020 14:00:56 GMT  
		Size: 2.1 MB (2074945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc7a620a01855a969584241d573d1e6acf55dee0e7e6c4f8d4c821b6b0064637`  
		Last Modified: Tue, 17 Mar 2020 20:59:55 GMT  
		Size: 1.2 MB (1160025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04bcc8eff174cea809be4c1a00052dce74463a60ea51cfb0c0da09ec1e0d8b42`  
		Last Modified: Tue, 17 Mar 2020 20:59:55 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15d59c8d4a0e2a02d465e919de1d0adb45841bbbeb21e78c588a3251cb9f2740`  
		Last Modified: Tue, 17 Mar 2020 20:59:55 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6` - linux; 386

```console
$ docker pull memcached@sha256:c34541b96410e9129064d823a4e89051fd9001f132c51841ca9d6f2fee21078c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.2 MB (31155198 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c89fc4282ec39b4634a263a8481002f3d90d3be4ece62cc10f9cf40d7608f85`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 26 Feb 2020 00:32:17 GMT
ADD file:08977fa54555a1ed2ae44a3aec04df157092a6c1c1b70ce0407cc2dc2f8bcd76 in / 
# Wed, 26 Feb 2020 00:32:17 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 10:57:50 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 26 Feb 2020 10:57:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Mar 2020 21:56:16 GMT
ENV MEMCACHED_VERSION=1.6.1
# Tue, 17 Mar 2020 21:56:17 GMT
ENV MEMCACHED_SHA1=6e337924dbf953bfabda512405d710d9757c97c1
# Tue, 17 Mar 2020 22:05:32 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 17 Mar 2020 22:05:33 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 17 Mar 2020 22:05:34 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 17 Mar 2020 22:05:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 17 Mar 2020 22:05:35 GMT
USER memcache
# Tue, 17 Mar 2020 22:05:35 GMT
EXPOSE 11211
# Tue, 17 Mar 2020 22:05:35 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:1de10f1ae2a5bfd5f34f19421ebd282580e443321e4947cdf5f943875782b018`  
		Last Modified: Wed, 26 Feb 2020 00:38:34 GMT  
		Size: 27.7 MB (27747667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40f6886cf964eb4f4025c8157f9756ae21437cdf1a57f5fe279849787aff082b`  
		Last Modified: Wed, 26 Feb 2020 11:06:50 GMT  
		Size: 4.9 KB (4893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d843b4e4e2bb25c8a0fb82174c608d57f8eb0ac3e8f3773c31c988a34857030`  
		Last Modified: Wed, 26 Feb 2020 11:06:50 GMT  
		Size: 2.2 MB (2208102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28a0ed0844b264f9c1207229402186f1fff548292e028cb9a1c254402763364c`  
		Last Modified: Tue, 17 Mar 2020 22:14:44 GMT  
		Size: 1.2 MB (1194128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c2889f61fb8cb96b3ec44d3036bda0cef5e06e7703a4df8876adf9792462aa8`  
		Last Modified: Tue, 17 Mar 2020 22:14:44 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7d9bc4abf0879c8f9c4cb3d9d4551d03033f7e3356fd9df07c8c69ee60ff63f`  
		Last Modified: Tue, 17 Mar 2020 22:14:44 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6` - linux; ppc64le

```console
$ docker pull memcached@sha256:010267e365a1b82e10d694473d416094c5a196dc8d778a8c2d383ac2558c6a50
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.1 MB (34061620 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dbb12046217f66e43361864882561c2b935d472dc219f6d90d6824a6cab4cad1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 26 Feb 2020 01:31:23 GMT
ADD file:430f1f769b86c60db1b8d2f96ed26c24837b3ff5730264be42a9c0cd8e43df7f in / 
# Wed, 26 Feb 2020 01:31:29 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 08:58:42 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 26 Feb 2020 08:59:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Mar 2020 22:07:27 GMT
ENV MEMCACHED_VERSION=1.6.1
# Tue, 17 Mar 2020 22:07:29 GMT
ENV MEMCACHED_SHA1=6e337924dbf953bfabda512405d710d9757c97c1
# Tue, 17 Mar 2020 22:17:35 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 17 Mar 2020 22:17:37 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 17 Mar 2020 22:17:43 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 17 Mar 2020 22:17:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 17 Mar 2020 22:17:47 GMT
USER memcache
# Tue, 17 Mar 2020 22:17:49 GMT
EXPOSE 11211
# Tue, 17 Mar 2020 22:17:52 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:975241fcd2057cc8f4cb8f066d68ed18877152b88da11e682911ccc3bc3da7c4`  
		Last Modified: Wed, 26 Feb 2020 01:52:57 GMT  
		Size: 30.5 MB (30518427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c4567bf2efa314a53153932738e79b856d675d83e768d2e2ce3ab5b45930ace`  
		Last Modified: Wed, 26 Feb 2020 09:10:20 GMT  
		Size: 5.0 KB (4985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63966b4eb4cf356b52b220fc08251ec17ddb06f1425096935b9dbe79c39e5bb5`  
		Last Modified: Wed, 26 Feb 2020 09:10:20 GMT  
		Size: 2.3 MB (2322659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f210835730fc44353def79514fb093d60f6442f97c0fffaa7dc0962a6ba887a`  
		Last Modified: Tue, 17 Mar 2020 22:27:10 GMT  
		Size: 1.2 MB (1215142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fde09d96ef673b71efb6670819cea32e1454fe672a42f7377f396277e48c40b7`  
		Last Modified: Tue, 17 Mar 2020 22:27:09 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efca2b06ccc0d3c5720838c60727aad27be7400487ab096e48113b6a2be2e5ae`  
		Last Modified: Tue, 17 Mar 2020 22:27:09 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:1.6.1`

```console
$ docker pull memcached@sha256:96fa7f208b93c7f62f1febf8b5c38f8fd45230a708207b3e7eda98b4cff93bfc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `memcached:1.6.1` - linux; amd64

```console
$ docker pull memcached@sha256:f01d94f9c4adae3a566151be2b41e9e0ab5410ef3fcb4e69e92226173c7f7259
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.5 MB (30483498 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:20188fe150aa349793b646f31dde86a97c2a60989b76bf01df11ec97e79f6a3f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 26 Feb 2020 00:37:39 GMT
ADD file:e5a364615e0f6961626089c7d658adbf8c8d95b3ae95a390a8bb33875317d434 in / 
# Wed, 26 Feb 2020 00:37:39 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 18:07:47 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 26 Feb 2020 18:07:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Mar 2020 23:22:04 GMT
ENV MEMCACHED_VERSION=1.6.1
# Tue, 17 Mar 2020 23:22:04 GMT
ENV MEMCACHED_SHA1=6e337924dbf953bfabda512405d710d9757c97c1
# Tue, 17 Mar 2020 23:30:13 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 17 Mar 2020 23:30:13 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 17 Mar 2020 23:30:14 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 17 Mar 2020 23:30:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 17 Mar 2020 23:30:14 GMT
USER memcache
# Tue, 17 Mar 2020 23:30:14 GMT
EXPOSE 11211
# Tue, 17 Mar 2020 23:30:14 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:68ced04f60ab5c7a5f1d0b0b4e7572c5a4c8cce44866513d30d9df1a15277d6b`  
		Last Modified: Wed, 26 Feb 2020 00:44:23 GMT  
		Size: 27.1 MB (27091819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7233c6ae94c59c690ba7007d1f0e360f97b515b3df0a5adc0a8e0c71e48dc836`  
		Last Modified: Wed, 26 Feb 2020 18:16:20 GMT  
		Size: 5.0 KB (4980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3945a4bf251bce21f9517716e4ed007325a8e8b279e52a09bc15fffa2f65b16d`  
		Last Modified: Wed, 26 Feb 2020 18:16:20 GMT  
		Size: 2.2 MB (2196514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9e46f4b34ecc2434e857dccae8dcefac20010d02aa70739107749e36164a43f`  
		Last Modified: Tue, 17 Mar 2020 23:38:46 GMT  
		Size: 1.2 MB (1189776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca1999a38cda2f5a4349e8b795ff37d1d1ba865a56a18defdaffac68af7800ce`  
		Last Modified: Tue, 17 Mar 2020 23:38:45 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4f797df323b4285de392809bad17d92950319a7753be796ab8b1a86d1666a85`  
		Last Modified: Tue, 17 Mar 2020 23:38:46 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.1` - linux; arm variant v5

```console
$ docker pull memcached@sha256:d32bdb11fd734410cd1be1ae96fa977048cd809329b1a9cae28f4ec2f8b8fb8c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.9 MB (27888005 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1aec9eb200e1be46e4a6da6e72866613bd30e78e8865abd3dfdcb42b7877cca2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 26 Feb 2020 00:47:49 GMT
ADD file:745d3236976c8213b805ca6d14f150561816cd2eeec5aa7e1aaea44d9d5675e9 in / 
# Wed, 26 Feb 2020 00:47:53 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 01:21:35 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 26 Feb 2020 01:23:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Mar 2020 20:48:50 GMT
ENV MEMCACHED_VERSION=1.6.1
# Tue, 17 Mar 2020 20:48:52 GMT
ENV MEMCACHED_SHA1=6e337924dbf953bfabda512405d710d9757c97c1
# Tue, 17 Mar 2020 22:19:10 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 17 Mar 2020 22:19:13 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 17 Mar 2020 22:19:24 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 17 Mar 2020 22:19:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 17 Mar 2020 22:19:28 GMT
USER memcache
# Tue, 17 Mar 2020 22:19:29 GMT
EXPOSE 11211
# Tue, 17 Mar 2020 22:19:31 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:d9f9009f908455fa93c5b3e0d3230df44ea75299b2de375ab35b74193f679076`  
		Last Modified: Wed, 26 Feb 2020 00:59:18 GMT  
		Size: 24.8 MB (24830277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f028832400faf7f954f74987eff7a1e300690055f9df70085c778e354351f5d8`  
		Last Modified: Tue, 10 Mar 2020 13:06:25 GMT  
		Size: 4.9 KB (4895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dee056e35538c22bed8fa9de89eaa5b3ce1bfbce6a93be0b7ce527c378f23cf4`  
		Last Modified: Tue, 10 Mar 2020 13:06:33 GMT  
		Size: 1.9 MB (1896817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4def82d8eadc3db4d32a027dc0072359c4a3133a6bfca570381eed5e782302be`  
		Last Modified: Tue, 17 Mar 2020 22:19:53 GMT  
		Size: 1.2 MB (1155608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82fdc512c93448bbc2be492053f7303bef1efa0a68d7f8f5bbaa64ce758b250e`  
		Last Modified: Tue, 17 Mar 2020 22:19:56 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8003ad16648f331b96907ecf19d95da34b2b68aedf312ca29f1fc6e34ede22ab`  
		Last Modified: Tue, 17 Mar 2020 22:20:07 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.1` - linux; arm variant v7

```console
$ docker pull memcached@sha256:cdf939e755f1f26e266767e417109b3ba044b51d444eff026e83bd1c7195fa9a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.6 MB (25644199 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b99a8df834c831b0c96ac194f07f1df3b4b1b22ac94731bc8ddd6f4f1df4419b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 26 Feb 2020 00:52:11 GMT
ADD file:2488038744e2e15217e67dd7f4bec5dcc7e9abe8a1010fe720a5ba7cbe7ab0eb in / 
# Wed, 26 Feb 2020 00:52:13 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 03:03:14 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 26 Feb 2020 03:05:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Mar 2020 22:23:13 GMT
ENV MEMCACHED_VERSION=1.6.1
# Tue, 17 Mar 2020 22:23:15 GMT
ENV MEMCACHED_SHA1=6e337924dbf953bfabda512405d710d9757c97c1
# Tue, 17 Mar 2020 22:51:58 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 17 Mar 2020 22:52:01 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 17 Mar 2020 22:52:11 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 17 Mar 2020 22:52:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 17 Mar 2020 22:52:15 GMT
USER memcache
# Tue, 17 Mar 2020 22:52:17 GMT
EXPOSE 11211
# Tue, 17 Mar 2020 22:52:19 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:fff3167bf8c79dc08baf67eb607823aadcbee2033f9620cc502e2c49423f605b`  
		Last Modified: Wed, 26 Feb 2020 01:07:32 GMT  
		Size: 22.7 MB (22699783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd762b0d48bc41e6bdfdb354ae48b55c2cbe60e2a0ad9cd60a9396304fb48660`  
		Last Modified: Wed, 26 Feb 2020 03:35:50 GMT  
		Size: 4.9 KB (4896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34dccc10f85111d1e9ad7f9118fc95ec338f9510a4fb1d7d847c500212185bf7`  
		Last Modified: Wed, 26 Feb 2020 03:35:57 GMT  
		Size: 1.8 MB (1811579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1aba4da49d87f5f9ee5f89839430139620889df5129d8f26fb948dd6e0738e1`  
		Last Modified: Wed, 18 Mar 2020 00:18:02 GMT  
		Size: 1.1 MB (1127532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:756d789cadf0cc90e8d82cad7000c52c7ad4c5d7984984c58b274a318c70c47c`  
		Last Modified: Wed, 18 Mar 2020 00:18:06 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d3d88a2570cc19347b319b789f0a3aafc02b99ac6c369e1343ba2315994bdb1`  
		Last Modified: Wed, 18 Mar 2020 00:18:17 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.1` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:89a48b7232e353e9d13fc62962805abcd59e6f69bfd363c03b0b47c0fba0534a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.1 MB (29091968 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a3d7d5d254344a16e0d4d3a008c5108f77c7e872f7f7649fa3ac50ce1aad6ed1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 26 Feb 2020 00:46:51 GMT
ADD file:a93818b0ffcb2823807811dffd78092a3e3f4981aabf48c3cb75f2fa319ac055 in / 
# Wed, 26 Feb 2020 00:46:55 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 13:34:13 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 26 Feb 2020 13:34:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Mar 2020 20:41:15 GMT
ENV MEMCACHED_VERSION=1.6.1
# Tue, 17 Mar 2020 20:41:16 GMT
ENV MEMCACHED_SHA1=6e337924dbf953bfabda512405d710d9757c97c1
# Tue, 17 Mar 2020 20:50:18 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 17 Mar 2020 20:50:18 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 17 Mar 2020 20:50:20 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 17 Mar 2020 20:50:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 17 Mar 2020 20:50:21 GMT
USER memcache
# Tue, 17 Mar 2020 20:50:22 GMT
EXPOSE 11211
# Tue, 17 Mar 2020 20:50:22 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:f338bc35613f66cfaad272234de7b77a91d6c5422855bf6239f2b0ff9d73f0a4`  
		Last Modified: Wed, 26 Feb 2020 00:56:15 GMT  
		Size: 25.9 MB (25851563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4d7ac360be705ceb72083cd1a2c07b2fd7f572f0cd8de06e6733c8f217739a2`  
		Last Modified: Wed, 26 Feb 2020 14:00:56 GMT  
		Size: 5.0 KB (5029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bd27757fe5a945d701f8f5bd7534c41588270d8f2b934ca8085e0a649cbbf91`  
		Last Modified: Wed, 26 Feb 2020 14:00:56 GMT  
		Size: 2.1 MB (2074945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc7a620a01855a969584241d573d1e6acf55dee0e7e6c4f8d4c821b6b0064637`  
		Last Modified: Tue, 17 Mar 2020 20:59:55 GMT  
		Size: 1.2 MB (1160025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04bcc8eff174cea809be4c1a00052dce74463a60ea51cfb0c0da09ec1e0d8b42`  
		Last Modified: Tue, 17 Mar 2020 20:59:55 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15d59c8d4a0e2a02d465e919de1d0adb45841bbbeb21e78c588a3251cb9f2740`  
		Last Modified: Tue, 17 Mar 2020 20:59:55 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.1` - linux; 386

```console
$ docker pull memcached@sha256:c34541b96410e9129064d823a4e89051fd9001f132c51841ca9d6f2fee21078c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.2 MB (31155198 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c89fc4282ec39b4634a263a8481002f3d90d3be4ece62cc10f9cf40d7608f85`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 26 Feb 2020 00:32:17 GMT
ADD file:08977fa54555a1ed2ae44a3aec04df157092a6c1c1b70ce0407cc2dc2f8bcd76 in / 
# Wed, 26 Feb 2020 00:32:17 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 10:57:50 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 26 Feb 2020 10:57:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Mar 2020 21:56:16 GMT
ENV MEMCACHED_VERSION=1.6.1
# Tue, 17 Mar 2020 21:56:17 GMT
ENV MEMCACHED_SHA1=6e337924dbf953bfabda512405d710d9757c97c1
# Tue, 17 Mar 2020 22:05:32 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 17 Mar 2020 22:05:33 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 17 Mar 2020 22:05:34 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 17 Mar 2020 22:05:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 17 Mar 2020 22:05:35 GMT
USER memcache
# Tue, 17 Mar 2020 22:05:35 GMT
EXPOSE 11211
# Tue, 17 Mar 2020 22:05:35 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:1de10f1ae2a5bfd5f34f19421ebd282580e443321e4947cdf5f943875782b018`  
		Last Modified: Wed, 26 Feb 2020 00:38:34 GMT  
		Size: 27.7 MB (27747667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40f6886cf964eb4f4025c8157f9756ae21437cdf1a57f5fe279849787aff082b`  
		Last Modified: Wed, 26 Feb 2020 11:06:50 GMT  
		Size: 4.9 KB (4893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d843b4e4e2bb25c8a0fb82174c608d57f8eb0ac3e8f3773c31c988a34857030`  
		Last Modified: Wed, 26 Feb 2020 11:06:50 GMT  
		Size: 2.2 MB (2208102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28a0ed0844b264f9c1207229402186f1fff548292e028cb9a1c254402763364c`  
		Last Modified: Tue, 17 Mar 2020 22:14:44 GMT  
		Size: 1.2 MB (1194128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c2889f61fb8cb96b3ec44d3036bda0cef5e06e7703a4df8876adf9792462aa8`  
		Last Modified: Tue, 17 Mar 2020 22:14:44 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7d9bc4abf0879c8f9c4cb3d9d4551d03033f7e3356fd9df07c8c69ee60ff63f`  
		Last Modified: Tue, 17 Mar 2020 22:14:44 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.1` - linux; ppc64le

```console
$ docker pull memcached@sha256:010267e365a1b82e10d694473d416094c5a196dc8d778a8c2d383ac2558c6a50
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.1 MB (34061620 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dbb12046217f66e43361864882561c2b935d472dc219f6d90d6824a6cab4cad1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 26 Feb 2020 01:31:23 GMT
ADD file:430f1f769b86c60db1b8d2f96ed26c24837b3ff5730264be42a9c0cd8e43df7f in / 
# Wed, 26 Feb 2020 01:31:29 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 08:58:42 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 26 Feb 2020 08:59:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Mar 2020 22:07:27 GMT
ENV MEMCACHED_VERSION=1.6.1
# Tue, 17 Mar 2020 22:07:29 GMT
ENV MEMCACHED_SHA1=6e337924dbf953bfabda512405d710d9757c97c1
# Tue, 17 Mar 2020 22:17:35 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 17 Mar 2020 22:17:37 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 17 Mar 2020 22:17:43 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 17 Mar 2020 22:17:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 17 Mar 2020 22:17:47 GMT
USER memcache
# Tue, 17 Mar 2020 22:17:49 GMT
EXPOSE 11211
# Tue, 17 Mar 2020 22:17:52 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:975241fcd2057cc8f4cb8f066d68ed18877152b88da11e682911ccc3bc3da7c4`  
		Last Modified: Wed, 26 Feb 2020 01:52:57 GMT  
		Size: 30.5 MB (30518427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c4567bf2efa314a53153932738e79b856d675d83e768d2e2ce3ab5b45930ace`  
		Last Modified: Wed, 26 Feb 2020 09:10:20 GMT  
		Size: 5.0 KB (4985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63966b4eb4cf356b52b220fc08251ec17ddb06f1425096935b9dbe79c39e5bb5`  
		Last Modified: Wed, 26 Feb 2020 09:10:20 GMT  
		Size: 2.3 MB (2322659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f210835730fc44353def79514fb093d60f6442f97c0fffaa7dc0962a6ba887a`  
		Last Modified: Tue, 17 Mar 2020 22:27:10 GMT  
		Size: 1.2 MB (1215142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fde09d96ef673b71efb6670819cea32e1454fe672a42f7377f396277e48c40b7`  
		Last Modified: Tue, 17 Mar 2020 22:27:09 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efca2b06ccc0d3c5720838c60727aad27be7400487ab096e48113b6a2be2e5ae`  
		Last Modified: Tue, 17 Mar 2020 22:27:09 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:1.6.1-alpine`

```console
$ docker pull memcached@sha256:c08f51064dceef8fda9462adb0cb9b1b5ad4f68e5db36c3ff05841fd232eeecd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `memcached:1.6.1-alpine` - linux; amd64

```console
$ docker pull memcached@sha256:db1aef4c33a45c3ff328f0e0ba709a014391f1eb7b2e89b814356d57fca61b01
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.8 MB (4752196 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6bcde295fb9adcc7178da810d6cac1a8bbce83fefd04129e7be63afb276ba7ed`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Sat, 18 Jan 2020 01:19:37 GMT
ADD file:e69d441d729412d24675dcd33e04580885df99981cec43de8c9b24015313ff8e in / 
# Sat, 18 Jan 2020 01:19:37 GMT
CMD ["/bin/sh"]
# Tue, 28 Jan 2020 00:54:55 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 28 Jan 2020 00:54:55 GMT
RUN apk add --no-cache cyrus-sasl-plain
# Tue, 17 Mar 2020 23:30:23 GMT
ENV MEMCACHED_VERSION=1.6.1
# Tue, 17 Mar 2020 23:30:23 GMT
ENV MEMCACHED_SHA1=6e337924dbf953bfabda512405d710d9757c97c1
# Tue, 17 Mar 2020 23:38:29 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		dpkg-dev dpkg 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		tar 		wget 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& make test 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 17 Mar 2020 23:38:30 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 17 Mar 2020 23:38:30 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 17 Mar 2020 23:38:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 17 Mar 2020 23:38:31 GMT
USER memcache
# Tue, 17 Mar 2020 23:38:31 GMT
EXPOSE 11211
# Tue, 17 Mar 2020 23:38:31 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:c9b1b535fdd91a9855fb7f82348177e5f019329a58c53c47272962dd60f71fc9`  
		Last Modified: Fri, 17 Jan 2020 08:04:01 GMT  
		Size: 2.8 MB (2802957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1e93bbcd3846fe31de80a08547eb76193129a81ae7bb50e73236c10f887dc3e`  
		Last Modified: Tue, 28 Jan 2020 01:03:09 GMT  
		Size: 1.2 KB (1231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a48b148dfd515f8ad8eab11710674fe24fa23f1b96349ede10ab1a78a632177`  
		Last Modified: Tue, 28 Jan 2020 01:03:10 GMT  
		Size: 15.1 KB (15093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:542ec47b81d1cd7a041bb77415cc5da2c64c1b2c9589b688f0b9117a883bba5a`  
		Last Modified: Tue, 17 Mar 2020 23:38:52 GMT  
		Size: 1.9 MB (1932512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65bc431706dcb4bc3b5127e45b8a5f8a0056eb6cdb92bbbec2e9fa9fa6217650`  
		Last Modified: Tue, 17 Mar 2020 23:38:51 GMT  
		Size: 282.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc508d65441fe61b4032e0d578353f660018e5129c37370415f2b7321fd1d2a4`  
		Last Modified: Tue, 17 Mar 2020 23:38:51 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.1-alpine` - linux; arm variant v6

```console
$ docker pull memcached@sha256:30a71800ac8815e2c8fb5ae9f56b45b61b7dcdd20a6eb28156c2d5b8b8fd8960
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4524432 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:524dd7062b34155e5603db803be952a17619b6f80c5f0f24d814d9c9db858f79`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Sat, 18 Jan 2020 01:53:16 GMT
ADD file:a1906f14a4e217a498b550f86a3d17c9012c02a6df0668043b63848c8fa44b9b in / 
# Sat, 18 Jan 2020 01:53:17 GMT
CMD ["/bin/sh"]
# Tue, 28 Jan 2020 00:52:27 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 28 Jan 2020 00:52:30 GMT
RUN apk add --no-cache cyrus-sasl-plain
# Tue, 17 Mar 2020 20:49:40 GMT
ENV MEMCACHED_VERSION=1.6.1
# Tue, 17 Mar 2020 20:49:41 GMT
ENV MEMCACHED_SHA1=6e337924dbf953bfabda512405d710d9757c97c1
# Tue, 17 Mar 2020 20:58:42 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		dpkg-dev dpkg 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		tar 		wget 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& make test 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 17 Mar 2020 20:58:43 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 17 Mar 2020 20:58:44 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 17 Mar 2020 20:58:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 17 Mar 2020 20:58:46 GMT
USER memcache
# Tue, 17 Mar 2020 20:58:46 GMT
EXPOSE 11211
# Tue, 17 Mar 2020 20:58:47 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:832e07764099264ef96e50a1e5e41c52d6b0809bd054e29508a6878aa59d156d`  
		Last Modified: Sat, 18 Jan 2020 01:53:52 GMT  
		Size: 2.6 MB (2617562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33c4279c48d90e0c3053099bb9ca915b67b4f057fdc1bfa737cdeff49f7fd3d4`  
		Last Modified: Tue, 28 Jan 2020 01:18:15 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d8eff54bf4684589855264a1239e93563b4da49264da619e3745d2446d2352f`  
		Last Modified: Tue, 28 Jan 2020 01:18:15 GMT  
		Size: 14.7 KB (14697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59e0525cb705a9cc4f63d347edc4befb0167ab3f726bfc56a2a2e9bc76b3c47d`  
		Last Modified: Tue, 17 Mar 2020 20:59:06 GMT  
		Size: 1.9 MB (1890509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c998ca8223a1d93ef5ea43ed575ae519454345d08422b171290c857d54b36ba9`  
		Last Modified: Tue, 17 Mar 2020 20:59:06 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbffc49509b88a96f211604a297cb07aa103f033cb1b53a5dc6b2ce8681abef0`  
		Last Modified: Tue, 17 Mar 2020 20:59:06 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.1-alpine` - linux; arm variant v7

```console
$ docker pull memcached@sha256:0bbd37ffdb170b94768803271712307a679ea3c2defe7fb0152090cec6ba4633
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4180800 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d9bb126ecd328f50fa969d980bead57d7b0ae41d51d35adfe2905e5b88cef512`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Sat, 18 Jan 2020 02:03:19 GMT
ADD file:4c815f4461ff3b8d481f43d84eb2548cb1adbb3015d370cab86dd7f4d3d94279 in / 
# Sat, 18 Jan 2020 02:03:22 GMT
CMD ["/bin/sh"]
# Tue, 28 Jan 2020 01:30:43 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 28 Jan 2020 01:30:55 GMT
RUN apk add --no-cache cyrus-sasl-plain
# Tue, 17 Mar 2020 22:52:32 GMT
ENV MEMCACHED_VERSION=1.6.1
# Tue, 17 Mar 2020 22:52:34 GMT
ENV MEMCACHED_SHA1=6e337924dbf953bfabda512405d710d9757c97c1
# Wed, 18 Mar 2020 01:16:18 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		dpkg-dev dpkg 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		tar 		wget 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& make test 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Wed, 18 Mar 2020 01:16:21 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 18 Mar 2020 01:16:32 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 18 Mar 2020 01:16:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 18 Mar 2020 01:16:36 GMT
USER memcache
# Wed, 18 Mar 2020 01:16:37 GMT
EXPOSE 11211
# Wed, 18 Mar 2020 01:16:39 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:3a2c5e3c37b2e3d749405512ef3793aa45a2f5c11615d9e9efa80179262cdf27`  
		Last Modified: Sat, 18 Jan 2020 02:04:05 GMT  
		Size: 2.4 MB (2419554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aa3e71e259912bc94119737267a874d423f639be13083765352c8d6f2fe2a6b`  
		Last Modified: Tue, 28 Jan 2020 12:23:43 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b9e1375e31fb539b7ca784d44d0cc4c37ac2e6f8239f4295213ca9500ccfcaa`  
		Last Modified: Tue, 28 Jan 2020 12:23:46 GMT  
		Size: 13.6 KB (13639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4efe2f16f62c2c6353e05ff8636454d71b14c132b3c3da88fc57f736b809dd2`  
		Last Modified: Wed, 18 Mar 2020 01:16:57 GMT  
		Size: 1.7 MB (1745940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6b847bebc1791a57ece10d729f50a457f4d3662fc77578ea1d9d9558919ee18`  
		Last Modified: Wed, 18 Mar 2020 01:17:01 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4c1bcfe68d4e7de06a63bb805865b81e7a0f434b774c0536c56b7b48ba5b2a3`  
		Last Modified: Wed, 18 Mar 2020 01:17:01 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.1-alpine` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:928c28f46dfe5dbcbceaa280f3e987bbad267d132d5fc5c1f952e7c935ca100b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4681073 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:668fc1e0a18d8c0a919cf8554bca06abaafcd581a191acae2a217c7687e03646`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Sat, 18 Jan 2020 01:39:43 GMT
ADD file:4109fa86dd80850e84c689ff9e6a3243e30ab1bbcc00c765969b3011bfbb43e1 in / 
# Sat, 18 Jan 2020 01:39:43 GMT
CMD ["/bin/sh"]
# Tue, 28 Jan 2020 00:53:38 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 28 Jan 2020 00:53:41 GMT
RUN apk add --no-cache cyrus-sasl-plain
# Tue, 17 Mar 2020 20:50:40 GMT
ENV MEMCACHED_VERSION=1.6.1
# Tue, 17 Mar 2020 20:50:41 GMT
ENV MEMCACHED_SHA1=6e337924dbf953bfabda512405d710d9757c97c1
# Tue, 17 Mar 2020 20:59:29 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		dpkg-dev dpkg 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		tar 		wget 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& make test 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 17 Mar 2020 20:59:30 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 17 Mar 2020 20:59:32 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 17 Mar 2020 20:59:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 17 Mar 2020 20:59:34 GMT
USER memcache
# Tue, 17 Mar 2020 20:59:35 GMT
EXPOSE 11211
# Tue, 17 Mar 2020 20:59:36 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:8fa90b21c985a6fcfff966bdfbde81cdd088de0aa8af38110057f6ac408f4408`  
		Last Modified: Sat, 18 Jan 2020 01:40:23 GMT  
		Size: 2.7 MB (2723075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cd06d9fb7c7820b59243e32290da8b6bc1e1719c0e1288f468936fa95091ff8`  
		Last Modified: Tue, 28 Jan 2020 01:11:01 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35ab3f89cfc542b0a3b8755ffd6bca6897778e9a3814c52589d388834b7156f2`  
		Last Modified: Tue, 28 Jan 2020 01:11:01 GMT  
		Size: 15.5 KB (15491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e7ea0f6e1e34d5cc2bcb05961ac73b83d75bc11a8bc2094d4bad1b2f127e437`  
		Last Modified: Tue, 17 Mar 2020 21:00:05 GMT  
		Size: 1.9 MB (1940839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43b9cee046785a0858fce8529dc10cb2203f0e2ab396231dda5cebfb18d94f78`  
		Last Modified: Tue, 17 Mar 2020 21:00:05 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8012377072c15ce103f473483c97b8e2324313c4b90d12d8d429c92a565976bf`  
		Last Modified: Tue, 17 Mar 2020 21:00:04 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.1-alpine` - linux; 386

```console
$ docker pull memcached@sha256:26e8ae37960af95ccb2d90e17e674c0c9a4df70535a4c33369813cd4252dc288
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.8 MB (4843276 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f9f4bc9657493d8c477aa7737dfba44f8aa7ec9daa2efe557e6e139e99b2fb81`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Sat, 18 Jan 2020 01:38:44 GMT
ADD file:381b617b92fe699ad4ef4f30e0d9599f89e43e252883348c420ebe2a0cccbd63 in / 
# Sat, 18 Jan 2020 01:38:45 GMT
CMD ["/bin/sh"]
# Tue, 28 Jan 2020 00:48:42 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 28 Jan 2020 00:48:43 GMT
RUN apk add --no-cache cyrus-sasl-plain
# Tue, 17 Mar 2020 22:05:51 GMT
ENV MEMCACHED_VERSION=1.6.1
# Tue, 17 Mar 2020 22:05:51 GMT
ENV MEMCACHED_SHA1=6e337924dbf953bfabda512405d710d9757c97c1
# Tue, 17 Mar 2020 22:14:29 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		dpkg-dev dpkg 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		tar 		wget 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& make test 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 17 Mar 2020 22:14:30 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 17 Mar 2020 22:14:30 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 17 Mar 2020 22:14:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 17 Mar 2020 22:14:31 GMT
USER memcache
# Tue, 17 Mar 2020 22:14:31 GMT
EXPOSE 11211
# Tue, 17 Mar 2020 22:14:31 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:f024b1263dc58db07a458b73ae1a2dca02ca55bef1ccd1fa3fd50656551fadf2`  
		Last Modified: Sat, 18 Jan 2020 01:39:18 GMT  
		Size: 2.8 MB (2806560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:431aabc4c24cdeaae3c25e5699ac6e79b8fb26d6b3bca55a800adfe777501e4e`  
		Last Modified: Tue, 28 Jan 2020 00:56:57 GMT  
		Size: 1.2 KB (1230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3597117016445fddae7449ab0e8e29d459d0e7cda1b6e76e2e3645338df003b7`  
		Last Modified: Tue, 28 Jan 2020 00:56:57 GMT  
		Size: 16.2 KB (16154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1840db45b1a27f8b00fa66768a3a172aed97e40512f841b032af22220c74f38`  
		Last Modified: Tue, 17 Mar 2020 22:14:49 GMT  
		Size: 2.0 MB (2018927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f71f6c3b0eac6fd20b6005cc8c0fceb8b30093c22f4cd918e1bf7e846dca3278`  
		Last Modified: Tue, 17 Mar 2020 22:14:49 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d725c8ed1dbb90202f4b25f3deccb5bcaff15386dc30af32f3f3c9cbd038281f`  
		Last Modified: Tue, 17 Mar 2020 22:14:49 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.1-alpine` - linux; ppc64le

```console
$ docker pull memcached@sha256:97381f0b46139d6041860dce1d3f378bb7c1a46852f9dbd6d85964f266101a35
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.8 MB (4834234 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a7bf667b9acf3f4784fc4f22b12e5a488fa8f65ad7e7cc00233086e0661a920`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Sat, 18 Jan 2020 02:20:41 GMT
ADD file:32ddb3d5255071cca51573ceee2464dd5a87c8d1cce514ae965b6e824d9ef24b in / 
# Sat, 18 Jan 2020 02:20:45 GMT
CMD ["/bin/sh"]
# Tue, 28 Jan 2020 00:56:10 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 28 Jan 2020 00:56:17 GMT
RUN apk add --no-cache cyrus-sasl-plain
# Tue, 17 Mar 2020 22:18:07 GMT
ENV MEMCACHED_VERSION=1.6.1
# Tue, 17 Mar 2020 22:18:09 GMT
ENV MEMCACHED_SHA1=6e337924dbf953bfabda512405d710d9757c97c1
# Tue, 17 Mar 2020 22:26:36 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		dpkg-dev dpkg 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		tar 		wget 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& make test 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 17 Mar 2020 22:26:37 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 17 Mar 2020 22:26:44 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 17 Mar 2020 22:26:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 17 Mar 2020 22:26:48 GMT
USER memcache
# Tue, 17 Mar 2020 22:26:53 GMT
EXPOSE 11211
# Tue, 17 Mar 2020 22:26:55 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:cd95c8a93e39dcaa0634a65d5b86a88bcd5c3092adb1f96504a7030faa165123`  
		Last Modified: Sat, 18 Jan 2020 02:21:25 GMT  
		Size: 2.8 MB (2822125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cc791749867123bab1a791891ae28e057ee5304e839f0e30fb11c01e3b117c9`  
		Last Modified: Tue, 28 Jan 2020 01:04:59 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17e510e23cde584149c483ecd997b1f57d4bd61ccaf28adef58583ae25ad6d5a`  
		Last Modified: Tue, 28 Jan 2020 01:04:58 GMT  
		Size: 16.1 KB (16135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e5709f59fa1d0e31b6f80b187befa21232cb667ac0b780535c3d698343ac7de`  
		Last Modified: Tue, 17 Mar 2020 22:27:26 GMT  
		Size: 2.0 MB (1994308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47c95bf2e7da41d366113c4a2b0f6a2766e707b9f316dee2881660aa41e32946`  
		Last Modified: Tue, 17 Mar 2020 22:27:25 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc7129936aeed99915bf58fa5dda941352c516c1975bfd50e7f41019973aca2d`  
		Last Modified: Tue, 17 Mar 2020 22:27:26 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:1.6-alpine`

```console
$ docker pull memcached@sha256:c08f51064dceef8fda9462adb0cb9b1b5ad4f68e5db36c3ff05841fd232eeecd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `memcached:1.6-alpine` - linux; amd64

```console
$ docker pull memcached@sha256:db1aef4c33a45c3ff328f0e0ba709a014391f1eb7b2e89b814356d57fca61b01
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.8 MB (4752196 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6bcde295fb9adcc7178da810d6cac1a8bbce83fefd04129e7be63afb276ba7ed`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Sat, 18 Jan 2020 01:19:37 GMT
ADD file:e69d441d729412d24675dcd33e04580885df99981cec43de8c9b24015313ff8e in / 
# Sat, 18 Jan 2020 01:19:37 GMT
CMD ["/bin/sh"]
# Tue, 28 Jan 2020 00:54:55 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 28 Jan 2020 00:54:55 GMT
RUN apk add --no-cache cyrus-sasl-plain
# Tue, 17 Mar 2020 23:30:23 GMT
ENV MEMCACHED_VERSION=1.6.1
# Tue, 17 Mar 2020 23:30:23 GMT
ENV MEMCACHED_SHA1=6e337924dbf953bfabda512405d710d9757c97c1
# Tue, 17 Mar 2020 23:38:29 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		dpkg-dev dpkg 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		tar 		wget 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& make test 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 17 Mar 2020 23:38:30 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 17 Mar 2020 23:38:30 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 17 Mar 2020 23:38:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 17 Mar 2020 23:38:31 GMT
USER memcache
# Tue, 17 Mar 2020 23:38:31 GMT
EXPOSE 11211
# Tue, 17 Mar 2020 23:38:31 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:c9b1b535fdd91a9855fb7f82348177e5f019329a58c53c47272962dd60f71fc9`  
		Last Modified: Fri, 17 Jan 2020 08:04:01 GMT  
		Size: 2.8 MB (2802957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1e93bbcd3846fe31de80a08547eb76193129a81ae7bb50e73236c10f887dc3e`  
		Last Modified: Tue, 28 Jan 2020 01:03:09 GMT  
		Size: 1.2 KB (1231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a48b148dfd515f8ad8eab11710674fe24fa23f1b96349ede10ab1a78a632177`  
		Last Modified: Tue, 28 Jan 2020 01:03:10 GMT  
		Size: 15.1 KB (15093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:542ec47b81d1cd7a041bb77415cc5da2c64c1b2c9589b688f0b9117a883bba5a`  
		Last Modified: Tue, 17 Mar 2020 23:38:52 GMT  
		Size: 1.9 MB (1932512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65bc431706dcb4bc3b5127e45b8a5f8a0056eb6cdb92bbbec2e9fa9fa6217650`  
		Last Modified: Tue, 17 Mar 2020 23:38:51 GMT  
		Size: 282.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc508d65441fe61b4032e0d578353f660018e5129c37370415f2b7321fd1d2a4`  
		Last Modified: Tue, 17 Mar 2020 23:38:51 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-alpine` - linux; arm variant v6

```console
$ docker pull memcached@sha256:30a71800ac8815e2c8fb5ae9f56b45b61b7dcdd20a6eb28156c2d5b8b8fd8960
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4524432 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:524dd7062b34155e5603db803be952a17619b6f80c5f0f24d814d9c9db858f79`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Sat, 18 Jan 2020 01:53:16 GMT
ADD file:a1906f14a4e217a498b550f86a3d17c9012c02a6df0668043b63848c8fa44b9b in / 
# Sat, 18 Jan 2020 01:53:17 GMT
CMD ["/bin/sh"]
# Tue, 28 Jan 2020 00:52:27 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 28 Jan 2020 00:52:30 GMT
RUN apk add --no-cache cyrus-sasl-plain
# Tue, 17 Mar 2020 20:49:40 GMT
ENV MEMCACHED_VERSION=1.6.1
# Tue, 17 Mar 2020 20:49:41 GMT
ENV MEMCACHED_SHA1=6e337924dbf953bfabda512405d710d9757c97c1
# Tue, 17 Mar 2020 20:58:42 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		dpkg-dev dpkg 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		tar 		wget 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& make test 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 17 Mar 2020 20:58:43 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 17 Mar 2020 20:58:44 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 17 Mar 2020 20:58:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 17 Mar 2020 20:58:46 GMT
USER memcache
# Tue, 17 Mar 2020 20:58:46 GMT
EXPOSE 11211
# Tue, 17 Mar 2020 20:58:47 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:832e07764099264ef96e50a1e5e41c52d6b0809bd054e29508a6878aa59d156d`  
		Last Modified: Sat, 18 Jan 2020 01:53:52 GMT  
		Size: 2.6 MB (2617562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33c4279c48d90e0c3053099bb9ca915b67b4f057fdc1bfa737cdeff49f7fd3d4`  
		Last Modified: Tue, 28 Jan 2020 01:18:15 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d8eff54bf4684589855264a1239e93563b4da49264da619e3745d2446d2352f`  
		Last Modified: Tue, 28 Jan 2020 01:18:15 GMT  
		Size: 14.7 KB (14697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59e0525cb705a9cc4f63d347edc4befb0167ab3f726bfc56a2a2e9bc76b3c47d`  
		Last Modified: Tue, 17 Mar 2020 20:59:06 GMT  
		Size: 1.9 MB (1890509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c998ca8223a1d93ef5ea43ed575ae519454345d08422b171290c857d54b36ba9`  
		Last Modified: Tue, 17 Mar 2020 20:59:06 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbffc49509b88a96f211604a297cb07aa103f033cb1b53a5dc6b2ce8681abef0`  
		Last Modified: Tue, 17 Mar 2020 20:59:06 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-alpine` - linux; arm variant v7

```console
$ docker pull memcached@sha256:0bbd37ffdb170b94768803271712307a679ea3c2defe7fb0152090cec6ba4633
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4180800 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d9bb126ecd328f50fa969d980bead57d7b0ae41d51d35adfe2905e5b88cef512`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Sat, 18 Jan 2020 02:03:19 GMT
ADD file:4c815f4461ff3b8d481f43d84eb2548cb1adbb3015d370cab86dd7f4d3d94279 in / 
# Sat, 18 Jan 2020 02:03:22 GMT
CMD ["/bin/sh"]
# Tue, 28 Jan 2020 01:30:43 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 28 Jan 2020 01:30:55 GMT
RUN apk add --no-cache cyrus-sasl-plain
# Tue, 17 Mar 2020 22:52:32 GMT
ENV MEMCACHED_VERSION=1.6.1
# Tue, 17 Mar 2020 22:52:34 GMT
ENV MEMCACHED_SHA1=6e337924dbf953bfabda512405d710d9757c97c1
# Wed, 18 Mar 2020 01:16:18 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		dpkg-dev dpkg 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		tar 		wget 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& make test 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Wed, 18 Mar 2020 01:16:21 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 18 Mar 2020 01:16:32 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 18 Mar 2020 01:16:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 18 Mar 2020 01:16:36 GMT
USER memcache
# Wed, 18 Mar 2020 01:16:37 GMT
EXPOSE 11211
# Wed, 18 Mar 2020 01:16:39 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:3a2c5e3c37b2e3d749405512ef3793aa45a2f5c11615d9e9efa80179262cdf27`  
		Last Modified: Sat, 18 Jan 2020 02:04:05 GMT  
		Size: 2.4 MB (2419554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aa3e71e259912bc94119737267a874d423f639be13083765352c8d6f2fe2a6b`  
		Last Modified: Tue, 28 Jan 2020 12:23:43 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b9e1375e31fb539b7ca784d44d0cc4c37ac2e6f8239f4295213ca9500ccfcaa`  
		Last Modified: Tue, 28 Jan 2020 12:23:46 GMT  
		Size: 13.6 KB (13639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4efe2f16f62c2c6353e05ff8636454d71b14c132b3c3da88fc57f736b809dd2`  
		Last Modified: Wed, 18 Mar 2020 01:16:57 GMT  
		Size: 1.7 MB (1745940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6b847bebc1791a57ece10d729f50a457f4d3662fc77578ea1d9d9558919ee18`  
		Last Modified: Wed, 18 Mar 2020 01:17:01 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4c1bcfe68d4e7de06a63bb805865b81e7a0f434b774c0536c56b7b48ba5b2a3`  
		Last Modified: Wed, 18 Mar 2020 01:17:01 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-alpine` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:928c28f46dfe5dbcbceaa280f3e987bbad267d132d5fc5c1f952e7c935ca100b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4681073 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:668fc1e0a18d8c0a919cf8554bca06abaafcd581a191acae2a217c7687e03646`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Sat, 18 Jan 2020 01:39:43 GMT
ADD file:4109fa86dd80850e84c689ff9e6a3243e30ab1bbcc00c765969b3011bfbb43e1 in / 
# Sat, 18 Jan 2020 01:39:43 GMT
CMD ["/bin/sh"]
# Tue, 28 Jan 2020 00:53:38 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 28 Jan 2020 00:53:41 GMT
RUN apk add --no-cache cyrus-sasl-plain
# Tue, 17 Mar 2020 20:50:40 GMT
ENV MEMCACHED_VERSION=1.6.1
# Tue, 17 Mar 2020 20:50:41 GMT
ENV MEMCACHED_SHA1=6e337924dbf953bfabda512405d710d9757c97c1
# Tue, 17 Mar 2020 20:59:29 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		dpkg-dev dpkg 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		tar 		wget 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& make test 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 17 Mar 2020 20:59:30 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 17 Mar 2020 20:59:32 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 17 Mar 2020 20:59:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 17 Mar 2020 20:59:34 GMT
USER memcache
# Tue, 17 Mar 2020 20:59:35 GMT
EXPOSE 11211
# Tue, 17 Mar 2020 20:59:36 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:8fa90b21c985a6fcfff966bdfbde81cdd088de0aa8af38110057f6ac408f4408`  
		Last Modified: Sat, 18 Jan 2020 01:40:23 GMT  
		Size: 2.7 MB (2723075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cd06d9fb7c7820b59243e32290da8b6bc1e1719c0e1288f468936fa95091ff8`  
		Last Modified: Tue, 28 Jan 2020 01:11:01 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35ab3f89cfc542b0a3b8755ffd6bca6897778e9a3814c52589d388834b7156f2`  
		Last Modified: Tue, 28 Jan 2020 01:11:01 GMT  
		Size: 15.5 KB (15491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e7ea0f6e1e34d5cc2bcb05961ac73b83d75bc11a8bc2094d4bad1b2f127e437`  
		Last Modified: Tue, 17 Mar 2020 21:00:05 GMT  
		Size: 1.9 MB (1940839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43b9cee046785a0858fce8529dc10cb2203f0e2ab396231dda5cebfb18d94f78`  
		Last Modified: Tue, 17 Mar 2020 21:00:05 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8012377072c15ce103f473483c97b8e2324313c4b90d12d8d429c92a565976bf`  
		Last Modified: Tue, 17 Mar 2020 21:00:04 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-alpine` - linux; 386

```console
$ docker pull memcached@sha256:26e8ae37960af95ccb2d90e17e674c0c9a4df70535a4c33369813cd4252dc288
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.8 MB (4843276 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f9f4bc9657493d8c477aa7737dfba44f8aa7ec9daa2efe557e6e139e99b2fb81`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Sat, 18 Jan 2020 01:38:44 GMT
ADD file:381b617b92fe699ad4ef4f30e0d9599f89e43e252883348c420ebe2a0cccbd63 in / 
# Sat, 18 Jan 2020 01:38:45 GMT
CMD ["/bin/sh"]
# Tue, 28 Jan 2020 00:48:42 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 28 Jan 2020 00:48:43 GMT
RUN apk add --no-cache cyrus-sasl-plain
# Tue, 17 Mar 2020 22:05:51 GMT
ENV MEMCACHED_VERSION=1.6.1
# Tue, 17 Mar 2020 22:05:51 GMT
ENV MEMCACHED_SHA1=6e337924dbf953bfabda512405d710d9757c97c1
# Tue, 17 Mar 2020 22:14:29 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		dpkg-dev dpkg 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		tar 		wget 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& make test 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 17 Mar 2020 22:14:30 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 17 Mar 2020 22:14:30 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 17 Mar 2020 22:14:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 17 Mar 2020 22:14:31 GMT
USER memcache
# Tue, 17 Mar 2020 22:14:31 GMT
EXPOSE 11211
# Tue, 17 Mar 2020 22:14:31 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:f024b1263dc58db07a458b73ae1a2dca02ca55bef1ccd1fa3fd50656551fadf2`  
		Last Modified: Sat, 18 Jan 2020 01:39:18 GMT  
		Size: 2.8 MB (2806560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:431aabc4c24cdeaae3c25e5699ac6e79b8fb26d6b3bca55a800adfe777501e4e`  
		Last Modified: Tue, 28 Jan 2020 00:56:57 GMT  
		Size: 1.2 KB (1230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3597117016445fddae7449ab0e8e29d459d0e7cda1b6e76e2e3645338df003b7`  
		Last Modified: Tue, 28 Jan 2020 00:56:57 GMT  
		Size: 16.2 KB (16154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1840db45b1a27f8b00fa66768a3a172aed97e40512f841b032af22220c74f38`  
		Last Modified: Tue, 17 Mar 2020 22:14:49 GMT  
		Size: 2.0 MB (2018927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f71f6c3b0eac6fd20b6005cc8c0fceb8b30093c22f4cd918e1bf7e846dca3278`  
		Last Modified: Tue, 17 Mar 2020 22:14:49 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d725c8ed1dbb90202f4b25f3deccb5bcaff15386dc30af32f3f3c9cbd038281f`  
		Last Modified: Tue, 17 Mar 2020 22:14:49 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-alpine` - linux; ppc64le

```console
$ docker pull memcached@sha256:97381f0b46139d6041860dce1d3f378bb7c1a46852f9dbd6d85964f266101a35
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.8 MB (4834234 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a7bf667b9acf3f4784fc4f22b12e5a488fa8f65ad7e7cc00233086e0661a920`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Sat, 18 Jan 2020 02:20:41 GMT
ADD file:32ddb3d5255071cca51573ceee2464dd5a87c8d1cce514ae965b6e824d9ef24b in / 
# Sat, 18 Jan 2020 02:20:45 GMT
CMD ["/bin/sh"]
# Tue, 28 Jan 2020 00:56:10 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 28 Jan 2020 00:56:17 GMT
RUN apk add --no-cache cyrus-sasl-plain
# Tue, 17 Mar 2020 22:18:07 GMT
ENV MEMCACHED_VERSION=1.6.1
# Tue, 17 Mar 2020 22:18:09 GMT
ENV MEMCACHED_SHA1=6e337924dbf953bfabda512405d710d9757c97c1
# Tue, 17 Mar 2020 22:26:36 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		dpkg-dev dpkg 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		tar 		wget 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& make test 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 17 Mar 2020 22:26:37 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 17 Mar 2020 22:26:44 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 17 Mar 2020 22:26:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 17 Mar 2020 22:26:48 GMT
USER memcache
# Tue, 17 Mar 2020 22:26:53 GMT
EXPOSE 11211
# Tue, 17 Mar 2020 22:26:55 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:cd95c8a93e39dcaa0634a65d5b86a88bcd5c3092adb1f96504a7030faa165123`  
		Last Modified: Sat, 18 Jan 2020 02:21:25 GMT  
		Size: 2.8 MB (2822125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cc791749867123bab1a791891ae28e057ee5304e839f0e30fb11c01e3b117c9`  
		Last Modified: Tue, 28 Jan 2020 01:04:59 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17e510e23cde584149c483ecd997b1f57d4bd61ccaf28adef58583ae25ad6d5a`  
		Last Modified: Tue, 28 Jan 2020 01:04:58 GMT  
		Size: 16.1 KB (16135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e5709f59fa1d0e31b6f80b187befa21232cb667ac0b780535c3d698343ac7de`  
		Last Modified: Tue, 17 Mar 2020 22:27:26 GMT  
		Size: 2.0 MB (1994308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47c95bf2e7da41d366113c4a2b0f6a2766e707b9f316dee2881660aa41e32946`  
		Last Modified: Tue, 17 Mar 2020 22:27:25 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc7129936aeed99915bf58fa5dda941352c516c1975bfd50e7f41019973aca2d`  
		Last Modified: Tue, 17 Mar 2020 22:27:26 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:1-alpine`

```console
$ docker pull memcached@sha256:891a989217a70d9b703bc93ea63e87c9853c0590458f2fec44c7cb95fa224858
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

### `memcached:1-alpine` - linux; amd64

```console
$ docker pull memcached@sha256:db1aef4c33a45c3ff328f0e0ba709a014391f1eb7b2e89b814356d57fca61b01
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.8 MB (4752196 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6bcde295fb9adcc7178da810d6cac1a8bbce83fefd04129e7be63afb276ba7ed`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Sat, 18 Jan 2020 01:19:37 GMT
ADD file:e69d441d729412d24675dcd33e04580885df99981cec43de8c9b24015313ff8e in / 
# Sat, 18 Jan 2020 01:19:37 GMT
CMD ["/bin/sh"]
# Tue, 28 Jan 2020 00:54:55 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 28 Jan 2020 00:54:55 GMT
RUN apk add --no-cache cyrus-sasl-plain
# Tue, 17 Mar 2020 23:30:23 GMT
ENV MEMCACHED_VERSION=1.6.1
# Tue, 17 Mar 2020 23:30:23 GMT
ENV MEMCACHED_SHA1=6e337924dbf953bfabda512405d710d9757c97c1
# Tue, 17 Mar 2020 23:38:29 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		dpkg-dev dpkg 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		tar 		wget 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& make test 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 17 Mar 2020 23:38:30 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 17 Mar 2020 23:38:30 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 17 Mar 2020 23:38:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 17 Mar 2020 23:38:31 GMT
USER memcache
# Tue, 17 Mar 2020 23:38:31 GMT
EXPOSE 11211
# Tue, 17 Mar 2020 23:38:31 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:c9b1b535fdd91a9855fb7f82348177e5f019329a58c53c47272962dd60f71fc9`  
		Last Modified: Fri, 17 Jan 2020 08:04:01 GMT  
		Size: 2.8 MB (2802957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1e93bbcd3846fe31de80a08547eb76193129a81ae7bb50e73236c10f887dc3e`  
		Last Modified: Tue, 28 Jan 2020 01:03:09 GMT  
		Size: 1.2 KB (1231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a48b148dfd515f8ad8eab11710674fe24fa23f1b96349ede10ab1a78a632177`  
		Last Modified: Tue, 28 Jan 2020 01:03:10 GMT  
		Size: 15.1 KB (15093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:542ec47b81d1cd7a041bb77415cc5da2c64c1b2c9589b688f0b9117a883bba5a`  
		Last Modified: Tue, 17 Mar 2020 23:38:52 GMT  
		Size: 1.9 MB (1932512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65bc431706dcb4bc3b5127e45b8a5f8a0056eb6cdb92bbbec2e9fa9fa6217650`  
		Last Modified: Tue, 17 Mar 2020 23:38:51 GMT  
		Size: 282.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc508d65441fe61b4032e0d578353f660018e5129c37370415f2b7321fd1d2a4`  
		Last Modified: Tue, 17 Mar 2020 23:38:51 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-alpine` - linux; arm variant v6

```console
$ docker pull memcached@sha256:30a71800ac8815e2c8fb5ae9f56b45b61b7dcdd20a6eb28156c2d5b8b8fd8960
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4524432 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:524dd7062b34155e5603db803be952a17619b6f80c5f0f24d814d9c9db858f79`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Sat, 18 Jan 2020 01:53:16 GMT
ADD file:a1906f14a4e217a498b550f86a3d17c9012c02a6df0668043b63848c8fa44b9b in / 
# Sat, 18 Jan 2020 01:53:17 GMT
CMD ["/bin/sh"]
# Tue, 28 Jan 2020 00:52:27 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 28 Jan 2020 00:52:30 GMT
RUN apk add --no-cache cyrus-sasl-plain
# Tue, 17 Mar 2020 20:49:40 GMT
ENV MEMCACHED_VERSION=1.6.1
# Tue, 17 Mar 2020 20:49:41 GMT
ENV MEMCACHED_SHA1=6e337924dbf953bfabda512405d710d9757c97c1
# Tue, 17 Mar 2020 20:58:42 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		dpkg-dev dpkg 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		tar 		wget 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& make test 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 17 Mar 2020 20:58:43 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 17 Mar 2020 20:58:44 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 17 Mar 2020 20:58:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 17 Mar 2020 20:58:46 GMT
USER memcache
# Tue, 17 Mar 2020 20:58:46 GMT
EXPOSE 11211
# Tue, 17 Mar 2020 20:58:47 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:832e07764099264ef96e50a1e5e41c52d6b0809bd054e29508a6878aa59d156d`  
		Last Modified: Sat, 18 Jan 2020 01:53:52 GMT  
		Size: 2.6 MB (2617562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33c4279c48d90e0c3053099bb9ca915b67b4f057fdc1bfa737cdeff49f7fd3d4`  
		Last Modified: Tue, 28 Jan 2020 01:18:15 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d8eff54bf4684589855264a1239e93563b4da49264da619e3745d2446d2352f`  
		Last Modified: Tue, 28 Jan 2020 01:18:15 GMT  
		Size: 14.7 KB (14697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59e0525cb705a9cc4f63d347edc4befb0167ab3f726bfc56a2a2e9bc76b3c47d`  
		Last Modified: Tue, 17 Mar 2020 20:59:06 GMT  
		Size: 1.9 MB (1890509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c998ca8223a1d93ef5ea43ed575ae519454345d08422b171290c857d54b36ba9`  
		Last Modified: Tue, 17 Mar 2020 20:59:06 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbffc49509b88a96f211604a297cb07aa103f033cb1b53a5dc6b2ce8681abef0`  
		Last Modified: Tue, 17 Mar 2020 20:59:06 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-alpine` - linux; arm variant v7

```console
$ docker pull memcached@sha256:0bbd37ffdb170b94768803271712307a679ea3c2defe7fb0152090cec6ba4633
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4180800 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d9bb126ecd328f50fa969d980bead57d7b0ae41d51d35adfe2905e5b88cef512`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Sat, 18 Jan 2020 02:03:19 GMT
ADD file:4c815f4461ff3b8d481f43d84eb2548cb1adbb3015d370cab86dd7f4d3d94279 in / 
# Sat, 18 Jan 2020 02:03:22 GMT
CMD ["/bin/sh"]
# Tue, 28 Jan 2020 01:30:43 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 28 Jan 2020 01:30:55 GMT
RUN apk add --no-cache cyrus-sasl-plain
# Tue, 17 Mar 2020 22:52:32 GMT
ENV MEMCACHED_VERSION=1.6.1
# Tue, 17 Mar 2020 22:52:34 GMT
ENV MEMCACHED_SHA1=6e337924dbf953bfabda512405d710d9757c97c1
# Wed, 18 Mar 2020 01:16:18 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		dpkg-dev dpkg 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		tar 		wget 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& make test 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Wed, 18 Mar 2020 01:16:21 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 18 Mar 2020 01:16:32 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 18 Mar 2020 01:16:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 18 Mar 2020 01:16:36 GMT
USER memcache
# Wed, 18 Mar 2020 01:16:37 GMT
EXPOSE 11211
# Wed, 18 Mar 2020 01:16:39 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:3a2c5e3c37b2e3d749405512ef3793aa45a2f5c11615d9e9efa80179262cdf27`  
		Last Modified: Sat, 18 Jan 2020 02:04:05 GMT  
		Size: 2.4 MB (2419554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aa3e71e259912bc94119737267a874d423f639be13083765352c8d6f2fe2a6b`  
		Last Modified: Tue, 28 Jan 2020 12:23:43 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b9e1375e31fb539b7ca784d44d0cc4c37ac2e6f8239f4295213ca9500ccfcaa`  
		Last Modified: Tue, 28 Jan 2020 12:23:46 GMT  
		Size: 13.6 KB (13639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4efe2f16f62c2c6353e05ff8636454d71b14c132b3c3da88fc57f736b809dd2`  
		Last Modified: Wed, 18 Mar 2020 01:16:57 GMT  
		Size: 1.7 MB (1745940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6b847bebc1791a57ece10d729f50a457f4d3662fc77578ea1d9d9558919ee18`  
		Last Modified: Wed, 18 Mar 2020 01:17:01 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4c1bcfe68d4e7de06a63bb805865b81e7a0f434b774c0536c56b7b48ba5b2a3`  
		Last Modified: Wed, 18 Mar 2020 01:17:01 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-alpine` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:928c28f46dfe5dbcbceaa280f3e987bbad267d132d5fc5c1f952e7c935ca100b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4681073 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:668fc1e0a18d8c0a919cf8554bca06abaafcd581a191acae2a217c7687e03646`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Sat, 18 Jan 2020 01:39:43 GMT
ADD file:4109fa86dd80850e84c689ff9e6a3243e30ab1bbcc00c765969b3011bfbb43e1 in / 
# Sat, 18 Jan 2020 01:39:43 GMT
CMD ["/bin/sh"]
# Tue, 28 Jan 2020 00:53:38 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 28 Jan 2020 00:53:41 GMT
RUN apk add --no-cache cyrus-sasl-plain
# Tue, 17 Mar 2020 20:50:40 GMT
ENV MEMCACHED_VERSION=1.6.1
# Tue, 17 Mar 2020 20:50:41 GMT
ENV MEMCACHED_SHA1=6e337924dbf953bfabda512405d710d9757c97c1
# Tue, 17 Mar 2020 20:59:29 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		dpkg-dev dpkg 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		tar 		wget 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& make test 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 17 Mar 2020 20:59:30 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 17 Mar 2020 20:59:32 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 17 Mar 2020 20:59:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 17 Mar 2020 20:59:34 GMT
USER memcache
# Tue, 17 Mar 2020 20:59:35 GMT
EXPOSE 11211
# Tue, 17 Mar 2020 20:59:36 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:8fa90b21c985a6fcfff966bdfbde81cdd088de0aa8af38110057f6ac408f4408`  
		Last Modified: Sat, 18 Jan 2020 01:40:23 GMT  
		Size: 2.7 MB (2723075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cd06d9fb7c7820b59243e32290da8b6bc1e1719c0e1288f468936fa95091ff8`  
		Last Modified: Tue, 28 Jan 2020 01:11:01 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35ab3f89cfc542b0a3b8755ffd6bca6897778e9a3814c52589d388834b7156f2`  
		Last Modified: Tue, 28 Jan 2020 01:11:01 GMT  
		Size: 15.5 KB (15491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e7ea0f6e1e34d5cc2bcb05961ac73b83d75bc11a8bc2094d4bad1b2f127e437`  
		Last Modified: Tue, 17 Mar 2020 21:00:05 GMT  
		Size: 1.9 MB (1940839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43b9cee046785a0858fce8529dc10cb2203f0e2ab396231dda5cebfb18d94f78`  
		Last Modified: Tue, 17 Mar 2020 21:00:05 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8012377072c15ce103f473483c97b8e2324313c4b90d12d8d429c92a565976bf`  
		Last Modified: Tue, 17 Mar 2020 21:00:04 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-alpine` - linux; 386

```console
$ docker pull memcached@sha256:26e8ae37960af95ccb2d90e17e674c0c9a4df70535a4c33369813cd4252dc288
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.8 MB (4843276 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f9f4bc9657493d8c477aa7737dfba44f8aa7ec9daa2efe557e6e139e99b2fb81`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Sat, 18 Jan 2020 01:38:44 GMT
ADD file:381b617b92fe699ad4ef4f30e0d9599f89e43e252883348c420ebe2a0cccbd63 in / 
# Sat, 18 Jan 2020 01:38:45 GMT
CMD ["/bin/sh"]
# Tue, 28 Jan 2020 00:48:42 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 28 Jan 2020 00:48:43 GMT
RUN apk add --no-cache cyrus-sasl-plain
# Tue, 17 Mar 2020 22:05:51 GMT
ENV MEMCACHED_VERSION=1.6.1
# Tue, 17 Mar 2020 22:05:51 GMT
ENV MEMCACHED_SHA1=6e337924dbf953bfabda512405d710d9757c97c1
# Tue, 17 Mar 2020 22:14:29 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		dpkg-dev dpkg 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		tar 		wget 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& make test 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 17 Mar 2020 22:14:30 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 17 Mar 2020 22:14:30 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 17 Mar 2020 22:14:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 17 Mar 2020 22:14:31 GMT
USER memcache
# Tue, 17 Mar 2020 22:14:31 GMT
EXPOSE 11211
# Tue, 17 Mar 2020 22:14:31 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:f024b1263dc58db07a458b73ae1a2dca02ca55bef1ccd1fa3fd50656551fadf2`  
		Last Modified: Sat, 18 Jan 2020 01:39:18 GMT  
		Size: 2.8 MB (2806560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:431aabc4c24cdeaae3c25e5699ac6e79b8fb26d6b3bca55a800adfe777501e4e`  
		Last Modified: Tue, 28 Jan 2020 00:56:57 GMT  
		Size: 1.2 KB (1230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3597117016445fddae7449ab0e8e29d459d0e7cda1b6e76e2e3645338df003b7`  
		Last Modified: Tue, 28 Jan 2020 00:56:57 GMT  
		Size: 16.2 KB (16154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1840db45b1a27f8b00fa66768a3a172aed97e40512f841b032af22220c74f38`  
		Last Modified: Tue, 17 Mar 2020 22:14:49 GMT  
		Size: 2.0 MB (2018927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f71f6c3b0eac6fd20b6005cc8c0fceb8b30093c22f4cd918e1bf7e846dca3278`  
		Last Modified: Tue, 17 Mar 2020 22:14:49 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d725c8ed1dbb90202f4b25f3deccb5bcaff15386dc30af32f3f3c9cbd038281f`  
		Last Modified: Tue, 17 Mar 2020 22:14:49 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-alpine` - linux; ppc64le

```console
$ docker pull memcached@sha256:97381f0b46139d6041860dce1d3f378bb7c1a46852f9dbd6d85964f266101a35
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.8 MB (4834234 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a7bf667b9acf3f4784fc4f22b12e5a488fa8f65ad7e7cc00233086e0661a920`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Sat, 18 Jan 2020 02:20:41 GMT
ADD file:32ddb3d5255071cca51573ceee2464dd5a87c8d1cce514ae965b6e824d9ef24b in / 
# Sat, 18 Jan 2020 02:20:45 GMT
CMD ["/bin/sh"]
# Tue, 28 Jan 2020 00:56:10 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 28 Jan 2020 00:56:17 GMT
RUN apk add --no-cache cyrus-sasl-plain
# Tue, 17 Mar 2020 22:18:07 GMT
ENV MEMCACHED_VERSION=1.6.1
# Tue, 17 Mar 2020 22:18:09 GMT
ENV MEMCACHED_SHA1=6e337924dbf953bfabda512405d710d9757c97c1
# Tue, 17 Mar 2020 22:26:36 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		dpkg-dev dpkg 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		tar 		wget 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& make test 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 17 Mar 2020 22:26:37 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 17 Mar 2020 22:26:44 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 17 Mar 2020 22:26:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 17 Mar 2020 22:26:48 GMT
USER memcache
# Tue, 17 Mar 2020 22:26:53 GMT
EXPOSE 11211
# Tue, 17 Mar 2020 22:26:55 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:cd95c8a93e39dcaa0634a65d5b86a88bcd5c3092adb1f96504a7030faa165123`  
		Last Modified: Sat, 18 Jan 2020 02:21:25 GMT  
		Size: 2.8 MB (2822125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cc791749867123bab1a791891ae28e057ee5304e839f0e30fb11c01e3b117c9`  
		Last Modified: Tue, 28 Jan 2020 01:04:59 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17e510e23cde584149c483ecd997b1f57d4bd61ccaf28adef58583ae25ad6d5a`  
		Last Modified: Tue, 28 Jan 2020 01:04:58 GMT  
		Size: 16.1 KB (16135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e5709f59fa1d0e31b6f80b187befa21232cb667ac0b780535c3d698343ac7de`  
		Last Modified: Tue, 17 Mar 2020 22:27:26 GMT  
		Size: 2.0 MB (1994308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47c95bf2e7da41d366113c4a2b0f6a2766e707b9f316dee2881660aa41e32946`  
		Last Modified: Tue, 17 Mar 2020 22:27:25 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc7129936aeed99915bf58fa5dda941352c516c1975bfd50e7f41019973aca2d`  
		Last Modified: Tue, 17 Mar 2020 22:27:26 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-alpine` - linux; s390x

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

## `memcached:alpine`

```console
$ docker pull memcached@sha256:891a989217a70d9b703bc93ea63e87c9853c0590458f2fec44c7cb95fa224858
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
$ docker pull memcached@sha256:db1aef4c33a45c3ff328f0e0ba709a014391f1eb7b2e89b814356d57fca61b01
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.8 MB (4752196 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6bcde295fb9adcc7178da810d6cac1a8bbce83fefd04129e7be63afb276ba7ed`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Sat, 18 Jan 2020 01:19:37 GMT
ADD file:e69d441d729412d24675dcd33e04580885df99981cec43de8c9b24015313ff8e in / 
# Sat, 18 Jan 2020 01:19:37 GMT
CMD ["/bin/sh"]
# Tue, 28 Jan 2020 00:54:55 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 28 Jan 2020 00:54:55 GMT
RUN apk add --no-cache cyrus-sasl-plain
# Tue, 17 Mar 2020 23:30:23 GMT
ENV MEMCACHED_VERSION=1.6.1
# Tue, 17 Mar 2020 23:30:23 GMT
ENV MEMCACHED_SHA1=6e337924dbf953bfabda512405d710d9757c97c1
# Tue, 17 Mar 2020 23:38:29 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		dpkg-dev dpkg 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		tar 		wget 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& make test 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 17 Mar 2020 23:38:30 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 17 Mar 2020 23:38:30 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 17 Mar 2020 23:38:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 17 Mar 2020 23:38:31 GMT
USER memcache
# Tue, 17 Mar 2020 23:38:31 GMT
EXPOSE 11211
# Tue, 17 Mar 2020 23:38:31 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:c9b1b535fdd91a9855fb7f82348177e5f019329a58c53c47272962dd60f71fc9`  
		Last Modified: Fri, 17 Jan 2020 08:04:01 GMT  
		Size: 2.8 MB (2802957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1e93bbcd3846fe31de80a08547eb76193129a81ae7bb50e73236c10f887dc3e`  
		Last Modified: Tue, 28 Jan 2020 01:03:09 GMT  
		Size: 1.2 KB (1231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a48b148dfd515f8ad8eab11710674fe24fa23f1b96349ede10ab1a78a632177`  
		Last Modified: Tue, 28 Jan 2020 01:03:10 GMT  
		Size: 15.1 KB (15093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:542ec47b81d1cd7a041bb77415cc5da2c64c1b2c9589b688f0b9117a883bba5a`  
		Last Modified: Tue, 17 Mar 2020 23:38:52 GMT  
		Size: 1.9 MB (1932512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65bc431706dcb4bc3b5127e45b8a5f8a0056eb6cdb92bbbec2e9fa9fa6217650`  
		Last Modified: Tue, 17 Mar 2020 23:38:51 GMT  
		Size: 282.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc508d65441fe61b4032e0d578353f660018e5129c37370415f2b7321fd1d2a4`  
		Last Modified: Tue, 17 Mar 2020 23:38:51 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:alpine` - linux; arm variant v6

```console
$ docker pull memcached@sha256:30a71800ac8815e2c8fb5ae9f56b45b61b7dcdd20a6eb28156c2d5b8b8fd8960
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4524432 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:524dd7062b34155e5603db803be952a17619b6f80c5f0f24d814d9c9db858f79`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Sat, 18 Jan 2020 01:53:16 GMT
ADD file:a1906f14a4e217a498b550f86a3d17c9012c02a6df0668043b63848c8fa44b9b in / 
# Sat, 18 Jan 2020 01:53:17 GMT
CMD ["/bin/sh"]
# Tue, 28 Jan 2020 00:52:27 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 28 Jan 2020 00:52:30 GMT
RUN apk add --no-cache cyrus-sasl-plain
# Tue, 17 Mar 2020 20:49:40 GMT
ENV MEMCACHED_VERSION=1.6.1
# Tue, 17 Mar 2020 20:49:41 GMT
ENV MEMCACHED_SHA1=6e337924dbf953bfabda512405d710d9757c97c1
# Tue, 17 Mar 2020 20:58:42 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		dpkg-dev dpkg 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		tar 		wget 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& make test 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 17 Mar 2020 20:58:43 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 17 Mar 2020 20:58:44 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 17 Mar 2020 20:58:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 17 Mar 2020 20:58:46 GMT
USER memcache
# Tue, 17 Mar 2020 20:58:46 GMT
EXPOSE 11211
# Tue, 17 Mar 2020 20:58:47 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:832e07764099264ef96e50a1e5e41c52d6b0809bd054e29508a6878aa59d156d`  
		Last Modified: Sat, 18 Jan 2020 01:53:52 GMT  
		Size: 2.6 MB (2617562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33c4279c48d90e0c3053099bb9ca915b67b4f057fdc1bfa737cdeff49f7fd3d4`  
		Last Modified: Tue, 28 Jan 2020 01:18:15 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d8eff54bf4684589855264a1239e93563b4da49264da619e3745d2446d2352f`  
		Last Modified: Tue, 28 Jan 2020 01:18:15 GMT  
		Size: 14.7 KB (14697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59e0525cb705a9cc4f63d347edc4befb0167ab3f726bfc56a2a2e9bc76b3c47d`  
		Last Modified: Tue, 17 Mar 2020 20:59:06 GMT  
		Size: 1.9 MB (1890509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c998ca8223a1d93ef5ea43ed575ae519454345d08422b171290c857d54b36ba9`  
		Last Modified: Tue, 17 Mar 2020 20:59:06 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbffc49509b88a96f211604a297cb07aa103f033cb1b53a5dc6b2ce8681abef0`  
		Last Modified: Tue, 17 Mar 2020 20:59:06 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:alpine` - linux; arm variant v7

```console
$ docker pull memcached@sha256:0bbd37ffdb170b94768803271712307a679ea3c2defe7fb0152090cec6ba4633
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4180800 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d9bb126ecd328f50fa969d980bead57d7b0ae41d51d35adfe2905e5b88cef512`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Sat, 18 Jan 2020 02:03:19 GMT
ADD file:4c815f4461ff3b8d481f43d84eb2548cb1adbb3015d370cab86dd7f4d3d94279 in / 
# Sat, 18 Jan 2020 02:03:22 GMT
CMD ["/bin/sh"]
# Tue, 28 Jan 2020 01:30:43 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 28 Jan 2020 01:30:55 GMT
RUN apk add --no-cache cyrus-sasl-plain
# Tue, 17 Mar 2020 22:52:32 GMT
ENV MEMCACHED_VERSION=1.6.1
# Tue, 17 Mar 2020 22:52:34 GMT
ENV MEMCACHED_SHA1=6e337924dbf953bfabda512405d710d9757c97c1
# Wed, 18 Mar 2020 01:16:18 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		dpkg-dev dpkg 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		tar 		wget 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& make test 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Wed, 18 Mar 2020 01:16:21 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 18 Mar 2020 01:16:32 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 18 Mar 2020 01:16:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 18 Mar 2020 01:16:36 GMT
USER memcache
# Wed, 18 Mar 2020 01:16:37 GMT
EXPOSE 11211
# Wed, 18 Mar 2020 01:16:39 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:3a2c5e3c37b2e3d749405512ef3793aa45a2f5c11615d9e9efa80179262cdf27`  
		Last Modified: Sat, 18 Jan 2020 02:04:05 GMT  
		Size: 2.4 MB (2419554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aa3e71e259912bc94119737267a874d423f639be13083765352c8d6f2fe2a6b`  
		Last Modified: Tue, 28 Jan 2020 12:23:43 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b9e1375e31fb539b7ca784d44d0cc4c37ac2e6f8239f4295213ca9500ccfcaa`  
		Last Modified: Tue, 28 Jan 2020 12:23:46 GMT  
		Size: 13.6 KB (13639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4efe2f16f62c2c6353e05ff8636454d71b14c132b3c3da88fc57f736b809dd2`  
		Last Modified: Wed, 18 Mar 2020 01:16:57 GMT  
		Size: 1.7 MB (1745940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6b847bebc1791a57ece10d729f50a457f4d3662fc77578ea1d9d9558919ee18`  
		Last Modified: Wed, 18 Mar 2020 01:17:01 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4c1bcfe68d4e7de06a63bb805865b81e7a0f434b774c0536c56b7b48ba5b2a3`  
		Last Modified: Wed, 18 Mar 2020 01:17:01 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:alpine` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:928c28f46dfe5dbcbceaa280f3e987bbad267d132d5fc5c1f952e7c935ca100b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4681073 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:668fc1e0a18d8c0a919cf8554bca06abaafcd581a191acae2a217c7687e03646`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Sat, 18 Jan 2020 01:39:43 GMT
ADD file:4109fa86dd80850e84c689ff9e6a3243e30ab1bbcc00c765969b3011bfbb43e1 in / 
# Sat, 18 Jan 2020 01:39:43 GMT
CMD ["/bin/sh"]
# Tue, 28 Jan 2020 00:53:38 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 28 Jan 2020 00:53:41 GMT
RUN apk add --no-cache cyrus-sasl-plain
# Tue, 17 Mar 2020 20:50:40 GMT
ENV MEMCACHED_VERSION=1.6.1
# Tue, 17 Mar 2020 20:50:41 GMT
ENV MEMCACHED_SHA1=6e337924dbf953bfabda512405d710d9757c97c1
# Tue, 17 Mar 2020 20:59:29 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		dpkg-dev dpkg 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		tar 		wget 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& make test 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 17 Mar 2020 20:59:30 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 17 Mar 2020 20:59:32 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 17 Mar 2020 20:59:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 17 Mar 2020 20:59:34 GMT
USER memcache
# Tue, 17 Mar 2020 20:59:35 GMT
EXPOSE 11211
# Tue, 17 Mar 2020 20:59:36 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:8fa90b21c985a6fcfff966bdfbde81cdd088de0aa8af38110057f6ac408f4408`  
		Last Modified: Sat, 18 Jan 2020 01:40:23 GMT  
		Size: 2.7 MB (2723075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cd06d9fb7c7820b59243e32290da8b6bc1e1719c0e1288f468936fa95091ff8`  
		Last Modified: Tue, 28 Jan 2020 01:11:01 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35ab3f89cfc542b0a3b8755ffd6bca6897778e9a3814c52589d388834b7156f2`  
		Last Modified: Tue, 28 Jan 2020 01:11:01 GMT  
		Size: 15.5 KB (15491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e7ea0f6e1e34d5cc2bcb05961ac73b83d75bc11a8bc2094d4bad1b2f127e437`  
		Last Modified: Tue, 17 Mar 2020 21:00:05 GMT  
		Size: 1.9 MB (1940839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43b9cee046785a0858fce8529dc10cb2203f0e2ab396231dda5cebfb18d94f78`  
		Last Modified: Tue, 17 Mar 2020 21:00:05 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8012377072c15ce103f473483c97b8e2324313c4b90d12d8d429c92a565976bf`  
		Last Modified: Tue, 17 Mar 2020 21:00:04 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:alpine` - linux; 386

```console
$ docker pull memcached@sha256:26e8ae37960af95ccb2d90e17e674c0c9a4df70535a4c33369813cd4252dc288
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.8 MB (4843276 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f9f4bc9657493d8c477aa7737dfba44f8aa7ec9daa2efe557e6e139e99b2fb81`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Sat, 18 Jan 2020 01:38:44 GMT
ADD file:381b617b92fe699ad4ef4f30e0d9599f89e43e252883348c420ebe2a0cccbd63 in / 
# Sat, 18 Jan 2020 01:38:45 GMT
CMD ["/bin/sh"]
# Tue, 28 Jan 2020 00:48:42 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 28 Jan 2020 00:48:43 GMT
RUN apk add --no-cache cyrus-sasl-plain
# Tue, 17 Mar 2020 22:05:51 GMT
ENV MEMCACHED_VERSION=1.6.1
# Tue, 17 Mar 2020 22:05:51 GMT
ENV MEMCACHED_SHA1=6e337924dbf953bfabda512405d710d9757c97c1
# Tue, 17 Mar 2020 22:14:29 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		dpkg-dev dpkg 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		tar 		wget 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& make test 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 17 Mar 2020 22:14:30 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 17 Mar 2020 22:14:30 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 17 Mar 2020 22:14:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 17 Mar 2020 22:14:31 GMT
USER memcache
# Tue, 17 Mar 2020 22:14:31 GMT
EXPOSE 11211
# Tue, 17 Mar 2020 22:14:31 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:f024b1263dc58db07a458b73ae1a2dca02ca55bef1ccd1fa3fd50656551fadf2`  
		Last Modified: Sat, 18 Jan 2020 01:39:18 GMT  
		Size: 2.8 MB (2806560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:431aabc4c24cdeaae3c25e5699ac6e79b8fb26d6b3bca55a800adfe777501e4e`  
		Last Modified: Tue, 28 Jan 2020 00:56:57 GMT  
		Size: 1.2 KB (1230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3597117016445fddae7449ab0e8e29d459d0e7cda1b6e76e2e3645338df003b7`  
		Last Modified: Tue, 28 Jan 2020 00:56:57 GMT  
		Size: 16.2 KB (16154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1840db45b1a27f8b00fa66768a3a172aed97e40512f841b032af22220c74f38`  
		Last Modified: Tue, 17 Mar 2020 22:14:49 GMT  
		Size: 2.0 MB (2018927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f71f6c3b0eac6fd20b6005cc8c0fceb8b30093c22f4cd918e1bf7e846dca3278`  
		Last Modified: Tue, 17 Mar 2020 22:14:49 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d725c8ed1dbb90202f4b25f3deccb5bcaff15386dc30af32f3f3c9cbd038281f`  
		Last Modified: Tue, 17 Mar 2020 22:14:49 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:alpine` - linux; ppc64le

```console
$ docker pull memcached@sha256:97381f0b46139d6041860dce1d3f378bb7c1a46852f9dbd6d85964f266101a35
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.8 MB (4834234 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a7bf667b9acf3f4784fc4f22b12e5a488fa8f65ad7e7cc00233086e0661a920`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Sat, 18 Jan 2020 02:20:41 GMT
ADD file:32ddb3d5255071cca51573ceee2464dd5a87c8d1cce514ae965b6e824d9ef24b in / 
# Sat, 18 Jan 2020 02:20:45 GMT
CMD ["/bin/sh"]
# Tue, 28 Jan 2020 00:56:10 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 28 Jan 2020 00:56:17 GMT
RUN apk add --no-cache cyrus-sasl-plain
# Tue, 17 Mar 2020 22:18:07 GMT
ENV MEMCACHED_VERSION=1.6.1
# Tue, 17 Mar 2020 22:18:09 GMT
ENV MEMCACHED_SHA1=6e337924dbf953bfabda512405d710d9757c97c1
# Tue, 17 Mar 2020 22:26:36 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		dpkg-dev dpkg 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		tar 		wget 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& make test 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 17 Mar 2020 22:26:37 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 17 Mar 2020 22:26:44 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 17 Mar 2020 22:26:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 17 Mar 2020 22:26:48 GMT
USER memcache
# Tue, 17 Mar 2020 22:26:53 GMT
EXPOSE 11211
# Tue, 17 Mar 2020 22:26:55 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:cd95c8a93e39dcaa0634a65d5b86a88bcd5c3092adb1f96504a7030faa165123`  
		Last Modified: Sat, 18 Jan 2020 02:21:25 GMT  
		Size: 2.8 MB (2822125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cc791749867123bab1a791891ae28e057ee5304e839f0e30fb11c01e3b117c9`  
		Last Modified: Tue, 28 Jan 2020 01:04:59 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17e510e23cde584149c483ecd997b1f57d4bd61ccaf28adef58583ae25ad6d5a`  
		Last Modified: Tue, 28 Jan 2020 01:04:58 GMT  
		Size: 16.1 KB (16135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e5709f59fa1d0e31b6f80b187befa21232cb667ac0b780535c3d698343ac7de`  
		Last Modified: Tue, 17 Mar 2020 22:27:26 GMT  
		Size: 2.0 MB (1994308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47c95bf2e7da41d366113c4a2b0f6a2766e707b9f316dee2881660aa41e32946`  
		Last Modified: Tue, 17 Mar 2020 22:27:25 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc7129936aeed99915bf58fa5dda941352c516c1975bfd50e7f41019973aca2d`  
		Last Modified: Tue, 17 Mar 2020 22:27:26 GMT  
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

## `memcached:latest`

```console
$ docker pull memcached@sha256:4cf938dddf9daf5228194a84e27bba4f82a934fa8a2c7c57f0114a15aa1de834
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `memcached:latest` - linux; amd64

```console
$ docker pull memcached@sha256:f01d94f9c4adae3a566151be2b41e9e0ab5410ef3fcb4e69e92226173c7f7259
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.5 MB (30483498 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:20188fe150aa349793b646f31dde86a97c2a60989b76bf01df11ec97e79f6a3f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 26 Feb 2020 00:37:39 GMT
ADD file:e5a364615e0f6961626089c7d658adbf8c8d95b3ae95a390a8bb33875317d434 in / 
# Wed, 26 Feb 2020 00:37:39 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 18:07:47 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 26 Feb 2020 18:07:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Mar 2020 23:22:04 GMT
ENV MEMCACHED_VERSION=1.6.1
# Tue, 17 Mar 2020 23:22:04 GMT
ENV MEMCACHED_SHA1=6e337924dbf953bfabda512405d710d9757c97c1
# Tue, 17 Mar 2020 23:30:13 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 17 Mar 2020 23:30:13 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 17 Mar 2020 23:30:14 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 17 Mar 2020 23:30:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 17 Mar 2020 23:30:14 GMT
USER memcache
# Tue, 17 Mar 2020 23:30:14 GMT
EXPOSE 11211
# Tue, 17 Mar 2020 23:30:14 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:68ced04f60ab5c7a5f1d0b0b4e7572c5a4c8cce44866513d30d9df1a15277d6b`  
		Last Modified: Wed, 26 Feb 2020 00:44:23 GMT  
		Size: 27.1 MB (27091819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7233c6ae94c59c690ba7007d1f0e360f97b515b3df0a5adc0a8e0c71e48dc836`  
		Last Modified: Wed, 26 Feb 2020 18:16:20 GMT  
		Size: 5.0 KB (4980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3945a4bf251bce21f9517716e4ed007325a8e8b279e52a09bc15fffa2f65b16d`  
		Last Modified: Wed, 26 Feb 2020 18:16:20 GMT  
		Size: 2.2 MB (2196514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9e46f4b34ecc2434e857dccae8dcefac20010d02aa70739107749e36164a43f`  
		Last Modified: Tue, 17 Mar 2020 23:38:46 GMT  
		Size: 1.2 MB (1189776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca1999a38cda2f5a4349e8b795ff37d1d1ba865a56a18defdaffac68af7800ce`  
		Last Modified: Tue, 17 Mar 2020 23:38:45 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4f797df323b4285de392809bad17d92950319a7753be796ab8b1a86d1666a85`  
		Last Modified: Tue, 17 Mar 2020 23:38:46 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:latest` - linux; arm variant v5

```console
$ docker pull memcached@sha256:d32bdb11fd734410cd1be1ae96fa977048cd809329b1a9cae28f4ec2f8b8fb8c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.9 MB (27888005 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1aec9eb200e1be46e4a6da6e72866613bd30e78e8865abd3dfdcb42b7877cca2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 26 Feb 2020 00:47:49 GMT
ADD file:745d3236976c8213b805ca6d14f150561816cd2eeec5aa7e1aaea44d9d5675e9 in / 
# Wed, 26 Feb 2020 00:47:53 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 01:21:35 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 26 Feb 2020 01:23:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Mar 2020 20:48:50 GMT
ENV MEMCACHED_VERSION=1.6.1
# Tue, 17 Mar 2020 20:48:52 GMT
ENV MEMCACHED_SHA1=6e337924dbf953bfabda512405d710d9757c97c1
# Tue, 17 Mar 2020 22:19:10 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 17 Mar 2020 22:19:13 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 17 Mar 2020 22:19:24 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 17 Mar 2020 22:19:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 17 Mar 2020 22:19:28 GMT
USER memcache
# Tue, 17 Mar 2020 22:19:29 GMT
EXPOSE 11211
# Tue, 17 Mar 2020 22:19:31 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:d9f9009f908455fa93c5b3e0d3230df44ea75299b2de375ab35b74193f679076`  
		Last Modified: Wed, 26 Feb 2020 00:59:18 GMT  
		Size: 24.8 MB (24830277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f028832400faf7f954f74987eff7a1e300690055f9df70085c778e354351f5d8`  
		Last Modified: Tue, 10 Mar 2020 13:06:25 GMT  
		Size: 4.9 KB (4895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dee056e35538c22bed8fa9de89eaa5b3ce1bfbce6a93be0b7ce527c378f23cf4`  
		Last Modified: Tue, 10 Mar 2020 13:06:33 GMT  
		Size: 1.9 MB (1896817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4def82d8eadc3db4d32a027dc0072359c4a3133a6bfca570381eed5e782302be`  
		Last Modified: Tue, 17 Mar 2020 22:19:53 GMT  
		Size: 1.2 MB (1155608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82fdc512c93448bbc2be492053f7303bef1efa0a68d7f8f5bbaa64ce758b250e`  
		Last Modified: Tue, 17 Mar 2020 22:19:56 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8003ad16648f331b96907ecf19d95da34b2b68aedf312ca29f1fc6e34ede22ab`  
		Last Modified: Tue, 17 Mar 2020 22:20:07 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:latest` - linux; arm variant v7

```console
$ docker pull memcached@sha256:cdf939e755f1f26e266767e417109b3ba044b51d444eff026e83bd1c7195fa9a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.6 MB (25644199 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b99a8df834c831b0c96ac194f07f1df3b4b1b22ac94731bc8ddd6f4f1df4419b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 26 Feb 2020 00:52:11 GMT
ADD file:2488038744e2e15217e67dd7f4bec5dcc7e9abe8a1010fe720a5ba7cbe7ab0eb in / 
# Wed, 26 Feb 2020 00:52:13 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 03:03:14 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 26 Feb 2020 03:05:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Mar 2020 22:23:13 GMT
ENV MEMCACHED_VERSION=1.6.1
# Tue, 17 Mar 2020 22:23:15 GMT
ENV MEMCACHED_SHA1=6e337924dbf953bfabda512405d710d9757c97c1
# Tue, 17 Mar 2020 22:51:58 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 17 Mar 2020 22:52:01 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 17 Mar 2020 22:52:11 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 17 Mar 2020 22:52:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 17 Mar 2020 22:52:15 GMT
USER memcache
# Tue, 17 Mar 2020 22:52:17 GMT
EXPOSE 11211
# Tue, 17 Mar 2020 22:52:19 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:fff3167bf8c79dc08baf67eb607823aadcbee2033f9620cc502e2c49423f605b`  
		Last Modified: Wed, 26 Feb 2020 01:07:32 GMT  
		Size: 22.7 MB (22699783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd762b0d48bc41e6bdfdb354ae48b55c2cbe60e2a0ad9cd60a9396304fb48660`  
		Last Modified: Wed, 26 Feb 2020 03:35:50 GMT  
		Size: 4.9 KB (4896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34dccc10f85111d1e9ad7f9118fc95ec338f9510a4fb1d7d847c500212185bf7`  
		Last Modified: Wed, 26 Feb 2020 03:35:57 GMT  
		Size: 1.8 MB (1811579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1aba4da49d87f5f9ee5f89839430139620889df5129d8f26fb948dd6e0738e1`  
		Last Modified: Wed, 18 Mar 2020 00:18:02 GMT  
		Size: 1.1 MB (1127532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:756d789cadf0cc90e8d82cad7000c52c7ad4c5d7984984c58b274a318c70c47c`  
		Last Modified: Wed, 18 Mar 2020 00:18:06 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d3d88a2570cc19347b319b789f0a3aafc02b99ac6c369e1343ba2315994bdb1`  
		Last Modified: Wed, 18 Mar 2020 00:18:17 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:latest` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:89a48b7232e353e9d13fc62962805abcd59e6f69bfd363c03b0b47c0fba0534a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.1 MB (29091968 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a3d7d5d254344a16e0d4d3a008c5108f77c7e872f7f7649fa3ac50ce1aad6ed1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 26 Feb 2020 00:46:51 GMT
ADD file:a93818b0ffcb2823807811dffd78092a3e3f4981aabf48c3cb75f2fa319ac055 in / 
# Wed, 26 Feb 2020 00:46:55 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 13:34:13 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 26 Feb 2020 13:34:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Mar 2020 20:41:15 GMT
ENV MEMCACHED_VERSION=1.6.1
# Tue, 17 Mar 2020 20:41:16 GMT
ENV MEMCACHED_SHA1=6e337924dbf953bfabda512405d710d9757c97c1
# Tue, 17 Mar 2020 20:50:18 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 17 Mar 2020 20:50:18 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 17 Mar 2020 20:50:20 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 17 Mar 2020 20:50:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 17 Mar 2020 20:50:21 GMT
USER memcache
# Tue, 17 Mar 2020 20:50:22 GMT
EXPOSE 11211
# Tue, 17 Mar 2020 20:50:22 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:f338bc35613f66cfaad272234de7b77a91d6c5422855bf6239f2b0ff9d73f0a4`  
		Last Modified: Wed, 26 Feb 2020 00:56:15 GMT  
		Size: 25.9 MB (25851563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4d7ac360be705ceb72083cd1a2c07b2fd7f572f0cd8de06e6733c8f217739a2`  
		Last Modified: Wed, 26 Feb 2020 14:00:56 GMT  
		Size: 5.0 KB (5029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bd27757fe5a945d701f8f5bd7534c41588270d8f2b934ca8085e0a649cbbf91`  
		Last Modified: Wed, 26 Feb 2020 14:00:56 GMT  
		Size: 2.1 MB (2074945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc7a620a01855a969584241d573d1e6acf55dee0e7e6c4f8d4c821b6b0064637`  
		Last Modified: Tue, 17 Mar 2020 20:59:55 GMT  
		Size: 1.2 MB (1160025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04bcc8eff174cea809be4c1a00052dce74463a60ea51cfb0c0da09ec1e0d8b42`  
		Last Modified: Tue, 17 Mar 2020 20:59:55 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15d59c8d4a0e2a02d465e919de1d0adb45841bbbeb21e78c588a3251cb9f2740`  
		Last Modified: Tue, 17 Mar 2020 20:59:55 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:latest` - linux; 386

```console
$ docker pull memcached@sha256:c34541b96410e9129064d823a4e89051fd9001f132c51841ca9d6f2fee21078c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.2 MB (31155198 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c89fc4282ec39b4634a263a8481002f3d90d3be4ece62cc10f9cf40d7608f85`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 26 Feb 2020 00:32:17 GMT
ADD file:08977fa54555a1ed2ae44a3aec04df157092a6c1c1b70ce0407cc2dc2f8bcd76 in / 
# Wed, 26 Feb 2020 00:32:17 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 10:57:50 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 26 Feb 2020 10:57:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Mar 2020 21:56:16 GMT
ENV MEMCACHED_VERSION=1.6.1
# Tue, 17 Mar 2020 21:56:17 GMT
ENV MEMCACHED_SHA1=6e337924dbf953bfabda512405d710d9757c97c1
# Tue, 17 Mar 2020 22:05:32 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 17 Mar 2020 22:05:33 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 17 Mar 2020 22:05:34 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 17 Mar 2020 22:05:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 17 Mar 2020 22:05:35 GMT
USER memcache
# Tue, 17 Mar 2020 22:05:35 GMT
EXPOSE 11211
# Tue, 17 Mar 2020 22:05:35 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:1de10f1ae2a5bfd5f34f19421ebd282580e443321e4947cdf5f943875782b018`  
		Last Modified: Wed, 26 Feb 2020 00:38:34 GMT  
		Size: 27.7 MB (27747667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40f6886cf964eb4f4025c8157f9756ae21437cdf1a57f5fe279849787aff082b`  
		Last Modified: Wed, 26 Feb 2020 11:06:50 GMT  
		Size: 4.9 KB (4893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d843b4e4e2bb25c8a0fb82174c608d57f8eb0ac3e8f3773c31c988a34857030`  
		Last Modified: Wed, 26 Feb 2020 11:06:50 GMT  
		Size: 2.2 MB (2208102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28a0ed0844b264f9c1207229402186f1fff548292e028cb9a1c254402763364c`  
		Last Modified: Tue, 17 Mar 2020 22:14:44 GMT  
		Size: 1.2 MB (1194128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c2889f61fb8cb96b3ec44d3036bda0cef5e06e7703a4df8876adf9792462aa8`  
		Last Modified: Tue, 17 Mar 2020 22:14:44 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7d9bc4abf0879c8f9c4cb3d9d4551d03033f7e3356fd9df07c8c69ee60ff63f`  
		Last Modified: Tue, 17 Mar 2020 22:14:44 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:latest` - linux; ppc64le

```console
$ docker pull memcached@sha256:010267e365a1b82e10d694473d416094c5a196dc8d778a8c2d383ac2558c6a50
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.1 MB (34061620 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dbb12046217f66e43361864882561c2b935d472dc219f6d90d6824a6cab4cad1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 26 Feb 2020 01:31:23 GMT
ADD file:430f1f769b86c60db1b8d2f96ed26c24837b3ff5730264be42a9c0cd8e43df7f in / 
# Wed, 26 Feb 2020 01:31:29 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 08:58:42 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 26 Feb 2020 08:59:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Mar 2020 22:07:27 GMT
ENV MEMCACHED_VERSION=1.6.1
# Tue, 17 Mar 2020 22:07:29 GMT
ENV MEMCACHED_SHA1=6e337924dbf953bfabda512405d710d9757c97c1
# Tue, 17 Mar 2020 22:17:35 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 17 Mar 2020 22:17:37 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 17 Mar 2020 22:17:43 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 17 Mar 2020 22:17:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 17 Mar 2020 22:17:47 GMT
USER memcache
# Tue, 17 Mar 2020 22:17:49 GMT
EXPOSE 11211
# Tue, 17 Mar 2020 22:17:52 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:975241fcd2057cc8f4cb8f066d68ed18877152b88da11e682911ccc3bc3da7c4`  
		Last Modified: Wed, 26 Feb 2020 01:52:57 GMT  
		Size: 30.5 MB (30518427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c4567bf2efa314a53153932738e79b856d675d83e768d2e2ce3ab5b45930ace`  
		Last Modified: Wed, 26 Feb 2020 09:10:20 GMT  
		Size: 5.0 KB (4985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63966b4eb4cf356b52b220fc08251ec17ddb06f1425096935b9dbe79c39e5bb5`  
		Last Modified: Wed, 26 Feb 2020 09:10:20 GMT  
		Size: 2.3 MB (2322659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f210835730fc44353def79514fb093d60f6442f97c0fffaa7dc0962a6ba887a`  
		Last Modified: Tue, 17 Mar 2020 22:27:10 GMT  
		Size: 1.2 MB (1215142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fde09d96ef673b71efb6670819cea32e1454fe672a42f7377f396277e48c40b7`  
		Last Modified: Tue, 17 Mar 2020 22:27:09 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efca2b06ccc0d3c5720838c60727aad27be7400487ab096e48113b6a2be2e5ae`  
		Last Modified: Tue, 17 Mar 2020 22:27:09 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:latest` - linux; s390x

```console
$ docker pull memcached@sha256:057b9567b3c01a5b0dbf1c7dba5b89d88df721093c01da5c6a1425c1f8ad6265
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.7 MB (28694839 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe2378496a97259729a8423d4b14be0ea1db6e01b3f9aa9e34431ef824d655e6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Sat, 28 Dec 2019 04:42:03 GMT
ADD file:eec6c56f8680753860198c3af0d94aabb87018ca30f6f6e346621a6bffe0e4b8 in / 
# Sat, 28 Dec 2019 04:42:04 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 09:52:58 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Sat, 28 Dec 2019 09:53:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 09:53:02 GMT
ENV MEMCACHED_VERSION=1.5.20
# Sat, 28 Dec 2019 09:53:02 GMT
ENV MEMCACHED_SHA1=5d3b5af3ce0a1483d655017db7228bcaeff10d47
# Sat, 28 Dec 2019 09:57:41 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Sat, 28 Dec 2019 09:57:41 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Sat, 28 Dec 2019 09:57:42 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Sat, 28 Dec 2019 09:57:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 28 Dec 2019 09:57:42 GMT
USER memcache
# Sat, 28 Dec 2019 09:57:42 GMT
EXPOSE 11211
# Sat, 28 Dec 2019 09:57:42 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:f7542f43e95fb32a870ee38d7f0e7bb23267ac8dcf709e3944311b0a30d7a479`  
		Last Modified: Sat, 28 Dec 2019 04:45:08 GMT  
		Size: 25.7 MB (25705315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10233ccd3a1a569a8ec38365e560732bbd6adbbe1646b79cee3569d59f7cef73`  
		Last Modified: Sat, 28 Dec 2019 09:57:55 GMT  
		Size: 5.0 KB (5022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f3e3dfd06ace4d055f1539e38c0fb68e4d1866043a1ba372c8c2f0fec48315d`  
		Last Modified: Sat, 28 Dec 2019 09:57:55 GMT  
		Size: 1.9 MB (1885865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47cce4b30798653a4fcf3fd9160a90374e103d5c1e877e69645d033c0f916e67`  
		Last Modified: Sat, 28 Dec 2019 09:57:55 GMT  
		Size: 1.1 MB (1098229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:982ba8604e516e190f19469aa238d4197aa0000182cbc54d57345a029b765600`  
		Last Modified: Sat, 28 Dec 2019 09:57:55 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aabfe12e62b1d54d9dce449f2dc85f703ade5574f14eadfa54a601a86cc96e54`  
		Last Modified: Sat, 28 Dec 2019 09:57:55 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
