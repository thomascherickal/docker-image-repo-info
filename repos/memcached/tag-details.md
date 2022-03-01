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
-	[`memcached:1.6.14`](#memcached1614)
-	[`memcached:1.6.14-alpine`](#memcached1614-alpine)
-	[`memcached:1.6.14-alpine3.15`](#memcached1614-alpine315)
-	[`memcached:1.6.14-bullseye`](#memcached1614-bullseye)
-	[`memcached:alpine`](#memcachedalpine)
-	[`memcached:alpine3.15`](#memcachedalpine315)
-	[`memcached:bullseye`](#memcachedbullseye)
-	[`memcached:latest`](#memcachedlatest)

## `memcached:1`

```console
$ docker pull memcached@sha256:e4bb2d212309e51166f29fe5404edf5caf784ada9ab3fde8dcf8226f337878aa
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
$ docker pull memcached@sha256:2c29149daad601e046074c6801fb570180d4eba60047135b71f51ea327ffcbc1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.0 MB (32954984 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6208dafa350f4dfbb3f2a16e20c2f2d256f894fd8695ac24b21663a732dee124`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 01 Mar 2022 02:13:29 GMT
ADD file:d48a85028743f16ed927507322e3e3beee187fbfadd0b781d4b89de197c64b5b in / 
# Tue, 01 Mar 2022 02:13:29 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 13:24:57 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 01 Mar 2022 13:25:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 13:25:02 GMT
ENV MEMCACHED_VERSION=1.6.14
# Tue, 01 Mar 2022 13:25:02 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Tue, 01 Mar 2022 13:28:58 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 01 Mar 2022 13:28:58 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 01 Mar 2022 13:28:59 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 01 Mar 2022 13:28:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 01 Mar 2022 13:29:00 GMT
USER memcache
# Tue, 01 Mar 2022 13:29:00 GMT
EXPOSE 11211
# Tue, 01 Mar 2022 13:29:00 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:f7a1c6dad28192bd417b78079d6ddc03cbca6d5ea46bba12769b235b6353c00c`  
		Last Modified: Tue, 01 Mar 2022 02:19:23 GMT  
		Size: 31.4 MB (31366396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3292b9ed039a5211ec564a1f170046ba2ad296a19beb778d3c7106a230301d27`  
		Last Modified: Tue, 01 Mar 2022 13:29:33 GMT  
		Size: 5.0 KB (4980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15c683705067bdb5151c087a9b5e91a37f498912588e29970e3ce07121334f03`  
		Last Modified: Tue, 01 Mar 2022 13:29:34 GMT  
		Size: 328.0 KB (328033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:091c46e57219c5fdd0a044c77fc12a24889bd1ce95e4d032e83f2ea09997ca1d`  
		Last Modified: Tue, 01 Mar 2022 13:29:34 GMT  
		Size: 1.3 MB (1255168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a26e7e13ba905fd75a5e3b2307ab4abee1bbcdc9b586d37fc2ff7984de1c92c3`  
		Last Modified: Tue, 01 Mar 2022 13:29:33 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75b625708cf5e763937f326c6fe55adcb4c4782926483ea2a3628012927922c7`  
		Last Modified: Tue, 01 Mar 2022 13:29:33 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1` - linux; arm variant v5

```console
$ docker pull memcached@sha256:839b663c2a5637a5a026d8bf63f2c3a5af62938b6becb246fe84e68bceb73742
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.5 MB (30457903 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:46c3d2c41f175e70fa19ec073355fc3376f15b3ca99f6fdb295b6cea57aede38`
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
# Fri, 11 Feb 2022 23:48:33 GMT
ENV MEMCACHED_VERSION=1.6.14
# Fri, 11 Feb 2022 23:48:33 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Fri, 11 Feb 2022 23:53:18 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Fri, 11 Feb 2022 23:53:19 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 11 Feb 2022 23:53:20 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 11 Feb 2022 23:53:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Feb 2022 23:53:21 GMT
USER memcache
# Fri, 11 Feb 2022 23:53:22 GMT
EXPOSE 11211
# Fri, 11 Feb 2022 23:53:22 GMT
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
	-	`sha256:4c595fdbb4287a9ef2b3565e1d9ac2caa7d17ac0810224d8a5d3c87313cc81b5`  
		Last Modified: Fri, 11 Feb 2022 23:54:16 GMT  
		Size: 1.2 MB (1226376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19c8ecb542750e6e603057b1e7bdb90fc58d45b604f20b2724d402a572f1b735`  
		Last Modified: Fri, 11 Feb 2022 23:54:15 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64d2e913eaab741b412c8fec5edbad97daed3a2c5f0a1a1fd376ea8ec7c28c52`  
		Last Modified: Fri, 11 Feb 2022 23:54:15 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1` - linux; arm variant v7

```console
$ docker pull memcached@sha256:c1ded327e0d4c11f7f00652600f4cbf465a119fed31e6e2541d516700e0e14c2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.1 MB (28080208 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:866cf84302a62bedfada61f236deccacb7585dc0ccce8a4e0e058b741bfafdc5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 01 Mar 2022 02:02:56 GMT
ADD file:c6b519323fd1fa09b9f8c8608778872e8fa6208cb0b42aaccdef4479a469f5f4 in / 
# Tue, 01 Mar 2022 02:02:57 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 14:02:17 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 01 Mar 2022 14:02:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 14:02:26 GMT
ENV MEMCACHED_VERSION=1.6.14
# Tue, 01 Mar 2022 14:02:26 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Tue, 01 Mar 2022 14:06:15 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 01 Mar 2022 14:06:16 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 01 Mar 2022 14:06:17 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 01 Mar 2022 14:06:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 01 Mar 2022 14:06:18 GMT
USER memcache
# Tue, 01 Mar 2022 14:06:19 GMT
EXPOSE 11211
# Tue, 01 Mar 2022 14:06:19 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:59dbb2ac3829352dd707e28e037734c9fbdef5b03aea31e3929ddcead949afee`  
		Last Modified: Tue, 01 Mar 2022 02:19:09 GMT  
		Size: 26.6 MB (26565105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45ff8679190bbfe567a01e354c79eb44efaa4564b0770a644b9eb6a28f10812c`  
		Last Modified: Tue, 01 Mar 2022 14:19:16 GMT  
		Size: 4.9 KB (4894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13db11031aa185885b3b1b9c74eba0d8ea9b07d5e8fec5870bc7df8d09585d2f`  
		Last Modified: Tue, 01 Mar 2022 14:19:16 GMT  
		Size: 312.0 KB (312009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:079efee4f8d1e8cea53f0cc6ddc4832de31e69c43411b81e790e0615eeea16aa`  
		Last Modified: Tue, 01 Mar 2022 14:19:16 GMT  
		Size: 1.2 MB (1197793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:050fbe09656330899bb983ba6d0871a6cc96349c4c049673a4ee53816db5ff7b`  
		Last Modified: Tue, 01 Mar 2022 14:19:16 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcca636453f4acf7b597c080e2d7c57ea366f36daae56acdd43664bb28dff985`  
		Last Modified: Tue, 01 Mar 2022 14:19:16 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:c59ae38d83ce474dc14423325e3f500a06e285938b4f4e8a013ae8967603d492
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.4 MB (31435417 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b5c5ad61ebd09fab08b612599fdf9e96be59696045e4765dac554781daef4d1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 01 Mar 2022 02:11:29 GMT
ADD file:9816c9c29627693c34afda4fa5e1a5e8a0f5aa3c5d5cfd920a4d89c77aab997d in / 
# Tue, 01 Mar 2022 02:11:30 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 12:44:12 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 01 Mar 2022 12:44:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 12:44:16 GMT
ENV MEMCACHED_VERSION=1.6.14
# Tue, 01 Mar 2022 12:44:17 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Tue, 01 Mar 2022 12:46:49 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 01 Mar 2022 12:46:50 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 01 Mar 2022 12:46:50 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 01 Mar 2022 12:46:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 01 Mar 2022 12:46:52 GMT
USER memcache
# Tue, 01 Mar 2022 12:46:53 GMT
EXPOSE 11211
# Tue, 01 Mar 2022 12:46:54 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:279a020076a7fbddfc996e4c55e605a8f322810c3eca21cdedbcb06beb0e1305`  
		Last Modified: Tue, 01 Mar 2022 02:18:24 GMT  
		Size: 30.1 MB (30057008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7dfd1ea3d9e177e785365db9a22591801c15e6a33097ba79a048e3387f4c43a`  
		Last Modified: Tue, 01 Mar 2022 12:47:45 GMT  
		Size: 4.9 KB (4902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e563a531f0653c96d3786deff2afe7190769b5929d06c8c234d89fd314bf2396`  
		Last Modified: Tue, 01 Mar 2022 12:47:45 GMT  
		Size: 119.2 KB (119172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1d1b1b990f1e4e95a5410acd589565956a1fd54c4df3b71a665dcfb23ac9f76`  
		Last Modified: Tue, 01 Mar 2022 12:47:46 GMT  
		Size: 1.3 MB (1253928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b8a7c0be94d102b9a04c359186fcf59b223183acc8b489d0ca12afb8f073027`  
		Last Modified: Tue, 01 Mar 2022 12:47:45 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:091c7ee2fb4e34177c30b2b9905bf098f304bea040ff7ca5700134d4921c2758`  
		Last Modified: Tue, 01 Mar 2022 12:47:45 GMT  
		Size: 120.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1` - linux; 386

```console
$ docker pull memcached@sha256:4c9eb4902e2601bad18a1783dbf7d64cf25f6121226d4772a5d36a7ac3e9db79
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.0 MB (33972554 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af09c75e25cf0ea60c4f155a25728e256411f07898946ea08e869eb6362e3a24`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 01 Mar 2022 02:07:32 GMT
ADD file:e92ab504d4c0d3bd63da83254e6ca400b607c32e0f5037039648559b91770870 in / 
# Tue, 01 Mar 2022 02:07:33 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 10:07:23 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 01 Mar 2022 10:07:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 10:07:30 GMT
ENV MEMCACHED_VERSION=1.6.14
# Tue, 01 Mar 2022 10:07:30 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Tue, 01 Mar 2022 10:11:57 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 01 Mar 2022 10:11:57 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 01 Mar 2022 10:11:58 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 01 Mar 2022 10:11:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 01 Mar 2022 10:11:58 GMT
USER memcache
# Tue, 01 Mar 2022 10:11:58 GMT
EXPOSE 11211
# Tue, 01 Mar 2022 10:11:59 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:04a87e821be7e4b29d48011b7aa4ff884ca57fd36995cb3b99fd2fc24ac562d8`  
		Last Modified: Tue, 01 Mar 2022 02:15:51 GMT  
		Size: 32.4 MB (32377389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe860ecc70fbef589f9779541d957321138c3f41d99742ca7ff2bb41b6787786`  
		Last Modified: Tue, 01 Mar 2022 10:13:02 GMT  
		Size: 4.9 KB (4889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71fbbf846282a29c58595e09b8a5d93a6348fc5a77d0bb513263f933972610e8`  
		Last Modified: Tue, 01 Mar 2022 10:13:03 GMT  
		Size: 336.6 KB (336603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f93f31af2adb455df5e2c7baaa190b479d463d37657734ee855d663709906a2`  
		Last Modified: Tue, 01 Mar 2022 10:13:03 GMT  
		Size: 1.3 MB (1253268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ea06973bd5c70feb976fde3006e5400760f293973d5a2a8f8a05a73105a5851`  
		Last Modified: Tue, 01 Mar 2022 10:13:02 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c85296c039a2ca9f99139e04d26550a26b109424a80e9377a115129110257b9`  
		Last Modified: Tue, 01 Mar 2022 10:13:02 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1` - linux; mips64le

```console
$ docker pull memcached@sha256:76269e61918b56719946fa47ffaebf468965e45dae401738fcd6d8ea6d9afdc1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.2 MB (31213138 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bdf2a1611553c4acfb426a9736777620af35250c1c3fde4997dd8fda25547725`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 01 Mar 2022 02:02:49 GMT
ADD file:1901e1e1292cbfcd557262ec5d08551cecd0070b24928414d220472664fe3fdf in / 
# Tue, 01 Mar 2022 02:02:49 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 03:43:18 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 01 Mar 2022 03:43:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 03:43:30 GMT
ENV MEMCACHED_VERSION=1.6.14
# Tue, 01 Mar 2022 03:43:30 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Tue, 01 Mar 2022 03:49:17 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 01 Mar 2022 03:49:17 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 01 Mar 2022 03:49:19 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 01 Mar 2022 03:49:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 01 Mar 2022 03:49:20 GMT
USER memcache
# Tue, 01 Mar 2022 03:49:20 GMT
EXPOSE 11211
# Tue, 01 Mar 2022 03:49:20 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:3baeb8c34a522fc616f97412d47dc1f665e93552c57aa8237ee1d673f9757cba`  
		Last Modified: Tue, 01 Mar 2022 02:12:25 GMT  
		Size: 29.6 MB (29632966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50a63f21594c0da6641452e9cd0caaf8727bae4ca86c617384198ab5d8e766ec`  
		Last Modified: Tue, 01 Mar 2022 03:49:43 GMT  
		Size: 5.0 KB (4979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dfb3a0cb8d59939fa0e67d13c57840042b1397d36d3c1918e50344eb405025d`  
		Last Modified: Tue, 01 Mar 2022 03:49:43 GMT  
		Size: 323.7 KB (323703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e632b2b5bf88ea94d56d701fa93b55516003db1fc7c855bb4569f2be0ddf3be`  
		Last Modified: Tue, 01 Mar 2022 03:49:43 GMT  
		Size: 1.3 MB (1251083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1fc0f9b2a7499de336af3103d86d1ffc3b90b62ea850295c0c57abbe68c753b`  
		Last Modified: Tue, 01 Mar 2022 03:49:43 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe1ee7b4dd056bb3eadc09b9893ce88a096e51500bbe841d1c145be10ba2b1f0`  
		Last Modified: Tue, 01 Mar 2022 03:49:43 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1` - linux; ppc64le

```console
$ docker pull memcached@sha256:4893f4daa742b31f414b08f98f8e7d0cbedaf63b8d88062bcf3c91a9522a2aab
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.0 MB (36957544 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8db953cc998ed06712eca57fe4ae2b8bb342ce991683fd7592495a21557d0940`
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
# Fri, 11 Feb 2022 23:47:36 GMT
ENV MEMCACHED_VERSION=1.6.14
# Fri, 11 Feb 2022 23:47:38 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Fri, 11 Feb 2022 23:53:07 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Fri, 11 Feb 2022 23:53:13 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 11 Feb 2022 23:53:34 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 11 Feb 2022 23:53:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Feb 2022 23:53:39 GMT
USER memcache
# Fri, 11 Feb 2022 23:53:41 GMT
EXPOSE 11211
# Fri, 11 Feb 2022 23:53:46 GMT
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
	-	`sha256:d5f2e5d5bb1609e336a37e97218d618550ec5ce28384c32b1141393ef6f04a03`  
		Last Modified: Fri, 11 Feb 2022 23:58:44 GMT  
		Size: 1.3 MB (1322220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76e6da4f290b1cff2fa5b1ad17d42333c67179332511db4da3bd2c5ce12bbdfa`  
		Last Modified: Fri, 11 Feb 2022 23:58:44 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fb140c5468aa121999bc169d30e4ce6b73795cdf67aa21c1dfd3d1194dd0b82`  
		Last Modified: Fri, 11 Feb 2022 23:58:44 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1` - linux; s390x

```console
$ docker pull memcached@sha256:14b3ae46a3b5dc4d1ca410da43e53ee0c44ad49ec398f235628f89bc8cc0a0cc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.2 MB (31217166 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:50f1b3aef9bc393e3b1a3fab35c702d6a9b9dd6fa2abd9d044b52385b9ccf549`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 01 Mar 2022 02:01:56 GMT
ADD file:d869ad3392a4e752c2f73d08a4cc13594c94bfc050bd037db0ca9827a0207072 in / 
# Tue, 01 Mar 2022 02:01:58 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 13:28:37 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 01 Mar 2022 13:28:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 13:28:40 GMT
ENV MEMCACHED_VERSION=1.6.14
# Tue, 01 Mar 2022 13:28:40 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Tue, 01 Mar 2022 13:31:58 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 01 Mar 2022 13:31:58 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 01 Mar 2022 13:31:58 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 01 Mar 2022 13:31:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 01 Mar 2022 13:31:59 GMT
USER memcache
# Tue, 01 Mar 2022 13:31:59 GMT
EXPOSE 11211
# Tue, 01 Mar 2022 13:31:59 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:f81abce72636770dac4258df46a31beeb6ad81dfddd5b7c9c3fa6942ea074922`  
		Last Modified: Tue, 01 Mar 2022 02:07:33 GMT  
		Size: 29.6 MB (29647132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b43f274641c42412c1e075acb3920020215603d1e1c938fa84211ea8b005988`  
		Last Modified: Tue, 01 Mar 2022 13:32:52 GMT  
		Size: 5.0 KB (5024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d135f121f1aff6ea16284d2286318c703c72dad45560bdc68ac2bc2371f8164`  
		Last Modified: Tue, 01 Mar 2022 13:32:52 GMT  
		Size: 324.1 KB (324102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9255401f181741c77541d42f93796b72c20077b2815b9e6c4e21b36f9bcccab6`  
		Last Modified: Tue, 01 Mar 2022 13:32:52 GMT  
		Size: 1.2 MB (1240500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5436de37a983faa64cc9d82c3a8272ae77b107e2f8bcd453f7aee5e3e92def7`  
		Last Modified: Tue, 01 Mar 2022 13:32:52 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8296feb21176186e1c4027cf5e8111ed103c7b2b30f1f4423a9303a0e7fd9d3`  
		Last Modified: Tue, 01 Mar 2022 13:32:52 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:1-alpine`

```console
$ docker pull memcached@sha256:a37fd6c034a7e4334d091beedffb525aae8af4acc0cee3030758ae3edc0c524b
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
$ docker pull memcached@sha256:e79dd6dea75bf64de1cd87b2204574865bcc12fcda9e1d5c63ce82e3271d4bdf
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.3 MB (5345174 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31403aa3ac88632da679879fcb0a3a627c6f50ec7da0659ae032f63d289d9587`
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
# Fri, 11 Feb 2022 23:43:32 GMT
ENV MEMCACHED_VERSION=1.6.14
# Fri, 11 Feb 2022 23:43:32 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Fri, 11 Feb 2022 23:47:43 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Fri, 11 Feb 2022 23:47:43 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 11 Feb 2022 23:47:44 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 11 Feb 2022 23:47:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Feb 2022 23:47:44 GMT
USER memcache
# Fri, 11 Feb 2022 23:47:45 GMT
EXPOSE 11211
# Fri, 11 Feb 2022 23:47:45 GMT
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
	-	`sha256:4afc0667aa68ec7c0a865809dcfee799f6357b1f6d6c4d6e58240cff71c6264d`  
		Last Modified: Fri, 11 Feb 2022 23:48:39 GMT  
		Size: 2.4 MB (2415863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef8943e1197199b34fc9e9230f24d760a30cdcf11c6b8fc48e89592e00da6edf`  
		Last Modified: Fri, 11 Feb 2022 23:48:38 GMT  
		Size: 283.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b10635796b46c66fb5447019c111ad88d5b808536aab4757aa60b57ffcc9d0da`  
		Last Modified: Fri, 11 Feb 2022 23:48:38 GMT  
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
$ docker pull memcached@sha256:c28cbb9d278a2ef6c4ef325c2fffa8bc4631258a341cb411d2a7bec9655007cb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.1 MB (5109831 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e10238b3468650bbfa09ac13b6115339c5305e3e92cb34bb47b6a03b2a93df01`
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
# Fri, 11 Feb 2022 23:59:43 GMT
ENV MEMCACHED_VERSION=1.6.14
# Fri, 11 Feb 2022 23:59:44 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Sat, 12 Feb 2022 00:02:34 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Sat, 12 Feb 2022 00:02:36 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Sat, 12 Feb 2022 00:02:36 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Sat, 12 Feb 2022 00:02:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 12 Feb 2022 00:02:38 GMT
USER memcache
# Sat, 12 Feb 2022 00:02:39 GMT
EXPOSE 11211
# Sat, 12 Feb 2022 00:02:40 GMT
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
	-	`sha256:98b2012c64d2efed092c8ec83344fc68be38873465f9e7b82616b504ca67ea14`  
		Last Modified: Sat, 12 Feb 2022 00:03:57 GMT  
		Size: 2.3 MB (2282236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b54695eeb42571708a7da87031a54d3f82b1be9e474102eeaa912ee51cb86d3`  
		Last Modified: Sat, 12 Feb 2022 00:03:57 GMT  
		Size: 283.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17690cc3c867c822f67c6edabb66fd363b8988e13ed76d6b2a512a4af041bd58`  
		Last Modified: Sat, 12 Feb 2022 00:03:57 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-alpine` - linux; 386

```console
$ docker pull memcached@sha256:5b9731ba5ab72d85a6ed73548a502d6e22d512f328daacddeb531c252745a1e7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.4 MB (5369203 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:83c422eacdcda2fa728cc1fc176ab0cd57a0be7766f0b517dcc64045b255d0a9`
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
# Fri, 11 Feb 2022 23:43:00 GMT
ENV MEMCACHED_VERSION=1.6.14
# Fri, 11 Feb 2022 23:43:01 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Fri, 11 Feb 2022 23:47:20 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Fri, 11 Feb 2022 23:47:20 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 11 Feb 2022 23:47:21 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 11 Feb 2022 23:47:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Feb 2022 23:47:22 GMT
USER memcache
# Fri, 11 Feb 2022 23:47:22 GMT
EXPOSE 11211
# Fri, 11 Feb 2022 23:47:22 GMT
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
	-	`sha256:62d0cbe6f51da8f3bfd9d0bfbbb510f173b231cfc4260066e5da12995d012223`  
		Last Modified: Fri, 11 Feb 2022 23:48:48 GMT  
		Size: 2.4 MB (2419277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfa2ab27dc5f099b91f7195a3d75e51e7f2c84ea56052a565dcbeba235da559b`  
		Last Modified: Fri, 11 Feb 2022 23:48:47 GMT  
		Size: 283.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0394921490062e0dab12bc6f8a3a5bd3f1a97dc261653593a22e3fa95776186`  
		Last Modified: Fri, 11 Feb 2022 23:48:47 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-alpine` - linux; ppc64le

```console
$ docker pull memcached@sha256:75cb5141098fb02bb0c554c31c00d28802b414593a6b41d430c10505ee943fe0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.3 MB (5315837 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4be74852968716dd05ad711f1cda531afac5b782fe0dd6692e5aed7d91d54466`
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
# Fri, 11 Feb 2022 23:54:02 GMT
ENV MEMCACHED_VERSION=1.6.14
# Fri, 11 Feb 2022 23:54:06 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Fri, 11 Feb 2022 23:57:48 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Fri, 11 Feb 2022 23:57:50 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 11 Feb 2022 23:57:55 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 11 Feb 2022 23:57:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Feb 2022 23:57:59 GMT
USER memcache
# Fri, 11 Feb 2022 23:58:01 GMT
EXPOSE 11211
# Fri, 11 Feb 2022 23:58:02 GMT
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
	-	`sha256:e9d933f0d59015113f25123de9b3460a03fdf091181f4c9330b1bb42c27a8cce`  
		Last Modified: Fri, 11 Feb 2022 23:59:16 GMT  
		Size: 2.4 MB (2373175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:659fd1f60c2bc05966f606e677370eeee3176f7d6dbd530b3f271ba313f8b0fe`  
		Last Modified: Fri, 11 Feb 2022 23:59:15 GMT  
		Size: 282.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8d9d86e7310ff252ce602224ce1643c6b8d50713444e43804cdb93912f89087`  
		Last Modified: Fri, 11 Feb 2022 23:59:15 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-alpine` - linux; s390x

```console
$ docker pull memcached@sha256:05d8b33e1a3927fd3ba6b7cd62b648d66a4f07da15103657791736e70515bd20
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4869494 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a751c73ff4357b7992c0a524e080537c462baa079ef3c7b96a3ce7b13699135`
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
# Fri, 11 Feb 2022 23:53:09 GMT
ENV MEMCACHED_VERSION=1.6.14
# Fri, 11 Feb 2022 23:53:09 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Fri, 11 Feb 2022 23:57:25 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Fri, 11 Feb 2022 23:57:25 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 11 Feb 2022 23:57:26 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 11 Feb 2022 23:57:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Feb 2022 23:57:26 GMT
USER memcache
# Fri, 11 Feb 2022 23:57:26 GMT
EXPOSE 11211
# Fri, 11 Feb 2022 23:57:26 GMT
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
	-	`sha256:7bccd1e890d9edaaa99814caec66d49d04d5245aca1fe8a2ac832be7e0e09c06`  
		Last Modified: Fri, 11 Feb 2022 23:58:42 GMT  
		Size: 2.1 MB (2148137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75931a88b924783decffcbf2e1fba6e58f393e9409dd37ffb26b7f6eecffdef2`  
		Last Modified: Fri, 11 Feb 2022 23:58:41 GMT  
		Size: 282.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2dd123370c89ee375732af5193be621336dd45eae2b9729fb66d0376bc915cc`  
		Last Modified: Fri, 11 Feb 2022 23:58:41 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:1-alpine3.15`

```console
$ docker pull memcached@sha256:76e5acd480d7bd36706f7873f5f7278ff5085b62840afffc3cefbcef0a3a9509
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
$ docker pull memcached@sha256:e79dd6dea75bf64de1cd87b2204574865bcc12fcda9e1d5c63ce82e3271d4bdf
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.3 MB (5345174 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31403aa3ac88632da679879fcb0a3a627c6f50ec7da0659ae032f63d289d9587`
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
# Fri, 11 Feb 2022 23:43:32 GMT
ENV MEMCACHED_VERSION=1.6.14
# Fri, 11 Feb 2022 23:43:32 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Fri, 11 Feb 2022 23:47:43 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Fri, 11 Feb 2022 23:47:43 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 11 Feb 2022 23:47:44 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 11 Feb 2022 23:47:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Feb 2022 23:47:44 GMT
USER memcache
# Fri, 11 Feb 2022 23:47:45 GMT
EXPOSE 11211
# Fri, 11 Feb 2022 23:47:45 GMT
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
	-	`sha256:4afc0667aa68ec7c0a865809dcfee799f6357b1f6d6c4d6e58240cff71c6264d`  
		Last Modified: Fri, 11 Feb 2022 23:48:39 GMT  
		Size: 2.4 MB (2415863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef8943e1197199b34fc9e9230f24d760a30cdcf11c6b8fc48e89592e00da6edf`  
		Last Modified: Fri, 11 Feb 2022 23:48:38 GMT  
		Size: 283.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b10635796b46c66fb5447019c111ad88d5b808536aab4757aa60b57ffcc9d0da`  
		Last Modified: Fri, 11 Feb 2022 23:48:38 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-alpine3.15` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:c28cbb9d278a2ef6c4ef325c2fffa8bc4631258a341cb411d2a7bec9655007cb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.1 MB (5109831 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e10238b3468650bbfa09ac13b6115339c5305e3e92cb34bb47b6a03b2a93df01`
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
# Fri, 11 Feb 2022 23:59:43 GMT
ENV MEMCACHED_VERSION=1.6.14
# Fri, 11 Feb 2022 23:59:44 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Sat, 12 Feb 2022 00:02:34 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Sat, 12 Feb 2022 00:02:36 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Sat, 12 Feb 2022 00:02:36 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Sat, 12 Feb 2022 00:02:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 12 Feb 2022 00:02:38 GMT
USER memcache
# Sat, 12 Feb 2022 00:02:39 GMT
EXPOSE 11211
# Sat, 12 Feb 2022 00:02:40 GMT
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
	-	`sha256:98b2012c64d2efed092c8ec83344fc68be38873465f9e7b82616b504ca67ea14`  
		Last Modified: Sat, 12 Feb 2022 00:03:57 GMT  
		Size: 2.3 MB (2282236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b54695eeb42571708a7da87031a54d3f82b1be9e474102eeaa912ee51cb86d3`  
		Last Modified: Sat, 12 Feb 2022 00:03:57 GMT  
		Size: 283.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17690cc3c867c822f67c6edabb66fd363b8988e13ed76d6b2a512a4af041bd58`  
		Last Modified: Sat, 12 Feb 2022 00:03:57 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-alpine3.15` - linux; 386

```console
$ docker pull memcached@sha256:5b9731ba5ab72d85a6ed73548a502d6e22d512f328daacddeb531c252745a1e7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.4 MB (5369203 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:83c422eacdcda2fa728cc1fc176ab0cd57a0be7766f0b517dcc64045b255d0a9`
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
# Fri, 11 Feb 2022 23:43:00 GMT
ENV MEMCACHED_VERSION=1.6.14
# Fri, 11 Feb 2022 23:43:01 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Fri, 11 Feb 2022 23:47:20 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Fri, 11 Feb 2022 23:47:20 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 11 Feb 2022 23:47:21 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 11 Feb 2022 23:47:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Feb 2022 23:47:22 GMT
USER memcache
# Fri, 11 Feb 2022 23:47:22 GMT
EXPOSE 11211
# Fri, 11 Feb 2022 23:47:22 GMT
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
	-	`sha256:62d0cbe6f51da8f3bfd9d0bfbbb510f173b231cfc4260066e5da12995d012223`  
		Last Modified: Fri, 11 Feb 2022 23:48:48 GMT  
		Size: 2.4 MB (2419277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfa2ab27dc5f099b91f7195a3d75e51e7f2c84ea56052a565dcbeba235da559b`  
		Last Modified: Fri, 11 Feb 2022 23:48:47 GMT  
		Size: 283.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0394921490062e0dab12bc6f8a3a5bd3f1a97dc261653593a22e3fa95776186`  
		Last Modified: Fri, 11 Feb 2022 23:48:47 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-alpine3.15` - linux; ppc64le

```console
$ docker pull memcached@sha256:75cb5141098fb02bb0c554c31c00d28802b414593a6b41d430c10505ee943fe0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.3 MB (5315837 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4be74852968716dd05ad711f1cda531afac5b782fe0dd6692e5aed7d91d54466`
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
# Fri, 11 Feb 2022 23:54:02 GMT
ENV MEMCACHED_VERSION=1.6.14
# Fri, 11 Feb 2022 23:54:06 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Fri, 11 Feb 2022 23:57:48 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Fri, 11 Feb 2022 23:57:50 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 11 Feb 2022 23:57:55 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 11 Feb 2022 23:57:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Feb 2022 23:57:59 GMT
USER memcache
# Fri, 11 Feb 2022 23:58:01 GMT
EXPOSE 11211
# Fri, 11 Feb 2022 23:58:02 GMT
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
	-	`sha256:e9d933f0d59015113f25123de9b3460a03fdf091181f4c9330b1bb42c27a8cce`  
		Last Modified: Fri, 11 Feb 2022 23:59:16 GMT  
		Size: 2.4 MB (2373175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:659fd1f60c2bc05966f606e677370eeee3176f7d6dbd530b3f271ba313f8b0fe`  
		Last Modified: Fri, 11 Feb 2022 23:59:15 GMT  
		Size: 282.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8d9d86e7310ff252ce602224ce1643c6b8d50713444e43804cdb93912f89087`  
		Last Modified: Fri, 11 Feb 2022 23:59:15 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-alpine3.15` - linux; s390x

```console
$ docker pull memcached@sha256:05d8b33e1a3927fd3ba6b7cd62b648d66a4f07da15103657791736e70515bd20
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4869494 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a751c73ff4357b7992c0a524e080537c462baa079ef3c7b96a3ce7b13699135`
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
# Fri, 11 Feb 2022 23:53:09 GMT
ENV MEMCACHED_VERSION=1.6.14
# Fri, 11 Feb 2022 23:53:09 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Fri, 11 Feb 2022 23:57:25 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Fri, 11 Feb 2022 23:57:25 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 11 Feb 2022 23:57:26 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 11 Feb 2022 23:57:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Feb 2022 23:57:26 GMT
USER memcache
# Fri, 11 Feb 2022 23:57:26 GMT
EXPOSE 11211
# Fri, 11 Feb 2022 23:57:26 GMT
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
	-	`sha256:7bccd1e890d9edaaa99814caec66d49d04d5245aca1fe8a2ac832be7e0e09c06`  
		Last Modified: Fri, 11 Feb 2022 23:58:42 GMT  
		Size: 2.1 MB (2148137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75931a88b924783decffcbf2e1fba6e58f393e9409dd37ffb26b7f6eecffdef2`  
		Last Modified: Fri, 11 Feb 2022 23:58:41 GMT  
		Size: 282.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2dd123370c89ee375732af5193be621336dd45eae2b9729fb66d0376bc915cc`  
		Last Modified: Fri, 11 Feb 2022 23:58:41 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:1-bullseye`

```console
$ docker pull memcached@sha256:e4bb2d212309e51166f29fe5404edf5caf784ada9ab3fde8dcf8226f337878aa
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
$ docker pull memcached@sha256:2c29149daad601e046074c6801fb570180d4eba60047135b71f51ea327ffcbc1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.0 MB (32954984 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6208dafa350f4dfbb3f2a16e20c2f2d256f894fd8695ac24b21663a732dee124`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 01 Mar 2022 02:13:29 GMT
ADD file:d48a85028743f16ed927507322e3e3beee187fbfadd0b781d4b89de197c64b5b in / 
# Tue, 01 Mar 2022 02:13:29 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 13:24:57 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 01 Mar 2022 13:25:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 13:25:02 GMT
ENV MEMCACHED_VERSION=1.6.14
# Tue, 01 Mar 2022 13:25:02 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Tue, 01 Mar 2022 13:28:58 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 01 Mar 2022 13:28:58 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 01 Mar 2022 13:28:59 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 01 Mar 2022 13:28:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 01 Mar 2022 13:29:00 GMT
USER memcache
# Tue, 01 Mar 2022 13:29:00 GMT
EXPOSE 11211
# Tue, 01 Mar 2022 13:29:00 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:f7a1c6dad28192bd417b78079d6ddc03cbca6d5ea46bba12769b235b6353c00c`  
		Last Modified: Tue, 01 Mar 2022 02:19:23 GMT  
		Size: 31.4 MB (31366396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3292b9ed039a5211ec564a1f170046ba2ad296a19beb778d3c7106a230301d27`  
		Last Modified: Tue, 01 Mar 2022 13:29:33 GMT  
		Size: 5.0 KB (4980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15c683705067bdb5151c087a9b5e91a37f498912588e29970e3ce07121334f03`  
		Last Modified: Tue, 01 Mar 2022 13:29:34 GMT  
		Size: 328.0 KB (328033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:091c46e57219c5fdd0a044c77fc12a24889bd1ce95e4d032e83f2ea09997ca1d`  
		Last Modified: Tue, 01 Mar 2022 13:29:34 GMT  
		Size: 1.3 MB (1255168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a26e7e13ba905fd75a5e3b2307ab4abee1bbcdc9b586d37fc2ff7984de1c92c3`  
		Last Modified: Tue, 01 Mar 2022 13:29:33 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75b625708cf5e763937f326c6fe55adcb4c4782926483ea2a3628012927922c7`  
		Last Modified: Tue, 01 Mar 2022 13:29:33 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-bullseye` - linux; arm variant v5

```console
$ docker pull memcached@sha256:839b663c2a5637a5a026d8bf63f2c3a5af62938b6becb246fe84e68bceb73742
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.5 MB (30457903 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:46c3d2c41f175e70fa19ec073355fc3376f15b3ca99f6fdb295b6cea57aede38`
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
# Fri, 11 Feb 2022 23:48:33 GMT
ENV MEMCACHED_VERSION=1.6.14
# Fri, 11 Feb 2022 23:48:33 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Fri, 11 Feb 2022 23:53:18 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Fri, 11 Feb 2022 23:53:19 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 11 Feb 2022 23:53:20 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 11 Feb 2022 23:53:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Feb 2022 23:53:21 GMT
USER memcache
# Fri, 11 Feb 2022 23:53:22 GMT
EXPOSE 11211
# Fri, 11 Feb 2022 23:53:22 GMT
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
	-	`sha256:4c595fdbb4287a9ef2b3565e1d9ac2caa7d17ac0810224d8a5d3c87313cc81b5`  
		Last Modified: Fri, 11 Feb 2022 23:54:16 GMT  
		Size: 1.2 MB (1226376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19c8ecb542750e6e603057b1e7bdb90fc58d45b604f20b2724d402a572f1b735`  
		Last Modified: Fri, 11 Feb 2022 23:54:15 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64d2e913eaab741b412c8fec5edbad97daed3a2c5f0a1a1fd376ea8ec7c28c52`  
		Last Modified: Fri, 11 Feb 2022 23:54:15 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-bullseye` - linux; arm variant v7

```console
$ docker pull memcached@sha256:c1ded327e0d4c11f7f00652600f4cbf465a119fed31e6e2541d516700e0e14c2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.1 MB (28080208 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:866cf84302a62bedfada61f236deccacb7585dc0ccce8a4e0e058b741bfafdc5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 01 Mar 2022 02:02:56 GMT
ADD file:c6b519323fd1fa09b9f8c8608778872e8fa6208cb0b42aaccdef4479a469f5f4 in / 
# Tue, 01 Mar 2022 02:02:57 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 14:02:17 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 01 Mar 2022 14:02:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 14:02:26 GMT
ENV MEMCACHED_VERSION=1.6.14
# Tue, 01 Mar 2022 14:02:26 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Tue, 01 Mar 2022 14:06:15 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 01 Mar 2022 14:06:16 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 01 Mar 2022 14:06:17 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 01 Mar 2022 14:06:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 01 Mar 2022 14:06:18 GMT
USER memcache
# Tue, 01 Mar 2022 14:06:19 GMT
EXPOSE 11211
# Tue, 01 Mar 2022 14:06:19 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:59dbb2ac3829352dd707e28e037734c9fbdef5b03aea31e3929ddcead949afee`  
		Last Modified: Tue, 01 Mar 2022 02:19:09 GMT  
		Size: 26.6 MB (26565105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45ff8679190bbfe567a01e354c79eb44efaa4564b0770a644b9eb6a28f10812c`  
		Last Modified: Tue, 01 Mar 2022 14:19:16 GMT  
		Size: 4.9 KB (4894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13db11031aa185885b3b1b9c74eba0d8ea9b07d5e8fec5870bc7df8d09585d2f`  
		Last Modified: Tue, 01 Mar 2022 14:19:16 GMT  
		Size: 312.0 KB (312009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:079efee4f8d1e8cea53f0cc6ddc4832de31e69c43411b81e790e0615eeea16aa`  
		Last Modified: Tue, 01 Mar 2022 14:19:16 GMT  
		Size: 1.2 MB (1197793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:050fbe09656330899bb983ba6d0871a6cc96349c4c049673a4ee53816db5ff7b`  
		Last Modified: Tue, 01 Mar 2022 14:19:16 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcca636453f4acf7b597c080e2d7c57ea366f36daae56acdd43664bb28dff985`  
		Last Modified: Tue, 01 Mar 2022 14:19:16 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-bullseye` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:c59ae38d83ce474dc14423325e3f500a06e285938b4f4e8a013ae8967603d492
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.4 MB (31435417 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b5c5ad61ebd09fab08b612599fdf9e96be59696045e4765dac554781daef4d1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 01 Mar 2022 02:11:29 GMT
ADD file:9816c9c29627693c34afda4fa5e1a5e8a0f5aa3c5d5cfd920a4d89c77aab997d in / 
# Tue, 01 Mar 2022 02:11:30 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 12:44:12 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 01 Mar 2022 12:44:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 12:44:16 GMT
ENV MEMCACHED_VERSION=1.6.14
# Tue, 01 Mar 2022 12:44:17 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Tue, 01 Mar 2022 12:46:49 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 01 Mar 2022 12:46:50 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 01 Mar 2022 12:46:50 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 01 Mar 2022 12:46:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 01 Mar 2022 12:46:52 GMT
USER memcache
# Tue, 01 Mar 2022 12:46:53 GMT
EXPOSE 11211
# Tue, 01 Mar 2022 12:46:54 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:279a020076a7fbddfc996e4c55e605a8f322810c3eca21cdedbcb06beb0e1305`  
		Last Modified: Tue, 01 Mar 2022 02:18:24 GMT  
		Size: 30.1 MB (30057008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7dfd1ea3d9e177e785365db9a22591801c15e6a33097ba79a048e3387f4c43a`  
		Last Modified: Tue, 01 Mar 2022 12:47:45 GMT  
		Size: 4.9 KB (4902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e563a531f0653c96d3786deff2afe7190769b5929d06c8c234d89fd314bf2396`  
		Last Modified: Tue, 01 Mar 2022 12:47:45 GMT  
		Size: 119.2 KB (119172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1d1b1b990f1e4e95a5410acd589565956a1fd54c4df3b71a665dcfb23ac9f76`  
		Last Modified: Tue, 01 Mar 2022 12:47:46 GMT  
		Size: 1.3 MB (1253928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b8a7c0be94d102b9a04c359186fcf59b223183acc8b489d0ca12afb8f073027`  
		Last Modified: Tue, 01 Mar 2022 12:47:45 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:091c7ee2fb4e34177c30b2b9905bf098f304bea040ff7ca5700134d4921c2758`  
		Last Modified: Tue, 01 Mar 2022 12:47:45 GMT  
		Size: 120.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-bullseye` - linux; 386

```console
$ docker pull memcached@sha256:4c9eb4902e2601bad18a1783dbf7d64cf25f6121226d4772a5d36a7ac3e9db79
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.0 MB (33972554 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af09c75e25cf0ea60c4f155a25728e256411f07898946ea08e869eb6362e3a24`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 01 Mar 2022 02:07:32 GMT
ADD file:e92ab504d4c0d3bd63da83254e6ca400b607c32e0f5037039648559b91770870 in / 
# Tue, 01 Mar 2022 02:07:33 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 10:07:23 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 01 Mar 2022 10:07:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 10:07:30 GMT
ENV MEMCACHED_VERSION=1.6.14
# Tue, 01 Mar 2022 10:07:30 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Tue, 01 Mar 2022 10:11:57 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 01 Mar 2022 10:11:57 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 01 Mar 2022 10:11:58 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 01 Mar 2022 10:11:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 01 Mar 2022 10:11:58 GMT
USER memcache
# Tue, 01 Mar 2022 10:11:58 GMT
EXPOSE 11211
# Tue, 01 Mar 2022 10:11:59 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:04a87e821be7e4b29d48011b7aa4ff884ca57fd36995cb3b99fd2fc24ac562d8`  
		Last Modified: Tue, 01 Mar 2022 02:15:51 GMT  
		Size: 32.4 MB (32377389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe860ecc70fbef589f9779541d957321138c3f41d99742ca7ff2bb41b6787786`  
		Last Modified: Tue, 01 Mar 2022 10:13:02 GMT  
		Size: 4.9 KB (4889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71fbbf846282a29c58595e09b8a5d93a6348fc5a77d0bb513263f933972610e8`  
		Last Modified: Tue, 01 Mar 2022 10:13:03 GMT  
		Size: 336.6 KB (336603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f93f31af2adb455df5e2c7baaa190b479d463d37657734ee855d663709906a2`  
		Last Modified: Tue, 01 Mar 2022 10:13:03 GMT  
		Size: 1.3 MB (1253268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ea06973bd5c70feb976fde3006e5400760f293973d5a2a8f8a05a73105a5851`  
		Last Modified: Tue, 01 Mar 2022 10:13:02 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c85296c039a2ca9f99139e04d26550a26b109424a80e9377a115129110257b9`  
		Last Modified: Tue, 01 Mar 2022 10:13:02 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-bullseye` - linux; mips64le

```console
$ docker pull memcached@sha256:76269e61918b56719946fa47ffaebf468965e45dae401738fcd6d8ea6d9afdc1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.2 MB (31213138 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bdf2a1611553c4acfb426a9736777620af35250c1c3fde4997dd8fda25547725`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 01 Mar 2022 02:02:49 GMT
ADD file:1901e1e1292cbfcd557262ec5d08551cecd0070b24928414d220472664fe3fdf in / 
# Tue, 01 Mar 2022 02:02:49 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 03:43:18 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 01 Mar 2022 03:43:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 03:43:30 GMT
ENV MEMCACHED_VERSION=1.6.14
# Tue, 01 Mar 2022 03:43:30 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Tue, 01 Mar 2022 03:49:17 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 01 Mar 2022 03:49:17 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 01 Mar 2022 03:49:19 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 01 Mar 2022 03:49:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 01 Mar 2022 03:49:20 GMT
USER memcache
# Tue, 01 Mar 2022 03:49:20 GMT
EXPOSE 11211
# Tue, 01 Mar 2022 03:49:20 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:3baeb8c34a522fc616f97412d47dc1f665e93552c57aa8237ee1d673f9757cba`  
		Last Modified: Tue, 01 Mar 2022 02:12:25 GMT  
		Size: 29.6 MB (29632966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50a63f21594c0da6641452e9cd0caaf8727bae4ca86c617384198ab5d8e766ec`  
		Last Modified: Tue, 01 Mar 2022 03:49:43 GMT  
		Size: 5.0 KB (4979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dfb3a0cb8d59939fa0e67d13c57840042b1397d36d3c1918e50344eb405025d`  
		Last Modified: Tue, 01 Mar 2022 03:49:43 GMT  
		Size: 323.7 KB (323703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e632b2b5bf88ea94d56d701fa93b55516003db1fc7c855bb4569f2be0ddf3be`  
		Last Modified: Tue, 01 Mar 2022 03:49:43 GMT  
		Size: 1.3 MB (1251083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1fc0f9b2a7499de336af3103d86d1ffc3b90b62ea850295c0c57abbe68c753b`  
		Last Modified: Tue, 01 Mar 2022 03:49:43 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe1ee7b4dd056bb3eadc09b9893ce88a096e51500bbe841d1c145be10ba2b1f0`  
		Last Modified: Tue, 01 Mar 2022 03:49:43 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-bullseye` - linux; ppc64le

```console
$ docker pull memcached@sha256:4893f4daa742b31f414b08f98f8e7d0cbedaf63b8d88062bcf3c91a9522a2aab
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.0 MB (36957544 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8db953cc998ed06712eca57fe4ae2b8bb342ce991683fd7592495a21557d0940`
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
# Fri, 11 Feb 2022 23:47:36 GMT
ENV MEMCACHED_VERSION=1.6.14
# Fri, 11 Feb 2022 23:47:38 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Fri, 11 Feb 2022 23:53:07 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Fri, 11 Feb 2022 23:53:13 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 11 Feb 2022 23:53:34 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 11 Feb 2022 23:53:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Feb 2022 23:53:39 GMT
USER memcache
# Fri, 11 Feb 2022 23:53:41 GMT
EXPOSE 11211
# Fri, 11 Feb 2022 23:53:46 GMT
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
	-	`sha256:d5f2e5d5bb1609e336a37e97218d618550ec5ce28384c32b1141393ef6f04a03`  
		Last Modified: Fri, 11 Feb 2022 23:58:44 GMT  
		Size: 1.3 MB (1322220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76e6da4f290b1cff2fa5b1ad17d42333c67179332511db4da3bd2c5ce12bbdfa`  
		Last Modified: Fri, 11 Feb 2022 23:58:44 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fb140c5468aa121999bc169d30e4ce6b73795cdf67aa21c1dfd3d1194dd0b82`  
		Last Modified: Fri, 11 Feb 2022 23:58:44 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-bullseye` - linux; s390x

```console
$ docker pull memcached@sha256:14b3ae46a3b5dc4d1ca410da43e53ee0c44ad49ec398f235628f89bc8cc0a0cc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.2 MB (31217166 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:50f1b3aef9bc393e3b1a3fab35c702d6a9b9dd6fa2abd9d044b52385b9ccf549`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 01 Mar 2022 02:01:56 GMT
ADD file:d869ad3392a4e752c2f73d08a4cc13594c94bfc050bd037db0ca9827a0207072 in / 
# Tue, 01 Mar 2022 02:01:58 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 13:28:37 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 01 Mar 2022 13:28:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 13:28:40 GMT
ENV MEMCACHED_VERSION=1.6.14
# Tue, 01 Mar 2022 13:28:40 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Tue, 01 Mar 2022 13:31:58 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 01 Mar 2022 13:31:58 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 01 Mar 2022 13:31:58 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 01 Mar 2022 13:31:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 01 Mar 2022 13:31:59 GMT
USER memcache
# Tue, 01 Mar 2022 13:31:59 GMT
EXPOSE 11211
# Tue, 01 Mar 2022 13:31:59 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:f81abce72636770dac4258df46a31beeb6ad81dfddd5b7c9c3fa6942ea074922`  
		Last Modified: Tue, 01 Mar 2022 02:07:33 GMT  
		Size: 29.6 MB (29647132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b43f274641c42412c1e075acb3920020215603d1e1c938fa84211ea8b005988`  
		Last Modified: Tue, 01 Mar 2022 13:32:52 GMT  
		Size: 5.0 KB (5024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d135f121f1aff6ea16284d2286318c703c72dad45560bdc68ac2bc2371f8164`  
		Last Modified: Tue, 01 Mar 2022 13:32:52 GMT  
		Size: 324.1 KB (324102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9255401f181741c77541d42f93796b72c20077b2815b9e6c4e21b36f9bcccab6`  
		Last Modified: Tue, 01 Mar 2022 13:32:52 GMT  
		Size: 1.2 MB (1240500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5436de37a983faa64cc9d82c3a8272ae77b107e2f8bcd453f7aee5e3e92def7`  
		Last Modified: Tue, 01 Mar 2022 13:32:52 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8296feb21176186e1c4027cf5e8111ed103c7b2b30f1f4423a9303a0e7fd9d3`  
		Last Modified: Tue, 01 Mar 2022 13:32:52 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:1.6`

```console
$ docker pull memcached@sha256:e4bb2d212309e51166f29fe5404edf5caf784ada9ab3fde8dcf8226f337878aa
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
$ docker pull memcached@sha256:2c29149daad601e046074c6801fb570180d4eba60047135b71f51ea327ffcbc1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.0 MB (32954984 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6208dafa350f4dfbb3f2a16e20c2f2d256f894fd8695ac24b21663a732dee124`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 01 Mar 2022 02:13:29 GMT
ADD file:d48a85028743f16ed927507322e3e3beee187fbfadd0b781d4b89de197c64b5b in / 
# Tue, 01 Mar 2022 02:13:29 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 13:24:57 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 01 Mar 2022 13:25:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 13:25:02 GMT
ENV MEMCACHED_VERSION=1.6.14
# Tue, 01 Mar 2022 13:25:02 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Tue, 01 Mar 2022 13:28:58 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 01 Mar 2022 13:28:58 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 01 Mar 2022 13:28:59 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 01 Mar 2022 13:28:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 01 Mar 2022 13:29:00 GMT
USER memcache
# Tue, 01 Mar 2022 13:29:00 GMT
EXPOSE 11211
# Tue, 01 Mar 2022 13:29:00 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:f7a1c6dad28192bd417b78079d6ddc03cbca6d5ea46bba12769b235b6353c00c`  
		Last Modified: Tue, 01 Mar 2022 02:19:23 GMT  
		Size: 31.4 MB (31366396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3292b9ed039a5211ec564a1f170046ba2ad296a19beb778d3c7106a230301d27`  
		Last Modified: Tue, 01 Mar 2022 13:29:33 GMT  
		Size: 5.0 KB (4980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15c683705067bdb5151c087a9b5e91a37f498912588e29970e3ce07121334f03`  
		Last Modified: Tue, 01 Mar 2022 13:29:34 GMT  
		Size: 328.0 KB (328033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:091c46e57219c5fdd0a044c77fc12a24889bd1ce95e4d032e83f2ea09997ca1d`  
		Last Modified: Tue, 01 Mar 2022 13:29:34 GMT  
		Size: 1.3 MB (1255168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a26e7e13ba905fd75a5e3b2307ab4abee1bbcdc9b586d37fc2ff7984de1c92c3`  
		Last Modified: Tue, 01 Mar 2022 13:29:33 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75b625708cf5e763937f326c6fe55adcb4c4782926483ea2a3628012927922c7`  
		Last Modified: Tue, 01 Mar 2022 13:29:33 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6` - linux; arm variant v5

```console
$ docker pull memcached@sha256:839b663c2a5637a5a026d8bf63f2c3a5af62938b6becb246fe84e68bceb73742
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.5 MB (30457903 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:46c3d2c41f175e70fa19ec073355fc3376f15b3ca99f6fdb295b6cea57aede38`
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
# Fri, 11 Feb 2022 23:48:33 GMT
ENV MEMCACHED_VERSION=1.6.14
# Fri, 11 Feb 2022 23:48:33 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Fri, 11 Feb 2022 23:53:18 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Fri, 11 Feb 2022 23:53:19 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 11 Feb 2022 23:53:20 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 11 Feb 2022 23:53:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Feb 2022 23:53:21 GMT
USER memcache
# Fri, 11 Feb 2022 23:53:22 GMT
EXPOSE 11211
# Fri, 11 Feb 2022 23:53:22 GMT
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
	-	`sha256:4c595fdbb4287a9ef2b3565e1d9ac2caa7d17ac0810224d8a5d3c87313cc81b5`  
		Last Modified: Fri, 11 Feb 2022 23:54:16 GMT  
		Size: 1.2 MB (1226376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19c8ecb542750e6e603057b1e7bdb90fc58d45b604f20b2724d402a572f1b735`  
		Last Modified: Fri, 11 Feb 2022 23:54:15 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64d2e913eaab741b412c8fec5edbad97daed3a2c5f0a1a1fd376ea8ec7c28c52`  
		Last Modified: Fri, 11 Feb 2022 23:54:15 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6` - linux; arm variant v7

```console
$ docker pull memcached@sha256:c1ded327e0d4c11f7f00652600f4cbf465a119fed31e6e2541d516700e0e14c2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.1 MB (28080208 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:866cf84302a62bedfada61f236deccacb7585dc0ccce8a4e0e058b741bfafdc5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 01 Mar 2022 02:02:56 GMT
ADD file:c6b519323fd1fa09b9f8c8608778872e8fa6208cb0b42aaccdef4479a469f5f4 in / 
# Tue, 01 Mar 2022 02:02:57 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 14:02:17 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 01 Mar 2022 14:02:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 14:02:26 GMT
ENV MEMCACHED_VERSION=1.6.14
# Tue, 01 Mar 2022 14:02:26 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Tue, 01 Mar 2022 14:06:15 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 01 Mar 2022 14:06:16 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 01 Mar 2022 14:06:17 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 01 Mar 2022 14:06:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 01 Mar 2022 14:06:18 GMT
USER memcache
# Tue, 01 Mar 2022 14:06:19 GMT
EXPOSE 11211
# Tue, 01 Mar 2022 14:06:19 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:59dbb2ac3829352dd707e28e037734c9fbdef5b03aea31e3929ddcead949afee`  
		Last Modified: Tue, 01 Mar 2022 02:19:09 GMT  
		Size: 26.6 MB (26565105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45ff8679190bbfe567a01e354c79eb44efaa4564b0770a644b9eb6a28f10812c`  
		Last Modified: Tue, 01 Mar 2022 14:19:16 GMT  
		Size: 4.9 KB (4894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13db11031aa185885b3b1b9c74eba0d8ea9b07d5e8fec5870bc7df8d09585d2f`  
		Last Modified: Tue, 01 Mar 2022 14:19:16 GMT  
		Size: 312.0 KB (312009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:079efee4f8d1e8cea53f0cc6ddc4832de31e69c43411b81e790e0615eeea16aa`  
		Last Modified: Tue, 01 Mar 2022 14:19:16 GMT  
		Size: 1.2 MB (1197793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:050fbe09656330899bb983ba6d0871a6cc96349c4c049673a4ee53816db5ff7b`  
		Last Modified: Tue, 01 Mar 2022 14:19:16 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcca636453f4acf7b597c080e2d7c57ea366f36daae56acdd43664bb28dff985`  
		Last Modified: Tue, 01 Mar 2022 14:19:16 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:c59ae38d83ce474dc14423325e3f500a06e285938b4f4e8a013ae8967603d492
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.4 MB (31435417 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b5c5ad61ebd09fab08b612599fdf9e96be59696045e4765dac554781daef4d1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 01 Mar 2022 02:11:29 GMT
ADD file:9816c9c29627693c34afda4fa5e1a5e8a0f5aa3c5d5cfd920a4d89c77aab997d in / 
# Tue, 01 Mar 2022 02:11:30 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 12:44:12 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 01 Mar 2022 12:44:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 12:44:16 GMT
ENV MEMCACHED_VERSION=1.6.14
# Tue, 01 Mar 2022 12:44:17 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Tue, 01 Mar 2022 12:46:49 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 01 Mar 2022 12:46:50 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 01 Mar 2022 12:46:50 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 01 Mar 2022 12:46:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 01 Mar 2022 12:46:52 GMT
USER memcache
# Tue, 01 Mar 2022 12:46:53 GMT
EXPOSE 11211
# Tue, 01 Mar 2022 12:46:54 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:279a020076a7fbddfc996e4c55e605a8f322810c3eca21cdedbcb06beb0e1305`  
		Last Modified: Tue, 01 Mar 2022 02:18:24 GMT  
		Size: 30.1 MB (30057008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7dfd1ea3d9e177e785365db9a22591801c15e6a33097ba79a048e3387f4c43a`  
		Last Modified: Tue, 01 Mar 2022 12:47:45 GMT  
		Size: 4.9 KB (4902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e563a531f0653c96d3786deff2afe7190769b5929d06c8c234d89fd314bf2396`  
		Last Modified: Tue, 01 Mar 2022 12:47:45 GMT  
		Size: 119.2 KB (119172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1d1b1b990f1e4e95a5410acd589565956a1fd54c4df3b71a665dcfb23ac9f76`  
		Last Modified: Tue, 01 Mar 2022 12:47:46 GMT  
		Size: 1.3 MB (1253928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b8a7c0be94d102b9a04c359186fcf59b223183acc8b489d0ca12afb8f073027`  
		Last Modified: Tue, 01 Mar 2022 12:47:45 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:091c7ee2fb4e34177c30b2b9905bf098f304bea040ff7ca5700134d4921c2758`  
		Last Modified: Tue, 01 Mar 2022 12:47:45 GMT  
		Size: 120.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6` - linux; 386

```console
$ docker pull memcached@sha256:4c9eb4902e2601bad18a1783dbf7d64cf25f6121226d4772a5d36a7ac3e9db79
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.0 MB (33972554 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af09c75e25cf0ea60c4f155a25728e256411f07898946ea08e869eb6362e3a24`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 01 Mar 2022 02:07:32 GMT
ADD file:e92ab504d4c0d3bd63da83254e6ca400b607c32e0f5037039648559b91770870 in / 
# Tue, 01 Mar 2022 02:07:33 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 10:07:23 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 01 Mar 2022 10:07:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 10:07:30 GMT
ENV MEMCACHED_VERSION=1.6.14
# Tue, 01 Mar 2022 10:07:30 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Tue, 01 Mar 2022 10:11:57 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 01 Mar 2022 10:11:57 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 01 Mar 2022 10:11:58 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 01 Mar 2022 10:11:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 01 Mar 2022 10:11:58 GMT
USER memcache
# Tue, 01 Mar 2022 10:11:58 GMT
EXPOSE 11211
# Tue, 01 Mar 2022 10:11:59 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:04a87e821be7e4b29d48011b7aa4ff884ca57fd36995cb3b99fd2fc24ac562d8`  
		Last Modified: Tue, 01 Mar 2022 02:15:51 GMT  
		Size: 32.4 MB (32377389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe860ecc70fbef589f9779541d957321138c3f41d99742ca7ff2bb41b6787786`  
		Last Modified: Tue, 01 Mar 2022 10:13:02 GMT  
		Size: 4.9 KB (4889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71fbbf846282a29c58595e09b8a5d93a6348fc5a77d0bb513263f933972610e8`  
		Last Modified: Tue, 01 Mar 2022 10:13:03 GMT  
		Size: 336.6 KB (336603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f93f31af2adb455df5e2c7baaa190b479d463d37657734ee855d663709906a2`  
		Last Modified: Tue, 01 Mar 2022 10:13:03 GMT  
		Size: 1.3 MB (1253268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ea06973bd5c70feb976fde3006e5400760f293973d5a2a8f8a05a73105a5851`  
		Last Modified: Tue, 01 Mar 2022 10:13:02 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c85296c039a2ca9f99139e04d26550a26b109424a80e9377a115129110257b9`  
		Last Modified: Tue, 01 Mar 2022 10:13:02 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6` - linux; mips64le

```console
$ docker pull memcached@sha256:76269e61918b56719946fa47ffaebf468965e45dae401738fcd6d8ea6d9afdc1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.2 MB (31213138 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bdf2a1611553c4acfb426a9736777620af35250c1c3fde4997dd8fda25547725`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 01 Mar 2022 02:02:49 GMT
ADD file:1901e1e1292cbfcd557262ec5d08551cecd0070b24928414d220472664fe3fdf in / 
# Tue, 01 Mar 2022 02:02:49 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 03:43:18 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 01 Mar 2022 03:43:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 03:43:30 GMT
ENV MEMCACHED_VERSION=1.6.14
# Tue, 01 Mar 2022 03:43:30 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Tue, 01 Mar 2022 03:49:17 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 01 Mar 2022 03:49:17 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 01 Mar 2022 03:49:19 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 01 Mar 2022 03:49:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 01 Mar 2022 03:49:20 GMT
USER memcache
# Tue, 01 Mar 2022 03:49:20 GMT
EXPOSE 11211
# Tue, 01 Mar 2022 03:49:20 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:3baeb8c34a522fc616f97412d47dc1f665e93552c57aa8237ee1d673f9757cba`  
		Last Modified: Tue, 01 Mar 2022 02:12:25 GMT  
		Size: 29.6 MB (29632966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50a63f21594c0da6641452e9cd0caaf8727bae4ca86c617384198ab5d8e766ec`  
		Last Modified: Tue, 01 Mar 2022 03:49:43 GMT  
		Size: 5.0 KB (4979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dfb3a0cb8d59939fa0e67d13c57840042b1397d36d3c1918e50344eb405025d`  
		Last Modified: Tue, 01 Mar 2022 03:49:43 GMT  
		Size: 323.7 KB (323703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e632b2b5bf88ea94d56d701fa93b55516003db1fc7c855bb4569f2be0ddf3be`  
		Last Modified: Tue, 01 Mar 2022 03:49:43 GMT  
		Size: 1.3 MB (1251083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1fc0f9b2a7499de336af3103d86d1ffc3b90b62ea850295c0c57abbe68c753b`  
		Last Modified: Tue, 01 Mar 2022 03:49:43 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe1ee7b4dd056bb3eadc09b9893ce88a096e51500bbe841d1c145be10ba2b1f0`  
		Last Modified: Tue, 01 Mar 2022 03:49:43 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6` - linux; ppc64le

```console
$ docker pull memcached@sha256:4893f4daa742b31f414b08f98f8e7d0cbedaf63b8d88062bcf3c91a9522a2aab
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.0 MB (36957544 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8db953cc998ed06712eca57fe4ae2b8bb342ce991683fd7592495a21557d0940`
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
# Fri, 11 Feb 2022 23:47:36 GMT
ENV MEMCACHED_VERSION=1.6.14
# Fri, 11 Feb 2022 23:47:38 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Fri, 11 Feb 2022 23:53:07 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Fri, 11 Feb 2022 23:53:13 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 11 Feb 2022 23:53:34 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 11 Feb 2022 23:53:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Feb 2022 23:53:39 GMT
USER memcache
# Fri, 11 Feb 2022 23:53:41 GMT
EXPOSE 11211
# Fri, 11 Feb 2022 23:53:46 GMT
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
	-	`sha256:d5f2e5d5bb1609e336a37e97218d618550ec5ce28384c32b1141393ef6f04a03`  
		Last Modified: Fri, 11 Feb 2022 23:58:44 GMT  
		Size: 1.3 MB (1322220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76e6da4f290b1cff2fa5b1ad17d42333c67179332511db4da3bd2c5ce12bbdfa`  
		Last Modified: Fri, 11 Feb 2022 23:58:44 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fb140c5468aa121999bc169d30e4ce6b73795cdf67aa21c1dfd3d1194dd0b82`  
		Last Modified: Fri, 11 Feb 2022 23:58:44 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6` - linux; s390x

```console
$ docker pull memcached@sha256:14b3ae46a3b5dc4d1ca410da43e53ee0c44ad49ec398f235628f89bc8cc0a0cc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.2 MB (31217166 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:50f1b3aef9bc393e3b1a3fab35c702d6a9b9dd6fa2abd9d044b52385b9ccf549`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 01 Mar 2022 02:01:56 GMT
ADD file:d869ad3392a4e752c2f73d08a4cc13594c94bfc050bd037db0ca9827a0207072 in / 
# Tue, 01 Mar 2022 02:01:58 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 13:28:37 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 01 Mar 2022 13:28:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 13:28:40 GMT
ENV MEMCACHED_VERSION=1.6.14
# Tue, 01 Mar 2022 13:28:40 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Tue, 01 Mar 2022 13:31:58 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 01 Mar 2022 13:31:58 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 01 Mar 2022 13:31:58 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 01 Mar 2022 13:31:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 01 Mar 2022 13:31:59 GMT
USER memcache
# Tue, 01 Mar 2022 13:31:59 GMT
EXPOSE 11211
# Tue, 01 Mar 2022 13:31:59 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:f81abce72636770dac4258df46a31beeb6ad81dfddd5b7c9c3fa6942ea074922`  
		Last Modified: Tue, 01 Mar 2022 02:07:33 GMT  
		Size: 29.6 MB (29647132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b43f274641c42412c1e075acb3920020215603d1e1c938fa84211ea8b005988`  
		Last Modified: Tue, 01 Mar 2022 13:32:52 GMT  
		Size: 5.0 KB (5024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d135f121f1aff6ea16284d2286318c703c72dad45560bdc68ac2bc2371f8164`  
		Last Modified: Tue, 01 Mar 2022 13:32:52 GMT  
		Size: 324.1 KB (324102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9255401f181741c77541d42f93796b72c20077b2815b9e6c4e21b36f9bcccab6`  
		Last Modified: Tue, 01 Mar 2022 13:32:52 GMT  
		Size: 1.2 MB (1240500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5436de37a983faa64cc9d82c3a8272ae77b107e2f8bcd453f7aee5e3e92def7`  
		Last Modified: Tue, 01 Mar 2022 13:32:52 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8296feb21176186e1c4027cf5e8111ed103c7b2b30f1f4423a9303a0e7fd9d3`  
		Last Modified: Tue, 01 Mar 2022 13:32:52 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:1.6-alpine`

```console
$ docker pull memcached@sha256:a37fd6c034a7e4334d091beedffb525aae8af4acc0cee3030758ae3edc0c524b
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
$ docker pull memcached@sha256:e79dd6dea75bf64de1cd87b2204574865bcc12fcda9e1d5c63ce82e3271d4bdf
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.3 MB (5345174 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31403aa3ac88632da679879fcb0a3a627c6f50ec7da0659ae032f63d289d9587`
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
# Fri, 11 Feb 2022 23:43:32 GMT
ENV MEMCACHED_VERSION=1.6.14
# Fri, 11 Feb 2022 23:43:32 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Fri, 11 Feb 2022 23:47:43 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Fri, 11 Feb 2022 23:47:43 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 11 Feb 2022 23:47:44 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 11 Feb 2022 23:47:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Feb 2022 23:47:44 GMT
USER memcache
# Fri, 11 Feb 2022 23:47:45 GMT
EXPOSE 11211
# Fri, 11 Feb 2022 23:47:45 GMT
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
	-	`sha256:4afc0667aa68ec7c0a865809dcfee799f6357b1f6d6c4d6e58240cff71c6264d`  
		Last Modified: Fri, 11 Feb 2022 23:48:39 GMT  
		Size: 2.4 MB (2415863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef8943e1197199b34fc9e9230f24d760a30cdcf11c6b8fc48e89592e00da6edf`  
		Last Modified: Fri, 11 Feb 2022 23:48:38 GMT  
		Size: 283.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b10635796b46c66fb5447019c111ad88d5b808536aab4757aa60b57ffcc9d0da`  
		Last Modified: Fri, 11 Feb 2022 23:48:38 GMT  
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
$ docker pull memcached@sha256:c28cbb9d278a2ef6c4ef325c2fffa8bc4631258a341cb411d2a7bec9655007cb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.1 MB (5109831 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e10238b3468650bbfa09ac13b6115339c5305e3e92cb34bb47b6a03b2a93df01`
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
# Fri, 11 Feb 2022 23:59:43 GMT
ENV MEMCACHED_VERSION=1.6.14
# Fri, 11 Feb 2022 23:59:44 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Sat, 12 Feb 2022 00:02:34 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Sat, 12 Feb 2022 00:02:36 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Sat, 12 Feb 2022 00:02:36 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Sat, 12 Feb 2022 00:02:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 12 Feb 2022 00:02:38 GMT
USER memcache
# Sat, 12 Feb 2022 00:02:39 GMT
EXPOSE 11211
# Sat, 12 Feb 2022 00:02:40 GMT
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
	-	`sha256:98b2012c64d2efed092c8ec83344fc68be38873465f9e7b82616b504ca67ea14`  
		Last Modified: Sat, 12 Feb 2022 00:03:57 GMT  
		Size: 2.3 MB (2282236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b54695eeb42571708a7da87031a54d3f82b1be9e474102eeaa912ee51cb86d3`  
		Last Modified: Sat, 12 Feb 2022 00:03:57 GMT  
		Size: 283.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17690cc3c867c822f67c6edabb66fd363b8988e13ed76d6b2a512a4af041bd58`  
		Last Modified: Sat, 12 Feb 2022 00:03:57 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-alpine` - linux; 386

```console
$ docker pull memcached@sha256:5b9731ba5ab72d85a6ed73548a502d6e22d512f328daacddeb531c252745a1e7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.4 MB (5369203 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:83c422eacdcda2fa728cc1fc176ab0cd57a0be7766f0b517dcc64045b255d0a9`
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
# Fri, 11 Feb 2022 23:43:00 GMT
ENV MEMCACHED_VERSION=1.6.14
# Fri, 11 Feb 2022 23:43:01 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Fri, 11 Feb 2022 23:47:20 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Fri, 11 Feb 2022 23:47:20 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 11 Feb 2022 23:47:21 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 11 Feb 2022 23:47:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Feb 2022 23:47:22 GMT
USER memcache
# Fri, 11 Feb 2022 23:47:22 GMT
EXPOSE 11211
# Fri, 11 Feb 2022 23:47:22 GMT
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
	-	`sha256:62d0cbe6f51da8f3bfd9d0bfbbb510f173b231cfc4260066e5da12995d012223`  
		Last Modified: Fri, 11 Feb 2022 23:48:48 GMT  
		Size: 2.4 MB (2419277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfa2ab27dc5f099b91f7195a3d75e51e7f2c84ea56052a565dcbeba235da559b`  
		Last Modified: Fri, 11 Feb 2022 23:48:47 GMT  
		Size: 283.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0394921490062e0dab12bc6f8a3a5bd3f1a97dc261653593a22e3fa95776186`  
		Last Modified: Fri, 11 Feb 2022 23:48:47 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-alpine` - linux; ppc64le

```console
$ docker pull memcached@sha256:75cb5141098fb02bb0c554c31c00d28802b414593a6b41d430c10505ee943fe0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.3 MB (5315837 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4be74852968716dd05ad711f1cda531afac5b782fe0dd6692e5aed7d91d54466`
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
# Fri, 11 Feb 2022 23:54:02 GMT
ENV MEMCACHED_VERSION=1.6.14
# Fri, 11 Feb 2022 23:54:06 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Fri, 11 Feb 2022 23:57:48 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Fri, 11 Feb 2022 23:57:50 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 11 Feb 2022 23:57:55 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 11 Feb 2022 23:57:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Feb 2022 23:57:59 GMT
USER memcache
# Fri, 11 Feb 2022 23:58:01 GMT
EXPOSE 11211
# Fri, 11 Feb 2022 23:58:02 GMT
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
	-	`sha256:e9d933f0d59015113f25123de9b3460a03fdf091181f4c9330b1bb42c27a8cce`  
		Last Modified: Fri, 11 Feb 2022 23:59:16 GMT  
		Size: 2.4 MB (2373175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:659fd1f60c2bc05966f606e677370eeee3176f7d6dbd530b3f271ba313f8b0fe`  
		Last Modified: Fri, 11 Feb 2022 23:59:15 GMT  
		Size: 282.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8d9d86e7310ff252ce602224ce1643c6b8d50713444e43804cdb93912f89087`  
		Last Modified: Fri, 11 Feb 2022 23:59:15 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-alpine` - linux; s390x

```console
$ docker pull memcached@sha256:05d8b33e1a3927fd3ba6b7cd62b648d66a4f07da15103657791736e70515bd20
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4869494 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a751c73ff4357b7992c0a524e080537c462baa079ef3c7b96a3ce7b13699135`
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
# Fri, 11 Feb 2022 23:53:09 GMT
ENV MEMCACHED_VERSION=1.6.14
# Fri, 11 Feb 2022 23:53:09 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Fri, 11 Feb 2022 23:57:25 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Fri, 11 Feb 2022 23:57:25 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 11 Feb 2022 23:57:26 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 11 Feb 2022 23:57:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Feb 2022 23:57:26 GMT
USER memcache
# Fri, 11 Feb 2022 23:57:26 GMT
EXPOSE 11211
# Fri, 11 Feb 2022 23:57:26 GMT
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
	-	`sha256:7bccd1e890d9edaaa99814caec66d49d04d5245aca1fe8a2ac832be7e0e09c06`  
		Last Modified: Fri, 11 Feb 2022 23:58:42 GMT  
		Size: 2.1 MB (2148137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75931a88b924783decffcbf2e1fba6e58f393e9409dd37ffb26b7f6eecffdef2`  
		Last Modified: Fri, 11 Feb 2022 23:58:41 GMT  
		Size: 282.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2dd123370c89ee375732af5193be621336dd45eae2b9729fb66d0376bc915cc`  
		Last Modified: Fri, 11 Feb 2022 23:58:41 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:1.6-alpine3.15`

```console
$ docker pull memcached@sha256:76e5acd480d7bd36706f7873f5f7278ff5085b62840afffc3cefbcef0a3a9509
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
$ docker pull memcached@sha256:e79dd6dea75bf64de1cd87b2204574865bcc12fcda9e1d5c63ce82e3271d4bdf
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.3 MB (5345174 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31403aa3ac88632da679879fcb0a3a627c6f50ec7da0659ae032f63d289d9587`
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
# Fri, 11 Feb 2022 23:43:32 GMT
ENV MEMCACHED_VERSION=1.6.14
# Fri, 11 Feb 2022 23:43:32 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Fri, 11 Feb 2022 23:47:43 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Fri, 11 Feb 2022 23:47:43 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 11 Feb 2022 23:47:44 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 11 Feb 2022 23:47:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Feb 2022 23:47:44 GMT
USER memcache
# Fri, 11 Feb 2022 23:47:45 GMT
EXPOSE 11211
# Fri, 11 Feb 2022 23:47:45 GMT
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
	-	`sha256:4afc0667aa68ec7c0a865809dcfee799f6357b1f6d6c4d6e58240cff71c6264d`  
		Last Modified: Fri, 11 Feb 2022 23:48:39 GMT  
		Size: 2.4 MB (2415863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef8943e1197199b34fc9e9230f24d760a30cdcf11c6b8fc48e89592e00da6edf`  
		Last Modified: Fri, 11 Feb 2022 23:48:38 GMT  
		Size: 283.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b10635796b46c66fb5447019c111ad88d5b808536aab4757aa60b57ffcc9d0da`  
		Last Modified: Fri, 11 Feb 2022 23:48:38 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-alpine3.15` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:c28cbb9d278a2ef6c4ef325c2fffa8bc4631258a341cb411d2a7bec9655007cb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.1 MB (5109831 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e10238b3468650bbfa09ac13b6115339c5305e3e92cb34bb47b6a03b2a93df01`
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
# Fri, 11 Feb 2022 23:59:43 GMT
ENV MEMCACHED_VERSION=1.6.14
# Fri, 11 Feb 2022 23:59:44 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Sat, 12 Feb 2022 00:02:34 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Sat, 12 Feb 2022 00:02:36 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Sat, 12 Feb 2022 00:02:36 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Sat, 12 Feb 2022 00:02:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 12 Feb 2022 00:02:38 GMT
USER memcache
# Sat, 12 Feb 2022 00:02:39 GMT
EXPOSE 11211
# Sat, 12 Feb 2022 00:02:40 GMT
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
	-	`sha256:98b2012c64d2efed092c8ec83344fc68be38873465f9e7b82616b504ca67ea14`  
		Last Modified: Sat, 12 Feb 2022 00:03:57 GMT  
		Size: 2.3 MB (2282236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b54695eeb42571708a7da87031a54d3f82b1be9e474102eeaa912ee51cb86d3`  
		Last Modified: Sat, 12 Feb 2022 00:03:57 GMT  
		Size: 283.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17690cc3c867c822f67c6edabb66fd363b8988e13ed76d6b2a512a4af041bd58`  
		Last Modified: Sat, 12 Feb 2022 00:03:57 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-alpine3.15` - linux; 386

```console
$ docker pull memcached@sha256:5b9731ba5ab72d85a6ed73548a502d6e22d512f328daacddeb531c252745a1e7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.4 MB (5369203 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:83c422eacdcda2fa728cc1fc176ab0cd57a0be7766f0b517dcc64045b255d0a9`
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
# Fri, 11 Feb 2022 23:43:00 GMT
ENV MEMCACHED_VERSION=1.6.14
# Fri, 11 Feb 2022 23:43:01 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Fri, 11 Feb 2022 23:47:20 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Fri, 11 Feb 2022 23:47:20 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 11 Feb 2022 23:47:21 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 11 Feb 2022 23:47:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Feb 2022 23:47:22 GMT
USER memcache
# Fri, 11 Feb 2022 23:47:22 GMT
EXPOSE 11211
# Fri, 11 Feb 2022 23:47:22 GMT
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
	-	`sha256:62d0cbe6f51da8f3bfd9d0bfbbb510f173b231cfc4260066e5da12995d012223`  
		Last Modified: Fri, 11 Feb 2022 23:48:48 GMT  
		Size: 2.4 MB (2419277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfa2ab27dc5f099b91f7195a3d75e51e7f2c84ea56052a565dcbeba235da559b`  
		Last Modified: Fri, 11 Feb 2022 23:48:47 GMT  
		Size: 283.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0394921490062e0dab12bc6f8a3a5bd3f1a97dc261653593a22e3fa95776186`  
		Last Modified: Fri, 11 Feb 2022 23:48:47 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-alpine3.15` - linux; ppc64le

```console
$ docker pull memcached@sha256:75cb5141098fb02bb0c554c31c00d28802b414593a6b41d430c10505ee943fe0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.3 MB (5315837 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4be74852968716dd05ad711f1cda531afac5b782fe0dd6692e5aed7d91d54466`
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
# Fri, 11 Feb 2022 23:54:02 GMT
ENV MEMCACHED_VERSION=1.6.14
# Fri, 11 Feb 2022 23:54:06 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Fri, 11 Feb 2022 23:57:48 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Fri, 11 Feb 2022 23:57:50 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 11 Feb 2022 23:57:55 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 11 Feb 2022 23:57:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Feb 2022 23:57:59 GMT
USER memcache
# Fri, 11 Feb 2022 23:58:01 GMT
EXPOSE 11211
# Fri, 11 Feb 2022 23:58:02 GMT
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
	-	`sha256:e9d933f0d59015113f25123de9b3460a03fdf091181f4c9330b1bb42c27a8cce`  
		Last Modified: Fri, 11 Feb 2022 23:59:16 GMT  
		Size: 2.4 MB (2373175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:659fd1f60c2bc05966f606e677370eeee3176f7d6dbd530b3f271ba313f8b0fe`  
		Last Modified: Fri, 11 Feb 2022 23:59:15 GMT  
		Size: 282.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8d9d86e7310ff252ce602224ce1643c6b8d50713444e43804cdb93912f89087`  
		Last Modified: Fri, 11 Feb 2022 23:59:15 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-alpine3.15` - linux; s390x

```console
$ docker pull memcached@sha256:05d8b33e1a3927fd3ba6b7cd62b648d66a4f07da15103657791736e70515bd20
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4869494 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a751c73ff4357b7992c0a524e080537c462baa079ef3c7b96a3ce7b13699135`
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
# Fri, 11 Feb 2022 23:53:09 GMT
ENV MEMCACHED_VERSION=1.6.14
# Fri, 11 Feb 2022 23:53:09 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Fri, 11 Feb 2022 23:57:25 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Fri, 11 Feb 2022 23:57:25 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 11 Feb 2022 23:57:26 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 11 Feb 2022 23:57:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Feb 2022 23:57:26 GMT
USER memcache
# Fri, 11 Feb 2022 23:57:26 GMT
EXPOSE 11211
# Fri, 11 Feb 2022 23:57:26 GMT
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
	-	`sha256:7bccd1e890d9edaaa99814caec66d49d04d5245aca1fe8a2ac832be7e0e09c06`  
		Last Modified: Fri, 11 Feb 2022 23:58:42 GMT  
		Size: 2.1 MB (2148137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75931a88b924783decffcbf2e1fba6e58f393e9409dd37ffb26b7f6eecffdef2`  
		Last Modified: Fri, 11 Feb 2022 23:58:41 GMT  
		Size: 282.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2dd123370c89ee375732af5193be621336dd45eae2b9729fb66d0376bc915cc`  
		Last Modified: Fri, 11 Feb 2022 23:58:41 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:1.6-bullseye`

```console
$ docker pull memcached@sha256:e4bb2d212309e51166f29fe5404edf5caf784ada9ab3fde8dcf8226f337878aa
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
$ docker pull memcached@sha256:2c29149daad601e046074c6801fb570180d4eba60047135b71f51ea327ffcbc1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.0 MB (32954984 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6208dafa350f4dfbb3f2a16e20c2f2d256f894fd8695ac24b21663a732dee124`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 01 Mar 2022 02:13:29 GMT
ADD file:d48a85028743f16ed927507322e3e3beee187fbfadd0b781d4b89de197c64b5b in / 
# Tue, 01 Mar 2022 02:13:29 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 13:24:57 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 01 Mar 2022 13:25:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 13:25:02 GMT
ENV MEMCACHED_VERSION=1.6.14
# Tue, 01 Mar 2022 13:25:02 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Tue, 01 Mar 2022 13:28:58 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 01 Mar 2022 13:28:58 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 01 Mar 2022 13:28:59 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 01 Mar 2022 13:28:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 01 Mar 2022 13:29:00 GMT
USER memcache
# Tue, 01 Mar 2022 13:29:00 GMT
EXPOSE 11211
# Tue, 01 Mar 2022 13:29:00 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:f7a1c6dad28192bd417b78079d6ddc03cbca6d5ea46bba12769b235b6353c00c`  
		Last Modified: Tue, 01 Mar 2022 02:19:23 GMT  
		Size: 31.4 MB (31366396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3292b9ed039a5211ec564a1f170046ba2ad296a19beb778d3c7106a230301d27`  
		Last Modified: Tue, 01 Mar 2022 13:29:33 GMT  
		Size: 5.0 KB (4980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15c683705067bdb5151c087a9b5e91a37f498912588e29970e3ce07121334f03`  
		Last Modified: Tue, 01 Mar 2022 13:29:34 GMT  
		Size: 328.0 KB (328033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:091c46e57219c5fdd0a044c77fc12a24889bd1ce95e4d032e83f2ea09997ca1d`  
		Last Modified: Tue, 01 Mar 2022 13:29:34 GMT  
		Size: 1.3 MB (1255168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a26e7e13ba905fd75a5e3b2307ab4abee1bbcdc9b586d37fc2ff7984de1c92c3`  
		Last Modified: Tue, 01 Mar 2022 13:29:33 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75b625708cf5e763937f326c6fe55adcb4c4782926483ea2a3628012927922c7`  
		Last Modified: Tue, 01 Mar 2022 13:29:33 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-bullseye` - linux; arm variant v5

```console
$ docker pull memcached@sha256:839b663c2a5637a5a026d8bf63f2c3a5af62938b6becb246fe84e68bceb73742
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.5 MB (30457903 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:46c3d2c41f175e70fa19ec073355fc3376f15b3ca99f6fdb295b6cea57aede38`
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
# Fri, 11 Feb 2022 23:48:33 GMT
ENV MEMCACHED_VERSION=1.6.14
# Fri, 11 Feb 2022 23:48:33 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Fri, 11 Feb 2022 23:53:18 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Fri, 11 Feb 2022 23:53:19 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 11 Feb 2022 23:53:20 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 11 Feb 2022 23:53:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Feb 2022 23:53:21 GMT
USER memcache
# Fri, 11 Feb 2022 23:53:22 GMT
EXPOSE 11211
# Fri, 11 Feb 2022 23:53:22 GMT
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
	-	`sha256:4c595fdbb4287a9ef2b3565e1d9ac2caa7d17ac0810224d8a5d3c87313cc81b5`  
		Last Modified: Fri, 11 Feb 2022 23:54:16 GMT  
		Size: 1.2 MB (1226376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19c8ecb542750e6e603057b1e7bdb90fc58d45b604f20b2724d402a572f1b735`  
		Last Modified: Fri, 11 Feb 2022 23:54:15 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64d2e913eaab741b412c8fec5edbad97daed3a2c5f0a1a1fd376ea8ec7c28c52`  
		Last Modified: Fri, 11 Feb 2022 23:54:15 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-bullseye` - linux; arm variant v7

```console
$ docker pull memcached@sha256:c1ded327e0d4c11f7f00652600f4cbf465a119fed31e6e2541d516700e0e14c2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.1 MB (28080208 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:866cf84302a62bedfada61f236deccacb7585dc0ccce8a4e0e058b741bfafdc5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 01 Mar 2022 02:02:56 GMT
ADD file:c6b519323fd1fa09b9f8c8608778872e8fa6208cb0b42aaccdef4479a469f5f4 in / 
# Tue, 01 Mar 2022 02:02:57 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 14:02:17 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 01 Mar 2022 14:02:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 14:02:26 GMT
ENV MEMCACHED_VERSION=1.6.14
# Tue, 01 Mar 2022 14:02:26 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Tue, 01 Mar 2022 14:06:15 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 01 Mar 2022 14:06:16 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 01 Mar 2022 14:06:17 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 01 Mar 2022 14:06:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 01 Mar 2022 14:06:18 GMT
USER memcache
# Tue, 01 Mar 2022 14:06:19 GMT
EXPOSE 11211
# Tue, 01 Mar 2022 14:06:19 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:59dbb2ac3829352dd707e28e037734c9fbdef5b03aea31e3929ddcead949afee`  
		Last Modified: Tue, 01 Mar 2022 02:19:09 GMT  
		Size: 26.6 MB (26565105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45ff8679190bbfe567a01e354c79eb44efaa4564b0770a644b9eb6a28f10812c`  
		Last Modified: Tue, 01 Mar 2022 14:19:16 GMT  
		Size: 4.9 KB (4894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13db11031aa185885b3b1b9c74eba0d8ea9b07d5e8fec5870bc7df8d09585d2f`  
		Last Modified: Tue, 01 Mar 2022 14:19:16 GMT  
		Size: 312.0 KB (312009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:079efee4f8d1e8cea53f0cc6ddc4832de31e69c43411b81e790e0615eeea16aa`  
		Last Modified: Tue, 01 Mar 2022 14:19:16 GMT  
		Size: 1.2 MB (1197793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:050fbe09656330899bb983ba6d0871a6cc96349c4c049673a4ee53816db5ff7b`  
		Last Modified: Tue, 01 Mar 2022 14:19:16 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcca636453f4acf7b597c080e2d7c57ea366f36daae56acdd43664bb28dff985`  
		Last Modified: Tue, 01 Mar 2022 14:19:16 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-bullseye` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:c59ae38d83ce474dc14423325e3f500a06e285938b4f4e8a013ae8967603d492
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.4 MB (31435417 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b5c5ad61ebd09fab08b612599fdf9e96be59696045e4765dac554781daef4d1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 01 Mar 2022 02:11:29 GMT
ADD file:9816c9c29627693c34afda4fa5e1a5e8a0f5aa3c5d5cfd920a4d89c77aab997d in / 
# Tue, 01 Mar 2022 02:11:30 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 12:44:12 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 01 Mar 2022 12:44:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 12:44:16 GMT
ENV MEMCACHED_VERSION=1.6.14
# Tue, 01 Mar 2022 12:44:17 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Tue, 01 Mar 2022 12:46:49 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 01 Mar 2022 12:46:50 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 01 Mar 2022 12:46:50 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 01 Mar 2022 12:46:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 01 Mar 2022 12:46:52 GMT
USER memcache
# Tue, 01 Mar 2022 12:46:53 GMT
EXPOSE 11211
# Tue, 01 Mar 2022 12:46:54 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:279a020076a7fbddfc996e4c55e605a8f322810c3eca21cdedbcb06beb0e1305`  
		Last Modified: Tue, 01 Mar 2022 02:18:24 GMT  
		Size: 30.1 MB (30057008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7dfd1ea3d9e177e785365db9a22591801c15e6a33097ba79a048e3387f4c43a`  
		Last Modified: Tue, 01 Mar 2022 12:47:45 GMT  
		Size: 4.9 KB (4902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e563a531f0653c96d3786deff2afe7190769b5929d06c8c234d89fd314bf2396`  
		Last Modified: Tue, 01 Mar 2022 12:47:45 GMT  
		Size: 119.2 KB (119172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1d1b1b990f1e4e95a5410acd589565956a1fd54c4df3b71a665dcfb23ac9f76`  
		Last Modified: Tue, 01 Mar 2022 12:47:46 GMT  
		Size: 1.3 MB (1253928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b8a7c0be94d102b9a04c359186fcf59b223183acc8b489d0ca12afb8f073027`  
		Last Modified: Tue, 01 Mar 2022 12:47:45 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:091c7ee2fb4e34177c30b2b9905bf098f304bea040ff7ca5700134d4921c2758`  
		Last Modified: Tue, 01 Mar 2022 12:47:45 GMT  
		Size: 120.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-bullseye` - linux; 386

```console
$ docker pull memcached@sha256:4c9eb4902e2601bad18a1783dbf7d64cf25f6121226d4772a5d36a7ac3e9db79
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.0 MB (33972554 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af09c75e25cf0ea60c4f155a25728e256411f07898946ea08e869eb6362e3a24`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 01 Mar 2022 02:07:32 GMT
ADD file:e92ab504d4c0d3bd63da83254e6ca400b607c32e0f5037039648559b91770870 in / 
# Tue, 01 Mar 2022 02:07:33 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 10:07:23 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 01 Mar 2022 10:07:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 10:07:30 GMT
ENV MEMCACHED_VERSION=1.6.14
# Tue, 01 Mar 2022 10:07:30 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Tue, 01 Mar 2022 10:11:57 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 01 Mar 2022 10:11:57 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 01 Mar 2022 10:11:58 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 01 Mar 2022 10:11:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 01 Mar 2022 10:11:58 GMT
USER memcache
# Tue, 01 Mar 2022 10:11:58 GMT
EXPOSE 11211
# Tue, 01 Mar 2022 10:11:59 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:04a87e821be7e4b29d48011b7aa4ff884ca57fd36995cb3b99fd2fc24ac562d8`  
		Last Modified: Tue, 01 Mar 2022 02:15:51 GMT  
		Size: 32.4 MB (32377389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe860ecc70fbef589f9779541d957321138c3f41d99742ca7ff2bb41b6787786`  
		Last Modified: Tue, 01 Mar 2022 10:13:02 GMT  
		Size: 4.9 KB (4889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71fbbf846282a29c58595e09b8a5d93a6348fc5a77d0bb513263f933972610e8`  
		Last Modified: Tue, 01 Mar 2022 10:13:03 GMT  
		Size: 336.6 KB (336603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f93f31af2adb455df5e2c7baaa190b479d463d37657734ee855d663709906a2`  
		Last Modified: Tue, 01 Mar 2022 10:13:03 GMT  
		Size: 1.3 MB (1253268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ea06973bd5c70feb976fde3006e5400760f293973d5a2a8f8a05a73105a5851`  
		Last Modified: Tue, 01 Mar 2022 10:13:02 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c85296c039a2ca9f99139e04d26550a26b109424a80e9377a115129110257b9`  
		Last Modified: Tue, 01 Mar 2022 10:13:02 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-bullseye` - linux; mips64le

```console
$ docker pull memcached@sha256:76269e61918b56719946fa47ffaebf468965e45dae401738fcd6d8ea6d9afdc1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.2 MB (31213138 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bdf2a1611553c4acfb426a9736777620af35250c1c3fde4997dd8fda25547725`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 01 Mar 2022 02:02:49 GMT
ADD file:1901e1e1292cbfcd557262ec5d08551cecd0070b24928414d220472664fe3fdf in / 
# Tue, 01 Mar 2022 02:02:49 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 03:43:18 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 01 Mar 2022 03:43:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 03:43:30 GMT
ENV MEMCACHED_VERSION=1.6.14
# Tue, 01 Mar 2022 03:43:30 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Tue, 01 Mar 2022 03:49:17 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 01 Mar 2022 03:49:17 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 01 Mar 2022 03:49:19 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 01 Mar 2022 03:49:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 01 Mar 2022 03:49:20 GMT
USER memcache
# Tue, 01 Mar 2022 03:49:20 GMT
EXPOSE 11211
# Tue, 01 Mar 2022 03:49:20 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:3baeb8c34a522fc616f97412d47dc1f665e93552c57aa8237ee1d673f9757cba`  
		Last Modified: Tue, 01 Mar 2022 02:12:25 GMT  
		Size: 29.6 MB (29632966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50a63f21594c0da6641452e9cd0caaf8727bae4ca86c617384198ab5d8e766ec`  
		Last Modified: Tue, 01 Mar 2022 03:49:43 GMT  
		Size: 5.0 KB (4979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dfb3a0cb8d59939fa0e67d13c57840042b1397d36d3c1918e50344eb405025d`  
		Last Modified: Tue, 01 Mar 2022 03:49:43 GMT  
		Size: 323.7 KB (323703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e632b2b5bf88ea94d56d701fa93b55516003db1fc7c855bb4569f2be0ddf3be`  
		Last Modified: Tue, 01 Mar 2022 03:49:43 GMT  
		Size: 1.3 MB (1251083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1fc0f9b2a7499de336af3103d86d1ffc3b90b62ea850295c0c57abbe68c753b`  
		Last Modified: Tue, 01 Mar 2022 03:49:43 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe1ee7b4dd056bb3eadc09b9893ce88a096e51500bbe841d1c145be10ba2b1f0`  
		Last Modified: Tue, 01 Mar 2022 03:49:43 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-bullseye` - linux; ppc64le

```console
$ docker pull memcached@sha256:4893f4daa742b31f414b08f98f8e7d0cbedaf63b8d88062bcf3c91a9522a2aab
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.0 MB (36957544 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8db953cc998ed06712eca57fe4ae2b8bb342ce991683fd7592495a21557d0940`
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
# Fri, 11 Feb 2022 23:47:36 GMT
ENV MEMCACHED_VERSION=1.6.14
# Fri, 11 Feb 2022 23:47:38 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Fri, 11 Feb 2022 23:53:07 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Fri, 11 Feb 2022 23:53:13 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 11 Feb 2022 23:53:34 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 11 Feb 2022 23:53:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Feb 2022 23:53:39 GMT
USER memcache
# Fri, 11 Feb 2022 23:53:41 GMT
EXPOSE 11211
# Fri, 11 Feb 2022 23:53:46 GMT
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
	-	`sha256:d5f2e5d5bb1609e336a37e97218d618550ec5ce28384c32b1141393ef6f04a03`  
		Last Modified: Fri, 11 Feb 2022 23:58:44 GMT  
		Size: 1.3 MB (1322220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76e6da4f290b1cff2fa5b1ad17d42333c67179332511db4da3bd2c5ce12bbdfa`  
		Last Modified: Fri, 11 Feb 2022 23:58:44 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fb140c5468aa121999bc169d30e4ce6b73795cdf67aa21c1dfd3d1194dd0b82`  
		Last Modified: Fri, 11 Feb 2022 23:58:44 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-bullseye` - linux; s390x

```console
$ docker pull memcached@sha256:14b3ae46a3b5dc4d1ca410da43e53ee0c44ad49ec398f235628f89bc8cc0a0cc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.2 MB (31217166 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:50f1b3aef9bc393e3b1a3fab35c702d6a9b9dd6fa2abd9d044b52385b9ccf549`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 01 Mar 2022 02:01:56 GMT
ADD file:d869ad3392a4e752c2f73d08a4cc13594c94bfc050bd037db0ca9827a0207072 in / 
# Tue, 01 Mar 2022 02:01:58 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 13:28:37 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 01 Mar 2022 13:28:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 13:28:40 GMT
ENV MEMCACHED_VERSION=1.6.14
# Tue, 01 Mar 2022 13:28:40 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Tue, 01 Mar 2022 13:31:58 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 01 Mar 2022 13:31:58 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 01 Mar 2022 13:31:58 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 01 Mar 2022 13:31:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 01 Mar 2022 13:31:59 GMT
USER memcache
# Tue, 01 Mar 2022 13:31:59 GMT
EXPOSE 11211
# Tue, 01 Mar 2022 13:31:59 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:f81abce72636770dac4258df46a31beeb6ad81dfddd5b7c9c3fa6942ea074922`  
		Last Modified: Tue, 01 Mar 2022 02:07:33 GMT  
		Size: 29.6 MB (29647132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b43f274641c42412c1e075acb3920020215603d1e1c938fa84211ea8b005988`  
		Last Modified: Tue, 01 Mar 2022 13:32:52 GMT  
		Size: 5.0 KB (5024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d135f121f1aff6ea16284d2286318c703c72dad45560bdc68ac2bc2371f8164`  
		Last Modified: Tue, 01 Mar 2022 13:32:52 GMT  
		Size: 324.1 KB (324102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9255401f181741c77541d42f93796b72c20077b2815b9e6c4e21b36f9bcccab6`  
		Last Modified: Tue, 01 Mar 2022 13:32:52 GMT  
		Size: 1.2 MB (1240500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5436de37a983faa64cc9d82c3a8272ae77b107e2f8bcd453f7aee5e3e92def7`  
		Last Modified: Tue, 01 Mar 2022 13:32:52 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8296feb21176186e1c4027cf5e8111ed103c7b2b30f1f4423a9303a0e7fd9d3`  
		Last Modified: Tue, 01 Mar 2022 13:32:52 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:1.6.14`

```console
$ docker pull memcached@sha256:e4bb2d212309e51166f29fe5404edf5caf784ada9ab3fde8dcf8226f337878aa
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

### `memcached:1.6.14` - linux; amd64

```console
$ docker pull memcached@sha256:2c29149daad601e046074c6801fb570180d4eba60047135b71f51ea327ffcbc1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.0 MB (32954984 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6208dafa350f4dfbb3f2a16e20c2f2d256f894fd8695ac24b21663a732dee124`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 01 Mar 2022 02:13:29 GMT
ADD file:d48a85028743f16ed927507322e3e3beee187fbfadd0b781d4b89de197c64b5b in / 
# Tue, 01 Mar 2022 02:13:29 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 13:24:57 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 01 Mar 2022 13:25:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 13:25:02 GMT
ENV MEMCACHED_VERSION=1.6.14
# Tue, 01 Mar 2022 13:25:02 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Tue, 01 Mar 2022 13:28:58 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 01 Mar 2022 13:28:58 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 01 Mar 2022 13:28:59 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 01 Mar 2022 13:28:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 01 Mar 2022 13:29:00 GMT
USER memcache
# Tue, 01 Mar 2022 13:29:00 GMT
EXPOSE 11211
# Tue, 01 Mar 2022 13:29:00 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:f7a1c6dad28192bd417b78079d6ddc03cbca6d5ea46bba12769b235b6353c00c`  
		Last Modified: Tue, 01 Mar 2022 02:19:23 GMT  
		Size: 31.4 MB (31366396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3292b9ed039a5211ec564a1f170046ba2ad296a19beb778d3c7106a230301d27`  
		Last Modified: Tue, 01 Mar 2022 13:29:33 GMT  
		Size: 5.0 KB (4980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15c683705067bdb5151c087a9b5e91a37f498912588e29970e3ce07121334f03`  
		Last Modified: Tue, 01 Mar 2022 13:29:34 GMT  
		Size: 328.0 KB (328033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:091c46e57219c5fdd0a044c77fc12a24889bd1ce95e4d032e83f2ea09997ca1d`  
		Last Modified: Tue, 01 Mar 2022 13:29:34 GMT  
		Size: 1.3 MB (1255168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a26e7e13ba905fd75a5e3b2307ab4abee1bbcdc9b586d37fc2ff7984de1c92c3`  
		Last Modified: Tue, 01 Mar 2022 13:29:33 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75b625708cf5e763937f326c6fe55adcb4c4782926483ea2a3628012927922c7`  
		Last Modified: Tue, 01 Mar 2022 13:29:33 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.14` - linux; arm variant v5

```console
$ docker pull memcached@sha256:839b663c2a5637a5a026d8bf63f2c3a5af62938b6becb246fe84e68bceb73742
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.5 MB (30457903 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:46c3d2c41f175e70fa19ec073355fc3376f15b3ca99f6fdb295b6cea57aede38`
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
# Fri, 11 Feb 2022 23:48:33 GMT
ENV MEMCACHED_VERSION=1.6.14
# Fri, 11 Feb 2022 23:48:33 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Fri, 11 Feb 2022 23:53:18 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Fri, 11 Feb 2022 23:53:19 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 11 Feb 2022 23:53:20 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 11 Feb 2022 23:53:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Feb 2022 23:53:21 GMT
USER memcache
# Fri, 11 Feb 2022 23:53:22 GMT
EXPOSE 11211
# Fri, 11 Feb 2022 23:53:22 GMT
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
	-	`sha256:4c595fdbb4287a9ef2b3565e1d9ac2caa7d17ac0810224d8a5d3c87313cc81b5`  
		Last Modified: Fri, 11 Feb 2022 23:54:16 GMT  
		Size: 1.2 MB (1226376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19c8ecb542750e6e603057b1e7bdb90fc58d45b604f20b2724d402a572f1b735`  
		Last Modified: Fri, 11 Feb 2022 23:54:15 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64d2e913eaab741b412c8fec5edbad97daed3a2c5f0a1a1fd376ea8ec7c28c52`  
		Last Modified: Fri, 11 Feb 2022 23:54:15 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.14` - linux; arm variant v7

```console
$ docker pull memcached@sha256:c1ded327e0d4c11f7f00652600f4cbf465a119fed31e6e2541d516700e0e14c2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.1 MB (28080208 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:866cf84302a62bedfada61f236deccacb7585dc0ccce8a4e0e058b741bfafdc5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 01 Mar 2022 02:02:56 GMT
ADD file:c6b519323fd1fa09b9f8c8608778872e8fa6208cb0b42aaccdef4479a469f5f4 in / 
# Tue, 01 Mar 2022 02:02:57 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 14:02:17 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 01 Mar 2022 14:02:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 14:02:26 GMT
ENV MEMCACHED_VERSION=1.6.14
# Tue, 01 Mar 2022 14:02:26 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Tue, 01 Mar 2022 14:06:15 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 01 Mar 2022 14:06:16 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 01 Mar 2022 14:06:17 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 01 Mar 2022 14:06:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 01 Mar 2022 14:06:18 GMT
USER memcache
# Tue, 01 Mar 2022 14:06:19 GMT
EXPOSE 11211
# Tue, 01 Mar 2022 14:06:19 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:59dbb2ac3829352dd707e28e037734c9fbdef5b03aea31e3929ddcead949afee`  
		Last Modified: Tue, 01 Mar 2022 02:19:09 GMT  
		Size: 26.6 MB (26565105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45ff8679190bbfe567a01e354c79eb44efaa4564b0770a644b9eb6a28f10812c`  
		Last Modified: Tue, 01 Mar 2022 14:19:16 GMT  
		Size: 4.9 KB (4894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13db11031aa185885b3b1b9c74eba0d8ea9b07d5e8fec5870bc7df8d09585d2f`  
		Last Modified: Tue, 01 Mar 2022 14:19:16 GMT  
		Size: 312.0 KB (312009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:079efee4f8d1e8cea53f0cc6ddc4832de31e69c43411b81e790e0615eeea16aa`  
		Last Modified: Tue, 01 Mar 2022 14:19:16 GMT  
		Size: 1.2 MB (1197793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:050fbe09656330899bb983ba6d0871a6cc96349c4c049673a4ee53816db5ff7b`  
		Last Modified: Tue, 01 Mar 2022 14:19:16 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcca636453f4acf7b597c080e2d7c57ea366f36daae56acdd43664bb28dff985`  
		Last Modified: Tue, 01 Mar 2022 14:19:16 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.14` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:c59ae38d83ce474dc14423325e3f500a06e285938b4f4e8a013ae8967603d492
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.4 MB (31435417 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b5c5ad61ebd09fab08b612599fdf9e96be59696045e4765dac554781daef4d1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 01 Mar 2022 02:11:29 GMT
ADD file:9816c9c29627693c34afda4fa5e1a5e8a0f5aa3c5d5cfd920a4d89c77aab997d in / 
# Tue, 01 Mar 2022 02:11:30 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 12:44:12 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 01 Mar 2022 12:44:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 12:44:16 GMT
ENV MEMCACHED_VERSION=1.6.14
# Tue, 01 Mar 2022 12:44:17 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Tue, 01 Mar 2022 12:46:49 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 01 Mar 2022 12:46:50 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 01 Mar 2022 12:46:50 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 01 Mar 2022 12:46:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 01 Mar 2022 12:46:52 GMT
USER memcache
# Tue, 01 Mar 2022 12:46:53 GMT
EXPOSE 11211
# Tue, 01 Mar 2022 12:46:54 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:279a020076a7fbddfc996e4c55e605a8f322810c3eca21cdedbcb06beb0e1305`  
		Last Modified: Tue, 01 Mar 2022 02:18:24 GMT  
		Size: 30.1 MB (30057008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7dfd1ea3d9e177e785365db9a22591801c15e6a33097ba79a048e3387f4c43a`  
		Last Modified: Tue, 01 Mar 2022 12:47:45 GMT  
		Size: 4.9 KB (4902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e563a531f0653c96d3786deff2afe7190769b5929d06c8c234d89fd314bf2396`  
		Last Modified: Tue, 01 Mar 2022 12:47:45 GMT  
		Size: 119.2 KB (119172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1d1b1b990f1e4e95a5410acd589565956a1fd54c4df3b71a665dcfb23ac9f76`  
		Last Modified: Tue, 01 Mar 2022 12:47:46 GMT  
		Size: 1.3 MB (1253928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b8a7c0be94d102b9a04c359186fcf59b223183acc8b489d0ca12afb8f073027`  
		Last Modified: Tue, 01 Mar 2022 12:47:45 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:091c7ee2fb4e34177c30b2b9905bf098f304bea040ff7ca5700134d4921c2758`  
		Last Modified: Tue, 01 Mar 2022 12:47:45 GMT  
		Size: 120.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.14` - linux; 386

```console
$ docker pull memcached@sha256:4c9eb4902e2601bad18a1783dbf7d64cf25f6121226d4772a5d36a7ac3e9db79
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.0 MB (33972554 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af09c75e25cf0ea60c4f155a25728e256411f07898946ea08e869eb6362e3a24`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 01 Mar 2022 02:07:32 GMT
ADD file:e92ab504d4c0d3bd63da83254e6ca400b607c32e0f5037039648559b91770870 in / 
# Tue, 01 Mar 2022 02:07:33 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 10:07:23 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 01 Mar 2022 10:07:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 10:07:30 GMT
ENV MEMCACHED_VERSION=1.6.14
# Tue, 01 Mar 2022 10:07:30 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Tue, 01 Mar 2022 10:11:57 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 01 Mar 2022 10:11:57 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 01 Mar 2022 10:11:58 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 01 Mar 2022 10:11:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 01 Mar 2022 10:11:58 GMT
USER memcache
# Tue, 01 Mar 2022 10:11:58 GMT
EXPOSE 11211
# Tue, 01 Mar 2022 10:11:59 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:04a87e821be7e4b29d48011b7aa4ff884ca57fd36995cb3b99fd2fc24ac562d8`  
		Last Modified: Tue, 01 Mar 2022 02:15:51 GMT  
		Size: 32.4 MB (32377389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe860ecc70fbef589f9779541d957321138c3f41d99742ca7ff2bb41b6787786`  
		Last Modified: Tue, 01 Mar 2022 10:13:02 GMT  
		Size: 4.9 KB (4889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71fbbf846282a29c58595e09b8a5d93a6348fc5a77d0bb513263f933972610e8`  
		Last Modified: Tue, 01 Mar 2022 10:13:03 GMT  
		Size: 336.6 KB (336603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f93f31af2adb455df5e2c7baaa190b479d463d37657734ee855d663709906a2`  
		Last Modified: Tue, 01 Mar 2022 10:13:03 GMT  
		Size: 1.3 MB (1253268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ea06973bd5c70feb976fde3006e5400760f293973d5a2a8f8a05a73105a5851`  
		Last Modified: Tue, 01 Mar 2022 10:13:02 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c85296c039a2ca9f99139e04d26550a26b109424a80e9377a115129110257b9`  
		Last Modified: Tue, 01 Mar 2022 10:13:02 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.14` - linux; mips64le

```console
$ docker pull memcached@sha256:76269e61918b56719946fa47ffaebf468965e45dae401738fcd6d8ea6d9afdc1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.2 MB (31213138 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bdf2a1611553c4acfb426a9736777620af35250c1c3fde4997dd8fda25547725`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 01 Mar 2022 02:02:49 GMT
ADD file:1901e1e1292cbfcd557262ec5d08551cecd0070b24928414d220472664fe3fdf in / 
# Tue, 01 Mar 2022 02:02:49 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 03:43:18 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 01 Mar 2022 03:43:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 03:43:30 GMT
ENV MEMCACHED_VERSION=1.6.14
# Tue, 01 Mar 2022 03:43:30 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Tue, 01 Mar 2022 03:49:17 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 01 Mar 2022 03:49:17 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 01 Mar 2022 03:49:19 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 01 Mar 2022 03:49:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 01 Mar 2022 03:49:20 GMT
USER memcache
# Tue, 01 Mar 2022 03:49:20 GMT
EXPOSE 11211
# Tue, 01 Mar 2022 03:49:20 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:3baeb8c34a522fc616f97412d47dc1f665e93552c57aa8237ee1d673f9757cba`  
		Last Modified: Tue, 01 Mar 2022 02:12:25 GMT  
		Size: 29.6 MB (29632966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50a63f21594c0da6641452e9cd0caaf8727bae4ca86c617384198ab5d8e766ec`  
		Last Modified: Tue, 01 Mar 2022 03:49:43 GMT  
		Size: 5.0 KB (4979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dfb3a0cb8d59939fa0e67d13c57840042b1397d36d3c1918e50344eb405025d`  
		Last Modified: Tue, 01 Mar 2022 03:49:43 GMT  
		Size: 323.7 KB (323703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e632b2b5bf88ea94d56d701fa93b55516003db1fc7c855bb4569f2be0ddf3be`  
		Last Modified: Tue, 01 Mar 2022 03:49:43 GMT  
		Size: 1.3 MB (1251083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1fc0f9b2a7499de336af3103d86d1ffc3b90b62ea850295c0c57abbe68c753b`  
		Last Modified: Tue, 01 Mar 2022 03:49:43 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe1ee7b4dd056bb3eadc09b9893ce88a096e51500bbe841d1c145be10ba2b1f0`  
		Last Modified: Tue, 01 Mar 2022 03:49:43 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.14` - linux; ppc64le

```console
$ docker pull memcached@sha256:4893f4daa742b31f414b08f98f8e7d0cbedaf63b8d88062bcf3c91a9522a2aab
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.0 MB (36957544 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8db953cc998ed06712eca57fe4ae2b8bb342ce991683fd7592495a21557d0940`
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
# Fri, 11 Feb 2022 23:47:36 GMT
ENV MEMCACHED_VERSION=1.6.14
# Fri, 11 Feb 2022 23:47:38 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Fri, 11 Feb 2022 23:53:07 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Fri, 11 Feb 2022 23:53:13 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 11 Feb 2022 23:53:34 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 11 Feb 2022 23:53:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Feb 2022 23:53:39 GMT
USER memcache
# Fri, 11 Feb 2022 23:53:41 GMT
EXPOSE 11211
# Fri, 11 Feb 2022 23:53:46 GMT
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
	-	`sha256:d5f2e5d5bb1609e336a37e97218d618550ec5ce28384c32b1141393ef6f04a03`  
		Last Modified: Fri, 11 Feb 2022 23:58:44 GMT  
		Size: 1.3 MB (1322220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76e6da4f290b1cff2fa5b1ad17d42333c67179332511db4da3bd2c5ce12bbdfa`  
		Last Modified: Fri, 11 Feb 2022 23:58:44 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fb140c5468aa121999bc169d30e4ce6b73795cdf67aa21c1dfd3d1194dd0b82`  
		Last Modified: Fri, 11 Feb 2022 23:58:44 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.14` - linux; s390x

```console
$ docker pull memcached@sha256:14b3ae46a3b5dc4d1ca410da43e53ee0c44ad49ec398f235628f89bc8cc0a0cc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.2 MB (31217166 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:50f1b3aef9bc393e3b1a3fab35c702d6a9b9dd6fa2abd9d044b52385b9ccf549`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 01 Mar 2022 02:01:56 GMT
ADD file:d869ad3392a4e752c2f73d08a4cc13594c94bfc050bd037db0ca9827a0207072 in / 
# Tue, 01 Mar 2022 02:01:58 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 13:28:37 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 01 Mar 2022 13:28:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 13:28:40 GMT
ENV MEMCACHED_VERSION=1.6.14
# Tue, 01 Mar 2022 13:28:40 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Tue, 01 Mar 2022 13:31:58 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 01 Mar 2022 13:31:58 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 01 Mar 2022 13:31:58 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 01 Mar 2022 13:31:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 01 Mar 2022 13:31:59 GMT
USER memcache
# Tue, 01 Mar 2022 13:31:59 GMT
EXPOSE 11211
# Tue, 01 Mar 2022 13:31:59 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:f81abce72636770dac4258df46a31beeb6ad81dfddd5b7c9c3fa6942ea074922`  
		Last Modified: Tue, 01 Mar 2022 02:07:33 GMT  
		Size: 29.6 MB (29647132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b43f274641c42412c1e075acb3920020215603d1e1c938fa84211ea8b005988`  
		Last Modified: Tue, 01 Mar 2022 13:32:52 GMT  
		Size: 5.0 KB (5024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d135f121f1aff6ea16284d2286318c703c72dad45560bdc68ac2bc2371f8164`  
		Last Modified: Tue, 01 Mar 2022 13:32:52 GMT  
		Size: 324.1 KB (324102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9255401f181741c77541d42f93796b72c20077b2815b9e6c4e21b36f9bcccab6`  
		Last Modified: Tue, 01 Mar 2022 13:32:52 GMT  
		Size: 1.2 MB (1240500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5436de37a983faa64cc9d82c3a8272ae77b107e2f8bcd453f7aee5e3e92def7`  
		Last Modified: Tue, 01 Mar 2022 13:32:52 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8296feb21176186e1c4027cf5e8111ed103c7b2b30f1f4423a9303a0e7fd9d3`  
		Last Modified: Tue, 01 Mar 2022 13:32:52 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:1.6.14-alpine`

```console
$ docker pull memcached@sha256:76e5acd480d7bd36706f7873f5f7278ff5085b62840afffc3cefbcef0a3a9509
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `memcached:1.6.14-alpine` - linux; amd64

```console
$ docker pull memcached@sha256:e79dd6dea75bf64de1cd87b2204574865bcc12fcda9e1d5c63ce82e3271d4bdf
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.3 MB (5345174 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31403aa3ac88632da679879fcb0a3a627c6f50ec7da0659ae032f63d289d9587`
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
# Fri, 11 Feb 2022 23:43:32 GMT
ENV MEMCACHED_VERSION=1.6.14
# Fri, 11 Feb 2022 23:43:32 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Fri, 11 Feb 2022 23:47:43 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Fri, 11 Feb 2022 23:47:43 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 11 Feb 2022 23:47:44 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 11 Feb 2022 23:47:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Feb 2022 23:47:44 GMT
USER memcache
# Fri, 11 Feb 2022 23:47:45 GMT
EXPOSE 11211
# Fri, 11 Feb 2022 23:47:45 GMT
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
	-	`sha256:4afc0667aa68ec7c0a865809dcfee799f6357b1f6d6c4d6e58240cff71c6264d`  
		Last Modified: Fri, 11 Feb 2022 23:48:39 GMT  
		Size: 2.4 MB (2415863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef8943e1197199b34fc9e9230f24d760a30cdcf11c6b8fc48e89592e00da6edf`  
		Last Modified: Fri, 11 Feb 2022 23:48:38 GMT  
		Size: 283.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b10635796b46c66fb5447019c111ad88d5b808536aab4757aa60b57ffcc9d0da`  
		Last Modified: Fri, 11 Feb 2022 23:48:38 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.14-alpine` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:c28cbb9d278a2ef6c4ef325c2fffa8bc4631258a341cb411d2a7bec9655007cb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.1 MB (5109831 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e10238b3468650bbfa09ac13b6115339c5305e3e92cb34bb47b6a03b2a93df01`
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
# Fri, 11 Feb 2022 23:59:43 GMT
ENV MEMCACHED_VERSION=1.6.14
# Fri, 11 Feb 2022 23:59:44 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Sat, 12 Feb 2022 00:02:34 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Sat, 12 Feb 2022 00:02:36 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Sat, 12 Feb 2022 00:02:36 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Sat, 12 Feb 2022 00:02:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 12 Feb 2022 00:02:38 GMT
USER memcache
# Sat, 12 Feb 2022 00:02:39 GMT
EXPOSE 11211
# Sat, 12 Feb 2022 00:02:40 GMT
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
	-	`sha256:98b2012c64d2efed092c8ec83344fc68be38873465f9e7b82616b504ca67ea14`  
		Last Modified: Sat, 12 Feb 2022 00:03:57 GMT  
		Size: 2.3 MB (2282236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b54695eeb42571708a7da87031a54d3f82b1be9e474102eeaa912ee51cb86d3`  
		Last Modified: Sat, 12 Feb 2022 00:03:57 GMT  
		Size: 283.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17690cc3c867c822f67c6edabb66fd363b8988e13ed76d6b2a512a4af041bd58`  
		Last Modified: Sat, 12 Feb 2022 00:03:57 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.14-alpine` - linux; 386

```console
$ docker pull memcached@sha256:5b9731ba5ab72d85a6ed73548a502d6e22d512f328daacddeb531c252745a1e7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.4 MB (5369203 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:83c422eacdcda2fa728cc1fc176ab0cd57a0be7766f0b517dcc64045b255d0a9`
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
# Fri, 11 Feb 2022 23:43:00 GMT
ENV MEMCACHED_VERSION=1.6.14
# Fri, 11 Feb 2022 23:43:01 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Fri, 11 Feb 2022 23:47:20 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Fri, 11 Feb 2022 23:47:20 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 11 Feb 2022 23:47:21 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 11 Feb 2022 23:47:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Feb 2022 23:47:22 GMT
USER memcache
# Fri, 11 Feb 2022 23:47:22 GMT
EXPOSE 11211
# Fri, 11 Feb 2022 23:47:22 GMT
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
	-	`sha256:62d0cbe6f51da8f3bfd9d0bfbbb510f173b231cfc4260066e5da12995d012223`  
		Last Modified: Fri, 11 Feb 2022 23:48:48 GMT  
		Size: 2.4 MB (2419277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfa2ab27dc5f099b91f7195a3d75e51e7f2c84ea56052a565dcbeba235da559b`  
		Last Modified: Fri, 11 Feb 2022 23:48:47 GMT  
		Size: 283.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0394921490062e0dab12bc6f8a3a5bd3f1a97dc261653593a22e3fa95776186`  
		Last Modified: Fri, 11 Feb 2022 23:48:47 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.14-alpine` - linux; ppc64le

```console
$ docker pull memcached@sha256:75cb5141098fb02bb0c554c31c00d28802b414593a6b41d430c10505ee943fe0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.3 MB (5315837 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4be74852968716dd05ad711f1cda531afac5b782fe0dd6692e5aed7d91d54466`
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
# Fri, 11 Feb 2022 23:54:02 GMT
ENV MEMCACHED_VERSION=1.6.14
# Fri, 11 Feb 2022 23:54:06 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Fri, 11 Feb 2022 23:57:48 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Fri, 11 Feb 2022 23:57:50 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 11 Feb 2022 23:57:55 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 11 Feb 2022 23:57:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Feb 2022 23:57:59 GMT
USER memcache
# Fri, 11 Feb 2022 23:58:01 GMT
EXPOSE 11211
# Fri, 11 Feb 2022 23:58:02 GMT
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
	-	`sha256:e9d933f0d59015113f25123de9b3460a03fdf091181f4c9330b1bb42c27a8cce`  
		Last Modified: Fri, 11 Feb 2022 23:59:16 GMT  
		Size: 2.4 MB (2373175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:659fd1f60c2bc05966f606e677370eeee3176f7d6dbd530b3f271ba313f8b0fe`  
		Last Modified: Fri, 11 Feb 2022 23:59:15 GMT  
		Size: 282.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8d9d86e7310ff252ce602224ce1643c6b8d50713444e43804cdb93912f89087`  
		Last Modified: Fri, 11 Feb 2022 23:59:15 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.14-alpine` - linux; s390x

```console
$ docker pull memcached@sha256:05d8b33e1a3927fd3ba6b7cd62b648d66a4f07da15103657791736e70515bd20
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4869494 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a751c73ff4357b7992c0a524e080537c462baa079ef3c7b96a3ce7b13699135`
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
# Fri, 11 Feb 2022 23:53:09 GMT
ENV MEMCACHED_VERSION=1.6.14
# Fri, 11 Feb 2022 23:53:09 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Fri, 11 Feb 2022 23:57:25 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Fri, 11 Feb 2022 23:57:25 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 11 Feb 2022 23:57:26 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 11 Feb 2022 23:57:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Feb 2022 23:57:26 GMT
USER memcache
# Fri, 11 Feb 2022 23:57:26 GMT
EXPOSE 11211
# Fri, 11 Feb 2022 23:57:26 GMT
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
	-	`sha256:7bccd1e890d9edaaa99814caec66d49d04d5245aca1fe8a2ac832be7e0e09c06`  
		Last Modified: Fri, 11 Feb 2022 23:58:42 GMT  
		Size: 2.1 MB (2148137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75931a88b924783decffcbf2e1fba6e58f393e9409dd37ffb26b7f6eecffdef2`  
		Last Modified: Fri, 11 Feb 2022 23:58:41 GMT  
		Size: 282.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2dd123370c89ee375732af5193be621336dd45eae2b9729fb66d0376bc915cc`  
		Last Modified: Fri, 11 Feb 2022 23:58:41 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:1.6.14-alpine3.15`

```console
$ docker pull memcached@sha256:76e5acd480d7bd36706f7873f5f7278ff5085b62840afffc3cefbcef0a3a9509
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `memcached:1.6.14-alpine3.15` - linux; amd64

```console
$ docker pull memcached@sha256:e79dd6dea75bf64de1cd87b2204574865bcc12fcda9e1d5c63ce82e3271d4bdf
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.3 MB (5345174 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31403aa3ac88632da679879fcb0a3a627c6f50ec7da0659ae032f63d289d9587`
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
# Fri, 11 Feb 2022 23:43:32 GMT
ENV MEMCACHED_VERSION=1.6.14
# Fri, 11 Feb 2022 23:43:32 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Fri, 11 Feb 2022 23:47:43 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Fri, 11 Feb 2022 23:47:43 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 11 Feb 2022 23:47:44 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 11 Feb 2022 23:47:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Feb 2022 23:47:44 GMT
USER memcache
# Fri, 11 Feb 2022 23:47:45 GMT
EXPOSE 11211
# Fri, 11 Feb 2022 23:47:45 GMT
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
	-	`sha256:4afc0667aa68ec7c0a865809dcfee799f6357b1f6d6c4d6e58240cff71c6264d`  
		Last Modified: Fri, 11 Feb 2022 23:48:39 GMT  
		Size: 2.4 MB (2415863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef8943e1197199b34fc9e9230f24d760a30cdcf11c6b8fc48e89592e00da6edf`  
		Last Modified: Fri, 11 Feb 2022 23:48:38 GMT  
		Size: 283.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b10635796b46c66fb5447019c111ad88d5b808536aab4757aa60b57ffcc9d0da`  
		Last Modified: Fri, 11 Feb 2022 23:48:38 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.14-alpine3.15` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:c28cbb9d278a2ef6c4ef325c2fffa8bc4631258a341cb411d2a7bec9655007cb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.1 MB (5109831 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e10238b3468650bbfa09ac13b6115339c5305e3e92cb34bb47b6a03b2a93df01`
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
# Fri, 11 Feb 2022 23:59:43 GMT
ENV MEMCACHED_VERSION=1.6.14
# Fri, 11 Feb 2022 23:59:44 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Sat, 12 Feb 2022 00:02:34 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Sat, 12 Feb 2022 00:02:36 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Sat, 12 Feb 2022 00:02:36 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Sat, 12 Feb 2022 00:02:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 12 Feb 2022 00:02:38 GMT
USER memcache
# Sat, 12 Feb 2022 00:02:39 GMT
EXPOSE 11211
# Sat, 12 Feb 2022 00:02:40 GMT
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
	-	`sha256:98b2012c64d2efed092c8ec83344fc68be38873465f9e7b82616b504ca67ea14`  
		Last Modified: Sat, 12 Feb 2022 00:03:57 GMT  
		Size: 2.3 MB (2282236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b54695eeb42571708a7da87031a54d3f82b1be9e474102eeaa912ee51cb86d3`  
		Last Modified: Sat, 12 Feb 2022 00:03:57 GMT  
		Size: 283.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17690cc3c867c822f67c6edabb66fd363b8988e13ed76d6b2a512a4af041bd58`  
		Last Modified: Sat, 12 Feb 2022 00:03:57 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.14-alpine3.15` - linux; 386

```console
$ docker pull memcached@sha256:5b9731ba5ab72d85a6ed73548a502d6e22d512f328daacddeb531c252745a1e7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.4 MB (5369203 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:83c422eacdcda2fa728cc1fc176ab0cd57a0be7766f0b517dcc64045b255d0a9`
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
# Fri, 11 Feb 2022 23:43:00 GMT
ENV MEMCACHED_VERSION=1.6.14
# Fri, 11 Feb 2022 23:43:01 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Fri, 11 Feb 2022 23:47:20 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Fri, 11 Feb 2022 23:47:20 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 11 Feb 2022 23:47:21 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 11 Feb 2022 23:47:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Feb 2022 23:47:22 GMT
USER memcache
# Fri, 11 Feb 2022 23:47:22 GMT
EXPOSE 11211
# Fri, 11 Feb 2022 23:47:22 GMT
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
	-	`sha256:62d0cbe6f51da8f3bfd9d0bfbbb510f173b231cfc4260066e5da12995d012223`  
		Last Modified: Fri, 11 Feb 2022 23:48:48 GMT  
		Size: 2.4 MB (2419277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfa2ab27dc5f099b91f7195a3d75e51e7f2c84ea56052a565dcbeba235da559b`  
		Last Modified: Fri, 11 Feb 2022 23:48:47 GMT  
		Size: 283.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0394921490062e0dab12bc6f8a3a5bd3f1a97dc261653593a22e3fa95776186`  
		Last Modified: Fri, 11 Feb 2022 23:48:47 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.14-alpine3.15` - linux; ppc64le

```console
$ docker pull memcached@sha256:75cb5141098fb02bb0c554c31c00d28802b414593a6b41d430c10505ee943fe0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.3 MB (5315837 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4be74852968716dd05ad711f1cda531afac5b782fe0dd6692e5aed7d91d54466`
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
# Fri, 11 Feb 2022 23:54:02 GMT
ENV MEMCACHED_VERSION=1.6.14
# Fri, 11 Feb 2022 23:54:06 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Fri, 11 Feb 2022 23:57:48 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Fri, 11 Feb 2022 23:57:50 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 11 Feb 2022 23:57:55 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 11 Feb 2022 23:57:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Feb 2022 23:57:59 GMT
USER memcache
# Fri, 11 Feb 2022 23:58:01 GMT
EXPOSE 11211
# Fri, 11 Feb 2022 23:58:02 GMT
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
	-	`sha256:e9d933f0d59015113f25123de9b3460a03fdf091181f4c9330b1bb42c27a8cce`  
		Last Modified: Fri, 11 Feb 2022 23:59:16 GMT  
		Size: 2.4 MB (2373175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:659fd1f60c2bc05966f606e677370eeee3176f7d6dbd530b3f271ba313f8b0fe`  
		Last Modified: Fri, 11 Feb 2022 23:59:15 GMT  
		Size: 282.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8d9d86e7310ff252ce602224ce1643c6b8d50713444e43804cdb93912f89087`  
		Last Modified: Fri, 11 Feb 2022 23:59:15 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.14-alpine3.15` - linux; s390x

```console
$ docker pull memcached@sha256:05d8b33e1a3927fd3ba6b7cd62b648d66a4f07da15103657791736e70515bd20
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4869494 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a751c73ff4357b7992c0a524e080537c462baa079ef3c7b96a3ce7b13699135`
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
# Fri, 11 Feb 2022 23:53:09 GMT
ENV MEMCACHED_VERSION=1.6.14
# Fri, 11 Feb 2022 23:53:09 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Fri, 11 Feb 2022 23:57:25 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Fri, 11 Feb 2022 23:57:25 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 11 Feb 2022 23:57:26 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 11 Feb 2022 23:57:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Feb 2022 23:57:26 GMT
USER memcache
# Fri, 11 Feb 2022 23:57:26 GMT
EXPOSE 11211
# Fri, 11 Feb 2022 23:57:26 GMT
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
	-	`sha256:7bccd1e890d9edaaa99814caec66d49d04d5245aca1fe8a2ac832be7e0e09c06`  
		Last Modified: Fri, 11 Feb 2022 23:58:42 GMT  
		Size: 2.1 MB (2148137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75931a88b924783decffcbf2e1fba6e58f393e9409dd37ffb26b7f6eecffdef2`  
		Last Modified: Fri, 11 Feb 2022 23:58:41 GMT  
		Size: 282.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2dd123370c89ee375732af5193be621336dd45eae2b9729fb66d0376bc915cc`  
		Last Modified: Fri, 11 Feb 2022 23:58:41 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:1.6.14-bullseye`

```console
$ docker pull memcached@sha256:e4bb2d212309e51166f29fe5404edf5caf784ada9ab3fde8dcf8226f337878aa
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

### `memcached:1.6.14-bullseye` - linux; amd64

```console
$ docker pull memcached@sha256:2c29149daad601e046074c6801fb570180d4eba60047135b71f51ea327ffcbc1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.0 MB (32954984 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6208dafa350f4dfbb3f2a16e20c2f2d256f894fd8695ac24b21663a732dee124`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 01 Mar 2022 02:13:29 GMT
ADD file:d48a85028743f16ed927507322e3e3beee187fbfadd0b781d4b89de197c64b5b in / 
# Tue, 01 Mar 2022 02:13:29 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 13:24:57 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 01 Mar 2022 13:25:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 13:25:02 GMT
ENV MEMCACHED_VERSION=1.6.14
# Tue, 01 Mar 2022 13:25:02 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Tue, 01 Mar 2022 13:28:58 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 01 Mar 2022 13:28:58 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 01 Mar 2022 13:28:59 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 01 Mar 2022 13:28:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 01 Mar 2022 13:29:00 GMT
USER memcache
# Tue, 01 Mar 2022 13:29:00 GMT
EXPOSE 11211
# Tue, 01 Mar 2022 13:29:00 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:f7a1c6dad28192bd417b78079d6ddc03cbca6d5ea46bba12769b235b6353c00c`  
		Last Modified: Tue, 01 Mar 2022 02:19:23 GMT  
		Size: 31.4 MB (31366396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3292b9ed039a5211ec564a1f170046ba2ad296a19beb778d3c7106a230301d27`  
		Last Modified: Tue, 01 Mar 2022 13:29:33 GMT  
		Size: 5.0 KB (4980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15c683705067bdb5151c087a9b5e91a37f498912588e29970e3ce07121334f03`  
		Last Modified: Tue, 01 Mar 2022 13:29:34 GMT  
		Size: 328.0 KB (328033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:091c46e57219c5fdd0a044c77fc12a24889bd1ce95e4d032e83f2ea09997ca1d`  
		Last Modified: Tue, 01 Mar 2022 13:29:34 GMT  
		Size: 1.3 MB (1255168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a26e7e13ba905fd75a5e3b2307ab4abee1bbcdc9b586d37fc2ff7984de1c92c3`  
		Last Modified: Tue, 01 Mar 2022 13:29:33 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75b625708cf5e763937f326c6fe55adcb4c4782926483ea2a3628012927922c7`  
		Last Modified: Tue, 01 Mar 2022 13:29:33 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.14-bullseye` - linux; arm variant v5

```console
$ docker pull memcached@sha256:839b663c2a5637a5a026d8bf63f2c3a5af62938b6becb246fe84e68bceb73742
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.5 MB (30457903 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:46c3d2c41f175e70fa19ec073355fc3376f15b3ca99f6fdb295b6cea57aede38`
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
# Fri, 11 Feb 2022 23:48:33 GMT
ENV MEMCACHED_VERSION=1.6.14
# Fri, 11 Feb 2022 23:48:33 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Fri, 11 Feb 2022 23:53:18 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Fri, 11 Feb 2022 23:53:19 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 11 Feb 2022 23:53:20 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 11 Feb 2022 23:53:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Feb 2022 23:53:21 GMT
USER memcache
# Fri, 11 Feb 2022 23:53:22 GMT
EXPOSE 11211
# Fri, 11 Feb 2022 23:53:22 GMT
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
	-	`sha256:4c595fdbb4287a9ef2b3565e1d9ac2caa7d17ac0810224d8a5d3c87313cc81b5`  
		Last Modified: Fri, 11 Feb 2022 23:54:16 GMT  
		Size: 1.2 MB (1226376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19c8ecb542750e6e603057b1e7bdb90fc58d45b604f20b2724d402a572f1b735`  
		Last Modified: Fri, 11 Feb 2022 23:54:15 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64d2e913eaab741b412c8fec5edbad97daed3a2c5f0a1a1fd376ea8ec7c28c52`  
		Last Modified: Fri, 11 Feb 2022 23:54:15 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.14-bullseye` - linux; arm variant v7

```console
$ docker pull memcached@sha256:c1ded327e0d4c11f7f00652600f4cbf465a119fed31e6e2541d516700e0e14c2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.1 MB (28080208 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:866cf84302a62bedfada61f236deccacb7585dc0ccce8a4e0e058b741bfafdc5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 01 Mar 2022 02:02:56 GMT
ADD file:c6b519323fd1fa09b9f8c8608778872e8fa6208cb0b42aaccdef4479a469f5f4 in / 
# Tue, 01 Mar 2022 02:02:57 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 14:02:17 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 01 Mar 2022 14:02:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 14:02:26 GMT
ENV MEMCACHED_VERSION=1.6.14
# Tue, 01 Mar 2022 14:02:26 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Tue, 01 Mar 2022 14:06:15 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 01 Mar 2022 14:06:16 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 01 Mar 2022 14:06:17 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 01 Mar 2022 14:06:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 01 Mar 2022 14:06:18 GMT
USER memcache
# Tue, 01 Mar 2022 14:06:19 GMT
EXPOSE 11211
# Tue, 01 Mar 2022 14:06:19 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:59dbb2ac3829352dd707e28e037734c9fbdef5b03aea31e3929ddcead949afee`  
		Last Modified: Tue, 01 Mar 2022 02:19:09 GMT  
		Size: 26.6 MB (26565105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45ff8679190bbfe567a01e354c79eb44efaa4564b0770a644b9eb6a28f10812c`  
		Last Modified: Tue, 01 Mar 2022 14:19:16 GMT  
		Size: 4.9 KB (4894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13db11031aa185885b3b1b9c74eba0d8ea9b07d5e8fec5870bc7df8d09585d2f`  
		Last Modified: Tue, 01 Mar 2022 14:19:16 GMT  
		Size: 312.0 KB (312009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:079efee4f8d1e8cea53f0cc6ddc4832de31e69c43411b81e790e0615eeea16aa`  
		Last Modified: Tue, 01 Mar 2022 14:19:16 GMT  
		Size: 1.2 MB (1197793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:050fbe09656330899bb983ba6d0871a6cc96349c4c049673a4ee53816db5ff7b`  
		Last Modified: Tue, 01 Mar 2022 14:19:16 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcca636453f4acf7b597c080e2d7c57ea366f36daae56acdd43664bb28dff985`  
		Last Modified: Tue, 01 Mar 2022 14:19:16 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.14-bullseye` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:c59ae38d83ce474dc14423325e3f500a06e285938b4f4e8a013ae8967603d492
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.4 MB (31435417 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b5c5ad61ebd09fab08b612599fdf9e96be59696045e4765dac554781daef4d1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 01 Mar 2022 02:11:29 GMT
ADD file:9816c9c29627693c34afda4fa5e1a5e8a0f5aa3c5d5cfd920a4d89c77aab997d in / 
# Tue, 01 Mar 2022 02:11:30 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 12:44:12 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 01 Mar 2022 12:44:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 12:44:16 GMT
ENV MEMCACHED_VERSION=1.6.14
# Tue, 01 Mar 2022 12:44:17 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Tue, 01 Mar 2022 12:46:49 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 01 Mar 2022 12:46:50 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 01 Mar 2022 12:46:50 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 01 Mar 2022 12:46:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 01 Mar 2022 12:46:52 GMT
USER memcache
# Tue, 01 Mar 2022 12:46:53 GMT
EXPOSE 11211
# Tue, 01 Mar 2022 12:46:54 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:279a020076a7fbddfc996e4c55e605a8f322810c3eca21cdedbcb06beb0e1305`  
		Last Modified: Tue, 01 Mar 2022 02:18:24 GMT  
		Size: 30.1 MB (30057008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7dfd1ea3d9e177e785365db9a22591801c15e6a33097ba79a048e3387f4c43a`  
		Last Modified: Tue, 01 Mar 2022 12:47:45 GMT  
		Size: 4.9 KB (4902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e563a531f0653c96d3786deff2afe7190769b5929d06c8c234d89fd314bf2396`  
		Last Modified: Tue, 01 Mar 2022 12:47:45 GMT  
		Size: 119.2 KB (119172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1d1b1b990f1e4e95a5410acd589565956a1fd54c4df3b71a665dcfb23ac9f76`  
		Last Modified: Tue, 01 Mar 2022 12:47:46 GMT  
		Size: 1.3 MB (1253928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b8a7c0be94d102b9a04c359186fcf59b223183acc8b489d0ca12afb8f073027`  
		Last Modified: Tue, 01 Mar 2022 12:47:45 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:091c7ee2fb4e34177c30b2b9905bf098f304bea040ff7ca5700134d4921c2758`  
		Last Modified: Tue, 01 Mar 2022 12:47:45 GMT  
		Size: 120.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.14-bullseye` - linux; 386

```console
$ docker pull memcached@sha256:4c9eb4902e2601bad18a1783dbf7d64cf25f6121226d4772a5d36a7ac3e9db79
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.0 MB (33972554 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af09c75e25cf0ea60c4f155a25728e256411f07898946ea08e869eb6362e3a24`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 01 Mar 2022 02:07:32 GMT
ADD file:e92ab504d4c0d3bd63da83254e6ca400b607c32e0f5037039648559b91770870 in / 
# Tue, 01 Mar 2022 02:07:33 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 10:07:23 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 01 Mar 2022 10:07:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 10:07:30 GMT
ENV MEMCACHED_VERSION=1.6.14
# Tue, 01 Mar 2022 10:07:30 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Tue, 01 Mar 2022 10:11:57 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 01 Mar 2022 10:11:57 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 01 Mar 2022 10:11:58 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 01 Mar 2022 10:11:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 01 Mar 2022 10:11:58 GMT
USER memcache
# Tue, 01 Mar 2022 10:11:58 GMT
EXPOSE 11211
# Tue, 01 Mar 2022 10:11:59 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:04a87e821be7e4b29d48011b7aa4ff884ca57fd36995cb3b99fd2fc24ac562d8`  
		Last Modified: Tue, 01 Mar 2022 02:15:51 GMT  
		Size: 32.4 MB (32377389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe860ecc70fbef589f9779541d957321138c3f41d99742ca7ff2bb41b6787786`  
		Last Modified: Tue, 01 Mar 2022 10:13:02 GMT  
		Size: 4.9 KB (4889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71fbbf846282a29c58595e09b8a5d93a6348fc5a77d0bb513263f933972610e8`  
		Last Modified: Tue, 01 Mar 2022 10:13:03 GMT  
		Size: 336.6 KB (336603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f93f31af2adb455df5e2c7baaa190b479d463d37657734ee855d663709906a2`  
		Last Modified: Tue, 01 Mar 2022 10:13:03 GMT  
		Size: 1.3 MB (1253268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ea06973bd5c70feb976fde3006e5400760f293973d5a2a8f8a05a73105a5851`  
		Last Modified: Tue, 01 Mar 2022 10:13:02 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c85296c039a2ca9f99139e04d26550a26b109424a80e9377a115129110257b9`  
		Last Modified: Tue, 01 Mar 2022 10:13:02 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.14-bullseye` - linux; mips64le

```console
$ docker pull memcached@sha256:76269e61918b56719946fa47ffaebf468965e45dae401738fcd6d8ea6d9afdc1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.2 MB (31213138 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bdf2a1611553c4acfb426a9736777620af35250c1c3fde4997dd8fda25547725`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 01 Mar 2022 02:02:49 GMT
ADD file:1901e1e1292cbfcd557262ec5d08551cecd0070b24928414d220472664fe3fdf in / 
# Tue, 01 Mar 2022 02:02:49 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 03:43:18 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 01 Mar 2022 03:43:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 03:43:30 GMT
ENV MEMCACHED_VERSION=1.6.14
# Tue, 01 Mar 2022 03:43:30 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Tue, 01 Mar 2022 03:49:17 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 01 Mar 2022 03:49:17 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 01 Mar 2022 03:49:19 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 01 Mar 2022 03:49:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 01 Mar 2022 03:49:20 GMT
USER memcache
# Tue, 01 Mar 2022 03:49:20 GMT
EXPOSE 11211
# Tue, 01 Mar 2022 03:49:20 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:3baeb8c34a522fc616f97412d47dc1f665e93552c57aa8237ee1d673f9757cba`  
		Last Modified: Tue, 01 Mar 2022 02:12:25 GMT  
		Size: 29.6 MB (29632966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50a63f21594c0da6641452e9cd0caaf8727bae4ca86c617384198ab5d8e766ec`  
		Last Modified: Tue, 01 Mar 2022 03:49:43 GMT  
		Size: 5.0 KB (4979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dfb3a0cb8d59939fa0e67d13c57840042b1397d36d3c1918e50344eb405025d`  
		Last Modified: Tue, 01 Mar 2022 03:49:43 GMT  
		Size: 323.7 KB (323703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e632b2b5bf88ea94d56d701fa93b55516003db1fc7c855bb4569f2be0ddf3be`  
		Last Modified: Tue, 01 Mar 2022 03:49:43 GMT  
		Size: 1.3 MB (1251083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1fc0f9b2a7499de336af3103d86d1ffc3b90b62ea850295c0c57abbe68c753b`  
		Last Modified: Tue, 01 Mar 2022 03:49:43 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe1ee7b4dd056bb3eadc09b9893ce88a096e51500bbe841d1c145be10ba2b1f0`  
		Last Modified: Tue, 01 Mar 2022 03:49:43 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.14-bullseye` - linux; ppc64le

```console
$ docker pull memcached@sha256:4893f4daa742b31f414b08f98f8e7d0cbedaf63b8d88062bcf3c91a9522a2aab
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.0 MB (36957544 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8db953cc998ed06712eca57fe4ae2b8bb342ce991683fd7592495a21557d0940`
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
# Fri, 11 Feb 2022 23:47:36 GMT
ENV MEMCACHED_VERSION=1.6.14
# Fri, 11 Feb 2022 23:47:38 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Fri, 11 Feb 2022 23:53:07 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Fri, 11 Feb 2022 23:53:13 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 11 Feb 2022 23:53:34 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 11 Feb 2022 23:53:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Feb 2022 23:53:39 GMT
USER memcache
# Fri, 11 Feb 2022 23:53:41 GMT
EXPOSE 11211
# Fri, 11 Feb 2022 23:53:46 GMT
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
	-	`sha256:d5f2e5d5bb1609e336a37e97218d618550ec5ce28384c32b1141393ef6f04a03`  
		Last Modified: Fri, 11 Feb 2022 23:58:44 GMT  
		Size: 1.3 MB (1322220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76e6da4f290b1cff2fa5b1ad17d42333c67179332511db4da3bd2c5ce12bbdfa`  
		Last Modified: Fri, 11 Feb 2022 23:58:44 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fb140c5468aa121999bc169d30e4ce6b73795cdf67aa21c1dfd3d1194dd0b82`  
		Last Modified: Fri, 11 Feb 2022 23:58:44 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.14-bullseye` - linux; s390x

```console
$ docker pull memcached@sha256:14b3ae46a3b5dc4d1ca410da43e53ee0c44ad49ec398f235628f89bc8cc0a0cc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.2 MB (31217166 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:50f1b3aef9bc393e3b1a3fab35c702d6a9b9dd6fa2abd9d044b52385b9ccf549`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 01 Mar 2022 02:01:56 GMT
ADD file:d869ad3392a4e752c2f73d08a4cc13594c94bfc050bd037db0ca9827a0207072 in / 
# Tue, 01 Mar 2022 02:01:58 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 13:28:37 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 01 Mar 2022 13:28:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 13:28:40 GMT
ENV MEMCACHED_VERSION=1.6.14
# Tue, 01 Mar 2022 13:28:40 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Tue, 01 Mar 2022 13:31:58 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 01 Mar 2022 13:31:58 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 01 Mar 2022 13:31:58 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 01 Mar 2022 13:31:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 01 Mar 2022 13:31:59 GMT
USER memcache
# Tue, 01 Mar 2022 13:31:59 GMT
EXPOSE 11211
# Tue, 01 Mar 2022 13:31:59 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:f81abce72636770dac4258df46a31beeb6ad81dfddd5b7c9c3fa6942ea074922`  
		Last Modified: Tue, 01 Mar 2022 02:07:33 GMT  
		Size: 29.6 MB (29647132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b43f274641c42412c1e075acb3920020215603d1e1c938fa84211ea8b005988`  
		Last Modified: Tue, 01 Mar 2022 13:32:52 GMT  
		Size: 5.0 KB (5024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d135f121f1aff6ea16284d2286318c703c72dad45560bdc68ac2bc2371f8164`  
		Last Modified: Tue, 01 Mar 2022 13:32:52 GMT  
		Size: 324.1 KB (324102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9255401f181741c77541d42f93796b72c20077b2815b9e6c4e21b36f9bcccab6`  
		Last Modified: Tue, 01 Mar 2022 13:32:52 GMT  
		Size: 1.2 MB (1240500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5436de37a983faa64cc9d82c3a8272ae77b107e2f8bcd453f7aee5e3e92def7`  
		Last Modified: Tue, 01 Mar 2022 13:32:52 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8296feb21176186e1c4027cf5e8111ed103c7b2b30f1f4423a9303a0e7fd9d3`  
		Last Modified: Tue, 01 Mar 2022 13:32:52 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:alpine`

```console
$ docker pull memcached@sha256:a37fd6c034a7e4334d091beedffb525aae8af4acc0cee3030758ae3edc0c524b
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
$ docker pull memcached@sha256:e79dd6dea75bf64de1cd87b2204574865bcc12fcda9e1d5c63ce82e3271d4bdf
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.3 MB (5345174 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31403aa3ac88632da679879fcb0a3a627c6f50ec7da0659ae032f63d289d9587`
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
# Fri, 11 Feb 2022 23:43:32 GMT
ENV MEMCACHED_VERSION=1.6.14
# Fri, 11 Feb 2022 23:43:32 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Fri, 11 Feb 2022 23:47:43 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Fri, 11 Feb 2022 23:47:43 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 11 Feb 2022 23:47:44 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 11 Feb 2022 23:47:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Feb 2022 23:47:44 GMT
USER memcache
# Fri, 11 Feb 2022 23:47:45 GMT
EXPOSE 11211
# Fri, 11 Feb 2022 23:47:45 GMT
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
	-	`sha256:4afc0667aa68ec7c0a865809dcfee799f6357b1f6d6c4d6e58240cff71c6264d`  
		Last Modified: Fri, 11 Feb 2022 23:48:39 GMT  
		Size: 2.4 MB (2415863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef8943e1197199b34fc9e9230f24d760a30cdcf11c6b8fc48e89592e00da6edf`  
		Last Modified: Fri, 11 Feb 2022 23:48:38 GMT  
		Size: 283.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b10635796b46c66fb5447019c111ad88d5b808536aab4757aa60b57ffcc9d0da`  
		Last Modified: Fri, 11 Feb 2022 23:48:38 GMT  
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
$ docker pull memcached@sha256:c28cbb9d278a2ef6c4ef325c2fffa8bc4631258a341cb411d2a7bec9655007cb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.1 MB (5109831 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e10238b3468650bbfa09ac13b6115339c5305e3e92cb34bb47b6a03b2a93df01`
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
# Fri, 11 Feb 2022 23:59:43 GMT
ENV MEMCACHED_VERSION=1.6.14
# Fri, 11 Feb 2022 23:59:44 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Sat, 12 Feb 2022 00:02:34 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Sat, 12 Feb 2022 00:02:36 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Sat, 12 Feb 2022 00:02:36 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Sat, 12 Feb 2022 00:02:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 12 Feb 2022 00:02:38 GMT
USER memcache
# Sat, 12 Feb 2022 00:02:39 GMT
EXPOSE 11211
# Sat, 12 Feb 2022 00:02:40 GMT
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
	-	`sha256:98b2012c64d2efed092c8ec83344fc68be38873465f9e7b82616b504ca67ea14`  
		Last Modified: Sat, 12 Feb 2022 00:03:57 GMT  
		Size: 2.3 MB (2282236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b54695eeb42571708a7da87031a54d3f82b1be9e474102eeaa912ee51cb86d3`  
		Last Modified: Sat, 12 Feb 2022 00:03:57 GMT  
		Size: 283.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17690cc3c867c822f67c6edabb66fd363b8988e13ed76d6b2a512a4af041bd58`  
		Last Modified: Sat, 12 Feb 2022 00:03:57 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:alpine` - linux; 386

```console
$ docker pull memcached@sha256:5b9731ba5ab72d85a6ed73548a502d6e22d512f328daacddeb531c252745a1e7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.4 MB (5369203 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:83c422eacdcda2fa728cc1fc176ab0cd57a0be7766f0b517dcc64045b255d0a9`
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
# Fri, 11 Feb 2022 23:43:00 GMT
ENV MEMCACHED_VERSION=1.6.14
# Fri, 11 Feb 2022 23:43:01 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Fri, 11 Feb 2022 23:47:20 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Fri, 11 Feb 2022 23:47:20 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 11 Feb 2022 23:47:21 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 11 Feb 2022 23:47:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Feb 2022 23:47:22 GMT
USER memcache
# Fri, 11 Feb 2022 23:47:22 GMT
EXPOSE 11211
# Fri, 11 Feb 2022 23:47:22 GMT
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
	-	`sha256:62d0cbe6f51da8f3bfd9d0bfbbb510f173b231cfc4260066e5da12995d012223`  
		Last Modified: Fri, 11 Feb 2022 23:48:48 GMT  
		Size: 2.4 MB (2419277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfa2ab27dc5f099b91f7195a3d75e51e7f2c84ea56052a565dcbeba235da559b`  
		Last Modified: Fri, 11 Feb 2022 23:48:47 GMT  
		Size: 283.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0394921490062e0dab12bc6f8a3a5bd3f1a97dc261653593a22e3fa95776186`  
		Last Modified: Fri, 11 Feb 2022 23:48:47 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:alpine` - linux; ppc64le

```console
$ docker pull memcached@sha256:75cb5141098fb02bb0c554c31c00d28802b414593a6b41d430c10505ee943fe0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.3 MB (5315837 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4be74852968716dd05ad711f1cda531afac5b782fe0dd6692e5aed7d91d54466`
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
# Fri, 11 Feb 2022 23:54:02 GMT
ENV MEMCACHED_VERSION=1.6.14
# Fri, 11 Feb 2022 23:54:06 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Fri, 11 Feb 2022 23:57:48 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Fri, 11 Feb 2022 23:57:50 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 11 Feb 2022 23:57:55 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 11 Feb 2022 23:57:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Feb 2022 23:57:59 GMT
USER memcache
# Fri, 11 Feb 2022 23:58:01 GMT
EXPOSE 11211
# Fri, 11 Feb 2022 23:58:02 GMT
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
	-	`sha256:e9d933f0d59015113f25123de9b3460a03fdf091181f4c9330b1bb42c27a8cce`  
		Last Modified: Fri, 11 Feb 2022 23:59:16 GMT  
		Size: 2.4 MB (2373175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:659fd1f60c2bc05966f606e677370eeee3176f7d6dbd530b3f271ba313f8b0fe`  
		Last Modified: Fri, 11 Feb 2022 23:59:15 GMT  
		Size: 282.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8d9d86e7310ff252ce602224ce1643c6b8d50713444e43804cdb93912f89087`  
		Last Modified: Fri, 11 Feb 2022 23:59:15 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:alpine` - linux; s390x

```console
$ docker pull memcached@sha256:05d8b33e1a3927fd3ba6b7cd62b648d66a4f07da15103657791736e70515bd20
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4869494 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a751c73ff4357b7992c0a524e080537c462baa079ef3c7b96a3ce7b13699135`
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
# Fri, 11 Feb 2022 23:53:09 GMT
ENV MEMCACHED_VERSION=1.6.14
# Fri, 11 Feb 2022 23:53:09 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Fri, 11 Feb 2022 23:57:25 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Fri, 11 Feb 2022 23:57:25 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 11 Feb 2022 23:57:26 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 11 Feb 2022 23:57:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Feb 2022 23:57:26 GMT
USER memcache
# Fri, 11 Feb 2022 23:57:26 GMT
EXPOSE 11211
# Fri, 11 Feb 2022 23:57:26 GMT
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
	-	`sha256:7bccd1e890d9edaaa99814caec66d49d04d5245aca1fe8a2ac832be7e0e09c06`  
		Last Modified: Fri, 11 Feb 2022 23:58:42 GMT  
		Size: 2.1 MB (2148137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75931a88b924783decffcbf2e1fba6e58f393e9409dd37ffb26b7f6eecffdef2`  
		Last Modified: Fri, 11 Feb 2022 23:58:41 GMT  
		Size: 282.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2dd123370c89ee375732af5193be621336dd45eae2b9729fb66d0376bc915cc`  
		Last Modified: Fri, 11 Feb 2022 23:58:41 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:alpine3.15`

```console
$ docker pull memcached@sha256:76e5acd480d7bd36706f7873f5f7278ff5085b62840afffc3cefbcef0a3a9509
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
$ docker pull memcached@sha256:e79dd6dea75bf64de1cd87b2204574865bcc12fcda9e1d5c63ce82e3271d4bdf
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.3 MB (5345174 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31403aa3ac88632da679879fcb0a3a627c6f50ec7da0659ae032f63d289d9587`
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
# Fri, 11 Feb 2022 23:43:32 GMT
ENV MEMCACHED_VERSION=1.6.14
# Fri, 11 Feb 2022 23:43:32 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Fri, 11 Feb 2022 23:47:43 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Fri, 11 Feb 2022 23:47:43 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 11 Feb 2022 23:47:44 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 11 Feb 2022 23:47:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Feb 2022 23:47:44 GMT
USER memcache
# Fri, 11 Feb 2022 23:47:45 GMT
EXPOSE 11211
# Fri, 11 Feb 2022 23:47:45 GMT
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
	-	`sha256:4afc0667aa68ec7c0a865809dcfee799f6357b1f6d6c4d6e58240cff71c6264d`  
		Last Modified: Fri, 11 Feb 2022 23:48:39 GMT  
		Size: 2.4 MB (2415863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef8943e1197199b34fc9e9230f24d760a30cdcf11c6b8fc48e89592e00da6edf`  
		Last Modified: Fri, 11 Feb 2022 23:48:38 GMT  
		Size: 283.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b10635796b46c66fb5447019c111ad88d5b808536aab4757aa60b57ffcc9d0da`  
		Last Modified: Fri, 11 Feb 2022 23:48:38 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:alpine3.15` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:c28cbb9d278a2ef6c4ef325c2fffa8bc4631258a341cb411d2a7bec9655007cb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.1 MB (5109831 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e10238b3468650bbfa09ac13b6115339c5305e3e92cb34bb47b6a03b2a93df01`
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
# Fri, 11 Feb 2022 23:59:43 GMT
ENV MEMCACHED_VERSION=1.6.14
# Fri, 11 Feb 2022 23:59:44 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Sat, 12 Feb 2022 00:02:34 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Sat, 12 Feb 2022 00:02:36 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Sat, 12 Feb 2022 00:02:36 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Sat, 12 Feb 2022 00:02:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 12 Feb 2022 00:02:38 GMT
USER memcache
# Sat, 12 Feb 2022 00:02:39 GMT
EXPOSE 11211
# Sat, 12 Feb 2022 00:02:40 GMT
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
	-	`sha256:98b2012c64d2efed092c8ec83344fc68be38873465f9e7b82616b504ca67ea14`  
		Last Modified: Sat, 12 Feb 2022 00:03:57 GMT  
		Size: 2.3 MB (2282236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b54695eeb42571708a7da87031a54d3f82b1be9e474102eeaa912ee51cb86d3`  
		Last Modified: Sat, 12 Feb 2022 00:03:57 GMT  
		Size: 283.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17690cc3c867c822f67c6edabb66fd363b8988e13ed76d6b2a512a4af041bd58`  
		Last Modified: Sat, 12 Feb 2022 00:03:57 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:alpine3.15` - linux; 386

```console
$ docker pull memcached@sha256:5b9731ba5ab72d85a6ed73548a502d6e22d512f328daacddeb531c252745a1e7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.4 MB (5369203 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:83c422eacdcda2fa728cc1fc176ab0cd57a0be7766f0b517dcc64045b255d0a9`
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
# Fri, 11 Feb 2022 23:43:00 GMT
ENV MEMCACHED_VERSION=1.6.14
# Fri, 11 Feb 2022 23:43:01 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Fri, 11 Feb 2022 23:47:20 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Fri, 11 Feb 2022 23:47:20 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 11 Feb 2022 23:47:21 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 11 Feb 2022 23:47:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Feb 2022 23:47:22 GMT
USER memcache
# Fri, 11 Feb 2022 23:47:22 GMT
EXPOSE 11211
# Fri, 11 Feb 2022 23:47:22 GMT
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
	-	`sha256:62d0cbe6f51da8f3bfd9d0bfbbb510f173b231cfc4260066e5da12995d012223`  
		Last Modified: Fri, 11 Feb 2022 23:48:48 GMT  
		Size: 2.4 MB (2419277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfa2ab27dc5f099b91f7195a3d75e51e7f2c84ea56052a565dcbeba235da559b`  
		Last Modified: Fri, 11 Feb 2022 23:48:47 GMT  
		Size: 283.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0394921490062e0dab12bc6f8a3a5bd3f1a97dc261653593a22e3fa95776186`  
		Last Modified: Fri, 11 Feb 2022 23:48:47 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:alpine3.15` - linux; ppc64le

```console
$ docker pull memcached@sha256:75cb5141098fb02bb0c554c31c00d28802b414593a6b41d430c10505ee943fe0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.3 MB (5315837 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4be74852968716dd05ad711f1cda531afac5b782fe0dd6692e5aed7d91d54466`
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
# Fri, 11 Feb 2022 23:54:02 GMT
ENV MEMCACHED_VERSION=1.6.14
# Fri, 11 Feb 2022 23:54:06 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Fri, 11 Feb 2022 23:57:48 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Fri, 11 Feb 2022 23:57:50 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 11 Feb 2022 23:57:55 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 11 Feb 2022 23:57:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Feb 2022 23:57:59 GMT
USER memcache
# Fri, 11 Feb 2022 23:58:01 GMT
EXPOSE 11211
# Fri, 11 Feb 2022 23:58:02 GMT
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
	-	`sha256:e9d933f0d59015113f25123de9b3460a03fdf091181f4c9330b1bb42c27a8cce`  
		Last Modified: Fri, 11 Feb 2022 23:59:16 GMT  
		Size: 2.4 MB (2373175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:659fd1f60c2bc05966f606e677370eeee3176f7d6dbd530b3f271ba313f8b0fe`  
		Last Modified: Fri, 11 Feb 2022 23:59:15 GMT  
		Size: 282.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8d9d86e7310ff252ce602224ce1643c6b8d50713444e43804cdb93912f89087`  
		Last Modified: Fri, 11 Feb 2022 23:59:15 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:alpine3.15` - linux; s390x

```console
$ docker pull memcached@sha256:05d8b33e1a3927fd3ba6b7cd62b648d66a4f07da15103657791736e70515bd20
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4869494 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a751c73ff4357b7992c0a524e080537c462baa079ef3c7b96a3ce7b13699135`
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
# Fri, 11 Feb 2022 23:53:09 GMT
ENV MEMCACHED_VERSION=1.6.14
# Fri, 11 Feb 2022 23:53:09 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Fri, 11 Feb 2022 23:57:25 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Fri, 11 Feb 2022 23:57:25 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 11 Feb 2022 23:57:26 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 11 Feb 2022 23:57:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Feb 2022 23:57:26 GMT
USER memcache
# Fri, 11 Feb 2022 23:57:26 GMT
EXPOSE 11211
# Fri, 11 Feb 2022 23:57:26 GMT
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
	-	`sha256:7bccd1e890d9edaaa99814caec66d49d04d5245aca1fe8a2ac832be7e0e09c06`  
		Last Modified: Fri, 11 Feb 2022 23:58:42 GMT  
		Size: 2.1 MB (2148137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75931a88b924783decffcbf2e1fba6e58f393e9409dd37ffb26b7f6eecffdef2`  
		Last Modified: Fri, 11 Feb 2022 23:58:41 GMT  
		Size: 282.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2dd123370c89ee375732af5193be621336dd45eae2b9729fb66d0376bc915cc`  
		Last Modified: Fri, 11 Feb 2022 23:58:41 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:bullseye`

```console
$ docker pull memcached@sha256:e4bb2d212309e51166f29fe5404edf5caf784ada9ab3fde8dcf8226f337878aa
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
$ docker pull memcached@sha256:2c29149daad601e046074c6801fb570180d4eba60047135b71f51ea327ffcbc1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.0 MB (32954984 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6208dafa350f4dfbb3f2a16e20c2f2d256f894fd8695ac24b21663a732dee124`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 01 Mar 2022 02:13:29 GMT
ADD file:d48a85028743f16ed927507322e3e3beee187fbfadd0b781d4b89de197c64b5b in / 
# Tue, 01 Mar 2022 02:13:29 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 13:24:57 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 01 Mar 2022 13:25:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 13:25:02 GMT
ENV MEMCACHED_VERSION=1.6.14
# Tue, 01 Mar 2022 13:25:02 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Tue, 01 Mar 2022 13:28:58 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 01 Mar 2022 13:28:58 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 01 Mar 2022 13:28:59 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 01 Mar 2022 13:28:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 01 Mar 2022 13:29:00 GMT
USER memcache
# Tue, 01 Mar 2022 13:29:00 GMT
EXPOSE 11211
# Tue, 01 Mar 2022 13:29:00 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:f7a1c6dad28192bd417b78079d6ddc03cbca6d5ea46bba12769b235b6353c00c`  
		Last Modified: Tue, 01 Mar 2022 02:19:23 GMT  
		Size: 31.4 MB (31366396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3292b9ed039a5211ec564a1f170046ba2ad296a19beb778d3c7106a230301d27`  
		Last Modified: Tue, 01 Mar 2022 13:29:33 GMT  
		Size: 5.0 KB (4980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15c683705067bdb5151c087a9b5e91a37f498912588e29970e3ce07121334f03`  
		Last Modified: Tue, 01 Mar 2022 13:29:34 GMT  
		Size: 328.0 KB (328033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:091c46e57219c5fdd0a044c77fc12a24889bd1ce95e4d032e83f2ea09997ca1d`  
		Last Modified: Tue, 01 Mar 2022 13:29:34 GMT  
		Size: 1.3 MB (1255168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a26e7e13ba905fd75a5e3b2307ab4abee1bbcdc9b586d37fc2ff7984de1c92c3`  
		Last Modified: Tue, 01 Mar 2022 13:29:33 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75b625708cf5e763937f326c6fe55adcb4c4782926483ea2a3628012927922c7`  
		Last Modified: Tue, 01 Mar 2022 13:29:33 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:bullseye` - linux; arm variant v5

```console
$ docker pull memcached@sha256:839b663c2a5637a5a026d8bf63f2c3a5af62938b6becb246fe84e68bceb73742
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.5 MB (30457903 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:46c3d2c41f175e70fa19ec073355fc3376f15b3ca99f6fdb295b6cea57aede38`
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
# Fri, 11 Feb 2022 23:48:33 GMT
ENV MEMCACHED_VERSION=1.6.14
# Fri, 11 Feb 2022 23:48:33 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Fri, 11 Feb 2022 23:53:18 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Fri, 11 Feb 2022 23:53:19 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 11 Feb 2022 23:53:20 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 11 Feb 2022 23:53:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Feb 2022 23:53:21 GMT
USER memcache
# Fri, 11 Feb 2022 23:53:22 GMT
EXPOSE 11211
# Fri, 11 Feb 2022 23:53:22 GMT
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
	-	`sha256:4c595fdbb4287a9ef2b3565e1d9ac2caa7d17ac0810224d8a5d3c87313cc81b5`  
		Last Modified: Fri, 11 Feb 2022 23:54:16 GMT  
		Size: 1.2 MB (1226376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19c8ecb542750e6e603057b1e7bdb90fc58d45b604f20b2724d402a572f1b735`  
		Last Modified: Fri, 11 Feb 2022 23:54:15 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64d2e913eaab741b412c8fec5edbad97daed3a2c5f0a1a1fd376ea8ec7c28c52`  
		Last Modified: Fri, 11 Feb 2022 23:54:15 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:bullseye` - linux; arm variant v7

```console
$ docker pull memcached@sha256:c1ded327e0d4c11f7f00652600f4cbf465a119fed31e6e2541d516700e0e14c2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.1 MB (28080208 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:866cf84302a62bedfada61f236deccacb7585dc0ccce8a4e0e058b741bfafdc5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 01 Mar 2022 02:02:56 GMT
ADD file:c6b519323fd1fa09b9f8c8608778872e8fa6208cb0b42aaccdef4479a469f5f4 in / 
# Tue, 01 Mar 2022 02:02:57 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 14:02:17 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 01 Mar 2022 14:02:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 14:02:26 GMT
ENV MEMCACHED_VERSION=1.6.14
# Tue, 01 Mar 2022 14:02:26 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Tue, 01 Mar 2022 14:06:15 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 01 Mar 2022 14:06:16 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 01 Mar 2022 14:06:17 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 01 Mar 2022 14:06:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 01 Mar 2022 14:06:18 GMT
USER memcache
# Tue, 01 Mar 2022 14:06:19 GMT
EXPOSE 11211
# Tue, 01 Mar 2022 14:06:19 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:59dbb2ac3829352dd707e28e037734c9fbdef5b03aea31e3929ddcead949afee`  
		Last Modified: Tue, 01 Mar 2022 02:19:09 GMT  
		Size: 26.6 MB (26565105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45ff8679190bbfe567a01e354c79eb44efaa4564b0770a644b9eb6a28f10812c`  
		Last Modified: Tue, 01 Mar 2022 14:19:16 GMT  
		Size: 4.9 KB (4894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13db11031aa185885b3b1b9c74eba0d8ea9b07d5e8fec5870bc7df8d09585d2f`  
		Last Modified: Tue, 01 Mar 2022 14:19:16 GMT  
		Size: 312.0 KB (312009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:079efee4f8d1e8cea53f0cc6ddc4832de31e69c43411b81e790e0615eeea16aa`  
		Last Modified: Tue, 01 Mar 2022 14:19:16 GMT  
		Size: 1.2 MB (1197793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:050fbe09656330899bb983ba6d0871a6cc96349c4c049673a4ee53816db5ff7b`  
		Last Modified: Tue, 01 Mar 2022 14:19:16 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcca636453f4acf7b597c080e2d7c57ea366f36daae56acdd43664bb28dff985`  
		Last Modified: Tue, 01 Mar 2022 14:19:16 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:bullseye` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:c59ae38d83ce474dc14423325e3f500a06e285938b4f4e8a013ae8967603d492
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.4 MB (31435417 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b5c5ad61ebd09fab08b612599fdf9e96be59696045e4765dac554781daef4d1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 01 Mar 2022 02:11:29 GMT
ADD file:9816c9c29627693c34afda4fa5e1a5e8a0f5aa3c5d5cfd920a4d89c77aab997d in / 
# Tue, 01 Mar 2022 02:11:30 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 12:44:12 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 01 Mar 2022 12:44:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 12:44:16 GMT
ENV MEMCACHED_VERSION=1.6.14
# Tue, 01 Mar 2022 12:44:17 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Tue, 01 Mar 2022 12:46:49 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 01 Mar 2022 12:46:50 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 01 Mar 2022 12:46:50 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 01 Mar 2022 12:46:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 01 Mar 2022 12:46:52 GMT
USER memcache
# Tue, 01 Mar 2022 12:46:53 GMT
EXPOSE 11211
# Tue, 01 Mar 2022 12:46:54 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:279a020076a7fbddfc996e4c55e605a8f322810c3eca21cdedbcb06beb0e1305`  
		Last Modified: Tue, 01 Mar 2022 02:18:24 GMT  
		Size: 30.1 MB (30057008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7dfd1ea3d9e177e785365db9a22591801c15e6a33097ba79a048e3387f4c43a`  
		Last Modified: Tue, 01 Mar 2022 12:47:45 GMT  
		Size: 4.9 KB (4902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e563a531f0653c96d3786deff2afe7190769b5929d06c8c234d89fd314bf2396`  
		Last Modified: Tue, 01 Mar 2022 12:47:45 GMT  
		Size: 119.2 KB (119172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1d1b1b990f1e4e95a5410acd589565956a1fd54c4df3b71a665dcfb23ac9f76`  
		Last Modified: Tue, 01 Mar 2022 12:47:46 GMT  
		Size: 1.3 MB (1253928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b8a7c0be94d102b9a04c359186fcf59b223183acc8b489d0ca12afb8f073027`  
		Last Modified: Tue, 01 Mar 2022 12:47:45 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:091c7ee2fb4e34177c30b2b9905bf098f304bea040ff7ca5700134d4921c2758`  
		Last Modified: Tue, 01 Mar 2022 12:47:45 GMT  
		Size: 120.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:bullseye` - linux; 386

```console
$ docker pull memcached@sha256:4c9eb4902e2601bad18a1783dbf7d64cf25f6121226d4772a5d36a7ac3e9db79
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.0 MB (33972554 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af09c75e25cf0ea60c4f155a25728e256411f07898946ea08e869eb6362e3a24`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 01 Mar 2022 02:07:32 GMT
ADD file:e92ab504d4c0d3bd63da83254e6ca400b607c32e0f5037039648559b91770870 in / 
# Tue, 01 Mar 2022 02:07:33 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 10:07:23 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 01 Mar 2022 10:07:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 10:07:30 GMT
ENV MEMCACHED_VERSION=1.6.14
# Tue, 01 Mar 2022 10:07:30 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Tue, 01 Mar 2022 10:11:57 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 01 Mar 2022 10:11:57 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 01 Mar 2022 10:11:58 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 01 Mar 2022 10:11:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 01 Mar 2022 10:11:58 GMT
USER memcache
# Tue, 01 Mar 2022 10:11:58 GMT
EXPOSE 11211
# Tue, 01 Mar 2022 10:11:59 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:04a87e821be7e4b29d48011b7aa4ff884ca57fd36995cb3b99fd2fc24ac562d8`  
		Last Modified: Tue, 01 Mar 2022 02:15:51 GMT  
		Size: 32.4 MB (32377389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe860ecc70fbef589f9779541d957321138c3f41d99742ca7ff2bb41b6787786`  
		Last Modified: Tue, 01 Mar 2022 10:13:02 GMT  
		Size: 4.9 KB (4889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71fbbf846282a29c58595e09b8a5d93a6348fc5a77d0bb513263f933972610e8`  
		Last Modified: Tue, 01 Mar 2022 10:13:03 GMT  
		Size: 336.6 KB (336603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f93f31af2adb455df5e2c7baaa190b479d463d37657734ee855d663709906a2`  
		Last Modified: Tue, 01 Mar 2022 10:13:03 GMT  
		Size: 1.3 MB (1253268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ea06973bd5c70feb976fde3006e5400760f293973d5a2a8f8a05a73105a5851`  
		Last Modified: Tue, 01 Mar 2022 10:13:02 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c85296c039a2ca9f99139e04d26550a26b109424a80e9377a115129110257b9`  
		Last Modified: Tue, 01 Mar 2022 10:13:02 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:bullseye` - linux; mips64le

```console
$ docker pull memcached@sha256:76269e61918b56719946fa47ffaebf468965e45dae401738fcd6d8ea6d9afdc1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.2 MB (31213138 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bdf2a1611553c4acfb426a9736777620af35250c1c3fde4997dd8fda25547725`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 01 Mar 2022 02:02:49 GMT
ADD file:1901e1e1292cbfcd557262ec5d08551cecd0070b24928414d220472664fe3fdf in / 
# Tue, 01 Mar 2022 02:02:49 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 03:43:18 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 01 Mar 2022 03:43:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 03:43:30 GMT
ENV MEMCACHED_VERSION=1.6.14
# Tue, 01 Mar 2022 03:43:30 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Tue, 01 Mar 2022 03:49:17 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 01 Mar 2022 03:49:17 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 01 Mar 2022 03:49:19 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 01 Mar 2022 03:49:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 01 Mar 2022 03:49:20 GMT
USER memcache
# Tue, 01 Mar 2022 03:49:20 GMT
EXPOSE 11211
# Tue, 01 Mar 2022 03:49:20 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:3baeb8c34a522fc616f97412d47dc1f665e93552c57aa8237ee1d673f9757cba`  
		Last Modified: Tue, 01 Mar 2022 02:12:25 GMT  
		Size: 29.6 MB (29632966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50a63f21594c0da6641452e9cd0caaf8727bae4ca86c617384198ab5d8e766ec`  
		Last Modified: Tue, 01 Mar 2022 03:49:43 GMT  
		Size: 5.0 KB (4979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dfb3a0cb8d59939fa0e67d13c57840042b1397d36d3c1918e50344eb405025d`  
		Last Modified: Tue, 01 Mar 2022 03:49:43 GMT  
		Size: 323.7 KB (323703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e632b2b5bf88ea94d56d701fa93b55516003db1fc7c855bb4569f2be0ddf3be`  
		Last Modified: Tue, 01 Mar 2022 03:49:43 GMT  
		Size: 1.3 MB (1251083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1fc0f9b2a7499de336af3103d86d1ffc3b90b62ea850295c0c57abbe68c753b`  
		Last Modified: Tue, 01 Mar 2022 03:49:43 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe1ee7b4dd056bb3eadc09b9893ce88a096e51500bbe841d1c145be10ba2b1f0`  
		Last Modified: Tue, 01 Mar 2022 03:49:43 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:bullseye` - linux; ppc64le

```console
$ docker pull memcached@sha256:4893f4daa742b31f414b08f98f8e7d0cbedaf63b8d88062bcf3c91a9522a2aab
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.0 MB (36957544 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8db953cc998ed06712eca57fe4ae2b8bb342ce991683fd7592495a21557d0940`
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
# Fri, 11 Feb 2022 23:47:36 GMT
ENV MEMCACHED_VERSION=1.6.14
# Fri, 11 Feb 2022 23:47:38 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Fri, 11 Feb 2022 23:53:07 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Fri, 11 Feb 2022 23:53:13 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 11 Feb 2022 23:53:34 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 11 Feb 2022 23:53:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Feb 2022 23:53:39 GMT
USER memcache
# Fri, 11 Feb 2022 23:53:41 GMT
EXPOSE 11211
# Fri, 11 Feb 2022 23:53:46 GMT
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
	-	`sha256:d5f2e5d5bb1609e336a37e97218d618550ec5ce28384c32b1141393ef6f04a03`  
		Last Modified: Fri, 11 Feb 2022 23:58:44 GMT  
		Size: 1.3 MB (1322220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76e6da4f290b1cff2fa5b1ad17d42333c67179332511db4da3bd2c5ce12bbdfa`  
		Last Modified: Fri, 11 Feb 2022 23:58:44 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fb140c5468aa121999bc169d30e4ce6b73795cdf67aa21c1dfd3d1194dd0b82`  
		Last Modified: Fri, 11 Feb 2022 23:58:44 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:bullseye` - linux; s390x

```console
$ docker pull memcached@sha256:14b3ae46a3b5dc4d1ca410da43e53ee0c44ad49ec398f235628f89bc8cc0a0cc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.2 MB (31217166 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:50f1b3aef9bc393e3b1a3fab35c702d6a9b9dd6fa2abd9d044b52385b9ccf549`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 01 Mar 2022 02:01:56 GMT
ADD file:d869ad3392a4e752c2f73d08a4cc13594c94bfc050bd037db0ca9827a0207072 in / 
# Tue, 01 Mar 2022 02:01:58 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 13:28:37 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 01 Mar 2022 13:28:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 13:28:40 GMT
ENV MEMCACHED_VERSION=1.6.14
# Tue, 01 Mar 2022 13:28:40 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Tue, 01 Mar 2022 13:31:58 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 01 Mar 2022 13:31:58 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 01 Mar 2022 13:31:58 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 01 Mar 2022 13:31:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 01 Mar 2022 13:31:59 GMT
USER memcache
# Tue, 01 Mar 2022 13:31:59 GMT
EXPOSE 11211
# Tue, 01 Mar 2022 13:31:59 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:f81abce72636770dac4258df46a31beeb6ad81dfddd5b7c9c3fa6942ea074922`  
		Last Modified: Tue, 01 Mar 2022 02:07:33 GMT  
		Size: 29.6 MB (29647132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b43f274641c42412c1e075acb3920020215603d1e1c938fa84211ea8b005988`  
		Last Modified: Tue, 01 Mar 2022 13:32:52 GMT  
		Size: 5.0 KB (5024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d135f121f1aff6ea16284d2286318c703c72dad45560bdc68ac2bc2371f8164`  
		Last Modified: Tue, 01 Mar 2022 13:32:52 GMT  
		Size: 324.1 KB (324102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9255401f181741c77541d42f93796b72c20077b2815b9e6c4e21b36f9bcccab6`  
		Last Modified: Tue, 01 Mar 2022 13:32:52 GMT  
		Size: 1.2 MB (1240500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5436de37a983faa64cc9d82c3a8272ae77b107e2f8bcd453f7aee5e3e92def7`  
		Last Modified: Tue, 01 Mar 2022 13:32:52 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8296feb21176186e1c4027cf5e8111ed103c7b2b30f1f4423a9303a0e7fd9d3`  
		Last Modified: Tue, 01 Mar 2022 13:32:52 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:latest`

```console
$ docker pull memcached@sha256:e4bb2d212309e51166f29fe5404edf5caf784ada9ab3fde8dcf8226f337878aa
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
$ docker pull memcached@sha256:2c29149daad601e046074c6801fb570180d4eba60047135b71f51ea327ffcbc1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.0 MB (32954984 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6208dafa350f4dfbb3f2a16e20c2f2d256f894fd8695ac24b21663a732dee124`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 01 Mar 2022 02:13:29 GMT
ADD file:d48a85028743f16ed927507322e3e3beee187fbfadd0b781d4b89de197c64b5b in / 
# Tue, 01 Mar 2022 02:13:29 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 13:24:57 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 01 Mar 2022 13:25:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 13:25:02 GMT
ENV MEMCACHED_VERSION=1.6.14
# Tue, 01 Mar 2022 13:25:02 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Tue, 01 Mar 2022 13:28:58 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 01 Mar 2022 13:28:58 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 01 Mar 2022 13:28:59 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 01 Mar 2022 13:28:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 01 Mar 2022 13:29:00 GMT
USER memcache
# Tue, 01 Mar 2022 13:29:00 GMT
EXPOSE 11211
# Tue, 01 Mar 2022 13:29:00 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:f7a1c6dad28192bd417b78079d6ddc03cbca6d5ea46bba12769b235b6353c00c`  
		Last Modified: Tue, 01 Mar 2022 02:19:23 GMT  
		Size: 31.4 MB (31366396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3292b9ed039a5211ec564a1f170046ba2ad296a19beb778d3c7106a230301d27`  
		Last Modified: Tue, 01 Mar 2022 13:29:33 GMT  
		Size: 5.0 KB (4980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15c683705067bdb5151c087a9b5e91a37f498912588e29970e3ce07121334f03`  
		Last Modified: Tue, 01 Mar 2022 13:29:34 GMT  
		Size: 328.0 KB (328033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:091c46e57219c5fdd0a044c77fc12a24889bd1ce95e4d032e83f2ea09997ca1d`  
		Last Modified: Tue, 01 Mar 2022 13:29:34 GMT  
		Size: 1.3 MB (1255168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a26e7e13ba905fd75a5e3b2307ab4abee1bbcdc9b586d37fc2ff7984de1c92c3`  
		Last Modified: Tue, 01 Mar 2022 13:29:33 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75b625708cf5e763937f326c6fe55adcb4c4782926483ea2a3628012927922c7`  
		Last Modified: Tue, 01 Mar 2022 13:29:33 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:latest` - linux; arm variant v5

```console
$ docker pull memcached@sha256:839b663c2a5637a5a026d8bf63f2c3a5af62938b6becb246fe84e68bceb73742
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.5 MB (30457903 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:46c3d2c41f175e70fa19ec073355fc3376f15b3ca99f6fdb295b6cea57aede38`
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
# Fri, 11 Feb 2022 23:48:33 GMT
ENV MEMCACHED_VERSION=1.6.14
# Fri, 11 Feb 2022 23:48:33 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Fri, 11 Feb 2022 23:53:18 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Fri, 11 Feb 2022 23:53:19 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 11 Feb 2022 23:53:20 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 11 Feb 2022 23:53:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Feb 2022 23:53:21 GMT
USER memcache
# Fri, 11 Feb 2022 23:53:22 GMT
EXPOSE 11211
# Fri, 11 Feb 2022 23:53:22 GMT
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
	-	`sha256:4c595fdbb4287a9ef2b3565e1d9ac2caa7d17ac0810224d8a5d3c87313cc81b5`  
		Last Modified: Fri, 11 Feb 2022 23:54:16 GMT  
		Size: 1.2 MB (1226376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19c8ecb542750e6e603057b1e7bdb90fc58d45b604f20b2724d402a572f1b735`  
		Last Modified: Fri, 11 Feb 2022 23:54:15 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64d2e913eaab741b412c8fec5edbad97daed3a2c5f0a1a1fd376ea8ec7c28c52`  
		Last Modified: Fri, 11 Feb 2022 23:54:15 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:latest` - linux; arm variant v7

```console
$ docker pull memcached@sha256:c1ded327e0d4c11f7f00652600f4cbf465a119fed31e6e2541d516700e0e14c2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.1 MB (28080208 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:866cf84302a62bedfada61f236deccacb7585dc0ccce8a4e0e058b741bfafdc5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 01 Mar 2022 02:02:56 GMT
ADD file:c6b519323fd1fa09b9f8c8608778872e8fa6208cb0b42aaccdef4479a469f5f4 in / 
# Tue, 01 Mar 2022 02:02:57 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 14:02:17 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 01 Mar 2022 14:02:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 14:02:26 GMT
ENV MEMCACHED_VERSION=1.6.14
# Tue, 01 Mar 2022 14:02:26 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Tue, 01 Mar 2022 14:06:15 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 01 Mar 2022 14:06:16 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 01 Mar 2022 14:06:17 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 01 Mar 2022 14:06:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 01 Mar 2022 14:06:18 GMT
USER memcache
# Tue, 01 Mar 2022 14:06:19 GMT
EXPOSE 11211
# Tue, 01 Mar 2022 14:06:19 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:59dbb2ac3829352dd707e28e037734c9fbdef5b03aea31e3929ddcead949afee`  
		Last Modified: Tue, 01 Mar 2022 02:19:09 GMT  
		Size: 26.6 MB (26565105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45ff8679190bbfe567a01e354c79eb44efaa4564b0770a644b9eb6a28f10812c`  
		Last Modified: Tue, 01 Mar 2022 14:19:16 GMT  
		Size: 4.9 KB (4894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13db11031aa185885b3b1b9c74eba0d8ea9b07d5e8fec5870bc7df8d09585d2f`  
		Last Modified: Tue, 01 Mar 2022 14:19:16 GMT  
		Size: 312.0 KB (312009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:079efee4f8d1e8cea53f0cc6ddc4832de31e69c43411b81e790e0615eeea16aa`  
		Last Modified: Tue, 01 Mar 2022 14:19:16 GMT  
		Size: 1.2 MB (1197793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:050fbe09656330899bb983ba6d0871a6cc96349c4c049673a4ee53816db5ff7b`  
		Last Modified: Tue, 01 Mar 2022 14:19:16 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcca636453f4acf7b597c080e2d7c57ea366f36daae56acdd43664bb28dff985`  
		Last Modified: Tue, 01 Mar 2022 14:19:16 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:latest` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:c59ae38d83ce474dc14423325e3f500a06e285938b4f4e8a013ae8967603d492
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.4 MB (31435417 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b5c5ad61ebd09fab08b612599fdf9e96be59696045e4765dac554781daef4d1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 01 Mar 2022 02:11:29 GMT
ADD file:9816c9c29627693c34afda4fa5e1a5e8a0f5aa3c5d5cfd920a4d89c77aab997d in / 
# Tue, 01 Mar 2022 02:11:30 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 12:44:12 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 01 Mar 2022 12:44:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 12:44:16 GMT
ENV MEMCACHED_VERSION=1.6.14
# Tue, 01 Mar 2022 12:44:17 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Tue, 01 Mar 2022 12:46:49 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 01 Mar 2022 12:46:50 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 01 Mar 2022 12:46:50 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 01 Mar 2022 12:46:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 01 Mar 2022 12:46:52 GMT
USER memcache
# Tue, 01 Mar 2022 12:46:53 GMT
EXPOSE 11211
# Tue, 01 Mar 2022 12:46:54 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:279a020076a7fbddfc996e4c55e605a8f322810c3eca21cdedbcb06beb0e1305`  
		Last Modified: Tue, 01 Mar 2022 02:18:24 GMT  
		Size: 30.1 MB (30057008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7dfd1ea3d9e177e785365db9a22591801c15e6a33097ba79a048e3387f4c43a`  
		Last Modified: Tue, 01 Mar 2022 12:47:45 GMT  
		Size: 4.9 KB (4902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e563a531f0653c96d3786deff2afe7190769b5929d06c8c234d89fd314bf2396`  
		Last Modified: Tue, 01 Mar 2022 12:47:45 GMT  
		Size: 119.2 KB (119172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1d1b1b990f1e4e95a5410acd589565956a1fd54c4df3b71a665dcfb23ac9f76`  
		Last Modified: Tue, 01 Mar 2022 12:47:46 GMT  
		Size: 1.3 MB (1253928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b8a7c0be94d102b9a04c359186fcf59b223183acc8b489d0ca12afb8f073027`  
		Last Modified: Tue, 01 Mar 2022 12:47:45 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:091c7ee2fb4e34177c30b2b9905bf098f304bea040ff7ca5700134d4921c2758`  
		Last Modified: Tue, 01 Mar 2022 12:47:45 GMT  
		Size: 120.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:latest` - linux; 386

```console
$ docker pull memcached@sha256:4c9eb4902e2601bad18a1783dbf7d64cf25f6121226d4772a5d36a7ac3e9db79
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.0 MB (33972554 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af09c75e25cf0ea60c4f155a25728e256411f07898946ea08e869eb6362e3a24`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 01 Mar 2022 02:07:32 GMT
ADD file:e92ab504d4c0d3bd63da83254e6ca400b607c32e0f5037039648559b91770870 in / 
# Tue, 01 Mar 2022 02:07:33 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 10:07:23 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 01 Mar 2022 10:07:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 10:07:30 GMT
ENV MEMCACHED_VERSION=1.6.14
# Tue, 01 Mar 2022 10:07:30 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Tue, 01 Mar 2022 10:11:57 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 01 Mar 2022 10:11:57 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 01 Mar 2022 10:11:58 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 01 Mar 2022 10:11:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 01 Mar 2022 10:11:58 GMT
USER memcache
# Tue, 01 Mar 2022 10:11:58 GMT
EXPOSE 11211
# Tue, 01 Mar 2022 10:11:59 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:04a87e821be7e4b29d48011b7aa4ff884ca57fd36995cb3b99fd2fc24ac562d8`  
		Last Modified: Tue, 01 Mar 2022 02:15:51 GMT  
		Size: 32.4 MB (32377389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe860ecc70fbef589f9779541d957321138c3f41d99742ca7ff2bb41b6787786`  
		Last Modified: Tue, 01 Mar 2022 10:13:02 GMT  
		Size: 4.9 KB (4889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71fbbf846282a29c58595e09b8a5d93a6348fc5a77d0bb513263f933972610e8`  
		Last Modified: Tue, 01 Mar 2022 10:13:03 GMT  
		Size: 336.6 KB (336603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f93f31af2adb455df5e2c7baaa190b479d463d37657734ee855d663709906a2`  
		Last Modified: Tue, 01 Mar 2022 10:13:03 GMT  
		Size: 1.3 MB (1253268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ea06973bd5c70feb976fde3006e5400760f293973d5a2a8f8a05a73105a5851`  
		Last Modified: Tue, 01 Mar 2022 10:13:02 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c85296c039a2ca9f99139e04d26550a26b109424a80e9377a115129110257b9`  
		Last Modified: Tue, 01 Mar 2022 10:13:02 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:latest` - linux; mips64le

```console
$ docker pull memcached@sha256:76269e61918b56719946fa47ffaebf468965e45dae401738fcd6d8ea6d9afdc1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.2 MB (31213138 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bdf2a1611553c4acfb426a9736777620af35250c1c3fde4997dd8fda25547725`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 01 Mar 2022 02:02:49 GMT
ADD file:1901e1e1292cbfcd557262ec5d08551cecd0070b24928414d220472664fe3fdf in / 
# Tue, 01 Mar 2022 02:02:49 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 03:43:18 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 01 Mar 2022 03:43:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 03:43:30 GMT
ENV MEMCACHED_VERSION=1.6.14
# Tue, 01 Mar 2022 03:43:30 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Tue, 01 Mar 2022 03:49:17 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 01 Mar 2022 03:49:17 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 01 Mar 2022 03:49:19 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 01 Mar 2022 03:49:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 01 Mar 2022 03:49:20 GMT
USER memcache
# Tue, 01 Mar 2022 03:49:20 GMT
EXPOSE 11211
# Tue, 01 Mar 2022 03:49:20 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:3baeb8c34a522fc616f97412d47dc1f665e93552c57aa8237ee1d673f9757cba`  
		Last Modified: Tue, 01 Mar 2022 02:12:25 GMT  
		Size: 29.6 MB (29632966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50a63f21594c0da6641452e9cd0caaf8727bae4ca86c617384198ab5d8e766ec`  
		Last Modified: Tue, 01 Mar 2022 03:49:43 GMT  
		Size: 5.0 KB (4979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dfb3a0cb8d59939fa0e67d13c57840042b1397d36d3c1918e50344eb405025d`  
		Last Modified: Tue, 01 Mar 2022 03:49:43 GMT  
		Size: 323.7 KB (323703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e632b2b5bf88ea94d56d701fa93b55516003db1fc7c855bb4569f2be0ddf3be`  
		Last Modified: Tue, 01 Mar 2022 03:49:43 GMT  
		Size: 1.3 MB (1251083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1fc0f9b2a7499de336af3103d86d1ffc3b90b62ea850295c0c57abbe68c753b`  
		Last Modified: Tue, 01 Mar 2022 03:49:43 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe1ee7b4dd056bb3eadc09b9893ce88a096e51500bbe841d1c145be10ba2b1f0`  
		Last Modified: Tue, 01 Mar 2022 03:49:43 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:latest` - linux; ppc64le

```console
$ docker pull memcached@sha256:4893f4daa742b31f414b08f98f8e7d0cbedaf63b8d88062bcf3c91a9522a2aab
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.0 MB (36957544 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8db953cc998ed06712eca57fe4ae2b8bb342ce991683fd7592495a21557d0940`
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
# Fri, 11 Feb 2022 23:47:36 GMT
ENV MEMCACHED_VERSION=1.6.14
# Fri, 11 Feb 2022 23:47:38 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Fri, 11 Feb 2022 23:53:07 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Fri, 11 Feb 2022 23:53:13 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 11 Feb 2022 23:53:34 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 11 Feb 2022 23:53:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Feb 2022 23:53:39 GMT
USER memcache
# Fri, 11 Feb 2022 23:53:41 GMT
EXPOSE 11211
# Fri, 11 Feb 2022 23:53:46 GMT
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
	-	`sha256:d5f2e5d5bb1609e336a37e97218d618550ec5ce28384c32b1141393ef6f04a03`  
		Last Modified: Fri, 11 Feb 2022 23:58:44 GMT  
		Size: 1.3 MB (1322220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76e6da4f290b1cff2fa5b1ad17d42333c67179332511db4da3bd2c5ce12bbdfa`  
		Last Modified: Fri, 11 Feb 2022 23:58:44 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fb140c5468aa121999bc169d30e4ce6b73795cdf67aa21c1dfd3d1194dd0b82`  
		Last Modified: Fri, 11 Feb 2022 23:58:44 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:latest` - linux; s390x

```console
$ docker pull memcached@sha256:14b3ae46a3b5dc4d1ca410da43e53ee0c44ad49ec398f235628f89bc8cc0a0cc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.2 MB (31217166 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:50f1b3aef9bc393e3b1a3fab35c702d6a9b9dd6fa2abd9d044b52385b9ccf549`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 01 Mar 2022 02:01:56 GMT
ADD file:d869ad3392a4e752c2f73d08a4cc13594c94bfc050bd037db0ca9827a0207072 in / 
# Tue, 01 Mar 2022 02:01:58 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 13:28:37 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 01 Mar 2022 13:28:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 13:28:40 GMT
ENV MEMCACHED_VERSION=1.6.14
# Tue, 01 Mar 2022 13:28:40 GMT
ENV MEMCACHED_SHA1=be64c11d34f04bd1855100b8b5ad9ae8b45e0ab0
# Tue, 01 Mar 2022 13:31:58 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 01 Mar 2022 13:31:58 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 01 Mar 2022 13:31:58 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 01 Mar 2022 13:31:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 01 Mar 2022 13:31:59 GMT
USER memcache
# Tue, 01 Mar 2022 13:31:59 GMT
EXPOSE 11211
# Tue, 01 Mar 2022 13:31:59 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:f81abce72636770dac4258df46a31beeb6ad81dfddd5b7c9c3fa6942ea074922`  
		Last Modified: Tue, 01 Mar 2022 02:07:33 GMT  
		Size: 29.6 MB (29647132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b43f274641c42412c1e075acb3920020215603d1e1c938fa84211ea8b005988`  
		Last Modified: Tue, 01 Mar 2022 13:32:52 GMT  
		Size: 5.0 KB (5024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d135f121f1aff6ea16284d2286318c703c72dad45560bdc68ac2bc2371f8164`  
		Last Modified: Tue, 01 Mar 2022 13:32:52 GMT  
		Size: 324.1 KB (324102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9255401f181741c77541d42f93796b72c20077b2815b9e6c4e21b36f9bcccab6`  
		Last Modified: Tue, 01 Mar 2022 13:32:52 GMT  
		Size: 1.2 MB (1240500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5436de37a983faa64cc9d82c3a8272ae77b107e2f8bcd453f7aee5e3e92def7`  
		Last Modified: Tue, 01 Mar 2022 13:32:52 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8296feb21176186e1c4027cf5e8111ed103c7b2b30f1f4423a9303a0e7fd9d3`  
		Last Modified: Tue, 01 Mar 2022 13:32:52 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
