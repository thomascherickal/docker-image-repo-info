## `postgres:alpine3.18`

```console
$ docker pull postgres@sha256:d3d9e58fdef1e21ef33af717faffd1959ab9ac1839d05a6bb211daa6c551b07f
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

### `postgres:alpine3.18` - linux; amd64

```console
$ docker pull postgres@sha256:69881b88ad67daa32c19ada50465f08219a96a197f6efcff3e5ee3d6f9bc8fe0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.3 MB (94257872 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dcf60561e4ebcf10745b9bfa6ed37c13d7a0cc6029a31ecdd0ea7950f0f6b283`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 30 Nov 2023 23:22:52 GMT
ADD file:fc714080c3bcbbce7ac746a10d7b4355ffa36293a8d435d62cd5359ea8eb8364 in / 
# Thu, 30 Nov 2023 23:22:52 GMT
CMD ["/bin/sh"]
# Mon, 11 Dec 2023 19:03:58 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql # buildkit
# Mon, 11 Dec 2023 19:03:58 GMT
ENV LANG=en_US.utf8
# Mon, 11 Dec 2023 19:03:58 GMT
RUN mkdir /docker-entrypoint-initdb.d # buildkit
# Mon, 11 Dec 2023 19:03:58 GMT
ENV PG_MAJOR=16
# Mon, 11 Dec 2023 19:03:58 GMT
ENV PG_VERSION=16.1
# Mon, 11 Dec 2023 19:03:58 GMT
ENV PG_SHA256=ce3c4d85d19b0121fe0d3f8ef1fa601f71989e86f8a66f7dc3ad546dd5564fec
# Mon, 11 Dec 2023 19:03:58 GMT
ENV DOCKER_PG_LLVM_DEPS=llvm15-dev 		clang15
# Mon, 11 Dec 2023 19:03:58 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		$DOCKER_PG_LLVM_DEPS 		bison 		coreutils 		dpkg-dev dpkg 		flex 		g++ 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openldap-dev 		openssl-dev 		perl-dev 		perl-ipc-run 		perl-utils 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		icu-dev 		lz4-dev 		zstd-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 		export LLVM_CONFIG="/usr/lib/llvm15/bin/llvm-config"; 	export CLANG=clang-15; 		./configure 		--enable-option-checking=fatal 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 		--with-lz4 		--with-zstd 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 		zstd 		icu-data-full 		$([ "$(apk --print-arch)" != 'ppc64le' ] && echo 'nss_wrapper') 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version # buildkit
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
	-	`sha256:c926b61bad3b94ae7351bafd0c184c159ebf0643b085f7ef1d47ecdc7316833c`  
		Last Modified: Thu, 30 Nov 2023 23:23:28 GMT  
		Size: 3.4 MB (3402422 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2557d8362158a3555cd1cddb3130778622e103045017aff42d1981bd5183b90f`  
		Last Modified: Tue, 12 Dec 2023 20:54:10 GMT  
		Size: 1.3 KB (1263 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c36fe88ffa30016f71e79ca364315be5820a51e5ac5940930190e7969b79c879`  
		Last Modified: Tue, 12 Dec 2023 20:54:10 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:988276ebbdb812b7d825c7a70218581c7caf6b33120875ff7e77e2ba4ff937b5`  
		Last Modified: Tue, 12 Dec 2023 20:54:12 GMT  
		Size: 90.8 MB (90839424 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4474e158aa55585c0e8a9ae1966a312e689092f2aac7da05885d247228198726`  
		Last Modified: Tue, 12 Dec 2023 20:54:10 GMT  
		Size: 9.6 KB (9562 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3653907409e7935968ed90cdb5017ea4dd3d9df95e838bc41df5dd302e2e4f2d`  
		Last Modified: Tue, 12 Dec 2023 20:54:10 GMT  
		Size: 129.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fb454b7251f4f350cd913e1f6c241ba04cb88ec6469ce0aebca0003468a7c6ce`  
		Last Modified: Tue, 12 Dec 2023 20:54:10 GMT  
		Size: 170.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2fa38e2660ea5744a516f89476fe02fc1bbe3cb47f3438d5719bbe63b00f9686`  
		Last Modified: Tue, 12 Dec 2023 20:54:11 GMT  
		Size: 4.8 KB (4786 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `postgres:alpine3.18` - unknown; unknown

```console
$ docker pull postgres@sha256:88ea331f1a9f379c25ac6b38f8e6271e8aaaf4cc048c52e2c9fb22a5bb2309c7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **841.4 KB (841372 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b43e2ad2c7c2f26236911adfde893e85d01e5380a075072f6a82eee0673be139`

```dockerfile
```

-	Layers:
	-	`sha256:8cd28f8ad2914167cbe614dae3b0c0439305ae731846adf73d87486c0c43030d`  
		Last Modified: Tue, 12 Dec 2023 20:54:10 GMT  
		Size: 806.5 KB (806494 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:f95d621b12cf3b04d7cfe2fdfd090fdc14c1cf671b23f2e709813d6eaa8cf9fe`  
		Last Modified: Tue, 12 Dec 2023 20:54:09 GMT  
		Size: 34.9 KB (34878 bytes)  
		MIME: application/vnd.in-toto+json

### `postgres:alpine3.18` - linux; arm variant v6

```console
$ docker pull postgres@sha256:c44233ec694660a96b376f013896b0d991bbef20d877d3ed966b2f2cf1cd7ec9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.9 MB (92892824 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:38b205ae595f4821b62ab5d9674dc9a239c40bbdd0a54cf4a1fccad552164322`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 30 Nov 2023 22:49:18 GMT
ADD file:dbf65487d049081dc2d39b3d99d2c64b6c89754e7e2996a46169d3512e59f32a in / 
# Thu, 30 Nov 2023 22:49:18 GMT
CMD ["/bin/sh"]
# Mon, 11 Dec 2023 19:03:58 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql # buildkit
# Mon, 11 Dec 2023 19:03:58 GMT
ENV LANG=en_US.utf8
# Mon, 11 Dec 2023 19:03:58 GMT
RUN mkdir /docker-entrypoint-initdb.d # buildkit
# Mon, 11 Dec 2023 19:03:58 GMT
ENV PG_MAJOR=16
# Mon, 11 Dec 2023 19:03:58 GMT
ENV PG_VERSION=16.1
# Mon, 11 Dec 2023 19:03:58 GMT
ENV PG_SHA256=ce3c4d85d19b0121fe0d3f8ef1fa601f71989e86f8a66f7dc3ad546dd5564fec
# Mon, 11 Dec 2023 19:03:58 GMT
ENV DOCKER_PG_LLVM_DEPS=llvm15-dev 		clang15
# Mon, 11 Dec 2023 19:03:58 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		$DOCKER_PG_LLVM_DEPS 		bison 		coreutils 		dpkg-dev dpkg 		flex 		g++ 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openldap-dev 		openssl-dev 		perl-dev 		perl-ipc-run 		perl-utils 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		icu-dev 		lz4-dev 		zstd-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 		export LLVM_CONFIG="/usr/lib/llvm15/bin/llvm-config"; 	export CLANG=clang-15; 		./configure 		--enable-option-checking=fatal 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 		--with-lz4 		--with-zstd 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 		zstd 		icu-data-full 		$([ "$(apk --print-arch)" != 'ppc64le' ] && echo 'nss_wrapper') 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version # buildkit
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
	-	`sha256:46b7e70f263defcda03c9b5a82322120ef90d426dacdeb76261afa3a7410c560`  
		Last Modified: Tue, 12 Dec 2023 22:40:42 GMT  
		Size: 89.7 MB (89729930 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1fc88bda956a77fd23696d97ddc61bdaeeb987389a1889a67fcdc0c3caded8ef`  
		Last Modified: Tue, 12 Dec 2023 22:40:38 GMT  
		Size: 9.6 KB (9565 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:eadaba0853959f371af65ef7784095a6f968c0b437a4462360954f0da867f39f`  
		Last Modified: Tue, 12 Dec 2023 22:40:39 GMT  
		Size: 129.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:453fa2d1b1aa813178a4ee1fd58d7054fd68d257dd2601d70815c0cb051ef509`  
		Last Modified: Tue, 12 Dec 2023 22:40:39 GMT  
		Size: 169.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:30214523781a975882b9be23844be12c4cee5e9728343aa44e648fa21d48f977`  
		Last Modified: Tue, 12 Dec 2023 22:40:40 GMT  
		Size: 4.8 KB (4785 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `postgres:alpine3.18` - unknown; unknown

```console
$ docker pull postgres@sha256:0e3579b326ef8955417a1730ee191897916c258cbd45fb4b674e6f72b6244841
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.8 KB (34790 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f1c52149565eed4ab5c22b224af07eedec596cde3e2c5c42b611d3a92652aea1`

```dockerfile
```

-	Layers:
	-	`sha256:cfc94011f4c8db643ec8fc11a4636674eebbba0e6be95f81cae46abe8d511214`  
		Last Modified: Tue, 12 Dec 2023 22:40:38 GMT  
		Size: 34.8 KB (34790 bytes)  
		MIME: application/vnd.in-toto+json

### `postgres:alpine3.18` - linux; arm variant v7

```console
$ docker pull postgres@sha256:74f9f33f32d911a5f05d5fc90e5d98a09503e0ab0c921865718a14fb19532c0d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.5 MB (87536900 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:85553e62dc58a1761cc3717ca116000fbb10196ab0ef123170825ab33eff8121`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 30 Nov 2023 22:49:28 GMT
ADD file:dcb85d43d1fb96861612c42288878b13debfa9d0b956adea1f2472d0c50f0144 in / 
# Thu, 30 Nov 2023 22:49:29 GMT
CMD ["/bin/sh"]
# Mon, 11 Dec 2023 19:03:58 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql # buildkit
# Mon, 11 Dec 2023 19:03:58 GMT
ENV LANG=en_US.utf8
# Mon, 11 Dec 2023 19:03:58 GMT
RUN mkdir /docker-entrypoint-initdb.d # buildkit
# Mon, 11 Dec 2023 19:03:58 GMT
ENV PG_MAJOR=16
# Mon, 11 Dec 2023 19:03:58 GMT
ENV PG_VERSION=16.1
# Mon, 11 Dec 2023 19:03:58 GMT
ENV PG_SHA256=ce3c4d85d19b0121fe0d3f8ef1fa601f71989e86f8a66f7dc3ad546dd5564fec
# Mon, 11 Dec 2023 19:03:58 GMT
ENV DOCKER_PG_LLVM_DEPS=llvm15-dev 		clang15
# Mon, 11 Dec 2023 19:03:58 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		$DOCKER_PG_LLVM_DEPS 		bison 		coreutils 		dpkg-dev dpkg 		flex 		g++ 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openldap-dev 		openssl-dev 		perl-dev 		perl-ipc-run 		perl-utils 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		icu-dev 		lz4-dev 		zstd-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 		export LLVM_CONFIG="/usr/lib/llvm15/bin/llvm-config"; 	export CLANG=clang-15; 		./configure 		--enable-option-checking=fatal 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 		--with-lz4 		--with-zstd 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 		zstd 		icu-data-full 		$([ "$(apk --print-arch)" != 'ppc64le' ] && echo 'nss_wrapper') 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version # buildkit
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
	-	`sha256:3bcc7cbad1f562c541e23d6ec52717b2c49ceaf88e535fb7d7e9501316f0fc54`  
		Last Modified: Wed, 13 Dec 2023 01:53:32 GMT  
		Size: 84.6 MB (84619870 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6aaa0d637011f4e4715941b8ad30f8ff177128978cf6a8c0bc673831d717ab7d`  
		Last Modified: Wed, 13 Dec 2023 01:53:29 GMT  
		Size: 9.6 KB (9564 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f7c0cdf1d5ec3c1316e174cb38b2c88641af332280497a5ddf826e6aa784fd60`  
		Last Modified: Wed, 13 Dec 2023 01:53:30 GMT  
		Size: 128.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4aff6cccaba07f1abf3e8a3623c238fb015dcde5dee20d17c723d7e8352abea0`  
		Last Modified: Wed, 13 Dec 2023 01:53:30 GMT  
		Size: 168.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f7c30adc67ccc3365e49e88faad7d0452b4b172d83ff6bf14f15def2e0daed1d`  
		Last Modified: Wed, 13 Dec 2023 01:53:30 GMT  
		Size: 4.8 KB (4788 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `postgres:alpine3.18` - unknown; unknown

```console
$ docker pull postgres@sha256:24359c08e419fc267171e0676e6b092feeb83bb9f3e8be593145581dc61f418a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **841.4 KB (841361 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f5c6314d43fdfe7aa6cf5cd9be041d993dcc3d4d9bcd09f7d202a75a11f1056a`

```dockerfile
```

-	Layers:
	-	`sha256:2e5ca639652697315954f9acc2273352386a14e07f2937fd01723ca6d545b034`  
		Last Modified: Wed, 13 Dec 2023 01:53:29 GMT  
		Size: 806.5 KB (806522 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:c26d138f01ac8f056c9b6ff94773c4374040e92559a4ca0d2a7e822e521fa749`  
		Last Modified: Wed, 13 Dec 2023 01:53:29 GMT  
		Size: 34.8 KB (34839 bytes)  
		MIME: application/vnd.in-toto+json

### `postgres:alpine3.18` - linux; arm64 variant v8

```console
$ docker pull postgres@sha256:1ccb6f61e86e8f92a9a3c30a983db63de181780514317189f2b31df86149f4f4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.2 MB (93201547 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f9c56f34f1a7ae7c89cdff55ee316c8bdad91171d875045646c5975951a38ce5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 30 Nov 2023 23:11:03 GMT
ADD file:d8a30995bbcd627f084912c728fda5483b6ba486de25af588a0956069d0bd7ad in / 
# Thu, 30 Nov 2023 23:11:03 GMT
CMD ["/bin/sh"]
# Mon, 11 Dec 2023 19:03:58 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql # buildkit
# Mon, 11 Dec 2023 19:03:58 GMT
ENV LANG=en_US.utf8
# Mon, 11 Dec 2023 19:03:58 GMT
RUN mkdir /docker-entrypoint-initdb.d # buildkit
# Mon, 11 Dec 2023 19:03:58 GMT
ENV PG_MAJOR=16
# Mon, 11 Dec 2023 19:03:58 GMT
ENV PG_VERSION=16.1
# Mon, 11 Dec 2023 19:03:58 GMT
ENV PG_SHA256=ce3c4d85d19b0121fe0d3f8ef1fa601f71989e86f8a66f7dc3ad546dd5564fec
# Mon, 11 Dec 2023 19:03:58 GMT
ENV DOCKER_PG_LLVM_DEPS=llvm15-dev 		clang15
# Mon, 11 Dec 2023 19:03:58 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		$DOCKER_PG_LLVM_DEPS 		bison 		coreutils 		dpkg-dev dpkg 		flex 		g++ 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openldap-dev 		openssl-dev 		perl-dev 		perl-ipc-run 		perl-utils 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		icu-dev 		lz4-dev 		zstd-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 		export LLVM_CONFIG="/usr/lib/llvm15/bin/llvm-config"; 	export CLANG=clang-15; 		./configure 		--enable-option-checking=fatal 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 		--with-lz4 		--with-zstd 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 		zstd 		icu-data-full 		$([ "$(apk --print-arch)" != 'ppc64le' ] && echo 'nss_wrapper') 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version # buildkit
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
	-	`sha256:f3aa49f43d2325dcd2ea85b08b44a7bb660db13a09e65b63d2cb3cbd51b7149b`  
		Last Modified: Wed, 13 Dec 2023 03:03:05 GMT  
		Size: 89.9 MB (89852488 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f66a5ab8125ab10899fd42c8d424b7a4aeca07351aaf0520e4a2d96f345c2c0a`  
		Last Modified: Wed, 13 Dec 2023 03:03:02 GMT  
		Size: 9.6 KB (9562 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8779fd16670501c3098e5ee16237d336412708dfc65643d180b531fa4e4e4917`  
		Last Modified: Wed, 13 Dec 2023 03:03:03 GMT  
		Size: 128.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:91eaf998d605de6262c48142125f2cb207223f53aecaaed50e5828d697085b6a`  
		Last Modified: Wed, 13 Dec 2023 03:03:04 GMT  
		Size: 170.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6377a21a48db01347dd24a39ee6064cf88a28bd024797667fe8fff04b9ce279e`  
		Last Modified: Wed, 13 Dec 2023 03:03:05 GMT  
		Size: 4.8 KB (4788 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `postgres:alpine3.18` - unknown; unknown

```console
$ docker pull postgres@sha256:4cb1e2353129cc1430fe972e938466c1ea227b021a2aa2eac97022fed1529451
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **841.4 KB (841389 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4eb1cd5d15f1d1a46e72bbe0c675ff6d33412e159ec4e1df0335f1e6337b510`

```dockerfile
```

-	Layers:
	-	`sha256:c378349989483703aa4e9fd0117cb1c081661992d13611f52e7aa7b60abc7056`  
		Last Modified: Wed, 13 Dec 2023 03:03:02 GMT  
		Size: 806.5 KB (806503 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:d53fcc6fd71e3cc2539dde9a9566e46ce1b49a02a8f5ad808694fa9ec6e3ac7f`  
		Last Modified: Wed, 13 Dec 2023 03:03:02 GMT  
		Size: 34.9 KB (34886 bytes)  
		MIME: application/vnd.in-toto+json

### `postgres:alpine3.18` - linux; 386

```console
$ docker pull postgres@sha256:9617c671922208a046ca296fdd9444d3d33e6f37459b9efd29d9c3810c87f153
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.6 MB (99637266 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e3deaf80a331297519e75e63935e98bbb92334283e70ef7a22af6d6d4a5bd053`
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
ENV PG_MAJOR=16
# Wed, 04 Oct 2023 14:54:45 GMT
ENV PG_VERSION=16.0
# Wed, 04 Oct 2023 14:54:45 GMT
ENV PG_SHA256=df9e823eb22330444e1d48e52cc65135a652a6fdb3ce325e3f08549339f51b99
# Wed, 04 Oct 2023 14:54:45 GMT
ENV DOCKER_PG_LLVM_DEPS=llvm15-dev 		clang15
# Wed, 04 Oct 2023 14:54:45 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		$DOCKER_PG_LLVM_DEPS 		bison 		coreutils 		dpkg-dev dpkg 		flex 		g++ 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openldap-dev 		openssl-dev 		perl-dev 		perl-ipc-run 		perl-utils 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		icu-dev 		lz4-dev 		zstd-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 		export LLVM_CONFIG="/usr/lib/llvm15/bin/llvm-config"; 	export CLANG=clang-15; 		./configure 		--enable-option-checking=fatal 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 		--with-lz4 		--with-zstd 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 		zstd 		icu-data-full 		$([ "$(apk --print-arch)" != 'ppc64le' ] && echo 'nss_wrapper') 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 	echo '{"spdxVersion":"SPDX-2.3","SPDXID":"SPDXRef-DOCUMENT","name":"postgres-sbom","packages":[{"name":"postgres","versionInfo":"16.0","SPDXID":"SPDXRef-Package--postgres","externalRefs":[{"referenceCategory":"PACKAGE-MANAGER","referenceType":"purl","referenceLocator":"pkg:generic/postgres@16.0?os_name=alpine&os_version=3.18"}],"licenseDeclared":"PostgreSQL"}]}' > /usr/local/postgres.spdx.json 	; 	postgres --version # buildkit
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
	-	`sha256:040933531e816b9c15b2e02d0f3ac6e0b50f774a57f292832999dd2be460ede2`  
		Last Modified: Tue, 17 Oct 2023 19:06:23 GMT  
		Size: 1.3 KB (1263 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:912e4698639810e9a147b355702c03f07a8cca29f4f0a2e8056568add01d974d`  
		Last Modified: Tue, 17 Oct 2023 19:06:23 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ef5823f4427326f9a8458ce25d51a20f8f6cf7b1417cbb92eb230f4eb4bc677e`  
		Last Modified: Tue, 17 Oct 2023 19:06:30 GMT  
		Size: 96.4 MB (96385484 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:59b167e5cb011be2e494748f40df10166c5342fe4f572684057fc3e9ccb63659`  
		Last Modified: Tue, 17 Oct 2023 19:06:23 GMT  
		Size: 9.6 KB (9563 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:742c4b4811bb7526353fa77f1d53cf34b0757cd72cda2a75f760d95f766e18c1`  
		Last Modified: Tue, 17 Oct 2023 19:06:24 GMT  
		Size: 128.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:55dc2f534511ac73d76f7813372ff4cf5508ba7cfa6844be05c38e738dbc74e1`  
		Last Modified: Tue, 17 Oct 2023 19:06:24 GMT  
		Size: 170.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1b37c8c3dce3ac5f32923ad96220b5bdfe03b38651452649d8c175252436e397`  
		Last Modified: Tue, 17 Oct 2023 19:06:24 GMT  
		Size: 4.8 KB (4785 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `postgres:alpine3.18` - unknown; unknown

```console
$ docker pull postgres@sha256:f0a8f524f13ba22ec5099e73e7c4132dfab707bb613fd068e357bfaa5cc74024
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.6 KB (36571 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e7407733ba225a866581a98547567926483a1a344c8624981fd700dffd96c4f6`

```dockerfile
```

-	Layers:
	-	`sha256:1574c1ea0917100abcbffd57a8505feb161bb1c635f4b058aa2b245d52ff9cb8`  
		Last Modified: Tue, 17 Oct 2023 19:06:23 GMT  
		Size: 36.6 KB (36571 bytes)  
		MIME: application/vnd.in-toto+json

### `postgres:alpine3.18` - linux; ppc64le

```console
$ docker pull postgres@sha256:24116d2591bbd014d69b6a7c3e816a4ebb50b7e04fcd8eeb973dcb1a5b37c76e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.0 MB (99974574 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:87968e42822daa0abc99d7976193809f08f6ffa2e2ddefdd44ad87a913bfb683`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 30 Nov 2023 23:19:04 GMT
ADD file:3450a1687b552498a987f87cb844b7f597c7181d7c3d31943d7b3036d5300d5e in / 
# Thu, 30 Nov 2023 23:19:05 GMT
CMD ["/bin/sh"]
# Mon, 11 Dec 2023 19:03:58 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql # buildkit
# Mon, 11 Dec 2023 19:03:58 GMT
ENV LANG=en_US.utf8
# Mon, 11 Dec 2023 19:03:58 GMT
RUN mkdir /docker-entrypoint-initdb.d # buildkit
# Mon, 11 Dec 2023 19:03:58 GMT
ENV PG_MAJOR=16
# Mon, 11 Dec 2023 19:03:58 GMT
ENV PG_VERSION=16.1
# Mon, 11 Dec 2023 19:03:58 GMT
ENV PG_SHA256=ce3c4d85d19b0121fe0d3f8ef1fa601f71989e86f8a66f7dc3ad546dd5564fec
# Mon, 11 Dec 2023 19:03:58 GMT
ENV DOCKER_PG_LLVM_DEPS=llvm15-dev 		clang15
# Mon, 11 Dec 2023 19:03:58 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		$DOCKER_PG_LLVM_DEPS 		bison 		coreutils 		dpkg-dev dpkg 		flex 		g++ 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openldap-dev 		openssl-dev 		perl-dev 		perl-ipc-run 		perl-utils 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		icu-dev 		lz4-dev 		zstd-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 		export LLVM_CONFIG="/usr/lib/llvm15/bin/llvm-config"; 	export CLANG=clang-15; 		./configure 		--enable-option-checking=fatal 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 		--with-lz4 		--with-zstd 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 		zstd 		icu-data-full 		$([ "$(apk --print-arch)" != 'ppc64le' ] && echo 'nss_wrapper') 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version # buildkit
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
	-	`sha256:2e846b8744a06b2422b11a41906a0563302e284f541fb93f0988a17255a440db`  
		Last Modified: Wed, 13 Dec 2023 03:23:48 GMT  
		Size: 96.6 MB (96610222 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:58ec174e7b2853cf69c85277b4eff908542bffaefb7d0b02320041067d9a4819`  
		Last Modified: Wed, 13 Dec 2023 03:23:45 GMT  
		Size: 9.6 KB (9564 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:476c734c8fdb789185307ef456f5b170bbbf717380f4616698978f06bcd1dc30`  
		Last Modified: Wed, 13 Dec 2023 03:23:46 GMT  
		Size: 129.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9f720f80557615531c209d726dbfb4b77c3495e1cc4cd1cb0867da6162fde7f8`  
		Last Modified: Wed, 13 Dec 2023 03:23:46 GMT  
		Size: 170.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0e91713b79d81446b9f59c114098ee9ac5b60a3fad2fbe9a48c9fbf169f28134`  
		Last Modified: Wed, 13 Dec 2023 03:23:47 GMT  
		Size: 4.8 KB (4787 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `postgres:alpine3.18` - unknown; unknown

```console
$ docker pull postgres@sha256:ad9c037652710e32c65f3abefae8dc10c6f6df0afcb00dae469780cf0affdf12
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **838.2 KB (838225 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e5bc43028e08aaed3289a28d01912ba2fff90234adc91479b4a98a02d65e11a`

```dockerfile
```

-	Layers:
	-	`sha256:46dc67eeb86eec4e7525c5ee81b3f25cc47216c736a8ba4f0a0d7b3f1c8cd8a6`  
		Last Modified: Wed, 13 Dec 2023 03:23:45 GMT  
		Size: 803.5 KB (803471 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:d9acc81e6e96b99b810c63bdbfd7b6af03dbd40a13e20e9b0a23ea75807ed10d`  
		Last Modified: Wed, 13 Dec 2023 03:23:45 GMT  
		Size: 34.8 KB (34754 bytes)  
		MIME: application/vnd.in-toto+json

### `postgres:alpine3.18` - linux; s390x

```console
$ docker pull postgres@sha256:2f46c1de9b1797c93301abe0bebf6809369a2d41e7412e8951581c69e3f98cc2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.9 MB (95916969 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:db5437eb2274087c5decc5a4b91e33248d34975a1fc29de3e3e352f7c76391c4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 30 Nov 2023 22:42:08 GMT
ADD file:50d6643abf7df167a927decd69d193b980557ff73cca48dce86d57e2ff25ad45 in / 
# Thu, 30 Nov 2023 22:42:09 GMT
CMD ["/bin/sh"]
# Mon, 11 Dec 2023 19:03:58 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql # buildkit
# Mon, 11 Dec 2023 19:03:58 GMT
ENV LANG=en_US.utf8
# Mon, 11 Dec 2023 19:03:58 GMT
RUN mkdir /docker-entrypoint-initdb.d # buildkit
# Mon, 11 Dec 2023 19:03:58 GMT
ENV PG_MAJOR=16
# Mon, 11 Dec 2023 19:03:58 GMT
ENV PG_VERSION=16.1
# Mon, 11 Dec 2023 19:03:58 GMT
ENV PG_SHA256=ce3c4d85d19b0121fe0d3f8ef1fa601f71989e86f8a66f7dc3ad546dd5564fec
# Mon, 11 Dec 2023 19:03:58 GMT
ENV DOCKER_PG_LLVM_DEPS=llvm15-dev 		clang15
# Mon, 11 Dec 2023 19:03:58 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		$DOCKER_PG_LLVM_DEPS 		bison 		coreutils 		dpkg-dev dpkg 		flex 		g++ 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openldap-dev 		openssl-dev 		perl-dev 		perl-ipc-run 		perl-utils 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		icu-dev 		lz4-dev 		zstd-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 		export LLVM_CONFIG="/usr/lib/llvm15/bin/llvm-config"; 	export CLANG=clang-15; 		./configure 		--enable-option-checking=fatal 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 		--with-lz4 		--with-zstd 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 		zstd 		icu-data-full 		$([ "$(apk --print-arch)" != 'ppc64le' ] && echo 'nss_wrapper') 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version # buildkit
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
	-	`sha256:0cead63ae84b93f86e0859449a310c8f05cfefe2a6987e5ac3051c209e72f8de`  
		Last Modified: Wed, 13 Dec 2023 01:10:53 GMT  
		Size: 92.7 MB (92683481 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ab17958c1031062ecdb9bb47ec374fdbc9911127a3afc78fc40ef5cdc66a9c39`  
		Last Modified: Wed, 13 Dec 2023 01:10:52 GMT  
		Size: 9.6 KB (9570 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4cbe45538fed15568c76cdb961d09212141515ff406bae311e01143f550cb6b8`  
		Last Modified: Wed, 13 Dec 2023 01:10:52 GMT  
		Size: 129.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:14c63236f9cf20be039c9ff2cec010ed07d9e1950e80e3da9193b4381e64e3d2`  
		Last Modified: Wed, 13 Dec 2023 01:10:52 GMT  
		Size: 168.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c32cd075c50afa28a5037f36cf900234e0dec418f67ddedd5aeeb280be4116a2`  
		Last Modified: Wed, 13 Dec 2023 01:10:53 GMT  
		Size: 4.8 KB (4789 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `postgres:alpine3.18` - unknown; unknown

```console
$ docker pull postgres@sha256:50992e6216ec6cc3e460a3aef7c895455fe9140a6d69882da0a11c69d78d81c6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **839.6 KB (839570 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d05ce84286d461b052bdb5f86d326ccbea21341c4f0710417b244c3217faf7ef`

```dockerfile
```

-	Layers:
	-	`sha256:4fb50bd06f160668b647b45b4b9892f3404c9b296159673a01b9c570c95c47f1`  
		Last Modified: Wed, 13 Dec 2023 01:10:51 GMT  
		Size: 804.9 KB (804858 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:3220e74ff58ae4f5690acf5bc86fcf0bbd38fbb7c29b07aa22feb768aba902c2`  
		Last Modified: Wed, 13 Dec 2023 01:10:51 GMT  
		Size: 34.7 KB (34712 bytes)  
		MIME: application/vnd.in-toto+json
