## `postgres:12-alpine3.19`

```console
$ docker pull postgres@sha256:cac5e044adfcd9b6d67a4b0b9228d83c512e52556d04516a654ca12b2fe03fe4
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 12
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm variant v6
	-	unknown; unknown
	-	linux; arm variant v7
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown
	-	linux; ppc64le
	-	unknown; unknown
	-	linux; s390x
	-	unknown; unknown

### `postgres:12-alpine3.19` - linux; amd64

```console
$ docker pull postgres@sha256:1709d042cb9676a12ffba55fa692fa188a6a718ee7e01f1fbc93549543ea818a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.0 MB (91958077 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:49bf1a422a6155b1530e7f4d62dbcb1d39ba365e64a0bbd32d22cbd7f9a7f4c2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Fri, 08 Dec 2023 01:20:49 GMT
ADD file:1f4eb46669b5b6275af19eb7471a6899a61c276aa7d925b8ae99310b14b75b92 in / 
# Fri, 08 Dec 2023 01:20:49 GMT
CMD ["/bin/sh"]
# Mon, 11 Dec 2023 19:03:58 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql # buildkit
# Mon, 11 Dec 2023 19:03:58 GMT
ENV LANG=en_US.utf8
# Mon, 11 Dec 2023 19:03:58 GMT
RUN mkdir /docker-entrypoint-initdb.d # buildkit
# Mon, 11 Dec 2023 19:03:58 GMT
ENV PG_MAJOR=12
# Mon, 11 Dec 2023 19:03:58 GMT
ENV PG_VERSION=12.17
# Mon, 11 Dec 2023 19:03:58 GMT
ENV PG_SHA256=93e8e1b23981d5f03c6c5763f77b28184c1ce4db7194fa466e2edb65d9c1c5f6
# Mon, 11 Dec 2023 19:03:58 GMT
ENV DOCKER_PG_LLVM_DEPS=llvm15-dev 		clang15
# Mon, 11 Dec 2023 19:03:58 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		$DOCKER_PG_LLVM_DEPS 		bison 		coreutils 		dpkg-dev dpkg 		flex 		g++ 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openldap-dev 		openssl-dev 		perl-dev 		perl-ipc-run 		perl-utils 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 		export LLVM_CONFIG="/usr/lib/llvm15/bin/llvm-config"; 	export CLANG=clang-15; 		./configure 		--enable-option-checking=fatal 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 		zstd 		icu-data-full 		$([ "$(apk --print-arch)" != 'ppc64le' ] && echo 'nss_wrapper') 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version # buildkit
# Mon, 11 Dec 2023 19:03:58 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample # buildkit
# Mon, 11 Dec 2023 19:03:58 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 3777 /var/run/postgresql # buildkit
# Mon, 11 Dec 2023 19:03:58 GMT
ENV PGDATA=/var/lib/postgresql/data
# Mon, 11 Dec 2023 19:03:58 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 1777 "$PGDATA" # buildkit
# Mon, 11 Dec 2023 19:03:58 GMT
VOLUME [/var/lib/postgresql/data]
# Mon, 11 Dec 2023 19:03:58 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 11 Dec 2023 19:03:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 11 Dec 2023 19:03:58 GMT
STOPSIGNAL SIGINT
# Mon, 11 Dec 2023 19:03:58 GMT
EXPOSE map[5432/tcp:{}]
# Mon, 11 Dec 2023 19:03:58 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:661ff4d9561e3fd050929ee5097067c34bafc523ee60f5294a37fd08056a73ca`  
		Last Modified: Fri, 08 Dec 2023 01:21:10 GMT  
		Size: 3.4 MB (3408480 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:278bd74f11e539371177efb5259f105ff73c9c3fa8d84d80f1f9be1e210fe8e8`  
		Last Modified: Tue, 12 Dec 2023 20:53:59 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fae7562a87d1a652a56a6f3039cf8a8032056afe758e1f59aaeb61afb2b1f3ce`  
		Last Modified: Tue, 12 Dec 2023 20:53:46 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:496edfe8aa3216399643da64b727158cccbc742a588a6d194308495056434cba`  
		Last Modified: Tue, 12 Dec 2023 20:54:03 GMT  
		Size: 88.5 MB (88534455 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e02d37e6e05a12ca550da70d0a8c2a1198905798a4550c159283f5beefbc8ef3`  
		Last Modified: Tue, 12 Dec 2023 20:53:59 GMT  
		Size: 8.7 KB (8686 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:31b6f245c3759451966f004829b10014c6f16bfad92868a17b29d50cb1c2db92`  
		Last Modified: Tue, 12 Dec 2023 20:53:59 GMT  
		Size: 128.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:cb4d9165bc64491329fc8a375034e8d460be2f7b1103ac68fe45e1f6cd9916fc`  
		Last Modified: Tue, 12 Dec 2023 20:54:00 GMT  
		Size: 170.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d7f3be2acbac529d63b0801a31107f0c37afe0261870ec22fda03d6d0db51b7d`  
		Last Modified: Tue, 12 Dec 2023 20:54:00 GMT  
		Size: 4.8 KB (4781 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `postgres:12-alpine3.19` - unknown; unknown

```console
$ docker pull postgres@sha256:1110e18e51db7945d46de859fe8cdf8f5b493495ec08b73d8e5e833a3dc82ef9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **839.4 KB (839441 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:16079d6cfd1e89c6891d5da0d803980dff6fae7d4c2fdeb394694dbf93454c9c`

```dockerfile
```

-	Layers:
	-	`sha256:a4b47ed61455c0a61cf74e9e64e98e3210b196bdbe33f2dde4972898c49c1c60`  
		Last Modified: Tue, 12 Dec 2023 20:53:59 GMT  
		Size: 804.8 KB (804761 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:7cc06840652849822446c4570cc00b7ce7e5f55e124aafc2c92a8c58deebb133`  
		Last Modified: Tue, 12 Dec 2023 20:53:59 GMT  
		Size: 34.7 KB (34680 bytes)  
		MIME: application/vnd.in-toto+json

### `postgres:12-alpine3.19` - linux; arm variant v6

```console
$ docker pull postgres@sha256:7746d109a2493417e1943891c7060968d8955bddcbdb7462e9e7ecd02e626692
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **90.9 MB (90859255 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f502b31722042a881f923ca41e094cb982c1bd92ed41813bc474bd16720f0052`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Fri, 08 Dec 2023 01:49:15 GMT
ADD file:d43ed267a41631ce0e5a4ef5aac821a75300a83f85ecb6259f5616852f89e989 in / 
# Fri, 08 Dec 2023 01:49:15 GMT
CMD ["/bin/sh"]
# Mon, 11 Dec 2023 19:03:58 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql # buildkit
# Mon, 11 Dec 2023 19:03:58 GMT
ENV LANG=en_US.utf8
# Mon, 11 Dec 2023 19:03:58 GMT
RUN mkdir /docker-entrypoint-initdb.d # buildkit
# Mon, 11 Dec 2023 19:03:58 GMT
ENV PG_MAJOR=12
# Mon, 11 Dec 2023 19:03:58 GMT
ENV PG_VERSION=12.17
# Mon, 11 Dec 2023 19:03:58 GMT
ENV PG_SHA256=93e8e1b23981d5f03c6c5763f77b28184c1ce4db7194fa466e2edb65d9c1c5f6
# Mon, 11 Dec 2023 19:03:58 GMT
ENV DOCKER_PG_LLVM_DEPS=llvm15-dev 		clang15
# Mon, 11 Dec 2023 19:03:58 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		$DOCKER_PG_LLVM_DEPS 		bison 		coreutils 		dpkg-dev dpkg 		flex 		g++ 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openldap-dev 		openssl-dev 		perl-dev 		perl-ipc-run 		perl-utils 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 		export LLVM_CONFIG="/usr/lib/llvm15/bin/llvm-config"; 	export CLANG=clang-15; 		./configure 		--enable-option-checking=fatal 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 		zstd 		icu-data-full 		$([ "$(apk --print-arch)" != 'ppc64le' ] && echo 'nss_wrapper') 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version # buildkit
# Mon, 11 Dec 2023 19:03:58 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample # buildkit
# Mon, 11 Dec 2023 19:03:58 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 3777 /var/run/postgresql # buildkit
# Mon, 11 Dec 2023 19:03:58 GMT
ENV PGDATA=/var/lib/postgresql/data
# Mon, 11 Dec 2023 19:03:58 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 1777 "$PGDATA" # buildkit
# Mon, 11 Dec 2023 19:03:58 GMT
VOLUME [/var/lib/postgresql/data]
# Mon, 11 Dec 2023 19:03:58 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 11 Dec 2023 19:03:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 11 Dec 2023 19:03:58 GMT
STOPSIGNAL SIGINT
# Mon, 11 Dec 2023 19:03:58 GMT
EXPOSE map[5432/tcp:{}]
# Mon, 11 Dec 2023 19:03:58 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:0803c38384d9fd0f9afaec8fd13d267547b660dcd46bb92a3d63c5d76e78b04c`  
		Last Modified: Fri, 08 Dec 2023 01:49:33 GMT  
		Size: 3.2 MB (3165143 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:93216e21790982df0e80b11285a7034d070a4c27658e9293911a2366ccc04d0f`  
		Last Modified: Tue, 12 Dec 2023 22:34:35 GMT  
		Size: 1.3 KB (1264 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:01f971838734b144cc183181c1a5434902d7407a183c836ec25e35654d41ad57`  
		Last Modified: Tue, 12 Dec 2023 22:34:35 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:41ce450f61f0afc4375c411de3f868cda908ad06c5ded68710df4c116d2d6af9`  
		Last Modified: Wed, 13 Dec 2023 00:00:39 GMT  
		Size: 87.7 MB (87678962 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e44db02cd1dc59e7a8dbf9771b7a8b51e63529181d7cf8375120108962919a92`  
		Last Modified: Wed, 13 Dec 2023 00:00:37 GMT  
		Size: 8.7 KB (8688 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:66e3c9d398141dc7f8c632a138f36b7ec1f71641e711064d495de0de83f3d9a8`  
		Last Modified: Wed, 13 Dec 2023 00:00:36 GMT  
		Size: 128.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:34d42dbe4d8a7d089a4feaaf6e50fcbac09e30541b95097d7f8ff69a37fe655b`  
		Last Modified: Wed, 13 Dec 2023 00:00:36 GMT  
		Size: 171.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:097a3ad0c296238246e08efcea24af6741c5a14a9de6613904cd0be19a25b173`  
		Last Modified: Wed, 13 Dec 2023 00:00:38 GMT  
		Size: 4.8 KB (4783 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `postgres:12-alpine3.19` - unknown; unknown

```console
$ docker pull postgres@sha256:04d3b5f64c0b57b56bbf496d919f056279e5770f68f32acb5b61ca0db12c2caa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.4 KB (34434 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ed659352f3ec811bbf7bfcef116eb0437ec37815d083d0e1cc619f4f620c266`

```dockerfile
```

-	Layers:
	-	`sha256:aa6e28d5b05919139ed1fff5c8a01f5a3c028763c06213695ab6d656407790f8`  
		Last Modified: Wed, 13 Dec 2023 00:00:36 GMT  
		Size: 34.4 KB (34434 bytes)  
		MIME: application/vnd.in-toto+json

### `postgres:12-alpine3.19` - linux; arm variant v7

```console
$ docker pull postgres@sha256:a9464f59e5494e63441ba46d140677c3478c428a88eb2d031df67b38fab47e46
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **85.4 MB (85400907 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:980c4f5db24917af6c39d32b4db4e6a9f16cad357cac92b0273a69026c7e2f28`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Fri, 08 Dec 2023 01:57:20 GMT
ADD file:13b9291053208eec61cd7c97bac2fa154380ad8d10182567763eea3e10c5882f in / 
# Fri, 08 Dec 2023 01:57:20 GMT
CMD ["/bin/sh"]
# Mon, 11 Dec 2023 19:03:58 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql # buildkit
# Mon, 11 Dec 2023 19:03:58 GMT
ENV LANG=en_US.utf8
# Mon, 11 Dec 2023 19:03:58 GMT
RUN mkdir /docker-entrypoint-initdb.d # buildkit
# Mon, 11 Dec 2023 19:03:58 GMT
ENV PG_MAJOR=12
# Mon, 11 Dec 2023 19:03:58 GMT
ENV PG_VERSION=12.17
# Mon, 11 Dec 2023 19:03:58 GMT
ENV PG_SHA256=93e8e1b23981d5f03c6c5763f77b28184c1ce4db7194fa466e2edb65d9c1c5f6
# Mon, 11 Dec 2023 19:03:58 GMT
ENV DOCKER_PG_LLVM_DEPS=llvm15-dev 		clang15
# Mon, 11 Dec 2023 19:03:58 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		$DOCKER_PG_LLVM_DEPS 		bison 		coreutils 		dpkg-dev dpkg 		flex 		g++ 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openldap-dev 		openssl-dev 		perl-dev 		perl-ipc-run 		perl-utils 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 		export LLVM_CONFIG="/usr/lib/llvm15/bin/llvm-config"; 	export CLANG=clang-15; 		./configure 		--enable-option-checking=fatal 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 		zstd 		icu-data-full 		$([ "$(apk --print-arch)" != 'ppc64le' ] && echo 'nss_wrapper') 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version # buildkit
# Mon, 11 Dec 2023 19:03:58 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample # buildkit
# Mon, 11 Dec 2023 19:03:58 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 3777 /var/run/postgresql # buildkit
# Mon, 11 Dec 2023 19:03:58 GMT
ENV PGDATA=/var/lib/postgresql/data
# Mon, 11 Dec 2023 19:03:58 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 1777 "$PGDATA" # buildkit
# Mon, 11 Dec 2023 19:03:58 GMT
VOLUME [/var/lib/postgresql/data]
# Mon, 11 Dec 2023 19:03:58 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 11 Dec 2023 19:03:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 11 Dec 2023 19:03:58 GMT
STOPSIGNAL SIGINT
# Mon, 11 Dec 2023 19:03:58 GMT
EXPOSE map[5432/tcp:{}]
# Mon, 11 Dec 2023 19:03:58 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:1086c24c41097f090ce847d192c11307e1715eeb563a2cf4f410b2a199ae1942`  
		Last Modified: Fri, 08 Dec 2023 01:57:36 GMT  
		Size: 2.9 MB (2918701 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:27ced7217800ddaf8587a82f36031cc326f5fad72be92ddaf3190274dfaf9349`  
		Last Modified: Sat, 09 Dec 2023 05:56:24 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:775f31fd0943cf8717d7b087da7493680a94ea12d1b324c7a9a10aa97815a8d9`  
		Last Modified: Sat, 09 Dec 2023 05:56:24 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:348e91193c216848a3ae4c81d3badf127ac13104ca063cef7c0ddc952bf797d4`  
		Last Modified: Wed, 13 Dec 2023 02:17:04 GMT  
		Size: 82.5 MB (82467060 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0feb86cc41a9d16d72f83c9aef02cb19826a7240b1b9738e84e749bf99b6636b`  
		Last Modified: Wed, 13 Dec 2023 02:17:01 GMT  
		Size: 8.7 KB (8687 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6abe0d23e176fa23b21c5a17e4d101250ce2f7dd36f20d2f343316825cd63646`  
		Last Modified: Wed, 13 Dec 2023 02:17:01 GMT  
		Size: 129.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b0d43dbe3bc5d722ad348aaba016e4debf4a1e88b2c5acde3337a74bfe30358c`  
		Last Modified: Wed, 13 Dec 2023 02:17:01 GMT  
		Size: 169.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a65f88d6a877df6616eea4f1e84dc5ceadf9283869e12e8baa1e65d12c012e55`  
		Last Modified: Wed, 13 Dec 2023 02:17:02 GMT  
		Size: 4.8 KB (4785 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `postgres:12-alpine3.19` - unknown; unknown

```console
$ docker pull postgres@sha256:9c77c01f3f5c41c0a3b4886ebb80283c4323806c6d741b8640f3bb62d7f12223
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **839.4 KB (839446 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8968c984fdd2eeccece19609dcd1daa76e98c900ad94c3e69c43221af2be3d12`

```dockerfile
```

-	Layers:
	-	`sha256:19528ae3084d6b6d1602bf1aa37addd506d5b8c96f3f2dbd19bf40e4f63f4783`  
		Last Modified: Wed, 13 Dec 2023 02:17:01 GMT  
		Size: 804.8 KB (804797 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:5cb5c5981ebf8f59d7ada1d0343ea00c7c2ba8675ce19c4c811300bf56051ed9`  
		Last Modified: Wed, 13 Dec 2023 02:17:01 GMT  
		Size: 34.6 KB (34649 bytes)  
		MIME: application/vnd.in-toto+json

### `postgres:12-alpine3.19` - linux; arm64 variant v8

```console
$ docker pull postgres@sha256:a3838df9b42ee4d611304bbbda354786da3257304e4af1ca43526dbe2fd4f097
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **90.8 MB (90798620 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:656ec81c295ac3700a17cf5be98a6b18eee9125b5e727c8ff4a13ef47a74733c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Fri, 08 Dec 2023 01:39:30 GMT
ADD file:8182c73f869a899cf624a59c400acb8226776d15e4d3a0d240a94e65340540d0 in / 
# Fri, 08 Dec 2023 01:39:30 GMT
CMD ["/bin/sh"]
# Mon, 11 Dec 2023 19:03:58 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql # buildkit
# Mon, 11 Dec 2023 19:03:58 GMT
ENV LANG=en_US.utf8
# Mon, 11 Dec 2023 19:03:58 GMT
RUN mkdir /docker-entrypoint-initdb.d # buildkit
# Mon, 11 Dec 2023 19:03:58 GMT
ENV PG_MAJOR=12
# Mon, 11 Dec 2023 19:03:58 GMT
ENV PG_VERSION=12.17
# Mon, 11 Dec 2023 19:03:58 GMT
ENV PG_SHA256=93e8e1b23981d5f03c6c5763f77b28184c1ce4db7194fa466e2edb65d9c1c5f6
# Mon, 11 Dec 2023 19:03:58 GMT
ENV DOCKER_PG_LLVM_DEPS=llvm15-dev 		clang15
# Mon, 11 Dec 2023 19:03:58 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		$DOCKER_PG_LLVM_DEPS 		bison 		coreutils 		dpkg-dev dpkg 		flex 		g++ 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openldap-dev 		openssl-dev 		perl-dev 		perl-ipc-run 		perl-utils 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 		export LLVM_CONFIG="/usr/lib/llvm15/bin/llvm-config"; 	export CLANG=clang-15; 		./configure 		--enable-option-checking=fatal 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 		zstd 		icu-data-full 		$([ "$(apk --print-arch)" != 'ppc64le' ] && echo 'nss_wrapper') 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version # buildkit
# Mon, 11 Dec 2023 19:03:58 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample # buildkit
# Mon, 11 Dec 2023 19:03:58 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 3777 /var/run/postgresql # buildkit
# Mon, 11 Dec 2023 19:03:58 GMT
ENV PGDATA=/var/lib/postgresql/data
# Mon, 11 Dec 2023 19:03:58 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 1777 "$PGDATA" # buildkit
# Mon, 11 Dec 2023 19:03:58 GMT
VOLUME [/var/lib/postgresql/data]
# Mon, 11 Dec 2023 19:03:58 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 11 Dec 2023 19:03:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 11 Dec 2023 19:03:58 GMT
STOPSIGNAL SIGINT
# Mon, 11 Dec 2023 19:03:58 GMT
EXPOSE map[5432/tcp:{}]
# Mon, 11 Dec 2023 19:03:58 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:c303524923177661067f7eb378c3dd5277088c2676ebd1cd78e68397bb80fdbf`  
		Last Modified: Fri, 08 Dec 2023 01:39:48 GMT  
		Size: 3.3 MB (3347794 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:20a13ecc88456148cc73b8941875af2463232293d6e48313a5d057f52f188e04`  
		Last Modified: Wed, 13 Dec 2023 02:39:21 GMT  
		Size: 1.3 KB (1262 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:01277bc8c6d336069acfe7e4b99842b4e64eb3c6b65bd1dd31d3a6a8a1d98b16`  
		Last Modified: Wed, 13 Dec 2023 02:39:21 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7103bbd8a925387bbbe3bd29d6ff6d3ccd25552154eafbabd23fec46a4227913`  
		Last Modified: Wed, 13 Dec 2023 04:22:35 GMT  
		Size: 87.4 MB (87435674 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:440244623968d68b74d1167a778a0cde5619fd22ce98bdd2a421b705a74fb526`  
		Last Modified: Wed, 13 Dec 2023 04:22:32 GMT  
		Size: 8.7 KB (8689 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2c94d4a27baa261514b53a3ffeb102b8ae03ceb21c07134537ffb010c4b3dcf1`  
		Last Modified: Wed, 13 Dec 2023 04:22:32 GMT  
		Size: 129.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e47b1021120c335c9ae4b9c9e43e82ab53c6bac5cda22ea73eff27f8bb167ec7`  
		Last Modified: Wed, 13 Dec 2023 04:22:33 GMT  
		Size: 169.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3cea58b8bfa67ee718996b025bc68b8e17d7abf94225c15a4b5f8b11c1e1ba7f`  
		Last Modified: Wed, 13 Dec 2023 04:22:33 GMT  
		Size: 4.8 KB (4787 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `postgres:12-alpine3.19` - unknown; unknown

```console
$ docker pull postgres@sha256:f6b3035238819be10e131cc7d289ae7115ef33f504516252777846eaebcc8153
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **839.3 KB (839295 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a8248de5453ffb393c30b95d30496f39019d61bf64ae775708d9260e3f9b42c`

```dockerfile
```

-	Layers:
	-	`sha256:49a996ee8ecedbc44b6605e7ec382e79c4b5377d86547f7a831ef2917fcee07e`  
		Last Modified: Wed, 13 Dec 2023 04:22:32 GMT  
		Size: 804.8 KB (804772 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:069530797a652e6cf28c20a04b0729e3fcc0eb3ba9c0ba140d55c6ad17df8540`  
		Last Modified: Wed, 13 Dec 2023 04:22:32 GMT  
		Size: 34.5 KB (34523 bytes)  
		MIME: application/vnd.in-toto+json

### `postgres:12-alpine3.19` - linux; ppc64le

```console
$ docker pull postgres@sha256:2b1dadf99224a2cbe4ed8159dac1eb0dde72a6eb35bbfa740b9196e3d8c64d87
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **96.4 MB (96421172 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19080ee7317131c5bf93891398533fc31fe0d0519b6902a862de2ebea6b18ad4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Fri, 08 Dec 2023 01:22:51 GMT
ADD file:052421189f8d269382daaaa8beb63c687e4d8ca908c421abdce53bcc627a40b4 in / 
# Fri, 08 Dec 2023 01:22:51 GMT
CMD ["/bin/sh"]
# Mon, 11 Dec 2023 19:03:58 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql # buildkit
# Mon, 11 Dec 2023 19:03:58 GMT
ENV LANG=en_US.utf8
# Mon, 11 Dec 2023 19:03:58 GMT
RUN mkdir /docker-entrypoint-initdb.d # buildkit
# Mon, 11 Dec 2023 19:03:58 GMT
ENV PG_MAJOR=12
# Mon, 11 Dec 2023 19:03:58 GMT
ENV PG_VERSION=12.17
# Mon, 11 Dec 2023 19:03:58 GMT
ENV PG_SHA256=93e8e1b23981d5f03c6c5763f77b28184c1ce4db7194fa466e2edb65d9c1c5f6
# Mon, 11 Dec 2023 19:03:58 GMT
ENV DOCKER_PG_LLVM_DEPS=llvm15-dev 		clang15
# Mon, 11 Dec 2023 19:03:58 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		$DOCKER_PG_LLVM_DEPS 		bison 		coreutils 		dpkg-dev dpkg 		flex 		g++ 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openldap-dev 		openssl-dev 		perl-dev 		perl-ipc-run 		perl-utils 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 		export LLVM_CONFIG="/usr/lib/llvm15/bin/llvm-config"; 	export CLANG=clang-15; 		./configure 		--enable-option-checking=fatal 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 		zstd 		icu-data-full 		$([ "$(apk --print-arch)" != 'ppc64le' ] && echo 'nss_wrapper') 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version # buildkit
# Mon, 11 Dec 2023 19:03:58 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample # buildkit
# Mon, 11 Dec 2023 19:03:58 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 3777 /var/run/postgresql # buildkit
# Mon, 11 Dec 2023 19:03:58 GMT
ENV PGDATA=/var/lib/postgresql/data
# Mon, 11 Dec 2023 19:03:58 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 1777 "$PGDATA" # buildkit
# Mon, 11 Dec 2023 19:03:58 GMT
VOLUME [/var/lib/postgresql/data]
# Mon, 11 Dec 2023 19:03:58 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 11 Dec 2023 19:03:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 11 Dec 2023 19:03:58 GMT
STOPSIGNAL SIGINT
# Mon, 11 Dec 2023 19:03:58 GMT
EXPOSE map[5432/tcp:{}]
# Mon, 11 Dec 2023 19:03:58 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:243ac51c334a47917a84be93e972ee6378987e9b3b917a5a8df29025e161c1f3`  
		Last Modified: Fri, 08 Dec 2023 01:23:14 GMT  
		Size: 3.4 MB (3358233 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6f51ffbccda0d404d0ffeda33fa1a948c925d8f36f5899665a15528b160466a7`  
		Last Modified: Sat, 09 Dec 2023 04:46:09 GMT  
		Size: 1.3 KB (1262 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d4c6b15c27b5856f2fea6198b0dfc83bfee906d7b94102503c986f1e789b8dd3`  
		Last Modified: Sat, 09 Dec 2023 04:46:09 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c9c979a4ca49b17e757509050180edf7e5ad3a227fcb6090c84bc0735b95a4c8`  
		Last Modified: Wed, 13 Dec 2023 04:01:28 GMT  
		Size: 93.0 MB (93047785 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:de7920bef8fbb041a4bdf06e4d81286546f7f99c1544364b9a4b411d83786d2d`  
		Last Modified: Wed, 13 Dec 2023 04:01:25 GMT  
		Size: 8.7 KB (8689 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b973031f92dd202bfe8822d99c1db770d4c0c427c474cbe46f32a833701687dd`  
		Last Modified: Wed, 13 Dec 2023 04:01:25 GMT  
		Size: 129.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:51af5bca0a17b3cd0063673e0c29126d57084ebfc72c4e3ae77fbd9d3c2f61d3`  
		Last Modified: Wed, 13 Dec 2023 04:01:25 GMT  
		Size: 170.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a7f22121252512feb4fc37631cb759f358265828db1893cefe291f48dc1ff109`  
		Last Modified: Wed, 13 Dec 2023 04:01:26 GMT  
		Size: 4.8 KB (4788 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `postgres:12-alpine3.19` - unknown; unknown

```console
$ docker pull postgres@sha256:2ccfe3d9ca5065fa1e33b3585a7323de21c1d0520b2bcefdd953ef6ac7d82f89
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **836.3 KB (836306 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a81f2fe7a477ff500502443888b4005f295338426c0623329dad352d58fdea26`

```dockerfile
```

-	Layers:
	-	`sha256:341509ab10c38dfcfbcd67d83d927324b162e2f4398bed7382086790779295c8`  
		Last Modified: Wed, 13 Dec 2023 04:01:25 GMT  
		Size: 801.7 KB (801744 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:d47f8b91baee1a66ccb521831ea42ed2abf674c6d3ccddcd8f11534fc4775913`  
		Last Modified: Wed, 13 Dec 2023 04:01:25 GMT  
		Size: 34.6 KB (34562 bytes)  
		MIME: application/vnd.in-toto+json

### `postgres:12-alpine3.19` - linux; s390x

```console
$ docker pull postgres@sha256:4ddc035c1dbd56bbee671832016edc619f20662e365389c27f660b1e70652ab1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.7 MB (100692387 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b0a34316089ead0b87420648e1305e8429f6ba0007e3d129642128c8847e691`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Fri, 08 Dec 2023 01:41:50 GMT
ADD file:47e0982fc3ae485c06d46f3c0022afd39ed7ec95fe755c2391e6b0cfcae65dfc in / 
# Fri, 08 Dec 2023 01:41:51 GMT
CMD ["/bin/sh"]
# Mon, 11 Dec 2023 19:03:58 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql # buildkit
# Mon, 11 Dec 2023 19:03:58 GMT
ENV LANG=en_US.utf8
# Mon, 11 Dec 2023 19:03:58 GMT
RUN mkdir /docker-entrypoint-initdb.d # buildkit
# Mon, 11 Dec 2023 19:03:58 GMT
ENV PG_MAJOR=12
# Mon, 11 Dec 2023 19:03:58 GMT
ENV PG_VERSION=12.17
# Mon, 11 Dec 2023 19:03:58 GMT
ENV PG_SHA256=93e8e1b23981d5f03c6c5763f77b28184c1ce4db7194fa466e2edb65d9c1c5f6
# Mon, 11 Dec 2023 19:03:58 GMT
ENV DOCKER_PG_LLVM_DEPS=llvm15-dev 		clang15
# Mon, 11 Dec 2023 19:03:58 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		$DOCKER_PG_LLVM_DEPS 		bison 		coreutils 		dpkg-dev dpkg 		flex 		g++ 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openldap-dev 		openssl-dev 		perl-dev 		perl-ipc-run 		perl-utils 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 		export LLVM_CONFIG="/usr/lib/llvm15/bin/llvm-config"; 	export CLANG=clang-15; 		./configure 		--enable-option-checking=fatal 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 		zstd 		icu-data-full 		$([ "$(apk --print-arch)" != 'ppc64le' ] && echo 'nss_wrapper') 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version # buildkit
# Mon, 11 Dec 2023 19:03:58 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample # buildkit
# Mon, 11 Dec 2023 19:03:58 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 3777 /var/run/postgresql # buildkit
# Mon, 11 Dec 2023 19:03:58 GMT
ENV PGDATA=/var/lib/postgresql/data
# Mon, 11 Dec 2023 19:03:58 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 1777 "$PGDATA" # buildkit
# Mon, 11 Dec 2023 19:03:58 GMT
VOLUME [/var/lib/postgresql/data]
# Mon, 11 Dec 2023 19:03:58 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 11 Dec 2023 19:03:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 11 Dec 2023 19:03:58 GMT
STOPSIGNAL SIGINT
# Mon, 11 Dec 2023 19:03:58 GMT
EXPOSE map[5432/tcp:{}]
# Mon, 11 Dec 2023 19:03:58 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:0fca3ee44ced87b7184bc23390283fdf10cfae0e844a25b785dd11c463815227`  
		Last Modified: Fri, 08 Dec 2023 01:42:30 GMT  
		Size: 3.2 MB (3242332 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:98867b7d9ef52d8ea690ad6ab7a1162c3ffb223f498cfe46c5a0c19b26b5df4a`  
		Last Modified: Sat, 09 Dec 2023 02:05:53 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:eca1d0e320956171da67959a489db8954c94e3093132a48ee544fcaf765d7784`  
		Last Modified: Sat, 09 Dec 2023 02:05:53 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:86dcc63c0f1f0cd3832b5878eab0804eae79acf504382870788f10a3d76775f8`  
		Last Modified: Wed, 13 Dec 2023 01:38:38 GMT  
		Size: 97.4 MB (97434901 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8de82bc7b578c36e30a132f9c67baa664aaa3d115684718a172575e582746d6f`  
		Last Modified: Wed, 13 Dec 2023 01:38:36 GMT  
		Size: 8.7 KB (8692 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5d49d9be391f102fee304d1983b7036941ff44476a5d8edf543d8bfb43a85094`  
		Last Modified: Wed, 13 Dec 2023 01:38:36 GMT  
		Size: 128.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ec21e6a1292c7c8e258de89cae41d4f9ae45b7229b7a561b9a531effaded48b4`  
		Last Modified: Wed, 13 Dec 2023 01:38:36 GMT  
		Size: 169.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:729c679cc0c509373baadfb35aeb24f8c6ed53c3818ff0b2c2cf498c199e320b`  
		Last Modified: Wed, 13 Dec 2023 01:38:37 GMT  
		Size: 4.8 KB (4789 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `postgres:12-alpine3.19` - unknown; unknown

```console
$ docker pull postgres@sha256:0b89f4387072a14bb74b3757064fd1af8bbe1d6a01be41be792b737a37385e35
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **837.6 KB (837639 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:02595f97a4dbc5244667493d6d188feba3ff01a055c1a221c4eb6a4a967c55b6`

```dockerfile
```

-	Layers:
	-	`sha256:b8c9908ae5aff691535c80bfaa2bdd1c28bc7076f27b07f74aa4300ab0246a69`  
		Last Modified: Wed, 13 Dec 2023 01:38:36 GMT  
		Size: 803.1 KB (803125 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:2bbe6412ce8b815dfeb919329a3a0d1b755b9de9d3f2828046355414cfe2af6a`  
		Last Modified: Wed, 13 Dec 2023 01:38:36 GMT  
		Size: 34.5 KB (34514 bytes)  
		MIME: application/vnd.in-toto+json
