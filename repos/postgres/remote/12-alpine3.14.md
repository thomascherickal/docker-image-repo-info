## `postgres:12-alpine3.14`

```console
$ docker pull postgres@sha256:de0effb7ca62f396168f4d3c35d9042e2a9d4da23e424daa90fee19859b57012
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 7
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `postgres:12-alpine3.14` - linux; amd64

```console
$ docker pull postgres@sha256:6a4bc35ca95a2325a16b50e4ca7a7d13e2c3947d9e947be194da6a690ee94185
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.2 MB (75151773 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d029edc386822ae1bb9c649cd81770e43ff615472c83a262b08cacfdd9c20d3c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Fri, 27 Aug 2021 22:48:02 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Fri, 27 Aug 2021 22:48:02 GMT
ENV LANG=en_US.utf8
# Fri, 27 Aug 2021 22:48:03 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 27 Aug 2021 23:02:48 GMT
ENV PG_MAJOR=12
# Fri, 27 Aug 2021 23:02:48 GMT
ENV PG_VERSION=12.8
# Fri, 27 Aug 2021 23:02:48 GMT
ENV PG_SHA256=e26401e090c34ccb15ffb33a111f340833833535a7b7c5cd11cd88ab57d9c62a
# Fri, 27 Aug 2021 23:09:35 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm11-dev clang g++ 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Fri, 27 Aug 2021 23:09:36 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample
# Fri, 27 Aug 2021 23:09:37 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 27 Aug 2021 23:09:37 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 27 Aug 2021 23:09:38 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 27 Aug 2021 23:09:38 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 27 Aug 2021 23:09:38 GMT
COPY file:ad28506adc606e446eefc263bc99d4cb809e608d4f550956143bf13c82c91f85 in /usr/local/bin/ 
# Fri, 27 Aug 2021 23:09:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 Aug 2021 23:09:39 GMT
STOPSIGNAL SIGINT
# Fri, 27 Aug 2021 23:09:39 GMT
EXPOSE 5432
# Fri, 27 Aug 2021 23:09:39 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:a0d0a0d46f8b52473982a3c466318f479767577551a53ffc9074c9fa7035982e`  
		Last Modified: Fri, 27 Aug 2021 17:20:13 GMT  
		Size: 2.8 MB (2814446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5034a66b99e67db609bf6b4f82bea915e39a42e6f03d11889f7406b4de9e99da`  
		Last Modified: Fri, 27 Aug 2021 23:28:20 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82e9eb77798bd506a06a9adab733c822c718be829c54d514b5789b07c0f1c164`  
		Last Modified: Fri, 27 Aug 2021 23:28:20 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57a44591d957552dc7e14c76e1dc436b97b5c1ef0228786742075e6a2abce481`  
		Last Modified: Fri, 27 Aug 2021 23:29:24 GMT  
		Size: 72.3 MB (72322443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1c9e53bf891ae35017b88b1b43f9063f28841a4f78d2fdd2b17eb3cd047ceb9`  
		Last Modified: Fri, 27 Aug 2021 23:29:15 GMT  
		Size: 8.7 KB (8693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3783fb52ad9d7f237df9a8c98265ee6c6738baf152c5b5f67e1dfdec32645b86`  
		Last Modified: Fri, 27 Aug 2021 23:29:14 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a73087232a9ed788892771d4f22df6d93388b023b14de63806771011081a569`  
		Last Modified: Fri, 27 Aug 2021 23:29:14 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e9916d2468d0724aa5631ab6b09bd30d12e8678aea6a81456e8e11ec0b68263`  
		Last Modified: Fri, 27 Aug 2021 23:29:14 GMT  
		Size: 4.4 KB (4405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:12-alpine3.14` - linux; arm variant v6

```console
$ docker pull postgres@sha256:f72fe297c8688a5de0bf8572ee2ae9cc37c900606a6b0c067eaaa69a7ffdacaf
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.8 MB (73756004 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ac9b181e6a838840bfb766c97930ff635fdcac57516347fa318b6dc5c6f6c48`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Fri, 27 Aug 2021 17:49:29 GMT
ADD file:1c1c4520d49cb6e8f795f3b953d1ed3c3c77868b98b53a455169c254fcec5acd in / 
# Fri, 27 Aug 2021 17:49:30 GMT
CMD ["/bin/sh"]
# Fri, 27 Aug 2021 22:04:28 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Fri, 27 Aug 2021 22:04:29 GMT
ENV LANG=en_US.utf8
# Fri, 27 Aug 2021 22:04:33 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 27 Aug 2021 22:16:21 GMT
ENV PG_MAJOR=12
# Fri, 27 Aug 2021 22:16:21 GMT
ENV PG_VERSION=12.8
# Fri, 27 Aug 2021 22:16:22 GMT
ENV PG_SHA256=e26401e090c34ccb15ffb33a111f340833833535a7b7c5cd11cd88ab57d9c62a
# Fri, 27 Aug 2021 22:20:58 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm11-dev clang g++ 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Fri, 27 Aug 2021 22:21:01 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample
# Fri, 27 Aug 2021 22:21:02 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 27 Aug 2021 22:21:03 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 27 Aug 2021 22:21:04 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 27 Aug 2021 22:21:05 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 27 Aug 2021 22:21:05 GMT
COPY file:ad28506adc606e446eefc263bc99d4cb809e608d4f550956143bf13c82c91f85 in /usr/local/bin/ 
# Fri, 27 Aug 2021 22:21:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 Aug 2021 22:21:06 GMT
STOPSIGNAL SIGINT
# Fri, 27 Aug 2021 22:21:07 GMT
EXPOSE 5432
# Fri, 27 Aug 2021 22:21:07 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:2e78c0f86ba9a1fed30df20cb48c9cc73e9626399f12749d36b892ff99c0ecf5`  
		Last Modified: Fri, 27 Aug 2021 17:50:55 GMT  
		Size: 2.6 MB (2627447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a768a51394fb89d634086ed31a7649653823611d054a16603974b9148da6f5b`  
		Last Modified: Fri, 27 Aug 2021 22:36:22 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e44aa70cad34222b58a50860314f35128c905e3265d6d7bf08054f3c70daeb3d`  
		Last Modified: Fri, 27 Aug 2021 22:36:22 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcb553ffd85a20766cd8f9c0c80cc1ba84a3186f9f3a5cbc3f8aca7fbfe371ee`  
		Last Modified: Fri, 27 Aug 2021 22:39:06 GMT  
		Size: 71.1 MB (71113671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f770f3f84ccc35d8047560c929059f4f0bc8d7ec89be2ffbfea78fd1b9bd2c14`  
		Last Modified: Fri, 27 Aug 2021 22:38:25 GMT  
		Size: 8.7 KB (8692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2529a95173021a92d845e6ba80202a17aa0590d1616b7f9d9415369c754f6ca5`  
		Last Modified: Fri, 27 Aug 2021 22:38:26 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db0cfb382bb6e74b5d93d8c1759bf7b3d422daab6098911062aa4009745747fd`  
		Last Modified: Fri, 27 Aug 2021 22:38:25 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8776678ffa4a5c26471c4cb52fa47da6512200042a4145fe7683afd03cd062f6`  
		Last Modified: Fri, 27 Aug 2021 22:38:26 GMT  
		Size: 4.4 KB (4403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:12-alpine3.14` - linux; arm variant v7

```console
$ docker pull postgres@sha256:0d4989f3eb4017802119aa2086f6c9c82222fd76b7c375e50d1eeedf672f3392
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.5 MB (69493269 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e5591ed9fa504b6ad762437127a94d9e2e03a4eb41eec17eba115ebc225904f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Fri, 27 Aug 2021 17:57:31 GMT
ADD file:a7da7992ccea54d3295231027614f138aa45c4d4a25ea6ec9bf7b316b9f67d95 in / 
# Fri, 27 Aug 2021 17:57:32 GMT
CMD ["/bin/sh"]
# Sat, 28 Aug 2021 00:08:07 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Sat, 28 Aug 2021 00:08:07 GMT
ENV LANG=en_US.utf8
# Sat, 28 Aug 2021 00:08:09 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 28 Aug 2021 00:18:31 GMT
ENV PG_MAJOR=12
# Sat, 28 Aug 2021 00:18:31 GMT
ENV PG_VERSION=12.8
# Sat, 28 Aug 2021 00:18:32 GMT
ENV PG_SHA256=e26401e090c34ccb15ffb33a111f340833833535a7b7c5cd11cd88ab57d9c62a
# Sat, 28 Aug 2021 00:23:05 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm11-dev clang g++ 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Sat, 28 Aug 2021 00:23:08 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample
# Sat, 28 Aug 2021 00:23:09 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Sat, 28 Aug 2021 00:23:10 GMT
ENV PGDATA=/var/lib/postgresql/data
# Sat, 28 Aug 2021 00:23:12 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Sat, 28 Aug 2021 00:23:12 GMT
VOLUME [/var/lib/postgresql/data]
# Sat, 28 Aug 2021 00:23:13 GMT
COPY file:ad28506adc606e446eefc263bc99d4cb809e608d4f550956143bf13c82c91f85 in /usr/local/bin/ 
# Sat, 28 Aug 2021 00:23:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 28 Aug 2021 00:23:14 GMT
STOPSIGNAL SIGINT
# Sat, 28 Aug 2021 00:23:14 GMT
EXPOSE 5432
# Sat, 28 Aug 2021 00:23:15 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:a14774a5a62e0f454febaec7cb603e18a6a8e25ef9da4a4da85b155bdd5e5a7a`  
		Last Modified: Fri, 27 Aug 2021 17:59:00 GMT  
		Size: 2.4 MB (2430419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:644c3f2a8fe3f377a2e021c2c2788a12425c35f5560621956858f68cba63d274`  
		Last Modified: Sat, 28 Aug 2021 00:41:21 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2240d9ddca5f179b1dcff799a11d280aa6b468e6758274079baf41bcdbb97c5`  
		Last Modified: Sat, 28 Aug 2021 00:41:21 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6f791e91e3a0aa9b190f96b4d123362954ece5ee5cdc88c3854a24c6e548554`  
		Last Modified: Sat, 28 Aug 2021 00:44:06 GMT  
		Size: 67.0 MB (67047964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbcf0841ba7a421ec9b043a21b48231df7f752145696e19e40138ff0e3322abd`  
		Last Modified: Sat, 28 Aug 2021 00:43:30 GMT  
		Size: 8.7 KB (8695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16c36048962233676ce98a8f3a5a1b6586967dfaed846802830a778f27bc6a05`  
		Last Modified: Sat, 28 Aug 2021 00:43:30 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19e50b2af1191b6a3d8a2851caf0076d50f384840d3df6d052f8dcdfa1678768`  
		Last Modified: Sat, 28 Aug 2021 00:43:30 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c1297865a6e8c5cb6bf6ee9a561362adb60181868c45f081533f418c8fceb6e`  
		Last Modified: Sat, 28 Aug 2021 00:43:30 GMT  
		Size: 4.4 KB (4403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:12-alpine3.14` - linux; arm64 variant v8

```console
$ docker pull postgres@sha256:70e9b4d714a67a51e918ed2950cc2c256c77e304f866540f047267d4a1d8d3ae
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.1 MB (74077545 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d755a1e54c73ca9f7e45a24e8cddf8c4a681f4ff2e3d32ecf0a01713e5144a2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Fri, 27 Aug 2021 17:39:33 GMT
ADD file:dc8af9c7bfe9f9541e1db38dea01c4201609f3075b31e108f2073ffed8c5e4b9 in / 
# Fri, 27 Aug 2021 17:39:33 GMT
CMD ["/bin/sh"]
# Sat, 28 Aug 2021 00:44:21 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Sat, 28 Aug 2021 00:44:21 GMT
ENV LANG=en_US.utf8
# Sat, 28 Aug 2021 00:44:22 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 28 Aug 2021 00:53:43 GMT
ENV PG_MAJOR=12
# Sat, 28 Aug 2021 00:53:43 GMT
ENV PG_VERSION=12.8
# Sat, 28 Aug 2021 00:53:43 GMT
ENV PG_SHA256=e26401e090c34ccb15ffb33a111f340833833535a7b7c5cd11cd88ab57d9c62a
# Sat, 28 Aug 2021 00:57:49 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm11-dev clang g++ 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Sat, 28 Aug 2021 00:57:50 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample
# Sat, 28 Aug 2021 00:57:50 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Sat, 28 Aug 2021 00:57:50 GMT
ENV PGDATA=/var/lib/postgresql/data
# Sat, 28 Aug 2021 00:57:51 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Sat, 28 Aug 2021 00:57:51 GMT
VOLUME [/var/lib/postgresql/data]
# Sat, 28 Aug 2021 00:57:51 GMT
COPY file:ad28506adc606e446eefc263bc99d4cb809e608d4f550956143bf13c82c91f85 in /usr/local/bin/ 
# Sat, 28 Aug 2021 00:57:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 28 Aug 2021 00:57:52 GMT
STOPSIGNAL SIGINT
# Sat, 28 Aug 2021 00:57:52 GMT
EXPOSE 5432
# Sat, 28 Aug 2021 00:57:52 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:552d1f2373af9bfe12033568ebbfb0ccbb0de11279f9a415a29207e264d7f4d9`  
		Last Modified: Fri, 27 Aug 2021 17:40:18 GMT  
		Size: 2.7 MB (2711827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7e9520c37213002780ab811214a7b664b01adbff78712b200a8ad6dac8f6ecb`  
		Last Modified: Sat, 28 Aug 2021 01:11:06 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e16841d04e832ad38f955594481fd7205810db3379719d35e62c344f12dc0ff`  
		Last Modified: Sat, 28 Aug 2021 01:11:06 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0440dcfa9b91ca24ded2fbd932aca87b3fb0c93af755f5b4e2cb4e73d2c52c4`  
		Last Modified: Sat, 28 Aug 2021 01:12:19 GMT  
		Size: 71.4 MB (71350836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ed9d984e10f14d207f6fb2b53fd332170841b49ac664e9764b4af55282ce378`  
		Last Modified: Sat, 28 Aug 2021 01:12:10 GMT  
		Size: 8.7 KB (8687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d90dc8768e81ac6891f5225e1a1269ec9c21a1a65060675611d6ad0eb91f969`  
		Last Modified: Sat, 28 Aug 2021 01:12:09 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c6fa6b757f14a242ce3c2cc251625722f5a2ba20d84cea6acc189beea8caea8`  
		Last Modified: Sat, 28 Aug 2021 01:12:09 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eaaddbee7f41181a2e744b0cc326ee421538e05a59bee63b8c707028e000e1da`  
		Last Modified: Sat, 28 Aug 2021 01:12:09 GMT  
		Size: 4.4 KB (4404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:12-alpine3.14` - linux; 386

```console
$ docker pull postgres@sha256:648286e2d7466fc1fbf489408d6ac8226f8ec02eb803177cfa700fc9cd1bbe39
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **79.9 MB (79865257 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:26f711e72ed9064be62adb463101d36b60a002f21c3fc6d2af9f9559e090f1b1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Fri, 27 Aug 2021 17:38:29 GMT
ADD file:42a7bc5a08b546b47049dd0f89ae4e7a8c86342f87000f39ade3ff52916a6c2e in / 
# Fri, 27 Aug 2021 17:38:30 GMT
CMD ["/bin/sh"]
# Fri, 27 Aug 2021 21:55:05 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Fri, 27 Aug 2021 21:55:05 GMT
ENV LANG=en_US.utf8
# Fri, 27 Aug 2021 21:55:06 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 27 Aug 2021 22:13:23 GMT
ENV PG_MAJOR=12
# Fri, 27 Aug 2021 22:13:23 GMT
ENV PG_VERSION=12.8
# Fri, 27 Aug 2021 22:13:23 GMT
ENV PG_SHA256=e26401e090c34ccb15ffb33a111f340833833535a7b7c5cd11cd88ab57d9c62a
# Fri, 27 Aug 2021 22:20:24 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm11-dev clang g++ 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Fri, 27 Aug 2021 22:20:27 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample
# Fri, 27 Aug 2021 22:20:29 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 27 Aug 2021 22:20:29 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 27 Aug 2021 22:20:30 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 27 Aug 2021 22:20:31 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 27 Aug 2021 22:20:31 GMT
COPY file:ad28506adc606e446eefc263bc99d4cb809e608d4f550956143bf13c82c91f85 in /usr/local/bin/ 
# Fri, 27 Aug 2021 22:20:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 Aug 2021 22:20:32 GMT
STOPSIGNAL SIGINT
# Fri, 27 Aug 2021 22:20:32 GMT
EXPOSE 5432
# Fri, 27 Aug 2021 22:20:32 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:b11ae9fc5d8a106cfed3a6f6c75e5b5b5797c566fac4411622b4055df6541286`  
		Last Modified: Fri, 27 Aug 2021 17:39:18 GMT  
		Size: 2.8 MB (2822857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b976c7cea63cd0c42b035f2167b42952bfe4b4c5c26d5c1828e46ccf08b16dd9`  
		Last Modified: Fri, 27 Aug 2021 22:41:30 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b58324ac0c0139295582dea67f31b819f305cd721ba1189ab4e66fbb574de652`  
		Last Modified: Fri, 27 Aug 2021 22:41:30 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f5267db7411f3f4f2c3c8f9fdc27167aff56c6d4c5a1c01281cfdcaa6f07951`  
		Last Modified: Fri, 27 Aug 2021 22:42:56 GMT  
		Size: 77.0 MB (77027513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a02db2197f2993236d6f27ed320beaef2d943c815eeb90f654324adcbc40628e`  
		Last Modified: Fri, 27 Aug 2021 22:42:43 GMT  
		Size: 8.7 KB (8691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2beb9701b7472ce4139a8d426f47e82a4f1b6f8f8dca145506419d1065ac7524`  
		Last Modified: Fri, 27 Aug 2021 22:42:42 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f4d8770d3d35a7fe4eb02b7a6a81c0b265aa623db0b5dfc491cdafe67a5b2df`  
		Last Modified: Fri, 27 Aug 2021 22:42:43 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ae5602b2cd23402d318411057d53dd800864a8dae45a677d3363bddf97e5ad7`  
		Last Modified: Fri, 27 Aug 2021 22:42:42 GMT  
		Size: 4.4 KB (4407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:12-alpine3.14` - linux; ppc64le

```console
$ docker pull postgres@sha256:e1582246465405020683d9873b43224c5bb8dde457966130385bdbae14527ae2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **80.0 MB (80040825 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a86f310640245a738df8a91fac145939f7340a69d4bef04a55bdaa86537002aa`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Fri, 27 Aug 2021 19:39:54 GMT
ADD file:d213c56ffc24a5051e8060fd0fec1a0520367c10d88ab16321c36336b6c66098 in / 
# Fri, 27 Aug 2021 19:39:59 GMT
CMD ["/bin/sh"]
# Fri, 27 Aug 2021 21:43:37 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Fri, 27 Aug 2021 21:43:39 GMT
ENV LANG=en_US.utf8
# Fri, 27 Aug 2021 21:43:48 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 27 Aug 2021 21:56:09 GMT
ENV PG_MAJOR=12
# Fri, 27 Aug 2021 21:56:13 GMT
ENV PG_VERSION=12.8
# Fri, 27 Aug 2021 21:56:17 GMT
ENV PG_SHA256=e26401e090c34ccb15ffb33a111f340833833535a7b7c5cd11cd88ab57d9c62a
# Fri, 27 Aug 2021 22:00:25 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm11-dev clang g++ 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Fri, 27 Aug 2021 22:00:34 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample
# Fri, 27 Aug 2021 22:00:41 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 27 Aug 2021 22:00:45 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 27 Aug 2021 22:00:52 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 27 Aug 2021 22:00:55 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 27 Aug 2021 22:00:57 GMT
COPY file:ad28506adc606e446eefc263bc99d4cb809e608d4f550956143bf13c82c91f85 in /usr/local/bin/ 
# Fri, 27 Aug 2021 22:00:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 Aug 2021 22:01:04 GMT
STOPSIGNAL SIGINT
# Fri, 27 Aug 2021 22:01:07 GMT
EXPOSE 5432
# Fri, 27 Aug 2021 22:01:10 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:63da8ca98f7b4b94381aed56862a60aecf355d9428b9aeb7c61d5bd017100c18`  
		Last Modified: Fri, 27 Aug 2021 19:41:06 GMT  
		Size: 2.8 MB (2812284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51b84363c8c0f2373e8b665451df1c6a11a9415fd4f1c773e8ce7aaafa836248`  
		Last Modified: Fri, 27 Aug 2021 22:17:39 GMT  
		Size: 1.3 KB (1287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7f2722689cf013f5f6333bf25f2c1fa26b298e09468166e2cbade7a81c0817c`  
		Last Modified: Fri, 27 Aug 2021 22:17:38 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1caa70f15a85167961e97fd471a85973ca3aaf2ded79345c6e10562475815075`  
		Last Modified: Fri, 27 Aug 2021 22:19:18 GMT  
		Size: 77.2 MB (77213650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a5ec1790a5b06ff3e69a3e71908049fe2f906a0cf1934e0d34f2e450935d134`  
		Last Modified: Fri, 27 Aug 2021 22:19:06 GMT  
		Size: 8.7 KB (8693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e48a4fc9ca10a63df87a505440eb26b8e8536e1101e78d0735c5b12eb5b88ce`  
		Last Modified: Fri, 27 Aug 2021 22:19:05 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16e1cbbc5eb85c5cecb83214a01e6f742163f20809a8219b821628ac5f006c01`  
		Last Modified: Fri, 27 Aug 2021 22:19:05 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da509b644257bde014a5d85d0b6da45f022f6b34310f759fa1f2577e4057effd`  
		Last Modified: Fri, 27 Aug 2021 22:19:05 GMT  
		Size: 4.4 KB (4407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:12-alpine3.14` - linux; s390x

```console
$ docker pull postgres@sha256:94f3e1f89aa1c4b401f9b80af60de4b0dfabb10d1329bfc4736a6f135a96b79b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.6 MB (76597826 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a6bdac1756246b9d1c024f87190dbe352f39f9996f4cbfea73aec9df4b43534b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Fri, 27 Aug 2021 17:41:29 GMT
ADD file:9b40ee281e8797067fb2ae207c406084cb81593090338a8b7cb09ade52168daa in / 
# Fri, 27 Aug 2021 17:41:30 GMT
CMD ["/bin/sh"]
# Sat, 28 Aug 2021 00:49:31 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Sat, 28 Aug 2021 00:49:32 GMT
ENV LANG=en_US.utf8
# Sat, 28 Aug 2021 00:49:32 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 28 Aug 2021 00:57:11 GMT
ENV PG_MAJOR=12
# Sat, 28 Aug 2021 00:57:11 GMT
ENV PG_VERSION=12.8
# Sat, 28 Aug 2021 00:57:11 GMT
ENV PG_SHA256=e26401e090c34ccb15ffb33a111f340833833535a7b7c5cd11cd88ab57d9c62a
# Sat, 28 Aug 2021 01:01:19 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm11-dev clang g++ 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Sat, 28 Aug 2021 01:01:30 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample
# Sat, 28 Aug 2021 01:01:32 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Sat, 28 Aug 2021 01:01:32 GMT
ENV PGDATA=/var/lib/postgresql/data
# Sat, 28 Aug 2021 01:01:34 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Sat, 28 Aug 2021 01:01:35 GMT
VOLUME [/var/lib/postgresql/data]
# Sat, 28 Aug 2021 01:01:35 GMT
COPY file:ad28506adc606e446eefc263bc99d4cb809e608d4f550956143bf13c82c91f85 in /usr/local/bin/ 
# Sat, 28 Aug 2021 01:01:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 28 Aug 2021 01:01:36 GMT
STOPSIGNAL SIGINT
# Sat, 28 Aug 2021 01:01:37 GMT
EXPOSE 5432
# Sat, 28 Aug 2021 01:01:38 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:da14cb6b6dc946dbb2d84386bcaca84e2d46f650767cd11bdb3331ec9d623988`  
		Last Modified: Fri, 27 Aug 2021 17:42:25 GMT  
		Size: 2.6 MB (2603464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31510cc6ab297041382a23f3ee5b4a7cf8e1a650f86836260bfcb82cbd35f7eb`  
		Last Modified: Sat, 28 Aug 2021 01:19:34 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a5c23a40fbc63d8bd8713694dbda49900c3198d4156a8b8ca18ccc15b793399`  
		Last Modified: Sat, 28 Aug 2021 01:19:33 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cddd35b50b1ce887711a99333fe656f26040b7329212321c34b8525f7b3186ef`  
		Last Modified: Sat, 28 Aug 2021 01:20:39 GMT  
		Size: 74.0 MB (73979479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86a4bc3e1583c99a303afcf0487f212d0e46895f5b908f9110a01b7b5dc26bf9`  
		Last Modified: Sat, 28 Aug 2021 01:20:29 GMT  
		Size: 8.7 KB (8689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:483370683f98a521c23511598e1d4ae81b73d8b8d038ae4b1150b248960817ed`  
		Last Modified: Sat, 28 Aug 2021 01:20:29 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7baef8b6957aede36c92347e76662535acf8704a0507a92b73dcd52bcafad30d`  
		Last Modified: Sat, 28 Aug 2021 01:20:29 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60ec00bf92fd9c32535f6d0850e7e097e545623a859caf7c3eab9d69d37fdbff`  
		Last Modified: Sat, 28 Aug 2021 01:20:29 GMT  
		Size: 4.4 KB (4406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
