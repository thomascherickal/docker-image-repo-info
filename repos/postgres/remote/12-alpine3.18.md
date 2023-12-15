## `postgres:12-alpine3.18`

```console
$ docker pull postgres@sha256:fb31f059837e6aff0b4c1f425cc9338f9c51761e5de9fa7e629942e1a26bfa77
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 14
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm variant v6
	-	unknown; unknown
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

### `postgres:12-alpine3.18` - linux; amd64

```console
$ docker pull postgres@sha256:c166f8ca3105b48952459efd4ec2d8c53dc7b6cfb831003182d35c16a56c7daf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **90.5 MB (90536973 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d44ea9f12c6a8dca51a9bcbf1f4460102f8dd173d2450342badb31b6092b12d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 30 Nov 2023 23:22:52 GMT
ADD file:fc714080c3bcbbce7ac746a10d7b4355ffa36293a8d435d62cd5359ea8eb8364 in / 
# Thu, 30 Nov 2023 23:22:52 GMT
CMD ["/bin/sh"]
# Wed, 13 Dec 2023 22:17:08 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql # buildkit
# Wed, 13 Dec 2023 22:17:08 GMT
ENV LANG=en_US.utf8
# Wed, 13 Dec 2023 22:17:08 GMT
RUN mkdir /docker-entrypoint-initdb.d # buildkit
# Wed, 13 Dec 2023 22:17:08 GMT
ENV PG_MAJOR=12
# Wed, 13 Dec 2023 22:17:08 GMT
ENV PG_VERSION=12.17
# Wed, 13 Dec 2023 22:17:08 GMT
ENV PG_SHA256=93e8e1b23981d5f03c6c5763f77b28184c1ce4db7194fa466e2edb65d9c1c5f6
# Wed, 13 Dec 2023 22:17:08 GMT
ENV DOCKER_PG_LLVM_DEPS=llvm15-dev 		clang15
# Wed, 13 Dec 2023 22:17:08 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		$DOCKER_PG_LLVM_DEPS 		bison 		coreutils 		dpkg-dev dpkg 		flex 		g++ 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openldap-dev 		openssl-dev 		perl-dev 		perl-ipc-run 		perl-utils 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 		export LLVM_CONFIG="/usr/lib/llvm15/bin/llvm-config"; 	export CLANG=clang-15; 		./configure 		--enable-option-checking=fatal 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 		zstd 		icu-data-full 		$([ "$(apk --print-arch)" != 'ppc64le' ] && echo 'nss_wrapper') 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version # buildkit
# Wed, 13 Dec 2023 22:17:08 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample # buildkit
# Wed, 13 Dec 2023 22:17:08 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 3777 /var/run/postgresql # buildkit
# Wed, 13 Dec 2023 22:17:08 GMT
ENV PGDATA=/var/lib/postgresql/data
# Wed, 13 Dec 2023 22:17:08 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 1777 "$PGDATA" # buildkit
# Wed, 13 Dec 2023 22:17:08 GMT
VOLUME [/var/lib/postgresql/data]
# Wed, 13 Dec 2023 22:17:08 GMT
COPY docker-entrypoint.sh docker-ensure-initdb.sh /usr/local/bin/ # buildkit
# Wed, 13 Dec 2023 22:17:08 GMT
RUN ln -sT docker-ensure-initdb.sh /usr/local/bin/docker-enforce-initdb.sh # buildkit
# Wed, 13 Dec 2023 22:17:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 13 Dec 2023 22:17:08 GMT
STOPSIGNAL SIGINT
# Wed, 13 Dec 2023 22:17:08 GMT
EXPOSE map[5432/tcp:{}]
# Wed, 13 Dec 2023 22:17:08 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:c926b61bad3b94ae7351bafd0c184c159ebf0643b085f7ef1d47ecdc7316833c`  
		Last Modified: Thu, 30 Nov 2023 23:23:28 GMT  
		Size: 3.4 MB (3402422 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4c68cbc5c4415e2796a06a9d23616176f14bbfb64439321a0bc5d7608eed10e9`  
		Last Modified: Thu, 14 Dec 2023 18:55:58 GMT  
		Size: 1.3 KB (1263 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:74565430d7de9d3885b677358bb042fef7abafdd2eff28db5a9d9886b28e94a5`  
		Last Modified: Thu, 14 Dec 2023 18:55:59 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f1a9a31edc4826a0b07a8929be3802989ba59caa3e44f92fe90e082086d625ef`  
		Last Modified: Thu, 14 Dec 2023 18:56:01 GMT  
		Size: 87.1 MB (87118658 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:85a2f7e096e61c54667f5cbe96c199d3c76ee9d590658cc5bf6082b877fd87e4`  
		Last Modified: Thu, 14 Dec 2023 18:55:58 GMT  
		Size: 8.7 KB (8692 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2e2f44e57a20efd9ad095933b03734cc4e6870f16ff1f3ee61c3ecfa5bc6e4e6`  
		Last Modified: Thu, 14 Dec 2023 18:55:59 GMT  
		Size: 129.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5a70275430cdaa72e746bf6572cdefb4f26c97688a60c740b718f0ef237ea215`  
		Last Modified: Thu, 14 Dec 2023 18:55:59 GMT  
		Size: 170.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9ce8d9841a714344af71698b7cd7069b45fbb1d753667c8d46d1602809d3eac0`  
		Last Modified: Thu, 14 Dec 2023 18:56:00 GMT  
		Size: 5.3 KB (5339 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:deb332bf1a495500f3bebf94d044bebf6353eedae267cff98419af2255672d23`  
		Last Modified: Thu, 14 Dec 2023 18:56:00 GMT  
		Size: 184.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `postgres:12-alpine3.18` - unknown; unknown

```console
$ docker pull postgres@sha256:511624d59dc162b550aa66991aa9b593938e73e1134ed3e481015850213443a1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **840.3 KB (840264 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fba5807283a8200afc4708b64f1c53aaed225edca20b4f15a1ea99ed3edf5a2f`

```dockerfile
```

-	Layers:
	-	`sha256:f76981173cd50fb9d5cc4279c61b464f7e8800e5c8f5dfb81ee77222eac3288e`  
		Last Modified: Thu, 14 Dec 2023 18:55:58 GMT  
		Size: 803.6 KB (803632 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:dab3dd063ee5651a84ae259cdfbafcd2b8dd665eab2203b1a3b074cd31210807`  
		Last Modified: Thu, 14 Dec 2023 18:55:58 GMT  
		Size: 36.6 KB (36632 bytes)  
		MIME: application/vnd.in-toto+json

### `postgres:12-alpine3.18` - linux; arm variant v6

```console
$ docker pull postgres@sha256:d01327b6f817e64ebd25f73d38f80f56c843726bb64c91e119d8f99708a1f37c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **89.4 MB (89350768 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f47f38e96395bc12e0cb0980dc65c7f9394ebe3f96d73bac008a8ac457504c7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 30 Nov 2023 22:49:18 GMT
ADD file:dbf65487d049081dc2d39b3d99d2c64b6c89754e7e2996a46169d3512e59f32a in / 
# Thu, 30 Nov 2023 22:49:18 GMT
CMD ["/bin/sh"]
# Wed, 13 Dec 2023 22:17:08 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql # buildkit
# Wed, 13 Dec 2023 22:17:08 GMT
ENV LANG=en_US.utf8
# Wed, 13 Dec 2023 22:17:08 GMT
RUN mkdir /docker-entrypoint-initdb.d # buildkit
# Wed, 13 Dec 2023 22:17:08 GMT
ENV PG_MAJOR=12
# Wed, 13 Dec 2023 22:17:08 GMT
ENV PG_VERSION=12.17
# Wed, 13 Dec 2023 22:17:08 GMT
ENV PG_SHA256=93e8e1b23981d5f03c6c5763f77b28184c1ce4db7194fa466e2edb65d9c1c5f6
# Wed, 13 Dec 2023 22:17:08 GMT
ENV DOCKER_PG_LLVM_DEPS=llvm15-dev 		clang15
# Wed, 13 Dec 2023 22:17:08 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		$DOCKER_PG_LLVM_DEPS 		bison 		coreutils 		dpkg-dev dpkg 		flex 		g++ 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openldap-dev 		openssl-dev 		perl-dev 		perl-ipc-run 		perl-utils 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 		export LLVM_CONFIG="/usr/lib/llvm15/bin/llvm-config"; 	export CLANG=clang-15; 		./configure 		--enable-option-checking=fatal 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 		zstd 		icu-data-full 		$([ "$(apk --print-arch)" != 'ppc64le' ] && echo 'nss_wrapper') 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version # buildkit
# Wed, 13 Dec 2023 22:17:08 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample # buildkit
# Wed, 13 Dec 2023 22:17:08 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 3777 /var/run/postgresql # buildkit
# Wed, 13 Dec 2023 22:17:08 GMT
ENV PGDATA=/var/lib/postgresql/data
# Wed, 13 Dec 2023 22:17:08 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 1777 "$PGDATA" # buildkit
# Wed, 13 Dec 2023 22:17:08 GMT
VOLUME [/var/lib/postgresql/data]
# Wed, 13 Dec 2023 22:17:08 GMT
COPY docker-entrypoint.sh docker-ensure-initdb.sh /usr/local/bin/ # buildkit
# Wed, 13 Dec 2023 22:17:08 GMT
RUN ln -sT docker-ensure-initdb.sh /usr/local/bin/docker-enforce-initdb.sh # buildkit
# Wed, 13 Dec 2023 22:17:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 13 Dec 2023 22:17:08 GMT
STOPSIGNAL SIGINT
# Wed, 13 Dec 2023 22:17:08 GMT
EXPOSE map[5432/tcp:{}]
# Wed, 13 Dec 2023 22:17:08 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:85ae953f9e6740471d4e1440b27721679dc7a511e112eb73df467a4cde26e421`  
		Last Modified: Thu, 30 Nov 2023 22:49:40 GMT  
		Size: 3.1 MB (3146870 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:99733932520adb79e9efc69d2e2eb3fdcf866ff3f27e44c498d477613b8f1009`  
		Last Modified: Tue, 12 Dec 2023 22:40:38 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8563d30a0024e9dd3241d3e57d864c72dde0de3fd4903d603de211fd26738a22`  
		Last Modified: Tue, 12 Dec 2023 22:40:38 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fe08a1556e6ad4d5c4a2bd55ac375cc5b3334f8a2e580f5dade84e65b34b61c5`  
		Last Modified: Wed, 13 Dec 2023 00:03:31 GMT  
		Size: 86.2 MB (86187998 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fee0323432a0a49ac6b3a8bdbb04318a00eb7de53507ed94304f996edf066422`  
		Last Modified: Wed, 13 Dec 2023 00:03:28 GMT  
		Size: 8.7 KB (8695 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:90401f21e3b26d26f8b8f2ae504972b66995e3b2cf8555e8837f051e6dce63a4`  
		Last Modified: Wed, 13 Dec 2023 00:03:28 GMT  
		Size: 129.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fd29c49d6784c364cfcad3ccdcfd62f1a3542bf9a80bd659d18d7c27a316ea4d`  
		Last Modified: Wed, 13 Dec 2023 00:03:28 GMT  
		Size: 169.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:216f261e5d5e961e5fc9261ceccb4de07fd46e683633b8f22c6598e186f0b83d`  
		Last Modified: Thu, 14 Dec 2023 18:56:55 GMT  
		Size: 5.3 KB (5343 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b21f0339d073f7bd5b002686f77f3abf1608d31ac6b4c29f7892ba36bd46189d`  
		Last Modified: Thu, 14 Dec 2023 18:56:55 GMT  
		Size: 188.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `postgres:12-alpine3.18` - unknown; unknown

```console
$ docker pull postgres@sha256:34056346d936810309d207e3951a44f8b037e9bf9100168876e45e2aa8eb241b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.4 KB (36383 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c35a257582d1742b6342d72ba0b9b65c9ed96b5a9473a24f35d37eb5e364240e`

```dockerfile
```

-	Layers:
	-	`sha256:cb363231208fd10e643a5d49e8f2d3621dc637ff44281daf8221542ec1b44adc`  
		Last Modified: Thu, 14 Dec 2023 18:56:54 GMT  
		Size: 36.4 KB (36383 bytes)  
		MIME: application/vnd.in-toto+json

### `postgres:12-alpine3.18` - linux; arm variant v7

```console
$ docker pull postgres@sha256:1c3e46349b44f19d67f64e2d687634e4092f406b0401367df5f96fbd09b2f9ed
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.1 MB (84095981 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:be569de453f52334b3ab9f61cfd6fcb28bc625b9656c6a94e8cd56e100a16a73`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 30 Nov 2023 22:49:28 GMT
ADD file:dcb85d43d1fb96861612c42288878b13debfa9d0b956adea1f2472d0c50f0144 in / 
# Thu, 30 Nov 2023 22:49:29 GMT
CMD ["/bin/sh"]
# Wed, 13 Dec 2023 22:17:08 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql # buildkit
# Wed, 13 Dec 2023 22:17:08 GMT
ENV LANG=en_US.utf8
# Wed, 13 Dec 2023 22:17:08 GMT
RUN mkdir /docker-entrypoint-initdb.d # buildkit
# Wed, 13 Dec 2023 22:17:08 GMT
ENV PG_MAJOR=12
# Wed, 13 Dec 2023 22:17:08 GMT
ENV PG_VERSION=12.17
# Wed, 13 Dec 2023 22:17:08 GMT
ENV PG_SHA256=93e8e1b23981d5f03c6c5763f77b28184c1ce4db7194fa466e2edb65d9c1c5f6
# Wed, 13 Dec 2023 22:17:08 GMT
ENV DOCKER_PG_LLVM_DEPS=llvm15-dev 		clang15
# Wed, 13 Dec 2023 22:17:08 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		$DOCKER_PG_LLVM_DEPS 		bison 		coreutils 		dpkg-dev dpkg 		flex 		g++ 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openldap-dev 		openssl-dev 		perl-dev 		perl-ipc-run 		perl-utils 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 		export LLVM_CONFIG="/usr/lib/llvm15/bin/llvm-config"; 	export CLANG=clang-15; 		./configure 		--enable-option-checking=fatal 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 		zstd 		icu-data-full 		$([ "$(apk --print-arch)" != 'ppc64le' ] && echo 'nss_wrapper') 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version # buildkit
# Wed, 13 Dec 2023 22:17:08 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample # buildkit
# Wed, 13 Dec 2023 22:17:08 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 3777 /var/run/postgresql # buildkit
# Wed, 13 Dec 2023 22:17:08 GMT
ENV PGDATA=/var/lib/postgresql/data
# Wed, 13 Dec 2023 22:17:08 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 1777 "$PGDATA" # buildkit
# Wed, 13 Dec 2023 22:17:08 GMT
VOLUME [/var/lib/postgresql/data]
# Wed, 13 Dec 2023 22:17:08 GMT
COPY docker-entrypoint.sh docker-ensure-initdb.sh /usr/local/bin/ # buildkit
# Wed, 13 Dec 2023 22:17:08 GMT
RUN ln -sT docker-ensure-initdb.sh /usr/local/bin/docker-enforce-initdb.sh # buildkit
# Wed, 13 Dec 2023 22:17:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 13 Dec 2023 22:17:08 GMT
STOPSIGNAL SIGINT
# Wed, 13 Dec 2023 22:17:08 GMT
EXPOSE map[5432/tcp:{}]
# Wed, 13 Dec 2023 22:17:08 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:2387a44129d2147bd4e806bf369f3db92eb3ad3b6b8825c739db364b8baa4e26`  
		Last Modified: Thu, 30 Nov 2023 22:49:56 GMT  
		Size: 2.9 MB (2901006 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c815d47e00d2d70d22df505cd75fee458db7a056e91cea2be9e903be7b3cf887`  
		Last Modified: Wed, 13 Dec 2023 01:53:29 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1cc211333283e058626a589bb51c6eea6895cc4988e59b83890811a76d7be3a1`  
		Last Modified: Wed, 13 Dec 2023 01:53:29 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2acd13f706b4696e70423ca204447ce05d2f2f2e21dce87ae6b38a7fbda4b680`  
		Last Modified: Wed, 13 Dec 2023 02:19:40 GMT  
		Size: 81.2 MB (81179082 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f2058ab1f9ad806fdda5428056813e5dc10a4a6f5dc70f53a235fa46d1ad38fa`  
		Last Modified: Wed, 13 Dec 2023 02:19:38 GMT  
		Size: 8.7 KB (8688 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fd6db46d991758399c823e5c458960f9e8dc453b7afc8f8cdef75c992d5aa8ae`  
		Last Modified: Wed, 13 Dec 2023 02:19:38 GMT  
		Size: 129.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:63e0610bb4ceae019c8946cff811cd905849ceb8b4c7359d805605c7f00cbb65`  
		Last Modified: Wed, 13 Dec 2023 02:19:38 GMT  
		Size: 170.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b966baeb948909e529f35923087de991a82ceba39df6837d664c5eb625404432`  
		Last Modified: Thu, 14 Dec 2023 19:33:55 GMT  
		Size: 5.3 KB (5343 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ea2aab7780e7d1b5108d0817cbfc05a43c530a78a7f31be55d5e3c76f34e82b4`  
		Last Modified: Thu, 14 Dec 2023 19:33:55 GMT  
		Size: 187.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `postgres:12-alpine3.18` - unknown; unknown

```console
$ docker pull postgres@sha256:1b6a1fa43916e0fd2f329944144c6130b887102abc5281238dfc94f32f383e64
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **840.2 KB (840250 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e9313d85aa81b95cde5a911fd4643f0e66ef26d70d2a4e42c2848b32222f460f`

```dockerfile
```

-	Layers:
	-	`sha256:21ccc9b2d55cb18b28ad1c6f8e7e8e8468b19e05c4b6f82137d9fb33467d7c1d`  
		Last Modified: Thu, 14 Dec 2023 19:33:55 GMT  
		Size: 803.7 KB (803652 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:782695e21d787e2425e618816f58dd463445f00e4419e4499a648c9911a704d3`  
		Last Modified: Thu, 14 Dec 2023 19:33:55 GMT  
		Size: 36.6 KB (36598 bytes)  
		MIME: application/vnd.in-toto+json

### `postgres:12-alpine3.18` - linux; arm64 variant v8

```console
$ docker pull postgres@sha256:a8bd3e54d52b6dbc6d21f48a5257e45dbdace2088df9729cbbc5bd9dc7f3298a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **89.6 MB (89565531 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:021f921f3bcba607e963323757d054afa1319a090994cca7ad9dcb5092ec970f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 30 Nov 2023 23:11:03 GMT
ADD file:d8a30995bbcd627f084912c728fda5483b6ba486de25af588a0956069d0bd7ad in / 
# Thu, 30 Nov 2023 23:11:03 GMT
CMD ["/bin/sh"]
# Wed, 13 Dec 2023 22:17:08 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql # buildkit
# Wed, 13 Dec 2023 22:17:08 GMT
ENV LANG=en_US.utf8
# Wed, 13 Dec 2023 22:17:08 GMT
RUN mkdir /docker-entrypoint-initdb.d # buildkit
# Wed, 13 Dec 2023 22:17:08 GMT
ENV PG_MAJOR=12
# Wed, 13 Dec 2023 22:17:08 GMT
ENV PG_VERSION=12.17
# Wed, 13 Dec 2023 22:17:08 GMT
ENV PG_SHA256=93e8e1b23981d5f03c6c5763f77b28184c1ce4db7194fa466e2edb65d9c1c5f6
# Wed, 13 Dec 2023 22:17:08 GMT
ENV DOCKER_PG_LLVM_DEPS=llvm15-dev 		clang15
# Wed, 13 Dec 2023 22:17:08 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		$DOCKER_PG_LLVM_DEPS 		bison 		coreutils 		dpkg-dev dpkg 		flex 		g++ 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openldap-dev 		openssl-dev 		perl-dev 		perl-ipc-run 		perl-utils 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 		export LLVM_CONFIG="/usr/lib/llvm15/bin/llvm-config"; 	export CLANG=clang-15; 		./configure 		--enable-option-checking=fatal 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 		zstd 		icu-data-full 		$([ "$(apk --print-arch)" != 'ppc64le' ] && echo 'nss_wrapper') 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version # buildkit
# Wed, 13 Dec 2023 22:17:08 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample # buildkit
# Wed, 13 Dec 2023 22:17:08 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 3777 /var/run/postgresql # buildkit
# Wed, 13 Dec 2023 22:17:08 GMT
ENV PGDATA=/var/lib/postgresql/data
# Wed, 13 Dec 2023 22:17:08 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 1777 "$PGDATA" # buildkit
# Wed, 13 Dec 2023 22:17:08 GMT
VOLUME [/var/lib/postgresql/data]
# Wed, 13 Dec 2023 22:17:08 GMT
COPY docker-entrypoint.sh docker-ensure-initdb.sh /usr/local/bin/ # buildkit
# Wed, 13 Dec 2023 22:17:08 GMT
RUN ln -sT docker-ensure-initdb.sh /usr/local/bin/docker-enforce-initdb.sh # buildkit
# Wed, 13 Dec 2023 22:17:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 13 Dec 2023 22:17:08 GMT
STOPSIGNAL SIGINT
# Wed, 13 Dec 2023 22:17:08 GMT
EXPOSE map[5432/tcp:{}]
# Wed, 13 Dec 2023 22:17:08 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:2c03dbb20264f09924f9eab176da44e5421e74a78b09531d3c63448a7baa7c59`  
		Last Modified: Thu, 30 Nov 2023 23:11:32 GMT  
		Size: 3.3 MB (3333033 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7f976195ad28258b2cce8a3feff1817f99cc57aaba200954d184c38814d91795`  
		Last Modified: Wed, 13 Dec 2023 03:03:02 GMT  
		Size: 1.3 KB (1262 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:03936fc3c66b1d124f91e7128a308d9c4de24f1374198667f3b5dcf9c8a0c88c`  
		Last Modified: Wed, 13 Dec 2023 03:03:02 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9ef347860bc89820d1d75c00c6503b6591fce5c417fbf050dff6eee524917973`  
		Last Modified: Wed, 13 Dec 2023 04:24:54 GMT  
		Size: 86.2 MB (86216606 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9a182a8c10e627868ef230783f2279c07db97636c94c01da9d7c2c2ddaf760eb`  
		Last Modified: Wed, 13 Dec 2023 04:24:51 GMT  
		Size: 8.7 KB (8689 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:dc96849a72a98d6c4de94cec3b9729ae5ab60dce8db0f6be05f1dab93129adfc`  
		Last Modified: Wed, 13 Dec 2023 04:24:51 GMT  
		Size: 128.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1c495160b3d43b7976618c89802c9b88c63b240b474001ceedfa5f1582823a9d`  
		Last Modified: Wed, 13 Dec 2023 04:24:51 GMT  
		Size: 169.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c4599ae63946ddd1bbf3ffeffa8ae229a805f87cb4ff4a0c27b83e1289095aa1`  
		Last Modified: Thu, 14 Dec 2023 20:30:39 GMT  
		Size: 5.3 KB (5341 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:32edbcd8b56e094c915181012f7c2d2b93603771c4919848b93acfc0398568cc`  
		Last Modified: Thu, 14 Dec 2023 20:30:39 GMT  
		Size: 187.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `postgres:12-alpine3.18` - unknown; unknown

```console
$ docker pull postgres@sha256:b9339e466a8b021db1f02c2f0d658f046ccbe8905aa05d38208cf19a22fe6aed
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **840.1 KB (840111 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a387d6fff0a87b567c0bbe7ecda2c643ce641b5b2ba95c01736331224bd09db3`

```dockerfile
```

-	Layers:
	-	`sha256:580e1b0e2e3a0f18ddca201bb6855410abb604aa0cf709723eb726bda06047df`  
		Last Modified: Thu, 14 Dec 2023 20:30:39 GMT  
		Size: 803.6 KB (803639 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:5c7ddf5b296f4cd4563ecb9f6787ace75624757da063fef6a0ec758ea265eff2`  
		Last Modified: Thu, 14 Dec 2023 20:30:38 GMT  
		Size: 36.5 KB (36472 bytes)  
		MIME: application/vnd.in-toto+json

### `postgres:12-alpine3.18` - linux; 386

```console
$ docker pull postgres@sha256:a0741d40d5bd742f05597ba999dd71f45793cf23670ff879f9e936934b18f5d8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.9 MB (95852348 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9f56cb02f523fa2ed59ede90b45aeb69205e6c4ff0ed6b737ee966e6ed808a31`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 28 Sep 2023 20:38:19 GMT
ADD file:8402753f294e403e92353bd65c86a6428c960be5116c0a15484b663a84f66fcd in / 
# Thu, 28 Sep 2023 20:38:20 GMT
CMD ["/bin/sh"]
# Wed, 04 Oct 2023 14:54:45 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql # buildkit
# Wed, 04 Oct 2023 14:54:45 GMT
ENV LANG=en_US.utf8
# Wed, 04 Oct 2023 14:54:45 GMT
RUN mkdir /docker-entrypoint-initdb.d # buildkit
# Wed, 04 Oct 2023 14:54:45 GMT
ENV PG_MAJOR=12
# Wed, 04 Oct 2023 14:54:45 GMT
ENV PG_VERSION=12.16
# Wed, 04 Oct 2023 14:54:45 GMT
ENV PG_SHA256=c5f1fff7a0f93e1ec3746417b0594290ece617b4995ed95b8d527af0ba0e38f3
# Wed, 04 Oct 2023 14:54:45 GMT
ENV DOCKER_PG_LLVM_DEPS=llvm15-dev 		clang15
# Wed, 04 Oct 2023 14:54:45 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		$DOCKER_PG_LLVM_DEPS 		bison 		coreutils 		dpkg-dev dpkg 		flex 		g++ 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openldap-dev 		openssl-dev 		perl-dev 		perl-ipc-run 		perl-utils 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 		export LLVM_CONFIG="/usr/lib/llvm15/bin/llvm-config"; 	export CLANG=clang-15; 		./configure 		--enable-option-checking=fatal 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 		zstd 		icu-data-full 		$([ "$(apk --print-arch)" != 'ppc64le' ] && echo 'nss_wrapper') 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 	echo '{"spdxVersion":"SPDX-2.3","SPDXID":"SPDXRef-DOCUMENT","name":"postgres-sbom","packages":[{"name":"postgres","versionInfo":"12.16","SPDXID":"SPDXRef-Package--postgres","externalRefs":[{"referenceCategory":"PACKAGE-MANAGER","referenceType":"purl","referenceLocator":"pkg:generic/postgres@12.16?os_name=alpine&os_version=3.18"}],"licenseDeclared":"PostgreSQL"}]}' > /usr/local/postgres.spdx.json 	; 	postgres --version # buildkit
# Wed, 04 Oct 2023 14:54:45 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample # buildkit
# Wed, 04 Oct 2023 14:54:45 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 3777 /var/run/postgresql # buildkit
# Wed, 04 Oct 2023 14:54:45 GMT
ENV PGDATA=/var/lib/postgresql/data
# Wed, 04 Oct 2023 14:54:45 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 1777 "$PGDATA" # buildkit
# Wed, 04 Oct 2023 14:54:45 GMT
VOLUME [/var/lib/postgresql/data]
# Wed, 04 Oct 2023 14:54:45 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Wed, 04 Oct 2023 14:54:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 04 Oct 2023 14:54:45 GMT
STOPSIGNAL SIGINT
# Wed, 04 Oct 2023 14:54:45 GMT
EXPOSE map[5432/tcp:{}]
# Wed, 04 Oct 2023 14:54:45 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:dc95107ad2a031a015320bb397f73ec151d738127175b31ad643120697dc7e90`  
		Last Modified: Thu, 28 Sep 2023 20:39:32 GMT  
		Size: 3.2 MB (3235757 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2361d49d5e884bc356dc3a99780fe07508c517deea56eb189574ffb4e7a2dade`  
		Last Modified: Tue, 17 Oct 2023 19:05:33 GMT  
		Size: 1.3 KB (1264 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a068e763669a8f750c7e4e490bc08e5cfcafee3ceeec1268c441caed8de1e3ad`  
		Last Modified: Tue, 17 Oct 2023 19:05:33 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:554c4cd7cd23d123a40f9dd10c22e960299c7f0507ef58453bff2785be2187f0`  
		Last Modified: Tue, 17 Oct 2023 19:05:38 GMT  
		Size: 92.6 MB (92601447 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:441829c9b7489c20cc0825871f33f9d008947d7954392bd93c836325b5480c2a`  
		Last Modified: Tue, 17 Oct 2023 19:05:33 GMT  
		Size: 8.7 KB (8684 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:45d9074f632e5552f352817fac358e7c54206f7fa917912b98605ce1a669b099`  
		Last Modified: Tue, 17 Oct 2023 19:05:34 GMT  
		Size: 128.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a0a937045b7db8d22d91233136b94cfe8db300f1492e5db8bcad97f0f932137e`  
		Last Modified: Tue, 17 Oct 2023 19:05:34 GMT  
		Size: 169.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:30d213c435b802ae62e5d7c8bb68c30846d2222660d605021a8d4683bb076da4`  
		Last Modified: Tue, 17 Oct 2023 19:05:34 GMT  
		Size: 4.8 KB (4783 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `postgres:12-alpine3.18` - unknown; unknown

```console
$ docker pull postgres@sha256:8084b81b32adbcd79ee069c00f2696eb1d13e0a060422aae3e4860fb8780c79a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.5 KB (35463 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:da24b46e49e553fe5181fc450989a6c2725ee9a3c6cbd2f0185448c33fad0fd0`

```dockerfile
```

-	Layers:
	-	`sha256:c470ab2df006d2edea58da160d6a535ed0b656a0b38cd130205aeb6b44906eb5`  
		Last Modified: Tue, 17 Oct 2023 19:05:33 GMT  
		Size: 35.5 KB (35463 bytes)  
		MIME: application/vnd.in-toto+json

### `postgres:12-alpine3.18` - linux; ppc64le

```console
$ docker pull postgres@sha256:cee470e285222c26539c727be6bb510c0cdf8c909f5f36c54b5762fb4f39301f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **96.1 MB (96060633 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:05f54bd0e9b66a39f97edbd4beef3ca5128a241ec24168e85e11b9eff04f0202`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 30 Nov 2023 23:19:04 GMT
ADD file:3450a1687b552498a987f87cb844b7f597c7181d7c3d31943d7b3036d5300d5e in / 
# Thu, 30 Nov 2023 23:19:05 GMT
CMD ["/bin/sh"]
# Wed, 13 Dec 2023 22:17:08 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql # buildkit
# Wed, 13 Dec 2023 22:17:08 GMT
ENV LANG=en_US.utf8
# Wed, 13 Dec 2023 22:17:08 GMT
RUN mkdir /docker-entrypoint-initdb.d # buildkit
# Wed, 13 Dec 2023 22:17:08 GMT
ENV PG_MAJOR=12
# Wed, 13 Dec 2023 22:17:08 GMT
ENV PG_VERSION=12.17
# Wed, 13 Dec 2023 22:17:08 GMT
ENV PG_SHA256=93e8e1b23981d5f03c6c5763f77b28184c1ce4db7194fa466e2edb65d9c1c5f6
# Wed, 13 Dec 2023 22:17:08 GMT
ENV DOCKER_PG_LLVM_DEPS=llvm15-dev 		clang15
# Wed, 13 Dec 2023 22:17:08 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		$DOCKER_PG_LLVM_DEPS 		bison 		coreutils 		dpkg-dev dpkg 		flex 		g++ 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openldap-dev 		openssl-dev 		perl-dev 		perl-ipc-run 		perl-utils 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 		export LLVM_CONFIG="/usr/lib/llvm15/bin/llvm-config"; 	export CLANG=clang-15; 		./configure 		--enable-option-checking=fatal 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 		zstd 		icu-data-full 		$([ "$(apk --print-arch)" != 'ppc64le' ] && echo 'nss_wrapper') 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version # buildkit
# Wed, 13 Dec 2023 22:17:08 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample # buildkit
# Wed, 13 Dec 2023 22:17:08 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 3777 /var/run/postgresql # buildkit
# Wed, 13 Dec 2023 22:17:08 GMT
ENV PGDATA=/var/lib/postgresql/data
# Wed, 13 Dec 2023 22:17:08 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 1777 "$PGDATA" # buildkit
# Wed, 13 Dec 2023 22:17:08 GMT
VOLUME [/var/lib/postgresql/data]
# Wed, 13 Dec 2023 22:17:08 GMT
COPY docker-entrypoint.sh docker-ensure-initdb.sh /usr/local/bin/ # buildkit
# Wed, 13 Dec 2023 22:17:08 GMT
RUN ln -sT docker-ensure-initdb.sh /usr/local/bin/docker-enforce-initdb.sh # buildkit
# Wed, 13 Dec 2023 22:17:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 13 Dec 2023 22:17:08 GMT
STOPSIGNAL SIGINT
# Wed, 13 Dec 2023 22:17:08 GMT
EXPOSE map[5432/tcp:{}]
# Wed, 13 Dec 2023 22:17:08 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:4e13780adf2776477b14ef9c0f4f563f820a2fde166d472218037b979e84d31a`  
		Last Modified: Thu, 30 Nov 2023 23:20:01 GMT  
		Size: 3.3 MB (3348322 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4bced4bbb414e40d55661e37f75a11c9c92e62c379348aee683b29464d6a543e`  
		Last Modified: Wed, 13 Dec 2023 03:23:45 GMT  
		Size: 1.3 KB (1264 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3a4a7ebeb5723f2d6edac750fb7416df4bc23bca2d60b598f19901333b484de5`  
		Last Modified: Wed, 13 Dec 2023 03:23:45 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:26c028d0452d5dfe156ee95f1f1d0c07b943e02a48ea132a0412cdeeb058ab01`  
		Last Modified: Wed, 13 Dec 2023 04:04:59 GMT  
		Size: 92.7 MB (92696399 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5ebd5e78778e2d350823d02a4b138ced1d1dc2ded82a036ed192a730d522bc36`  
		Last Modified: Wed, 13 Dec 2023 04:04:56 GMT  
		Size: 8.7 KB (8697 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d49e53cfcf6e3fd755c070248fdc87015f5ebd427d2c4efb770f007ff6c1ba06`  
		Last Modified: Wed, 13 Dec 2023 04:04:56 GMT  
		Size: 129.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:da8e2a8df68058384110ca50e3cbdb65bc21ff3b0482b059d7619ce601ded983`  
		Last Modified: Wed, 13 Dec 2023 04:04:56 GMT  
		Size: 169.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ca350c0668027f2509c477387a29846567cfe77483344d1d122a55ce3039ac9c`  
		Last Modified: Thu, 14 Dec 2023 19:28:50 GMT  
		Size: 5.3 KB (5347 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3c49e46fb59f7dad7e0fedcfc8d892cacdf720485fe4ca1dafa1fd47c7ff1869`  
		Last Modified: Thu, 14 Dec 2023 19:28:50 GMT  
		Size: 190.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `postgres:12-alpine3.18` - unknown; unknown

```console
$ docker pull postgres@sha256:4851d969b7a58c599bf9a67b93fdc7c037de57f24f586d919eb0a51c712d0d69
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **837.1 KB (837107 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ec01b0a13a515f8b33f877a3b24a57d93b9b61738a80612c310976addeb1084`

```dockerfile
```

-	Layers:
	-	`sha256:2f95912f46ed1ffe34663615d36411021caf40d7bb14d7c657e9b5c3f4de610c`  
		Last Modified: Thu, 14 Dec 2023 19:28:50 GMT  
		Size: 800.6 KB (800603 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:34671e2de2ba970a0aeadd298eda08a76ffc8b203f7fe8fbc7549915b2b553c1`  
		Last Modified: Thu, 14 Dec 2023 19:28:50 GMT  
		Size: 36.5 KB (36504 bytes)  
		MIME: application/vnd.in-toto+json

### `postgres:12-alpine3.18` - linux; s390x

```console
$ docker pull postgres@sha256:68fc1daa389af8db77819a37ac490156b99fee0a7ed2d08eece0a77118c04cdc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.1 MB (92100915 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:01d4705f8a708de4a2671046f7996b2fa806f1c1bae65b29d211def5a9448867`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 30 Nov 2023 22:42:08 GMT
ADD file:50d6643abf7df167a927decd69d193b980557ff73cca48dce86d57e2ff25ad45 in / 
# Thu, 30 Nov 2023 22:42:09 GMT
CMD ["/bin/sh"]
# Wed, 13 Dec 2023 22:17:08 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql # buildkit
# Wed, 13 Dec 2023 22:17:08 GMT
ENV LANG=en_US.utf8
# Wed, 13 Dec 2023 22:17:08 GMT
RUN mkdir /docker-entrypoint-initdb.d # buildkit
# Wed, 13 Dec 2023 22:17:08 GMT
ENV PG_MAJOR=12
# Wed, 13 Dec 2023 22:17:08 GMT
ENV PG_VERSION=12.17
# Wed, 13 Dec 2023 22:17:08 GMT
ENV PG_SHA256=93e8e1b23981d5f03c6c5763f77b28184c1ce4db7194fa466e2edb65d9c1c5f6
# Wed, 13 Dec 2023 22:17:08 GMT
ENV DOCKER_PG_LLVM_DEPS=llvm15-dev 		clang15
# Wed, 13 Dec 2023 22:17:08 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		$DOCKER_PG_LLVM_DEPS 		bison 		coreutils 		dpkg-dev dpkg 		flex 		g++ 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openldap-dev 		openssl-dev 		perl-dev 		perl-ipc-run 		perl-utils 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 		export LLVM_CONFIG="/usr/lib/llvm15/bin/llvm-config"; 	export CLANG=clang-15; 		./configure 		--enable-option-checking=fatal 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 		zstd 		icu-data-full 		$([ "$(apk --print-arch)" != 'ppc64le' ] && echo 'nss_wrapper') 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version # buildkit
# Wed, 13 Dec 2023 22:17:08 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample # buildkit
# Wed, 13 Dec 2023 22:17:08 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 3777 /var/run/postgresql # buildkit
# Wed, 13 Dec 2023 22:17:08 GMT
ENV PGDATA=/var/lib/postgresql/data
# Wed, 13 Dec 2023 22:17:08 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 1777 "$PGDATA" # buildkit
# Wed, 13 Dec 2023 22:17:08 GMT
VOLUME [/var/lib/postgresql/data]
# Wed, 13 Dec 2023 22:17:08 GMT
COPY docker-entrypoint.sh docker-ensure-initdb.sh /usr/local/bin/ # buildkit
# Wed, 13 Dec 2023 22:17:08 GMT
RUN ln -sT docker-ensure-initdb.sh /usr/local/bin/docker-enforce-initdb.sh # buildkit
# Wed, 13 Dec 2023 22:17:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 13 Dec 2023 22:17:08 GMT
STOPSIGNAL SIGINT
# Wed, 13 Dec 2023 22:17:08 GMT
EXPOSE map[5432/tcp:{}]
# Wed, 13 Dec 2023 22:17:08 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:2ea477e1c0c3db3337ee1d7c659f8c465021a65c036998ed3fa3b667d4b30153`  
		Last Modified: Thu, 30 Nov 2023 22:42:52 GMT  
		Size: 3.2 MB (3217454 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5d9eca7e3578b4c16792649c73fb65141bee2d048a99d88a9450e527a42ff6c9`  
		Last Modified: Wed, 13 Dec 2023 01:10:51 GMT  
		Size: 1.3 KB (1262 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6dd2ac5a1eda861bfa4578d408f9e37fb3e11394e1c790c366377d9f15578e1c`  
		Last Modified: Wed, 13 Dec 2023 01:10:51 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ccbf1e0820e49d3c30bfed5e11cf34350a43c65fac7d3e2ea776a4b26e149f51`  
		Last Modified: Wed, 13 Dec 2023 01:41:38 GMT  
		Size: 88.9 MB (88867564 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:04593fc5ca46c22d6f396571f65dadb2dfe435c372947cb6e4a0d58cd00a43b5`  
		Last Modified: Wed, 13 Dec 2023 01:41:37 GMT  
		Size: 8.7 KB (8689 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ad6d43e3414c1b0406e18110c3e94238061c2364e0d71b7d7f090dbd815e6b55`  
		Last Modified: Wed, 13 Dec 2023 01:41:37 GMT  
		Size: 128.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d3bfb7a64f336da1f0b968402ea2bb70801e8169433189649eae56400c83adc2`  
		Last Modified: Wed, 13 Dec 2023 01:41:37 GMT  
		Size: 170.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8045465f19cee9aac190d4a9ea55f7f47754bc91177c6ef4d69ee356cf966aef`  
		Last Modified: Thu, 14 Dec 2023 19:30:34 GMT  
		Size: 5.3 KB (5344 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b8f1f711088b7c86e01240ff2f20f2258437228ed9101e6613421c1975cae788`  
		Last Modified: Thu, 14 Dec 2023 19:30:34 GMT  
		Size: 188.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `postgres:12-alpine3.18` - unknown; unknown

```console
$ docker pull postgres@sha256:2bced84ce6a925ab4e2d01275e0fa4b8d342cf6c243d5766c9d2691cd5ea5fab
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **838.5 KB (838462 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:94c8c7632b91f2bdc62c081185e95ffcf994e3392ac403fff2ab1152035ecc3f`

```dockerfile
```

-	Layers:
	-	`sha256:9367a1ef782212f64518fc779f63e3e897a672378fa31ab170239f80fceac3bd`  
		Last Modified: Thu, 14 Dec 2023 19:30:34 GMT  
		Size: 802.0 KB (801996 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:7b47d48bdbbf2f3308b1646d7fa713fa56c71c4c033903ca0c192b9f404c7b03`  
		Last Modified: Thu, 14 Dec 2023 19:30:34 GMT  
		Size: 36.5 KB (36466 bytes)  
		MIME: application/vnd.in-toto+json
