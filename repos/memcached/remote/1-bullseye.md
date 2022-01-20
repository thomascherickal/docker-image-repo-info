## `memcached:1-bullseye`

```console
$ docker pull memcached@sha256:9aa65bd26ecf559025ebd45e2f4c2ead175ea13b5e592c5111ac3aadc41934c1
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
$ docker pull memcached@sha256:e2dd7976ed6edbc881ebd6de310bd00b2764b9b7a21d743842e883d02cacc7e2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.1 MB (28074595 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7402f04880743431826d95de0a6a4e8207149078770b0cdf8da0fbbd351673b8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 21 Dec 2021 01:59:48 GMT
ADD file:6a5555c3e40db91fae5bb112464a4c405a976de17ff64c98f25d3033a6a608d8 in / 
# Tue, 21 Dec 2021 01:59:48 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 07:31:47 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 21 Dec 2021 07:31:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 20 Jan 2022 01:07:49 GMT
ENV MEMCACHED_VERSION=1.6.13
# Thu, 20 Jan 2022 01:07:49 GMT
ENV MEMCACHED_SHA1=b9da57ba63ba8de8a980fe0fe2fedc8d59e1dfe3
# Thu, 20 Jan 2022 01:12:13 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 20 Jan 2022 01:12:14 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 20 Jan 2022 01:12:15 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 20 Jan 2022 01:12:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 20 Jan 2022 01:12:16 GMT
USER memcache
# Thu, 20 Jan 2022 01:12:17 GMT
EXPOSE 11211
# Thu, 20 Jan 2022 01:12:17 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:d0061d6703dc4975804c3419e00c85efbe3f1b79c86d87e048fa14a683e88e31`  
		Last Modified: Tue, 21 Dec 2021 02:15:26 GMT  
		Size: 26.6 MB (26560815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6b7e1b0583a78d22dbd2c5732cb188f178724c8c9c11c260ff372f47420f98d`  
		Last Modified: Tue, 21 Dec 2021 07:49:12 GMT  
		Size: 4.9 KB (4896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5a011a0f1099a4b8d3fe15ce9936137a1db8c4e8171f9ab6f141cb6abd24fd7`  
		Last Modified: Tue, 21 Dec 2021 07:49:13 GMT  
		Size: 312.0 KB (312006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edc5c94228d4df658e1b34bf983386a4d376d30e0f514a060c7435fd949d5473`  
		Last Modified: Thu, 20 Jan 2022 01:25:59 GMT  
		Size: 1.2 MB (1196470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0c4e1681bfee0c9662177878b964f3562510410cf0045d1be5dbb651c8ceca6`  
		Last Modified: Thu, 20 Jan 2022 01:25:58 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc8e4e9859bb885ba04671cde7c8793ef29da1f6685de7a1e0a634296e4ef112`  
		Last Modified: Thu, 20 Jan 2022 01:25:58 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-bullseye` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:1b24c0a5f4143bd534d4cf29fd88d648e7a96d8c7b8f2626d198aa7352d739b2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.4 MB (31421990 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a8b1a75a9c94601798efa678f741a30113a489169fd0d0036687730bb012d40d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 21 Dec 2021 01:42:23 GMT
ADD file:986f91febed4aa8e2072081ff8419d52ba2060510822e717086d3b3d9469e4d7 in / 
# Tue, 21 Dec 2021 01:42:24 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 02:41:54 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 21 Dec 2021 02:41:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 20 Jan 2022 02:11:00 GMT
ENV MEMCACHED_VERSION=1.6.13
# Thu, 20 Jan 2022 02:11:00 GMT
ENV MEMCACHED_SHA1=b9da57ba63ba8de8a980fe0fe2fedc8d59e1dfe3
# Thu, 20 Jan 2022 02:13:44 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 20 Jan 2022 02:13:45 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 20 Jan 2022 02:13:45 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 20 Jan 2022 02:13:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 20 Jan 2022 02:13:47 GMT
USER memcache
# Thu, 20 Jan 2022 02:13:48 GMT
EXPOSE 11211
# Thu, 20 Jan 2022 02:13:49 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:927a35006d93ea08499b57046904046d7926cd76fb17be193e3e74f56d634a08`  
		Last Modified: Tue, 21 Dec 2021 01:48:54 GMT  
		Size: 30.0 MB (30043793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e0d416ba392877fa24343ce6a6095813283199d22f957608eb5f21ca8160b31`  
		Last Modified: Tue, 21 Dec 2021 02:45:27 GMT  
		Size: 4.9 KB (4904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b4cd3f3e45eff1ee912f3bc7dd16f38c07d488a99910c9c11922cad72b814ae`  
		Last Modified: Tue, 21 Dec 2021 02:45:28 GMT  
		Size: 119.2 KB (119209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1997323c7e6de3b1bf321d50e73e483991128230238469cf59e3f63569b451c`  
		Last Modified: Thu, 20 Jan 2022 02:17:41 GMT  
		Size: 1.3 MB (1253677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f59d6c4411a30e9612b02bf1bb1b192d528cb63361e0eac0fe3afbb84a4d351`  
		Last Modified: Thu, 20 Jan 2022 02:17:40 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fb04af4b7e0bfe9388fd64ac7716fbe8826f8556549acbdab8242f241bbb2ab`  
		Last Modified: Thu, 20 Jan 2022 02:17:41 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-bullseye` - linux; 386

```console
$ docker pull memcached@sha256:49e6442a8399d3043e7d046ed333fe89bdb26c7ff76328cdcb0c66d3602b2a49
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.0 MB (33965012 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:020a47b3c16dac7693da9e60d46ac56df23d075bbf9710b4207011490682b0f3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 21 Dec 2021 01:40:06 GMT
ADD file:6b67a0d4d176747cc8cefbd105facde82f1795467bf02eb45e8385c91cdc9c41 in / 
# Tue, 21 Dec 2021 01:40:09 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 07:51:54 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 21 Dec 2021 07:52:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 19 Jan 2022 23:48:26 GMT
ENV MEMCACHED_VERSION=1.6.13
# Wed, 19 Jan 2022 23:48:27 GMT
ENV MEMCACHED_SHA1=b9da57ba63ba8de8a980fe0fe2fedc8d59e1dfe3
# Wed, 19 Jan 2022 23:52:44 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 19 Jan 2022 23:52:44 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 19 Jan 2022 23:52:45 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 19 Jan 2022 23:52:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 19 Jan 2022 23:52:45 GMT
USER memcache
# Wed, 19 Jan 2022 23:52:46 GMT
EXPOSE 11211
# Wed, 19 Jan 2022 23:52:46 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:9b9a100d632569e96aeb2d7b0bc45bc436609bb61335815f207994f3b557f0f7`  
		Last Modified: Tue, 21 Dec 2021 01:48:45 GMT  
		Size: 32.4 MB (32370850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa8ed5a0897a80c3dd4f666ad1ce77fc69f815010aabe14ed263e3a2844f23de`  
		Last Modified: Tue, 21 Dec 2021 07:57:46 GMT  
		Size: 4.9 KB (4893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bfa0cba205c2a7200c7c876508a043cee5924603cc514cc028a149516f2d281`  
		Last Modified: Tue, 21 Dec 2021 07:57:47 GMT  
		Size: 336.6 KB (336602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fab69132096896cd9cb316ae471647d759a28f3beef7060defeb4dd11cc9633b`  
		Last Modified: Wed, 19 Jan 2022 23:58:13 GMT  
		Size: 1.3 MB (1252259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:363bda59d05c4b0f652f7718e1bb8d47a6e23f9ce2a95ce9c35b8aeb9b5a28e1`  
		Last Modified: Wed, 19 Jan 2022 23:58:13 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d82fe4a5f058291d0d32d79de80c39328493be293ae7f7e6f2d12e1dfa169933`  
		Last Modified: Wed, 19 Jan 2022 23:58:13 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-bullseye` - linux; mips64le

```console
$ docker pull memcached@sha256:4d946a5c9f6153b4d75d3ecb5c2261603a11c71c37d896fb394ea78960db05e3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.2 MB (31198599 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f80ef92e5cf7dec082a743e3f3d23419482a151d15d2569cdafcda4561954818`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 21 Dec 2021 02:09:07 GMT
ADD file:9e5931d5ed32a23b2e93bd8846258c647613637c581b6813bbc7d7e6b86bbdf5 in / 
# Tue, 21 Dec 2021 02:09:08 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 03:55:53 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 21 Dec 2021 03:56:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 20 Jan 2022 00:07:28 GMT
ENV MEMCACHED_VERSION=1.6.13
# Thu, 20 Jan 2022 00:07:28 GMT
ENV MEMCACHED_SHA1=b9da57ba63ba8de8a980fe0fe2fedc8d59e1dfe3
# Thu, 20 Jan 2022 00:13:23 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 20 Jan 2022 00:13:23 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 20 Jan 2022 00:13:25 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 20 Jan 2022 00:13:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 20 Jan 2022 00:13:26 GMT
USER memcache
# Thu, 20 Jan 2022 00:13:26 GMT
EXPOSE 11211
# Thu, 20 Jan 2022 00:13:27 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:6a6edb95e2485a5b9b3c44b27b7ebad16384c0e08a3d61b7e48c65d7278763cf`  
		Last Modified: Tue, 21 Dec 2021 02:18:14 GMT  
		Size: 29.6 MB (29619177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d8863ea22b340cf477721beae8012cdec62392ebe36462562fe97e70339bff3`  
		Last Modified: Tue, 21 Dec 2021 04:02:33 GMT  
		Size: 5.0 KB (4980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37db9004b7abf8bc313b4a2d45e2e98a4b8a4b626793b7236586e794c79847b2`  
		Last Modified: Tue, 21 Dec 2021 04:02:33 GMT  
		Size: 323.7 KB (323702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a433e70cfd23c4ef6dafa88705e6d3174b22de82a72af00a5bce9420fe3cf15`  
		Last Modified: Thu, 20 Jan 2022 00:13:54 GMT  
		Size: 1.3 MB (1250332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01906d69dc0ad3039718b238cdeedc15b6f158350619520ca09ad92288def773`  
		Last Modified: Thu, 20 Jan 2022 00:13:54 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddd9829736e478885942d88a42cda9807c98c0878bb7cbad662f9d3038604c02`  
		Last Modified: Thu, 20 Jan 2022 00:13:53 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-bullseye` - linux; ppc64le

```console
$ docker pull memcached@sha256:96bb749f6954eea636ae16caec16a3aeeb64cd167418a98d348045cb459f2f5f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.9 MB (36942882 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7c3861724290167adde7d4a56ecd63a01b18e1d999b084f450ab114e4bf70408`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 21 Dec 2021 02:20:24 GMT
ADD file:078a17bf7e519cb7a60fbbf743ba7e5897554201cb44957154ab518d6991a033 in / 
# Tue, 21 Dec 2021 02:20:28 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 05:09:20 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 21 Dec 2021 05:09:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 20 Jan 2022 01:06:59 GMT
ENV MEMCACHED_VERSION=1.6.13
# Thu, 20 Jan 2022 01:07:03 GMT
ENV MEMCACHED_SHA1=b9da57ba63ba8de8a980fe0fe2fedc8d59e1dfe3
# Thu, 20 Jan 2022 01:12:11 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 20 Jan 2022 01:12:13 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 20 Jan 2022 01:12:19 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 20 Jan 2022 01:12:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 20 Jan 2022 01:12:30 GMT
USER memcache
# Thu, 20 Jan 2022 01:12:36 GMT
EXPOSE 11211
# Thu, 20 Jan 2022 01:12:39 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:3345479fea0cdce1382b927b0908af4f239b288b30efa203c50edf7ac0cb055e`  
		Last Modified: Tue, 21 Dec 2021 02:29:20 GMT  
		Size: 35.3 MB (35258992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:260a46cf3dd0567a7e3bb225544bcee947dcfd1ae543a7fc3f5554a4750ea821`  
		Last Modified: Tue, 21 Dec 2021 05:17:58 GMT  
		Size: 5.0 KB (4986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1840d2c3d22c5b30c6d81f686f94908b0f23b14cb10519053b3434a78125677e`  
		Last Modified: Tue, 21 Dec 2021 05:17:59 GMT  
		Size: 356.9 KB (356895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98049dbc7e31ea6eb15e11aaf7ce0d1300ce8192b9b9480680e7b4921bf000a1`  
		Last Modified: Thu, 20 Jan 2022 01:17:57 GMT  
		Size: 1.3 MB (1321601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea621b2de9dcc7e2760960260bbd3056119c41b506097f79d16139e9a59e7d5d`  
		Last Modified: Thu, 20 Jan 2022 01:17:56 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:072156166234b50f53675c2559174b90ee6b330403f28fcd3e11747138f62dda`  
		Last Modified: Thu, 20 Jan 2022 01:17:56 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-bullseye` - linux; s390x

```console
$ docker pull memcached@sha256:ac5a3ef461209de009ec2cfd936762e374ca6394398c82df477c0f182f48387f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.2 MB (31211231 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ff3ea88647820a1eca0b3e9c3ceb53d59512de495a751eecc48414ba7bd3ea55`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 21 Dec 2021 01:42:27 GMT
ADD file:c8a482d41bf09dfb6484bf2a6e38535bf0594d26dd6eedd5abde4e3cc811fa6c in / 
# Tue, 21 Dec 2021 01:42:29 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 03:12:14 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 21 Dec 2021 03:12:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 20 Jan 2022 00:14:30 GMT
ENV MEMCACHED_VERSION=1.6.13
# Thu, 20 Jan 2022 00:14:30 GMT
ENV MEMCACHED_SHA1=b9da57ba63ba8de8a980fe0fe2fedc8d59e1dfe3
# Thu, 20 Jan 2022 00:21:52 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 20 Jan 2022 00:21:52 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 20 Jan 2022 00:21:52 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 20 Jan 2022 00:21:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 20 Jan 2022 00:21:53 GMT
USER memcache
# Thu, 20 Jan 2022 00:21:53 GMT
EXPOSE 11211
# Thu, 20 Jan 2022 00:21:53 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:12562551722a758d23ceea9abcdc2bee737e38c8f62a0f3d3afb2cc2626c28b1`  
		Last Modified: Tue, 21 Dec 2021 01:48:15 GMT  
		Size: 29.6 MB (29641636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:849c9b856e86bed85b14eff1a55b4a7f44de4539562e985fc69474140aaab326`  
		Last Modified: Tue, 21 Dec 2021 03:16:46 GMT  
		Size: 5.0 KB (5027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33bfb5bdc76b73fe600374c1510bbcb81e22bd430db8461477baf6d27de2854d`  
		Last Modified: Tue, 21 Dec 2021 03:16:46 GMT  
		Size: 324.1 KB (324102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0cf9c05999fd14a43d159660389e5c87951f0abdba08eac304ee7cd74908594`  
		Last Modified: Thu, 20 Jan 2022 00:26:38 GMT  
		Size: 1.2 MB (1240059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1664702a0638d67025039678f679ac38923f93f78a146e9d4e71a76ccbe2d7a`  
		Last Modified: Thu, 20 Jan 2022 00:26:39 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cab6aa21541e1c3ba636b8a2d51298a3c523d5f2c37ca723fba92a9452cd36ab`  
		Last Modified: Thu, 20 Jan 2022 00:26:39 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
