<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `memcached`

-	[`memcached:1`](#memcached1)
-	[`memcached:1.6`](#memcached16)
-	[`memcached:1.6.3`](#memcached163)
-	[`memcached:1.6.3-alpine`](#memcached163-alpine)
-	[`memcached:1.6-alpine`](#memcached16-alpine)
-	[`memcached:1-alpine`](#memcached1-alpine)
-	[`memcached:alpine`](#memcachedalpine)
-	[`memcached:latest`](#memcachedlatest)

## `memcached:1`

```console
$ docker pull memcached@sha256:7d02e468382d4e2c54574f18088eb0127979fa135f6aa55f96e94185b7166215
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
$ docker pull memcached@sha256:6bdc214f60e191847cf0f57721aba4ba68cc3357eb38fc8ea31e935c350c5e0c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.5 MB (30485763 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ac3dd24663f48d13eca8fc54d99547759af3dace518eaff1dc413120737ece5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 31 Mar 2020 01:21:01 GMT
ADD file:d1f1b387a158136fb0f8096c8a8ecf5fc146be4e85c1c3c345d44c927692723a in / 
# Tue, 31 Mar 2020 01:21:01 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 13:20:36 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 31 Mar 2020 13:20:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Apr 2020 04:26:20 GMT
ENV MEMCACHED_VERSION=1.6.3
# Wed, 01 Apr 2020 04:26:20 GMT
ENV MEMCACHED_SHA1=bcd6d0c076ca2b62e9bd31f6669acc8563df7db1
# Wed, 01 Apr 2020 04:34:30 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 01 Apr 2020 04:34:30 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 01 Apr 2020 04:34:31 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 01 Apr 2020 04:34:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Apr 2020 04:34:31 GMT
USER memcache
# Wed, 01 Apr 2020 04:34:32 GMT
EXPOSE 11211
# Wed, 01 Apr 2020 04:34:32 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:c499e6d256d6d4a546f1c141e04b5b4951983ba7581e39deaf5cc595289ee70f`  
		Last Modified: Tue, 31 Mar 2020 01:26:37 GMT  
		Size: 27.1 MB (27091862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:512f277e1da84b0b9319530d40c48750bb22b13f4816d103040d20c0635c28be`  
		Last Modified: Tue, 31 Mar 2020 13:29:52 GMT  
		Size: 5.0 KB (4984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdda69e165e26c667ba223dc215274101c3c6e41db182bd651aadf5e5623fc35`  
		Last Modified: Tue, 31 Mar 2020 13:29:53 GMT  
		Size: 2.2 MB (2196476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43b37ee911063bfa8e0a60293b8ba301a22c3b29e26bf39c33f017e1b4bef28e`  
		Last Modified: Wed, 01 Apr 2020 04:43:03 GMT  
		Size: 1.2 MB (1192033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b83bd7ea262edefd8fa75ce5e40145b491e787de8d3806265e986a60cad606e0`  
		Last Modified: Wed, 01 Apr 2020 04:43:03 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc4fa7c552bc03701653c81434f6e3f7312745deb0c26e039e7565acca70ea54`  
		Last Modified: Wed, 01 Apr 2020 04:43:03 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1` - linux; arm variant v5

```console
$ docker pull memcached@sha256:aa492daa963294573d6319a6a19d392cce213240b81078dba65869e538611c97
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.9 MB (27889314 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c0ec6623b84d3061e2fa7dab933f5e39cc8c9b170bbf6fd5ce0b4baf35341c30`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 31 Mar 2020 01:24:54 GMT
ADD file:e08ed9e60228d351de400af5746474777a562d99f17e0cb1ce3e3d352e9ec751 in / 
# Tue, 31 Mar 2020 01:24:56 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 01:54:28 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 31 Mar 2020 01:55:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Mar 2020 19:48:28 GMT
ENV MEMCACHED_VERSION=1.6.3
# Tue, 31 Mar 2020 19:48:30 GMT
ENV MEMCACHED_SHA1=bcd6d0c076ca2b62e9bd31f6669acc8563df7db1
# Tue, 31 Mar 2020 20:49:40 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 31 Mar 2020 20:49:43 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 31 Mar 2020 20:49:54 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 31 Mar 2020 20:49:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 31 Mar 2020 20:49:58 GMT
USER memcache
# Tue, 31 Mar 2020 20:50:00 GMT
EXPOSE 11211
# Tue, 31 Mar 2020 20:50:02 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:440df189aa3df85587f2d7d348500930481b3752dcb887d212de9b44b49076dd`  
		Last Modified: Tue, 31 Mar 2020 01:33:04 GMT  
		Size: 24.8 MB (24830324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bde8351817341fa2fec288d97635ede228892bbb58fc5c6ca54441acef6f0766`  
		Last Modified: Tue, 31 Mar 2020 03:24:42 GMT  
		Size: 4.9 KB (4896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b011e5f13bdf6608cafa62557b3c877e4794590eaadced0b8a49fe24a28d110`  
		Last Modified: Tue, 31 Mar 2020 03:24:44 GMT  
		Size: 1.9 MB (1896786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d15532e44d1b4cbd93a29d2f59e8d316aac3697819e686b863a04b7306f66e97`  
		Last Modified: Tue, 31 Mar 2020 20:50:23 GMT  
		Size: 1.2 MB (1156899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51aa0f21d752e0ddd5092569a00faade9a48585be4787ea0915d3bcd56ee1de5`  
		Last Modified: Tue, 31 Mar 2020 20:50:27 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e86f84b137f1eb137ff83d27d7cff6eee693a6dab12d7ce99ff0c2a77a49b6ae`  
		Last Modified: Tue, 31 Mar 2020 20:50:28 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1` - linux; arm variant v7

```console
$ docker pull memcached@sha256:d54eb37ba24eeb017adff9ad74f97c71f8232153c291be63893eb6ade8836656
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.6 MB (25646260 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0d8ee9533c9e5e31033a1bc594eeac7543678ca190a7b66d654a6b5385f8e5a7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 31 Mar 2020 01:48:12 GMT
ADD file:8c3ed0df404a6bcaf7583e71796cb4c1f40e87288953a21d4ee5946079c3274f in / 
# Tue, 31 Mar 2020 01:48:13 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 03:27:08 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 31 Mar 2020 03:28:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Mar 2020 20:51:09 GMT
ENV MEMCACHED_VERSION=1.6.3
# Tue, 31 Mar 2020 20:51:11 GMT
ENV MEMCACHED_SHA1=bcd6d0c076ca2b62e9bd31f6669acc8563df7db1
# Tue, 31 Mar 2020 21:21:03 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 31 Mar 2020 21:21:07 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 31 Mar 2020 21:21:18 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 31 Mar 2020 21:21:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 31 Mar 2020 21:21:22 GMT
USER memcache
# Tue, 31 Mar 2020 21:21:24 GMT
EXPOSE 11211
# Tue, 31 Mar 2020 21:21:26 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:98098fa10651fdba12c848231b7428536a120e17637f1f9e0d25c63880483fcc`  
		Last Modified: Tue, 31 Mar 2020 01:56:24 GMT  
		Size: 22.7 MB (22699731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a7a42e48b851419bcd11506631a8d336fb394d979dcea8feb4830f38ba7cfd7`  
		Last Modified: Tue, 31 Mar 2020 04:39:27 GMT  
		Size: 4.9 KB (4899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc96c4fde110b7a8691d85cf0523cd326fbfd1bcbf928719f6173cd292c91305`  
		Last Modified: Tue, 31 Mar 2020 04:39:35 GMT  
		Size: 1.8 MB (1811551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2a043ecd402e02473caef2834dd90c40a3a16ee899cb87574bf7fb8b1183adb`  
		Last Modified: Tue, 31 Mar 2020 23:12:26 GMT  
		Size: 1.1 MB (1129671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6b3946960ee59ded096d4489e81d9cd3af3506ce6f99c79f38648217430a2f0`  
		Last Modified: Tue, 31 Mar 2020 23:12:24 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34b5c1dda6f0d125b29798f04589e1f46502983dbe8f4cf5763a2a2592148191`  
		Last Modified: Tue, 31 Mar 2020 23:12:30 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:056b511f1e97a6619c24aadc781560db65e25abc0c3a98bbe25b52d81b24e78c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.1 MB (29094504 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:142fbd99d85857a0807b95f6c5621c5006b38c522d78f4f8e088fdd6a4061db8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 31 Mar 2020 02:05:33 GMT
ADD file:47ab456123ae97a527249191ff2bc0014e7ef0ae186aec91bf6a63eb077ecb91 in / 
# Tue, 31 Mar 2020 02:05:35 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 08:39:07 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 31 Mar 2020 08:39:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Apr 2020 04:44:54 GMT
ENV MEMCACHED_VERSION=1.6.3
# Wed, 01 Apr 2020 04:44:55 GMT
ENV MEMCACHED_SHA1=bcd6d0c076ca2b62e9bd31f6669acc8563df7db1
# Wed, 01 Apr 2020 04:54:03 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 01 Apr 2020 04:54:05 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 01 Apr 2020 04:54:07 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 01 Apr 2020 04:54:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Apr 2020 04:54:08 GMT
USER memcache
# Wed, 01 Apr 2020 04:54:08 GMT
EXPOSE 11211
# Wed, 01 Apr 2020 04:54:09 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:a6c32b8bc1ce2b374630673ded1d5ef5a98936d045bf0632fcf599dc2229d493`  
		Last Modified: Tue, 31 Mar 2020 02:12:15 GMT  
		Size: 25.9 MB (25851645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72560398e0dc8991a53cd07c580b14e3c2024d7af30d2dfe8428d913006af5a9`  
		Last Modified: Tue, 31 Mar 2020 08:48:55 GMT  
		Size: 5.0 KB (5028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4febdbdc3565b2d569ed0a6885c548a5755cd9a2b52c21b351d254c83e6fff7`  
		Last Modified: Tue, 31 Mar 2020 08:48:55 GMT  
		Size: 2.1 MB (2074952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b1797ec4dd007a4f822abca922aa457a793f2ba04b4481e6c1f0de7e34b32d8`  
		Last Modified: Wed, 01 Apr 2020 05:12:38 GMT  
		Size: 1.2 MB (1162471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b9601a34125cd3cfe733ea2ce11005afc0ec6f02bd14b34d5d5ce92a9dadb1c`  
		Last Modified: Wed, 01 Apr 2020 05:12:39 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:703422421b84c80f0ed9b79b040ba35dbf37e06c80b5e9681455202c1b2091f6`  
		Last Modified: Wed, 01 Apr 2020 05:12:38 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1` - linux; 386

```console
$ docker pull memcached@sha256:45e70e58745f9b65a1fdbea626d26be12194087fa3f2ebc06647d23dd8ff4dd3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.2 MB (31156562 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7371335c883334e01e87c4a4b5cf189b8b2876ff43cd38604954befcf0afc780`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 31 Mar 2020 00:39:42 GMT
ADD file:a453117866661af4ddfa21203d65ce6661efeaeca2a1704e09747c83b4c58e47 in / 
# Tue, 31 Mar 2020 00:39:42 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 11:45:29 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 31 Mar 2020 11:45:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Apr 2020 00:36:05 GMT
ENV MEMCACHED_VERSION=1.6.3
# Wed, 01 Apr 2020 00:36:06 GMT
ENV MEMCACHED_SHA1=bcd6d0c076ca2b62e9bd31f6669acc8563df7db1
# Wed, 01 Apr 2020 00:45:06 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 01 Apr 2020 00:45:06 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 01 Apr 2020 00:45:08 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 01 Apr 2020 00:45:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Apr 2020 00:45:09 GMT
USER memcache
# Wed, 01 Apr 2020 00:45:09 GMT
EXPOSE 11211
# Wed, 01 Apr 2020 00:45:10 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:2314106a15e49c7908bebb2c697dcaf3d6a1626b70fe72bc0c0cb71eb216ddc3`  
		Last Modified: Tue, 31 Mar 2020 00:45:31 GMT  
		Size: 27.7 MB (27747648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3bafab0976764495dda52d0c16addb4770d62d8f9de55728b752ff3448f2292`  
		Last Modified: Tue, 31 Mar 2020 11:55:29 GMT  
		Size: 4.9 KB (4899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8307e5e61ebc9ed2430c9e45ba3437aa1deebed0882ce15c36616e0debf28b36`  
		Last Modified: Tue, 31 Mar 2020 11:55:29 GMT  
		Size: 2.2 MB (2208079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2346314e755e47f2a21140be69437185fef4416c21871e9bea2504e4011aa31c`  
		Last Modified: Wed, 01 Apr 2020 00:54:20 GMT  
		Size: 1.2 MB (1195528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04f73e333f816b2d2fa26694d21c4c50e393e11ecbe6c172966071f7a5c60a31`  
		Last Modified: Wed, 01 Apr 2020 00:54:20 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:882932b666818b8fc239f2047d12a409ec5f211424e6321a671aabd98da708bc`  
		Last Modified: Wed, 01 Apr 2020 00:54:20 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1` - linux; ppc64le

```console
$ docker pull memcached@sha256:9d4d92103d08915f9f79003636917f96ee58591cf3fc4bf22c5331ee582ea6d1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.1 MB (34064010 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:296aceabbfb0b475275d0104ab416027cdcb9ac9c53140cb7791a505e2a8ff70`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 31 Mar 2020 01:32:42 GMT
ADD file:36c02e92574faba45b64cfed78a0a0359d65ad175b17128bf554a2a5c0086ff5 in / 
# Tue, 31 Mar 2020 01:32:47 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 12:45:58 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 31 Mar 2020 12:46:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Apr 2020 05:38:36 GMT
ENV MEMCACHED_VERSION=1.6.3
# Wed, 01 Apr 2020 05:38:38 GMT
ENV MEMCACHED_SHA1=bcd6d0c076ca2b62e9bd31f6669acc8563df7db1
# Wed, 01 Apr 2020 05:48:45 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 01 Apr 2020 05:48:47 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 01 Apr 2020 05:48:55 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 01 Apr 2020 05:49:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Apr 2020 05:49:05 GMT
USER memcache
# Wed, 01 Apr 2020 05:49:09 GMT
EXPOSE 11211
# Wed, 01 Apr 2020 05:49:14 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:9df6bbae5eeb29e9aac2f39cff517c694cce60f01ee477abcdedcd8e8c01c38f`  
		Last Modified: Tue, 31 Mar 2020 01:45:59 GMT  
		Size: 30.5 MB (30518493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2786c1a6fbad6e8c56e4f7e33b4d41c64efd06c4cdb303a50c07ee1f4c5f7a69`  
		Last Modified: Tue, 31 Mar 2020 12:58:00 GMT  
		Size: 5.0 KB (4987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:722cfb50c03533f4b5c83c84a2f565dbcdbf63c01460ae91d35aafacd94454fe`  
		Last Modified: Tue, 31 Mar 2020 12:58:00 GMT  
		Size: 2.3 MB (2322647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7e848dce4e6fd08decef8fe4b047462a693bef7d0e19a1b08a71731d057769a`  
		Last Modified: Wed, 01 Apr 2020 05:58:55 GMT  
		Size: 1.2 MB (1217474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6b9f0c55a9cb31a1fe9245e8b6fd7289e71e07b1cde1a80fd6aa8636933e374`  
		Last Modified: Wed, 01 Apr 2020 05:58:54 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e3672877c4fc4ef3ec6151c6b363981966fa03e2cfbae0ba80f168670103a2a`  
		Last Modified: Wed, 01 Apr 2020 05:58:55 GMT  
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
$ docker pull memcached@sha256:24bafb41bd77e33e791c5154d157ff38af129d747264f84bdc11ea091fa63000
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
$ docker pull memcached@sha256:6bdc214f60e191847cf0f57721aba4ba68cc3357eb38fc8ea31e935c350c5e0c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.5 MB (30485763 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ac3dd24663f48d13eca8fc54d99547759af3dace518eaff1dc413120737ece5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 31 Mar 2020 01:21:01 GMT
ADD file:d1f1b387a158136fb0f8096c8a8ecf5fc146be4e85c1c3c345d44c927692723a in / 
# Tue, 31 Mar 2020 01:21:01 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 13:20:36 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 31 Mar 2020 13:20:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Apr 2020 04:26:20 GMT
ENV MEMCACHED_VERSION=1.6.3
# Wed, 01 Apr 2020 04:26:20 GMT
ENV MEMCACHED_SHA1=bcd6d0c076ca2b62e9bd31f6669acc8563df7db1
# Wed, 01 Apr 2020 04:34:30 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 01 Apr 2020 04:34:30 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 01 Apr 2020 04:34:31 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 01 Apr 2020 04:34:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Apr 2020 04:34:31 GMT
USER memcache
# Wed, 01 Apr 2020 04:34:32 GMT
EXPOSE 11211
# Wed, 01 Apr 2020 04:34:32 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:c499e6d256d6d4a546f1c141e04b5b4951983ba7581e39deaf5cc595289ee70f`  
		Last Modified: Tue, 31 Mar 2020 01:26:37 GMT  
		Size: 27.1 MB (27091862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:512f277e1da84b0b9319530d40c48750bb22b13f4816d103040d20c0635c28be`  
		Last Modified: Tue, 31 Mar 2020 13:29:52 GMT  
		Size: 5.0 KB (4984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdda69e165e26c667ba223dc215274101c3c6e41db182bd651aadf5e5623fc35`  
		Last Modified: Tue, 31 Mar 2020 13:29:53 GMT  
		Size: 2.2 MB (2196476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43b37ee911063bfa8e0a60293b8ba301a22c3b29e26bf39c33f017e1b4bef28e`  
		Last Modified: Wed, 01 Apr 2020 04:43:03 GMT  
		Size: 1.2 MB (1192033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b83bd7ea262edefd8fa75ce5e40145b491e787de8d3806265e986a60cad606e0`  
		Last Modified: Wed, 01 Apr 2020 04:43:03 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc4fa7c552bc03701653c81434f6e3f7312745deb0c26e039e7565acca70ea54`  
		Last Modified: Wed, 01 Apr 2020 04:43:03 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6` - linux; arm variant v5

```console
$ docker pull memcached@sha256:aa492daa963294573d6319a6a19d392cce213240b81078dba65869e538611c97
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.9 MB (27889314 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c0ec6623b84d3061e2fa7dab933f5e39cc8c9b170bbf6fd5ce0b4baf35341c30`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 31 Mar 2020 01:24:54 GMT
ADD file:e08ed9e60228d351de400af5746474777a562d99f17e0cb1ce3e3d352e9ec751 in / 
# Tue, 31 Mar 2020 01:24:56 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 01:54:28 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 31 Mar 2020 01:55:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Mar 2020 19:48:28 GMT
ENV MEMCACHED_VERSION=1.6.3
# Tue, 31 Mar 2020 19:48:30 GMT
ENV MEMCACHED_SHA1=bcd6d0c076ca2b62e9bd31f6669acc8563df7db1
# Tue, 31 Mar 2020 20:49:40 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 31 Mar 2020 20:49:43 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 31 Mar 2020 20:49:54 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 31 Mar 2020 20:49:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 31 Mar 2020 20:49:58 GMT
USER memcache
# Tue, 31 Mar 2020 20:50:00 GMT
EXPOSE 11211
# Tue, 31 Mar 2020 20:50:02 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:440df189aa3df85587f2d7d348500930481b3752dcb887d212de9b44b49076dd`  
		Last Modified: Tue, 31 Mar 2020 01:33:04 GMT  
		Size: 24.8 MB (24830324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bde8351817341fa2fec288d97635ede228892bbb58fc5c6ca54441acef6f0766`  
		Last Modified: Tue, 31 Mar 2020 03:24:42 GMT  
		Size: 4.9 KB (4896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b011e5f13bdf6608cafa62557b3c877e4794590eaadced0b8a49fe24a28d110`  
		Last Modified: Tue, 31 Mar 2020 03:24:44 GMT  
		Size: 1.9 MB (1896786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d15532e44d1b4cbd93a29d2f59e8d316aac3697819e686b863a04b7306f66e97`  
		Last Modified: Tue, 31 Mar 2020 20:50:23 GMT  
		Size: 1.2 MB (1156899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51aa0f21d752e0ddd5092569a00faade9a48585be4787ea0915d3bcd56ee1de5`  
		Last Modified: Tue, 31 Mar 2020 20:50:27 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e86f84b137f1eb137ff83d27d7cff6eee693a6dab12d7ce99ff0c2a77a49b6ae`  
		Last Modified: Tue, 31 Mar 2020 20:50:28 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6` - linux; arm variant v7

```console
$ docker pull memcached@sha256:d54eb37ba24eeb017adff9ad74f97c71f8232153c291be63893eb6ade8836656
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.6 MB (25646260 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0d8ee9533c9e5e31033a1bc594eeac7543678ca190a7b66d654a6b5385f8e5a7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 31 Mar 2020 01:48:12 GMT
ADD file:8c3ed0df404a6bcaf7583e71796cb4c1f40e87288953a21d4ee5946079c3274f in / 
# Tue, 31 Mar 2020 01:48:13 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 03:27:08 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 31 Mar 2020 03:28:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Mar 2020 20:51:09 GMT
ENV MEMCACHED_VERSION=1.6.3
# Tue, 31 Mar 2020 20:51:11 GMT
ENV MEMCACHED_SHA1=bcd6d0c076ca2b62e9bd31f6669acc8563df7db1
# Tue, 31 Mar 2020 21:21:03 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 31 Mar 2020 21:21:07 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 31 Mar 2020 21:21:18 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 31 Mar 2020 21:21:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 31 Mar 2020 21:21:22 GMT
USER memcache
# Tue, 31 Mar 2020 21:21:24 GMT
EXPOSE 11211
# Tue, 31 Mar 2020 21:21:26 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:98098fa10651fdba12c848231b7428536a120e17637f1f9e0d25c63880483fcc`  
		Last Modified: Tue, 31 Mar 2020 01:56:24 GMT  
		Size: 22.7 MB (22699731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a7a42e48b851419bcd11506631a8d336fb394d979dcea8feb4830f38ba7cfd7`  
		Last Modified: Tue, 31 Mar 2020 04:39:27 GMT  
		Size: 4.9 KB (4899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc96c4fde110b7a8691d85cf0523cd326fbfd1bcbf928719f6173cd292c91305`  
		Last Modified: Tue, 31 Mar 2020 04:39:35 GMT  
		Size: 1.8 MB (1811551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2a043ecd402e02473caef2834dd90c40a3a16ee899cb87574bf7fb8b1183adb`  
		Last Modified: Tue, 31 Mar 2020 23:12:26 GMT  
		Size: 1.1 MB (1129671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6b3946960ee59ded096d4489e81d9cd3af3506ce6f99c79f38648217430a2f0`  
		Last Modified: Tue, 31 Mar 2020 23:12:24 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34b5c1dda6f0d125b29798f04589e1f46502983dbe8f4cf5763a2a2592148191`  
		Last Modified: Tue, 31 Mar 2020 23:12:30 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:056b511f1e97a6619c24aadc781560db65e25abc0c3a98bbe25b52d81b24e78c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.1 MB (29094504 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:142fbd99d85857a0807b95f6c5621c5006b38c522d78f4f8e088fdd6a4061db8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 31 Mar 2020 02:05:33 GMT
ADD file:47ab456123ae97a527249191ff2bc0014e7ef0ae186aec91bf6a63eb077ecb91 in / 
# Tue, 31 Mar 2020 02:05:35 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 08:39:07 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 31 Mar 2020 08:39:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Apr 2020 04:44:54 GMT
ENV MEMCACHED_VERSION=1.6.3
# Wed, 01 Apr 2020 04:44:55 GMT
ENV MEMCACHED_SHA1=bcd6d0c076ca2b62e9bd31f6669acc8563df7db1
# Wed, 01 Apr 2020 04:54:03 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 01 Apr 2020 04:54:05 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 01 Apr 2020 04:54:07 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 01 Apr 2020 04:54:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Apr 2020 04:54:08 GMT
USER memcache
# Wed, 01 Apr 2020 04:54:08 GMT
EXPOSE 11211
# Wed, 01 Apr 2020 04:54:09 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:a6c32b8bc1ce2b374630673ded1d5ef5a98936d045bf0632fcf599dc2229d493`  
		Last Modified: Tue, 31 Mar 2020 02:12:15 GMT  
		Size: 25.9 MB (25851645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72560398e0dc8991a53cd07c580b14e3c2024d7af30d2dfe8428d913006af5a9`  
		Last Modified: Tue, 31 Mar 2020 08:48:55 GMT  
		Size: 5.0 KB (5028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4febdbdc3565b2d569ed0a6885c548a5755cd9a2b52c21b351d254c83e6fff7`  
		Last Modified: Tue, 31 Mar 2020 08:48:55 GMT  
		Size: 2.1 MB (2074952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b1797ec4dd007a4f822abca922aa457a793f2ba04b4481e6c1f0de7e34b32d8`  
		Last Modified: Wed, 01 Apr 2020 05:12:38 GMT  
		Size: 1.2 MB (1162471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b9601a34125cd3cfe733ea2ce11005afc0ec6f02bd14b34d5d5ce92a9dadb1c`  
		Last Modified: Wed, 01 Apr 2020 05:12:39 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:703422421b84c80f0ed9b79b040ba35dbf37e06c80b5e9681455202c1b2091f6`  
		Last Modified: Wed, 01 Apr 2020 05:12:38 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6` - linux; 386

```console
$ docker pull memcached@sha256:45e70e58745f9b65a1fdbea626d26be12194087fa3f2ebc06647d23dd8ff4dd3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.2 MB (31156562 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7371335c883334e01e87c4a4b5cf189b8b2876ff43cd38604954befcf0afc780`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 31 Mar 2020 00:39:42 GMT
ADD file:a453117866661af4ddfa21203d65ce6661efeaeca2a1704e09747c83b4c58e47 in / 
# Tue, 31 Mar 2020 00:39:42 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 11:45:29 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 31 Mar 2020 11:45:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Apr 2020 00:36:05 GMT
ENV MEMCACHED_VERSION=1.6.3
# Wed, 01 Apr 2020 00:36:06 GMT
ENV MEMCACHED_SHA1=bcd6d0c076ca2b62e9bd31f6669acc8563df7db1
# Wed, 01 Apr 2020 00:45:06 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 01 Apr 2020 00:45:06 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 01 Apr 2020 00:45:08 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 01 Apr 2020 00:45:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Apr 2020 00:45:09 GMT
USER memcache
# Wed, 01 Apr 2020 00:45:09 GMT
EXPOSE 11211
# Wed, 01 Apr 2020 00:45:10 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:2314106a15e49c7908bebb2c697dcaf3d6a1626b70fe72bc0c0cb71eb216ddc3`  
		Last Modified: Tue, 31 Mar 2020 00:45:31 GMT  
		Size: 27.7 MB (27747648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3bafab0976764495dda52d0c16addb4770d62d8f9de55728b752ff3448f2292`  
		Last Modified: Tue, 31 Mar 2020 11:55:29 GMT  
		Size: 4.9 KB (4899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8307e5e61ebc9ed2430c9e45ba3437aa1deebed0882ce15c36616e0debf28b36`  
		Last Modified: Tue, 31 Mar 2020 11:55:29 GMT  
		Size: 2.2 MB (2208079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2346314e755e47f2a21140be69437185fef4416c21871e9bea2504e4011aa31c`  
		Last Modified: Wed, 01 Apr 2020 00:54:20 GMT  
		Size: 1.2 MB (1195528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04f73e333f816b2d2fa26694d21c4c50e393e11ecbe6c172966071f7a5c60a31`  
		Last Modified: Wed, 01 Apr 2020 00:54:20 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:882932b666818b8fc239f2047d12a409ec5f211424e6321a671aabd98da708bc`  
		Last Modified: Wed, 01 Apr 2020 00:54:20 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6` - linux; ppc64le

```console
$ docker pull memcached@sha256:9d4d92103d08915f9f79003636917f96ee58591cf3fc4bf22c5331ee582ea6d1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.1 MB (34064010 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:296aceabbfb0b475275d0104ab416027cdcb9ac9c53140cb7791a505e2a8ff70`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 31 Mar 2020 01:32:42 GMT
ADD file:36c02e92574faba45b64cfed78a0a0359d65ad175b17128bf554a2a5c0086ff5 in / 
# Tue, 31 Mar 2020 01:32:47 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 12:45:58 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 31 Mar 2020 12:46:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Apr 2020 05:38:36 GMT
ENV MEMCACHED_VERSION=1.6.3
# Wed, 01 Apr 2020 05:38:38 GMT
ENV MEMCACHED_SHA1=bcd6d0c076ca2b62e9bd31f6669acc8563df7db1
# Wed, 01 Apr 2020 05:48:45 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 01 Apr 2020 05:48:47 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 01 Apr 2020 05:48:55 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 01 Apr 2020 05:49:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Apr 2020 05:49:05 GMT
USER memcache
# Wed, 01 Apr 2020 05:49:09 GMT
EXPOSE 11211
# Wed, 01 Apr 2020 05:49:14 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:9df6bbae5eeb29e9aac2f39cff517c694cce60f01ee477abcdedcd8e8c01c38f`  
		Last Modified: Tue, 31 Mar 2020 01:45:59 GMT  
		Size: 30.5 MB (30518493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2786c1a6fbad6e8c56e4f7e33b4d41c64efd06c4cdb303a50c07ee1f4c5f7a69`  
		Last Modified: Tue, 31 Mar 2020 12:58:00 GMT  
		Size: 5.0 KB (4987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:722cfb50c03533f4b5c83c84a2f565dbcdbf63c01460ae91d35aafacd94454fe`  
		Last Modified: Tue, 31 Mar 2020 12:58:00 GMT  
		Size: 2.3 MB (2322647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7e848dce4e6fd08decef8fe4b047462a693bef7d0e19a1b08a71731d057769a`  
		Last Modified: Wed, 01 Apr 2020 05:58:55 GMT  
		Size: 1.2 MB (1217474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6b9f0c55a9cb31a1fe9245e8b6fd7289e71e07b1cde1a80fd6aa8636933e374`  
		Last Modified: Wed, 01 Apr 2020 05:58:54 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e3672877c4fc4ef3ec6151c6b363981966fa03e2cfbae0ba80f168670103a2a`  
		Last Modified: Wed, 01 Apr 2020 05:58:55 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:1.6.3`

```console
$ docker pull memcached@sha256:24bafb41bd77e33e791c5154d157ff38af129d747264f84bdc11ea091fa63000
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `memcached:1.6.3` - linux; amd64

```console
$ docker pull memcached@sha256:6bdc214f60e191847cf0f57721aba4ba68cc3357eb38fc8ea31e935c350c5e0c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.5 MB (30485763 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ac3dd24663f48d13eca8fc54d99547759af3dace518eaff1dc413120737ece5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 31 Mar 2020 01:21:01 GMT
ADD file:d1f1b387a158136fb0f8096c8a8ecf5fc146be4e85c1c3c345d44c927692723a in / 
# Tue, 31 Mar 2020 01:21:01 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 13:20:36 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 31 Mar 2020 13:20:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Apr 2020 04:26:20 GMT
ENV MEMCACHED_VERSION=1.6.3
# Wed, 01 Apr 2020 04:26:20 GMT
ENV MEMCACHED_SHA1=bcd6d0c076ca2b62e9bd31f6669acc8563df7db1
# Wed, 01 Apr 2020 04:34:30 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 01 Apr 2020 04:34:30 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 01 Apr 2020 04:34:31 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 01 Apr 2020 04:34:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Apr 2020 04:34:31 GMT
USER memcache
# Wed, 01 Apr 2020 04:34:32 GMT
EXPOSE 11211
# Wed, 01 Apr 2020 04:34:32 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:c499e6d256d6d4a546f1c141e04b5b4951983ba7581e39deaf5cc595289ee70f`  
		Last Modified: Tue, 31 Mar 2020 01:26:37 GMT  
		Size: 27.1 MB (27091862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:512f277e1da84b0b9319530d40c48750bb22b13f4816d103040d20c0635c28be`  
		Last Modified: Tue, 31 Mar 2020 13:29:52 GMT  
		Size: 5.0 KB (4984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdda69e165e26c667ba223dc215274101c3c6e41db182bd651aadf5e5623fc35`  
		Last Modified: Tue, 31 Mar 2020 13:29:53 GMT  
		Size: 2.2 MB (2196476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43b37ee911063bfa8e0a60293b8ba301a22c3b29e26bf39c33f017e1b4bef28e`  
		Last Modified: Wed, 01 Apr 2020 04:43:03 GMT  
		Size: 1.2 MB (1192033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b83bd7ea262edefd8fa75ce5e40145b491e787de8d3806265e986a60cad606e0`  
		Last Modified: Wed, 01 Apr 2020 04:43:03 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc4fa7c552bc03701653c81434f6e3f7312745deb0c26e039e7565acca70ea54`  
		Last Modified: Wed, 01 Apr 2020 04:43:03 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.3` - linux; arm variant v5

```console
$ docker pull memcached@sha256:aa492daa963294573d6319a6a19d392cce213240b81078dba65869e538611c97
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.9 MB (27889314 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c0ec6623b84d3061e2fa7dab933f5e39cc8c9b170bbf6fd5ce0b4baf35341c30`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 31 Mar 2020 01:24:54 GMT
ADD file:e08ed9e60228d351de400af5746474777a562d99f17e0cb1ce3e3d352e9ec751 in / 
# Tue, 31 Mar 2020 01:24:56 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 01:54:28 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 31 Mar 2020 01:55:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Mar 2020 19:48:28 GMT
ENV MEMCACHED_VERSION=1.6.3
# Tue, 31 Mar 2020 19:48:30 GMT
ENV MEMCACHED_SHA1=bcd6d0c076ca2b62e9bd31f6669acc8563df7db1
# Tue, 31 Mar 2020 20:49:40 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 31 Mar 2020 20:49:43 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 31 Mar 2020 20:49:54 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 31 Mar 2020 20:49:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 31 Mar 2020 20:49:58 GMT
USER memcache
# Tue, 31 Mar 2020 20:50:00 GMT
EXPOSE 11211
# Tue, 31 Mar 2020 20:50:02 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:440df189aa3df85587f2d7d348500930481b3752dcb887d212de9b44b49076dd`  
		Last Modified: Tue, 31 Mar 2020 01:33:04 GMT  
		Size: 24.8 MB (24830324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bde8351817341fa2fec288d97635ede228892bbb58fc5c6ca54441acef6f0766`  
		Last Modified: Tue, 31 Mar 2020 03:24:42 GMT  
		Size: 4.9 KB (4896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b011e5f13bdf6608cafa62557b3c877e4794590eaadced0b8a49fe24a28d110`  
		Last Modified: Tue, 31 Mar 2020 03:24:44 GMT  
		Size: 1.9 MB (1896786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d15532e44d1b4cbd93a29d2f59e8d316aac3697819e686b863a04b7306f66e97`  
		Last Modified: Tue, 31 Mar 2020 20:50:23 GMT  
		Size: 1.2 MB (1156899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51aa0f21d752e0ddd5092569a00faade9a48585be4787ea0915d3bcd56ee1de5`  
		Last Modified: Tue, 31 Mar 2020 20:50:27 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e86f84b137f1eb137ff83d27d7cff6eee693a6dab12d7ce99ff0c2a77a49b6ae`  
		Last Modified: Tue, 31 Mar 2020 20:50:28 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.3` - linux; arm variant v7

```console
$ docker pull memcached@sha256:d54eb37ba24eeb017adff9ad74f97c71f8232153c291be63893eb6ade8836656
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.6 MB (25646260 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0d8ee9533c9e5e31033a1bc594eeac7543678ca190a7b66d654a6b5385f8e5a7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 31 Mar 2020 01:48:12 GMT
ADD file:8c3ed0df404a6bcaf7583e71796cb4c1f40e87288953a21d4ee5946079c3274f in / 
# Tue, 31 Mar 2020 01:48:13 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 03:27:08 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 31 Mar 2020 03:28:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Mar 2020 20:51:09 GMT
ENV MEMCACHED_VERSION=1.6.3
# Tue, 31 Mar 2020 20:51:11 GMT
ENV MEMCACHED_SHA1=bcd6d0c076ca2b62e9bd31f6669acc8563df7db1
# Tue, 31 Mar 2020 21:21:03 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 31 Mar 2020 21:21:07 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 31 Mar 2020 21:21:18 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 31 Mar 2020 21:21:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 31 Mar 2020 21:21:22 GMT
USER memcache
# Tue, 31 Mar 2020 21:21:24 GMT
EXPOSE 11211
# Tue, 31 Mar 2020 21:21:26 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:98098fa10651fdba12c848231b7428536a120e17637f1f9e0d25c63880483fcc`  
		Last Modified: Tue, 31 Mar 2020 01:56:24 GMT  
		Size: 22.7 MB (22699731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a7a42e48b851419bcd11506631a8d336fb394d979dcea8feb4830f38ba7cfd7`  
		Last Modified: Tue, 31 Mar 2020 04:39:27 GMT  
		Size: 4.9 KB (4899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc96c4fde110b7a8691d85cf0523cd326fbfd1bcbf928719f6173cd292c91305`  
		Last Modified: Tue, 31 Mar 2020 04:39:35 GMT  
		Size: 1.8 MB (1811551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2a043ecd402e02473caef2834dd90c40a3a16ee899cb87574bf7fb8b1183adb`  
		Last Modified: Tue, 31 Mar 2020 23:12:26 GMT  
		Size: 1.1 MB (1129671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6b3946960ee59ded096d4489e81d9cd3af3506ce6f99c79f38648217430a2f0`  
		Last Modified: Tue, 31 Mar 2020 23:12:24 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34b5c1dda6f0d125b29798f04589e1f46502983dbe8f4cf5763a2a2592148191`  
		Last Modified: Tue, 31 Mar 2020 23:12:30 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.3` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:056b511f1e97a6619c24aadc781560db65e25abc0c3a98bbe25b52d81b24e78c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.1 MB (29094504 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:142fbd99d85857a0807b95f6c5621c5006b38c522d78f4f8e088fdd6a4061db8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 31 Mar 2020 02:05:33 GMT
ADD file:47ab456123ae97a527249191ff2bc0014e7ef0ae186aec91bf6a63eb077ecb91 in / 
# Tue, 31 Mar 2020 02:05:35 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 08:39:07 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 31 Mar 2020 08:39:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Apr 2020 04:44:54 GMT
ENV MEMCACHED_VERSION=1.6.3
# Wed, 01 Apr 2020 04:44:55 GMT
ENV MEMCACHED_SHA1=bcd6d0c076ca2b62e9bd31f6669acc8563df7db1
# Wed, 01 Apr 2020 04:54:03 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 01 Apr 2020 04:54:05 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 01 Apr 2020 04:54:07 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 01 Apr 2020 04:54:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Apr 2020 04:54:08 GMT
USER memcache
# Wed, 01 Apr 2020 04:54:08 GMT
EXPOSE 11211
# Wed, 01 Apr 2020 04:54:09 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:a6c32b8bc1ce2b374630673ded1d5ef5a98936d045bf0632fcf599dc2229d493`  
		Last Modified: Tue, 31 Mar 2020 02:12:15 GMT  
		Size: 25.9 MB (25851645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72560398e0dc8991a53cd07c580b14e3c2024d7af30d2dfe8428d913006af5a9`  
		Last Modified: Tue, 31 Mar 2020 08:48:55 GMT  
		Size: 5.0 KB (5028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4febdbdc3565b2d569ed0a6885c548a5755cd9a2b52c21b351d254c83e6fff7`  
		Last Modified: Tue, 31 Mar 2020 08:48:55 GMT  
		Size: 2.1 MB (2074952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b1797ec4dd007a4f822abca922aa457a793f2ba04b4481e6c1f0de7e34b32d8`  
		Last Modified: Wed, 01 Apr 2020 05:12:38 GMT  
		Size: 1.2 MB (1162471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b9601a34125cd3cfe733ea2ce11005afc0ec6f02bd14b34d5d5ce92a9dadb1c`  
		Last Modified: Wed, 01 Apr 2020 05:12:39 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:703422421b84c80f0ed9b79b040ba35dbf37e06c80b5e9681455202c1b2091f6`  
		Last Modified: Wed, 01 Apr 2020 05:12:38 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.3` - linux; 386

```console
$ docker pull memcached@sha256:45e70e58745f9b65a1fdbea626d26be12194087fa3f2ebc06647d23dd8ff4dd3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.2 MB (31156562 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7371335c883334e01e87c4a4b5cf189b8b2876ff43cd38604954befcf0afc780`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 31 Mar 2020 00:39:42 GMT
ADD file:a453117866661af4ddfa21203d65ce6661efeaeca2a1704e09747c83b4c58e47 in / 
# Tue, 31 Mar 2020 00:39:42 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 11:45:29 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 31 Mar 2020 11:45:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Apr 2020 00:36:05 GMT
ENV MEMCACHED_VERSION=1.6.3
# Wed, 01 Apr 2020 00:36:06 GMT
ENV MEMCACHED_SHA1=bcd6d0c076ca2b62e9bd31f6669acc8563df7db1
# Wed, 01 Apr 2020 00:45:06 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 01 Apr 2020 00:45:06 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 01 Apr 2020 00:45:08 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 01 Apr 2020 00:45:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Apr 2020 00:45:09 GMT
USER memcache
# Wed, 01 Apr 2020 00:45:09 GMT
EXPOSE 11211
# Wed, 01 Apr 2020 00:45:10 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:2314106a15e49c7908bebb2c697dcaf3d6a1626b70fe72bc0c0cb71eb216ddc3`  
		Last Modified: Tue, 31 Mar 2020 00:45:31 GMT  
		Size: 27.7 MB (27747648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3bafab0976764495dda52d0c16addb4770d62d8f9de55728b752ff3448f2292`  
		Last Modified: Tue, 31 Mar 2020 11:55:29 GMT  
		Size: 4.9 KB (4899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8307e5e61ebc9ed2430c9e45ba3437aa1deebed0882ce15c36616e0debf28b36`  
		Last Modified: Tue, 31 Mar 2020 11:55:29 GMT  
		Size: 2.2 MB (2208079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2346314e755e47f2a21140be69437185fef4416c21871e9bea2504e4011aa31c`  
		Last Modified: Wed, 01 Apr 2020 00:54:20 GMT  
		Size: 1.2 MB (1195528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04f73e333f816b2d2fa26694d21c4c50e393e11ecbe6c172966071f7a5c60a31`  
		Last Modified: Wed, 01 Apr 2020 00:54:20 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:882932b666818b8fc239f2047d12a409ec5f211424e6321a671aabd98da708bc`  
		Last Modified: Wed, 01 Apr 2020 00:54:20 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.3` - linux; ppc64le

```console
$ docker pull memcached@sha256:9d4d92103d08915f9f79003636917f96ee58591cf3fc4bf22c5331ee582ea6d1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.1 MB (34064010 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:296aceabbfb0b475275d0104ab416027cdcb9ac9c53140cb7791a505e2a8ff70`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 31 Mar 2020 01:32:42 GMT
ADD file:36c02e92574faba45b64cfed78a0a0359d65ad175b17128bf554a2a5c0086ff5 in / 
# Tue, 31 Mar 2020 01:32:47 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 12:45:58 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 31 Mar 2020 12:46:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Apr 2020 05:38:36 GMT
ENV MEMCACHED_VERSION=1.6.3
# Wed, 01 Apr 2020 05:38:38 GMT
ENV MEMCACHED_SHA1=bcd6d0c076ca2b62e9bd31f6669acc8563df7db1
# Wed, 01 Apr 2020 05:48:45 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 01 Apr 2020 05:48:47 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 01 Apr 2020 05:48:55 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 01 Apr 2020 05:49:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Apr 2020 05:49:05 GMT
USER memcache
# Wed, 01 Apr 2020 05:49:09 GMT
EXPOSE 11211
# Wed, 01 Apr 2020 05:49:14 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:9df6bbae5eeb29e9aac2f39cff517c694cce60f01ee477abcdedcd8e8c01c38f`  
		Last Modified: Tue, 31 Mar 2020 01:45:59 GMT  
		Size: 30.5 MB (30518493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2786c1a6fbad6e8c56e4f7e33b4d41c64efd06c4cdb303a50c07ee1f4c5f7a69`  
		Last Modified: Tue, 31 Mar 2020 12:58:00 GMT  
		Size: 5.0 KB (4987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:722cfb50c03533f4b5c83c84a2f565dbcdbf63c01460ae91d35aafacd94454fe`  
		Last Modified: Tue, 31 Mar 2020 12:58:00 GMT  
		Size: 2.3 MB (2322647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7e848dce4e6fd08decef8fe4b047462a693bef7d0e19a1b08a71731d057769a`  
		Last Modified: Wed, 01 Apr 2020 05:58:55 GMT  
		Size: 1.2 MB (1217474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6b9f0c55a9cb31a1fe9245e8b6fd7289e71e07b1cde1a80fd6aa8636933e374`  
		Last Modified: Wed, 01 Apr 2020 05:58:54 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e3672877c4fc4ef3ec6151c6b363981966fa03e2cfbae0ba80f168670103a2a`  
		Last Modified: Wed, 01 Apr 2020 05:58:55 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:1.6.3-alpine`

```console
$ docker pull memcached@sha256:087841c25b352730f083aeb30d2d07440a238345e31016e9bca6242e9a30c014
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `memcached:1.6.3-alpine` - linux; amd64

```console
$ docker pull memcached@sha256:504421bbf708add1d72e89d605ea3ea63d4b781866405bcfa5446e0172ad16eb
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.4 MB (4371683 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:801fa8ca11ab6a7fd7c3976f966b1a4b804a1f28db61aaf9156e1835dc78c55b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 23 Mar 2020 21:19:34 GMT
ADD file:0c4555f363c2672e350001f1293e689875a3760afe7b3f9146886afe67121cba in / 
# Mon, 23 Mar 2020 21:19:34 GMT
CMD ["/bin/sh"]
# Tue, 24 Mar 2020 00:40:06 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 24 Mar 2020 00:40:07 GMT
RUN apk add --no-cache cyrus-sasl-plain
# Wed, 01 Apr 2020 04:34:39 GMT
ENV MEMCACHED_VERSION=1.6.3
# Wed, 01 Apr 2020 04:34:39 GMT
ENV MEMCACHED_SHA1=bcd6d0c076ca2b62e9bd31f6669acc8563df7db1
# Wed, 01 Apr 2020 04:42:43 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		dpkg-dev dpkg 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		tar 		wget 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& make test 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Wed, 01 Apr 2020 04:42:43 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 01 Apr 2020 04:42:44 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 01 Apr 2020 04:42:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Apr 2020 04:42:45 GMT
USER memcache
# Wed, 01 Apr 2020 04:42:45 GMT
EXPOSE 11211
# Wed, 01 Apr 2020 04:42:45 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:aad63a9339440e7c3e1fff2b988991b9bfb81280042fa7f39a5e327023056819`  
		Last Modified: Mon, 23 Mar 2020 21:19:53 GMT  
		Size: 2.8 MB (2803255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a5fb4ad400df404c486089fa4098e9e6bfdb1528c2ee85cbd5614e8a97f1f9a`  
		Last Modified: Tue, 24 Mar 2020 00:48:55 GMT  
		Size: 1.2 KB (1230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb602a49f6f4777651777faab36b80d92a2f1dbe36d865c0cce4e182439c6b5e`  
		Last Modified: Tue, 24 Mar 2020 00:48:55 GMT  
		Size: 15.1 KB (15099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9170b88a2b9dff1d8fed938f8b1fbed86749b7d29b6208fa1e833c1c5447371`  
		Last Modified: Wed, 01 Apr 2020 04:43:08 GMT  
		Size: 1.6 MB (1551693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c57ce97f5eb3f42443e03945bf4f06e8d666362f8231445fd3d2663b875b45d`  
		Last Modified: Wed, 01 Apr 2020 04:43:08 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d8a359c2a701b1da7a72d2fc7a48c413792eeab01fecc13e555114ec5fefecb`  
		Last Modified: Wed, 01 Apr 2020 04:43:08 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.3-alpine` - linux; arm variant v6

```console
$ docker pull memcached@sha256:e54f5e55a14b5162d421327cccb9cda48be89d264d9a1f48f5c93a286e69f39f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.1 MB (4148717 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:904fb49ed16723e4d5093b937c02b08e15f7c710350f1e169073dae639179d42`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 23 Mar 2020 21:49:26 GMT
ADD file:e2fdfc637b534345942caf4097883508a5ed23be97d85ccc3357b8277aaa5430 in / 
# Mon, 23 Mar 2020 21:49:27 GMT
CMD ["/bin/sh"]
# Mon, 23 Mar 2020 23:15:28 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Mon, 23 Mar 2020 23:15:34 GMT
RUN apk add --no-cache cyrus-sasl-plain
# Tue, 31 Mar 2020 19:49:46 GMT
ENV MEMCACHED_VERSION=1.6.3
# Tue, 31 Mar 2020 19:49:47 GMT
ENV MEMCACHED_SHA1=bcd6d0c076ca2b62e9bd31f6669acc8563df7db1
# Tue, 31 Mar 2020 19:59:09 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		dpkg-dev dpkg 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		tar 		wget 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& make test 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 31 Mar 2020 19:59:10 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 31 Mar 2020 19:59:13 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 31 Mar 2020 19:59:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 31 Mar 2020 19:59:15 GMT
USER memcache
# Tue, 31 Mar 2020 19:59:15 GMT
EXPOSE 11211
# Tue, 31 Mar 2020 19:59:16 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:0776aeec3430c5a5ba3f43937f0ee6a7770a1fe81a318c9d94cc76512e5375e9`  
		Last Modified: Mon, 23 Mar 2020 21:49:50 GMT  
		Size: 2.6 MB (2618579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f329bb895b7588f4de54c119f39a5f656520bc2310d39893460c4398814112d`  
		Last Modified: Mon, 23 Mar 2020 23:25:38 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6bd8017eeb8ecce1d6b238f86b96a1af52d1a9dd44bc0da4c0573f58a7f51a8`  
		Last Modified: Mon, 23 Mar 2020 23:25:38 GMT  
		Size: 14.7 KB (14695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97a1fc78f0dd1f4d19a9b453400ea3d5bf6515aefe2044cea13a0fbbf7176ab7`  
		Last Modified: Tue, 31 Mar 2020 19:59:29 GMT  
		Size: 1.5 MB (1513779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d36dc6635f5960f1ed529c19648cde5341e1ac518cea270e90f260fe3183ff57`  
		Last Modified: Tue, 31 Mar 2020 19:59:29 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7f6bf3b6679ec09f33841e74c14bb0c5784632df49b25276e5c61960bcd43be`  
		Last Modified: Tue, 31 Mar 2020 19:59:29 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.3-alpine` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:799a51f3fbf3504dee7e5152154ac2ab528b2674eb037b211597b4ed702365e0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.3 MB (4294297 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:60c011071a320179ee9e80babe7d159b06f5f64be786388cca8fa903fd7a6f3a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 23 Mar 2020 21:39:52 GMT
ADD file:746a5c3838a898d6acf7877552ff13d1ab40d0036ace7a662e7c747018315ddb in / 
# Mon, 23 Mar 2020 21:39:53 GMT
CMD ["/bin/sh"]
# Tue, 24 Mar 2020 05:16:12 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 24 Mar 2020 05:16:15 GMT
RUN apk add --no-cache cyrus-sasl-plain
# Wed, 01 Apr 2020 04:54:17 GMT
ENV MEMCACHED_VERSION=1.6.3
# Wed, 01 Apr 2020 04:54:18 GMT
ENV MEMCACHED_SHA1=bcd6d0c076ca2b62e9bd31f6669acc8563df7db1
# Wed, 01 Apr 2020 05:12:17 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		dpkg-dev dpkg 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		tar 		wget 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& make test 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Wed, 01 Apr 2020 05:12:18 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 01 Apr 2020 05:12:20 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 01 Apr 2020 05:12:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Apr 2020 05:12:21 GMT
USER memcache
# Wed, 01 Apr 2020 05:12:21 GMT
EXPOSE 11211
# Wed, 01 Apr 2020 05:12:22 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:8a0637ca1ac98db4cf29f7632449c92801adc80cf0da2cd9c9e39882ce466561`  
		Last Modified: Mon, 23 Mar 2020 21:40:19 GMT  
		Size: 2.7 MB (2723139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd1bfe9c2142f88c6e142b39adf7ba4fe722789b650d5a54184ff336826ae16f`  
		Last Modified: Tue, 24 Mar 2020 05:25:36 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f4d8154a8d6d9edf61516528f99c62d27eb41f8602571ae30fdf745976e2c6e`  
		Last Modified: Tue, 24 Mar 2020 05:25:35 GMT  
		Size: 15.5 KB (15490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7f106af3c2ed3a7290ace796d3928ebace90adf39411884be3a63a0df58c99c`  
		Last Modified: Wed, 01 Apr 2020 05:12:48 GMT  
		Size: 1.6 MB (1554004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ddd0a23420ce85ddf49ae379a74b2adc3afdc6c6f34003263083f8ed39126ab`  
		Last Modified: Wed, 01 Apr 2020 05:12:47 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bac1f8b4b923cdd7efd688cf758bd3e14304ad2bc41d5732d2f73d1b6d65434b`  
		Last Modified: Wed, 01 Apr 2020 05:12:47 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.3-alpine` - linux; 386

```console
$ docker pull memcached@sha256:d05780d5c31011aff04ebd8af83f27031e669630042d061a6789e57298135010
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4472019 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91afec457abab7b418a13cc0ec15b9b886444899fd1bd6012f8139d6bd71aca8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 23 Mar 2020 21:38:28 GMT
ADD file:99c8234abafd4fa915c0b826eb0e3be0e6aaa7c1e33cb1214ef71a99e9c02e06 in / 
# Mon, 23 Mar 2020 21:38:28 GMT
CMD ["/bin/sh"]
# Tue, 24 Mar 2020 04:55:12 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 24 Mar 2020 04:55:13 GMT
RUN apk add --no-cache cyrus-sasl-plain
# Wed, 01 Apr 2020 00:45:25 GMT
ENV MEMCACHED_VERSION=1.6.3
# Wed, 01 Apr 2020 00:45:26 GMT
ENV MEMCACHED_SHA1=bcd6d0c076ca2b62e9bd31f6669acc8563df7db1
# Wed, 01 Apr 2020 00:54:03 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		dpkg-dev dpkg 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		tar 		wget 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& make test 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Wed, 01 Apr 2020 00:54:04 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 01 Apr 2020 00:54:04 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 01 Apr 2020 00:54:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Apr 2020 00:54:05 GMT
USER memcache
# Wed, 01 Apr 2020 00:54:05 GMT
EXPOSE 11211
# Wed, 01 Apr 2020 00:54:05 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:43f6a4398e1c9e860dfb5c93d7049ab9eedf814513bd6d07e06077c560303c7a`  
		Last Modified: Mon, 23 Mar 2020 21:38:48 GMT  
		Size: 2.8 MB (2806122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a31d073afa8dea3b0bfd6eeb6ebffc6447996f0e9cabebf9d749474ac22cdf2d`  
		Last Modified: Tue, 24 Mar 2020 05:04:58 GMT  
		Size: 1.2 KB (1230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:905909a3db778acdf7295903cff6ee7b27263e33facc5982475e7b60831413fc`  
		Last Modified: Tue, 24 Mar 2020 05:04:58 GMT  
		Size: 16.1 KB (16146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:084fe9c6c267a28b7ef7682ca30611f165ec248e04aa077a2a2d73f4457fabab`  
		Last Modified: Wed, 01 Apr 2020 00:54:25 GMT  
		Size: 1.6 MB (1648120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e913734356dc8bab85686d97ef17baaca409de999cb2b9fabe5ce05705f0e8cc`  
		Last Modified: Wed, 01 Apr 2020 00:54:25 GMT  
		Size: 280.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e4fafb5feec45ada3475ec22c6c9b55762badb826cec0d46db5aafec25b9e3f`  
		Last Modified: Wed, 01 Apr 2020 00:54:25 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.3-alpine` - linux; ppc64le

```console
$ docker pull memcached@sha256:e39ab357bebea313936e055707ba4ae986ff9f2c9f6884b1f2ef0241a4d03f59
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.4 MB (4448402 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2860d592b00ed82e9bc857eb9cf6873241d6f7d3f1162977a81fee56b5a4c4d8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 23 Mar 2020 21:21:29 GMT
ADD file:4b35131542b9682214e1c2c72fe3cea215a10e2f775e87befecd80fe2228d5a0 in / 
# Mon, 23 Mar 2020 21:21:32 GMT
CMD ["/bin/sh"]
# Tue, 24 Mar 2020 02:24:20 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 24 Mar 2020 02:24:25 GMT
RUN apk add --no-cache cyrus-sasl-plain
# Wed, 01 Apr 2020 05:49:31 GMT
ENV MEMCACHED_VERSION=1.6.3
# Wed, 01 Apr 2020 05:49:35 GMT
ENV MEMCACHED_SHA1=bcd6d0c076ca2b62e9bd31f6669acc8563df7db1
# Wed, 01 Apr 2020 05:58:02 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		dpkg-dev dpkg 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		tar 		wget 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& make test 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Wed, 01 Apr 2020 05:58:03 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 01 Apr 2020 05:58:12 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 01 Apr 2020 05:58:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Apr 2020 05:58:20 GMT
USER memcache
# Wed, 01 Apr 2020 05:58:22 GMT
EXPOSE 11211
# Wed, 01 Apr 2020 05:58:25 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:bc1c99f4ba60de0d3ca52dc6855483e24c91884e33df71f502bbff6eb909d9b9`  
		Last Modified: Mon, 23 Mar 2020 21:22:12 GMT  
		Size: 2.8 MB (2820052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c50bd2ca891d67079878bf06e36ba609e8528e83369265c92fbd3b03e6e839f1`  
		Last Modified: Tue, 24 Mar 2020 02:34:02 GMT  
		Size: 1.3 KB (1263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a4704e4e496c0d18b40f484fc715146c1f427050210b40271112edcf751a698`  
		Last Modified: Tue, 24 Mar 2020 02:34:02 GMT  
		Size: 16.1 KB (16131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10436c8816f1c5f62f5007787e0a21833b186a194f03d364bf347f6e7a587004`  
		Last Modified: Wed, 01 Apr 2020 05:59:14 GMT  
		Size: 1.6 MB (1610549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07449479f271de853b60dfdf76a99142a7c6b26b5e985c6112595bf6d31f54b1`  
		Last Modified: Wed, 01 Apr 2020 05:59:14 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de62a3b128b893893b9888ff271738dbb09a45ea52b8ad30f386427dc7497448`  
		Last Modified: Wed, 01 Apr 2020 05:59:14 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:1.6-alpine`

```console
$ docker pull memcached@sha256:651b7a83bcd78f9cfcb56ec230428b321f6b4cb8c8a26449454f77dc5d4ecf04
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
$ docker pull memcached@sha256:504421bbf708add1d72e89d605ea3ea63d4b781866405bcfa5446e0172ad16eb
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.4 MB (4371683 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:801fa8ca11ab6a7fd7c3976f966b1a4b804a1f28db61aaf9156e1835dc78c55b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 23 Mar 2020 21:19:34 GMT
ADD file:0c4555f363c2672e350001f1293e689875a3760afe7b3f9146886afe67121cba in / 
# Mon, 23 Mar 2020 21:19:34 GMT
CMD ["/bin/sh"]
# Tue, 24 Mar 2020 00:40:06 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 24 Mar 2020 00:40:07 GMT
RUN apk add --no-cache cyrus-sasl-plain
# Wed, 01 Apr 2020 04:34:39 GMT
ENV MEMCACHED_VERSION=1.6.3
# Wed, 01 Apr 2020 04:34:39 GMT
ENV MEMCACHED_SHA1=bcd6d0c076ca2b62e9bd31f6669acc8563df7db1
# Wed, 01 Apr 2020 04:42:43 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		dpkg-dev dpkg 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		tar 		wget 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& make test 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Wed, 01 Apr 2020 04:42:43 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 01 Apr 2020 04:42:44 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 01 Apr 2020 04:42:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Apr 2020 04:42:45 GMT
USER memcache
# Wed, 01 Apr 2020 04:42:45 GMT
EXPOSE 11211
# Wed, 01 Apr 2020 04:42:45 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:aad63a9339440e7c3e1fff2b988991b9bfb81280042fa7f39a5e327023056819`  
		Last Modified: Mon, 23 Mar 2020 21:19:53 GMT  
		Size: 2.8 MB (2803255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a5fb4ad400df404c486089fa4098e9e6bfdb1528c2ee85cbd5614e8a97f1f9a`  
		Last Modified: Tue, 24 Mar 2020 00:48:55 GMT  
		Size: 1.2 KB (1230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb602a49f6f4777651777faab36b80d92a2f1dbe36d865c0cce4e182439c6b5e`  
		Last Modified: Tue, 24 Mar 2020 00:48:55 GMT  
		Size: 15.1 KB (15099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9170b88a2b9dff1d8fed938f8b1fbed86749b7d29b6208fa1e833c1c5447371`  
		Last Modified: Wed, 01 Apr 2020 04:43:08 GMT  
		Size: 1.6 MB (1551693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c57ce97f5eb3f42443e03945bf4f06e8d666362f8231445fd3d2663b875b45d`  
		Last Modified: Wed, 01 Apr 2020 04:43:08 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d8a359c2a701b1da7a72d2fc7a48c413792eeab01fecc13e555114ec5fefecb`  
		Last Modified: Wed, 01 Apr 2020 04:43:08 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-alpine` - linux; arm variant v6

```console
$ docker pull memcached@sha256:e54f5e55a14b5162d421327cccb9cda48be89d264d9a1f48f5c93a286e69f39f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.1 MB (4148717 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:904fb49ed16723e4d5093b937c02b08e15f7c710350f1e169073dae639179d42`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 23 Mar 2020 21:49:26 GMT
ADD file:e2fdfc637b534345942caf4097883508a5ed23be97d85ccc3357b8277aaa5430 in / 
# Mon, 23 Mar 2020 21:49:27 GMT
CMD ["/bin/sh"]
# Mon, 23 Mar 2020 23:15:28 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Mon, 23 Mar 2020 23:15:34 GMT
RUN apk add --no-cache cyrus-sasl-plain
# Tue, 31 Mar 2020 19:49:46 GMT
ENV MEMCACHED_VERSION=1.6.3
# Tue, 31 Mar 2020 19:49:47 GMT
ENV MEMCACHED_SHA1=bcd6d0c076ca2b62e9bd31f6669acc8563df7db1
# Tue, 31 Mar 2020 19:59:09 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		dpkg-dev dpkg 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		tar 		wget 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& make test 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 31 Mar 2020 19:59:10 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 31 Mar 2020 19:59:13 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 31 Mar 2020 19:59:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 31 Mar 2020 19:59:15 GMT
USER memcache
# Tue, 31 Mar 2020 19:59:15 GMT
EXPOSE 11211
# Tue, 31 Mar 2020 19:59:16 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:0776aeec3430c5a5ba3f43937f0ee6a7770a1fe81a318c9d94cc76512e5375e9`  
		Last Modified: Mon, 23 Mar 2020 21:49:50 GMT  
		Size: 2.6 MB (2618579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f329bb895b7588f4de54c119f39a5f656520bc2310d39893460c4398814112d`  
		Last Modified: Mon, 23 Mar 2020 23:25:38 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6bd8017eeb8ecce1d6b238f86b96a1af52d1a9dd44bc0da4c0573f58a7f51a8`  
		Last Modified: Mon, 23 Mar 2020 23:25:38 GMT  
		Size: 14.7 KB (14695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97a1fc78f0dd1f4d19a9b453400ea3d5bf6515aefe2044cea13a0fbbf7176ab7`  
		Last Modified: Tue, 31 Mar 2020 19:59:29 GMT  
		Size: 1.5 MB (1513779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d36dc6635f5960f1ed529c19648cde5341e1ac518cea270e90f260fe3183ff57`  
		Last Modified: Tue, 31 Mar 2020 19:59:29 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7f6bf3b6679ec09f33841e74c14bb0c5784632df49b25276e5c61960bcd43be`  
		Last Modified: Tue, 31 Mar 2020 19:59:29 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-alpine` - linux; arm variant v7

```console
$ docker pull memcached@sha256:ec8c62ad113b358298092e63b474e8aeebb5b1e1bfabb2e6ff525646dc7458f1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3826282 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5af1281a25c9479c7ad3e80e07f3e7b43e774841795c9f93004bf124abe4b0f4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 23 Mar 2020 21:57:55 GMT
ADD file:3bde6b6fd06efbf24e66446c6d32f72294fc749ae9ee6191776242e92b2f8ab4 in / 
# Mon, 23 Mar 2020 21:57:56 GMT
CMD ["/bin/sh"]
# Mon, 23 Mar 2020 22:14:07 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Mon, 23 Mar 2020 22:14:20 GMT
RUN apk add --no-cache cyrus-sasl-plain
# Tue, 24 Mar 2020 01:47:18 GMT
ENV MEMCACHED_VERSION=1.6.2
# Tue, 24 Mar 2020 01:47:22 GMT
ENV MEMCACHED_SHA1=a6a07f0433adaa13a3cafdf8c26acb640cdd001f
# Tue, 24 Mar 2020 03:19:47 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		dpkg-dev dpkg 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		tar 		wget 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& make test 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 24 Mar 2020 03:19:50 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 24 Mar 2020 03:20:01 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 24 Mar 2020 03:20:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 24 Mar 2020 03:20:05 GMT
USER memcache
# Tue, 24 Mar 2020 03:20:07 GMT
EXPOSE 11211
# Tue, 24 Mar 2020 03:20:09 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:d9bf605ce3d4449f4b90035c3e21d691806324781d43a5287b1da25a01779d6b`  
		Last Modified: Mon, 23 Mar 2020 21:58:16 GMT  
		Size: 2.4 MB (2420493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eae54837c45cf98e10469ba87b255979740486d00d9407bc2fcdf1492469dc04`  
		Last Modified: Mon, 23 Mar 2020 22:42:38 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1459ca388d9e53a94cbb39e64789568710013f3b46396b24ea0729b570f74403`  
		Last Modified: Mon, 23 Mar 2020 22:42:44 GMT  
		Size: 13.6 KB (13638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f84775e4ae618e04e599d46af2006e35d62d9046f4908e660cc533b9cbb8c36`  
		Last Modified: Tue, 24 Mar 2020 03:21:11 GMT  
		Size: 1.4 MB (1390486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dd59b3062e02dcff6cd6cbe35ba1e84c44a571112a65c4dd0ad640b905e4ae3`  
		Last Modified: Tue, 24 Mar 2020 03:21:09 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f53094e3dbce9c8d482bfb7123a06c9a0e4e74102891a4aecc833167acbb64db`  
		Last Modified: Tue, 24 Mar 2020 03:21:15 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-alpine` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:799a51f3fbf3504dee7e5152154ac2ab528b2674eb037b211597b4ed702365e0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.3 MB (4294297 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:60c011071a320179ee9e80babe7d159b06f5f64be786388cca8fa903fd7a6f3a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 23 Mar 2020 21:39:52 GMT
ADD file:746a5c3838a898d6acf7877552ff13d1ab40d0036ace7a662e7c747018315ddb in / 
# Mon, 23 Mar 2020 21:39:53 GMT
CMD ["/bin/sh"]
# Tue, 24 Mar 2020 05:16:12 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 24 Mar 2020 05:16:15 GMT
RUN apk add --no-cache cyrus-sasl-plain
# Wed, 01 Apr 2020 04:54:17 GMT
ENV MEMCACHED_VERSION=1.6.3
# Wed, 01 Apr 2020 04:54:18 GMT
ENV MEMCACHED_SHA1=bcd6d0c076ca2b62e9bd31f6669acc8563df7db1
# Wed, 01 Apr 2020 05:12:17 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		dpkg-dev dpkg 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		tar 		wget 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& make test 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Wed, 01 Apr 2020 05:12:18 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 01 Apr 2020 05:12:20 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 01 Apr 2020 05:12:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Apr 2020 05:12:21 GMT
USER memcache
# Wed, 01 Apr 2020 05:12:21 GMT
EXPOSE 11211
# Wed, 01 Apr 2020 05:12:22 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:8a0637ca1ac98db4cf29f7632449c92801adc80cf0da2cd9c9e39882ce466561`  
		Last Modified: Mon, 23 Mar 2020 21:40:19 GMT  
		Size: 2.7 MB (2723139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd1bfe9c2142f88c6e142b39adf7ba4fe722789b650d5a54184ff336826ae16f`  
		Last Modified: Tue, 24 Mar 2020 05:25:36 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f4d8154a8d6d9edf61516528f99c62d27eb41f8602571ae30fdf745976e2c6e`  
		Last Modified: Tue, 24 Mar 2020 05:25:35 GMT  
		Size: 15.5 KB (15490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7f106af3c2ed3a7290ace796d3928ebace90adf39411884be3a63a0df58c99c`  
		Last Modified: Wed, 01 Apr 2020 05:12:48 GMT  
		Size: 1.6 MB (1554004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ddd0a23420ce85ddf49ae379a74b2adc3afdc6c6f34003263083f8ed39126ab`  
		Last Modified: Wed, 01 Apr 2020 05:12:47 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bac1f8b4b923cdd7efd688cf758bd3e14304ad2bc41d5732d2f73d1b6d65434b`  
		Last Modified: Wed, 01 Apr 2020 05:12:47 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-alpine` - linux; 386

```console
$ docker pull memcached@sha256:d05780d5c31011aff04ebd8af83f27031e669630042d061a6789e57298135010
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4472019 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91afec457abab7b418a13cc0ec15b9b886444899fd1bd6012f8139d6bd71aca8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 23 Mar 2020 21:38:28 GMT
ADD file:99c8234abafd4fa915c0b826eb0e3be0e6aaa7c1e33cb1214ef71a99e9c02e06 in / 
# Mon, 23 Mar 2020 21:38:28 GMT
CMD ["/bin/sh"]
# Tue, 24 Mar 2020 04:55:12 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 24 Mar 2020 04:55:13 GMT
RUN apk add --no-cache cyrus-sasl-plain
# Wed, 01 Apr 2020 00:45:25 GMT
ENV MEMCACHED_VERSION=1.6.3
# Wed, 01 Apr 2020 00:45:26 GMT
ENV MEMCACHED_SHA1=bcd6d0c076ca2b62e9bd31f6669acc8563df7db1
# Wed, 01 Apr 2020 00:54:03 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		dpkg-dev dpkg 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		tar 		wget 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& make test 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Wed, 01 Apr 2020 00:54:04 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 01 Apr 2020 00:54:04 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 01 Apr 2020 00:54:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Apr 2020 00:54:05 GMT
USER memcache
# Wed, 01 Apr 2020 00:54:05 GMT
EXPOSE 11211
# Wed, 01 Apr 2020 00:54:05 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:43f6a4398e1c9e860dfb5c93d7049ab9eedf814513bd6d07e06077c560303c7a`  
		Last Modified: Mon, 23 Mar 2020 21:38:48 GMT  
		Size: 2.8 MB (2806122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a31d073afa8dea3b0bfd6eeb6ebffc6447996f0e9cabebf9d749474ac22cdf2d`  
		Last Modified: Tue, 24 Mar 2020 05:04:58 GMT  
		Size: 1.2 KB (1230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:905909a3db778acdf7295903cff6ee7b27263e33facc5982475e7b60831413fc`  
		Last Modified: Tue, 24 Mar 2020 05:04:58 GMT  
		Size: 16.1 KB (16146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:084fe9c6c267a28b7ef7682ca30611f165ec248e04aa077a2a2d73f4457fabab`  
		Last Modified: Wed, 01 Apr 2020 00:54:25 GMT  
		Size: 1.6 MB (1648120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e913734356dc8bab85686d97ef17baaca409de999cb2b9fabe5ce05705f0e8cc`  
		Last Modified: Wed, 01 Apr 2020 00:54:25 GMT  
		Size: 280.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e4fafb5feec45ada3475ec22c6c9b55762badb826cec0d46db5aafec25b9e3f`  
		Last Modified: Wed, 01 Apr 2020 00:54:25 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-alpine` - linux; ppc64le

```console
$ docker pull memcached@sha256:e39ab357bebea313936e055707ba4ae986ff9f2c9f6884b1f2ef0241a4d03f59
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.4 MB (4448402 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2860d592b00ed82e9bc857eb9cf6873241d6f7d3f1162977a81fee56b5a4c4d8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 23 Mar 2020 21:21:29 GMT
ADD file:4b35131542b9682214e1c2c72fe3cea215a10e2f775e87befecd80fe2228d5a0 in / 
# Mon, 23 Mar 2020 21:21:32 GMT
CMD ["/bin/sh"]
# Tue, 24 Mar 2020 02:24:20 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 24 Mar 2020 02:24:25 GMT
RUN apk add --no-cache cyrus-sasl-plain
# Wed, 01 Apr 2020 05:49:31 GMT
ENV MEMCACHED_VERSION=1.6.3
# Wed, 01 Apr 2020 05:49:35 GMT
ENV MEMCACHED_SHA1=bcd6d0c076ca2b62e9bd31f6669acc8563df7db1
# Wed, 01 Apr 2020 05:58:02 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		dpkg-dev dpkg 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		tar 		wget 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& make test 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Wed, 01 Apr 2020 05:58:03 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 01 Apr 2020 05:58:12 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 01 Apr 2020 05:58:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Apr 2020 05:58:20 GMT
USER memcache
# Wed, 01 Apr 2020 05:58:22 GMT
EXPOSE 11211
# Wed, 01 Apr 2020 05:58:25 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:bc1c99f4ba60de0d3ca52dc6855483e24c91884e33df71f502bbff6eb909d9b9`  
		Last Modified: Mon, 23 Mar 2020 21:22:12 GMT  
		Size: 2.8 MB (2820052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c50bd2ca891d67079878bf06e36ba609e8528e83369265c92fbd3b03e6e839f1`  
		Last Modified: Tue, 24 Mar 2020 02:34:02 GMT  
		Size: 1.3 KB (1263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a4704e4e496c0d18b40f484fc715146c1f427050210b40271112edcf751a698`  
		Last Modified: Tue, 24 Mar 2020 02:34:02 GMT  
		Size: 16.1 KB (16131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10436c8816f1c5f62f5007787e0a21833b186a194f03d364bf347f6e7a587004`  
		Last Modified: Wed, 01 Apr 2020 05:59:14 GMT  
		Size: 1.6 MB (1610549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07449479f271de853b60dfdf76a99142a7c6b26b5e985c6112595bf6d31f54b1`  
		Last Modified: Wed, 01 Apr 2020 05:59:14 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de62a3b128b893893b9888ff271738dbb09a45ea52b8ad30f386427dc7497448`  
		Last Modified: Wed, 01 Apr 2020 05:59:14 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:1-alpine`

```console
$ docker pull memcached@sha256:17bd52c925cecb11d9b5e107ec9b9cf81fe2e5326900141f50bf8e8c19bb9ab1
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
$ docker pull memcached@sha256:504421bbf708add1d72e89d605ea3ea63d4b781866405bcfa5446e0172ad16eb
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.4 MB (4371683 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:801fa8ca11ab6a7fd7c3976f966b1a4b804a1f28db61aaf9156e1835dc78c55b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 23 Mar 2020 21:19:34 GMT
ADD file:0c4555f363c2672e350001f1293e689875a3760afe7b3f9146886afe67121cba in / 
# Mon, 23 Mar 2020 21:19:34 GMT
CMD ["/bin/sh"]
# Tue, 24 Mar 2020 00:40:06 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 24 Mar 2020 00:40:07 GMT
RUN apk add --no-cache cyrus-sasl-plain
# Wed, 01 Apr 2020 04:34:39 GMT
ENV MEMCACHED_VERSION=1.6.3
# Wed, 01 Apr 2020 04:34:39 GMT
ENV MEMCACHED_SHA1=bcd6d0c076ca2b62e9bd31f6669acc8563df7db1
# Wed, 01 Apr 2020 04:42:43 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		dpkg-dev dpkg 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		tar 		wget 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& make test 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Wed, 01 Apr 2020 04:42:43 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 01 Apr 2020 04:42:44 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 01 Apr 2020 04:42:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Apr 2020 04:42:45 GMT
USER memcache
# Wed, 01 Apr 2020 04:42:45 GMT
EXPOSE 11211
# Wed, 01 Apr 2020 04:42:45 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:aad63a9339440e7c3e1fff2b988991b9bfb81280042fa7f39a5e327023056819`  
		Last Modified: Mon, 23 Mar 2020 21:19:53 GMT  
		Size: 2.8 MB (2803255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a5fb4ad400df404c486089fa4098e9e6bfdb1528c2ee85cbd5614e8a97f1f9a`  
		Last Modified: Tue, 24 Mar 2020 00:48:55 GMT  
		Size: 1.2 KB (1230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb602a49f6f4777651777faab36b80d92a2f1dbe36d865c0cce4e182439c6b5e`  
		Last Modified: Tue, 24 Mar 2020 00:48:55 GMT  
		Size: 15.1 KB (15099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9170b88a2b9dff1d8fed938f8b1fbed86749b7d29b6208fa1e833c1c5447371`  
		Last Modified: Wed, 01 Apr 2020 04:43:08 GMT  
		Size: 1.6 MB (1551693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c57ce97f5eb3f42443e03945bf4f06e8d666362f8231445fd3d2663b875b45d`  
		Last Modified: Wed, 01 Apr 2020 04:43:08 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d8a359c2a701b1da7a72d2fc7a48c413792eeab01fecc13e555114ec5fefecb`  
		Last Modified: Wed, 01 Apr 2020 04:43:08 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-alpine` - linux; arm variant v6

```console
$ docker pull memcached@sha256:e54f5e55a14b5162d421327cccb9cda48be89d264d9a1f48f5c93a286e69f39f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.1 MB (4148717 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:904fb49ed16723e4d5093b937c02b08e15f7c710350f1e169073dae639179d42`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 23 Mar 2020 21:49:26 GMT
ADD file:e2fdfc637b534345942caf4097883508a5ed23be97d85ccc3357b8277aaa5430 in / 
# Mon, 23 Mar 2020 21:49:27 GMT
CMD ["/bin/sh"]
# Mon, 23 Mar 2020 23:15:28 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Mon, 23 Mar 2020 23:15:34 GMT
RUN apk add --no-cache cyrus-sasl-plain
# Tue, 31 Mar 2020 19:49:46 GMT
ENV MEMCACHED_VERSION=1.6.3
# Tue, 31 Mar 2020 19:49:47 GMT
ENV MEMCACHED_SHA1=bcd6d0c076ca2b62e9bd31f6669acc8563df7db1
# Tue, 31 Mar 2020 19:59:09 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		dpkg-dev dpkg 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		tar 		wget 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& make test 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 31 Mar 2020 19:59:10 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 31 Mar 2020 19:59:13 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 31 Mar 2020 19:59:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 31 Mar 2020 19:59:15 GMT
USER memcache
# Tue, 31 Mar 2020 19:59:15 GMT
EXPOSE 11211
# Tue, 31 Mar 2020 19:59:16 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:0776aeec3430c5a5ba3f43937f0ee6a7770a1fe81a318c9d94cc76512e5375e9`  
		Last Modified: Mon, 23 Mar 2020 21:49:50 GMT  
		Size: 2.6 MB (2618579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f329bb895b7588f4de54c119f39a5f656520bc2310d39893460c4398814112d`  
		Last Modified: Mon, 23 Mar 2020 23:25:38 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6bd8017eeb8ecce1d6b238f86b96a1af52d1a9dd44bc0da4c0573f58a7f51a8`  
		Last Modified: Mon, 23 Mar 2020 23:25:38 GMT  
		Size: 14.7 KB (14695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97a1fc78f0dd1f4d19a9b453400ea3d5bf6515aefe2044cea13a0fbbf7176ab7`  
		Last Modified: Tue, 31 Mar 2020 19:59:29 GMT  
		Size: 1.5 MB (1513779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d36dc6635f5960f1ed529c19648cde5341e1ac518cea270e90f260fe3183ff57`  
		Last Modified: Tue, 31 Mar 2020 19:59:29 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7f6bf3b6679ec09f33841e74c14bb0c5784632df49b25276e5c61960bcd43be`  
		Last Modified: Tue, 31 Mar 2020 19:59:29 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-alpine` - linux; arm variant v7

```console
$ docker pull memcached@sha256:ec8c62ad113b358298092e63b474e8aeebb5b1e1bfabb2e6ff525646dc7458f1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3826282 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5af1281a25c9479c7ad3e80e07f3e7b43e774841795c9f93004bf124abe4b0f4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 23 Mar 2020 21:57:55 GMT
ADD file:3bde6b6fd06efbf24e66446c6d32f72294fc749ae9ee6191776242e92b2f8ab4 in / 
# Mon, 23 Mar 2020 21:57:56 GMT
CMD ["/bin/sh"]
# Mon, 23 Mar 2020 22:14:07 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Mon, 23 Mar 2020 22:14:20 GMT
RUN apk add --no-cache cyrus-sasl-plain
# Tue, 24 Mar 2020 01:47:18 GMT
ENV MEMCACHED_VERSION=1.6.2
# Tue, 24 Mar 2020 01:47:22 GMT
ENV MEMCACHED_SHA1=a6a07f0433adaa13a3cafdf8c26acb640cdd001f
# Tue, 24 Mar 2020 03:19:47 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		dpkg-dev dpkg 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		tar 		wget 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& make test 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 24 Mar 2020 03:19:50 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 24 Mar 2020 03:20:01 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 24 Mar 2020 03:20:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 24 Mar 2020 03:20:05 GMT
USER memcache
# Tue, 24 Mar 2020 03:20:07 GMT
EXPOSE 11211
# Tue, 24 Mar 2020 03:20:09 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:d9bf605ce3d4449f4b90035c3e21d691806324781d43a5287b1da25a01779d6b`  
		Last Modified: Mon, 23 Mar 2020 21:58:16 GMT  
		Size: 2.4 MB (2420493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eae54837c45cf98e10469ba87b255979740486d00d9407bc2fcdf1492469dc04`  
		Last Modified: Mon, 23 Mar 2020 22:42:38 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1459ca388d9e53a94cbb39e64789568710013f3b46396b24ea0729b570f74403`  
		Last Modified: Mon, 23 Mar 2020 22:42:44 GMT  
		Size: 13.6 KB (13638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f84775e4ae618e04e599d46af2006e35d62d9046f4908e660cc533b9cbb8c36`  
		Last Modified: Tue, 24 Mar 2020 03:21:11 GMT  
		Size: 1.4 MB (1390486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dd59b3062e02dcff6cd6cbe35ba1e84c44a571112a65c4dd0ad640b905e4ae3`  
		Last Modified: Tue, 24 Mar 2020 03:21:09 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f53094e3dbce9c8d482bfb7123a06c9a0e4e74102891a4aecc833167acbb64db`  
		Last Modified: Tue, 24 Mar 2020 03:21:15 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-alpine` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:799a51f3fbf3504dee7e5152154ac2ab528b2674eb037b211597b4ed702365e0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.3 MB (4294297 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:60c011071a320179ee9e80babe7d159b06f5f64be786388cca8fa903fd7a6f3a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 23 Mar 2020 21:39:52 GMT
ADD file:746a5c3838a898d6acf7877552ff13d1ab40d0036ace7a662e7c747018315ddb in / 
# Mon, 23 Mar 2020 21:39:53 GMT
CMD ["/bin/sh"]
# Tue, 24 Mar 2020 05:16:12 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 24 Mar 2020 05:16:15 GMT
RUN apk add --no-cache cyrus-sasl-plain
# Wed, 01 Apr 2020 04:54:17 GMT
ENV MEMCACHED_VERSION=1.6.3
# Wed, 01 Apr 2020 04:54:18 GMT
ENV MEMCACHED_SHA1=bcd6d0c076ca2b62e9bd31f6669acc8563df7db1
# Wed, 01 Apr 2020 05:12:17 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		dpkg-dev dpkg 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		tar 		wget 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& make test 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Wed, 01 Apr 2020 05:12:18 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 01 Apr 2020 05:12:20 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 01 Apr 2020 05:12:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Apr 2020 05:12:21 GMT
USER memcache
# Wed, 01 Apr 2020 05:12:21 GMT
EXPOSE 11211
# Wed, 01 Apr 2020 05:12:22 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:8a0637ca1ac98db4cf29f7632449c92801adc80cf0da2cd9c9e39882ce466561`  
		Last Modified: Mon, 23 Mar 2020 21:40:19 GMT  
		Size: 2.7 MB (2723139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd1bfe9c2142f88c6e142b39adf7ba4fe722789b650d5a54184ff336826ae16f`  
		Last Modified: Tue, 24 Mar 2020 05:25:36 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f4d8154a8d6d9edf61516528f99c62d27eb41f8602571ae30fdf745976e2c6e`  
		Last Modified: Tue, 24 Mar 2020 05:25:35 GMT  
		Size: 15.5 KB (15490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7f106af3c2ed3a7290ace796d3928ebace90adf39411884be3a63a0df58c99c`  
		Last Modified: Wed, 01 Apr 2020 05:12:48 GMT  
		Size: 1.6 MB (1554004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ddd0a23420ce85ddf49ae379a74b2adc3afdc6c6f34003263083f8ed39126ab`  
		Last Modified: Wed, 01 Apr 2020 05:12:47 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bac1f8b4b923cdd7efd688cf758bd3e14304ad2bc41d5732d2f73d1b6d65434b`  
		Last Modified: Wed, 01 Apr 2020 05:12:47 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-alpine` - linux; 386

```console
$ docker pull memcached@sha256:d05780d5c31011aff04ebd8af83f27031e669630042d061a6789e57298135010
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4472019 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91afec457abab7b418a13cc0ec15b9b886444899fd1bd6012f8139d6bd71aca8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 23 Mar 2020 21:38:28 GMT
ADD file:99c8234abafd4fa915c0b826eb0e3be0e6aaa7c1e33cb1214ef71a99e9c02e06 in / 
# Mon, 23 Mar 2020 21:38:28 GMT
CMD ["/bin/sh"]
# Tue, 24 Mar 2020 04:55:12 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 24 Mar 2020 04:55:13 GMT
RUN apk add --no-cache cyrus-sasl-plain
# Wed, 01 Apr 2020 00:45:25 GMT
ENV MEMCACHED_VERSION=1.6.3
# Wed, 01 Apr 2020 00:45:26 GMT
ENV MEMCACHED_SHA1=bcd6d0c076ca2b62e9bd31f6669acc8563df7db1
# Wed, 01 Apr 2020 00:54:03 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		dpkg-dev dpkg 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		tar 		wget 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& make test 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Wed, 01 Apr 2020 00:54:04 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 01 Apr 2020 00:54:04 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 01 Apr 2020 00:54:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Apr 2020 00:54:05 GMT
USER memcache
# Wed, 01 Apr 2020 00:54:05 GMT
EXPOSE 11211
# Wed, 01 Apr 2020 00:54:05 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:43f6a4398e1c9e860dfb5c93d7049ab9eedf814513bd6d07e06077c560303c7a`  
		Last Modified: Mon, 23 Mar 2020 21:38:48 GMT  
		Size: 2.8 MB (2806122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a31d073afa8dea3b0bfd6eeb6ebffc6447996f0e9cabebf9d749474ac22cdf2d`  
		Last Modified: Tue, 24 Mar 2020 05:04:58 GMT  
		Size: 1.2 KB (1230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:905909a3db778acdf7295903cff6ee7b27263e33facc5982475e7b60831413fc`  
		Last Modified: Tue, 24 Mar 2020 05:04:58 GMT  
		Size: 16.1 KB (16146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:084fe9c6c267a28b7ef7682ca30611f165ec248e04aa077a2a2d73f4457fabab`  
		Last Modified: Wed, 01 Apr 2020 00:54:25 GMT  
		Size: 1.6 MB (1648120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e913734356dc8bab85686d97ef17baaca409de999cb2b9fabe5ce05705f0e8cc`  
		Last Modified: Wed, 01 Apr 2020 00:54:25 GMT  
		Size: 280.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e4fafb5feec45ada3475ec22c6c9b55762badb826cec0d46db5aafec25b9e3f`  
		Last Modified: Wed, 01 Apr 2020 00:54:25 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-alpine` - linux; ppc64le

```console
$ docker pull memcached@sha256:e39ab357bebea313936e055707ba4ae986ff9f2c9f6884b1f2ef0241a4d03f59
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.4 MB (4448402 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2860d592b00ed82e9bc857eb9cf6873241d6f7d3f1162977a81fee56b5a4c4d8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 23 Mar 2020 21:21:29 GMT
ADD file:4b35131542b9682214e1c2c72fe3cea215a10e2f775e87befecd80fe2228d5a0 in / 
# Mon, 23 Mar 2020 21:21:32 GMT
CMD ["/bin/sh"]
# Tue, 24 Mar 2020 02:24:20 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 24 Mar 2020 02:24:25 GMT
RUN apk add --no-cache cyrus-sasl-plain
# Wed, 01 Apr 2020 05:49:31 GMT
ENV MEMCACHED_VERSION=1.6.3
# Wed, 01 Apr 2020 05:49:35 GMT
ENV MEMCACHED_SHA1=bcd6d0c076ca2b62e9bd31f6669acc8563df7db1
# Wed, 01 Apr 2020 05:58:02 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		dpkg-dev dpkg 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		tar 		wget 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& make test 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Wed, 01 Apr 2020 05:58:03 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 01 Apr 2020 05:58:12 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 01 Apr 2020 05:58:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Apr 2020 05:58:20 GMT
USER memcache
# Wed, 01 Apr 2020 05:58:22 GMT
EXPOSE 11211
# Wed, 01 Apr 2020 05:58:25 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:bc1c99f4ba60de0d3ca52dc6855483e24c91884e33df71f502bbff6eb909d9b9`  
		Last Modified: Mon, 23 Mar 2020 21:22:12 GMT  
		Size: 2.8 MB (2820052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c50bd2ca891d67079878bf06e36ba609e8528e83369265c92fbd3b03e6e839f1`  
		Last Modified: Tue, 24 Mar 2020 02:34:02 GMT  
		Size: 1.3 KB (1263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a4704e4e496c0d18b40f484fc715146c1f427050210b40271112edcf751a698`  
		Last Modified: Tue, 24 Mar 2020 02:34:02 GMT  
		Size: 16.1 KB (16131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10436c8816f1c5f62f5007787e0a21833b186a194f03d364bf347f6e7a587004`  
		Last Modified: Wed, 01 Apr 2020 05:59:14 GMT  
		Size: 1.6 MB (1610549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07449479f271de853b60dfdf76a99142a7c6b26b5e985c6112595bf6d31f54b1`  
		Last Modified: Wed, 01 Apr 2020 05:59:14 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de62a3b128b893893b9888ff271738dbb09a45ea52b8ad30f386427dc7497448`  
		Last Modified: Wed, 01 Apr 2020 05:59:14 GMT  
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
$ docker pull memcached@sha256:17bd52c925cecb11d9b5e107ec9b9cf81fe2e5326900141f50bf8e8c19bb9ab1
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
$ docker pull memcached@sha256:504421bbf708add1d72e89d605ea3ea63d4b781866405bcfa5446e0172ad16eb
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.4 MB (4371683 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:801fa8ca11ab6a7fd7c3976f966b1a4b804a1f28db61aaf9156e1835dc78c55b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 23 Mar 2020 21:19:34 GMT
ADD file:0c4555f363c2672e350001f1293e689875a3760afe7b3f9146886afe67121cba in / 
# Mon, 23 Mar 2020 21:19:34 GMT
CMD ["/bin/sh"]
# Tue, 24 Mar 2020 00:40:06 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 24 Mar 2020 00:40:07 GMT
RUN apk add --no-cache cyrus-sasl-plain
# Wed, 01 Apr 2020 04:34:39 GMT
ENV MEMCACHED_VERSION=1.6.3
# Wed, 01 Apr 2020 04:34:39 GMT
ENV MEMCACHED_SHA1=bcd6d0c076ca2b62e9bd31f6669acc8563df7db1
# Wed, 01 Apr 2020 04:42:43 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		dpkg-dev dpkg 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		tar 		wget 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& make test 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Wed, 01 Apr 2020 04:42:43 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 01 Apr 2020 04:42:44 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 01 Apr 2020 04:42:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Apr 2020 04:42:45 GMT
USER memcache
# Wed, 01 Apr 2020 04:42:45 GMT
EXPOSE 11211
# Wed, 01 Apr 2020 04:42:45 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:aad63a9339440e7c3e1fff2b988991b9bfb81280042fa7f39a5e327023056819`  
		Last Modified: Mon, 23 Mar 2020 21:19:53 GMT  
		Size: 2.8 MB (2803255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a5fb4ad400df404c486089fa4098e9e6bfdb1528c2ee85cbd5614e8a97f1f9a`  
		Last Modified: Tue, 24 Mar 2020 00:48:55 GMT  
		Size: 1.2 KB (1230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb602a49f6f4777651777faab36b80d92a2f1dbe36d865c0cce4e182439c6b5e`  
		Last Modified: Tue, 24 Mar 2020 00:48:55 GMT  
		Size: 15.1 KB (15099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9170b88a2b9dff1d8fed938f8b1fbed86749b7d29b6208fa1e833c1c5447371`  
		Last Modified: Wed, 01 Apr 2020 04:43:08 GMT  
		Size: 1.6 MB (1551693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c57ce97f5eb3f42443e03945bf4f06e8d666362f8231445fd3d2663b875b45d`  
		Last Modified: Wed, 01 Apr 2020 04:43:08 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d8a359c2a701b1da7a72d2fc7a48c413792eeab01fecc13e555114ec5fefecb`  
		Last Modified: Wed, 01 Apr 2020 04:43:08 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:alpine` - linux; arm variant v6

```console
$ docker pull memcached@sha256:e54f5e55a14b5162d421327cccb9cda48be89d264d9a1f48f5c93a286e69f39f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.1 MB (4148717 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:904fb49ed16723e4d5093b937c02b08e15f7c710350f1e169073dae639179d42`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 23 Mar 2020 21:49:26 GMT
ADD file:e2fdfc637b534345942caf4097883508a5ed23be97d85ccc3357b8277aaa5430 in / 
# Mon, 23 Mar 2020 21:49:27 GMT
CMD ["/bin/sh"]
# Mon, 23 Mar 2020 23:15:28 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Mon, 23 Mar 2020 23:15:34 GMT
RUN apk add --no-cache cyrus-sasl-plain
# Tue, 31 Mar 2020 19:49:46 GMT
ENV MEMCACHED_VERSION=1.6.3
# Tue, 31 Mar 2020 19:49:47 GMT
ENV MEMCACHED_SHA1=bcd6d0c076ca2b62e9bd31f6669acc8563df7db1
# Tue, 31 Mar 2020 19:59:09 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		dpkg-dev dpkg 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		tar 		wget 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& make test 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 31 Mar 2020 19:59:10 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 31 Mar 2020 19:59:13 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 31 Mar 2020 19:59:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 31 Mar 2020 19:59:15 GMT
USER memcache
# Tue, 31 Mar 2020 19:59:15 GMT
EXPOSE 11211
# Tue, 31 Mar 2020 19:59:16 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:0776aeec3430c5a5ba3f43937f0ee6a7770a1fe81a318c9d94cc76512e5375e9`  
		Last Modified: Mon, 23 Mar 2020 21:49:50 GMT  
		Size: 2.6 MB (2618579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f329bb895b7588f4de54c119f39a5f656520bc2310d39893460c4398814112d`  
		Last Modified: Mon, 23 Mar 2020 23:25:38 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6bd8017eeb8ecce1d6b238f86b96a1af52d1a9dd44bc0da4c0573f58a7f51a8`  
		Last Modified: Mon, 23 Mar 2020 23:25:38 GMT  
		Size: 14.7 KB (14695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97a1fc78f0dd1f4d19a9b453400ea3d5bf6515aefe2044cea13a0fbbf7176ab7`  
		Last Modified: Tue, 31 Mar 2020 19:59:29 GMT  
		Size: 1.5 MB (1513779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d36dc6635f5960f1ed529c19648cde5341e1ac518cea270e90f260fe3183ff57`  
		Last Modified: Tue, 31 Mar 2020 19:59:29 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7f6bf3b6679ec09f33841e74c14bb0c5784632df49b25276e5c61960bcd43be`  
		Last Modified: Tue, 31 Mar 2020 19:59:29 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:alpine` - linux; arm variant v7

```console
$ docker pull memcached@sha256:ec8c62ad113b358298092e63b474e8aeebb5b1e1bfabb2e6ff525646dc7458f1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3826282 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5af1281a25c9479c7ad3e80e07f3e7b43e774841795c9f93004bf124abe4b0f4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 23 Mar 2020 21:57:55 GMT
ADD file:3bde6b6fd06efbf24e66446c6d32f72294fc749ae9ee6191776242e92b2f8ab4 in / 
# Mon, 23 Mar 2020 21:57:56 GMT
CMD ["/bin/sh"]
# Mon, 23 Mar 2020 22:14:07 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Mon, 23 Mar 2020 22:14:20 GMT
RUN apk add --no-cache cyrus-sasl-plain
# Tue, 24 Mar 2020 01:47:18 GMT
ENV MEMCACHED_VERSION=1.6.2
# Tue, 24 Mar 2020 01:47:22 GMT
ENV MEMCACHED_SHA1=a6a07f0433adaa13a3cafdf8c26acb640cdd001f
# Tue, 24 Mar 2020 03:19:47 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		dpkg-dev dpkg 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		tar 		wget 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& make test 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 24 Mar 2020 03:19:50 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 24 Mar 2020 03:20:01 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 24 Mar 2020 03:20:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 24 Mar 2020 03:20:05 GMT
USER memcache
# Tue, 24 Mar 2020 03:20:07 GMT
EXPOSE 11211
# Tue, 24 Mar 2020 03:20:09 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:d9bf605ce3d4449f4b90035c3e21d691806324781d43a5287b1da25a01779d6b`  
		Last Modified: Mon, 23 Mar 2020 21:58:16 GMT  
		Size: 2.4 MB (2420493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eae54837c45cf98e10469ba87b255979740486d00d9407bc2fcdf1492469dc04`  
		Last Modified: Mon, 23 Mar 2020 22:42:38 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1459ca388d9e53a94cbb39e64789568710013f3b46396b24ea0729b570f74403`  
		Last Modified: Mon, 23 Mar 2020 22:42:44 GMT  
		Size: 13.6 KB (13638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f84775e4ae618e04e599d46af2006e35d62d9046f4908e660cc533b9cbb8c36`  
		Last Modified: Tue, 24 Mar 2020 03:21:11 GMT  
		Size: 1.4 MB (1390486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dd59b3062e02dcff6cd6cbe35ba1e84c44a571112a65c4dd0ad640b905e4ae3`  
		Last Modified: Tue, 24 Mar 2020 03:21:09 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f53094e3dbce9c8d482bfb7123a06c9a0e4e74102891a4aecc833167acbb64db`  
		Last Modified: Tue, 24 Mar 2020 03:21:15 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:alpine` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:799a51f3fbf3504dee7e5152154ac2ab528b2674eb037b211597b4ed702365e0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.3 MB (4294297 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:60c011071a320179ee9e80babe7d159b06f5f64be786388cca8fa903fd7a6f3a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 23 Mar 2020 21:39:52 GMT
ADD file:746a5c3838a898d6acf7877552ff13d1ab40d0036ace7a662e7c747018315ddb in / 
# Mon, 23 Mar 2020 21:39:53 GMT
CMD ["/bin/sh"]
# Tue, 24 Mar 2020 05:16:12 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 24 Mar 2020 05:16:15 GMT
RUN apk add --no-cache cyrus-sasl-plain
# Wed, 01 Apr 2020 04:54:17 GMT
ENV MEMCACHED_VERSION=1.6.3
# Wed, 01 Apr 2020 04:54:18 GMT
ENV MEMCACHED_SHA1=bcd6d0c076ca2b62e9bd31f6669acc8563df7db1
# Wed, 01 Apr 2020 05:12:17 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		dpkg-dev dpkg 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		tar 		wget 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& make test 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Wed, 01 Apr 2020 05:12:18 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 01 Apr 2020 05:12:20 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 01 Apr 2020 05:12:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Apr 2020 05:12:21 GMT
USER memcache
# Wed, 01 Apr 2020 05:12:21 GMT
EXPOSE 11211
# Wed, 01 Apr 2020 05:12:22 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:8a0637ca1ac98db4cf29f7632449c92801adc80cf0da2cd9c9e39882ce466561`  
		Last Modified: Mon, 23 Mar 2020 21:40:19 GMT  
		Size: 2.7 MB (2723139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd1bfe9c2142f88c6e142b39adf7ba4fe722789b650d5a54184ff336826ae16f`  
		Last Modified: Tue, 24 Mar 2020 05:25:36 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f4d8154a8d6d9edf61516528f99c62d27eb41f8602571ae30fdf745976e2c6e`  
		Last Modified: Tue, 24 Mar 2020 05:25:35 GMT  
		Size: 15.5 KB (15490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7f106af3c2ed3a7290ace796d3928ebace90adf39411884be3a63a0df58c99c`  
		Last Modified: Wed, 01 Apr 2020 05:12:48 GMT  
		Size: 1.6 MB (1554004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ddd0a23420ce85ddf49ae379a74b2adc3afdc6c6f34003263083f8ed39126ab`  
		Last Modified: Wed, 01 Apr 2020 05:12:47 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bac1f8b4b923cdd7efd688cf758bd3e14304ad2bc41d5732d2f73d1b6d65434b`  
		Last Modified: Wed, 01 Apr 2020 05:12:47 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:alpine` - linux; 386

```console
$ docker pull memcached@sha256:d05780d5c31011aff04ebd8af83f27031e669630042d061a6789e57298135010
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4472019 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91afec457abab7b418a13cc0ec15b9b886444899fd1bd6012f8139d6bd71aca8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 23 Mar 2020 21:38:28 GMT
ADD file:99c8234abafd4fa915c0b826eb0e3be0e6aaa7c1e33cb1214ef71a99e9c02e06 in / 
# Mon, 23 Mar 2020 21:38:28 GMT
CMD ["/bin/sh"]
# Tue, 24 Mar 2020 04:55:12 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 24 Mar 2020 04:55:13 GMT
RUN apk add --no-cache cyrus-sasl-plain
# Wed, 01 Apr 2020 00:45:25 GMT
ENV MEMCACHED_VERSION=1.6.3
# Wed, 01 Apr 2020 00:45:26 GMT
ENV MEMCACHED_SHA1=bcd6d0c076ca2b62e9bd31f6669acc8563df7db1
# Wed, 01 Apr 2020 00:54:03 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		dpkg-dev dpkg 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		tar 		wget 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& make test 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Wed, 01 Apr 2020 00:54:04 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 01 Apr 2020 00:54:04 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 01 Apr 2020 00:54:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Apr 2020 00:54:05 GMT
USER memcache
# Wed, 01 Apr 2020 00:54:05 GMT
EXPOSE 11211
# Wed, 01 Apr 2020 00:54:05 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:43f6a4398e1c9e860dfb5c93d7049ab9eedf814513bd6d07e06077c560303c7a`  
		Last Modified: Mon, 23 Mar 2020 21:38:48 GMT  
		Size: 2.8 MB (2806122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a31d073afa8dea3b0bfd6eeb6ebffc6447996f0e9cabebf9d749474ac22cdf2d`  
		Last Modified: Tue, 24 Mar 2020 05:04:58 GMT  
		Size: 1.2 KB (1230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:905909a3db778acdf7295903cff6ee7b27263e33facc5982475e7b60831413fc`  
		Last Modified: Tue, 24 Mar 2020 05:04:58 GMT  
		Size: 16.1 KB (16146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:084fe9c6c267a28b7ef7682ca30611f165ec248e04aa077a2a2d73f4457fabab`  
		Last Modified: Wed, 01 Apr 2020 00:54:25 GMT  
		Size: 1.6 MB (1648120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e913734356dc8bab85686d97ef17baaca409de999cb2b9fabe5ce05705f0e8cc`  
		Last Modified: Wed, 01 Apr 2020 00:54:25 GMT  
		Size: 280.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e4fafb5feec45ada3475ec22c6c9b55762badb826cec0d46db5aafec25b9e3f`  
		Last Modified: Wed, 01 Apr 2020 00:54:25 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:alpine` - linux; ppc64le

```console
$ docker pull memcached@sha256:e39ab357bebea313936e055707ba4ae986ff9f2c9f6884b1f2ef0241a4d03f59
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.4 MB (4448402 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2860d592b00ed82e9bc857eb9cf6873241d6f7d3f1162977a81fee56b5a4c4d8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 23 Mar 2020 21:21:29 GMT
ADD file:4b35131542b9682214e1c2c72fe3cea215a10e2f775e87befecd80fe2228d5a0 in / 
# Mon, 23 Mar 2020 21:21:32 GMT
CMD ["/bin/sh"]
# Tue, 24 Mar 2020 02:24:20 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 24 Mar 2020 02:24:25 GMT
RUN apk add --no-cache cyrus-sasl-plain
# Wed, 01 Apr 2020 05:49:31 GMT
ENV MEMCACHED_VERSION=1.6.3
# Wed, 01 Apr 2020 05:49:35 GMT
ENV MEMCACHED_SHA1=bcd6d0c076ca2b62e9bd31f6669acc8563df7db1
# Wed, 01 Apr 2020 05:58:02 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		dpkg-dev dpkg 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		tar 		wget 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& make test 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Wed, 01 Apr 2020 05:58:03 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 01 Apr 2020 05:58:12 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 01 Apr 2020 05:58:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Apr 2020 05:58:20 GMT
USER memcache
# Wed, 01 Apr 2020 05:58:22 GMT
EXPOSE 11211
# Wed, 01 Apr 2020 05:58:25 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:bc1c99f4ba60de0d3ca52dc6855483e24c91884e33df71f502bbff6eb909d9b9`  
		Last Modified: Mon, 23 Mar 2020 21:22:12 GMT  
		Size: 2.8 MB (2820052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c50bd2ca891d67079878bf06e36ba609e8528e83369265c92fbd3b03e6e839f1`  
		Last Modified: Tue, 24 Mar 2020 02:34:02 GMT  
		Size: 1.3 KB (1263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a4704e4e496c0d18b40f484fc715146c1f427050210b40271112edcf751a698`  
		Last Modified: Tue, 24 Mar 2020 02:34:02 GMT  
		Size: 16.1 KB (16131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10436c8816f1c5f62f5007787e0a21833b186a194f03d364bf347f6e7a587004`  
		Last Modified: Wed, 01 Apr 2020 05:59:14 GMT  
		Size: 1.6 MB (1610549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07449479f271de853b60dfdf76a99142a7c6b26b5e985c6112595bf6d31f54b1`  
		Last Modified: Wed, 01 Apr 2020 05:59:14 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de62a3b128b893893b9888ff271738dbb09a45ea52b8ad30f386427dc7497448`  
		Last Modified: Wed, 01 Apr 2020 05:59:14 GMT  
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
$ docker pull memcached@sha256:7d02e468382d4e2c54574f18088eb0127979fa135f6aa55f96e94185b7166215
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
$ docker pull memcached@sha256:6bdc214f60e191847cf0f57721aba4ba68cc3357eb38fc8ea31e935c350c5e0c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.5 MB (30485763 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ac3dd24663f48d13eca8fc54d99547759af3dace518eaff1dc413120737ece5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 31 Mar 2020 01:21:01 GMT
ADD file:d1f1b387a158136fb0f8096c8a8ecf5fc146be4e85c1c3c345d44c927692723a in / 
# Tue, 31 Mar 2020 01:21:01 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 13:20:36 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 31 Mar 2020 13:20:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Apr 2020 04:26:20 GMT
ENV MEMCACHED_VERSION=1.6.3
# Wed, 01 Apr 2020 04:26:20 GMT
ENV MEMCACHED_SHA1=bcd6d0c076ca2b62e9bd31f6669acc8563df7db1
# Wed, 01 Apr 2020 04:34:30 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 01 Apr 2020 04:34:30 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 01 Apr 2020 04:34:31 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 01 Apr 2020 04:34:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Apr 2020 04:34:31 GMT
USER memcache
# Wed, 01 Apr 2020 04:34:32 GMT
EXPOSE 11211
# Wed, 01 Apr 2020 04:34:32 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:c499e6d256d6d4a546f1c141e04b5b4951983ba7581e39deaf5cc595289ee70f`  
		Last Modified: Tue, 31 Mar 2020 01:26:37 GMT  
		Size: 27.1 MB (27091862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:512f277e1da84b0b9319530d40c48750bb22b13f4816d103040d20c0635c28be`  
		Last Modified: Tue, 31 Mar 2020 13:29:52 GMT  
		Size: 5.0 KB (4984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdda69e165e26c667ba223dc215274101c3c6e41db182bd651aadf5e5623fc35`  
		Last Modified: Tue, 31 Mar 2020 13:29:53 GMT  
		Size: 2.2 MB (2196476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43b37ee911063bfa8e0a60293b8ba301a22c3b29e26bf39c33f017e1b4bef28e`  
		Last Modified: Wed, 01 Apr 2020 04:43:03 GMT  
		Size: 1.2 MB (1192033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b83bd7ea262edefd8fa75ce5e40145b491e787de8d3806265e986a60cad606e0`  
		Last Modified: Wed, 01 Apr 2020 04:43:03 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc4fa7c552bc03701653c81434f6e3f7312745deb0c26e039e7565acca70ea54`  
		Last Modified: Wed, 01 Apr 2020 04:43:03 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:latest` - linux; arm variant v5

```console
$ docker pull memcached@sha256:aa492daa963294573d6319a6a19d392cce213240b81078dba65869e538611c97
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.9 MB (27889314 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c0ec6623b84d3061e2fa7dab933f5e39cc8c9b170bbf6fd5ce0b4baf35341c30`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 31 Mar 2020 01:24:54 GMT
ADD file:e08ed9e60228d351de400af5746474777a562d99f17e0cb1ce3e3d352e9ec751 in / 
# Tue, 31 Mar 2020 01:24:56 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 01:54:28 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 31 Mar 2020 01:55:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Mar 2020 19:48:28 GMT
ENV MEMCACHED_VERSION=1.6.3
# Tue, 31 Mar 2020 19:48:30 GMT
ENV MEMCACHED_SHA1=bcd6d0c076ca2b62e9bd31f6669acc8563df7db1
# Tue, 31 Mar 2020 20:49:40 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 31 Mar 2020 20:49:43 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 31 Mar 2020 20:49:54 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 31 Mar 2020 20:49:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 31 Mar 2020 20:49:58 GMT
USER memcache
# Tue, 31 Mar 2020 20:50:00 GMT
EXPOSE 11211
# Tue, 31 Mar 2020 20:50:02 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:440df189aa3df85587f2d7d348500930481b3752dcb887d212de9b44b49076dd`  
		Last Modified: Tue, 31 Mar 2020 01:33:04 GMT  
		Size: 24.8 MB (24830324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bde8351817341fa2fec288d97635ede228892bbb58fc5c6ca54441acef6f0766`  
		Last Modified: Tue, 31 Mar 2020 03:24:42 GMT  
		Size: 4.9 KB (4896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b011e5f13bdf6608cafa62557b3c877e4794590eaadced0b8a49fe24a28d110`  
		Last Modified: Tue, 31 Mar 2020 03:24:44 GMT  
		Size: 1.9 MB (1896786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d15532e44d1b4cbd93a29d2f59e8d316aac3697819e686b863a04b7306f66e97`  
		Last Modified: Tue, 31 Mar 2020 20:50:23 GMT  
		Size: 1.2 MB (1156899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51aa0f21d752e0ddd5092569a00faade9a48585be4787ea0915d3bcd56ee1de5`  
		Last Modified: Tue, 31 Mar 2020 20:50:27 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e86f84b137f1eb137ff83d27d7cff6eee693a6dab12d7ce99ff0c2a77a49b6ae`  
		Last Modified: Tue, 31 Mar 2020 20:50:28 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:latest` - linux; arm variant v7

```console
$ docker pull memcached@sha256:d54eb37ba24eeb017adff9ad74f97c71f8232153c291be63893eb6ade8836656
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.6 MB (25646260 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0d8ee9533c9e5e31033a1bc594eeac7543678ca190a7b66d654a6b5385f8e5a7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 31 Mar 2020 01:48:12 GMT
ADD file:8c3ed0df404a6bcaf7583e71796cb4c1f40e87288953a21d4ee5946079c3274f in / 
# Tue, 31 Mar 2020 01:48:13 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 03:27:08 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 31 Mar 2020 03:28:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Mar 2020 20:51:09 GMT
ENV MEMCACHED_VERSION=1.6.3
# Tue, 31 Mar 2020 20:51:11 GMT
ENV MEMCACHED_SHA1=bcd6d0c076ca2b62e9bd31f6669acc8563df7db1
# Tue, 31 Mar 2020 21:21:03 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 31 Mar 2020 21:21:07 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 31 Mar 2020 21:21:18 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 31 Mar 2020 21:21:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 31 Mar 2020 21:21:22 GMT
USER memcache
# Tue, 31 Mar 2020 21:21:24 GMT
EXPOSE 11211
# Tue, 31 Mar 2020 21:21:26 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:98098fa10651fdba12c848231b7428536a120e17637f1f9e0d25c63880483fcc`  
		Last Modified: Tue, 31 Mar 2020 01:56:24 GMT  
		Size: 22.7 MB (22699731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a7a42e48b851419bcd11506631a8d336fb394d979dcea8feb4830f38ba7cfd7`  
		Last Modified: Tue, 31 Mar 2020 04:39:27 GMT  
		Size: 4.9 KB (4899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc96c4fde110b7a8691d85cf0523cd326fbfd1bcbf928719f6173cd292c91305`  
		Last Modified: Tue, 31 Mar 2020 04:39:35 GMT  
		Size: 1.8 MB (1811551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2a043ecd402e02473caef2834dd90c40a3a16ee899cb87574bf7fb8b1183adb`  
		Last Modified: Tue, 31 Mar 2020 23:12:26 GMT  
		Size: 1.1 MB (1129671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6b3946960ee59ded096d4489e81d9cd3af3506ce6f99c79f38648217430a2f0`  
		Last Modified: Tue, 31 Mar 2020 23:12:24 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34b5c1dda6f0d125b29798f04589e1f46502983dbe8f4cf5763a2a2592148191`  
		Last Modified: Tue, 31 Mar 2020 23:12:30 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:latest` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:056b511f1e97a6619c24aadc781560db65e25abc0c3a98bbe25b52d81b24e78c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.1 MB (29094504 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:142fbd99d85857a0807b95f6c5621c5006b38c522d78f4f8e088fdd6a4061db8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 31 Mar 2020 02:05:33 GMT
ADD file:47ab456123ae97a527249191ff2bc0014e7ef0ae186aec91bf6a63eb077ecb91 in / 
# Tue, 31 Mar 2020 02:05:35 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 08:39:07 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 31 Mar 2020 08:39:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Apr 2020 04:44:54 GMT
ENV MEMCACHED_VERSION=1.6.3
# Wed, 01 Apr 2020 04:44:55 GMT
ENV MEMCACHED_SHA1=bcd6d0c076ca2b62e9bd31f6669acc8563df7db1
# Wed, 01 Apr 2020 04:54:03 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 01 Apr 2020 04:54:05 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 01 Apr 2020 04:54:07 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 01 Apr 2020 04:54:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Apr 2020 04:54:08 GMT
USER memcache
# Wed, 01 Apr 2020 04:54:08 GMT
EXPOSE 11211
# Wed, 01 Apr 2020 04:54:09 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:a6c32b8bc1ce2b374630673ded1d5ef5a98936d045bf0632fcf599dc2229d493`  
		Last Modified: Tue, 31 Mar 2020 02:12:15 GMT  
		Size: 25.9 MB (25851645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72560398e0dc8991a53cd07c580b14e3c2024d7af30d2dfe8428d913006af5a9`  
		Last Modified: Tue, 31 Mar 2020 08:48:55 GMT  
		Size: 5.0 KB (5028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4febdbdc3565b2d569ed0a6885c548a5755cd9a2b52c21b351d254c83e6fff7`  
		Last Modified: Tue, 31 Mar 2020 08:48:55 GMT  
		Size: 2.1 MB (2074952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b1797ec4dd007a4f822abca922aa457a793f2ba04b4481e6c1f0de7e34b32d8`  
		Last Modified: Wed, 01 Apr 2020 05:12:38 GMT  
		Size: 1.2 MB (1162471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b9601a34125cd3cfe733ea2ce11005afc0ec6f02bd14b34d5d5ce92a9dadb1c`  
		Last Modified: Wed, 01 Apr 2020 05:12:39 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:703422421b84c80f0ed9b79b040ba35dbf37e06c80b5e9681455202c1b2091f6`  
		Last Modified: Wed, 01 Apr 2020 05:12:38 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:latest` - linux; 386

```console
$ docker pull memcached@sha256:45e70e58745f9b65a1fdbea626d26be12194087fa3f2ebc06647d23dd8ff4dd3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.2 MB (31156562 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7371335c883334e01e87c4a4b5cf189b8b2876ff43cd38604954befcf0afc780`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 31 Mar 2020 00:39:42 GMT
ADD file:a453117866661af4ddfa21203d65ce6661efeaeca2a1704e09747c83b4c58e47 in / 
# Tue, 31 Mar 2020 00:39:42 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 11:45:29 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 31 Mar 2020 11:45:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Apr 2020 00:36:05 GMT
ENV MEMCACHED_VERSION=1.6.3
# Wed, 01 Apr 2020 00:36:06 GMT
ENV MEMCACHED_SHA1=bcd6d0c076ca2b62e9bd31f6669acc8563df7db1
# Wed, 01 Apr 2020 00:45:06 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 01 Apr 2020 00:45:06 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 01 Apr 2020 00:45:08 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 01 Apr 2020 00:45:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Apr 2020 00:45:09 GMT
USER memcache
# Wed, 01 Apr 2020 00:45:09 GMT
EXPOSE 11211
# Wed, 01 Apr 2020 00:45:10 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:2314106a15e49c7908bebb2c697dcaf3d6a1626b70fe72bc0c0cb71eb216ddc3`  
		Last Modified: Tue, 31 Mar 2020 00:45:31 GMT  
		Size: 27.7 MB (27747648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3bafab0976764495dda52d0c16addb4770d62d8f9de55728b752ff3448f2292`  
		Last Modified: Tue, 31 Mar 2020 11:55:29 GMT  
		Size: 4.9 KB (4899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8307e5e61ebc9ed2430c9e45ba3437aa1deebed0882ce15c36616e0debf28b36`  
		Last Modified: Tue, 31 Mar 2020 11:55:29 GMT  
		Size: 2.2 MB (2208079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2346314e755e47f2a21140be69437185fef4416c21871e9bea2504e4011aa31c`  
		Last Modified: Wed, 01 Apr 2020 00:54:20 GMT  
		Size: 1.2 MB (1195528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04f73e333f816b2d2fa26694d21c4c50e393e11ecbe6c172966071f7a5c60a31`  
		Last Modified: Wed, 01 Apr 2020 00:54:20 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:882932b666818b8fc239f2047d12a409ec5f211424e6321a671aabd98da708bc`  
		Last Modified: Wed, 01 Apr 2020 00:54:20 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:latest` - linux; ppc64le

```console
$ docker pull memcached@sha256:9d4d92103d08915f9f79003636917f96ee58591cf3fc4bf22c5331ee582ea6d1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.1 MB (34064010 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:296aceabbfb0b475275d0104ab416027cdcb9ac9c53140cb7791a505e2a8ff70`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 31 Mar 2020 01:32:42 GMT
ADD file:36c02e92574faba45b64cfed78a0a0359d65ad175b17128bf554a2a5c0086ff5 in / 
# Tue, 31 Mar 2020 01:32:47 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 12:45:58 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 31 Mar 2020 12:46:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Apr 2020 05:38:36 GMT
ENV MEMCACHED_VERSION=1.6.3
# Wed, 01 Apr 2020 05:38:38 GMT
ENV MEMCACHED_SHA1=bcd6d0c076ca2b62e9bd31f6669acc8563df7db1
# Wed, 01 Apr 2020 05:48:45 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 01 Apr 2020 05:48:47 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 01 Apr 2020 05:48:55 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 01 Apr 2020 05:49:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Apr 2020 05:49:05 GMT
USER memcache
# Wed, 01 Apr 2020 05:49:09 GMT
EXPOSE 11211
# Wed, 01 Apr 2020 05:49:14 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:9df6bbae5eeb29e9aac2f39cff517c694cce60f01ee477abcdedcd8e8c01c38f`  
		Last Modified: Tue, 31 Mar 2020 01:45:59 GMT  
		Size: 30.5 MB (30518493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2786c1a6fbad6e8c56e4f7e33b4d41c64efd06c4cdb303a50c07ee1f4c5f7a69`  
		Last Modified: Tue, 31 Mar 2020 12:58:00 GMT  
		Size: 5.0 KB (4987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:722cfb50c03533f4b5c83c84a2f565dbcdbf63c01460ae91d35aafacd94454fe`  
		Last Modified: Tue, 31 Mar 2020 12:58:00 GMT  
		Size: 2.3 MB (2322647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7e848dce4e6fd08decef8fe4b047462a693bef7d0e19a1b08a71731d057769a`  
		Last Modified: Wed, 01 Apr 2020 05:58:55 GMT  
		Size: 1.2 MB (1217474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6b9f0c55a9cb31a1fe9245e8b6fd7289e71e07b1cde1a80fd6aa8636933e374`  
		Last Modified: Wed, 01 Apr 2020 05:58:54 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e3672877c4fc4ef3ec6151c6b363981966fa03e2cfbae0ba80f168670103a2a`  
		Last Modified: Wed, 01 Apr 2020 05:58:55 GMT  
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
