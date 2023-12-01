## `redis:6-alpine3.18`

```console
$ docker pull redis@sha256:60e49e22fa5706cd8df7d5e0bc50ee9bab7c608039fa653c4d961014237cca46
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

### `redis:6-alpine3.18` - linux; amd64

```console
$ docker pull redis@sha256:5a681a870b0bf72958b46b27e60c7d61910e202024118258ea5d9dcc0c49eb0b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **11.3 MB (11280442 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b02069be932b500874a253ffc86d508b3d9301bfded6eab9645a4ae9d958cad`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Fri, 10 Nov 2023 15:23:15 GMT
ADD file:fc714080c3bcbbce7ac746a10d7b4355ffa36293a8d435d62cd5359ea8eb8364 in / 
# Fri, 10 Nov 2023 15:23:15 GMT
CMD ["/bin/sh"]
# Fri, 10 Nov 2023 15:23:15 GMT
RUN addgroup -S -g 1000 redis && adduser -S -G redis -u 999 redis # buildkit
# Fri, 10 Nov 2023 15:23:15 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		tzdata # buildkit
# Fri, 10 Nov 2023 15:23:15 GMT
ENV REDIS_VERSION=6.2.14
# Fri, 10 Nov 2023 15:23:15 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-6.2.14.tar.gz
# Fri, 10 Nov 2023 15:23:15 GMT
ENV REDIS_DOWNLOAD_SHA=34e74856cbd66fdb3a684fb349d93961d8c7aa668b06f81fd93ff267d09bc277
# Fri, 10 Nov 2023 15:23:15 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		dpkg-dev dpkg 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 		wget 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version; 		echo '{"spdxVersion":"SPDX-2.3","SPDXID":"SPDXRef-DOCUMENT","name":"redis-server-sbom","packages":[{"name":"redis-server","versionInfo":"6.2.14","SPDXID":"SPDXRef-Package--redis-server","externalRefs":[{"referenceCategory":"PACKAGE-MANAGER","referenceType":"purl","referenceLocator":"pkg:generic/redis-server@6.2.14?os_name=alpine&os_version=3.18"}],"licenseDeclared":"BSD-3-Clause"}]}' > /usr/local/redis.spdx.json # buildkit
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
	-	`sha256:c926b61bad3b94ae7351bafd0c184c159ebf0643b085f7ef1d47ecdc7316833c`  
		Last Modified: Thu, 30 Nov 2023 23:23:28 GMT  
		Size: 3.4 MB (3402422 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:67913ae4fda9ca61c1158afce45d1c535a4b24dcaf0e57e87d1218220074fee3`  
		Last Modified: Fri, 01 Dec 2023 00:11:35 GMT  
		Size: 1.2 KB (1244 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:990d91781c91a72dfce8edd9c4d2997c1df742924df2b237e430687b79b92ba6`  
		Last Modified: Fri, 01 Dec 2023 00:11:35 GMT  
		Size: 347.3 KB (347329 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:180e726b1ca7c7a79c7d4bf57db66fd6282b99be5eb74aa889b392f2a6187f05`  
		Last Modified: Fri, 01 Dec 2023 00:11:35 GMT  
		Size: 7.5 MB (7528754 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:10db30073339e0582d3f082c533e19446a82d3c6834a7286c6098a8f5ef63865`  
		Last Modified: Fri, 01 Dec 2023 00:11:35 GMT  
		Size: 99.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:79a7b919c3e26ccae3cffc5657d7d7caaf00e98ea71f5beec669f0382953f658`  
		Last Modified: Fri, 01 Dec 2023 00:11:36 GMT  
		Size: 562.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `redis:6-alpine3.18` - unknown; unknown

```console
$ docker pull redis@sha256:95be21dafaa13d90a070967f05fd594b9721e82924664f56b7d5f9fadb2230fe
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **716.9 KB (716878 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19066c7413a758ce5674381854c6aeb5467a4bb1cba3a3fe4faf6ee03430e926`

```dockerfile
```

-	Layers:
	-	`sha256:caacb604011c553f578eefb693848983387ccaadc17508449b9d791e86593d4b`  
		Last Modified: Fri, 01 Dec 2023 00:11:35 GMT  
		Size: 689.9 KB (689936 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:d04ac61396b978bbcc3f56815b0d4ed0f8375d3511d41f96bcdbc01846338ee4`  
		Last Modified: Fri, 01 Dec 2023 00:11:35 GMT  
		Size: 26.9 KB (26942 bytes)  
		MIME: application/vnd.in-toto+json

### `redis:6-alpine3.18` - linux; arm variant v6

```console
$ docker pull redis@sha256:2a108447374b501b317eb7faf73a18c8d9a66a74dd0d3d307fe5bd37038a53ca
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **11.1 MB (11071832 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9180b72073b73ca042bed2f0b89e960d7bdef9ca9dd6a05f5cf9b4a79f90900c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Fri, 10 Nov 2023 15:23:15 GMT
ADD file:dbf65487d049081dc2d39b3d99d2c64b6c89754e7e2996a46169d3512e59f32a in / 
# Fri, 10 Nov 2023 15:23:15 GMT
CMD ["/bin/sh"]
# Fri, 10 Nov 2023 15:23:15 GMT
RUN addgroup -S -g 1000 redis && adduser -S -G redis -u 999 redis # buildkit
# Fri, 10 Nov 2023 15:23:15 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		tzdata # buildkit
# Fri, 10 Nov 2023 15:23:15 GMT
ENV REDIS_VERSION=6.2.14
# Fri, 10 Nov 2023 15:23:15 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-6.2.14.tar.gz
# Fri, 10 Nov 2023 15:23:15 GMT
ENV REDIS_DOWNLOAD_SHA=34e74856cbd66fdb3a684fb349d93961d8c7aa668b06f81fd93ff267d09bc277
# Fri, 10 Nov 2023 15:23:15 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		dpkg-dev dpkg 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 		wget 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version; 		echo '{"spdxVersion":"SPDX-2.3","SPDXID":"SPDXRef-DOCUMENT","name":"redis-server-sbom","packages":[{"name":"redis-server","versionInfo":"6.2.14","SPDXID":"SPDXRef-Package--redis-server","externalRefs":[{"referenceCategory":"PACKAGE-MANAGER","referenceType":"purl","referenceLocator":"pkg:generic/redis-server@6.2.14?os_name=alpine&os_version=3.18"}],"licenseDeclared":"BSD-3-Clause"}]}' > /usr/local/redis.spdx.json # buildkit
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
	-	`sha256:85ae953f9e6740471d4e1440b27721679dc7a511e112eb73df467a4cde26e421`  
		Last Modified: Thu, 30 Nov 2023 22:49:40 GMT  
		Size: 3.1 MB (3146870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2df6971ddb905457479c4708f0ba2df2d0b73234e6ca7da3a95d571965c34209`  
		Last Modified: Fri, 01 Dec 2023 13:21:30 GMT  
		Size: 1.2 KB (1245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd378497a98b60ccc98f26d3bfcbee0c84c52dd634b34c30aab141e23257bd5b`  
		Last Modified: Fri, 01 Dec 2023 13:21:30 GMT  
		Size: 347.1 KB (347147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d73ffec47d794144a9af163c77af7e9830c6b474a681182beade1f5403bb100f`  
		Last Modified: Fri, 01 Dec 2023 13:23:18 GMT  
		Size: 7.6 MB (7575872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0308d0ca18b1df8a0e05c881bc0012990f828cf347b7a2fe7d1720ac958c742`  
		Last Modified: Fri, 01 Dec 2023 13:23:17 GMT  
		Size: 100.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc050f01e74df07e6ed639cf0d692ff8a4cf8804d778899e8a63626b8947bc4f`  
		Last Modified: Fri, 01 Dec 2023 13:23:17 GMT  
		Size: 566.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:6-alpine3.18` - linux; arm variant v7

```console
$ docker pull redis@sha256:90fa985e28de247cca9e796adce777b9048c89130b4b7dfea1d2ed1ab9495dad
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.7 MB (10712425 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1bfb80ad68bdc809cc9ef8abc627b9782521c01bb2d08b4e151bee730fe55af3`
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
ENV REDIS_VERSION=6.2.14
# Fri, 10 Nov 2023 15:23:15 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-6.2.14.tar.gz
# Fri, 10 Nov 2023 15:23:15 GMT
ENV REDIS_DOWNLOAD_SHA=34e74856cbd66fdb3a684fb349d93961d8c7aa668b06f81fd93ff267d09bc277
# Fri, 10 Nov 2023 15:23:15 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		dpkg-dev dpkg 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 		wget 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version; 		echo '{"spdxVersion":"SPDX-2.3","SPDXID":"SPDXRef-DOCUMENT","name":"redis-server-sbom","packages":[{"name":"redis-server","versionInfo":"6.2.14","SPDXID":"SPDXRef-Package--redis-server","externalRefs":[{"referenceCategory":"PACKAGE-MANAGER","referenceType":"purl","referenceLocator":"pkg:generic/redis-server@6.2.14?os_name=alpine&os_version=3.18"}],"licenseDeclared":"BSD-3-Clause"}]}' > /usr/local/redis.spdx.json # buildkit
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
	-	`sha256:62be91d0bffc106dc22c28630ad30554010da271a4b93e989da70f70d0c832db`  
		Last Modified: Fri, 01 Dec 2023 11:55:12 GMT  
		Size: 7.5 MB (7462501 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ac4f3c7f0fa2752bb8a65f419a2db580e7b5c2381e0b5d29a6264e93933ac633`  
		Last Modified: Fri, 01 Dec 2023 11:55:11 GMT  
		Size: 101.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:475d3c795ba00556aaef98a08248b22564c07df25f622d4e61b958a4565fdaed`  
		Last Modified: Fri, 01 Dec 2023 11:55:11 GMT  
		Size: 568.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `redis:6-alpine3.18` - unknown; unknown

```console
$ docker pull redis@sha256:96edd0b892ac56697ab767b15a99eda8918c5acaf4a2382ce4ecd2a83b8c3b3d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **719.4 KB (719367 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0da9446c260a7037172769f0100b0168647ffbecf1253b655915b014f677633f`

```dockerfile
```

-	Layers:
	-	`sha256:83fe0a3c677761782771a84314dd9dd947e0139d3b0dc83906cc08b8f4de7a30`  
		Last Modified: Fri, 01 Dec 2023 11:55:12 GMT  
		Size: 692.5 KB (692464 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:2fbdc335a2bbf89824177bb0733440623700ec4402d4345f03f5a9430bb738e2`  
		Last Modified: Fri, 01 Dec 2023 11:55:11 GMT  
		Size: 26.9 KB (26903 bytes)  
		MIME: application/vnd.in-toto+json

### `redis:6-alpine3.18` - linux; arm64 variant v8

```console
$ docker pull redis@sha256:c876cb9e3815c3715e2236a7fa8962cd45258f3feb79e6d15731216041e1b8be
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **11.3 MB (11280995 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bf5ccad43774ae126d04a9b913fce85cbe2c95a3ae6dcb70f5be11a0e8d73b88`
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
ENV REDIS_VERSION=6.2.14
# Fri, 10 Nov 2023 15:23:15 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-6.2.14.tar.gz
# Fri, 10 Nov 2023 15:23:15 GMT
ENV REDIS_DOWNLOAD_SHA=34e74856cbd66fdb3a684fb349d93961d8c7aa668b06f81fd93ff267d09bc277
# Fri, 10 Nov 2023 15:23:15 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		dpkg-dev dpkg 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 		wget 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version; 		echo '{"spdxVersion":"SPDX-2.3","SPDXID":"SPDXRef-DOCUMENT","name":"redis-server-sbom","packages":[{"name":"redis-server","versionInfo":"6.2.14","SPDXID":"SPDXRef-Package--redis-server","externalRefs":[{"referenceCategory":"PACKAGE-MANAGER","referenceType":"purl","referenceLocator":"pkg:generic/redis-server@6.2.14?os_name=alpine&os_version=3.18"}],"licenseDeclared":"BSD-3-Clause"}]}' > /usr/local/redis.spdx.json # buildkit
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
	-	`sha256:db0d69a97f36a4dd3981cce5c152729afed26f73e44bd69185923a92c56c1f15`  
		Last Modified: Fri, 01 Dec 2023 14:24:39 GMT  
		Size: 7.6 MB (7598423 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ada110cb8891ca88d649c4b31354cc4ad6e83f3558ef82bfdb70c285a8d6a0f9`  
		Last Modified: Fri, 01 Dec 2023 14:24:38 GMT  
		Size: 100.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3cf0ad6022b5c12a738c6793e79be3b923295086c99be18125f042f15bdfd8fa`  
		Last Modified: Fri, 01 Dec 2023 14:24:39 GMT  
		Size: 568.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `redis:6-alpine3.18` - unknown; unknown

```console
$ docker pull redis@sha256:e16d2117592d55baf4deb905c93d25ba76de20d5f96bffcda07672b367ad23df
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **716.7 KB (716744 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1e49e57767b55378029e2e4ec8e26db64b99fce353b14cbf6348a1c0c883e766`

```dockerfile
```

-	Layers:
	-	`sha256:51c3a0fae578bef3d4f627c6bb0c9401049803448d61d2b3691e7fb18a0fe834`  
		Last Modified: Fri, 01 Dec 2023 14:24:39 GMT  
		Size: 690.0 KB (689951 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:c13bc34d83c66ddb3fe807d77033155bcc665a7081d0c94360784196d419ec0a`  
		Last Modified: Fri, 01 Dec 2023 14:24:38 GMT  
		Size: 26.8 KB (26793 bytes)  
		MIME: application/vnd.in-toto+json

### `redis:6-alpine3.18` - linux; 386

```console
$ docker pull redis@sha256:43b0ec519618aa5b0b5ec64af253058ef8b31fba16107466b16c67e921aedf7f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.1 MB (13138490 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:642ea7d7630df7e2f8d6e56232555f51d0f9594ff5a4ce55feef7739d7d76cae`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Thu, 28 Sep 2023 20:38:19 GMT
ADD file:8402753f294e403e92353bd65c86a6428c960be5116c0a15484b663a84f66fcd in / 
# Thu, 28 Sep 2023 20:38:20 GMT
CMD ["/bin/sh"]
# Thu, 19 Oct 2023 13:19:06 GMT
RUN addgroup -S -g 1000 redis && adduser -S -G redis -u 999 redis # buildkit
# Thu, 19 Oct 2023 13:19:06 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		tzdata # buildkit
# Thu, 19 Oct 2023 13:19:06 GMT
ENV REDIS_VERSION=6.2.14
# Thu, 19 Oct 2023 13:19:06 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-6.2.14.tar.gz
# Thu, 19 Oct 2023 13:19:06 GMT
ENV REDIS_DOWNLOAD_SHA=34e74856cbd66fdb3a684fb349d93961d8c7aa668b06f81fd93ff267d09bc277
# Thu, 19 Oct 2023 13:19:06 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		dpkg-dev dpkg 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 		wget 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version # buildkit
# Thu, 19 Oct 2023 13:19:06 GMT
RUN mkdir /data && chown redis:redis /data # buildkit
# Thu, 19 Oct 2023 13:19:06 GMT
VOLUME [/data]
# Thu, 19 Oct 2023 13:19:06 GMT
WORKDIR /data
# Thu, 19 Oct 2023 13:19:06 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 19 Oct 2023 13:19:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 19 Oct 2023 13:19:06 GMT
EXPOSE map[6379/tcp:{}]
# Thu, 19 Oct 2023 13:19:06 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:dc95107ad2a031a015320bb397f73ec151d738127175b31ad643120697dc7e90`  
		Last Modified: Thu, 28 Sep 2023 20:39:32 GMT  
		Size: 3.2 MB (3235757 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c84bfc582fee8b30ba784a17fcd5ee0ac7c3371df042cb20166990c97a9b539d`  
		Last Modified: Sat, 04 Nov 2023 00:01:56 GMT  
		Size: 1.2 KB (1244 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2f490dd3e48a0900b55a6c612d2ee709942fd485b1c5e8b943750270d64f609f`  
		Last Modified: Sat, 04 Nov 2023 00:01:56 GMT  
		Size: 347.4 KB (347357 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fc86aa0627cfdc338dc5f4f503743ba0e328fdb92a3ff95e383ad20c500a647f`  
		Last Modified: Sat, 04 Nov 2023 00:01:57 GMT  
		Size: 9.6 MB (9553427 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c810e2a0effcf90fb157a0dd02354226670379e1fbaacb97b2b09db8c9268233`  
		Last Modified: Sat, 04 Nov 2023 00:01:56 GMT  
		Size: 100.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:144f71b2d38c1ac4b19e82eecdd2ee3ce9a13871634be6ccec5ff52510cd936a`  
		Last Modified: Sat, 04 Nov 2023 00:01:57 GMT  
		Size: 573.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `redis:6-alpine3.18` - unknown; unknown

```console
$ docker pull redis@sha256:ff2a2517e1becfe3e790e4b1ed9dad64256f99a3be142b55b8ee16995c6a2128
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.6 KB (25564 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2091a60c10b28d843b5948fa55316f2f15f1888f688b5ec435c607b0c0108a5a`

```dockerfile
```

-	Layers:
	-	`sha256:9559934fe0f4ebdf1323c0cd1ad83d87c1257cdcb323bc5e5e7bab249c668a72`  
		Last Modified: Sat, 04 Nov 2023 00:01:56 GMT  
		Size: 25.6 KB (25564 bytes)  
		MIME: application/vnd.in-toto+json

### `redis:6-alpine3.18` - linux; ppc64le

```console
$ docker pull redis@sha256:3cebc79af77df84ce8d797744e176aa568b18f098612fd02b9a41fc085a6c3cd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **11.8 MB (11837493 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e2bda5c7f72111cc04dd6136d8de472692573203ab51e3804c83338fae58666`
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
ENV REDIS_VERSION=6.2.14
# Fri, 10 Nov 2023 15:23:15 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-6.2.14.tar.gz
# Fri, 10 Nov 2023 15:23:15 GMT
ENV REDIS_DOWNLOAD_SHA=34e74856cbd66fdb3a684fb349d93961d8c7aa668b06f81fd93ff267d09bc277
# Fri, 10 Nov 2023 15:23:15 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		dpkg-dev dpkg 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 		wget 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version; 		echo '{"spdxVersion":"SPDX-2.3","SPDXID":"SPDXRef-DOCUMENT","name":"redis-server-sbom","packages":[{"name":"redis-server","versionInfo":"6.2.14","SPDXID":"SPDXRef-Package--redis-server","externalRefs":[{"referenceCategory":"PACKAGE-MANAGER","referenceType":"purl","referenceLocator":"pkg:generic/redis-server@6.2.14?os_name=alpine&os_version=3.18"}],"licenseDeclared":"BSD-3-Clause"}]}' > /usr/local/redis.spdx.json # buildkit
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
	-	`sha256:183b9aab37a2272f558c7a240098a4953cab46143e9b510b1c29aa66e95a44fe`  
		Last Modified: Fri, 01 Dec 2023 13:03:46 GMT  
		Size: 8.1 MB (8139567 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:022accbccdb0d252593f5e62055f17612892482b8c5a72e4b2de8df6e42fdb8c`  
		Last Modified: Fri, 01 Dec 2023 13:03:45 GMT  
		Size: 101.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7de84b0ae09e0d319ff670b37d5a79c69289fdbb6294d3451ac59ef021300996`  
		Last Modified: Fri, 01 Dec 2023 13:03:45 GMT  
		Size: 571.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `redis:6-alpine3.18` - unknown; unknown

```console
$ docker pull redis@sha256:9a664b90e10dd9c5e80ed1478af99d3459e9fd609e961d95ea92a5fefbf30da9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **715.2 KB (715181 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a7227bcabeb0f1ceb3d3a41b33cd2eec6902bf70842538b7f7002313140ad57d`

```dockerfile
```

-	Layers:
	-	`sha256:8b97b729f4296a8525a95484b18e1b04d4d012b91f5aa89fc59ee4e0e8303779`  
		Last Modified: Fri, 01 Dec 2023 13:03:46 GMT  
		Size: 688.3 KB (688346 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:5eca81f8f17822b59c8a3ac445ef42dd18f6647a57c35f6c5e2388882b95a18a`  
		Last Modified: Fri, 01 Dec 2023 13:03:45 GMT  
		Size: 26.8 KB (26835 bytes)  
		MIME: application/vnd.in-toto+json

### `redis:6-alpine3.18` - linux; s390x

```console
$ docker pull redis@sha256:a6ee579e1e4fbec8f22df06aea43e3d84ff047d4e757770d906aaf59f879c968
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **11.4 MB (11393427 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:27493449551e02e9f19ceaa52c2d514e3693eccaa97515dabb1d616386ac6081`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Fri, 10 Nov 2023 15:23:15 GMT
ADD file:50d6643abf7df167a927decd69d193b980557ff73cca48dce86d57e2ff25ad45 in / 
# Fri, 10 Nov 2023 15:23:15 GMT
CMD ["/bin/sh"]
# Fri, 10 Nov 2023 15:23:15 GMT
RUN addgroup -S -g 1000 redis && adduser -S -G redis -u 999 redis # buildkit
# Fri, 10 Nov 2023 15:23:15 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		tzdata # buildkit
# Fri, 10 Nov 2023 15:23:15 GMT
ENV REDIS_VERSION=6.2.14
# Fri, 10 Nov 2023 15:23:15 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-6.2.14.tar.gz
# Fri, 10 Nov 2023 15:23:15 GMT
ENV REDIS_DOWNLOAD_SHA=34e74856cbd66fdb3a684fb349d93961d8c7aa668b06f81fd93ff267d09bc277
# Fri, 10 Nov 2023 15:23:15 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		dpkg-dev dpkg 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 		wget 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version; 		echo '{"spdxVersion":"SPDX-2.3","SPDXID":"SPDXRef-DOCUMENT","name":"redis-server-sbom","packages":[{"name":"redis-server","versionInfo":"6.2.14","SPDXID":"SPDXRef-Package--redis-server","externalRefs":[{"referenceCategory":"PACKAGE-MANAGER","referenceType":"purl","referenceLocator":"pkg:generic/redis-server@6.2.14?os_name=alpine&os_version=3.18"}],"licenseDeclared":"BSD-3-Clause"}]}' > /usr/local/redis.spdx.json # buildkit
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
	-	`sha256:2ea477e1c0c3db3337ee1d7c659f8c465021a65c036998ed3fa3b667d4b30153`  
		Last Modified: Thu, 30 Nov 2023 22:42:52 GMT  
		Size: 3.2 MB (3217454 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:72e6dd364dbbcb95d95bf4b0b2cec1273c6f92a8b8fb677cf42d41a68c140b14`  
		Last Modified: Fri, 01 Dec 2023 12:23:54 GMT  
		Size: 1.2 KB (1244 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c9e329ccf1820b22a93f390432f82d6899038db625bc0c3195393a0aa8ccbed6`  
		Last Modified: Fri, 01 Dec 2023 12:23:55 GMT  
		Size: 347.4 KB (347368 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3d4b6edefa1db64f35c716085c6d3fd2a4c63805a30d9553ffa8faf418a904f5`  
		Last Modified: Fri, 01 Dec 2023 12:26:17 GMT  
		Size: 7.8 MB (7826658 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:76eee91cd5d0bd5cadccf2c516203a1a1e148fee490f8ea3e84f99919ebe9e68`  
		Last Modified: Fri, 01 Dec 2023 12:26:16 GMT  
		Size: 100.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b349e2d73aba7e70a0de0f76e5085424330e9deceafe83438b1e09f05542d46d`  
		Last Modified: Fri, 01 Dec 2023 12:26:16 GMT  
		Size: 571.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `redis:6-alpine3.18` - unknown; unknown

```console
$ docker pull redis@sha256:d0e619baba0150d6366ad6a5f648118978fe090e792e28431ba8a3109c4c20db
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **715.1 KB (715079 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ff43c5d09dea95e415f55c71b7574cfa9b107e845ec2d65b25c3cbc3d1ffe336`

```dockerfile
```

-	Layers:
	-	`sha256:8fb70b6254ce54c0680fcc7845d2f9ae30540af4b7448bfef280334fe583c1eb`  
		Last Modified: Fri, 01 Dec 2023 12:26:16 GMT  
		Size: 688.3 KB (688300 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:56d1dbbd28b8079882a87893c4aff6717bc62075639e58c29831e546254b27a4`  
		Last Modified: Fri, 01 Dec 2023 12:26:16 GMT  
		Size: 26.8 KB (26779 bytes)  
		MIME: application/vnd.in-toto+json
