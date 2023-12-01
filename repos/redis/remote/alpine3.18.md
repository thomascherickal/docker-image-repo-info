## `redis:alpine3.18`

```console
$ docker pull redis@sha256:a7a1bec025e8f5cc2e8d8bdc6ad8372073fedd79fae7b7200141aa0864a7e4e8
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

### `redis:alpine3.18` - linux; amd64

```console
$ docker pull redis@sha256:9e3f3a58c85904fe2d40088b5b69dfe688ba3eff91320f2849df3eeea5d2bf7d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.6 MB (15624494 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d6420819df1b0de1008141a23b4a6fa4c658ff699e2f10db129b7891b7256661`
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
	-	`sha256:c926b61bad3b94ae7351bafd0c184c159ebf0643b085f7ef1d47ecdc7316833c`  
		Last Modified: Thu, 30 Nov 2023 23:23:28 GMT  
		Size: 3.4 MB (3402422 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:88ee276465ceaeddd42b045aaa18ed436174e65b326ca2e24e1f32051740a3ae`  
		Last Modified: Fri, 01 Dec 2023 00:12:15 GMT  
		Size: 1.2 KB (1244 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4ba2c8f9b916fe6173a82e0a4aa979410387f773c7a166e80c37f070d30ce322`  
		Last Modified: Fri, 01 Dec 2023 00:12:15 GMT  
		Size: 347.3 KB (347309 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:86024d2069a54ad7df24ef5c1c9c31df78ceff57605358f363f5da94dad684f7`  
		Last Modified: Fri, 01 Dec 2023 00:12:16 GMT  
		Size: 11.9 MB (11872823 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:cc50070e1a927919dc3852040dc3a6c20b1804e02cc4feba592ab5f86f1f9205`  
		Last Modified: Fri, 01 Dec 2023 00:12:15 GMT  
		Size: 100.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5e1605eb5694a43274f94c9f23da092574c7e3ebe12b568a79f1a610e69d6587`  
		Last Modified: Fri, 01 Dec 2023 00:12:16 GMT  
		Size: 564.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `redis:alpine3.18` - unknown; unknown

```console
$ docker pull redis@sha256:c05a452c4af9eb319648dbdd347ede6e897079ae4b149641e75ce9e7ef1be024
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **718.1 KB (718065 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5cea50775c389bd3b07958bb5eba5d745c57afb34233b75b3349063b27e985cc`

```dockerfile
```

-	Layers:
	-	`sha256:0072bf82dee999dde07f60c1bc273806a9910295c3d57dbc24ac0ac5854bee64`  
		Last Modified: Fri, 01 Dec 2023 00:12:15 GMT  
		Size: 690.5 KB (690530 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:fa4dc7d2b6e1c7aabb54d2c8abcd5f33508cda341ad57789beaff59d47cf867d`  
		Last Modified: Fri, 01 Dec 2023 00:12:15 GMT  
		Size: 27.5 KB (27535 bytes)  
		MIME: application/vnd.in-toto+json

### `redis:alpine3.18` - linux; arm variant v6

```console
$ docker pull redis@sha256:51a49eaa042ef1661290eede107a8b08cfc49e97d411dbd0a1ca5c25047e2244
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.7 MB (17662977 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa8b69849dcebedc73f43e4eace58f5027b2d8f34899bb0a52032dc6d4048b1e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Thu, 28 Sep 2023 20:49:16 GMT
ADD file:2222b03381ff0fce22edd647f5c60529ec6a72202f8d3cb1d6e4648ebcd19a1e in / 
# Thu, 28 Sep 2023 20:49:16 GMT
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
	-	`sha256:91cb83b91ee16f1ee0d588fccef56ab5dbb5689a64e5373caf33d7e4fe52ceb4`  
		Last Modified: Thu, 28 Sep 2023 20:51:25 GMT  
		Size: 3.1 MB (3145291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a63c4a2c988c14d91bd1bb24d26d73d206d9ca3a20b02760ebf137a1fbd73d42`  
		Last Modified: Sat, 04 Nov 2023 00:15:51 GMT  
		Size: 1.2 KB (1245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48418e23975922d413d904980fa6f97cacdcd980409557f2d959ecb456922426`  
		Last Modified: Sat, 04 Nov 2023 00:15:51 GMT  
		Size: 347.2 KB (347164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ff1be6d21a4e1cfbe3c01dd714be73f4e369eb0154a6ae6d9340c51e180c113`  
		Last Modified: Thu, 16 Nov 2023 01:23:37 GMT  
		Size: 14.2 MB (14168578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c38ee51022a80f8a4d396c4c132e6cec009d1e6305acee8dd9c86a33dfb6f088`  
		Last Modified: Thu, 16 Nov 2023 01:23:34 GMT  
		Size: 100.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75f43529154f4a50fe7940d85032673aeaf5a8dbd09a08678abc0fddb6128ab9`  
		Last Modified: Thu, 16 Nov 2023 01:23:34 GMT  
		Size: 567.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:alpine3.18` - linux; arm variant v7

```console
$ docker pull redis@sha256:b2865b55ac1594cfc4e025779271208741d2fd22c4311284fb687fece13de10f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.1 MB (17133456 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fd6dd1ed296a212da2c79800e8009341e1e28ad60d7f3407b51b5c6b151a852e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Thu, 28 Sep 2023 20:59:24 GMT
ADD file:61f54a318ad79861c6177783bb4c604412b5d952f45a9aa12ff97f4dccba7f73 in / 
# Thu, 28 Sep 2023 20:59:24 GMT
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
	-	`sha256:622a0779436eb93ceea635e910268f867c2eba47d4f62f0bd45f0bd165af3572`  
		Last Modified: Thu, 28 Sep 2023 21:00:50 GMT  
		Size: 2.9 MB (2899905 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:da8bcc30219a3b5ad7547cb998dbc925d87391c679fec1abae88483d4839fa51`  
		Last Modified: Tue, 03 Oct 2023 23:23:43 GMT  
		Size: 1.2 KB (1245 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1a1e96038724920ff29465fba0c7aca16d709e1f1d94b903204ed8b6af9e8387`  
		Last Modified: Tue, 03 Oct 2023 23:23:43 GMT  
		Size: 347.0 KB (346994 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c974a79c66f6ffbbdb488117f05ff5e40b96ba6e891ce10446d8d725fdf4cc5a`  
		Last Modified: Thu, 16 Nov 2023 08:03:53 GMT  
		Size: 13.9 MB (13884615 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:db97c126d17a8a9c63732ac2966c0ab79aeafbef869724445b2df371d7b795af`  
		Last Modified: Thu, 16 Nov 2023 08:03:53 GMT  
		Size: 101.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2d69df5baf25119b81583231ded6feb7c7de767f1915143c3829e8c2839377cb`  
		Last Modified: Thu, 16 Nov 2023 08:03:53 GMT  
		Size: 564.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `redis:alpine3.18` - unknown; unknown

```console
$ docker pull redis@sha256:5d2002d89d6f8916622542747b64a3374afe6fa25ee1e4869135785736340afe
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **721.5 KB (721451 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c7d9c810f2369076b8402b9ab1d5c75e4b4d3a84cd5cea55d69176e78347a934`

```dockerfile
```

-	Layers:
	-	`sha256:6244e7c4c039e412462af8fc2f0a01f817f0b3a27d8855f4c8dc386cbef0f431`  
		Last Modified: Thu, 16 Nov 2023 08:03:53 GMT  
		Size: 693.9 KB (693941 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:81a73c0b58722f99b4cf23ba558694e3b47a80ce6c99ecd14e708cab5864cebe`  
		Last Modified: Thu, 16 Nov 2023 08:03:52 GMT  
		Size: 27.5 KB (27510 bytes)  
		MIME: application/vnd.in-toto+json

### `redis:alpine3.18` - linux; arm64 variant v8

```console
$ docker pull redis@sha256:43076a37580453c7d2516cff8e4aa6b5a8af2c86366ff8b8b4bde0b0b1fb0c32
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.1 MB (18085158 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f9825906c4729a1edf445de2a66ab546115b54f915a009b396c96bd412d43735`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Thu, 28 Sep 2023 20:39:33 GMT
ADD file:ff3112828967e8004a3264d7ece3f81c88e6a1d44d360b9b5613caab15b41717 in / 
# Thu, 28 Sep 2023 20:39:34 GMT
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
	-	`sha256:579b34f0a95bb83b3acd6b3249ddc52c3d80f5c84b13c944e9e324feb86dd329`  
		Last Modified: Thu, 28 Sep 2023 20:40:08 GMT  
		Size: 3.3 MB (3331831 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2e0feb8fddc533ebe8fa3e28ab60443a2b6a5a7e46ff3560b1e79f4ff945a70f`  
		Last Modified: Tue, 03 Oct 2023 23:02:00 GMT  
		Size: 1.2 KB (1243 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a743b36a722987becef2b73971d75377bee67a2a6577cbdfddc1da3634eb4a73`  
		Last Modified: Tue, 03 Oct 2023 23:02:01 GMT  
		Size: 347.6 KB (347581 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e921a448359a4fec1c9fc2b03da1676cc4a0cbce73a7ff503faafc2128f3f070`  
		Last Modified: Thu, 16 Nov 2023 01:36:33 GMT  
		Size: 14.4 MB (14403801 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ead72011169f10ebef949b2a6c940c6190ebbed1146fb53b8edc2dff870d3d21`  
		Last Modified: Thu, 16 Nov 2023 01:36:32 GMT  
		Size: 100.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a6335bc74acc3ee6c090362f9f80d236e7955e347e8198a46c0860d058478df7`  
		Last Modified: Thu, 16 Nov 2023 01:36:32 GMT  
		Size: 570.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `redis:alpine3.18` - unknown; unknown

```console
$ docker pull redis@sha256:4ff411fbb9a1ef2e1b78399b3629d44b22c902c2caf9cb49a58634b6c1eb9fc7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **718.8 KB (718803 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:06ca52cf96a1847941fe639363ffe04d0a90df49e222a3e56cc60e6e14b53454`

```dockerfile
```

-	Layers:
	-	`sha256:de880ad0e056e005a63ee3ffb9425fe45fcfb58f2075287a089bd663eaad5030`  
		Last Modified: Thu, 16 Nov 2023 01:36:33 GMT  
		Size: 691.4 KB (691416 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:0170c07b267b2d700f2d071909e7c71ce5b7ef6ae51604d7304f424d468ca514`  
		Last Modified: Thu, 16 Nov 2023 01:36:32 GMT  
		Size: 27.4 KB (27387 bytes)  
		MIME: application/vnd.in-toto+json

### `redis:alpine3.18` - linux; 386

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

### `redis:alpine3.18` - unknown; unknown

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

### `redis:alpine3.18` - linux; ppc64le

```console
$ docker pull redis@sha256:cd31e92484e7a53603cd2ab62fdd7e212bfcb9d0323c5ef853e342e3b55a4c8b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.8 MB (18786607 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d3b338c738c31f47e6d30cf17b57d475d0e6e4c44a980b35aac3738ae2ca828`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Thu, 28 Sep 2023 21:22:20 GMT
ADD file:a720acb99214334c501363d564d8cae9b90d062ccf8a24a5ba1c831545b783dd in / 
# Thu, 28 Sep 2023 21:22:21 GMT
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
	-	`sha256:cd37f9856024d6685ac0233823aded690551c5872d6a27699a96c6a479d20f6f`  
		Last Modified: Thu, 28 Sep 2023 21:23:43 GMT  
		Size: 3.3 MB (3346508 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e963944e7d7c85e7e5202f0596efabc5d145dfc37f6e0a9b481b7e185470e576`  
		Last Modified: Tue, 03 Oct 2023 23:04:16 GMT  
		Size: 1.2 KB (1245 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d5c07f1f59e5142c61f551a02105a3fe01c28e7ae009ba3c9ef69dc54d2c90a8`  
		Last Modified: Tue, 03 Oct 2023 23:04:16 GMT  
		Size: 347.6 KB (347649 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:12647f7344c9fb8b6544692f81d9db510849807696923910e8840fc32e1e23ad`  
		Last Modified: Thu, 16 Nov 2023 05:52:26 GMT  
		Size: 15.1 MB (15090505 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3a9c7caf202e8921408c2056e5c3f8e43e64eb48d41df34de99d75ce9b971dfe`  
		Last Modified: Thu, 16 Nov 2023 05:52:25 GMT  
		Size: 99.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1d06b48051e37c85df8061b077131eda5965ff6df7bf665819df1f01fa5122d7`  
		Last Modified: Thu, 16 Nov 2023 05:52:25 GMT  
		Size: 569.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `redis:alpine3.18` - unknown; unknown

```console
$ docker pull redis@sha256:1e36ccd32a4cffa5c9691cdae75bc522bbed12295ceb50fcc9dfe5d314802c73
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **717.3 KB (717252 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f873b732ec8e3346bc0fd52972072cd39dae22c9c3e78ea6e87a1df0a15e15aa`

```dockerfile
```

-	Layers:
	-	`sha256:aead00e7eacd99acc82319b1d14a2506396d096e1ad5169e4079980fd1c30ebe`  
		Last Modified: Thu, 16 Nov 2023 05:52:25 GMT  
		Size: 689.8 KB (689819 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:7d7dd1bdb30490f86b480cd3fb4e7a2dbf9f63bd291cd4245585ece1aacae19f`  
		Last Modified: Thu, 16 Nov 2023 05:52:25 GMT  
		Size: 27.4 KB (27433 bytes)  
		MIME: application/vnd.in-toto+json

### `redis:alpine3.18` - linux; s390x

```console
$ docker pull redis@sha256:ea9b693d60dbd98c87fd71bc42aaa429a2d643dd68557921c71409ed0bbce12e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.0 MB (18044280 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:39c8fb56946704a1460c9b97eadc9f06862f215fb3e09845bc320dd702989612`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Thu, 28 Sep 2023 20:41:43 GMT
ADD file:fd3808a676fc56c1380e55b2ddbf4014d9371346cf789860b336bc9f00729ed0 in / 
# Thu, 28 Sep 2023 20:41:44 GMT
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
	-	`sha256:47539bffe0f44273ec7731d86be2a6171359b3847c9b60c6ac74c4875c3264af`  
		Last Modified: Thu, 28 Sep 2023 20:43:18 GMT  
		Size: 3.2 MB (3215103 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2f8fb319e3e2b6d090a150207805753dae05abe1df53b9dae9b211d46986bb8e`  
		Last Modified: Tue, 03 Oct 2023 23:15:31 GMT  
		Size: 1.2 KB (1243 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8b8fdacac4cf0c35819b1f0be78d8bed53f4dfdce11d17b3918d554a29299129`  
		Last Modified: Tue, 03 Oct 2023 23:15:31 GMT  
		Size: 347.4 KB (347360 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:cfec83eed03384c04d238a85244bfe4fa77d9788401e3c64004b6a2dc2de55b4`  
		Last Modified: Thu, 16 Nov 2023 01:25:13 GMT  
		Size: 14.5 MB (14479873 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2323097004788df00d7c273b8f3e1a314c3a6319de30ab9a92ff8d40d1704eaf`  
		Last Modified: Thu, 16 Nov 2023 01:25:13 GMT  
		Size: 101.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:81c8a36593a6814de18dc4771efb91c0a3c039149322ce1c8ae8d2d10b144d93`  
		Last Modified: Thu, 16 Nov 2023 01:25:13 GMT  
		Size: 568.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `redis:alpine3.18` - unknown; unknown

```console
$ docker pull redis@sha256:623d67c0f57b220297ca25f47e5ee27ccc4f206897e12d7980921e06847c205c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **717.1 KB (717130 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:13b37a386ba12e7494779c023606693d1a8b82930c187e10986d3644e985b995`

```dockerfile
```

-	Layers:
	-	`sha256:f9322b40c861dd963a5d571146663c0acaf010008db75bd58978a892e81926f1`  
		Last Modified: Thu, 16 Nov 2023 01:25:13 GMT  
		Size: 689.8 KB (689761 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:14c35f1320ccc9b1bae2306fac2e8d290dc7843e17ef2f232d2e7ce49de7414b`  
		Last Modified: Thu, 16 Nov 2023 01:25:13 GMT  
		Size: 27.4 KB (27369 bytes)  
		MIME: application/vnd.in-toto+json
