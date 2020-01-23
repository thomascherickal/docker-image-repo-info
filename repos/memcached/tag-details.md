<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `memcached`

-	[`memcached:1`](#memcached1)
-	[`memcached:1.5`](#memcached15)
-	[`memcached:1.5.20`](#memcached1520)
-	[`memcached:1.5.20-alpine`](#memcached1520-alpine)
-	[`memcached:1.5-alpine`](#memcached15-alpine)
-	[`memcached:1-alpine`](#memcached1-alpine)
-	[`memcached:alpine`](#memcachedalpine)
-	[`memcached:latest`](#memcachedlatest)

## `memcached:1`

```console
$ docker pull memcached@sha256:2f561d372672bedc970880d64ac0444f877bda1b1605c0bfd4baf4f20fb4c343
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
$ docker pull memcached@sha256:850e5421b841d813966f5e210ff8758fe4d085efef463fb847282af59ca32546
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.5 MB (30474381 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b32d3ed7da92b981b892dff6b378374f7331a44f31e8d2f9533d5d92dba62171`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Sat, 28 Dec 2019 04:21:22 GMT
ADD file:04caaf303199c81ff1a94e2e39d5096f9d02b73294b82758e5bc6e23aff94272 in / 
# Sat, 28 Dec 2019 04:21:23 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 13:58:49 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Sat, 28 Dec 2019 13:58:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 13:58:55 GMT
ENV MEMCACHED_VERSION=1.5.20
# Sat, 28 Dec 2019 13:58:55 GMT
ENV MEMCACHED_SHA1=5d3b5af3ce0a1483d655017db7228bcaeff10d47
# Sat, 28 Dec 2019 14:06:59 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Sat, 28 Dec 2019 14:07:00 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Sat, 28 Dec 2019 14:07:01 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Sat, 28 Dec 2019 14:07:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 28 Dec 2019 14:07:01 GMT
USER memcache
# Sat, 28 Dec 2019 14:07:01 GMT
EXPOSE 11211
# Sat, 28 Dec 2019 14:07:02 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:8ec398bc03560e0fa56440e96da307cdf0b1ad153f459b52bca53ae7ddb8236d`  
		Last Modified: Sat, 28 Dec 2019 04:25:53 GMT  
		Size: 27.1 MB (27092274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60e10c2aa199f4392bf1ddbfa150c6839c390eb66d1774c68eddacd8c11b8642`  
		Last Modified: Sat, 28 Dec 2019 14:07:19 GMT  
		Size: 5.0 KB (4980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:288dc9f908106487c0bad762aaa118ac1198279015f1d5440c3139be04ed7f2f`  
		Last Modified: Sat, 28 Dec 2019 14:07:20 GMT  
		Size: 2.2 MB (2196480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a244ab9e1e9de308e7c856704ec0378f73f5f996f979eaad845ac3f1a49f86bc`  
		Last Modified: Sat, 28 Dec 2019 14:07:20 GMT  
		Size: 1.2 MB (1180238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9db86ad11ed8bbffd528085a0ddb67ac989b020992ffd4c0032b263ee7dad22a`  
		Last Modified: Sat, 28 Dec 2019 14:07:19 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:356f3b62ef2b4bd1cf49aa61dbbe1f11643c2f85f62cbe081e4d7de8d8f39ff2`  
		Last Modified: Sat, 28 Dec 2019 14:07:19 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1` - linux; arm variant v5

```console
$ docker pull memcached@sha256:62ccc1796a81315fcbb198c87cb07d58578fba2a105e6ecf52116b5cc1b3cb58
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.9 MB (27874841 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c09d14e5d8cab36aa360bb194317306af61877c397472ba60fd53b4fe1c20c7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 22 Nov 2019 12:13:54 GMT
ADD file:94ed554e445cf749e10644dfa0d836103c120a6ea388bf6dc9f18f7c6b2f095a in / 
# Fri, 22 Nov 2019 12:13:56 GMT
CMD ["bash"]
# Fri, 22 Nov 2019 12:44:01 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Fri, 22 Nov 2019 12:45:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Nov 2019 12:45:25 GMT
ENV MEMCACHED_VERSION=1.5.20
# Fri, 22 Nov 2019 12:45:26 GMT
ENV MEMCACHED_SHA1=5d3b5af3ce0a1483d655017db7228bcaeff10d47
# Wed, 11 Dec 2019 01:15:09 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 11 Dec 2019 01:15:12 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 11 Dec 2019 01:15:22 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 11 Dec 2019 01:15:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 Dec 2019 01:15:25 GMT
USER memcache
# Wed, 11 Dec 2019 01:15:27 GMT
EXPOSE 11211
# Wed, 11 Dec 2019 01:15:28 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:45ae7e8aa5bfd9e1b0db11d7fa5a56a8af11b69fc56707d763f89aa2c61b7e8f`  
		Last Modified: Fri, 22 Nov 2019 12:22:20 GMT  
		Size: 24.8 MB (24829480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7abfa51b826ab2a750aacd0ca0db5eca44bd315eebc7100f88cdaaba729433ee`  
		Last Modified: Wed, 11 Dec 2019 01:15:54 GMT  
		Size: 4.9 KB (4898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22b994f77a11fb8adc23b3e9263cc757d84ddf5528b1352d8bdb638ee9318747`  
		Last Modified: Wed, 11 Dec 2019 01:15:57 GMT  
		Size: 1.9 MB (1896875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f47c6f9dfd6813351ceaddc6807dbb4f5c53bdd8405f4642bf0b0c97ada6279`  
		Last Modified: Wed, 11 Dec 2019 01:15:56 GMT  
		Size: 1.1 MB (1143179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:957ac1f455448be6a6d88a76911ae99cf5148ddb776613c6634f7f641c223db8`  
		Last Modified: Wed, 11 Dec 2019 01:15:54 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04dab8c47bbee2c7ef5a52817e160cd9ef97368f73d41f1423320924bf025467`  
		Last Modified: Wed, 11 Dec 2019 01:15:54 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1` - linux; arm variant v7

```console
$ docker pull memcached@sha256:e680132321a0e3a9373f3f40206cedcdaf2667aaa29b64650ce029d756a1971d
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.6 MB (25621613 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e6ae16ecc7ca54d8e4edbc4cacb7d11f1984818935ceaaee7bc287c4176b93e2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 17 Oct 2019 00:05:51 GMT
ADD file:aec8ae5d1bd3bffdcab55efc79e947f802af8efa4266cc074679cc305949f7b9 in / 
# Thu, 17 Oct 2019 00:05:55 GMT
CMD ["bash"]
# Thu, 17 Oct 2019 01:11:52 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Thu, 17 Oct 2019 01:12:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 13 Nov 2019 22:58:06 GMT
ENV MEMCACHED_VERSION=1.5.20
# Wed, 13 Nov 2019 22:58:07 GMT
ENV MEMCACHED_SHA1=5d3b5af3ce0a1483d655017db7228bcaeff10d47
# Thu, 14 Nov 2019 22:35:28 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libsasl2-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		$enableExtstore 	&& make -j "$(nproc)" 		&& make test 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 14 Nov 2019 22:35:31 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 14 Nov 2019 22:35:42 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 14 Nov 2019 22:35:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 14 Nov 2019 22:35:45 GMT
USER memcache
# Thu, 14 Nov 2019 22:35:46 GMT
EXPOSE 11211
# Thu, 14 Nov 2019 22:35:48 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:ffb3a1edd2f5d689daee77b16634ddec87a4f724ac3bbef287c397ea731af2ac`  
		Last Modified: Thu, 17 Oct 2019 00:15:00 GMT  
		Size: 22.7 MB (22711906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcf6d2564d271d74fae4672d14f92fcbe87ead7e1298e8915908de657ab8e5c3`  
		Last Modified: Thu, 14 Nov 2019 22:36:15 GMT  
		Size: 4.9 KB (4891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:109decf50675f59a1197b904e45765ee2fd2056f02aec9d04196b007bfb911d4`  
		Last Modified: Thu, 14 Nov 2019 22:36:18 GMT  
		Size: 1.8 MB (1811613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae8ec6f57a9302a06ef868ed6c3811c6e03d109fa28a5bfdd295111d128eab77`  
		Last Modified: Thu, 14 Nov 2019 22:36:16 GMT  
		Size: 1.1 MB (1092796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59288dbdc770325d3abf8e56283deb225dab1c9ada4503ffa3457077c6d52bef`  
		Last Modified: Thu, 14 Nov 2019 22:36:15 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68a7926932d9f3025d519c57860153bf9ff247f787ade2f50b94b483828878b8`  
		Last Modified: Thu, 14 Nov 2019 22:36:15 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:dfd1cdee25d29bf6e12665a09451649f477ba08ef6d95fdb43211a4b364e8228
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.1 MB (29076734 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:94a900befbdf811a79a52b4b2d3c54fbc579986fa21168096939b7e5f8f77eb1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Sat, 28 Dec 2019 04:41:08 GMT
ADD file:b45fd612576b682e93ab91addbc4387a6609ace4bc092e5b615323964bba33c3 in / 
# Sat, 28 Dec 2019 04:41:11 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 09:26:00 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Sat, 28 Dec 2019 09:26:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 09:26:11 GMT
ENV MEMCACHED_VERSION=1.5.20
# Sat, 28 Dec 2019 09:26:12 GMT
ENV MEMCACHED_SHA1=5d3b5af3ce0a1483d655017db7228bcaeff10d47
# Sat, 28 Dec 2019 09:34:56 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Sat, 28 Dec 2019 09:34:57 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Sat, 28 Dec 2019 09:34:59 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Sat, 28 Dec 2019 09:35:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 28 Dec 2019 09:35:01 GMT
USER memcache
# Sat, 28 Dec 2019 09:35:02 GMT
EXPOSE 11211
# Sat, 28 Dec 2019 09:35:02 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:fb62b7c746da1f79992359282f2d8b7f93da8c48dc138ec6b2a36130efd42635`  
		Last Modified: Sat, 28 Dec 2019 04:46:58 GMT  
		Size: 25.9 MB (25850702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b07d5eaa7d9c3d15b1121c61ab46c1765a21a82bce1dd1e376d2ecf09865928`  
		Last Modified: Sat, 28 Dec 2019 09:35:37 GMT  
		Size: 5.0 KB (5029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ea19e96eb15c540f804c57bd35c31b3a8137b38c15e8f31fd26a93422e4c5bb`  
		Last Modified: Sat, 28 Dec 2019 09:35:37 GMT  
		Size: 2.1 MB (2074929 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f5fb8100575d7dac36d76ca7c3a506210dc9a25cfa5aa974ee0e1420fd62c19`  
		Last Modified: Sat, 28 Dec 2019 09:35:37 GMT  
		Size: 1.1 MB (1145667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:734ac2f49087d47d7a139a37e1b9dc10afd8aff2ad495cdcc9949658f6bc6845`  
		Last Modified: Sat, 28 Dec 2019 09:35:36 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cd59d3ba33a5d9b9eedb4d229178fddb6e8a12fdbbc5a976364bbd3faf6cb52`  
		Last Modified: Sat, 28 Dec 2019 09:35:36 GMT  
		Size: 120.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1` - linux; 386

```console
$ docker pull memcached@sha256:0f8ee210458e9c6d6662477682ae70695caa17b36de73d06a659620bc7bb919f
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.1 MB (31140927 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0199eb106fa984cf5f81efb1bb8c68c546b9fe108349a022f7a8ac7bfa1ab357`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Sat, 28 Dec 2019 04:39:35 GMT
ADD file:447f0758c9f5653f03d964e54a38c18f24cf4c43e05fc38e7a76aebd6d6bafa8 in / 
# Sat, 28 Dec 2019 04:39:35 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 15:01:45 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Sat, 28 Dec 2019 15:01:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 15:01:51 GMT
ENV MEMCACHED_VERSION=1.5.20
# Sat, 28 Dec 2019 15:01:51 GMT
ENV MEMCACHED_SHA1=5d3b5af3ce0a1483d655017db7228bcaeff10d47
# Sat, 28 Dec 2019 15:10:18 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Sat, 28 Dec 2019 15:10:19 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Sat, 28 Dec 2019 15:10:20 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Sat, 28 Dec 2019 15:10:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 28 Dec 2019 15:10:20 GMT
USER memcache
# Sat, 28 Dec 2019 15:10:21 GMT
EXPOSE 11211
# Sat, 28 Dec 2019 15:10:21 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:5536417213b9f46f2118943c1151912954d6077afe03a32e68521774cc358095`  
		Last Modified: Sat, 28 Dec 2019 04:44:24 GMT  
		Size: 27.7 MB (27747020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f952840b6779a17e1998bfb1e145d53747c667708443e724483989c54a63ee4`  
		Last Modified: Sat, 28 Dec 2019 15:10:44 GMT  
		Size: 4.9 KB (4896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a656e047a0d4ae15c61be416063049cdb41f91945f6159a14e71aca03b6efa0`  
		Last Modified: Sat, 28 Dec 2019 15:10:45 GMT  
		Size: 2.2 MB (2208081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a53ed12be1a50e398a859c745767c1d6aff64b16b1ac35487dfc6c4b2f5055e6`  
		Last Modified: Sat, 28 Dec 2019 15:10:45 GMT  
		Size: 1.2 MB (1180520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efe3d9a88c4bc05a24a9f780eacb3c159d64e3dd03cae5246de72e523d748706`  
		Last Modified: Sat, 28 Dec 2019 15:10:44 GMT  
		Size: 289.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5c516b8df5a22933466c3edea0e576a2f0c7bb325a1197d6e67dc33cedbef29`  
		Last Modified: Sat, 28 Dec 2019 15:10:44 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1` - linux; ppc64le

```console
$ docker pull memcached@sha256:feb8e81074da9abdb0cbcad6c65c24453a318f0e0a342c558e3046ab3a7911b3
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.0 MB (34046630 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8eb752b8385ac8444ce410843f8b46f5674d023be19f9e65c8f7ec8b1d5c9152`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Sat, 28 Dec 2019 04:20:39 GMT
ADD file:abec4f3d6a54bb0725560d826d07e99da3d6b582433c6dd95605626c67d7c2d6 in / 
# Sat, 28 Dec 2019 04:20:43 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 13:00:10 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Sat, 28 Dec 2019 13:00:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 13:00:25 GMT
ENV MEMCACHED_VERSION=1.5.20
# Sat, 28 Dec 2019 13:00:27 GMT
ENV MEMCACHED_SHA1=5d3b5af3ce0a1483d655017db7228bcaeff10d47
# Sat, 28 Dec 2019 13:09:37 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Sat, 28 Dec 2019 13:09:38 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Sat, 28 Dec 2019 13:09:41 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Sat, 28 Dec 2019 13:09:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 28 Dec 2019 13:09:45 GMT
USER memcache
# Sat, 28 Dec 2019 13:09:48 GMT
EXPOSE 11211
# Sat, 28 Dec 2019 13:09:51 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:37e6f4d596ea5c3cc92914bd95508a4192c8834c4edaff414734885929b07800`  
		Last Modified: Sat, 28 Dec 2019 04:28:05 GMT  
		Size: 30.5 MB (30517529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7537865582bff5727f1fb50d0cf11718db483efcd8716843fd29e410fb78ed0`  
		Last Modified: Sat, 28 Dec 2019 13:10:14 GMT  
		Size: 5.0 KB (4984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fb3e2d1d77f48e789fa0cce495a195d95d150ffec8e78572548a08a1f3fad14`  
		Last Modified: Sat, 28 Dec 2019 13:10:15 GMT  
		Size: 2.3 MB (2322686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a8b268f98197e3ec2bf2013e77fa416602cc296241528892dce9b192492eca3`  
		Last Modified: Sat, 28 Dec 2019 13:10:14 GMT  
		Size: 1.2 MB (1201022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e4c8a7095e41fca0197a8eaae09593a3d239a078dcdf8d867c382e6bdabe392`  
		Last Modified: Sat, 28 Dec 2019 13:10:14 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c73af1c8cf2cea3e6dc53ba3a3a3253bbe7d931c663d600f51a1d844e26fc2f`  
		Last Modified: Sat, 28 Dec 2019 13:10:14 GMT  
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

## `memcached:1.5`

```console
$ docker pull memcached@sha256:2f561d372672bedc970880d64ac0444f877bda1b1605c0bfd4baf4f20fb4c343
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

### `memcached:1.5` - linux; amd64

```console
$ docker pull memcached@sha256:850e5421b841d813966f5e210ff8758fe4d085efef463fb847282af59ca32546
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.5 MB (30474381 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b32d3ed7da92b981b892dff6b378374f7331a44f31e8d2f9533d5d92dba62171`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Sat, 28 Dec 2019 04:21:22 GMT
ADD file:04caaf303199c81ff1a94e2e39d5096f9d02b73294b82758e5bc6e23aff94272 in / 
# Sat, 28 Dec 2019 04:21:23 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 13:58:49 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Sat, 28 Dec 2019 13:58:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 13:58:55 GMT
ENV MEMCACHED_VERSION=1.5.20
# Sat, 28 Dec 2019 13:58:55 GMT
ENV MEMCACHED_SHA1=5d3b5af3ce0a1483d655017db7228bcaeff10d47
# Sat, 28 Dec 2019 14:06:59 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Sat, 28 Dec 2019 14:07:00 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Sat, 28 Dec 2019 14:07:01 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Sat, 28 Dec 2019 14:07:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 28 Dec 2019 14:07:01 GMT
USER memcache
# Sat, 28 Dec 2019 14:07:01 GMT
EXPOSE 11211
# Sat, 28 Dec 2019 14:07:02 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:8ec398bc03560e0fa56440e96da307cdf0b1ad153f459b52bca53ae7ddb8236d`  
		Last Modified: Sat, 28 Dec 2019 04:25:53 GMT  
		Size: 27.1 MB (27092274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60e10c2aa199f4392bf1ddbfa150c6839c390eb66d1774c68eddacd8c11b8642`  
		Last Modified: Sat, 28 Dec 2019 14:07:19 GMT  
		Size: 5.0 KB (4980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:288dc9f908106487c0bad762aaa118ac1198279015f1d5440c3139be04ed7f2f`  
		Last Modified: Sat, 28 Dec 2019 14:07:20 GMT  
		Size: 2.2 MB (2196480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a244ab9e1e9de308e7c856704ec0378f73f5f996f979eaad845ac3f1a49f86bc`  
		Last Modified: Sat, 28 Dec 2019 14:07:20 GMT  
		Size: 1.2 MB (1180238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9db86ad11ed8bbffd528085a0ddb67ac989b020992ffd4c0032b263ee7dad22a`  
		Last Modified: Sat, 28 Dec 2019 14:07:19 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:356f3b62ef2b4bd1cf49aa61dbbe1f11643c2f85f62cbe081e4d7de8d8f39ff2`  
		Last Modified: Sat, 28 Dec 2019 14:07:19 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.5` - linux; arm variant v5

```console
$ docker pull memcached@sha256:62ccc1796a81315fcbb198c87cb07d58578fba2a105e6ecf52116b5cc1b3cb58
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.9 MB (27874841 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c09d14e5d8cab36aa360bb194317306af61877c397472ba60fd53b4fe1c20c7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 22 Nov 2019 12:13:54 GMT
ADD file:94ed554e445cf749e10644dfa0d836103c120a6ea388bf6dc9f18f7c6b2f095a in / 
# Fri, 22 Nov 2019 12:13:56 GMT
CMD ["bash"]
# Fri, 22 Nov 2019 12:44:01 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Fri, 22 Nov 2019 12:45:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Nov 2019 12:45:25 GMT
ENV MEMCACHED_VERSION=1.5.20
# Fri, 22 Nov 2019 12:45:26 GMT
ENV MEMCACHED_SHA1=5d3b5af3ce0a1483d655017db7228bcaeff10d47
# Wed, 11 Dec 2019 01:15:09 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 11 Dec 2019 01:15:12 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 11 Dec 2019 01:15:22 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 11 Dec 2019 01:15:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 Dec 2019 01:15:25 GMT
USER memcache
# Wed, 11 Dec 2019 01:15:27 GMT
EXPOSE 11211
# Wed, 11 Dec 2019 01:15:28 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:45ae7e8aa5bfd9e1b0db11d7fa5a56a8af11b69fc56707d763f89aa2c61b7e8f`  
		Last Modified: Fri, 22 Nov 2019 12:22:20 GMT  
		Size: 24.8 MB (24829480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7abfa51b826ab2a750aacd0ca0db5eca44bd315eebc7100f88cdaaba729433ee`  
		Last Modified: Wed, 11 Dec 2019 01:15:54 GMT  
		Size: 4.9 KB (4898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22b994f77a11fb8adc23b3e9263cc757d84ddf5528b1352d8bdb638ee9318747`  
		Last Modified: Wed, 11 Dec 2019 01:15:57 GMT  
		Size: 1.9 MB (1896875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f47c6f9dfd6813351ceaddc6807dbb4f5c53bdd8405f4642bf0b0c97ada6279`  
		Last Modified: Wed, 11 Dec 2019 01:15:56 GMT  
		Size: 1.1 MB (1143179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:957ac1f455448be6a6d88a76911ae99cf5148ddb776613c6634f7f641c223db8`  
		Last Modified: Wed, 11 Dec 2019 01:15:54 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04dab8c47bbee2c7ef5a52817e160cd9ef97368f73d41f1423320924bf025467`  
		Last Modified: Wed, 11 Dec 2019 01:15:54 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.5` - linux; arm variant v7

```console
$ docker pull memcached@sha256:e680132321a0e3a9373f3f40206cedcdaf2667aaa29b64650ce029d756a1971d
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.6 MB (25621613 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e6ae16ecc7ca54d8e4edbc4cacb7d11f1984818935ceaaee7bc287c4176b93e2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 17 Oct 2019 00:05:51 GMT
ADD file:aec8ae5d1bd3bffdcab55efc79e947f802af8efa4266cc074679cc305949f7b9 in / 
# Thu, 17 Oct 2019 00:05:55 GMT
CMD ["bash"]
# Thu, 17 Oct 2019 01:11:52 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Thu, 17 Oct 2019 01:12:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 13 Nov 2019 22:58:06 GMT
ENV MEMCACHED_VERSION=1.5.20
# Wed, 13 Nov 2019 22:58:07 GMT
ENV MEMCACHED_SHA1=5d3b5af3ce0a1483d655017db7228bcaeff10d47
# Thu, 14 Nov 2019 22:35:28 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libsasl2-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		$enableExtstore 	&& make -j "$(nproc)" 		&& make test 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 14 Nov 2019 22:35:31 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 14 Nov 2019 22:35:42 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 14 Nov 2019 22:35:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 14 Nov 2019 22:35:45 GMT
USER memcache
# Thu, 14 Nov 2019 22:35:46 GMT
EXPOSE 11211
# Thu, 14 Nov 2019 22:35:48 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:ffb3a1edd2f5d689daee77b16634ddec87a4f724ac3bbef287c397ea731af2ac`  
		Last Modified: Thu, 17 Oct 2019 00:15:00 GMT  
		Size: 22.7 MB (22711906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcf6d2564d271d74fae4672d14f92fcbe87ead7e1298e8915908de657ab8e5c3`  
		Last Modified: Thu, 14 Nov 2019 22:36:15 GMT  
		Size: 4.9 KB (4891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:109decf50675f59a1197b904e45765ee2fd2056f02aec9d04196b007bfb911d4`  
		Last Modified: Thu, 14 Nov 2019 22:36:18 GMT  
		Size: 1.8 MB (1811613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae8ec6f57a9302a06ef868ed6c3811c6e03d109fa28a5bfdd295111d128eab77`  
		Last Modified: Thu, 14 Nov 2019 22:36:16 GMT  
		Size: 1.1 MB (1092796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59288dbdc770325d3abf8e56283deb225dab1c9ada4503ffa3457077c6d52bef`  
		Last Modified: Thu, 14 Nov 2019 22:36:15 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68a7926932d9f3025d519c57860153bf9ff247f787ade2f50b94b483828878b8`  
		Last Modified: Thu, 14 Nov 2019 22:36:15 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.5` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:dfd1cdee25d29bf6e12665a09451649f477ba08ef6d95fdb43211a4b364e8228
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.1 MB (29076734 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:94a900befbdf811a79a52b4b2d3c54fbc579986fa21168096939b7e5f8f77eb1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Sat, 28 Dec 2019 04:41:08 GMT
ADD file:b45fd612576b682e93ab91addbc4387a6609ace4bc092e5b615323964bba33c3 in / 
# Sat, 28 Dec 2019 04:41:11 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 09:26:00 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Sat, 28 Dec 2019 09:26:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 09:26:11 GMT
ENV MEMCACHED_VERSION=1.5.20
# Sat, 28 Dec 2019 09:26:12 GMT
ENV MEMCACHED_SHA1=5d3b5af3ce0a1483d655017db7228bcaeff10d47
# Sat, 28 Dec 2019 09:34:56 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Sat, 28 Dec 2019 09:34:57 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Sat, 28 Dec 2019 09:34:59 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Sat, 28 Dec 2019 09:35:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 28 Dec 2019 09:35:01 GMT
USER memcache
# Sat, 28 Dec 2019 09:35:02 GMT
EXPOSE 11211
# Sat, 28 Dec 2019 09:35:02 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:fb62b7c746da1f79992359282f2d8b7f93da8c48dc138ec6b2a36130efd42635`  
		Last Modified: Sat, 28 Dec 2019 04:46:58 GMT  
		Size: 25.9 MB (25850702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b07d5eaa7d9c3d15b1121c61ab46c1765a21a82bce1dd1e376d2ecf09865928`  
		Last Modified: Sat, 28 Dec 2019 09:35:37 GMT  
		Size: 5.0 KB (5029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ea19e96eb15c540f804c57bd35c31b3a8137b38c15e8f31fd26a93422e4c5bb`  
		Last Modified: Sat, 28 Dec 2019 09:35:37 GMT  
		Size: 2.1 MB (2074929 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f5fb8100575d7dac36d76ca7c3a506210dc9a25cfa5aa974ee0e1420fd62c19`  
		Last Modified: Sat, 28 Dec 2019 09:35:37 GMT  
		Size: 1.1 MB (1145667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:734ac2f49087d47d7a139a37e1b9dc10afd8aff2ad495cdcc9949658f6bc6845`  
		Last Modified: Sat, 28 Dec 2019 09:35:36 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cd59d3ba33a5d9b9eedb4d229178fddb6e8a12fdbbc5a976364bbd3faf6cb52`  
		Last Modified: Sat, 28 Dec 2019 09:35:36 GMT  
		Size: 120.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.5` - linux; 386

```console
$ docker pull memcached@sha256:0f8ee210458e9c6d6662477682ae70695caa17b36de73d06a659620bc7bb919f
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.1 MB (31140927 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0199eb106fa984cf5f81efb1bb8c68c546b9fe108349a022f7a8ac7bfa1ab357`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Sat, 28 Dec 2019 04:39:35 GMT
ADD file:447f0758c9f5653f03d964e54a38c18f24cf4c43e05fc38e7a76aebd6d6bafa8 in / 
# Sat, 28 Dec 2019 04:39:35 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 15:01:45 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Sat, 28 Dec 2019 15:01:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 15:01:51 GMT
ENV MEMCACHED_VERSION=1.5.20
# Sat, 28 Dec 2019 15:01:51 GMT
ENV MEMCACHED_SHA1=5d3b5af3ce0a1483d655017db7228bcaeff10d47
# Sat, 28 Dec 2019 15:10:18 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Sat, 28 Dec 2019 15:10:19 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Sat, 28 Dec 2019 15:10:20 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Sat, 28 Dec 2019 15:10:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 28 Dec 2019 15:10:20 GMT
USER memcache
# Sat, 28 Dec 2019 15:10:21 GMT
EXPOSE 11211
# Sat, 28 Dec 2019 15:10:21 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:5536417213b9f46f2118943c1151912954d6077afe03a32e68521774cc358095`  
		Last Modified: Sat, 28 Dec 2019 04:44:24 GMT  
		Size: 27.7 MB (27747020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f952840b6779a17e1998bfb1e145d53747c667708443e724483989c54a63ee4`  
		Last Modified: Sat, 28 Dec 2019 15:10:44 GMT  
		Size: 4.9 KB (4896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a656e047a0d4ae15c61be416063049cdb41f91945f6159a14e71aca03b6efa0`  
		Last Modified: Sat, 28 Dec 2019 15:10:45 GMT  
		Size: 2.2 MB (2208081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a53ed12be1a50e398a859c745767c1d6aff64b16b1ac35487dfc6c4b2f5055e6`  
		Last Modified: Sat, 28 Dec 2019 15:10:45 GMT  
		Size: 1.2 MB (1180520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efe3d9a88c4bc05a24a9f780eacb3c159d64e3dd03cae5246de72e523d748706`  
		Last Modified: Sat, 28 Dec 2019 15:10:44 GMT  
		Size: 289.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5c516b8df5a22933466c3edea0e576a2f0c7bb325a1197d6e67dc33cedbef29`  
		Last Modified: Sat, 28 Dec 2019 15:10:44 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.5` - linux; ppc64le

```console
$ docker pull memcached@sha256:feb8e81074da9abdb0cbcad6c65c24453a318f0e0a342c558e3046ab3a7911b3
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.0 MB (34046630 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8eb752b8385ac8444ce410843f8b46f5674d023be19f9e65c8f7ec8b1d5c9152`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Sat, 28 Dec 2019 04:20:39 GMT
ADD file:abec4f3d6a54bb0725560d826d07e99da3d6b582433c6dd95605626c67d7c2d6 in / 
# Sat, 28 Dec 2019 04:20:43 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 13:00:10 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Sat, 28 Dec 2019 13:00:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 13:00:25 GMT
ENV MEMCACHED_VERSION=1.5.20
# Sat, 28 Dec 2019 13:00:27 GMT
ENV MEMCACHED_SHA1=5d3b5af3ce0a1483d655017db7228bcaeff10d47
# Sat, 28 Dec 2019 13:09:37 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Sat, 28 Dec 2019 13:09:38 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Sat, 28 Dec 2019 13:09:41 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Sat, 28 Dec 2019 13:09:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 28 Dec 2019 13:09:45 GMT
USER memcache
# Sat, 28 Dec 2019 13:09:48 GMT
EXPOSE 11211
# Sat, 28 Dec 2019 13:09:51 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:37e6f4d596ea5c3cc92914bd95508a4192c8834c4edaff414734885929b07800`  
		Last Modified: Sat, 28 Dec 2019 04:28:05 GMT  
		Size: 30.5 MB (30517529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7537865582bff5727f1fb50d0cf11718db483efcd8716843fd29e410fb78ed0`  
		Last Modified: Sat, 28 Dec 2019 13:10:14 GMT  
		Size: 5.0 KB (4984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fb3e2d1d77f48e789fa0cce495a195d95d150ffec8e78572548a08a1f3fad14`  
		Last Modified: Sat, 28 Dec 2019 13:10:15 GMT  
		Size: 2.3 MB (2322686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a8b268f98197e3ec2bf2013e77fa416602cc296241528892dce9b192492eca3`  
		Last Modified: Sat, 28 Dec 2019 13:10:14 GMT  
		Size: 1.2 MB (1201022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e4c8a7095e41fca0197a8eaae09593a3d239a078dcdf8d867c382e6bdabe392`  
		Last Modified: Sat, 28 Dec 2019 13:10:14 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c73af1c8cf2cea3e6dc53ba3a3a3253bbe7d931c663d600f51a1d844e26fc2f`  
		Last Modified: Sat, 28 Dec 2019 13:10:14 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.5` - linux; s390x

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

## `memcached:1.5.20`

```console
$ docker pull memcached@sha256:2f561d372672bedc970880d64ac0444f877bda1b1605c0bfd4baf4f20fb4c343
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

### `memcached:1.5.20` - linux; amd64

```console
$ docker pull memcached@sha256:850e5421b841d813966f5e210ff8758fe4d085efef463fb847282af59ca32546
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.5 MB (30474381 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b32d3ed7da92b981b892dff6b378374f7331a44f31e8d2f9533d5d92dba62171`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Sat, 28 Dec 2019 04:21:22 GMT
ADD file:04caaf303199c81ff1a94e2e39d5096f9d02b73294b82758e5bc6e23aff94272 in / 
# Sat, 28 Dec 2019 04:21:23 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 13:58:49 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Sat, 28 Dec 2019 13:58:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 13:58:55 GMT
ENV MEMCACHED_VERSION=1.5.20
# Sat, 28 Dec 2019 13:58:55 GMT
ENV MEMCACHED_SHA1=5d3b5af3ce0a1483d655017db7228bcaeff10d47
# Sat, 28 Dec 2019 14:06:59 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Sat, 28 Dec 2019 14:07:00 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Sat, 28 Dec 2019 14:07:01 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Sat, 28 Dec 2019 14:07:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 28 Dec 2019 14:07:01 GMT
USER memcache
# Sat, 28 Dec 2019 14:07:01 GMT
EXPOSE 11211
# Sat, 28 Dec 2019 14:07:02 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:8ec398bc03560e0fa56440e96da307cdf0b1ad153f459b52bca53ae7ddb8236d`  
		Last Modified: Sat, 28 Dec 2019 04:25:53 GMT  
		Size: 27.1 MB (27092274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60e10c2aa199f4392bf1ddbfa150c6839c390eb66d1774c68eddacd8c11b8642`  
		Last Modified: Sat, 28 Dec 2019 14:07:19 GMT  
		Size: 5.0 KB (4980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:288dc9f908106487c0bad762aaa118ac1198279015f1d5440c3139be04ed7f2f`  
		Last Modified: Sat, 28 Dec 2019 14:07:20 GMT  
		Size: 2.2 MB (2196480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a244ab9e1e9de308e7c856704ec0378f73f5f996f979eaad845ac3f1a49f86bc`  
		Last Modified: Sat, 28 Dec 2019 14:07:20 GMT  
		Size: 1.2 MB (1180238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9db86ad11ed8bbffd528085a0ddb67ac989b020992ffd4c0032b263ee7dad22a`  
		Last Modified: Sat, 28 Dec 2019 14:07:19 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:356f3b62ef2b4bd1cf49aa61dbbe1f11643c2f85f62cbe081e4d7de8d8f39ff2`  
		Last Modified: Sat, 28 Dec 2019 14:07:19 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.5.20` - linux; arm variant v5

```console
$ docker pull memcached@sha256:62ccc1796a81315fcbb198c87cb07d58578fba2a105e6ecf52116b5cc1b3cb58
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.9 MB (27874841 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c09d14e5d8cab36aa360bb194317306af61877c397472ba60fd53b4fe1c20c7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 22 Nov 2019 12:13:54 GMT
ADD file:94ed554e445cf749e10644dfa0d836103c120a6ea388bf6dc9f18f7c6b2f095a in / 
# Fri, 22 Nov 2019 12:13:56 GMT
CMD ["bash"]
# Fri, 22 Nov 2019 12:44:01 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Fri, 22 Nov 2019 12:45:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Nov 2019 12:45:25 GMT
ENV MEMCACHED_VERSION=1.5.20
# Fri, 22 Nov 2019 12:45:26 GMT
ENV MEMCACHED_SHA1=5d3b5af3ce0a1483d655017db7228bcaeff10d47
# Wed, 11 Dec 2019 01:15:09 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 11 Dec 2019 01:15:12 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 11 Dec 2019 01:15:22 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 11 Dec 2019 01:15:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 Dec 2019 01:15:25 GMT
USER memcache
# Wed, 11 Dec 2019 01:15:27 GMT
EXPOSE 11211
# Wed, 11 Dec 2019 01:15:28 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:45ae7e8aa5bfd9e1b0db11d7fa5a56a8af11b69fc56707d763f89aa2c61b7e8f`  
		Last Modified: Fri, 22 Nov 2019 12:22:20 GMT  
		Size: 24.8 MB (24829480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7abfa51b826ab2a750aacd0ca0db5eca44bd315eebc7100f88cdaaba729433ee`  
		Last Modified: Wed, 11 Dec 2019 01:15:54 GMT  
		Size: 4.9 KB (4898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22b994f77a11fb8adc23b3e9263cc757d84ddf5528b1352d8bdb638ee9318747`  
		Last Modified: Wed, 11 Dec 2019 01:15:57 GMT  
		Size: 1.9 MB (1896875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f47c6f9dfd6813351ceaddc6807dbb4f5c53bdd8405f4642bf0b0c97ada6279`  
		Last Modified: Wed, 11 Dec 2019 01:15:56 GMT  
		Size: 1.1 MB (1143179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:957ac1f455448be6a6d88a76911ae99cf5148ddb776613c6634f7f641c223db8`  
		Last Modified: Wed, 11 Dec 2019 01:15:54 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04dab8c47bbee2c7ef5a52817e160cd9ef97368f73d41f1423320924bf025467`  
		Last Modified: Wed, 11 Dec 2019 01:15:54 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.5.20` - linux; arm variant v7

```console
$ docker pull memcached@sha256:e680132321a0e3a9373f3f40206cedcdaf2667aaa29b64650ce029d756a1971d
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.6 MB (25621613 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e6ae16ecc7ca54d8e4edbc4cacb7d11f1984818935ceaaee7bc287c4176b93e2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 17 Oct 2019 00:05:51 GMT
ADD file:aec8ae5d1bd3bffdcab55efc79e947f802af8efa4266cc074679cc305949f7b9 in / 
# Thu, 17 Oct 2019 00:05:55 GMT
CMD ["bash"]
# Thu, 17 Oct 2019 01:11:52 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Thu, 17 Oct 2019 01:12:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 13 Nov 2019 22:58:06 GMT
ENV MEMCACHED_VERSION=1.5.20
# Wed, 13 Nov 2019 22:58:07 GMT
ENV MEMCACHED_SHA1=5d3b5af3ce0a1483d655017db7228bcaeff10d47
# Thu, 14 Nov 2019 22:35:28 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libsasl2-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		$enableExtstore 	&& make -j "$(nproc)" 		&& make test 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 14 Nov 2019 22:35:31 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 14 Nov 2019 22:35:42 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 14 Nov 2019 22:35:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 14 Nov 2019 22:35:45 GMT
USER memcache
# Thu, 14 Nov 2019 22:35:46 GMT
EXPOSE 11211
# Thu, 14 Nov 2019 22:35:48 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:ffb3a1edd2f5d689daee77b16634ddec87a4f724ac3bbef287c397ea731af2ac`  
		Last Modified: Thu, 17 Oct 2019 00:15:00 GMT  
		Size: 22.7 MB (22711906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcf6d2564d271d74fae4672d14f92fcbe87ead7e1298e8915908de657ab8e5c3`  
		Last Modified: Thu, 14 Nov 2019 22:36:15 GMT  
		Size: 4.9 KB (4891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:109decf50675f59a1197b904e45765ee2fd2056f02aec9d04196b007bfb911d4`  
		Last Modified: Thu, 14 Nov 2019 22:36:18 GMT  
		Size: 1.8 MB (1811613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae8ec6f57a9302a06ef868ed6c3811c6e03d109fa28a5bfdd295111d128eab77`  
		Last Modified: Thu, 14 Nov 2019 22:36:16 GMT  
		Size: 1.1 MB (1092796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59288dbdc770325d3abf8e56283deb225dab1c9ada4503ffa3457077c6d52bef`  
		Last Modified: Thu, 14 Nov 2019 22:36:15 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68a7926932d9f3025d519c57860153bf9ff247f787ade2f50b94b483828878b8`  
		Last Modified: Thu, 14 Nov 2019 22:36:15 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.5.20` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:dfd1cdee25d29bf6e12665a09451649f477ba08ef6d95fdb43211a4b364e8228
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.1 MB (29076734 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:94a900befbdf811a79a52b4b2d3c54fbc579986fa21168096939b7e5f8f77eb1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Sat, 28 Dec 2019 04:41:08 GMT
ADD file:b45fd612576b682e93ab91addbc4387a6609ace4bc092e5b615323964bba33c3 in / 
# Sat, 28 Dec 2019 04:41:11 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 09:26:00 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Sat, 28 Dec 2019 09:26:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 09:26:11 GMT
ENV MEMCACHED_VERSION=1.5.20
# Sat, 28 Dec 2019 09:26:12 GMT
ENV MEMCACHED_SHA1=5d3b5af3ce0a1483d655017db7228bcaeff10d47
# Sat, 28 Dec 2019 09:34:56 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Sat, 28 Dec 2019 09:34:57 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Sat, 28 Dec 2019 09:34:59 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Sat, 28 Dec 2019 09:35:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 28 Dec 2019 09:35:01 GMT
USER memcache
# Sat, 28 Dec 2019 09:35:02 GMT
EXPOSE 11211
# Sat, 28 Dec 2019 09:35:02 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:fb62b7c746da1f79992359282f2d8b7f93da8c48dc138ec6b2a36130efd42635`  
		Last Modified: Sat, 28 Dec 2019 04:46:58 GMT  
		Size: 25.9 MB (25850702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b07d5eaa7d9c3d15b1121c61ab46c1765a21a82bce1dd1e376d2ecf09865928`  
		Last Modified: Sat, 28 Dec 2019 09:35:37 GMT  
		Size: 5.0 KB (5029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ea19e96eb15c540f804c57bd35c31b3a8137b38c15e8f31fd26a93422e4c5bb`  
		Last Modified: Sat, 28 Dec 2019 09:35:37 GMT  
		Size: 2.1 MB (2074929 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f5fb8100575d7dac36d76ca7c3a506210dc9a25cfa5aa974ee0e1420fd62c19`  
		Last Modified: Sat, 28 Dec 2019 09:35:37 GMT  
		Size: 1.1 MB (1145667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:734ac2f49087d47d7a139a37e1b9dc10afd8aff2ad495cdcc9949658f6bc6845`  
		Last Modified: Sat, 28 Dec 2019 09:35:36 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cd59d3ba33a5d9b9eedb4d229178fddb6e8a12fdbbc5a976364bbd3faf6cb52`  
		Last Modified: Sat, 28 Dec 2019 09:35:36 GMT  
		Size: 120.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.5.20` - linux; 386

```console
$ docker pull memcached@sha256:0f8ee210458e9c6d6662477682ae70695caa17b36de73d06a659620bc7bb919f
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.1 MB (31140927 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0199eb106fa984cf5f81efb1bb8c68c546b9fe108349a022f7a8ac7bfa1ab357`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Sat, 28 Dec 2019 04:39:35 GMT
ADD file:447f0758c9f5653f03d964e54a38c18f24cf4c43e05fc38e7a76aebd6d6bafa8 in / 
# Sat, 28 Dec 2019 04:39:35 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 15:01:45 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Sat, 28 Dec 2019 15:01:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 15:01:51 GMT
ENV MEMCACHED_VERSION=1.5.20
# Sat, 28 Dec 2019 15:01:51 GMT
ENV MEMCACHED_SHA1=5d3b5af3ce0a1483d655017db7228bcaeff10d47
# Sat, 28 Dec 2019 15:10:18 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Sat, 28 Dec 2019 15:10:19 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Sat, 28 Dec 2019 15:10:20 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Sat, 28 Dec 2019 15:10:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 28 Dec 2019 15:10:20 GMT
USER memcache
# Sat, 28 Dec 2019 15:10:21 GMT
EXPOSE 11211
# Sat, 28 Dec 2019 15:10:21 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:5536417213b9f46f2118943c1151912954d6077afe03a32e68521774cc358095`  
		Last Modified: Sat, 28 Dec 2019 04:44:24 GMT  
		Size: 27.7 MB (27747020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f952840b6779a17e1998bfb1e145d53747c667708443e724483989c54a63ee4`  
		Last Modified: Sat, 28 Dec 2019 15:10:44 GMT  
		Size: 4.9 KB (4896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a656e047a0d4ae15c61be416063049cdb41f91945f6159a14e71aca03b6efa0`  
		Last Modified: Sat, 28 Dec 2019 15:10:45 GMT  
		Size: 2.2 MB (2208081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a53ed12be1a50e398a859c745767c1d6aff64b16b1ac35487dfc6c4b2f5055e6`  
		Last Modified: Sat, 28 Dec 2019 15:10:45 GMT  
		Size: 1.2 MB (1180520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efe3d9a88c4bc05a24a9f780eacb3c159d64e3dd03cae5246de72e523d748706`  
		Last Modified: Sat, 28 Dec 2019 15:10:44 GMT  
		Size: 289.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5c516b8df5a22933466c3edea0e576a2f0c7bb325a1197d6e67dc33cedbef29`  
		Last Modified: Sat, 28 Dec 2019 15:10:44 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.5.20` - linux; ppc64le

```console
$ docker pull memcached@sha256:feb8e81074da9abdb0cbcad6c65c24453a318f0e0a342c558e3046ab3a7911b3
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.0 MB (34046630 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8eb752b8385ac8444ce410843f8b46f5674d023be19f9e65c8f7ec8b1d5c9152`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Sat, 28 Dec 2019 04:20:39 GMT
ADD file:abec4f3d6a54bb0725560d826d07e99da3d6b582433c6dd95605626c67d7c2d6 in / 
# Sat, 28 Dec 2019 04:20:43 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 13:00:10 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Sat, 28 Dec 2019 13:00:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 13:00:25 GMT
ENV MEMCACHED_VERSION=1.5.20
# Sat, 28 Dec 2019 13:00:27 GMT
ENV MEMCACHED_SHA1=5d3b5af3ce0a1483d655017db7228bcaeff10d47
# Sat, 28 Dec 2019 13:09:37 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Sat, 28 Dec 2019 13:09:38 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Sat, 28 Dec 2019 13:09:41 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Sat, 28 Dec 2019 13:09:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 28 Dec 2019 13:09:45 GMT
USER memcache
# Sat, 28 Dec 2019 13:09:48 GMT
EXPOSE 11211
# Sat, 28 Dec 2019 13:09:51 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:37e6f4d596ea5c3cc92914bd95508a4192c8834c4edaff414734885929b07800`  
		Last Modified: Sat, 28 Dec 2019 04:28:05 GMT  
		Size: 30.5 MB (30517529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7537865582bff5727f1fb50d0cf11718db483efcd8716843fd29e410fb78ed0`  
		Last Modified: Sat, 28 Dec 2019 13:10:14 GMT  
		Size: 5.0 KB (4984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fb3e2d1d77f48e789fa0cce495a195d95d150ffec8e78572548a08a1f3fad14`  
		Last Modified: Sat, 28 Dec 2019 13:10:15 GMT  
		Size: 2.3 MB (2322686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a8b268f98197e3ec2bf2013e77fa416602cc296241528892dce9b192492eca3`  
		Last Modified: Sat, 28 Dec 2019 13:10:14 GMT  
		Size: 1.2 MB (1201022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e4c8a7095e41fca0197a8eaae09593a3d239a078dcdf8d867c382e6bdabe392`  
		Last Modified: Sat, 28 Dec 2019 13:10:14 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c73af1c8cf2cea3e6dc53ba3a3a3253bbe7d931c663d600f51a1d844e26fc2f`  
		Last Modified: Sat, 28 Dec 2019 13:10:14 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.5.20` - linux; s390x

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

## `memcached:1.5.20-alpine`

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

### `memcached:1.5.20-alpine` - linux; amd64

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

### `memcached:1.5.20-alpine` - linux; arm variant v6

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

### `memcached:1.5.20-alpine` - linux; arm variant v7

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

### `memcached:1.5.20-alpine` - linux; arm64 variant v8

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

### `memcached:1.5.20-alpine` - linux; 386

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

### `memcached:1.5.20-alpine` - linux; ppc64le

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

### `memcached:1.5.20-alpine` - linux; s390x

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

## `memcached:1.5-alpine`

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

### `memcached:1.5-alpine` - linux; amd64

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

### `memcached:1.5-alpine` - linux; arm variant v6

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

### `memcached:1.5-alpine` - linux; arm variant v7

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

### `memcached:1.5-alpine` - linux; arm64 variant v8

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

### `memcached:1.5-alpine` - linux; 386

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

### `memcached:1.5-alpine` - linux; ppc64le

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

### `memcached:1.5-alpine` - linux; s390x

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

## `memcached:1-alpine`

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

### `memcached:1-alpine` - linux; amd64

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

### `memcached:1-alpine` - linux; arm variant v6

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

### `memcached:1-alpine` - linux; arm variant v7

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

### `memcached:1-alpine` - linux; arm64 variant v8

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

### `memcached:1-alpine` - linux; 386

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

### `memcached:1-alpine` - linux; ppc64le

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

## `memcached:latest`

```console
$ docker pull memcached@sha256:2f561d372672bedc970880d64ac0444f877bda1b1605c0bfd4baf4f20fb4c343
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
$ docker pull memcached@sha256:850e5421b841d813966f5e210ff8758fe4d085efef463fb847282af59ca32546
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.5 MB (30474381 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b32d3ed7da92b981b892dff6b378374f7331a44f31e8d2f9533d5d92dba62171`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Sat, 28 Dec 2019 04:21:22 GMT
ADD file:04caaf303199c81ff1a94e2e39d5096f9d02b73294b82758e5bc6e23aff94272 in / 
# Sat, 28 Dec 2019 04:21:23 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 13:58:49 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Sat, 28 Dec 2019 13:58:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 13:58:55 GMT
ENV MEMCACHED_VERSION=1.5.20
# Sat, 28 Dec 2019 13:58:55 GMT
ENV MEMCACHED_SHA1=5d3b5af3ce0a1483d655017db7228bcaeff10d47
# Sat, 28 Dec 2019 14:06:59 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Sat, 28 Dec 2019 14:07:00 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Sat, 28 Dec 2019 14:07:01 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Sat, 28 Dec 2019 14:07:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 28 Dec 2019 14:07:01 GMT
USER memcache
# Sat, 28 Dec 2019 14:07:01 GMT
EXPOSE 11211
# Sat, 28 Dec 2019 14:07:02 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:8ec398bc03560e0fa56440e96da307cdf0b1ad153f459b52bca53ae7ddb8236d`  
		Last Modified: Sat, 28 Dec 2019 04:25:53 GMT  
		Size: 27.1 MB (27092274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60e10c2aa199f4392bf1ddbfa150c6839c390eb66d1774c68eddacd8c11b8642`  
		Last Modified: Sat, 28 Dec 2019 14:07:19 GMT  
		Size: 5.0 KB (4980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:288dc9f908106487c0bad762aaa118ac1198279015f1d5440c3139be04ed7f2f`  
		Last Modified: Sat, 28 Dec 2019 14:07:20 GMT  
		Size: 2.2 MB (2196480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a244ab9e1e9de308e7c856704ec0378f73f5f996f979eaad845ac3f1a49f86bc`  
		Last Modified: Sat, 28 Dec 2019 14:07:20 GMT  
		Size: 1.2 MB (1180238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9db86ad11ed8bbffd528085a0ddb67ac989b020992ffd4c0032b263ee7dad22a`  
		Last Modified: Sat, 28 Dec 2019 14:07:19 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:356f3b62ef2b4bd1cf49aa61dbbe1f11643c2f85f62cbe081e4d7de8d8f39ff2`  
		Last Modified: Sat, 28 Dec 2019 14:07:19 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:latest` - linux; arm variant v5

```console
$ docker pull memcached@sha256:62ccc1796a81315fcbb198c87cb07d58578fba2a105e6ecf52116b5cc1b3cb58
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.9 MB (27874841 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c09d14e5d8cab36aa360bb194317306af61877c397472ba60fd53b4fe1c20c7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 22 Nov 2019 12:13:54 GMT
ADD file:94ed554e445cf749e10644dfa0d836103c120a6ea388bf6dc9f18f7c6b2f095a in / 
# Fri, 22 Nov 2019 12:13:56 GMT
CMD ["bash"]
# Fri, 22 Nov 2019 12:44:01 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Fri, 22 Nov 2019 12:45:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Nov 2019 12:45:25 GMT
ENV MEMCACHED_VERSION=1.5.20
# Fri, 22 Nov 2019 12:45:26 GMT
ENV MEMCACHED_SHA1=5d3b5af3ce0a1483d655017db7228bcaeff10d47
# Wed, 11 Dec 2019 01:15:09 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 11 Dec 2019 01:15:12 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 11 Dec 2019 01:15:22 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 11 Dec 2019 01:15:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 Dec 2019 01:15:25 GMT
USER memcache
# Wed, 11 Dec 2019 01:15:27 GMT
EXPOSE 11211
# Wed, 11 Dec 2019 01:15:28 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:45ae7e8aa5bfd9e1b0db11d7fa5a56a8af11b69fc56707d763f89aa2c61b7e8f`  
		Last Modified: Fri, 22 Nov 2019 12:22:20 GMT  
		Size: 24.8 MB (24829480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7abfa51b826ab2a750aacd0ca0db5eca44bd315eebc7100f88cdaaba729433ee`  
		Last Modified: Wed, 11 Dec 2019 01:15:54 GMT  
		Size: 4.9 KB (4898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22b994f77a11fb8adc23b3e9263cc757d84ddf5528b1352d8bdb638ee9318747`  
		Last Modified: Wed, 11 Dec 2019 01:15:57 GMT  
		Size: 1.9 MB (1896875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f47c6f9dfd6813351ceaddc6807dbb4f5c53bdd8405f4642bf0b0c97ada6279`  
		Last Modified: Wed, 11 Dec 2019 01:15:56 GMT  
		Size: 1.1 MB (1143179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:957ac1f455448be6a6d88a76911ae99cf5148ddb776613c6634f7f641c223db8`  
		Last Modified: Wed, 11 Dec 2019 01:15:54 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04dab8c47bbee2c7ef5a52817e160cd9ef97368f73d41f1423320924bf025467`  
		Last Modified: Wed, 11 Dec 2019 01:15:54 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:latest` - linux; arm variant v7

```console
$ docker pull memcached@sha256:e680132321a0e3a9373f3f40206cedcdaf2667aaa29b64650ce029d756a1971d
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.6 MB (25621613 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e6ae16ecc7ca54d8e4edbc4cacb7d11f1984818935ceaaee7bc287c4176b93e2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 17 Oct 2019 00:05:51 GMT
ADD file:aec8ae5d1bd3bffdcab55efc79e947f802af8efa4266cc074679cc305949f7b9 in / 
# Thu, 17 Oct 2019 00:05:55 GMT
CMD ["bash"]
# Thu, 17 Oct 2019 01:11:52 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Thu, 17 Oct 2019 01:12:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 13 Nov 2019 22:58:06 GMT
ENV MEMCACHED_VERSION=1.5.20
# Wed, 13 Nov 2019 22:58:07 GMT
ENV MEMCACHED_SHA1=5d3b5af3ce0a1483d655017db7228bcaeff10d47
# Thu, 14 Nov 2019 22:35:28 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libsasl2-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		$enableExtstore 	&& make -j "$(nproc)" 		&& make test 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 14 Nov 2019 22:35:31 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 14 Nov 2019 22:35:42 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 14 Nov 2019 22:35:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 14 Nov 2019 22:35:45 GMT
USER memcache
# Thu, 14 Nov 2019 22:35:46 GMT
EXPOSE 11211
# Thu, 14 Nov 2019 22:35:48 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:ffb3a1edd2f5d689daee77b16634ddec87a4f724ac3bbef287c397ea731af2ac`  
		Last Modified: Thu, 17 Oct 2019 00:15:00 GMT  
		Size: 22.7 MB (22711906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcf6d2564d271d74fae4672d14f92fcbe87ead7e1298e8915908de657ab8e5c3`  
		Last Modified: Thu, 14 Nov 2019 22:36:15 GMT  
		Size: 4.9 KB (4891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:109decf50675f59a1197b904e45765ee2fd2056f02aec9d04196b007bfb911d4`  
		Last Modified: Thu, 14 Nov 2019 22:36:18 GMT  
		Size: 1.8 MB (1811613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae8ec6f57a9302a06ef868ed6c3811c6e03d109fa28a5bfdd295111d128eab77`  
		Last Modified: Thu, 14 Nov 2019 22:36:16 GMT  
		Size: 1.1 MB (1092796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59288dbdc770325d3abf8e56283deb225dab1c9ada4503ffa3457077c6d52bef`  
		Last Modified: Thu, 14 Nov 2019 22:36:15 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68a7926932d9f3025d519c57860153bf9ff247f787ade2f50b94b483828878b8`  
		Last Modified: Thu, 14 Nov 2019 22:36:15 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:latest` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:dfd1cdee25d29bf6e12665a09451649f477ba08ef6d95fdb43211a4b364e8228
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.1 MB (29076734 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:94a900befbdf811a79a52b4b2d3c54fbc579986fa21168096939b7e5f8f77eb1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Sat, 28 Dec 2019 04:41:08 GMT
ADD file:b45fd612576b682e93ab91addbc4387a6609ace4bc092e5b615323964bba33c3 in / 
# Sat, 28 Dec 2019 04:41:11 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 09:26:00 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Sat, 28 Dec 2019 09:26:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 09:26:11 GMT
ENV MEMCACHED_VERSION=1.5.20
# Sat, 28 Dec 2019 09:26:12 GMT
ENV MEMCACHED_SHA1=5d3b5af3ce0a1483d655017db7228bcaeff10d47
# Sat, 28 Dec 2019 09:34:56 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Sat, 28 Dec 2019 09:34:57 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Sat, 28 Dec 2019 09:34:59 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Sat, 28 Dec 2019 09:35:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 28 Dec 2019 09:35:01 GMT
USER memcache
# Sat, 28 Dec 2019 09:35:02 GMT
EXPOSE 11211
# Sat, 28 Dec 2019 09:35:02 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:fb62b7c746da1f79992359282f2d8b7f93da8c48dc138ec6b2a36130efd42635`  
		Last Modified: Sat, 28 Dec 2019 04:46:58 GMT  
		Size: 25.9 MB (25850702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b07d5eaa7d9c3d15b1121c61ab46c1765a21a82bce1dd1e376d2ecf09865928`  
		Last Modified: Sat, 28 Dec 2019 09:35:37 GMT  
		Size: 5.0 KB (5029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ea19e96eb15c540f804c57bd35c31b3a8137b38c15e8f31fd26a93422e4c5bb`  
		Last Modified: Sat, 28 Dec 2019 09:35:37 GMT  
		Size: 2.1 MB (2074929 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f5fb8100575d7dac36d76ca7c3a506210dc9a25cfa5aa974ee0e1420fd62c19`  
		Last Modified: Sat, 28 Dec 2019 09:35:37 GMT  
		Size: 1.1 MB (1145667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:734ac2f49087d47d7a139a37e1b9dc10afd8aff2ad495cdcc9949658f6bc6845`  
		Last Modified: Sat, 28 Dec 2019 09:35:36 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cd59d3ba33a5d9b9eedb4d229178fddb6e8a12fdbbc5a976364bbd3faf6cb52`  
		Last Modified: Sat, 28 Dec 2019 09:35:36 GMT  
		Size: 120.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:latest` - linux; 386

```console
$ docker pull memcached@sha256:0f8ee210458e9c6d6662477682ae70695caa17b36de73d06a659620bc7bb919f
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.1 MB (31140927 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0199eb106fa984cf5f81efb1bb8c68c546b9fe108349a022f7a8ac7bfa1ab357`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Sat, 28 Dec 2019 04:39:35 GMT
ADD file:447f0758c9f5653f03d964e54a38c18f24cf4c43e05fc38e7a76aebd6d6bafa8 in / 
# Sat, 28 Dec 2019 04:39:35 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 15:01:45 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Sat, 28 Dec 2019 15:01:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 15:01:51 GMT
ENV MEMCACHED_VERSION=1.5.20
# Sat, 28 Dec 2019 15:01:51 GMT
ENV MEMCACHED_SHA1=5d3b5af3ce0a1483d655017db7228bcaeff10d47
# Sat, 28 Dec 2019 15:10:18 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Sat, 28 Dec 2019 15:10:19 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Sat, 28 Dec 2019 15:10:20 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Sat, 28 Dec 2019 15:10:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 28 Dec 2019 15:10:20 GMT
USER memcache
# Sat, 28 Dec 2019 15:10:21 GMT
EXPOSE 11211
# Sat, 28 Dec 2019 15:10:21 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:5536417213b9f46f2118943c1151912954d6077afe03a32e68521774cc358095`  
		Last Modified: Sat, 28 Dec 2019 04:44:24 GMT  
		Size: 27.7 MB (27747020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f952840b6779a17e1998bfb1e145d53747c667708443e724483989c54a63ee4`  
		Last Modified: Sat, 28 Dec 2019 15:10:44 GMT  
		Size: 4.9 KB (4896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a656e047a0d4ae15c61be416063049cdb41f91945f6159a14e71aca03b6efa0`  
		Last Modified: Sat, 28 Dec 2019 15:10:45 GMT  
		Size: 2.2 MB (2208081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a53ed12be1a50e398a859c745767c1d6aff64b16b1ac35487dfc6c4b2f5055e6`  
		Last Modified: Sat, 28 Dec 2019 15:10:45 GMT  
		Size: 1.2 MB (1180520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efe3d9a88c4bc05a24a9f780eacb3c159d64e3dd03cae5246de72e523d748706`  
		Last Modified: Sat, 28 Dec 2019 15:10:44 GMT  
		Size: 289.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5c516b8df5a22933466c3edea0e576a2f0c7bb325a1197d6e67dc33cedbef29`  
		Last Modified: Sat, 28 Dec 2019 15:10:44 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:latest` - linux; ppc64le

```console
$ docker pull memcached@sha256:feb8e81074da9abdb0cbcad6c65c24453a318f0e0a342c558e3046ab3a7911b3
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.0 MB (34046630 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8eb752b8385ac8444ce410843f8b46f5674d023be19f9e65c8f7ec8b1d5c9152`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Sat, 28 Dec 2019 04:20:39 GMT
ADD file:abec4f3d6a54bb0725560d826d07e99da3d6b582433c6dd95605626c67d7c2d6 in / 
# Sat, 28 Dec 2019 04:20:43 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 13:00:10 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Sat, 28 Dec 2019 13:00:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 13:00:25 GMT
ENV MEMCACHED_VERSION=1.5.20
# Sat, 28 Dec 2019 13:00:27 GMT
ENV MEMCACHED_SHA1=5d3b5af3ce0a1483d655017db7228bcaeff10d47
# Sat, 28 Dec 2019 13:09:37 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Sat, 28 Dec 2019 13:09:38 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Sat, 28 Dec 2019 13:09:41 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Sat, 28 Dec 2019 13:09:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 28 Dec 2019 13:09:45 GMT
USER memcache
# Sat, 28 Dec 2019 13:09:48 GMT
EXPOSE 11211
# Sat, 28 Dec 2019 13:09:51 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:37e6f4d596ea5c3cc92914bd95508a4192c8834c4edaff414734885929b07800`  
		Last Modified: Sat, 28 Dec 2019 04:28:05 GMT  
		Size: 30.5 MB (30517529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7537865582bff5727f1fb50d0cf11718db483efcd8716843fd29e410fb78ed0`  
		Last Modified: Sat, 28 Dec 2019 13:10:14 GMT  
		Size: 5.0 KB (4984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fb3e2d1d77f48e789fa0cce495a195d95d150ffec8e78572548a08a1f3fad14`  
		Last Modified: Sat, 28 Dec 2019 13:10:15 GMT  
		Size: 2.3 MB (2322686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a8b268f98197e3ec2bf2013e77fa416602cc296241528892dce9b192492eca3`  
		Last Modified: Sat, 28 Dec 2019 13:10:14 GMT  
		Size: 1.2 MB (1201022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e4c8a7095e41fca0197a8eaae09593a3d239a078dcdf8d867c382e6bdabe392`  
		Last Modified: Sat, 28 Dec 2019 13:10:14 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c73af1c8cf2cea3e6dc53ba3a3a3253bbe7d931c663d600f51a1d844e26fc2f`  
		Last Modified: Sat, 28 Dec 2019 13:10:14 GMT  
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
