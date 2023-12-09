## `redis:7-alpine`

```console
$ docker pull redis@sha256:98d94645f02f00518a028b75b56aef1da510b2fbbad77235f8c65da56c9cebe6
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 13
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown
	-	linux; 386
	-	unknown; unknown
	-	linux; ppc64le
	-	unknown; unknown
	-	linux; s390x
	-	unknown; unknown

### `redis:7-alpine` - linux; amd64

```console
$ docker pull redis@sha256:62c97f250e61ea79bb3f8bf9a3e40b7b2144f8d8f5d7bd19547923055914aa79
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.8 MB (16755173 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d2d4688fcebeb127fbc1e00693c3b4165ba8a02bf1e0347dd7d9ba38f6199afe`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Fri, 08 Dec 2023 01:20:49 GMT
ADD file:1f4eb46669b5b6275af19eb7471a6899a61c276aa7d925b8ae99310b14b75b92 in / 
# Fri, 08 Dec 2023 01:20:49 GMT
CMD ["/bin/sh"]
# Fri, 08 Dec 2023 04:19:49 GMT
RUN set -eux; 	addgroup -S -g 1000 redis; 	adduser -S -G redis -u 999 redis # buildkit
# Fri, 08 Dec 2023 04:19:49 GMT
RUN set -eux; 	apk add --no-cache 		tzdata 	; # buildkit
# Fri, 08 Dec 2023 04:19:49 GMT
ENV GOSU_VERSION=1.17
# Fri, 08 Dec 2023 04:19:49 GMT
RUN set -eux; 	apk add --no-cache --virtual .gosu-fetch gnupg; 	arch="$(apk --print-arch)"; 	case "$arch" in 		'x86_64') url='https://github.com/tianon/gosu/releases/download/1.17/gosu-amd64'; sha256='bbc4136d03ab138b1ad66fa4fc051bafc6cc7ffae632b069a53657279a450de3' ;; 		'aarch64') url='https://github.com/tianon/gosu/releases/download/1.17/gosu-arm64'; sha256='c3805a85d17f4454c23d7059bcb97e1ec1af272b90126e79ed002342de08389b' ;; 		'armhf') url='https://github.com/tianon/gosu/releases/download/1.17/gosu-armhf'; sha256='e5866286277ff2a2159fb9196fea13e0a59d3f1091ea46ddb985160b94b6841b' ;; 		'x86') url='https://github.com/tianon/gosu/releases/download/1.17/gosu-i386'; sha256='087dbb8fe479537e64f9c86fa49ff3b41dee1cbd28739a19aaef83dc8186b1ca' ;; 		'ppc64le') url='https://github.com/tianon/gosu/releases/download/1.17/gosu-ppc64el'; sha256='1891acdcfa70046818ab6ed3c52b9d42fa10fbb7b340eb429c8c7849691dbd76' ;; 		'riscv64') url='https://github.com/tianon/gosu/releases/download/1.17/gosu-riscv64'; sha256='38a6444b57adce135c42d5a3689f616fc7803ddc7a07ff6f946f2ebc67a26ba6' ;; 		's390x') url='https://github.com/tianon/gosu/releases/download/1.17/gosu-s390x'; sha256='69873bab588192f760547ca1f75b27cfcf106e9f7403fee6fd0600bc914979d0' ;; 		'armv7') url='https://github.com/tianon/gosu/releases/download/1.17/gosu-armhf'; sha256='e5866286277ff2a2159fb9196fea13e0a59d3f1091ea46ddb985160b94b6841b' ;; 		*) echo >&2 "error: unsupported gosu architecture: '$arch'"; exit 1 ;; 	esac; 	wget -O /usr/local/bin/gosu.asc "$url.asc"; 	wget -O /usr/local/bin/gosu "$url"; 	echo "$sha256 */usr/local/bin/gosu" | sha256sum -c -; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apk del --no-network .gosu-fetch; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Fri, 08 Dec 2023 04:19:49 GMT
ENV REDIS_VERSION=7.2.3
# Fri, 08 Dec 2023 04:19:49 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-7.2.3.tar.gz
# Fri, 08 Dec 2023 04:19:49 GMT
ENV REDIS_DOWNLOAD_SHA=3e2b196d6eb4ddb9e743088bfc2915ccbb42d40f5a8a3edd8cb69c716ec34be7
# Fri, 08 Dec 2023 04:19:49 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		dpkg-dev dpkg 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 		wget 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version; 		echo '{"spdxVersion":"SPDX-2.3","SPDXID":"SPDXRef-DOCUMENT","name":"redis-server-sbom","packages":[{"name":"redis-server","versionInfo":"7.2.3","SPDXID":"SPDXRef-Package--redis-server","externalRefs":[{"referenceCategory":"PACKAGE-MANAGER","referenceType":"purl","referenceLocator":"pkg:generic/redis-server@7.2.3?os_name=alpine&os_version=3.19"}],"licenseDeclared":"BSD-3-Clause"}]}' > /usr/local/redis.spdx.json # buildkit
# Fri, 08 Dec 2023 04:19:49 GMT
RUN mkdir /data && chown redis:redis /data # buildkit
# Fri, 08 Dec 2023 04:19:49 GMT
VOLUME [/data]
# Fri, 08 Dec 2023 04:19:49 GMT
WORKDIR /data
# Fri, 08 Dec 2023 04:19:49 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Fri, 08 Dec 2023 04:19:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 08 Dec 2023 04:19:49 GMT
EXPOSE map[6379/tcp:{}]
# Fri, 08 Dec 2023 04:19:49 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:661ff4d9561e3fd050929ee5097067c34bafc523ee60f5294a37fd08056a73ca`  
		Last Modified: Fri, 08 Dec 2023 01:21:10 GMT  
		Size: 3.4 MB (3408480 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:963a98d2b6c2b2c83b3eaaf5753aa5983decc8c29cdd6fbfecb93dc9bcc90472`  
		Last Modified: Fri, 08 Dec 2023 20:12:01 GMT  
		Size: 1.2 KB (1242 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:dddcc6acb2edad879c0c36d968f2469d8f0ee881451258667e250552367cfed6`  
		Last Modified: Fri, 08 Dec 2023 20:12:01 GMT  
		Size: 345.0 KB (344953 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ff0ac71727e765cea4fc55ed7cada0db3dd40341bd7a0cbc615b79bf77fe0040`  
		Last Modified: Fri, 08 Dec 2023 20:12:01 GMT  
		Size: 1.0 MB (1015367 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7959e5ad61f461d5bbf7f2677604a49e644774f4d3bf938c32508f74690d30ee`  
		Last Modified: Fri, 08 Dec 2023 20:12:02 GMT  
		Size: 12.0 MB (11984432 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d767cfa2fc0916b08c0d72ecf5cc9fca421b5b8f61a231e70d9eaf8d34928f0d`  
		Last Modified: Fri, 08 Dec 2023 20:12:02 GMT  
		Size: 100.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:64281ae03186c6cf997878818b85ca7398e3216c2f583729eca871f5bcc63393`  
		Last Modified: Fri, 08 Dec 2023 20:12:02 GMT  
		Size: 567.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `redis:7-alpine` - unknown; unknown

```console
$ docker pull redis@sha256:e23f860aa56bdd6dd3466382000c4182429d9972c7269d58775bd908bba95a51
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **728.6 KB (728583 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:79e5829646acb698ce3a7bb587a054d813bcf33882f4937311880dcbf6178dea`

```dockerfile
```

-	Layers:
	-	`sha256:c58b9936fc9698f6bb25f629b5d5a3732ea8cc714af36537dc893b12d5c1f86f`  
		Last Modified: Fri, 08 Dec 2023 20:12:01 GMT  
		Size: 693.2 KB (693171 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:a1589fab3d087c5f0f5016144b04d761fb5de738b234170809e9092dda42bd54`  
		Last Modified: Fri, 08 Dec 2023 20:12:01 GMT  
		Size: 35.4 KB (35412 bytes)  
		MIME: application/vnd.in-toto+json

### `redis:7-alpine` - linux; arm variant v6

```console
$ docker pull redis@sha256:cfb3c5629ec846b1665d348f8c82ed160c911cab5a2cc88053f4219ab4b5835c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.7 MB (16656349 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dac73fd681d89123dbc6c97cd74ae86d296e9cb81a0ce64f69821ce659e43a33`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Fri, 08 Dec 2023 01:49:15 GMT
ADD file:d43ed267a41631ce0e5a4ef5aac821a75300a83f85ecb6259f5616852f89e989 in / 
# Fri, 08 Dec 2023 01:49:15 GMT
CMD ["/bin/sh"]
# Fri, 08 Dec 2023 04:19:49 GMT
RUN set -eux; 	addgroup -S -g 1000 redis; 	adduser -S -G redis -u 999 redis # buildkit
# Fri, 08 Dec 2023 04:19:49 GMT
RUN set -eux; 	apk add --no-cache 		tzdata 	; # buildkit
# Fri, 08 Dec 2023 04:19:49 GMT
ENV GOSU_VERSION=1.17
# Fri, 08 Dec 2023 04:19:49 GMT
RUN set -eux; 	apk add --no-cache --virtual .gosu-fetch gnupg; 	arch="$(apk --print-arch)"; 	case "$arch" in 		'x86_64') url='https://github.com/tianon/gosu/releases/download/1.17/gosu-amd64'; sha256='bbc4136d03ab138b1ad66fa4fc051bafc6cc7ffae632b069a53657279a450de3' ;; 		'aarch64') url='https://github.com/tianon/gosu/releases/download/1.17/gosu-arm64'; sha256='c3805a85d17f4454c23d7059bcb97e1ec1af272b90126e79ed002342de08389b' ;; 		'armhf') url='https://github.com/tianon/gosu/releases/download/1.17/gosu-armhf'; sha256='e5866286277ff2a2159fb9196fea13e0a59d3f1091ea46ddb985160b94b6841b' ;; 		'x86') url='https://github.com/tianon/gosu/releases/download/1.17/gosu-i386'; sha256='087dbb8fe479537e64f9c86fa49ff3b41dee1cbd28739a19aaef83dc8186b1ca' ;; 		'ppc64le') url='https://github.com/tianon/gosu/releases/download/1.17/gosu-ppc64el'; sha256='1891acdcfa70046818ab6ed3c52b9d42fa10fbb7b340eb429c8c7849691dbd76' ;; 		'riscv64') url='https://github.com/tianon/gosu/releases/download/1.17/gosu-riscv64'; sha256='38a6444b57adce135c42d5a3689f616fc7803ddc7a07ff6f946f2ebc67a26ba6' ;; 		's390x') url='https://github.com/tianon/gosu/releases/download/1.17/gosu-s390x'; sha256='69873bab588192f760547ca1f75b27cfcf106e9f7403fee6fd0600bc914979d0' ;; 		'armv7') url='https://github.com/tianon/gosu/releases/download/1.17/gosu-armhf'; sha256='e5866286277ff2a2159fb9196fea13e0a59d3f1091ea46ddb985160b94b6841b' ;; 		*) echo >&2 "error: unsupported gosu architecture: '$arch'"; exit 1 ;; 	esac; 	wget -O /usr/local/bin/gosu.asc "$url.asc"; 	wget -O /usr/local/bin/gosu "$url"; 	echo "$sha256 */usr/local/bin/gosu" | sha256sum -c -; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apk del --no-network .gosu-fetch; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Fri, 08 Dec 2023 04:19:49 GMT
ENV REDIS_VERSION=7.2.3
# Fri, 08 Dec 2023 04:19:49 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-7.2.3.tar.gz
# Fri, 08 Dec 2023 04:19:49 GMT
ENV REDIS_DOWNLOAD_SHA=3e2b196d6eb4ddb9e743088bfc2915ccbb42d40f5a8a3edd8cb69c716ec34be7
# Fri, 08 Dec 2023 04:19:49 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		dpkg-dev dpkg 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 		wget 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version; 		echo '{"spdxVersion":"SPDX-2.3","SPDXID":"SPDXRef-DOCUMENT","name":"redis-server-sbom","packages":[{"name":"redis-server","versionInfo":"7.2.3","SPDXID":"SPDXRef-Package--redis-server","externalRefs":[{"referenceCategory":"PACKAGE-MANAGER","referenceType":"purl","referenceLocator":"pkg:generic/redis-server@7.2.3?os_name=alpine&os_version=3.19"}],"licenseDeclared":"BSD-3-Clause"}]}' > /usr/local/redis.spdx.json # buildkit
# Fri, 08 Dec 2023 04:19:49 GMT
RUN mkdir /data && chown redis:redis /data # buildkit
# Fri, 08 Dec 2023 04:19:49 GMT
VOLUME [/data]
# Fri, 08 Dec 2023 04:19:49 GMT
WORKDIR /data
# Fri, 08 Dec 2023 04:19:49 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Fri, 08 Dec 2023 04:19:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 08 Dec 2023 04:19:49 GMT
EXPOSE map[6379/tcp:{}]
# Fri, 08 Dec 2023 04:19:49 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:0803c38384d9fd0f9afaec8fd13d267547b660dcd46bb92a3d63c5d76e78b04c`  
		Last Modified: Fri, 08 Dec 2023 01:49:33 GMT  
		Size: 3.2 MB (3165143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15513cd9cea097c1921c9f08e8fac00098368ba235b464628834dfc302fb8ae7`  
		Last Modified: Fri, 08 Dec 2023 21:43:26 GMT  
		Size: 1.2 KB (1243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96a53b50774dc0da01401e192404fea5dcc1e19182aa7b55ca2e2720e74a9ec4`  
		Last Modified: Fri, 08 Dec 2023 21:43:24 GMT  
		Size: 345.0 KB (344964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5268407b1c98a778587e2afabab3573fc54108f90e060fcb1b1c0428ade07d9c`  
		Last Modified: Fri, 08 Dec 2023 21:43:24 GMT  
		Size: 981.7 KB (981726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3eae0a77d69485f28a6cdf718c0703a604e4b07648327eafa29b4b87cc8aca9`  
		Last Modified: Fri, 08 Dec 2023 21:43:26 GMT  
		Size: 12.2 MB (12162574 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:011b6a418792eb6f5ed6c497a0d82e282037984f56a69a90425de4677229b263`  
		Last Modified: Fri, 08 Dec 2023 21:43:24 GMT  
		Size: 101.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de813acd1ea15d98c5b8ea4c1e4c8f330541f8b0ab219b548425f53c9619673f`  
		Last Modified: Fri, 08 Dec 2023 21:43:24 GMT  
		Size: 566.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:7-alpine` - linux; arm variant v7

```console
$ docker pull redis@sha256:b0b8f54fcdc7c6e686189b7004f17cb04f7924496a0c1b3ba1dc54b5946ffb62
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.1 MB (15139650 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d0209ff74ef8a459089300d73037501e292b8756a6ba5a6110b5b6fd694a8f36`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Fri, 10 Nov 2023 15:23:15 GMT
ADD file:dcb85d43d1fb96861612c42288878b13debfa9d0b956adea1f2472d0c50f0144 in / 
# Fri, 10 Nov 2023 15:23:15 GMT
CMD ["/bin/sh"]
# Fri, 10 Nov 2023 15:23:15 GMT
RUN addgroup -S -g 1000 redis && adduser -S -G redis -u 999 redis # buildkit
# Fri, 10 Nov 2023 15:23:15 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		tzdata # buildkit
# Fri, 10 Nov 2023 15:23:15 GMT
ENV REDIS_VERSION=7.2.3
# Fri, 10 Nov 2023 15:23:15 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-7.2.3.tar.gz
# Fri, 10 Nov 2023 15:23:15 GMT
ENV REDIS_DOWNLOAD_SHA=3e2b196d6eb4ddb9e743088bfc2915ccbb42d40f5a8a3edd8cb69c716ec34be7
# Fri, 10 Nov 2023 15:23:15 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		dpkg-dev dpkg 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 		wget 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version; 		echo '{"spdxVersion":"SPDX-2.3","SPDXID":"SPDXRef-DOCUMENT","name":"redis-server-sbom","packages":[{"name":"redis-server","versionInfo":"7.2.3","SPDXID":"SPDXRef-Package--redis-server","externalRefs":[{"referenceCategory":"PACKAGE-MANAGER","referenceType":"purl","referenceLocator":"pkg:generic/redis-server@7.2.3?os_name=alpine&os_version=3.18"}],"licenseDeclared":"BSD-3-Clause"}]}' > /usr/local/redis.spdx.json # buildkit
# Fri, 10 Nov 2023 15:23:15 GMT
RUN mkdir /data && chown redis:redis /data # buildkit
# Fri, 10 Nov 2023 15:23:15 GMT
VOLUME [/data]
# Fri, 10 Nov 2023 15:23:15 GMT
WORKDIR /data
# Fri, 10 Nov 2023 15:23:15 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Fri, 10 Nov 2023 15:23:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 10 Nov 2023 15:23:15 GMT
EXPOSE map[6379/tcp:{}]
# Fri, 10 Nov 2023 15:23:15 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:2387a44129d2147bd4e806bf369f3db92eb3ad3b6b8825c739db364b8baa4e26`  
		Last Modified: Thu, 30 Nov 2023 22:49:56 GMT  
		Size: 2.9 MB (2901006 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1506ef5fd24d7f718f4fe36a0f415b1813ab739f8b6f4980aef5dd6b52b2baa1`  
		Last Modified: Fri, 01 Dec 2023 11:53:20 GMT  
		Size: 1.2 KB (1244 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:62980244a675df70d66eb7e32695d7de4f436510ed34e29439cdd35eef6999e5`  
		Last Modified: Fri, 01 Dec 2023 11:53:20 GMT  
		Size: 347.0 KB (346973 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:df3245056ee1029b3b70d4a1f27e6cb76fe146f749320e64c22d0bc4d33c5602`  
		Last Modified: Fri, 01 Dec 2023 11:53:21 GMT  
		Size: 11.9 MB (11889728 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a79ecc406e4a689c89463f4a9224a7820979aaecb243cd361fec508a7653f611`  
		Last Modified: Fri, 01 Dec 2023 11:53:20 GMT  
		Size: 100.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3495f10b62b30a6429ee06f159defbb1cc18d18bd727c618200ea14c5d4b77a6`  
		Last Modified: Fri, 01 Dec 2023 11:53:21 GMT  
		Size: 567.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `redis:7-alpine` - unknown; unknown

```console
$ docker pull redis@sha256:bf706ae317812c49cb69b41160466eb39860323f771077fde345c7e930095634
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **720.6 KB (720584 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c03f09c520ef78e3fe7d60193d0013bfcb1188a816af897c491009338831c727`

```dockerfile
```

-	Layers:
	-	`sha256:89c587f254613a7f67d3c509199e8c9a6f0d7b79ad757e4b8b4b310d0e3f013d`  
		Last Modified: Fri, 01 Dec 2023 11:53:21 GMT  
		Size: 693.1 KB (693074 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:d6cdc4d1e363b3436290090146d5cbe2b2bc52700867d332e976557bd6777229`  
		Last Modified: Fri, 01 Dec 2023 11:53:20 GMT  
		Size: 27.5 KB (27510 bytes)  
		MIME: application/vnd.in-toto+json

### `redis:7-alpine` - linux; arm64 variant v8

```console
$ docker pull redis@sha256:fbda7c40d869d69ca7ac681e0e5fb5c28a463d657ef4ed4cecdfec559ae26b03
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.7 MB (15727649 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ea03d063dd7b859715f21f0e1074d53a9d1b415527aee69607845f4e4dbf90d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Fri, 10 Nov 2023 15:23:15 GMT
ADD file:d8a30995bbcd627f084912c728fda5483b6ba486de25af588a0956069d0bd7ad in / 
# Fri, 10 Nov 2023 15:23:15 GMT
CMD ["/bin/sh"]
# Fri, 10 Nov 2023 15:23:15 GMT
RUN addgroup -S -g 1000 redis && adduser -S -G redis -u 999 redis # buildkit
# Fri, 10 Nov 2023 15:23:15 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		tzdata # buildkit
# Fri, 10 Nov 2023 15:23:15 GMT
ENV REDIS_VERSION=7.2.3
# Fri, 10 Nov 2023 15:23:15 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-7.2.3.tar.gz
# Fri, 10 Nov 2023 15:23:15 GMT
ENV REDIS_DOWNLOAD_SHA=3e2b196d6eb4ddb9e743088bfc2915ccbb42d40f5a8a3edd8cb69c716ec34be7
# Fri, 10 Nov 2023 15:23:15 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		dpkg-dev dpkg 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 		wget 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version; 		echo '{"spdxVersion":"SPDX-2.3","SPDXID":"SPDXRef-DOCUMENT","name":"redis-server-sbom","packages":[{"name":"redis-server","versionInfo":"7.2.3","SPDXID":"SPDXRef-Package--redis-server","externalRefs":[{"referenceCategory":"PACKAGE-MANAGER","referenceType":"purl","referenceLocator":"pkg:generic/redis-server@7.2.3?os_name=alpine&os_version=3.18"}],"licenseDeclared":"BSD-3-Clause"}]}' > /usr/local/redis.spdx.json # buildkit
# Fri, 10 Nov 2023 15:23:15 GMT
RUN mkdir /data && chown redis:redis /data # buildkit
# Fri, 10 Nov 2023 15:23:15 GMT
VOLUME [/data]
# Fri, 10 Nov 2023 15:23:15 GMT
WORKDIR /data
# Fri, 10 Nov 2023 15:23:15 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Fri, 10 Nov 2023 15:23:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 10 Nov 2023 15:23:15 GMT
EXPOSE map[6379/tcp:{}]
# Fri, 10 Nov 2023 15:23:15 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:2c03dbb20264f09924f9eab176da44e5421e74a78b09531d3c63448a7baa7c59`  
		Last Modified: Thu, 30 Nov 2023 23:11:32 GMT  
		Size: 3.3 MB (3333033 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4a7bf3ed1ee186dc3229ea97c5f0545f1cc1718eda6c13471069fcc133849b48`  
		Last Modified: Fri, 01 Dec 2023 14:23:03 GMT  
		Size: 1.2 KB (1245 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4d3fbcb2e10941e55233f69384bbd3ab1a6f88a75f1a652d592cf0207888b073`  
		Last Modified: Fri, 01 Dec 2023 14:23:05 GMT  
		Size: 347.6 KB (347594 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:936f93d9ec245419a1026b98fd09b35a2ea688d22c86df146452a8b00f0caced`  
		Last Modified: Fri, 01 Dec 2023 14:23:04 GMT  
		Size: 12.0 MB (12045077 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3f6cc7bdb77ba0584f33de52987c03bc9a9f5964978810204e4690b2795f49c5`  
		Last Modified: Fri, 01 Dec 2023 14:23:03 GMT  
		Size: 100.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8cabe57d2142b06761291e4be31ce3e2b17ab6b49b31bbe083039de9e4805652`  
		Last Modified: Fri, 01 Dec 2023 14:23:05 GMT  
		Size: 568.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `redis:7-alpine` - unknown; unknown

```console
$ docker pull redis@sha256:30af35b69617ae087214d58ddd181920048d8db8b81c434440ed17ad15678dad
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **717.9 KB (717936 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:28b6131c20dfd362b4bce0f006194fdde7df39668c7e4d65c73d838e73d6b19e`

```dockerfile
```

-	Layers:
	-	`sha256:f62697bf17be17674870f65948eeb7429710ff4afe3d106f37dd2b5ee5a4633c`  
		Last Modified: Fri, 01 Dec 2023 14:23:04 GMT  
		Size: 690.5 KB (690549 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:866743621556a61e803bb30ee845cee214e8189cf7dfd9438c6ac7e556b10f12`  
		Last Modified: Fri, 01 Dec 2023 14:23:03 GMT  
		Size: 27.4 KB (27387 bytes)  
		MIME: application/vnd.in-toto+json

### `redis:7-alpine` - linux; 386

```console
$ docker pull redis@sha256:aa9dc6761b6f8f71796b2ce3700d48472d2ab8a5494a2ff22dc7a0d90d77144e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.4 MB (17371869 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e3f7fd026f58a172e1cdb492b5e35f3779b8c93f93c88dff88083dc3503fe53`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Thu, 28 Sep 2023 20:38:19 GMT
ADD file:8402753f294e403e92353bd65c86a6428c960be5116c0a15484b663a84f66fcd in / 
# Thu, 28 Sep 2023 20:38:20 GMT
CMD ["/bin/sh"]
# Wed, 01 Nov 2023 16:56:23 GMT
RUN addgroup -S -g 1000 redis && adduser -S -G redis -u 999 redis # buildkit
# Wed, 01 Nov 2023 16:56:23 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		tzdata # buildkit
# Wed, 01 Nov 2023 16:56:23 GMT
ENV REDIS_VERSION=7.2.3
# Wed, 01 Nov 2023 16:56:23 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-7.2.3.tar.gz
# Wed, 01 Nov 2023 16:56:23 GMT
ENV REDIS_DOWNLOAD_SHA=3e2b196d6eb4ddb9e743088bfc2915ccbb42d40f5a8a3edd8cb69c716ec34be7
# Wed, 01 Nov 2023 16:56:23 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		dpkg-dev dpkg 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 		wget 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version # buildkit
# Wed, 01 Nov 2023 16:56:23 GMT
RUN mkdir /data && chown redis:redis /data # buildkit
# Wed, 01 Nov 2023 16:56:23 GMT
VOLUME [/data]
# Wed, 01 Nov 2023 16:56:23 GMT
WORKDIR /data
# Wed, 01 Nov 2023 16:56:23 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Wed, 01 Nov 2023 16:56:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Nov 2023 16:56:23 GMT
EXPOSE map[6379/tcp:{}]
# Wed, 01 Nov 2023 16:56:23 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:dc95107ad2a031a015320bb397f73ec151d738127175b31ad643120697dc7e90`  
		Last Modified: Thu, 28 Sep 2023 20:39:32 GMT  
		Size: 3.2 MB (3235757 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:10ba638cd9c74c2570d6e68edb4d19831d4c65064424f614e651fe60d12850c5`  
		Last Modified: Sat, 04 Nov 2023 00:03:19 GMT  
		Size: 1.2 KB (1243 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:dfdec2761f7c9b3d7ab9c0de9990ee8cc6794a57c8e2ca5ee47143c57c32a5ca`  
		Last Modified: Sat, 04 Nov 2023 00:03:19 GMT  
		Size: 347.4 KB (347384 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e9d58bc8b6ecb0e5cf9dfa04905f8813d211ebdb5b4905f44a43f989e87c27e2`  
		Last Modified: Sat, 04 Nov 2023 00:03:20 GMT  
		Size: 13.8 MB (13786777 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fc4b2d08907cb2d39691f9ade7907ac921a9e1c53e836947684f1eb59d2d7dc7`  
		Last Modified: Sat, 04 Nov 2023 00:03:19 GMT  
		Size: 100.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c0806d930b0b74b0f7a58593c281d48cb8d3307d50bb094ed21c06b1bd2720fb`  
		Last Modified: Sat, 04 Nov 2023 00:03:20 GMT  
		Size: 576.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `redis:7-alpine` - unknown; unknown

```console
$ docker pull redis@sha256:e9054dfb62b0f41f88a18627bdbf3396fe1653adfec9990fab8f26bfed3da465
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.1 KB (26146 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:79f149987d135976df961ee2f0c1d47ecd9af2782025f4343d8a21b47897fa32`

```dockerfile
```

-	Layers:
	-	`sha256:612873743f62d6da907754c1af029c9fe3043a84304761780847b5b894fe1023`  
		Last Modified: Sat, 04 Nov 2023 00:03:18 GMT  
		Size: 26.1 KB (26146 bytes)  
		MIME: application/vnd.in-toto+json

### `redis:7-alpine` - linux; ppc64le

```console
$ docker pull redis@sha256:03156658d164dd3c5522819c9ed5738da641947a1a2cbb6ce9bfd3a23fc33105
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.4 MB (16444761 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19c9a03b1afda99f72adbbd0977901ff287a12636583cdc3ce1af41e72241667`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Fri, 10 Nov 2023 15:23:15 GMT
ADD file:3450a1687b552498a987f87cb844b7f597c7181d7c3d31943d7b3036d5300d5e in / 
# Fri, 10 Nov 2023 15:23:15 GMT
CMD ["/bin/sh"]
# Fri, 10 Nov 2023 15:23:15 GMT
RUN addgroup -S -g 1000 redis && adduser -S -G redis -u 999 redis # buildkit
# Fri, 10 Nov 2023 15:23:15 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		tzdata # buildkit
# Fri, 10 Nov 2023 15:23:15 GMT
ENV REDIS_VERSION=7.2.3
# Fri, 10 Nov 2023 15:23:15 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-7.2.3.tar.gz
# Fri, 10 Nov 2023 15:23:15 GMT
ENV REDIS_DOWNLOAD_SHA=3e2b196d6eb4ddb9e743088bfc2915ccbb42d40f5a8a3edd8cb69c716ec34be7
# Fri, 10 Nov 2023 15:23:15 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		dpkg-dev dpkg 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 		wget 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version; 		echo '{"spdxVersion":"SPDX-2.3","SPDXID":"SPDXRef-DOCUMENT","name":"redis-server-sbom","packages":[{"name":"redis-server","versionInfo":"7.2.3","SPDXID":"SPDXRef-Package--redis-server","externalRefs":[{"referenceCategory":"PACKAGE-MANAGER","referenceType":"purl","referenceLocator":"pkg:generic/redis-server@7.2.3?os_name=alpine&os_version=3.18"}],"licenseDeclared":"BSD-3-Clause"}]}' > /usr/local/redis.spdx.json # buildkit
# Fri, 10 Nov 2023 15:23:15 GMT
RUN mkdir /data && chown redis:redis /data # buildkit
# Fri, 10 Nov 2023 15:23:15 GMT
VOLUME [/data]
# Fri, 10 Nov 2023 15:23:15 GMT
WORKDIR /data
# Fri, 10 Nov 2023 15:23:15 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Fri, 10 Nov 2023 15:23:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 10 Nov 2023 15:23:15 GMT
EXPOSE map[6379/tcp:{}]
# Fri, 10 Nov 2023 15:23:15 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:4e13780adf2776477b14ef9c0f4f563f820a2fde166d472218037b979e84d31a`  
		Last Modified: Thu, 30 Nov 2023 23:20:01 GMT  
		Size: 3.3 MB (3348322 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:22d838ff435f29e2ab4eac4b792b25be0ed7646e56a1e0123ef076df6a24d5f7`  
		Last Modified: Fri, 01 Dec 2023 13:00:58 GMT  
		Size: 1.2 KB (1245 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8e5c9eca873bc348a1c5e4a07292eb197e0d824e0b6f759acf6e637aaa4246e2`  
		Last Modified: Fri, 01 Dec 2023 13:00:58 GMT  
		Size: 347.7 KB (347655 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:116c7351cccd52cb84e8bf8610ae9355c056834ea9e85f4d5655d50b84660fad`  
		Last Modified: Fri, 01 Dec 2023 13:00:59 GMT  
		Size: 12.7 MB (12746835 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d03ef4ddb3be99c5dea2a9f3b45303dc9a61918f8825096c27ea94f5590e9591`  
		Last Modified: Fri, 01 Dec 2023 13:00:58 GMT  
		Size: 101.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:398db60f320004b73a75adf42b944acb5f19156f0d4eb247b5fd353a333b386d`  
		Last Modified: Fri, 01 Dec 2023 13:00:59 GMT  
		Size: 571.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `redis:7-alpine` - unknown; unknown

```console
$ docker pull redis@sha256:89c1f07ff6debf9997d252dd52809bf257f6e050bf1f7269eebe08d8a1397fc3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **716.4 KB (716389 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a1f508d3ef66e266b8f916812e95b5cd6eef66004a0c5ea885630e29b04b978e`

```dockerfile
```

-	Layers:
	-	`sha256:b815684fdc23cc967713b39fb391239e8f55b2f75f6a0056809085523d014895`  
		Last Modified: Fri, 01 Dec 2023 13:00:58 GMT  
		Size: 689.0 KB (688952 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:ffd2637a1a5d46934f8ee9536ed6522e22b014527d40accb3f53e9afd202a1b1`  
		Last Modified: Fri, 01 Dec 2023 13:00:58 GMT  
		Size: 27.4 KB (27437 bytes)  
		MIME: application/vnd.in-toto+json

### `redis:7-alpine` - linux; s390x

```console
$ docker pull redis@sha256:0bf196ac5a8859218ad80f232fee462e9a7c4ba3671e092840c5d9969363fa01
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.1 MB (17115770 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7bb15e8275d08450942b02190955b9cf3d1f78dc6bc9d290fe273d35937512a4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Fri, 08 Dec 2023 01:41:50 GMT
ADD file:47e0982fc3ae485c06d46f3c0022afd39ed7ec95fe755c2391e6b0cfcae65dfc in / 
# Fri, 08 Dec 2023 01:41:51 GMT
CMD ["/bin/sh"]
# Fri, 08 Dec 2023 04:19:49 GMT
RUN set -eux; 	addgroup -S -g 1000 redis; 	adduser -S -G redis -u 999 redis # buildkit
# Fri, 08 Dec 2023 04:19:49 GMT
RUN set -eux; 	apk add --no-cache 		tzdata 	; # buildkit
# Fri, 08 Dec 2023 04:19:49 GMT
ENV GOSU_VERSION=1.17
# Fri, 08 Dec 2023 04:19:49 GMT
RUN set -eux; 	apk add --no-cache --virtual .gosu-fetch gnupg; 	arch="$(apk --print-arch)"; 	case "$arch" in 		'x86_64') url='https://github.com/tianon/gosu/releases/download/1.17/gosu-amd64'; sha256='bbc4136d03ab138b1ad66fa4fc051bafc6cc7ffae632b069a53657279a450de3' ;; 		'aarch64') url='https://github.com/tianon/gosu/releases/download/1.17/gosu-arm64'; sha256='c3805a85d17f4454c23d7059bcb97e1ec1af272b90126e79ed002342de08389b' ;; 		'armhf') url='https://github.com/tianon/gosu/releases/download/1.17/gosu-armhf'; sha256='e5866286277ff2a2159fb9196fea13e0a59d3f1091ea46ddb985160b94b6841b' ;; 		'x86') url='https://github.com/tianon/gosu/releases/download/1.17/gosu-i386'; sha256='087dbb8fe479537e64f9c86fa49ff3b41dee1cbd28739a19aaef83dc8186b1ca' ;; 		'ppc64le') url='https://github.com/tianon/gosu/releases/download/1.17/gosu-ppc64el'; sha256='1891acdcfa70046818ab6ed3c52b9d42fa10fbb7b340eb429c8c7849691dbd76' ;; 		'riscv64') url='https://github.com/tianon/gosu/releases/download/1.17/gosu-riscv64'; sha256='38a6444b57adce135c42d5a3689f616fc7803ddc7a07ff6f946f2ebc67a26ba6' ;; 		's390x') url='https://github.com/tianon/gosu/releases/download/1.17/gosu-s390x'; sha256='69873bab588192f760547ca1f75b27cfcf106e9f7403fee6fd0600bc914979d0' ;; 		'armv7') url='https://github.com/tianon/gosu/releases/download/1.17/gosu-armhf'; sha256='e5866286277ff2a2159fb9196fea13e0a59d3f1091ea46ddb985160b94b6841b' ;; 		*) echo >&2 "error: unsupported gosu architecture: '$arch'"; exit 1 ;; 	esac; 	wget -O /usr/local/bin/gosu.asc "$url.asc"; 	wget -O /usr/local/bin/gosu "$url"; 	echo "$sha256 */usr/local/bin/gosu" | sha256sum -c -; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apk del --no-network .gosu-fetch; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Fri, 08 Dec 2023 04:19:49 GMT
ENV REDIS_VERSION=7.2.3
# Fri, 08 Dec 2023 04:19:49 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-7.2.3.tar.gz
# Fri, 08 Dec 2023 04:19:49 GMT
ENV REDIS_DOWNLOAD_SHA=3e2b196d6eb4ddb9e743088bfc2915ccbb42d40f5a8a3edd8cb69c716ec34be7
# Fri, 08 Dec 2023 04:19:49 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		dpkg-dev dpkg 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 		wget 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version; 		echo '{"spdxVersion":"SPDX-2.3","SPDXID":"SPDXRef-DOCUMENT","name":"redis-server-sbom","packages":[{"name":"redis-server","versionInfo":"7.2.3","SPDXID":"SPDXRef-Package--redis-server","externalRefs":[{"referenceCategory":"PACKAGE-MANAGER","referenceType":"purl","referenceLocator":"pkg:generic/redis-server@7.2.3?os_name=alpine&os_version=3.19"}],"licenseDeclared":"BSD-3-Clause"}]}' > /usr/local/redis.spdx.json # buildkit
# Fri, 08 Dec 2023 04:19:49 GMT
RUN mkdir /data && chown redis:redis /data # buildkit
# Fri, 08 Dec 2023 04:19:49 GMT
VOLUME [/data]
# Fri, 08 Dec 2023 04:19:49 GMT
WORKDIR /data
# Fri, 08 Dec 2023 04:19:49 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Fri, 08 Dec 2023 04:19:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 08 Dec 2023 04:19:49 GMT
EXPOSE map[6379/tcp:{}]
# Fri, 08 Dec 2023 04:19:49 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:0fca3ee44ced87b7184bc23390283fdf10cfae0e844a25b785dd11c463815227`  
		Last Modified: Fri, 08 Dec 2023 01:42:30 GMT  
		Size: 3.2 MB (3242332 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9965d4e9f11aaf54ddc8f41acf2e021fd00ce3476ec31607febca7112f51c655`  
		Last Modified: Fri, 08 Dec 2023 22:32:36 GMT  
		Size: 1.2 KB (1242 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a3cbd28413e82f02a4c81d1afc99a2d1d5f21c96af1bf30306c93012f22a6b31`  
		Last Modified: Fri, 08 Dec 2023 22:32:36 GMT  
		Size: 345.0 KB (344960 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4d416124e22a7946a00399ac2e14731c1516c0320893c15e0178b17271453cf5`  
		Last Modified: Fri, 08 Dec 2023 22:32:36 GMT  
		Size: 979.0 KB (978996 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9e939d6cebb582ca66bc72afc66f8059903911d6e548ae9ff3aa0f3b2c2ddd8f`  
		Last Modified: Fri, 08 Dec 2023 22:32:37 GMT  
		Size: 12.5 MB (12547534 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2ce333b4abe63b4ecb44278e44427e94a8034d9d1f3486d000d5d77b0ebdc597`  
		Last Modified: Fri, 08 Dec 2023 22:32:37 GMT  
		Size: 101.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:32b50326564b1e422dde8db6cf3b775a35d225d6671f479a729c20cf0dc02112`  
		Last Modified: Fri, 08 Dec 2023 22:32:37 GMT  
		Size: 573.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `redis:7-alpine` - unknown; unknown

```console
$ docker pull redis@sha256:c54c01a0124ff08591634ce3911916e7b9f04e68f7205cd2373b22ef7d3f2a9f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **726.9 KB (726942 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cfc64898716c2e327a885872e767b038dff787e7a5bc1c7aac5dc5b42416a8ad`

```dockerfile
```

-	Layers:
	-	`sha256:24645707093311145ad0d3fbce15cc7e010189753416c5890b70f401b79d188a`  
		Last Modified: Fri, 08 Dec 2023 22:32:36 GMT  
		Size: 691.5 KB (691535 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:56aa60b10fde834710a8684d263c2e14f9249934badcaeeb5489a326d7fb78e0`  
		Last Modified: Fri, 08 Dec 2023 22:32:36 GMT  
		Size: 35.4 KB (35407 bytes)  
		MIME: application/vnd.in-toto+json
