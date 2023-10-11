## `redis:7-bookworm`

```console
$ docker pull redis@sha256:55f70c57c74b25d00c38ff60726da1caee17202774af2de365c36628d9b3c7e1
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 16
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm variant v5
	-	unknown; unknown
	-	linux; arm variant v7
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

### `redis:7-bookworm` - linux; amd64

```console
$ docker pull redis@sha256:28aa338c21f38494f6ce55dd3dba3b96f00f7da4a84f273c801a685dbfd66d94
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.4 MB (51427190 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5b0542ad1e7734b17905e99f80defc1f0a7748dd6d6f1648949eb45583d087de`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Wed, 06 Sep 2023 21:03:16 GMT
ADD file:55ad846fa191e603f48090eae0e4a7149c4066b94406593ec1898ad2c3347937 in / 
# Wed, 06 Sep 2023 21:03:16 GMT
CMD ["bash"]
# Wed, 06 Sep 2023 21:03:16 GMT
RUN groupadd -r -g 999 redis && useradd -r -g redis -u 999 redis # buildkit
# Wed, 06 Sep 2023 21:03:16 GMT
ENV GOSU_VERSION=1.16
# Wed, 06 Sep 2023 21:03:16 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Wed, 06 Sep 2023 21:03:16 GMT
ENV REDIS_VERSION=7.2.1
# Wed, 06 Sep 2023 21:03:16 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-7.2.1.tar.gz
# Wed, 06 Sep 2023 21:03:16 GMT
ENV REDIS_DOWNLOAD_SHA=5c76d990a1b1c5f949bcd1eed90d0c8a4f70369bdbdcb40288c561ddf88967a4
# Wed, 06 Sep 2023 21:03:16 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				dpkg-dev 		gcc 		libc6-dev 		libssl-dev 		make 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		redis-cli --version; 	redis-server --version # buildkit
# Wed, 06 Sep 2023 21:03:16 GMT
RUN mkdir /data && chown redis:redis /data # buildkit
# Wed, 06 Sep 2023 21:03:16 GMT
VOLUME [/data]
# Wed, 06 Sep 2023 21:03:16 GMT
WORKDIR /data
# Wed, 06 Sep 2023 21:03:16 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Wed, 06 Sep 2023 21:03:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 06 Sep 2023 21:03:16 GMT
EXPOSE map[6379/tcp:{}]
# Wed, 06 Sep 2023 21:03:16 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:a378f10b321842c3042cdeff4f6997f34f4cb21f2eff27704b7f6193ab7b5fea`  
		Last Modified: Wed, 11 Oct 2023 18:39:34 GMT  
		Size: 29.1 MB (29149874 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3c75410c1f8b4830146d79153b677a7ad05acc0d806394ade9bc99b74b8d2f5c`  
		Last Modified: Wed, 11 Oct 2023 19:01:31 GMT  
		Size: 1.1 KB (1101 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:667874757cc14509db1ff8dc204c80802123cbaa8b40c4a85bc5ba5f63b3161c`  
		Last Modified: Wed, 11 Oct 2023 19:01:31 GMT  
		Size: 1.4 MB (1439899 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7150b93d249d2e2452a04f3e6cdc5d360407f6e4865fdd7f8ee65da99f945fb8`  
		Last Modified: Wed, 11 Oct 2023 19:01:34 GMT  
		Size: 20.8 MB (20835618 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ed7c83735e284f05034aed569d607687e904f323bb051a9efc39e8be0bb9533b`  
		Last Modified: Wed, 11 Oct 2023 19:01:31 GMT  
		Size: 95.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3fa899a007ab2c3778a4aca2b9cae642930b50bea94b54eaf110df004f78cd2e`  
		Last Modified: Wed, 11 Oct 2023 19:01:32 GMT  
		Size: 571.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `redis:7-bookworm` - unknown; unknown

```console
$ docker pull redis@sha256:bb2437e4c53d0d898bfd399601e1e23dca2ee2afcf3acfddc6822c5a45927ac4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2895047 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ece259f95fda286c2b43e385eb555e586575d3b19dfe9e62c6ebbafae04ff42`

```dockerfile
```

-	Layers:
	-	`sha256:d9a56db828b285f996af40acead2c4b7dc198c4648a1bf2da29f54d9aa010b5d`  
		Last Modified: Wed, 11 Oct 2023 19:01:31 GMT  
		Size: 2.9 MB (2865613 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:c1b9cf720b9e64d5196e13e20777f8ee01650a7d06e77660f9cdc17d77653c39`  
		Last Modified: Wed, 11 Oct 2023 19:01:31 GMT  
		Size: 29.4 KB (29434 bytes)  
		MIME: application/vnd.in-toto+json

### `redis:7-bookworm` - linux; arm variant v5

```console
$ docker pull redis@sha256:23bba2cde2e0276a2e39cbe6d6805a33766d3999669de80745a7d443dce52dfe
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.2 MB (52217779 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:30b4f88c26c33dd84fb801cc423627b1aafc9f611930af78ef9fc48853ef209f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Wed, 06 Sep 2023 21:03:16 GMT
ADD file:a4ac238e8d5bf843acb96f72c03d55e0a7f2fca33ba16d7631d397176acf8c3a in / 
# Wed, 06 Sep 2023 21:03:16 GMT
CMD ["bash"]
# Wed, 06 Sep 2023 21:03:16 GMT
RUN groupadd -r -g 999 redis && useradd -r -g redis -u 999 redis # buildkit
# Wed, 06 Sep 2023 21:03:16 GMT
ENV GOSU_VERSION=1.16
# Wed, 06 Sep 2023 21:03:16 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Wed, 06 Sep 2023 21:03:16 GMT
ENV REDIS_VERSION=7.2.1
# Wed, 06 Sep 2023 21:03:16 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-7.2.1.tar.gz
# Wed, 06 Sep 2023 21:03:16 GMT
ENV REDIS_DOWNLOAD_SHA=5c76d990a1b1c5f949bcd1eed90d0c8a4f70369bdbdcb40288c561ddf88967a4
# Wed, 06 Sep 2023 21:03:16 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				dpkg-dev 		gcc 		libc6-dev 		libssl-dev 		make 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		redis-cli --version; 	redis-server --version # buildkit
# Wed, 06 Sep 2023 21:03:16 GMT
RUN mkdir /data && chown redis:redis /data # buildkit
# Wed, 06 Sep 2023 21:03:16 GMT
VOLUME [/data]
# Wed, 06 Sep 2023 21:03:16 GMT
WORKDIR /data
# Wed, 06 Sep 2023 21:03:16 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Wed, 06 Sep 2023 21:03:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 06 Sep 2023 21:03:16 GMT
EXPOSE map[6379/tcp:{}]
# Wed, 06 Sep 2023 21:03:16 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:9de40a7a125e0755ac5cf1e38c2f8a6b3d3c005cfc82323d13f5dceb50381fd7`  
		Last Modified: Wed, 20 Sep 2023 00:54:44 GMT  
		Size: 27.0 MB (26983563 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:299bb4cd29dc5b8be1f3c38c6c1d9ef4125248241474b565ef0df955292fb69f`  
		Last Modified: Tue, 03 Oct 2023 22:59:44 GMT  
		Size: 1.1 KB (1103 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:da677a025068c1a4d002c4f637737dbbe86fd03d8ae2ba8f7533bac519ff1138`  
		Last Modified: Tue, 03 Oct 2023 22:59:44 GMT  
		Size: 1.4 MB (1413205 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d304776e2c925bf4cc34c2ceba2ec196f763438c838cf9c249276cb632430b36`  
		Last Modified: Tue, 03 Oct 2023 22:59:45 GMT  
		Size: 23.8 MB (23819209 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c7dedd86f396c295a92f6e9751d2fa1d2b84e038e0a82e5523eefebe336e04e6`  
		Last Modified: Tue, 03 Oct 2023 22:59:44 GMT  
		Size: 97.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6edf393cbce210da14ea2ca4659f7237153243267c5ee99a0a67fb04fdd345ac`  
		Last Modified: Tue, 03 Oct 2023 22:59:45 GMT  
		Size: 570.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `redis:7-bookworm` - unknown; unknown

```console
$ docker pull redis@sha256:36db5bb9d70b4c8c434fa3ff93b34d5d1edaf8538567c1bea20602416ac1c006
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.2 KB (29192 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d603d50971de789d03fc6f1a3ae8392b2fdbbc4f4fe4f1d859db76a35bfd9d7`

```dockerfile
```

-	Layers:
	-	`sha256:8ec513cad8ac9238fad69168f47a37cee7891caaf2da962953b566fd175a0d19`  
		Last Modified: Tue, 03 Oct 2023 22:59:44 GMT  
		Size: 29.2 KB (29192 bytes)  
		MIME: application/vnd.in-toto+json

### `redis:7-bookworm` - linux; arm variant v7

```console
$ docker pull redis@sha256:1572de9f2dfe5bab954ce08b76a0fc3ee98f297350a1775c270d2879a0b23bc6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.2 MB (49165011 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8925ba6c7f27852a290fba798c02d2aff950e44428ec261580f147acce216db1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Wed, 06 Sep 2023 21:03:16 GMT
ADD file:56b69c762bd03a9b00a1677740f7209aac08bac69a9e73563e326b9b0efbbfcc in / 
# Wed, 06 Sep 2023 21:03:16 GMT
CMD ["bash"]
# Wed, 06 Sep 2023 21:03:16 GMT
RUN groupadd -r -g 999 redis && useradd -r -g redis -u 999 redis # buildkit
# Wed, 06 Sep 2023 21:03:16 GMT
ENV GOSU_VERSION=1.16
# Wed, 06 Sep 2023 21:03:16 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Wed, 06 Sep 2023 21:03:16 GMT
ENV REDIS_VERSION=7.2.1
# Wed, 06 Sep 2023 21:03:16 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-7.2.1.tar.gz
# Wed, 06 Sep 2023 21:03:16 GMT
ENV REDIS_DOWNLOAD_SHA=5c76d990a1b1c5f949bcd1eed90d0c8a4f70369bdbdcb40288c561ddf88967a4
# Wed, 06 Sep 2023 21:03:16 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				dpkg-dev 		gcc 		libc6-dev 		libssl-dev 		make 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		redis-cli --version; 	redis-server --version # buildkit
# Wed, 06 Sep 2023 21:03:16 GMT
RUN mkdir /data && chown redis:redis /data # buildkit
# Wed, 06 Sep 2023 21:03:16 GMT
VOLUME [/data]
# Wed, 06 Sep 2023 21:03:16 GMT
WORKDIR /data
# Wed, 06 Sep 2023 21:03:16 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Wed, 06 Sep 2023 21:03:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 06 Sep 2023 21:03:16 GMT
EXPOSE map[6379/tcp:{}]
# Wed, 06 Sep 2023 21:03:16 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:e0b5206657a67707f4c57136f811162ce89a951fec109a406df7508d59e644cb`  
		Last Modified: Wed, 20 Sep 2023 05:01:16 GMT  
		Size: 24.8 MB (24805628 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9a13aa129b823c8550f5d5ef3f5cfda683448b0febdf912919fad56e833519e6`  
		Last Modified: Tue, 03 Oct 2023 23:22:36 GMT  
		Size: 1.1 KB (1103 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:26fb8a28b158b07e13172776c7869b0fcbd8b18d3aebfe14fa14a69e202679bc`  
		Last Modified: Tue, 03 Oct 2023 23:22:37 GMT  
		Size: 1.4 MB (1404213 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f991bbd31f2bc0fd9a4c5ad87029b4256ef5aa95ac30de815db0b836f816157b`  
		Last Modified: Tue, 03 Oct 2023 23:22:38 GMT  
		Size: 23.0 MB (22953367 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:87e63c1626dc112fdda941df7fc2ab00935bca764d3806c5c24491be214889e1`  
		Last Modified: Tue, 03 Oct 2023 23:22:37 GMT  
		Size: 96.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ff910584067f663c235cc75cb1fec85ff46af85656223073a72bf29bc53495b8`  
		Last Modified: Tue, 03 Oct 2023 23:22:37 GMT  
		Size: 572.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `redis:7-bookworm` - unknown; unknown

```console
$ docker pull redis@sha256:f7c8ae4592c793ec2dff0d5d1120738adb8bc0c4094109a3698f6d3c3d243c55
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2880087 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:24140b2470ee70efbaa14757c4889d645afd2ce7049315b73865ae4520b3d8dc`

```dockerfile
```

-	Layers:
	-	`sha256:2c67a956c7c7db4107ed2b6504170869b784f62ac12af7c297b34416b8548804`  
		Last Modified: Tue, 03 Oct 2023 23:22:37 GMT  
		Size: 2.9 MB (2850679 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:435808cc97bf09905d49acbedc9cd3c410e0b5f316490453faee1e1b28833e53`  
		Last Modified: Tue, 03 Oct 2023 23:22:36 GMT  
		Size: 29.4 KB (29408 bytes)  
		MIME: application/vnd.in-toto+json

### `redis:7-bookworm` - linux; arm64 variant v8

```console
$ docker pull redis@sha256:52423c1abd3f131a07c13eebc25a9cd931297d44e8368b228cb9984d039b3f9d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.1 MB (56136765 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:db32f19a80e6724015fc6a6f4c99731a7d4f88809a6e227313f19e1cde872734`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Wed, 06 Sep 2023 21:03:16 GMT
ADD file:ec1a6e0aedd76c8fdc8544775f8b553f58950e9435f5cfe919f39374e222cfbb in / 
# Wed, 06 Sep 2023 21:03:16 GMT
CMD ["bash"]
# Wed, 06 Sep 2023 21:03:16 GMT
RUN groupadd -r -g 999 redis && useradd -r -g redis -u 999 redis # buildkit
# Wed, 06 Sep 2023 21:03:16 GMT
ENV GOSU_VERSION=1.16
# Wed, 06 Sep 2023 21:03:16 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Wed, 06 Sep 2023 21:03:16 GMT
ENV REDIS_VERSION=7.2.1
# Wed, 06 Sep 2023 21:03:16 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-7.2.1.tar.gz
# Wed, 06 Sep 2023 21:03:16 GMT
ENV REDIS_DOWNLOAD_SHA=5c76d990a1b1c5f949bcd1eed90d0c8a4f70369bdbdcb40288c561ddf88967a4
# Wed, 06 Sep 2023 21:03:16 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				dpkg-dev 		gcc 		libc6-dev 		libssl-dev 		make 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		redis-cli --version; 	redis-server --version # buildkit
# Wed, 06 Sep 2023 21:03:16 GMT
RUN mkdir /data && chown redis:redis /data # buildkit
# Wed, 06 Sep 2023 21:03:16 GMT
VOLUME [/data]
# Wed, 06 Sep 2023 21:03:16 GMT
WORKDIR /data
# Wed, 06 Sep 2023 21:03:16 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Wed, 06 Sep 2023 21:03:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 06 Sep 2023 21:03:16 GMT
EXPOSE map[6379/tcp:{}]
# Wed, 06 Sep 2023 21:03:16 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:e886f0f47ef56fcadb6ecaf2116056bbdb273e0afe07ed034498b198d386c04e`  
		Last Modified: Wed, 20 Sep 2023 02:47:36 GMT  
		Size: 29.2 MB (29157221 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:457c001fd3ab0b1fd2982bbdf7fcd87cfe23e4fd6e6c2b1985d844350a83fd4d`  
		Last Modified: Tue, 03 Oct 2023 23:01:03 GMT  
		Size: 1.1 KB (1103 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6631c396a6801c022fffda7948e7456b388b027e99c053a80c91aa5969900266`  
		Last Modified: Tue, 03 Oct 2023 23:01:04 GMT  
		Size: 1.4 MB (1367692 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5b3bbf47b73bc7dc383c3345d5337bc7316ada9122aa5f6e6e8908de1359b18a`  
		Last Modified: Tue, 03 Oct 2023 23:01:06 GMT  
		Size: 25.6 MB (25610049 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:243ce8b1e9f31ccd9bdd8c747f0a4f1e171340a46e4d35e80a7ce6ac26d363fb`  
		Last Modified: Tue, 03 Oct 2023 23:01:03 GMT  
		Size: 95.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7d9a2aec0feefc5a119404a107c85df6fe4f9903c14b97537f096dcee6800c7e`  
		Last Modified: Tue, 03 Oct 2023 23:01:05 GMT  
		Size: 573.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `redis:7-bookworm` - unknown; unknown

```console
$ docker pull redis@sha256:b1ef20225c2c57d4504e2b753db19eacbc80a9c6ff2a64cb5c6c82bf66450d92
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2874538 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ca654f876b291bcf3c0568b6648592d5aeb45f72b01e3b631874e940985e4bc5`

```dockerfile
```

-	Layers:
	-	`sha256:697bec6399df7f0ffa678c6135f606a91cd252e1fa9eaf9357fadb4818b60017`  
		Last Modified: Tue, 03 Oct 2023 23:01:04 GMT  
		Size: 2.8 MB (2845253 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:8aadf0f038c5d1c58fa8a338a1b8e6463615a1582abe9d900857919f7819717f`  
		Last Modified: Tue, 03 Oct 2023 23:01:03 GMT  
		Size: 29.3 KB (29285 bytes)  
		MIME: application/vnd.in-toto+json

### `redis:7-bookworm` - linux; 386

```console
$ docker pull redis@sha256:7caa5be15a43f7536d6a7c92ebdd60300013272c73174c769a8d22173fb70dad
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.8 MB (56846110 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:043743b7e2df811b96129a45b9554442dd5a558c3a8037bf78e4a6c9a1484ca7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Wed, 06 Sep 2023 21:03:16 GMT
ADD file:efe81f7066129aa6293627bfe4ea78b957897ba5ede951970156fccf1dbcde88 in / 
# Wed, 06 Sep 2023 21:03:16 GMT
CMD ["bash"]
# Wed, 06 Sep 2023 21:03:16 GMT
RUN groupadd -r -g 999 redis && useradd -r -g redis -u 999 redis # buildkit
# Wed, 06 Sep 2023 21:03:16 GMT
ENV GOSU_VERSION=1.16
# Wed, 06 Sep 2023 21:03:16 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Wed, 06 Sep 2023 21:03:16 GMT
ENV REDIS_VERSION=7.2.1
# Wed, 06 Sep 2023 21:03:16 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-7.2.1.tar.gz
# Wed, 06 Sep 2023 21:03:16 GMT
ENV REDIS_DOWNLOAD_SHA=5c76d990a1b1c5f949bcd1eed90d0c8a4f70369bdbdcb40288c561ddf88967a4
# Wed, 06 Sep 2023 21:03:16 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				dpkg-dev 		gcc 		libc6-dev 		libssl-dev 		make 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		redis-cli --version; 	redis-server --version # buildkit
# Wed, 06 Sep 2023 21:03:16 GMT
RUN mkdir /data && chown redis:redis /data # buildkit
# Wed, 06 Sep 2023 21:03:16 GMT
VOLUME [/data]
# Wed, 06 Sep 2023 21:03:16 GMT
WORKDIR /data
# Wed, 06 Sep 2023 21:03:16 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Wed, 06 Sep 2023 21:03:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 06 Sep 2023 21:03:16 GMT
EXPOSE map[6379/tcp:{}]
# Wed, 06 Sep 2023 21:03:16 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:6ac07f93e07a1bad4555e13bd8efd06169988669fc88df95f4bf296a2b44523d`  
		Last Modified: Wed, 20 Sep 2023 00:46:48 GMT  
		Size: 30.1 MB (30141894 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:299bb4cd29dc5b8be1f3c38c6c1d9ef4125248241474b565ef0df955292fb69f`  
		Last Modified: Tue, 03 Oct 2023 22:59:44 GMT  
		Size: 1.1 KB (1103 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:54e8b77295fae1f5e14674dce7e8772f74291b7a3fd2cbfa6153ef247146d7e9`  
		Last Modified: Tue, 03 Oct 2023 23:00:17 GMT  
		Size: 1.4 MB (1411602 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4375b9402520101bb96d36588ad1d352b0608752628facbe9f7739440c00280f`  
		Last Modified: Tue, 03 Oct 2023 23:00:18 GMT  
		Size: 25.3 MB (25290809 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f2af616e829901a88e881ac4712c8e76d67b411b98dfaf73eb1b5829b9824830`  
		Last Modified: Tue, 03 Oct 2023 23:00:17 GMT  
		Size: 97.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7c83a20d293ba74d539082c9e45057e82708aa30a7edbd2d410e25178037d414`  
		Last Modified: Tue, 03 Oct 2023 23:00:17 GMT  
		Size: 573.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `redis:7-bookworm` - unknown; unknown

```console
$ docker pull redis@sha256:9751271d9daeea272ffa7756970a93b80f68be1704b91fdc88e4efed061e048a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.2 KB (29164 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:23d0ce1db278083753c55f8ccfee905f7a5d8214aab854f41693e65f47b37b2f`

```dockerfile
```

-	Layers:
	-	`sha256:cc2c13a706bee2844acc7ea4db90579aa591cb448a72273ed01c8494c007be2c`  
		Last Modified: Tue, 03 Oct 2023 23:00:16 GMT  
		Size: 29.2 KB (29164 bytes)  
		MIME: application/vnd.in-toto+json

### `redis:7-bookworm` - linux; mips64le

```console
$ docker pull redis@sha256:5972d9afdcf76c6c20d97811f5a7f69cf1940e34d5f281c48155fa3095e4ed40
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.5 MB (56500185 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d48628c5a89e6ace8455dfc447e4693d811eeb8b2da811d037d337a95717b8b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Wed, 06 Sep 2023 21:03:16 GMT
ADD file:850547a08e38ebc5a3659df86e70039a8d9828ae26ae485b077c98a959248dcb in / 
# Wed, 06 Sep 2023 21:03:16 GMT
CMD ["bash"]
# Wed, 06 Sep 2023 21:03:16 GMT
RUN groupadd -r -g 999 redis && useradd -r -g redis -u 999 redis # buildkit
# Wed, 06 Sep 2023 21:03:16 GMT
ENV GOSU_VERSION=1.16
# Wed, 06 Sep 2023 21:03:16 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Wed, 06 Sep 2023 21:03:16 GMT
ENV REDIS_VERSION=7.2.1
# Wed, 06 Sep 2023 21:03:16 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-7.2.1.tar.gz
# Wed, 06 Sep 2023 21:03:16 GMT
ENV REDIS_DOWNLOAD_SHA=5c76d990a1b1c5f949bcd1eed90d0c8a4f70369bdbdcb40288c561ddf88967a4
# Wed, 06 Sep 2023 21:03:16 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				dpkg-dev 		gcc 		libc6-dev 		libssl-dev 		make 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		redis-cli --version; 	redis-server --version # buildkit
# Wed, 06 Sep 2023 21:03:16 GMT
RUN mkdir /data && chown redis:redis /data # buildkit
# Wed, 06 Sep 2023 21:03:16 GMT
VOLUME [/data]
# Wed, 06 Sep 2023 21:03:16 GMT
WORKDIR /data
# Wed, 06 Sep 2023 21:03:16 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Wed, 06 Sep 2023 21:03:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 06 Sep 2023 21:03:16 GMT
EXPOSE map[6379/tcp:{}]
# Wed, 06 Sep 2023 21:03:16 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:0f581c6294fe7421dfee024e2c7dddd73ef3fbd7ff23b05bc3c1bf9f50885e85`  
		Last Modified: Wed, 20 Sep 2023 03:20:59 GMT  
		Size: 29.1 MB (29121674 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c6d44a2ed54cccb98e0c8d8bfd3e9348ee3a0bf1428969f7a2c62fe9a0972d5d`  
		Last Modified: Tue, 03 Oct 2023 23:05:50 GMT  
		Size: 1.1 KB (1101 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:bcfa00742665f7e553b3bc45e87c03bd98bc4da28e1f5bfda6e8789427814cee`  
		Last Modified: Tue, 03 Oct 2023 23:05:50 GMT  
		Size: 1.3 MB (1324116 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ba13329995a4529e131930d11af821e0c03d1329576c068f613ebb3fee309468`  
		Last Modified: Tue, 03 Oct 2023 23:05:53 GMT  
		Size: 26.1 MB (26052597 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2ed5d403365cf084baf61edef65d6736c7c696aeee49bf9b51c02864eb539b74`  
		Last Modified: Tue, 03 Oct 2023 23:05:50 GMT  
		Size: 95.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:772d7570c390780b55ed8dbc2593254efd11bf1c8911ee8e352722fea09c33ab`  
		Last Modified: Tue, 03 Oct 2023 23:05:51 GMT  
		Size: 570.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `redis:7-bookworm` - unknown; unknown

```console
$ docker pull redis@sha256:071c90d898c9abc5d3a2cec22d88f289a4d306d00633d7f028c4c434b8e81ff9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.2 KB (29154 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:adce51c1deb33c8d58cc86c84fe80637254738f908824fa803dc67cde3e44693`

```dockerfile
```

-	Layers:
	-	`sha256:fd5d5a8662e63cfc9c1a67e74512bc1a4e79b2dc4bfcbcc53f3d5c6d8f67ba8a`  
		Last Modified: Tue, 03 Oct 2023 23:05:50 GMT  
		Size: 29.2 KB (29154 bytes)  
		MIME: application/vnd.in-toto+json

### `redis:7-bookworm` - linux; ppc64le

```console
$ docker pull redis@sha256:843ed83e9b61ce98d0d5c7997e413f84aa21337aad9a2f1d0d6a500648f84ca3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.0 MB (63006835 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dee3a12f4fdfb64b4c326d8cb5471a63cb9b929a34052445f407bf6afa8a203f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Wed, 06 Sep 2023 21:03:16 GMT
ADD file:9a37b479e68a0d18babbef8dd04d09a0e6844a0080876d14144a34bfd9d0897a in / 
# Wed, 06 Sep 2023 21:03:16 GMT
CMD ["bash"]
# Wed, 06 Sep 2023 21:03:16 GMT
RUN groupadd -r -g 999 redis && useradd -r -g redis -u 999 redis # buildkit
# Wed, 06 Sep 2023 21:03:16 GMT
ENV GOSU_VERSION=1.16
# Wed, 06 Sep 2023 21:03:16 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Wed, 06 Sep 2023 21:03:16 GMT
ENV REDIS_VERSION=7.2.1
# Wed, 06 Sep 2023 21:03:16 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-7.2.1.tar.gz
# Wed, 06 Sep 2023 21:03:16 GMT
ENV REDIS_DOWNLOAD_SHA=5c76d990a1b1c5f949bcd1eed90d0c8a4f70369bdbdcb40288c561ddf88967a4
# Wed, 06 Sep 2023 21:03:16 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				dpkg-dev 		gcc 		libc6-dev 		libssl-dev 		make 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		redis-cli --version; 	redis-server --version # buildkit
# Wed, 06 Sep 2023 21:03:16 GMT
RUN mkdir /data && chown redis:redis /data # buildkit
# Wed, 06 Sep 2023 21:03:16 GMT
VOLUME [/data]
# Wed, 06 Sep 2023 21:03:16 GMT
WORKDIR /data
# Wed, 06 Sep 2023 21:03:16 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Wed, 06 Sep 2023 21:03:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 06 Sep 2023 21:03:16 GMT
EXPOSE map[6379/tcp:{}]
# Wed, 06 Sep 2023 21:03:16 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:696a66e961f2033dcf69b003ad7faf28ed2248da58efa1c08a9d496739a8eeeb`  
		Last Modified: Wed, 20 Sep 2023 08:49:51 GMT  
		Size: 33.1 MB (33119461 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f7a5e143415842a5f669709af637faa5a01610f07493b4465e9dd6acf35e33fb`  
		Last Modified: Tue, 03 Oct 2023 23:02:37 GMT  
		Size: 1.1 KB (1103 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b5a8c07cdef0780ba543dc1c5271114516e2654b4927b012c80217e3654d4d1c`  
		Last Modified: Tue, 03 Oct 2023 23:02:38 GMT  
		Size: 1.4 MB (1358927 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d4d135571fcd0043cfb676f8366d34a0e087f635634bd92e887ef11c3ee77888`  
		Last Modified: Tue, 03 Oct 2023 23:02:40 GMT  
		Size: 28.5 MB (28526642 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b3677e8b31440a9fce03dc8a94637f5a3818f5e80a308df78abfdd32b47e1439`  
		Last Modified: Tue, 03 Oct 2023 23:02:38 GMT  
		Size: 97.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:74e78a99561925da9f9c49fdc4c799ccb137c5d248326e41c991d5086c6d845e`  
		Last Modified: Tue, 03 Oct 2023 23:02:39 GMT  
		Size: 573.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `redis:7-bookworm` - unknown; unknown

```console
$ docker pull redis@sha256:478b5d69ed06c55d81b95e8c883c268466b995697d723d236543da81c7085bda
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2898467 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:40221f3907041cdb8ed9691da6ada2993068f206f0c7ea5fbc788bd27454f2e3`

```dockerfile
```

-	Layers:
	-	`sha256:cadf019405d4d49523a2ecb00ed53e7ad2fe384f4b1ece330e99e811f047aac1`  
		Last Modified: Tue, 03 Oct 2023 23:02:38 GMT  
		Size: 2.9 MB (2869132 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:7a792d7d262ee2709fafb5cec29b9bb23ead43889de5bfc133f28cf3e0d879fd`  
		Last Modified: Tue, 03 Oct 2023 23:02:37 GMT  
		Size: 29.3 KB (29335 bytes)  
		MIME: application/vnd.in-toto+json

### `redis:7-bookworm` - linux; s390x

```console
$ docker pull redis@sha256:4f99b355cbcc64766db9e7a99a2f2dcc98d5a5a37ac12ea263c87af41a4a0d1b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.5 MB (53547945 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:86e8b4be815efd8397d633e210a10d49cdc1c23bfefdbdf041781b589023297e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Wed, 06 Sep 2023 21:03:16 GMT
ADD file:6ed982ad3e8566d63315a27a81b33069910952aef4b2d3e0b607bd2caeac7ca4 in / 
# Wed, 06 Sep 2023 21:03:16 GMT
CMD ["bash"]
# Wed, 06 Sep 2023 21:03:16 GMT
RUN groupadd -r -g 999 redis && useradd -r -g redis -u 999 redis # buildkit
# Wed, 06 Sep 2023 21:03:16 GMT
ENV GOSU_VERSION=1.16
# Wed, 06 Sep 2023 21:03:16 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Wed, 06 Sep 2023 21:03:16 GMT
ENV REDIS_VERSION=7.2.1
# Wed, 06 Sep 2023 21:03:16 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-7.2.1.tar.gz
# Wed, 06 Sep 2023 21:03:16 GMT
ENV REDIS_DOWNLOAD_SHA=5c76d990a1b1c5f949bcd1eed90d0c8a4f70369bdbdcb40288c561ddf88967a4
# Wed, 06 Sep 2023 21:03:16 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				dpkg-dev 		gcc 		libc6-dev 		libssl-dev 		make 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		redis-cli --version; 	redis-server --version # buildkit
# Wed, 06 Sep 2023 21:03:16 GMT
RUN mkdir /data && chown redis:redis /data # buildkit
# Wed, 06 Sep 2023 21:03:16 GMT
VOLUME [/data]
# Wed, 06 Sep 2023 21:03:16 GMT
WORKDIR /data
# Wed, 06 Sep 2023 21:03:16 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Wed, 06 Sep 2023 21:03:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 06 Sep 2023 21:03:16 GMT
EXPOSE map[6379/tcp:{}]
# Wed, 06 Sep 2023 21:03:16 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:26dcff366e33abcf08b812052a4c12496aa406aa267655e984aa7a84ca254cd8`  
		Last Modified: Wed, 20 Sep 2023 02:59:47 GMT  
		Size: 27.5 MB (27489966 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:98793b8f09c9ffcfade45e13946ac7a76a944ca573ead98a5554d3f8926dd6b9`  
		Last Modified: Tue, 03 Oct 2023 23:36:31 GMT  
		Size: 1.1 KB (1101 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3a7422a5babea5a71de43f5cce871efed4ceccf350cd2b85f8934ca20b47a7e0`  
		Last Modified: Tue, 03 Oct 2023 23:36:31 GMT  
		Size: 1.4 MB (1401400 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:40656bdaeb66134712a28da5d14a8e38796929fe2a67914ed8f9281b16f2aead`  
		Last Modified: Wed, 04 Oct 2023 00:01:34 GMT  
		Size: 24.7 MB (24654777 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:05ab2b899997da6c3b91f828692a9db89a58b487623547f414a4944f53ce640f`  
		Last Modified: Wed, 04 Oct 2023 00:01:32 GMT  
		Size: 96.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7c4b44d973a2d66a95318271fd479259f5e6bcc45ae8b3131ed743d7aae89190`  
		Last Modified: Wed, 04 Oct 2023 00:01:32 GMT  
		Size: 573.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `redis:7-bookworm` - unknown; unknown

```console
$ docker pull redis@sha256:f18cf80411269f4c68497bca128cfc5aa9b93e335e64d7922447c5a63af1ec75
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2880890 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3424f99ec99d0dddc93d29dd0fe9edadb2a51edaf1e12fd97a09f98cd8417ac2`

```dockerfile
```

-	Layers:
	-	`sha256:e0c1edb9912cffa07c6babbdfabd11726350577edc45b87ccd0f12e0183b1b01`  
		Last Modified: Wed, 04 Oct 2023 00:01:32 GMT  
		Size: 2.9 MB (2851623 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:1cafb95bcc438fe54a401a79ecbf7f1f9e1add16c67653448222a4c67ffb7437`  
		Last Modified: Wed, 04 Oct 2023 00:01:32 GMT  
		Size: 29.3 KB (29267 bytes)  
		MIME: application/vnd.in-toto+json
