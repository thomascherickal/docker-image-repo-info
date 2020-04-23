## `memcached:latest`

```console
$ docker pull memcached@sha256:2934bcb599356f91bc3f1cdf9cad71ad2a41a2c800c14dd7562ed12f10935925
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
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
$ docker pull memcached@sha256:9eddbead7cb3e16a4acfc24160524eaa6b4d6b399e229d53e21ac3ca988be86c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.5 MB (30492322 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:683b58b6465dc45d04feef9004e16bfe0281495f5331419ec65872923b988553`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 16 Apr 2020 03:22:36 GMT
ADD file:865f9041e12eb341f0a394764ddc11db49cbc8b91d4fb57c6fb1960b68b1bb41 in / 
# Thu, 16 Apr 2020 03:22:36 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 09:01:47 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Thu, 16 Apr 2020 09:01:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 09:01:52 GMT
ENV MEMCACHED_VERSION=1.6.5
# Thu, 16 Apr 2020 09:01:52 GMT
ENV MEMCACHED_SHA1=1ddb5f37f69946b63512ad0f89dc448ff7ba5713
# Thu, 16 Apr 2020 09:10:54 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 16 Apr 2020 09:10:55 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 16 Apr 2020 09:10:56 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 16 Apr 2020 09:10:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 16 Apr 2020 09:10:56 GMT
USER memcache
# Thu, 16 Apr 2020 09:10:57 GMT
EXPOSE 11211
# Thu, 16 Apr 2020 09:10:57 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:123275d6e508d282237a22fefa5aef822b719a06496444ea89efa65da523fc4b`  
		Last Modified: Thu, 16 Apr 2020 03:31:44 GMT  
		Size: 27.1 MB (27098147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cd5009273ce372e945eff9d465c3b9483feafbe19f9dc6e1f158b184b4e112a`  
		Last Modified: Thu, 16 Apr 2020 09:11:23 GMT  
		Size: 5.0 KB (4982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3eaadb451d5774749b9f23e4acd4354848a513f3222fc10fc45f19e7f431b8fe`  
		Last Modified: Thu, 16 Apr 2020 09:11:24 GMT  
		Size: 2.2 MB (2196543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a68eb9be399922992c4a03a30b64a2b49e357dd09e695a4baf86e2692d2221dd`  
		Last Modified: Thu, 16 Apr 2020 09:11:24 GMT  
		Size: 1.2 MB (1192241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21bced5496d960c3f0117e3a0025b8af1e4cd1a8539fea1e26405385a513d09c`  
		Last Modified: Thu, 16 Apr 2020 09:11:24 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34e88f202390fc25200b44fa925889d3821279298543f224be8f98210dc33be6`  
		Last Modified: Thu, 16 Apr 2020 09:11:23 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:latest` - linux; arm variant v5

```console
$ docker pull memcached@sha256:1f4935dd0107cf9cdb6e9164e41ada5092ddac93d048167c94e3611a3db32175
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.9 MB (27895602 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:050184fb78c6e102b8c4f58464d01aeb5b2f00cc2c4a6368ae78cda9f16fac32`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 16 Apr 2020 00:50:14 GMT
ADD file:761a556ec2a7d8c742c860e429c9b9ba3f7abfcd9383c6b3767499de6dcad4bc in / 
# Thu, 16 Apr 2020 00:50:15 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 01:20:06 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Thu, 16 Apr 2020 01:21:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 01:21:39 GMT
ENV MEMCACHED_VERSION=1.6.5
# Thu, 16 Apr 2020 01:21:41 GMT
ENV MEMCACHED_SHA1=1ddb5f37f69946b63512ad0f89dc448ff7ba5713
# Thu, 16 Apr 2020 01:52:48 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 16 Apr 2020 01:52:52 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 16 Apr 2020 01:53:03 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 16 Apr 2020 01:53:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 16 Apr 2020 01:53:06 GMT
USER memcache
# Thu, 16 Apr 2020 01:53:09 GMT
EXPOSE 11211
# Thu, 16 Apr 2020 01:53:11 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:600369660a591bc9594fcf333a847fe997901785f7032d3ad2822b2812c13243`  
		Last Modified: Thu, 16 Apr 2020 00:58:26 GMT  
		Size: 24.8 MB (24836437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83b28efba0bcc6fbfeccf6561801abdbc28d2b64d489f76ee8191a0e4b10e37d`  
		Last Modified: Thu, 16 Apr 2020 01:53:20 GMT  
		Size: 4.9 KB (4891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cc33a1fa2e0b9f8c854ee94cd9adb7ef5ffb735c0a70cc01ccabe5908c4a9d8`  
		Last Modified: Thu, 16 Apr 2020 01:53:23 GMT  
		Size: 1.9 MB (1896808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ace54d112c6a1b7877ddb9dd0d888fc77035cc99c3c294c69d5154ac2cfc4b4`  
		Last Modified: Thu, 16 Apr 2020 01:53:28 GMT  
		Size: 1.2 MB (1157058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90fb24ae48dfbd7b3cb65e78556275a263ddb0964a8761b181efaf5a4075082c`  
		Last Modified: Thu, 16 Apr 2020 01:53:37 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d567aeaee62d3bcefc4ecc969a2ef321a2b67bcb144dea02783037b035fffad2`  
		Last Modified: Thu, 16 Apr 2020 01:53:37 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:latest` - linux; arm variant v7

```console
$ docker pull memcached@sha256:54bcd309e2f20393d4697e22b71344137d3f1fdeb447078522a5a2d6a464117e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.6 MB (25646504 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd1835a38d745cc54481b86a3603e5fe1771df287e08d6061cb35577ce92b735`
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
# Tue, 14 Apr 2020 01:21:52 GMT
ENV MEMCACHED_VERSION=1.6.5
# Tue, 14 Apr 2020 01:21:54 GMT
ENV MEMCACHED_SHA1=1ddb5f37f69946b63512ad0f89dc448ff7ba5713
# Tue, 14 Apr 2020 01:50:54 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 14 Apr 2020 01:50:57 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 14 Apr 2020 01:51:07 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 14 Apr 2020 01:51:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 14 Apr 2020 01:51:11 GMT
USER memcache
# Tue, 14 Apr 2020 01:51:12 GMT
EXPOSE 11211
# Tue, 14 Apr 2020 01:51:14 GMT
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
	-	`sha256:dca1ebe9584513d346175a7b8dc24e8a0e1f282079ab035f21745b1efb49aee2`  
		Last Modified: Tue, 14 Apr 2020 03:14:41 GMT  
		Size: 1.1 MB (1129915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3670b9b896bea4402ae6cf76d7c5690c7be94b8712a6ba9bdbc5162c478c3f4a`  
		Last Modified: Tue, 14 Apr 2020 03:14:40 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13fc7c30db064f3e3c4355aa5316e9ee78fc6d5727ba346d8289b531a5244235`  
		Last Modified: Tue, 14 Apr 2020 03:14:46 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:latest` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:1b63b6173baa070dca266b74e1df313fef3b26aee9284d695af1498737f34cb6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.1 MB (29101115 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d0a838ee3058b61425f78fcd97c68e539c3dd067b5dd2fb5cf62018062d254ec`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 23 Apr 2020 00:54:55 GMT
ADD file:581ee9c3c19f0d971aeda008fd399f59171cae75e8936b967dbf3888db4fc0d0 in / 
# Thu, 23 Apr 2020 00:54:58 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 03:03:20 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Thu, 23 Apr 2020 03:03:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 03:03:30 GMT
ENV MEMCACHED_VERSION=1.6.5
# Thu, 23 Apr 2020 03:03:31 GMT
ENV MEMCACHED_SHA1=1ddb5f37f69946b63512ad0f89dc448ff7ba5713
# Thu, 23 Apr 2020 03:31:48 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 23 Apr 2020 03:31:49 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 23 Apr 2020 03:31:51 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 23 Apr 2020 03:31:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Apr 2020 03:31:53 GMT
USER memcache
# Thu, 23 Apr 2020 03:31:54 GMT
EXPOSE 11211
# Thu, 23 Apr 2020 03:31:55 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:bdc84a41f2513e28e99efeff9fcbb196b7df9883fb30532184bd67ca415b4673`  
		Last Modified: Thu, 23 Apr 2020 01:03:27 GMT  
		Size: 25.9 MB (25857800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b8ed987f36e3ad8893c5c7ce9e42aeb35d67e90daf262dde60d86dfa94814f5`  
		Last Modified: Thu, 23 Apr 2020 03:32:22 GMT  
		Size: 5.0 KB (5028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:360e6a91a753e3a018e26a9d22b25766c2ebd2231cbc3e245648aead98ddde08`  
		Last Modified: Thu, 23 Apr 2020 03:32:23 GMT  
		Size: 2.1 MB (2074961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4a836f92da3f2b418fee687d52a49dc5c67ed60998eb59b18bd9db12d131b39`  
		Last Modified: Thu, 23 Apr 2020 03:32:22 GMT  
		Size: 1.2 MB (1162917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efbfa008b3b7db8d9a84dbe0e5c602cb0bcd8c73f3756fd94eb9818c17b45829`  
		Last Modified: Thu, 23 Apr 2020 03:32:22 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95e9585a94db0285470fac037a11f3b7b0cad7c683c37919c8d98b3750839884`  
		Last Modified: Thu, 23 Apr 2020 03:32:22 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:latest` - linux; 386

```console
$ docker pull memcached@sha256:4cd7c8a145c4b502f84c55f41e0ae4971614a237b96076093edb951df16af86f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.2 MB (31163013 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66532fde035d2034732c7b657027f1f342acdb811b1d859d9f6ed3bc370262e2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 23 Apr 2020 00:39:36 GMT
ADD file:ca6a74f6b738c738c033152fab2a9aacf22bec5f19a994e6a02b5f919ee33ee9 in / 
# Thu, 23 Apr 2020 00:39:36 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 01:29:35 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Thu, 23 Apr 2020 01:29:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 01:29:42 GMT
ENV MEMCACHED_VERSION=1.6.5
# Thu, 23 Apr 2020 01:29:42 GMT
ENV MEMCACHED_SHA1=1ddb5f37f69946b63512ad0f89dc448ff7ba5713
# Thu, 23 Apr 2020 01:38:20 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 23 Apr 2020 01:38:20 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 23 Apr 2020 01:38:21 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 23 Apr 2020 01:38:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Apr 2020 01:38:21 GMT
USER memcache
# Thu, 23 Apr 2020 01:38:21 GMT
EXPOSE 11211
# Thu, 23 Apr 2020 01:38:21 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:5d3da8f33b97fc107a05b3255a55836b76df9f817de632b1fb63c6e9c024f0df`  
		Last Modified: Thu, 23 Apr 2020 00:44:35 GMT  
		Size: 27.8 MB (27753972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c3cb2639d5e9c8ab44fd2bbe5bedbb5c4d33378f9781d558d2ac27611ecd673`  
		Last Modified: Thu, 23 Apr 2020 01:38:35 GMT  
		Size: 4.9 KB (4898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6f2f84fd6631cbca67ed46fd3b380a42475afb287d8e990ded3d3a91fded71a`  
		Last Modified: Thu, 23 Apr 2020 01:38:35 GMT  
		Size: 2.2 MB (2208055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae882751a1fc445bebd4d4f545c0c69529396863b7ac0b3fc3137b2c3cecbfaa`  
		Last Modified: Thu, 23 Apr 2020 01:38:35 GMT  
		Size: 1.2 MB (1195679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d53c7886eeb4da4192fe5caceac337d1fa31afc20be46a9476fd10e35bd4d81e`  
		Last Modified: Thu, 23 Apr 2020 01:38:35 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43f9bc6252b62803993a04eff4ad6e08d728474f2c446e92d32b5ab3ac38ab08`  
		Last Modified: Thu, 23 Apr 2020 01:38:35 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:latest` - linux; mips64le

```console
$ docker pull memcached@sha256:37443af1d21860af4e933db9c5901eb2334d29a83ba221ac01c9a77298ec38f8
```

-	Docker Version: 19.03.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.7 MB (28725217 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:86a54bd34452343aa3a8f6e631804252b62cdf1fb36e95356f304eebac4ca028`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 16 Apr 2020 03:30:32 GMT
ADD file:1324f1b90326c771ad3fbeba783010d46ba465c130b2b400ff60232e52bc4bbb in / 
# Thu, 16 Apr 2020 03:30:33 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 06:48:56 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Thu, 16 Apr 2020 06:49:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 06:49:10 GMT
ENV MEMCACHED_VERSION=1.6.5
# Thu, 16 Apr 2020 06:49:11 GMT
ENV MEMCACHED_SHA1=1ddb5f37f69946b63512ad0f89dc448ff7ba5713
# Thu, 16 Apr 2020 07:00:08 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 16 Apr 2020 07:00:09 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 16 Apr 2020 07:00:11 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 16 Apr 2020 07:00:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 16 Apr 2020 07:00:12 GMT
USER memcache
# Thu, 16 Apr 2020 07:00:12 GMT
EXPOSE 11211
# Thu, 16 Apr 2020 07:00:13 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:9d68bbb6bb3e325311e23872a0324580a3e32aea907701fa94bab81e80ff88c4`  
		Last Modified: Thu, 16 Apr 2020 03:56:50 GMT  
		Size: 25.8 MB (25762172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:785715caab3f56abc177362b8199fd005f80b317c038df3a45c5bd1403c44ad4`  
		Last Modified: Thu, 16 Apr 2020 07:00:29 GMT  
		Size: 5.0 KB (4983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d7f59cac83da5b1ac93cef4097b98628adff0484596ed417e3ec37182291062`  
		Last Modified: Thu, 16 Apr 2020 07:00:31 GMT  
		Size: 1.8 MB (1775990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96ff54829cc31369ac9b0e95e0689f6fc93229eec69c55c0d7e975e2937cdc84`  
		Last Modified: Thu, 16 Apr 2020 07:00:31 GMT  
		Size: 1.2 MB (1181663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a58a488b9bf07f7fcb8988ab4c67c47cc46f3e4bae17572806460fbe03a380eb`  
		Last Modified: Thu, 16 Apr 2020 07:00:30 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9534a0c87d7e09580b6f25e662699f34a06a9e545c58950262cebcefbb118d5e`  
		Last Modified: Thu, 16 Apr 2020 07:00:30 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:latest` - linux; ppc64le

```console
$ docker pull memcached@sha256:276923dcc9e512c2f1c08118d810f65debcec9b6687c842faf1d3eec94306030
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.1 MB (34070732 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:757225c0b9a3b4adb4ce9c18b375416ef9c481aa42e85bc7542e0dbd4ae0cec5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 16 Apr 2020 01:38:30 GMT
ADD file:9beea54416432abbd09d26b965c3c8e5bea8e233113f9bc308294c0008ee886f in / 
# Thu, 16 Apr 2020 01:38:39 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 02:51:43 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Thu, 16 Apr 2020 02:52:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 02:52:16 GMT
ENV MEMCACHED_VERSION=1.6.5
# Thu, 16 Apr 2020 02:52:26 GMT
ENV MEMCACHED_SHA1=1ddb5f37f69946b63512ad0f89dc448ff7ba5713
# Thu, 16 Apr 2020 03:07:11 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& make -j "$(nproc)" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 	&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 16 Apr 2020 03:07:14 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 16 Apr 2020 03:07:22 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 16 Apr 2020 03:07:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 16 Apr 2020 03:07:29 GMT
USER memcache
# Thu, 16 Apr 2020 03:07:34 GMT
EXPOSE 11211
# Thu, 16 Apr 2020 03:07:39 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:f268991f8af64097bbfefa3f01dd3fdb7f715051a3681f352504a3ecaa9d3596`  
		Last Modified: Thu, 16 Apr 2020 01:54:39 GMT  
		Size: 30.5 MB (30524651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97f54728ddf3d5bb9060696766575c26ec0bb229622818d0e5dd8a5ab0553926`  
		Last Modified: Thu, 16 Apr 2020 03:08:14 GMT  
		Size: 5.0 KB (4984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac80ca64d3e34a34f53513e845287c7a5bdf39f59d0bb72678a8081c97176068`  
		Last Modified: Thu, 16 Apr 2020 03:08:14 GMT  
		Size: 2.3 MB (2322683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6e5e36550d8e4f020336d5d1dab133cf1465839cba3f2c78d91d55b68ff2c3e`  
		Last Modified: Thu, 16 Apr 2020 03:08:14 GMT  
		Size: 1.2 MB (1218011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f2baec843adb884a462036750346dcb278d276ef643b2cf4f3db9fa55c9fadc`  
		Last Modified: Thu, 16 Apr 2020 03:08:13 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fe0a71e5ce63dce2c34dd1bcaa4198872841b8d7f50911091a547d527f80108`  
		Last Modified: Thu, 16 Apr 2020 03:08:13 GMT  
		Size: 118.0 B  
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
