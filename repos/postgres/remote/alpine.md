## `postgres:alpine`

```console
$ docker pull postgres@sha256:a1b267d05ee39210d162185f52645687c7e63fbe25b8c58ccd7f81f0a7e2ad97
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

### `postgres:alpine` - linux; amd64

```console
$ docker pull postgres@sha256:cd1f1132c8a8c92e8ba8a876d41710220cb2fe2a6fd7e89981af8f40a6bdba42
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.7 MB (95689476 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:212541dc5d3d47cb2b7333b47464af18acc65b748301bbbee816bbf4c07d20e9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Fri, 08 Dec 2023 01:20:49 GMT
ADD file:1f4eb46669b5b6275af19eb7471a6899a61c276aa7d925b8ae99310b14b75b92 in / 
# Fri, 08 Dec 2023 01:20:49 GMT
CMD ["/bin/sh"]
# Wed, 13 Dec 2023 22:17:08 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql # buildkit
# Wed, 13 Dec 2023 22:17:08 GMT
ENV LANG=en_US.utf8
# Wed, 13 Dec 2023 22:17:08 GMT
RUN mkdir /docker-entrypoint-initdb.d # buildkit
# Wed, 13 Dec 2023 22:17:08 GMT
ENV PG_MAJOR=16
# Wed, 13 Dec 2023 22:17:08 GMT
ENV PG_VERSION=16.1
# Wed, 13 Dec 2023 22:17:08 GMT
ENV PG_SHA256=ce3c4d85d19b0121fe0d3f8ef1fa601f71989e86f8a66f7dc3ad546dd5564fec
# Wed, 13 Dec 2023 22:17:08 GMT
ENV DOCKER_PG_LLVM_DEPS=llvm15-dev 		clang15
# Wed, 13 Dec 2023 22:17:08 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		$DOCKER_PG_LLVM_DEPS 		bison 		coreutils 		dpkg-dev dpkg 		flex 		g++ 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openldap-dev 		openssl-dev 		perl-dev 		perl-ipc-run 		perl-utils 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		icu-dev 		lz4-dev 		zstd-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 		export LLVM_CONFIG="/usr/lib/llvm15/bin/llvm-config"; 	export CLANG=clang-15; 		./configure 		--enable-option-checking=fatal 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 		--with-lz4 		--with-zstd 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 		zstd 		icu-data-full 		$([ "$(apk --print-arch)" != 'ppc64le' ] && echo 'nss_wrapper') 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version # buildkit
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
	-	`sha256:661ff4d9561e3fd050929ee5097067c34bafc523ee60f5294a37fd08056a73ca`  
		Last Modified: Fri, 08 Dec 2023 01:21:10 GMT  
		Size: 3.4 MB (3408480 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8df61a580835a37bebc8249217ef3903a871ab236f12031c158de12eb10a6c8b`  
		Last Modified: Thu, 14 Dec 2023 18:55:21 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:73cae0abb5d44ae73f11f06df41badfa5cd8cd7f80bbf6f9f2863cc54f98e937`  
		Last Modified: Thu, 14 Dec 2023 18:55:22 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:742592b22bac5c8c9e3ffab051ba7754c52ca5d8fdb6b951f27829395823f624`  
		Last Modified: Thu, 14 Dec 2023 18:55:23 GMT  
		Size: 92.3 MB (92264230 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c1c34308d9d2b308162244c638e480b527761227e210df0c5a89cd142e1ac5d6`  
		Last Modified: Thu, 14 Dec 2023 18:55:21 GMT  
		Size: 9.6 KB (9564 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:14bfb625f63b31eb00c6ad1f2807bc802c42f9aa0618a3a9b4bd3d6d85296e0e`  
		Last Modified: Thu, 14 Dec 2023 18:55:19 GMT  
		Size: 129.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:db11692d92da0650b5f4284c75a6254eb3319e35dffd62f8c8d25154a558b218`  
		Last Modified: Thu, 14 Dec 2023 18:55:22 GMT  
		Size: 170.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:38f40ca4652ebed71c2625a1ea2b4131431e03b7315b579f24cb64a3cb36c89e`  
		Last Modified: Thu, 14 Dec 2023 18:55:23 GMT  
		Size: 5.3 KB (5341 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d73c6d20388dbf44e3890ac235c12746ae23876b4372baa83dcc8086a69b54d3`  
		Last Modified: Thu, 14 Dec 2023 18:55:23 GMT  
		Size: 185.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `postgres:alpine` - unknown; unknown

```console
$ docker pull postgres@sha256:2aa16fce7a166a3b43186da643d94ddf477c261116ef5d4179e95776b40ee8e6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **846.3 KB (846296 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:364e013d55221c31f3ef190c299450dfe4f996e5b093587737f892f32cc08a2a`

```dockerfile
```

-	Layers:
	-	`sha256:2a563dd17ec55397ef4c485cb753535ed0972686112ad49744cbc6f110656016`  
		Last Modified: Thu, 14 Dec 2023 18:55:21 GMT  
		Size: 807.9 KB (807923 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:52fdf4ab6a614ddaaee74be7986c38713666cfb896fe1cdd1f29515ad0686d46`  
		Last Modified: Thu, 14 Dec 2023 18:55:21 GMT  
		Size: 38.4 KB (38373 bytes)  
		MIME: application/vnd.in-toto+json

### `postgres:alpine` - linux; arm variant v6

```console
$ docker pull postgres@sha256:3f63da59195f4eb2212c119f5442ad6b79b4c1ecc9da5f53481139c88aac8ba5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.4 MB (94409647 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:28f9c46be8465fb50b0cc61c2744cab1a2e1476c3a3050267d4bd5c3bce3ceab`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Fri, 08 Dec 2023 01:49:15 GMT
ADD file:d43ed267a41631ce0e5a4ef5aac821a75300a83f85ecb6259f5616852f89e989 in / 
# Fri, 08 Dec 2023 01:49:15 GMT
CMD ["/bin/sh"]
# Wed, 13 Dec 2023 22:17:08 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql # buildkit
# Wed, 13 Dec 2023 22:17:08 GMT
ENV LANG=en_US.utf8
# Wed, 13 Dec 2023 22:17:08 GMT
RUN mkdir /docker-entrypoint-initdb.d # buildkit
# Wed, 13 Dec 2023 22:17:08 GMT
ENV PG_MAJOR=16
# Wed, 13 Dec 2023 22:17:08 GMT
ENV PG_VERSION=16.1
# Wed, 13 Dec 2023 22:17:08 GMT
ENV PG_SHA256=ce3c4d85d19b0121fe0d3f8ef1fa601f71989e86f8a66f7dc3ad546dd5564fec
# Wed, 13 Dec 2023 22:17:08 GMT
ENV DOCKER_PG_LLVM_DEPS=llvm15-dev 		clang15
# Wed, 13 Dec 2023 22:17:08 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		$DOCKER_PG_LLVM_DEPS 		bison 		coreutils 		dpkg-dev dpkg 		flex 		g++ 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openldap-dev 		openssl-dev 		perl-dev 		perl-ipc-run 		perl-utils 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		icu-dev 		lz4-dev 		zstd-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 		export LLVM_CONFIG="/usr/lib/llvm15/bin/llvm-config"; 	export CLANG=clang-15; 		./configure 		--enable-option-checking=fatal 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 		--with-lz4 		--with-zstd 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 		zstd 		icu-data-full 		$([ "$(apk --print-arch)" != 'ppc64le' ] && echo 'nss_wrapper') 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version # buildkit
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
	-	`sha256:d71315b5ee5b0e036249894858dd3ac63b35152436e201ca4e40145dcbb172da`  
		Last Modified: Tue, 12 Dec 2023 22:34:38 GMT  
		Size: 91.2 MB (91227735 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:034f274888d6fb10a2122003a2a97a9ace1048a9ae609749a427da242aaf0ba1`  
		Last Modified: Tue, 12 Dec 2023 22:34:35 GMT  
		Size: 9.6 KB (9564 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:117a5e8499ff6d99646751d4dcb38e52901871b7340218b6a9b7750a5c58e144`  
		Last Modified: Tue, 12 Dec 2023 22:34:36 GMT  
		Size: 128.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6b820665b51f66c9c0211d062f1fdb6d59a56428ba09f522ff0c67cb00b81905`  
		Last Modified: Tue, 12 Dec 2023 22:34:36 GMT  
		Size: 169.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:521cf8fd850b8c832d0c5c6fc9874fc3bf0ab781852afe8191be874a8da4f9c7`  
		Last Modified: Thu, 14 Dec 2023 18:54:13 GMT  
		Size: 5.3 KB (5342 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7f542bfe7041e0a58ab88bef5c8d016b0776c94e49d85a64ccd9b180ef4e60f1`  
		Last Modified: Thu, 14 Dec 2023 18:54:13 GMT  
		Size: 186.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `postgres:alpine` - unknown; unknown

```console
$ docker pull postgres@sha256:3b03a49cf9320b82a9838a9dd7dc46a68e49df8a9261d5a008f2d586c9f31a82
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.2 KB (38156 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f0aa3194162eff1e4a52d6ca4d92065cf5c4b29800c8b9393c7d1c93f801945c`

```dockerfile
```

-	Layers:
	-	`sha256:dbeb675af7f910a5a7f54f089becb7ddcced48b39feded453a493816859deefe`  
		Last Modified: Thu, 14 Dec 2023 18:54:13 GMT  
		Size: 38.2 KB (38156 bytes)  
		MIME: application/vnd.in-toto+json

### `postgres:alpine` - linux; arm variant v7

```console
$ docker pull postgres@sha256:c73f611762879db6d2d1edf97dbe6dc92c8bbeb57c62ce7017ead58d78bf0e63
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **88.9 MB (88852347 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1a9ca8abe598a030aed1f71eaa5b51b211bed7bc5e9f0698b84b7f748adb6620`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Fri, 08 Dec 2023 01:57:20 GMT
ADD file:13b9291053208eec61cd7c97bac2fa154380ad8d10182567763eea3e10c5882f in / 
# Fri, 08 Dec 2023 01:57:20 GMT
CMD ["/bin/sh"]
# Wed, 13 Dec 2023 22:17:08 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql # buildkit
# Wed, 13 Dec 2023 22:17:08 GMT
ENV LANG=en_US.utf8
# Wed, 13 Dec 2023 22:17:08 GMT
RUN mkdir /docker-entrypoint-initdb.d # buildkit
# Wed, 13 Dec 2023 22:17:08 GMT
ENV PG_MAJOR=16
# Wed, 13 Dec 2023 22:17:08 GMT
ENV PG_VERSION=16.1
# Wed, 13 Dec 2023 22:17:08 GMT
ENV PG_SHA256=ce3c4d85d19b0121fe0d3f8ef1fa601f71989e86f8a66f7dc3ad546dd5564fec
# Wed, 13 Dec 2023 22:17:08 GMT
ENV DOCKER_PG_LLVM_DEPS=llvm15-dev 		clang15
# Wed, 13 Dec 2023 22:17:08 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		$DOCKER_PG_LLVM_DEPS 		bison 		coreutils 		dpkg-dev dpkg 		flex 		g++ 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openldap-dev 		openssl-dev 		perl-dev 		perl-ipc-run 		perl-utils 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		icu-dev 		lz4-dev 		zstd-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 		export LLVM_CONFIG="/usr/lib/llvm15/bin/llvm-config"; 	export CLANG=clang-15; 		./configure 		--enable-option-checking=fatal 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 		--with-lz4 		--with-zstd 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 		zstd 		icu-data-full 		$([ "$(apk --print-arch)" != 'ppc64le' ] && echo 'nss_wrapper') 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version # buildkit
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
	-	`sha256:e72861c604db855230bd7b80a774ffffdd6024fe92ce087c7ad357a2955ed6bb`  
		Last Modified: Wed, 13 Dec 2023 01:47:42 GMT  
		Size: 85.9 MB (85916879 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a5a981d049d780e843c01944eb17d8718584541b24fc52a2f61940c510479fee`  
		Last Modified: Wed, 13 Dec 2023 01:47:39 GMT  
		Size: 9.6 KB (9563 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a50f2bf67d032b48f9b8036fbe82ad8d9d652cb14948065cb1496474c9d39aa3`  
		Last Modified: Wed, 13 Dec 2023 01:47:39 GMT  
		Size: 129.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e0e35eae078d9e0db0a36170817a7bb1c145958d8aaa28c9e392a3cb3a1c64ca`  
		Last Modified: Wed, 13 Dec 2023 01:47:39 GMT  
		Size: 170.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a5dcee82304c3c1c8062f7cc73c9654ad627de8a66b2100a345f49889792322e`  
		Last Modified: Thu, 14 Dec 2023 19:26:35 GMT  
		Size: 5.3 KB (5342 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:87c5b5dbde7999c9ee2f6728471bf3f200ba56b3a8f638ed0ffaf01970fc84ff`  
		Last Modified: Thu, 14 Dec 2023 19:26:35 GMT  
		Size: 187.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `postgres:alpine` - unknown; unknown

```console
$ docker pull postgres@sha256:269cd3cbb2bd8da855bf1bd90e240643677176a7420e121a324ef8d1d008cf4f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **846.3 KB (846346 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a463019c6cafe7ed2be6e735f1531212ce4b0fcc59e856a154502d4958d06eb3`

```dockerfile
```

-	Layers:
	-	`sha256:971dd171fab2bd2a37cd67d783b013194462b22bd4334689f8fde4ed2f38111b`  
		Last Modified: Thu, 14 Dec 2023 19:26:35 GMT  
		Size: 808.0 KB (807975 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:3ccdf23d0128a2e161897e4766c53ff031d63c2d0fd4ba343b4c2e89c77a643d`  
		Last Modified: Thu, 14 Dec 2023 19:26:35 GMT  
		Size: 38.4 KB (38371 bytes)  
		MIME: application/vnd.in-toto+json

### `postgres:alpine` - linux; arm64 variant v8

```console
$ docker pull postgres@sha256:4dda7d57cd9aabfb16535b3327d710b629485a947b110b993635fae203ecace6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.4 MB (94441203 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:feb0c7a0478c32cfb147ebee685563433537c5802ddddbc7f96cc54ae24db7c1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Fri, 08 Dec 2023 01:39:30 GMT
ADD file:8182c73f869a899cf624a59c400acb8226776d15e4d3a0d240a94e65340540d0 in / 
# Fri, 08 Dec 2023 01:39:30 GMT
CMD ["/bin/sh"]
# Wed, 13 Dec 2023 22:17:08 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql # buildkit
# Wed, 13 Dec 2023 22:17:08 GMT
ENV LANG=en_US.utf8
# Wed, 13 Dec 2023 22:17:08 GMT
RUN mkdir /docker-entrypoint-initdb.d # buildkit
# Wed, 13 Dec 2023 22:17:08 GMT
ENV PG_MAJOR=16
# Wed, 13 Dec 2023 22:17:08 GMT
ENV PG_VERSION=16.1
# Wed, 13 Dec 2023 22:17:08 GMT
ENV PG_SHA256=ce3c4d85d19b0121fe0d3f8ef1fa601f71989e86f8a66f7dc3ad546dd5564fec
# Wed, 13 Dec 2023 22:17:08 GMT
ENV DOCKER_PG_LLVM_DEPS=llvm15-dev 		clang15
# Wed, 13 Dec 2023 22:17:08 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		$DOCKER_PG_LLVM_DEPS 		bison 		coreutils 		dpkg-dev dpkg 		flex 		g++ 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openldap-dev 		openssl-dev 		perl-dev 		perl-ipc-run 		perl-utils 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		icu-dev 		lz4-dev 		zstd-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 		export LLVM_CONFIG="/usr/lib/llvm15/bin/llvm-config"; 	export CLANG=clang-15; 		./configure 		--enable-option-checking=fatal 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 		--with-lz4 		--with-zstd 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 		zstd 		icu-data-full 		$([ "$(apk --print-arch)" != 'ppc64le' ] && echo 'nss_wrapper') 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version # buildkit
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
	-	`sha256:eec44e821ea0eec8e21b2f03ff892b24c41f5cafd0990be4e3d4a4f2146d9beb`  
		Last Modified: Wed, 13 Dec 2023 02:39:24 GMT  
		Size: 91.1 MB (91076639 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:00862d56f995a615bbac1ad730089473f1136f7a3936019f99237031d6f6ec94`  
		Last Modified: Wed, 13 Dec 2023 02:39:21 GMT  
		Size: 9.6 KB (9562 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2572a4326bc7c4fc3e5b3d09db7e53adf33d63acbf73658b316f26c3e5acc1fc`  
		Last Modified: Wed, 13 Dec 2023 02:39:22 GMT  
		Size: 129.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fa3276f3132639a74b449c4edc63c4a46308425614cca5e683f10f16d4018956`  
		Last Modified: Wed, 13 Dec 2023 02:39:22 GMT  
		Size: 169.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:18a643c8e0f634c61f390af972bb47790ff04758a8ddbc5091e040fb908bdcb5`  
		Last Modified: Thu, 14 Dec 2023 20:19:52 GMT  
		Size: 5.3 KB (5345 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b68d07e166304babbc10d8534aef5b75369d27976463fab522acfe4c49c865b6`  
		Last Modified: Thu, 14 Dec 2023 20:19:52 GMT  
		Size: 187.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `postgres:alpine` - unknown; unknown

```console
$ docker pull postgres@sha256:be6b0349ed5f8c86e3db95213a78922a53164a5ca094267c466dd522d70a97a0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **846.2 KB (846159 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:39b31695e817f42047493994527c5b881067b472c11754f973919a3c29e75882`

```dockerfile
```

-	Layers:
	-	`sha256:3dae3f126b04bbff1eebd0f0ac3827e5dac6fcbc1e1df58c03c2db57e2dcf963`  
		Last Modified: Thu, 14 Dec 2023 20:19:52 GMT  
		Size: 807.9 KB (807938 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:3595baaaa77cd4b72663e6fb0871d21945e9489a5df1c6697b3caa51c1082bb9`  
		Last Modified: Thu, 14 Dec 2023 20:19:52 GMT  
		Size: 38.2 KB (38221 bytes)  
		MIME: application/vnd.in-toto+json

### `postgres:alpine` - linux; 386

```console
$ docker pull postgres@sha256:af6180194ef793fc473323e7b8ca5b66016148188459cc88e8e83316f00fb1b7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.0 MB (100964216 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f2d352c038e5c9aa50f3d034cc7d4a796d25b16af5f3c60092d8d0143b467fbf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Fri, 08 Dec 2023 01:38:25 GMT
ADD file:bd52540f209ba362654d795d7893669c819d35011a16f9f319301727a33b3bd9 in / 
# Fri, 08 Dec 2023 01:38:25 GMT
CMD ["/bin/sh"]
# Wed, 13 Dec 2023 22:17:08 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql # buildkit
# Wed, 13 Dec 2023 22:17:08 GMT
ENV LANG=en_US.utf8
# Wed, 13 Dec 2023 22:17:08 GMT
RUN mkdir /docker-entrypoint-initdb.d # buildkit
# Wed, 13 Dec 2023 22:17:08 GMT
ENV PG_MAJOR=16
# Wed, 13 Dec 2023 22:17:08 GMT
ENV PG_VERSION=16.1
# Wed, 13 Dec 2023 22:17:08 GMT
ENV PG_SHA256=ce3c4d85d19b0121fe0d3f8ef1fa601f71989e86f8a66f7dc3ad546dd5564fec
# Wed, 13 Dec 2023 22:17:08 GMT
ENV DOCKER_PG_LLVM_DEPS=llvm15-dev 		clang15
# Wed, 13 Dec 2023 22:17:08 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		$DOCKER_PG_LLVM_DEPS 		bison 		coreutils 		dpkg-dev dpkg 		flex 		g++ 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openldap-dev 		openssl-dev 		perl-dev 		perl-ipc-run 		perl-utils 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		icu-dev 		lz4-dev 		zstd-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 		export LLVM_CONFIG="/usr/lib/llvm15/bin/llvm-config"; 	export CLANG=clang-15; 		./configure 		--enable-option-checking=fatal 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 		--with-lz4 		--with-zstd 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 		zstd 		icu-data-full 		$([ "$(apk --print-arch)" != 'ppc64le' ] && echo 'nss_wrapper') 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version # buildkit
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
	-	`sha256:9acd8b4c9d4385585f74dabb4bc6b3351888710ae37ec5dbd9ea950281b8f9bb`  
		Last Modified: Fri, 08 Dec 2023 01:38:43 GMT  
		Size: 3.2 MB (3244115 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0a41842e56dd64707c6205956f93c803e9733eb4e41ae87a78827616595b985e`  
		Last Modified: Thu, 14 Dec 2023 18:55:30 GMT  
		Size: 1.3 KB (1264 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:862f1cc654121b7ec0d47e5d91eb07b358ed65abcb9e87cc6c8728a96ffd2f78`  
		Last Modified: Thu, 14 Dec 2023 18:55:30 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:133b0a1265a410bb6837ba8c6d4966c496b8b4e94f87cab16716d2972f35a193`  
		Last Modified: Thu, 14 Dec 2023 18:55:50 GMT  
		Size: 97.7 MB (97703337 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d946b41854e630641a6466ee992a2e8a220882595e91d7b426dd94c5acc27b9d`  
		Last Modified: Thu, 14 Dec 2023 18:55:47 GMT  
		Size: 9.6 KB (9563 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:95ea4e97a89add68a5e9fb9d8863e4f9de6c9421b4d39d8ca0070174f89cc77b`  
		Last Modified: Thu, 14 Dec 2023 18:55:47 GMT  
		Size: 129.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:58c48ac9d16a7135c623ed3adee7c13be26114d4abca91c2d4305d305901241c`  
		Last Modified: Thu, 14 Dec 2023 18:55:47 GMT  
		Size: 169.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a4d6d049d8f58a6bcba5561b387ae3db9e6fb90e4095d83c5ba79795cd5a86bf`  
		Last Modified: Thu, 14 Dec 2023 18:55:48 GMT  
		Size: 5.3 KB (5339 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:334efd66e33f5918ead5eaba255092cc679ec365a54cbbd90aa011563938e31b`  
		Last Modified: Thu, 14 Dec 2023 18:55:48 GMT  
		Size: 184.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `postgres:alpine` - unknown; unknown

```console
$ docker pull postgres@sha256:70b54ac7599457436fe5bc33722345b785a0505587d7c2813b233114bff245d0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.1 KB (38107 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c812b615a9751960a7b9fa4875e0cba365a614ca07e135243517acb0c48db379`

```dockerfile
```

-	Layers:
	-	`sha256:cbe6c83fb7622c0bb2ba6f633eeef54532ec02905136c49e70c1ae55b6ef9081`  
		Last Modified: Thu, 14 Dec 2023 18:55:47 GMT  
		Size: 38.1 KB (38107 bytes)  
		MIME: application/vnd.in-toto+json

### `postgres:alpine` - linux; ppc64le

```console
$ docker pull postgres@sha256:1ad73e6eb6bb15821b3d631d73c5472a819dff12c03b482f1bd3c9f08cd78d70
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.3 MB (100321329 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ff3bf83b15be982c26575d3887393dd264f330ed208ca40ef9970d20322bf8b6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Fri, 08 Dec 2023 01:22:51 GMT
ADD file:052421189f8d269382daaaa8beb63c687e4d8ca908c421abdce53bcc627a40b4 in / 
# Fri, 08 Dec 2023 01:22:51 GMT
CMD ["/bin/sh"]
# Wed, 13 Dec 2023 22:17:08 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql # buildkit
# Wed, 13 Dec 2023 22:17:08 GMT
ENV LANG=en_US.utf8
# Wed, 13 Dec 2023 22:17:08 GMT
RUN mkdir /docker-entrypoint-initdb.d # buildkit
# Wed, 13 Dec 2023 22:17:08 GMT
ENV PG_MAJOR=16
# Wed, 13 Dec 2023 22:17:08 GMT
ENV PG_VERSION=16.1
# Wed, 13 Dec 2023 22:17:08 GMT
ENV PG_SHA256=ce3c4d85d19b0121fe0d3f8ef1fa601f71989e86f8a66f7dc3ad546dd5564fec
# Wed, 13 Dec 2023 22:17:08 GMT
ENV DOCKER_PG_LLVM_DEPS=llvm15-dev 		clang15
# Wed, 13 Dec 2023 22:17:08 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		$DOCKER_PG_LLVM_DEPS 		bison 		coreutils 		dpkg-dev dpkg 		flex 		g++ 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openldap-dev 		openssl-dev 		perl-dev 		perl-ipc-run 		perl-utils 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		icu-dev 		lz4-dev 		zstd-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 		export LLVM_CONFIG="/usr/lib/llvm15/bin/llvm-config"; 	export CLANG=clang-15; 		./configure 		--enable-option-checking=fatal 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 		--with-lz4 		--with-zstd 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 		zstd 		icu-data-full 		$([ "$(apk --print-arch)" != 'ppc64le' ] && echo 'nss_wrapper') 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version # buildkit
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
	-	`sha256:5112316be92d5d0e7af2c637ee3c362ab5ae90506ae0af7537129ae3f222fb57`  
		Last Modified: Wed, 13 Dec 2023 02:15:10 GMT  
		Size: 96.9 MB (96946315 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ad50ef0ec22e20cd08b4521d3376888118c0901b67c7ff14a5fe31b5730013f6`  
		Last Modified: Wed, 13 Dec 2023 02:15:07 GMT  
		Size: 9.6 KB (9572 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f81fe48d1cbaea009f509d8c9d00094a7d6e0a5431b3e408d0827833b20d7c24`  
		Last Modified: Wed, 13 Dec 2023 02:15:07 GMT  
		Size: 128.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:840e83be41fffdfdb6435fc54a3af5807f3f661ae31df6a2f8df5647a6cb7457`  
		Last Modified: Wed, 13 Dec 2023 02:15:07 GMT  
		Size: 170.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:188eed5e9dfdfd4e39ef9432b54b05e1e478597fd87cfc68f2a198d2963f2a85`  
		Last Modified: Thu, 14 Dec 2023 19:16:56 GMT  
		Size: 5.3 KB (5346 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e3553fa11a9d236e7a1cb318441c6c987994b2e4fc3cc4a7daf205a8da7cd604`  
		Last Modified: Thu, 14 Dec 2023 19:16:56 GMT  
		Size: 187.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `postgres:alpine` - unknown; unknown

```console
$ docker pull postgres@sha256:7ce8c8947bec365c16f9025d12bd82ac838647f56caa66cd84f8771d66828673
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **843.2 KB (843186 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f121120f1011474bab27707d6f71a9269e5078fcee5cdfab08cee5b92c064d83`

```dockerfile
```

-	Layers:
	-	`sha256:c8d52783e68806e950a975564f5037ee986178134e070307b8a7372e2a76a99d`  
		Last Modified: Thu, 14 Dec 2023 19:16:56 GMT  
		Size: 804.9 KB (804918 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:27286c1f07b1f6cbfcc73ddfd2c6ce703547ecd5c6316cbbcbf62696e9ff3707`  
		Last Modified: Thu, 14 Dec 2023 19:16:56 GMT  
		Size: 38.3 KB (38268 bytes)  
		MIME: application/vnd.in-toto+json

### `postgres:alpine` - linux; s390x

```console
$ docker pull postgres@sha256:cf944a797dcbdab4f45799de67c03c7b02e5c514a06dfc3364019e3e2d250e69
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.6 MB (104598883 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ae582b1d8fab2ce4f9278b1c98d4a9a45fabaf69fda9332d5438a7c35d2c7c3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Fri, 08 Dec 2023 01:41:50 GMT
ADD file:47e0982fc3ae485c06d46f3c0022afd39ed7ec95fe755c2391e6b0cfcae65dfc in / 
# Fri, 08 Dec 2023 01:41:51 GMT
CMD ["/bin/sh"]
# Wed, 13 Dec 2023 22:17:08 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql # buildkit
# Wed, 13 Dec 2023 22:17:08 GMT
ENV LANG=en_US.utf8
# Wed, 13 Dec 2023 22:17:08 GMT
RUN mkdir /docker-entrypoint-initdb.d # buildkit
# Wed, 13 Dec 2023 22:17:08 GMT
ENV PG_MAJOR=16
# Wed, 13 Dec 2023 22:17:08 GMT
ENV PG_VERSION=16.1
# Wed, 13 Dec 2023 22:17:08 GMT
ENV PG_SHA256=ce3c4d85d19b0121fe0d3f8ef1fa601f71989e86f8a66f7dc3ad546dd5564fec
# Wed, 13 Dec 2023 22:17:08 GMT
ENV DOCKER_PG_LLVM_DEPS=llvm15-dev 		clang15
# Wed, 13 Dec 2023 22:17:08 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		$DOCKER_PG_LLVM_DEPS 		bison 		coreutils 		dpkg-dev dpkg 		flex 		g++ 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openldap-dev 		openssl-dev 		perl-dev 		perl-ipc-run 		perl-utils 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		icu-dev 		lz4-dev 		zstd-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 		export LLVM_CONFIG="/usr/lib/llvm15/bin/llvm-config"; 	export CLANG=clang-15; 		./configure 		--enable-option-checking=fatal 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 		--with-lz4 		--with-zstd 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 		zstd 		icu-data-full 		$([ "$(apk --print-arch)" != 'ppc64le' ] && echo 'nss_wrapper') 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version # buildkit
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
	-	`sha256:a7f7010d76ceff0dd4d000eb71ffad9ed7a5b575adfbe651d85a97439db3c560`  
		Last Modified: Wed, 13 Dec 2023 00:46:10 GMT  
		Size: 101.3 MB (101339778 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:686b71a99b6050515a9c6d7c8e1fad4d4fc041f26d668347d98acd8bb432cc23`  
		Last Modified: Wed, 13 Dec 2023 00:46:05 GMT  
		Size: 9.6 KB (9567 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:00267657344730f1fffe25c3b23bc0234549149769ff7fdceb16e66bf3f96353`  
		Last Modified: Wed, 13 Dec 2023 00:46:05 GMT  
		Size: 128.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:049476ec6f047890d876f7e6b687ce80a4acec89f0edc0b47d3a2d69fd8e28fc`  
		Last Modified: Wed, 13 Dec 2023 00:46:06 GMT  
		Size: 170.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3055e3f00dc9be2123487c9f4a8674b7c4bef8a355ebce85ea9e8f842a0f556d`  
		Last Modified: Thu, 14 Dec 2023 19:09:00 GMT  
		Size: 5.3 KB (5345 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d68620b29ae3a8009a59f250628781f7aedb7c247f33e556c47fbd82cd9e8204`  
		Last Modified: Thu, 14 Dec 2023 19:09:00 GMT  
		Size: 187.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `postgres:alpine` - unknown; unknown

```console
$ docker pull postgres@sha256:c948364c9830eb1c2c69d1a5eba5a8646833ed96fb8cf6880fae72aab001c4bd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **844.5 KB (844500 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c7fc0dc491b1ae58a055d3872efee15577f515919ea7a9583d1a23167e2d44de`

```dockerfile
```

-	Layers:
	-	`sha256:7561819123f2c91c980d42da1582b021dddd41438e400f155ba26dce3e3cb7aa`  
		Last Modified: Thu, 14 Dec 2023 19:09:00 GMT  
		Size: 806.3 KB (806287 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:6ee697db750c61f90257b8428cb970b3d737aa41a9c81a461e753b478e178dc9`  
		Last Modified: Thu, 14 Dec 2023 19:09:00 GMT  
		Size: 38.2 KB (38213 bytes)  
		MIME: application/vnd.in-toto+json
