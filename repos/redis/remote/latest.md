## `redis:latest`

```console
$ docker pull redis@sha256:4ab9df56369ea0c81b47dd5fd9228fd4982dbf9dbafa1089b9cd1c41c14af1ff
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

### `redis:latest` - linux; amd64

```console
$ docker pull redis@sha256:213c0c68315a183fed6d47e6839a3f7edbaf85a777ef16a1485d1729260081cd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.4 MB (51426164 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66e396a38800abbf1fab51e4f25c5a2275d60e9fc4f2c7ccbb09ce2c6fc62db8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Wed, 18 Oct 2023 09:03:13 GMT
ADD file:fbd8521c24ed758023728505c18d7a0d6d101bc77fd772a4af9b65049b943864 in / 
# Wed, 18 Oct 2023 09:03:13 GMT
CMD ["bash"]
# Wed, 18 Oct 2023 09:03:13 GMT
RUN groupadd -r -g 999 redis && useradd -r -g redis -u 999 redis # buildkit
# Wed, 18 Oct 2023 09:03:13 GMT
ENV GOSU_VERSION=1.16
# Wed, 18 Oct 2023 09:03:13 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Wed, 18 Oct 2023 09:03:13 GMT
ENV REDIS_VERSION=7.2.2
# Wed, 18 Oct 2023 09:03:13 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-7.2.2.tar.gz
# Wed, 18 Oct 2023 09:03:13 GMT
ENV REDIS_DOWNLOAD_SHA=ca999be08800edc6d265379c4c7aafad92f0ee400692e4e2d69829ab4b4c3d08
# Wed, 18 Oct 2023 09:03:13 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				dpkg-dev 		gcc 		libc6-dev 		libssl-dev 		make 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		redis-cli --version; 	redis-server --version # buildkit
# Wed, 18 Oct 2023 09:03:13 GMT
RUN mkdir /data && chown redis:redis /data # buildkit
# Wed, 18 Oct 2023 09:03:13 GMT
VOLUME [/data]
# Wed, 18 Oct 2023 09:03:13 GMT
WORKDIR /data
# Wed, 18 Oct 2023 09:03:13 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Wed, 18 Oct 2023 09:03:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 18 Oct 2023 09:03:13 GMT
EXPOSE map[6379/tcp:{}]
# Wed, 18 Oct 2023 09:03:13 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:578acb154839e9d0034432e8f53756d6f53ba62cf8c7ea5218a2476bf5b58fc9`  
		Last Modified: Wed, 01 Nov 2023 00:25:30 GMT  
		Size: 29.1 MB (29149836 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:84fabc2ec71c3f09bd700b8ed3c89ecc6883065535a33d6a7e4338df1cc84001`  
		Last Modified: Wed, 01 Nov 2023 01:04:18 GMT  
		Size: 1.1 KB (1101 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:97e3a2c7600c65ad61623f466d17e0c81317d1f39c65f8ad73ca078ec0b12976`  
		Last Modified: Wed, 01 Nov 2023 01:04:18 GMT  
		Size: 1.4 MB (1439861 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a41326ea4d3e0ea620afebc57fcb94f8dd02216702247f1d52bab9fd038132c0`  
		Last Modified: Wed, 01 Nov 2023 01:04:19 GMT  
		Size: 20.8 MB (20834666 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:925323722c7117ecc202ec03dbbb0fa9b0050dfebdbb444c8acff5ab53e5ac3d`  
		Last Modified: Wed, 01 Nov 2023 01:04:18 GMT  
		Size: 97.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0626a32dd9d8b5ebfbdcf2a70ff8508198e16cc8dbd4962b63295302673703cf`  
		Last Modified: Wed, 01 Nov 2023 01:04:19 GMT  
		Size: 571.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `redis:latest` - unknown; unknown

```console
$ docker pull redis@sha256:368e0aa99238efcd20733505587eea35b396d23bdb96e04ec91b71c2941f730f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 MB (3063099 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b8de1bb1652ae988e010416ea49e0296390eb9a969840412b98564f970749ad`

```dockerfile
```

-	Layers:
	-	`sha256:c29d65889ccb975bd29ec5148c1a119a2368ded5053c0142223ad479cdac8ac7`  
		Last Modified: Wed, 01 Nov 2023 01:04:18 GMT  
		Size: 3.0 MB (3033665 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:720e493d9271e9b1e89e53e19dd0b8ba78ccf0cc6220f824795582f8a4810e83`  
		Last Modified: Wed, 01 Nov 2023 01:04:18 GMT  
		Size: 29.4 KB (29434 bytes)  
		MIME: application/vnd.in-toto+json

### `redis:latest` - linux; arm variant v5

```console
$ docker pull redis@sha256:f128f882b7d7fedd24d3e04093480b64728a47766329b6324bb279d9f5f3596b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.5 MB (47515161 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c4851040ba8845bbac5b8b92216b2d23d2211cd4ba2d1c4781ec55e682cec22e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Wed, 18 Oct 2023 09:03:13 GMT
ADD file:c00ddcb556a3791b020308012fd4d7749535c34d372bac47f6ff687a7652b25f in / 
# Wed, 18 Oct 2023 09:03:13 GMT
CMD ["bash"]
# Wed, 18 Oct 2023 09:03:13 GMT
RUN groupadd -r -g 999 redis && useradd -r -g redis -u 999 redis # buildkit
# Wed, 18 Oct 2023 09:03:13 GMT
ENV GOSU_VERSION=1.16
# Wed, 18 Oct 2023 09:03:13 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Wed, 18 Oct 2023 09:03:13 GMT
ENV REDIS_VERSION=7.2.2
# Wed, 18 Oct 2023 09:03:13 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-7.2.2.tar.gz
# Wed, 18 Oct 2023 09:03:13 GMT
ENV REDIS_DOWNLOAD_SHA=ca999be08800edc6d265379c4c7aafad92f0ee400692e4e2d69829ab4b4c3d08
# Wed, 18 Oct 2023 09:03:13 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				dpkg-dev 		gcc 		libc6-dev 		libssl-dev 		make 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		redis-cli --version; 	redis-server --version # buildkit
# Wed, 18 Oct 2023 09:03:13 GMT
RUN mkdir /data && chown redis:redis /data # buildkit
# Wed, 18 Oct 2023 09:03:13 GMT
VOLUME [/data]
# Wed, 18 Oct 2023 09:03:13 GMT
WORKDIR /data
# Wed, 18 Oct 2023 09:03:13 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Wed, 18 Oct 2023 09:03:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 18 Oct 2023 09:03:13 GMT
EXPOSE map[6379/tcp:{}]
# Wed, 18 Oct 2023 09:03:13 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:8d7feeb74478e4770869563dfee6adf560c449e1ac037f4250fde21517f75323`  
		Last Modified: Wed, 01 Nov 2023 00:51:29 GMT  
		Size: 26.9 MB (26921998 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b4e2daa8cb2edb9834ea413392fc875380b84865d4783c0123de01e4e4238dd2`  
		Last Modified: Wed, 01 Nov 2023 01:04:02 GMT  
		Size: 1.1 KB (1101 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ffa4885fb8ab738900322f698116c5d314bf0f6f32d426600ce1fcd399f4b684`  
		Last Modified: Wed, 01 Nov 2023 01:04:03 GMT  
		Size: 1.4 MB (1417831 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f1da07950ea414e594bb9637515c66ca73cb26500003585ac603b3b8f27fc620`  
		Last Modified: Wed, 01 Nov 2023 18:09:42 GMT  
		Size: 19.2 MB (19173531 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:598caec338c5fad322b49c5f98740d1fea506a1656775641f1e525793331b131`  
		Last Modified: Wed, 01 Nov 2023 18:09:40 GMT  
		Size: 97.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a27fb7dfa8590ea9d0b3d9d9bb748a26c1824bcb5d599a290e03ee9d42480e51`  
		Last Modified: Wed, 01 Nov 2023 18:09:40 GMT  
		Size: 571.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `redis:latest` - unknown; unknown

```console
$ docker pull redis@sha256:6c620d9e106acb35dcbbe379289e79a6bda26b0b88b145290b11dbc146b350b4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.2 KB (29193 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d76390c838da2413f6ddf5ef655e1d75a3671ed42f7a4921369f83b2ddaa0d87`

```dockerfile
```

-	Layers:
	-	`sha256:3d8813c5988b1edf139324ca0e08065c6182ee680cc63a0aa3d344d0db8bc605`  
		Last Modified: Wed, 01 Nov 2023 18:09:40 GMT  
		Size: 29.2 KB (29193 bytes)  
		MIME: application/vnd.in-toto+json

### `redis:latest` - linux; arm variant v7

```console
$ docker pull redis@sha256:8c8b1b7ef4862c2a146b5842510a0f5e3950af992273d7071e66d85e94c15019
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.8 MB (44756292 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:80504458edbcb6d46cb07ee34274fcda6dd1f3ccaaf9865f67bbe27df9a96eb6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Wed, 18 Oct 2023 09:03:13 GMT
ADD file:fbe34fcf46c7cb91e83b67f7381d8971c97842aadd3e081994eaee4c08043106 in / 
# Wed, 18 Oct 2023 09:03:13 GMT
CMD ["bash"]
# Wed, 18 Oct 2023 09:03:13 GMT
RUN groupadd -r -g 999 redis && useradd -r -g redis -u 999 redis # buildkit
# Wed, 18 Oct 2023 09:03:13 GMT
ENV GOSU_VERSION=1.16
# Wed, 18 Oct 2023 09:03:13 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Wed, 18 Oct 2023 09:03:13 GMT
ENV REDIS_VERSION=7.2.2
# Wed, 18 Oct 2023 09:03:13 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-7.2.2.tar.gz
# Wed, 18 Oct 2023 09:03:13 GMT
ENV REDIS_DOWNLOAD_SHA=ca999be08800edc6d265379c4c7aafad92f0ee400692e4e2d69829ab4b4c3d08
# Wed, 18 Oct 2023 09:03:13 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				dpkg-dev 		gcc 		libc6-dev 		libssl-dev 		make 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		redis-cli --version; 	redis-server --version # buildkit
# Wed, 18 Oct 2023 09:03:13 GMT
RUN mkdir /data && chown redis:redis /data # buildkit
# Wed, 18 Oct 2023 09:03:13 GMT
VOLUME [/data]
# Wed, 18 Oct 2023 09:03:13 GMT
WORKDIR /data
# Wed, 18 Oct 2023 09:03:13 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Wed, 18 Oct 2023 09:03:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 18 Oct 2023 09:03:13 GMT
EXPOSE map[6379/tcp:{}]
# Wed, 18 Oct 2023 09:03:13 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:0a684901cedc28e6abb4cde4579d23d26345d871acd708a5bf266c562fe15b4d`  
		Last Modified: Wed, 01 Nov 2023 01:02:13 GMT  
		Size: 24.7 MB (24748900 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:617a5bb075ca9ddc1eb82c65d1143bd96893ac6c46fe1236147db51b49e51b4a`  
		Last Modified: Thu, 02 Nov 2023 00:56:45 GMT  
		Size: 1.1 KB (1100 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a4547e8862e542c75d209b53dded5cbc13781e2dc177f88f0a281511f318d33c`  
		Last Modified: Thu, 02 Nov 2023 00:56:46 GMT  
		Size: 1.4 MB (1408389 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f2b3f6afc7d629666fc90acccd961e715e8ca62ece48a639ab3f388e0e06024c`  
		Last Modified: Thu, 02 Nov 2023 00:56:47 GMT  
		Size: 18.6 MB (18597203 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0e52c0dc3ed09696d3c33b8440d0022b7de129f1842a3749da42aea792ea11bb`  
		Last Modified: Thu, 02 Nov 2023 00:56:46 GMT  
		Size: 96.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2c45d099dcfee06122fde9f82481e321e841675af1c3299db0d50ff47ee27587`  
		Last Modified: Thu, 02 Nov 2023 00:56:47 GMT  
		Size: 572.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `redis:latest` - unknown; unknown

```console
$ docker pull redis@sha256:f4183639b51ebca3fb5c637a70bede7c80224f63eaede5ec64f0d9c9f276c886
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3037641 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:02120e08fe2f5b3d2ceaf37047467a12f02f7295b5d090d48f09f60ff94c37e6`

```dockerfile
```

-	Layers:
	-	`sha256:8688d8a5a52f10ed1fba352b85c148d29e49ea6f677c7540d6d8bdab468a8050`  
		Last Modified: Thu, 02 Nov 2023 00:56:46 GMT  
		Size: 3.0 MB (3008233 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:8f4e66bfcf45ecad6823df98fea18970e47bb60a201badf75760ba1d9d136347`  
		Last Modified: Thu, 02 Nov 2023 00:56:45 GMT  
		Size: 29.4 KB (29408 bytes)  
		MIME: application/vnd.in-toto+json

### `redis:latest` - linux; arm64 variant v8

```console
$ docker pull redis@sha256:d23b32d067294eed9597c7bed44f6e3945bf3f2898bcb574df9193c0f64cf6dd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.4 MB (50402175 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:279a07cfa3394450f63f88afab8f8bdd019addafd11a63b43a3dee7130f8a4e0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Wed, 18 Oct 2023 09:03:13 GMT
ADD file:c58f86cd28b3a97f884e2a46f8fe60a2c5c1f443e198bd10e3277b4f3653736a in / 
# Wed, 18 Oct 2023 09:03:13 GMT
CMD ["bash"]
# Wed, 18 Oct 2023 09:03:13 GMT
RUN groupadd -r -g 999 redis && useradd -r -g redis -u 999 redis # buildkit
# Wed, 18 Oct 2023 09:03:13 GMT
ENV GOSU_VERSION=1.16
# Wed, 18 Oct 2023 09:03:13 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Wed, 18 Oct 2023 09:03:13 GMT
ENV REDIS_VERSION=7.2.2
# Wed, 18 Oct 2023 09:03:13 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-7.2.2.tar.gz
# Wed, 18 Oct 2023 09:03:13 GMT
ENV REDIS_DOWNLOAD_SHA=ca999be08800edc6d265379c4c7aafad92f0ee400692e4e2d69829ab4b4c3d08
# Wed, 18 Oct 2023 09:03:13 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				dpkg-dev 		gcc 		libc6-dev 		libssl-dev 		make 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		redis-cli --version; 	redis-server --version # buildkit
# Wed, 18 Oct 2023 09:03:13 GMT
RUN mkdir /data && chown redis:redis /data # buildkit
# Wed, 18 Oct 2023 09:03:13 GMT
VOLUME [/data]
# Wed, 18 Oct 2023 09:03:13 GMT
WORKDIR /data
# Wed, 18 Oct 2023 09:03:13 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Wed, 18 Oct 2023 09:03:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 18 Oct 2023 09:03:13 GMT
EXPOSE map[6379/tcp:{}]
# Wed, 18 Oct 2023 09:03:13 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:31ce7ceb6d443e2ab4ae91695fea10e1443417fd94c40a46994d5a96940ea1ca`  
		Last Modified: Wed, 01 Nov 2023 00:43:07 GMT  
		Size: 29.2 MB (29179119 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3e7e9ad93cf6b1248afb9cbcd552f247529f92a4f2edef7dd873a5607d6d5c22`  
		Last Modified: Wed, 01 Nov 2023 20:29:42 GMT  
		Size: 1.1 KB (1101 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:71b55c03cd63a316ab14ede434b879fbee364dc591e843c93e73ec10bf2a534e`  
		Last Modified: Wed, 01 Nov 2023 20:29:43 GMT  
		Size: 1.4 MB (1372460 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:48a1c2d6489ff8c0262c47fa699592508780f306ee91af0cd3883813bf16309b`  
		Last Modified: Wed, 01 Nov 2023 20:29:43 GMT  
		Size: 19.8 MB (19848794 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fb6c83a525319c17c6e2e6a7ff6f3e89898e33be928c9302219388b2615d6507`  
		Last Modified: Wed, 01 Nov 2023 20:29:42 GMT  
		Size: 95.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8d695b9149d28fb846008a0bb0aa3c03886d0f6b75acc3c35140dfd85c85107e`  
		Last Modified: Wed, 01 Nov 2023 20:29:43 GMT  
		Size: 574.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `redis:latest` - unknown; unknown

```console
$ docker pull redis@sha256:6687c424b2ef213a042a677b65023bdcbf5429cffb9a546ea31418bfad1944d0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3038131 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9df6b3a428063c7806af8950a996c142253684579423e93323f1676ecfbf96ee`

```dockerfile
```

-	Layers:
	-	`sha256:badb6712ef52d55220b98de2e344f8c4ff060cc62d98c19405c68885bbfb4974`  
		Last Modified: Wed, 01 Nov 2023 20:29:43 GMT  
		Size: 3.0 MB (3008846 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:c6f1444550d080fd612bdaaba0f3d3a4fa54ac82e0be7bc02ac52dbdd9de4b73`  
		Last Modified: Wed, 01 Nov 2023 20:29:42 GMT  
		Size: 29.3 KB (29285 bytes)  
		MIME: application/vnd.in-toto+json

### `redis:latest` - linux; 386

```console
$ docker pull redis@sha256:0a5ad905c1902665cef570d6f4c26ec01831aca03c9b5c0551536a71c40ab3e4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.5 MB (51489476 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3fe0dbe1052037e1f2a9cc2ee32336af7a5dcce0ee2d45ad3c383cb0c9278dee`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Wed, 18 Oct 2023 09:03:13 GMT
ADD file:0c94521fdd9c0a4fdeeb9aad23e68cd053fba0dcd7c3af550aefa79377816e31 in / 
# Wed, 18 Oct 2023 09:03:13 GMT
CMD ["bash"]
# Wed, 18 Oct 2023 09:03:13 GMT
RUN groupadd -r -g 999 redis && useradd -r -g redis -u 999 redis # buildkit
# Wed, 18 Oct 2023 09:03:13 GMT
ENV GOSU_VERSION=1.16
# Wed, 18 Oct 2023 09:03:13 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Wed, 18 Oct 2023 09:03:13 GMT
ENV REDIS_VERSION=7.2.2
# Wed, 18 Oct 2023 09:03:13 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-7.2.2.tar.gz
# Wed, 18 Oct 2023 09:03:13 GMT
ENV REDIS_DOWNLOAD_SHA=ca999be08800edc6d265379c4c7aafad92f0ee400692e4e2d69829ab4b4c3d08
# Wed, 18 Oct 2023 09:03:13 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				dpkg-dev 		gcc 		libc6-dev 		libssl-dev 		make 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		redis-cli --version; 	redis-server --version # buildkit
# Wed, 18 Oct 2023 09:03:13 GMT
RUN mkdir /data && chown redis:redis /data # buildkit
# Wed, 18 Oct 2023 09:03:13 GMT
VOLUME [/data]
# Wed, 18 Oct 2023 09:03:13 GMT
WORKDIR /data
# Wed, 18 Oct 2023 09:03:13 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Wed, 18 Oct 2023 09:03:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 18 Oct 2023 09:03:13 GMT
EXPOSE map[6379/tcp:{}]
# Wed, 18 Oct 2023 09:03:13 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:98bdfce9af831c2a0d0bfcca812d0039cd1666986550f552b4b4c625bd5aa31c`  
		Last Modified: Wed, 01 Nov 2023 00:43:26 GMT  
		Size: 30.2 MB (30164042 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:01156462b42c8010e5e73c369f7235a3ea7d80ca41c06cd93cb26e000beb69d8`  
		Last Modified: Wed, 01 Nov 2023 01:04:32 GMT  
		Size: 1.1 KB (1099 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:51fda6075d7ac4899fee81a1d33afc3cdf854f1a00d27ac4a21c997a6e277e92`  
		Last Modified: Wed, 01 Nov 2023 01:04:32 GMT  
		Size: 1.4 MB (1416417 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:071b1dc3fe9f415cc8adde303983bc43fb46cc37df29ea0fa6878eae956b48bf`  
		Last Modified: Wed, 01 Nov 2023 01:04:33 GMT  
		Size: 19.9 MB (19907217 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:133196f8778a15080dd6f242c3a0bd8c162136414c80a5bda6ff50cf15234cfa`  
		Last Modified: Wed, 01 Nov 2023 01:04:32 GMT  
		Size: 97.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5035cc12125b8e0c7c3650ec19365fa2c3d1cb29a7ade2c74d5dcc614b6f05b0`  
		Last Modified: Wed, 01 Nov 2023 01:04:33 GMT  
		Size: 572.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `redis:latest` - unknown; unknown

```console
$ docker pull redis@sha256:cd971095a858f8d2132670d4f58286b76821b6fd96c2bc64785b609a94fe88c9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.2 KB (29164 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:119df0d9750a9c6e07ec883c007f051422a5ba61e5aa2d136cdfadef1345dedd`

```dockerfile
```

-	Layers:
	-	`sha256:fbe77b316ac59861b1cd70ab73af1f67320a8f00b2ecc94773cbf754a5b2ce25`  
		Last Modified: Wed, 01 Nov 2023 01:04:32 GMT  
		Size: 29.2 KB (29164 bytes)  
		MIME: application/vnd.in-toto+json

### `redis:latest` - linux; mips64le

```console
$ docker pull redis@sha256:c9aacf8a873fc3cdc52c4a52fde50fd2a1ecea1f243bb77437ecf24ea8908146
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.7 MB (50689822 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5cf6c102dc1760d1929ecc10e1a59634d699a233004e3a85d4eaad5239cf8589`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Wed, 11 Oct 2023 17:49:32 GMT
ADD file:2abda0a72972a417d4f7f530ca8fa1ee7e85e25d4015fd4e70acf903cfd96d3d in / 
# Wed, 11 Oct 2023 17:49:36 GMT
CMD ["bash"]
# Wed, 18 Oct 2023 09:03:13 GMT
RUN groupadd -r -g 999 redis && useradd -r -g redis -u 999 redis # buildkit
# Wed, 18 Oct 2023 09:03:13 GMT
ENV GOSU_VERSION=1.16
# Wed, 18 Oct 2023 09:03:13 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Wed, 18 Oct 2023 09:03:13 GMT
ENV REDIS_VERSION=7.2.2
# Wed, 18 Oct 2023 09:03:13 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-7.2.2.tar.gz
# Wed, 18 Oct 2023 09:03:13 GMT
ENV REDIS_DOWNLOAD_SHA=ca999be08800edc6d265379c4c7aafad92f0ee400692e4e2d69829ab4b4c3d08
# Wed, 18 Oct 2023 09:03:13 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				dpkg-dev 		gcc 		libc6-dev 		libssl-dev 		make 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		redis-cli --version; 	redis-server --version # buildkit
# Wed, 18 Oct 2023 09:03:13 GMT
RUN mkdir /data && chown redis:redis /data # buildkit
# Wed, 18 Oct 2023 09:03:13 GMT
VOLUME [/data]
# Wed, 18 Oct 2023 09:03:13 GMT
WORKDIR /data
# Wed, 18 Oct 2023 09:03:13 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Wed, 18 Oct 2023 09:03:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 18 Oct 2023 09:03:13 GMT
EXPOSE map[6379/tcp:{}]
# Wed, 18 Oct 2023 09:03:13 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:f11870ec99d788b4b160d9f3f4c0a79904290083d8930b26e5d13579226e07f0`  
		Last Modified: Wed, 11 Oct 2023 18:00:43 GMT  
		Size: 29.1 MB (29142026 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fbef53a2ae54aa6da8baffc9a4c14871e6dacb2590f7980ee553e2f54700a3e9`  
		Last Modified: Sat, 14 Oct 2023 06:27:28 GMT  
		Size: 1.1 KB (1101 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:260b6381008909814f5663e7a0db3e0d4bfa346c861012259cf0beb100b43e22`  
		Last Modified: Sat, 14 Oct 2023 06:27:29 GMT  
		Size: 1.3 MB (1327967 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:08b2027003d136328bfea1a6ae31831a89ec0a265089ebd8924bdc459652cfac`  
		Last Modified: Thu, 19 Oct 2023 01:07:37 GMT  
		Size: 20.2 MB (20218028 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c09247a19ae4fbed60104d023ec00fc145d9d7e822616f16222cde9c74f7dc89`  
		Last Modified: Thu, 19 Oct 2023 01:07:35 GMT  
		Size: 96.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e56c08de67a48c4116b64159f7833ca693aabaf1c81270122e85ec878b7f2c1d`  
		Last Modified: Thu, 19 Oct 2023 01:07:35 GMT  
		Size: 572.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `redis:latest` - unknown; unknown

```console
$ docker pull redis@sha256:f056326c8380f9fa14052f4105656eea3b1268ecec3ce87ade9e0f3f4d21d3ba
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.2 KB (29154 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:24494e34dfc1b929b3c26ac29d6c32cdde7c1f4bcd04fd6259c224271dd6754e`

```dockerfile
```

-	Layers:
	-	`sha256:5cd9aa07422ab490204b1c59e01f6622af66ae41aa7765a8c21bea6336b9c9cd`  
		Last Modified: Thu, 19 Oct 2023 01:07:35 GMT  
		Size: 29.2 KB (29154 bytes)  
		MIME: application/vnd.in-toto+json

### `redis:latest` - linux; ppc64le

```console
$ docker pull redis@sha256:702f7297619657f47a7a9505d6d6887f4886e6b05abd36bbf2d0e2a8ec2228af
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.4 MB (56397344 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:30de894e060ba732484b32b3fb3525b2c826d7d361c91e7952d0568cd746cbb0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Wed, 18 Oct 2023 09:03:13 GMT
ADD file:f36d600ab8508979b5763875a75f35555fa0a83d2656cbcdfa50978c6ae97353 in / 
# Wed, 18 Oct 2023 09:03:13 GMT
CMD ["bash"]
# Wed, 18 Oct 2023 09:03:13 GMT
RUN groupadd -r -g 999 redis && useradd -r -g redis -u 999 redis # buildkit
# Wed, 18 Oct 2023 09:03:13 GMT
ENV GOSU_VERSION=1.16
# Wed, 18 Oct 2023 09:03:13 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Wed, 18 Oct 2023 09:03:13 GMT
ENV REDIS_VERSION=7.2.2
# Wed, 18 Oct 2023 09:03:13 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-7.2.2.tar.gz
# Wed, 18 Oct 2023 09:03:13 GMT
ENV REDIS_DOWNLOAD_SHA=ca999be08800edc6d265379c4c7aafad92f0ee400692e4e2d69829ab4b4c3d08
# Wed, 18 Oct 2023 09:03:13 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				dpkg-dev 		gcc 		libc6-dev 		libssl-dev 		make 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		redis-cli --version; 	redis-server --version # buildkit
# Wed, 18 Oct 2023 09:03:13 GMT
RUN mkdir /data && chown redis:redis /data # buildkit
# Wed, 18 Oct 2023 09:03:13 GMT
VOLUME [/data]
# Wed, 18 Oct 2023 09:03:13 GMT
WORKDIR /data
# Wed, 18 Oct 2023 09:03:13 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Wed, 18 Oct 2023 09:03:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 18 Oct 2023 09:03:13 GMT
EXPOSE map[6379/tcp:{}]
# Wed, 18 Oct 2023 09:03:13 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:e56c8f20d7d119ff87eb044f21bfd5a4b30bf8436fc5fac12871095a6bd1517c`  
		Last Modified: Wed, 01 Nov 2023 00:26:10 GMT  
		Size: 33.1 MB (33141482 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:30eb1f390b33ba896a65663a485f84d900f33b782b5542f03dd5dcd5b0d61b90`  
		Last Modified: Thu, 02 Nov 2023 01:33:12 GMT  
		Size: 1.1 KB (1100 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:34a0412f09050ee5410e2131194a2b46a2379fcc1abd646979ee501f385f182e`  
		Last Modified: Thu, 02 Nov 2023 01:33:12 GMT  
		Size: 1.4 MB (1362564 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:53358f62636db0838dd2684249a24baec534fde40763ccd61ecf3b129331a2b1`  
		Last Modified: Thu, 02 Nov 2023 01:33:13 GMT  
		Size: 21.9 MB (21891500 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e1d6c0647cdb2fca606afe83ecd6bd8bb5941f3728e144ee76e0db222034a9e0`  
		Last Modified: Thu, 02 Nov 2023 01:33:12 GMT  
		Size: 96.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:32d7622a65af7ecd50cedd1a1c0a484a16ad2ffc47d54bfb7839c8562a2fb002`  
		Last Modified: Thu, 02 Nov 2023 01:33:13 GMT  
		Size: 570.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `redis:latest` - unknown; unknown

```console
$ docker pull redis@sha256:22dcf95546de2ad78e7f8368685b4c62fe3b908bfa8d4d526d40dccc6a97faa2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 MB (3051528 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a2e786afa2e029670dcf5532600fb61379353d3c06a2e5120f22dfc8298f2db`

```dockerfile
```

-	Layers:
	-	`sha256:d462b9f5ddb875beba700e1ed306d752a5e98dd285113be98b18e21748b40be8`  
		Last Modified: Thu, 02 Nov 2023 01:33:13 GMT  
		Size: 3.0 MB (3022193 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:a997bd5170f5d1d64b627ad4ac43e00ba4d3ae53397f34d047666b1b0a2f2aab`  
		Last Modified: Thu, 02 Nov 2023 01:33:12 GMT  
		Size: 29.3 KB (29335 bytes)  
		MIME: application/vnd.in-toto+json

### `redis:latest` - linux; s390x

```console
$ docker pull redis@sha256:90ae7d115d79d98e317bd48816776302b8acffd695090ae756f89794f7635842
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.7 MB (48725277 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:414aab32b6110392cc9ce65c450c9c19b9dbdffae735402ae910927d4647402e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Wed, 18 Oct 2023 09:03:13 GMT
ADD file:2764e93c5bba50564937cce7bcaa7c7d3bdc3fd0d53a7bb09e6955e6fda8d7c2 in / 
# Wed, 18 Oct 2023 09:03:13 GMT
CMD ["bash"]
# Wed, 18 Oct 2023 09:03:13 GMT
RUN groupadd -r -g 999 redis && useradd -r -g redis -u 999 redis # buildkit
# Wed, 18 Oct 2023 09:03:13 GMT
ENV GOSU_VERSION=1.16
# Wed, 18 Oct 2023 09:03:13 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Wed, 18 Oct 2023 09:03:13 GMT
ENV REDIS_VERSION=7.2.2
# Wed, 18 Oct 2023 09:03:13 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-7.2.2.tar.gz
# Wed, 18 Oct 2023 09:03:13 GMT
ENV REDIS_DOWNLOAD_SHA=ca999be08800edc6d265379c4c7aafad92f0ee400692e4e2d69829ab4b4c3d08
# Wed, 18 Oct 2023 09:03:13 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				dpkg-dev 		gcc 		libc6-dev 		libssl-dev 		make 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		redis-cli --version; 	redis-server --version # buildkit
# Wed, 18 Oct 2023 09:03:13 GMT
RUN mkdir /data && chown redis:redis /data # buildkit
# Wed, 18 Oct 2023 09:03:13 GMT
VOLUME [/data]
# Wed, 18 Oct 2023 09:03:13 GMT
WORKDIR /data
# Wed, 18 Oct 2023 09:03:13 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Wed, 18 Oct 2023 09:03:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 18 Oct 2023 09:03:13 GMT
EXPOSE map[6379/tcp:{}]
# Wed, 18 Oct 2023 09:03:13 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:ac72f5406002214602d5a625a21b606af78a78e99e377d3140a83021f7edd666`  
		Last Modified: Wed, 01 Nov 2023 00:48:04 GMT  
		Size: 27.5 MB (27512766 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7af95d3a845d86462fed65a7bd1cd60b7b0d1c7d7f01a60a0bcba77277dc4e49`  
		Last Modified: Wed, 01 Nov 2023 17:26:46 GMT  
		Size: 1.1 KB (1100 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8258ba0fcf28cfcf1ee5b82cfd63a1c2bfa8495a162f9686c3ad668cfcb147a2`  
		Last Modified: Wed, 01 Nov 2023 17:26:46 GMT  
		Size: 1.4 MB (1406096 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ca62a262920c5c56e1213580bf221f1188e8550ef20e393996c49686e4b544b1`  
		Last Modified: Wed, 01 Nov 2023 17:26:47 GMT  
		Size: 19.8 MB (19804614 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:37a7097930c2cc2cf953974bc5fd44dfaa3c89d786b5261002873510d906258f`  
		Last Modified: Wed, 01 Nov 2023 17:26:46 GMT  
		Size: 97.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:afbacaa51701e4429dcead6fa99dc359357e76ee3ccdec9cf6ac8950ffd341bc`  
		Last Modified: Wed, 01 Nov 2023 17:26:47 GMT  
		Size: 572.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `redis:latest` - unknown; unknown

```console
$ docker pull redis@sha256:b87e88dd7f9cbcc9f2d072b737ce1405d05c4cd024bef48459982bc5dadf5219
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 MB (3052483 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3fb93b737f902b754cf154eeeb2e7da67f7791098664ba65d8e2a5b40c1bd1e8`

```dockerfile
```

-	Layers:
	-	`sha256:bdc36d2e51037ba142f6d459ead5614d5732583ba531de5f471674a88e002e89`  
		Last Modified: Wed, 01 Nov 2023 17:26:46 GMT  
		Size: 3.0 MB (3023216 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:98b53c9e267b1ce48f6a3450f5825f95b0abeadd3ee7383bc7a79c5266417d92`  
		Last Modified: Wed, 01 Nov 2023 17:26:46 GMT  
		Size: 29.3 KB (29267 bytes)  
		MIME: application/vnd.in-toto+json
