## `memcached:latest`

```console
$ docker pull memcached@sha256:b7d1f1fb739d0be8a0fda935f66c16482f1403f5c1fd10a2af2510f47527342d
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
$ docker pull memcached@sha256:f75b33dee0a094f0b21823ab09f9093420554fdf0cee8859a3416a4083148e1c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.0 MB (32954492 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fa6cf68061c21613f43882bc3e8e3791bea6c85fa0f5dcd1bf1b09f204704d08`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 26 Jan 2022 01:40:35 GMT
ADD file:90495c24c897ec47982e200f732f8be3109fcd791691ddffae0756898f91024f in / 
# Wed, 26 Jan 2022 01:40:36 GMT
CMD ["bash"]
# Thu, 27 Jan 2022 00:51:04 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Thu, 27 Jan 2022 00:51:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 27 Jan 2022 00:51:08 GMT
ENV MEMCACHED_VERSION=1.6.13
# Thu, 27 Jan 2022 00:51:08 GMT
ENV MEMCACHED_SHA1=b9da57ba63ba8de8a980fe0fe2fedc8d59e1dfe3
# Thu, 27 Jan 2022 00:55:12 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 27 Jan 2022 00:55:12 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 27 Jan 2022 00:55:13 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 27 Jan 2022 00:55:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 27 Jan 2022 00:55:13 GMT
USER memcache
# Thu, 27 Jan 2022 00:55:14 GMT
EXPOSE 11211
# Thu, 27 Jan 2022 00:55:14 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:5eb5b503b37671af16371272f9c5313a3e82f1d0756e14506704489ad9900803`  
		Last Modified: Wed, 26 Jan 2022 01:46:39 GMT  
		Size: 31.4 MB (31366257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:621eeff48eb485be4f7065c2f25d58c18b70c06bc66edc19124521f348574615`  
		Last Modified: Thu, 27 Jan 2022 00:55:49 GMT  
		Size: 5.0 KB (4984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:409a3a19cade4c90e13ae5af026e3a9bdf949b1581f9a07afba8252e310cb956`  
		Last Modified: Thu, 27 Jan 2022 00:55:49 GMT  
		Size: 328.0 KB (328047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47942dd2f3d022cbaaede8ed1b33b497cb6a5c5888e33024f726eca11d59655c`  
		Last Modified: Thu, 27 Jan 2022 00:55:49 GMT  
		Size: 1.3 MB (1254797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:566107c88b8565d26ad6c8ea4e5fcf68d871ccfca87e4fd225511e41bf798377`  
		Last Modified: Thu, 27 Jan 2022 00:55:49 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb36f55586ede012bc5ce758c321f3132c1f6465f24d5ae6e2463dd21b0d9d01`  
		Last Modified: Thu, 27 Jan 2022 00:55:49 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:latest` - linux; arm variant v5

```console
$ docker pull memcached@sha256:2dd9fd0d12a120a69d41187791c51b849c3ba4e10dd571962f49a3d0f5537eba
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.5 MB (30456983 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:51153e9eb2eaa79aa946649768b11b0b1d02a188e75c96c2354b26bc86fc62ed`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 26 Jan 2022 01:41:57 GMT
ADD file:4ccea3cb033595f7bd9896126e94a8a19199b987bedd87b3c0700d8b29baa1fb in / 
# Wed, 26 Jan 2022 01:41:58 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 14:00:44 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 26 Jan 2022 14:00:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 14:00:55 GMT
ENV MEMCACHED_VERSION=1.6.13
# Wed, 26 Jan 2022 14:00:55 GMT
ENV MEMCACHED_SHA1=b9da57ba63ba8de8a980fe0fe2fedc8d59e1dfe3
# Wed, 26 Jan 2022 14:05:27 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 26 Jan 2022 14:05:28 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 26 Jan 2022 14:05:30 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 26 Jan 2022 14:05:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Jan 2022 14:05:31 GMT
USER memcache
# Wed, 26 Jan 2022 14:05:31 GMT
EXPOSE 11211
# Wed, 26 Jan 2022 14:05:32 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:247ff78919074ec9db7cccd537dd6eb4d7e2788013b7ef07443e345d91c8a588`  
		Last Modified: Wed, 26 Jan 2022 01:57:36 GMT  
		Size: 28.9 MB (28909638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d649537bd44196deaa98c053b0373a1618e97147a3ac8766f25c9d200903485`  
		Last Modified: Wed, 26 Jan 2022 14:06:25 GMT  
		Size: 4.9 KB (4894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c8144a9e735d924ec1bf79c48e4c1f47a0b67c2b394b9fe4e1520f2cef8dd73`  
		Last Modified: Wed, 26 Jan 2022 14:06:25 GMT  
		Size: 316.6 KB (316587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de5c5d76cfc6046dc56bf9cb03efb68ab232b203f7fd09417840e8e9648a1a7d`  
		Last Modified: Wed, 26 Jan 2022 14:06:26 GMT  
		Size: 1.2 MB (1225456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c4cf3291b780e680963a0803f66a513290a08a26ecfabaaea4ab3b7f6277eab`  
		Last Modified: Wed, 26 Jan 2022 14:06:25 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:271787b627cceacf595b9a1a60dc0fb6f0d11293c646d4d858de8ac52962f35c`  
		Last Modified: Wed, 26 Jan 2022 14:06:25 GMT  
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
