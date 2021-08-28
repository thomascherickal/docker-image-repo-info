## `postgres:alpine`

```console
$ docker pull postgres@sha256:a70babcd0e8f86272c35d6efcf8070c597c1f31b3d19727eece213a09929dd55
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

### `postgres:alpine` - linux; amd64

```console
$ docker pull postgres@sha256:3ff2a17bb5bc1f9723032da16edb21e55d2af1e2e0f1beda68818a58ead33016
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.8 MB (75820510 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b8c450ae09036f6ee1af4c641f3df3199a7f8d80771056e42d8cf18ea4291018`
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
# Fri, 27 Aug 2021 22:55:02 GMT
ENV PG_MAJOR=13
# Fri, 27 Aug 2021 22:55:02 GMT
ENV PG_VERSION=13.4
# Fri, 27 Aug 2021 22:55:02 GMT
ENV PG_SHA256=ea93e10390245f1ce461a54eb5f99a48d8cabd3a08ce4d652ec2169a357bc0cd
# Fri, 27 Aug 2021 23:02:26 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm11-dev clang g++ 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Fri, 27 Aug 2021 23:02:27 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample
# Fri, 27 Aug 2021 23:02:28 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 27 Aug 2021 23:02:28 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 27 Aug 2021 23:02:29 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 27 Aug 2021 23:02:29 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 27 Aug 2021 23:02:29 GMT
COPY file:ad28506adc606e446eefc263bc99d4cb809e608d4f550956143bf13c82c91f85 in /usr/local/bin/ 
# Fri, 27 Aug 2021 23:02:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 Aug 2021 23:02:29 GMT
STOPSIGNAL SIGINT
# Fri, 27 Aug 2021 23:02:30 GMT
EXPOSE 5432
# Fri, 27 Aug 2021 23:02:30 GMT
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
	-	`sha256:314b9347faf5633a113c4ee344dd7f6df334d51198900d6a90e7d821e079c255`  
		Last Modified: Fri, 27 Aug 2021 23:28:51 GMT  
		Size: 73.0 MB (72990848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2625be9fae825d78a790ea9011a2158a72bc90330fe5910d9337aec3cafbf34f`  
		Last Modified: Fri, 27 Aug 2021 23:28:41 GMT  
		Size: 9.0 KB (9025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ec8358e2a993be48001f5b136400de7f312c61743b58750565605a6704e82e4`  
		Last Modified: Fri, 27 Aug 2021 23:28:41 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e9ccfc29d86510f6297bc5869ce92182e27c70e34c8415c54675acfba85e7e2`  
		Last Modified: Fri, 27 Aug 2021 23:28:41 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a4d94e5dde0c66ff39657b12281a85fa3b7907f96fa6f2eaa86c5009529bb83`  
		Last Modified: Fri, 27 Aug 2021 23:28:41 GMT  
		Size: 4.4 KB (4403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:alpine` - linux; arm variant v6

```console
$ docker pull postgres@sha256:ddbe35e212ea606dccf383f91796b64e8e6ebb09adc84c15352b0c7e06c05d30
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.3 MB (74349702 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7d4a9e5e6439501bfe9ebc7b4d578ec8f7826c49db5e6b54d597fcb6a717ab8`
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
# Fri, 27 Aug 2021 22:11:01 GMT
ENV PG_MAJOR=13
# Fri, 27 Aug 2021 22:11:01 GMT
ENV PG_VERSION=13.4
# Fri, 27 Aug 2021 22:11:02 GMT
ENV PG_SHA256=ea93e10390245f1ce461a54eb5f99a48d8cabd3a08ce4d652ec2169a357bc0cd
# Fri, 27 Aug 2021 22:15:53 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm11-dev clang g++ 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Fri, 27 Aug 2021 22:15:55 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample
# Fri, 27 Aug 2021 22:15:57 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 27 Aug 2021 22:15:57 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 27 Aug 2021 22:15:58 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 27 Aug 2021 22:15:59 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 27 Aug 2021 22:15:59 GMT
COPY file:ad28506adc606e446eefc263bc99d4cb809e608d4f550956143bf13c82c91f85 in /usr/local/bin/ 
# Fri, 27 Aug 2021 22:16:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 Aug 2021 22:16:00 GMT
STOPSIGNAL SIGINT
# Fri, 27 Aug 2021 22:16:01 GMT
EXPOSE 5432
# Fri, 27 Aug 2021 22:16:01 GMT
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
	-	`sha256:c018f2d7562b26e9e7678d6f16b70ae9d3dc62d233e4b804a8938b88052b8c7d`  
		Last Modified: Fri, 27 Aug 2021 22:37:56 GMT  
		Size: 71.7 MB (71707032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1deef91998cf99ab4a814cb3b86167409ef111ff157c22f97c1d2b69c59488d7`  
		Last Modified: Fri, 27 Aug 2021 22:37:14 GMT  
		Size: 9.0 KB (9030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46bb2f8c2daac7de1b44c33625dd309b22534e50f4ba8fb5ceff0bf3820053ac`  
		Last Modified: Fri, 27 Aug 2021 22:37:14 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1173e8b71a75edb15ae41018c5ad714445716252a8e49c86478a7392d4069845`  
		Last Modified: Fri, 27 Aug 2021 22:37:14 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ab3cb46101216a976f75d67ac5eff5736466622fb8185decc8e79ee77f9bdb1`  
		Last Modified: Fri, 27 Aug 2021 22:37:14 GMT  
		Size: 4.4 KB (4405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:alpine` - linux; arm variant v7

```console
$ docker pull postgres@sha256:910ed0104f0e85d2dee3d28fe99e1d25320ac8d3aee5460e6892bd3740a9ad68
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.1 MB (70059898 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f59ffb34722f238d9adab7742cf0ca9ad2237990847fe5e087dfdcd3075754c6`
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
# Sat, 28 Aug 2021 00:13:26 GMT
ENV PG_MAJOR=13
# Sat, 28 Aug 2021 00:13:26 GMT
ENV PG_VERSION=13.4
# Sat, 28 Aug 2021 00:13:27 GMT
ENV PG_SHA256=ea93e10390245f1ce461a54eb5f99a48d8cabd3a08ce4d652ec2169a357bc0cd
# Sat, 28 Aug 2021 00:17:54 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm11-dev clang g++ 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Sat, 28 Aug 2021 00:17:57 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample
# Sat, 28 Aug 2021 00:17:59 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Sat, 28 Aug 2021 00:17:59 GMT
ENV PGDATA=/var/lib/postgresql/data
# Sat, 28 Aug 2021 00:18:01 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Sat, 28 Aug 2021 00:18:02 GMT
VOLUME [/var/lib/postgresql/data]
# Sat, 28 Aug 2021 00:18:02 GMT
COPY file:ad28506adc606e446eefc263bc99d4cb809e608d4f550956143bf13c82c91f85 in /usr/local/bin/ 
# Sat, 28 Aug 2021 00:18:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 28 Aug 2021 00:18:03 GMT
STOPSIGNAL SIGINT
# Sat, 28 Aug 2021 00:18:04 GMT
EXPOSE 5432
# Sat, 28 Aug 2021 00:18:04 GMT
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
	-	`sha256:0aca1e81a84b2a2768c6b1397718244d5d48fc7edb835da6f8fd683468ecc3b1`  
		Last Modified: Sat, 28 Aug 2021 00:42:54 GMT  
		Size: 67.6 MB (67614257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9132b07616878fbd7a39ed27813185b1140428d0f20985e2a5338c72cffafd65`  
		Last Modified: Sat, 28 Aug 2021 00:42:18 GMT  
		Size: 9.0 KB (9026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ceb0f4f8d99a4231f09db78fb50a6334eb56daa9cd6b1313b2f1df06441f331`  
		Last Modified: Sat, 28 Aug 2021 00:42:18 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ae7c4cc9e8a76a3000d2bed6195da87517f0899347bb154e56bfae38fb28f97`  
		Last Modified: Sat, 28 Aug 2021 00:42:18 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12608f5f0514c44f8fc56e7d6bab511dde79d00723cf0be505909cd7cadfd13a`  
		Last Modified: Sat, 28 Aug 2021 00:42:18 GMT  
		Size: 4.4 KB (4408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:alpine` - linux; arm64 variant v8

```console
$ docker pull postgres@sha256:3a7eaa354394f1dc11eb110f3135400832ad09d980921b4d24caeb9226e2eb23
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.7 MB (74700653 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eeffcec048204b4440fd951b2c48d1048d5b246f19ef05cbe213167241db67e7`
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
# Sat, 28 Aug 2021 00:49:10 GMT
ENV PG_MAJOR=13
# Sat, 28 Aug 2021 00:49:10 GMT
ENV PG_VERSION=13.4
# Sat, 28 Aug 2021 00:49:10 GMT
ENV PG_SHA256=ea93e10390245f1ce461a54eb5f99a48d8cabd3a08ce4d652ec2169a357bc0cd
# Sat, 28 Aug 2021 00:53:25 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm11-dev clang g++ 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Sat, 28 Aug 2021 00:53:26 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample
# Sat, 28 Aug 2021 00:53:27 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Sat, 28 Aug 2021 00:53:27 GMT
ENV PGDATA=/var/lib/postgresql/data
# Sat, 28 Aug 2021 00:53:28 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Sat, 28 Aug 2021 00:53:28 GMT
VOLUME [/var/lib/postgresql/data]
# Sat, 28 Aug 2021 00:53:28 GMT
COPY file:ad28506adc606e446eefc263bc99d4cb809e608d4f550956143bf13c82c91f85 in /usr/local/bin/ 
# Sat, 28 Aug 2021 00:53:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 28 Aug 2021 00:53:29 GMT
STOPSIGNAL SIGINT
# Sat, 28 Aug 2021 00:53:29 GMT
EXPOSE 5432
# Sat, 28 Aug 2021 00:53:29 GMT
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
	-	`sha256:1bb4d6f8fad8ebba71faba880b3d152251eda84af9cc4f9f19a76ae702854529`  
		Last Modified: Sat, 28 Aug 2021 01:11:40 GMT  
		Size: 72.0 MB (71973606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6f008f9b3af6cffa847e18efdadbe64323bfc76eb64d92de09312dd655a4999`  
		Last Modified: Sat, 28 Aug 2021 01:11:30 GMT  
		Size: 9.0 KB (9023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84c0172d9e883fb1170a5d2703ad040ff312698837d9b6efc4ffc781bcda5369`  
		Last Modified: Sat, 28 Aug 2021 01:11:30 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5f0ebb20912a45b37e806282a43fe11c2baac7f93a7ccf067fa22c8f14bed29`  
		Last Modified: Sat, 28 Aug 2021 01:11:30 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:732c8a488b4e87dbdd43989df1790daecd0d85292117d01a93598d87e2e0ab2d`  
		Last Modified: Sat, 28 Aug 2021 01:11:30 GMT  
		Size: 4.4 KB (4406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:alpine` - linux; 386

```console
$ docker pull postgres@sha256:99733c4c9c4b7c79a07271cbbd9f943bade86e6cefd1d92b2f159b3d63325299
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **80.6 MB (80571848 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a2374cbf4f9fb337b0866717e26a18dd025743d07632147a6c74a8d5d4197dd`
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
# Fri, 27 Aug 2021 22:04:55 GMT
ENV PG_MAJOR=13
# Fri, 27 Aug 2021 22:04:55 GMT
ENV PG_VERSION=13.4
# Fri, 27 Aug 2021 22:04:55 GMT
ENV PG_SHA256=ea93e10390245f1ce461a54eb5f99a48d8cabd3a08ce4d652ec2169a357bc0cd
# Fri, 27 Aug 2021 22:12:55 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm11-dev clang g++ 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Fri, 27 Aug 2021 22:12:57 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample
# Fri, 27 Aug 2021 22:12:59 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 27 Aug 2021 22:12:59 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 27 Aug 2021 22:13:01 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 27 Aug 2021 22:13:01 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 27 Aug 2021 22:13:01 GMT
COPY file:ad28506adc606e446eefc263bc99d4cb809e608d4f550956143bf13c82c91f85 in /usr/local/bin/ 
# Fri, 27 Aug 2021 22:13:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 Aug 2021 22:13:02 GMT
STOPSIGNAL SIGINT
# Fri, 27 Aug 2021 22:13:02 GMT
EXPOSE 5432
# Fri, 27 Aug 2021 22:13:03 GMT
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
	-	`sha256:c4a0027285a357c3031a13240a635cc7ebc3b2605492a295f9d844a95a150a2d`  
		Last Modified: Fri, 27 Aug 2021 22:42:13 GMT  
		Size: 77.7 MB (77733771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f80ffc4a1ed42d39f582086eb8a6ffb3f73bab0dd572ece3603ff45b30e44d5`  
		Last Modified: Fri, 27 Aug 2021 22:41:59 GMT  
		Size: 9.0 KB (9025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e26c46dcba46a84cb5d45ec070956bc6571083d6a03403c1f972df49e5baef90`  
		Last Modified: Fri, 27 Aug 2021 22:41:59 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d7c982a1820f41f0b875b2d15d7744226839c49d2b4a8f3dc5b625ee5f3e5fb`  
		Last Modified: Fri, 27 Aug 2021 22:41:59 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62d8f07f232e816305152e38202c9e6f3c3d38df05c80884f8af96c12db6956a`  
		Last Modified: Fri, 27 Aug 2021 22:41:59 GMT  
		Size: 4.4 KB (4406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:alpine` - linux; ppc64le

```console
$ docker pull postgres@sha256:1a9ca68648f15671ffdb44334e884745d71c679a25584f9e7f10dc78375720cb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **80.7 MB (80738091 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b76cb0909881af4717420f8d7a5d04d9bb7ba62f759542d19f3c344023d32414`
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
# Fri, 27 Aug 2021 21:49:37 GMT
ENV PG_MAJOR=13
# Fri, 27 Aug 2021 21:49:42 GMT
ENV PG_VERSION=13.4
# Fri, 27 Aug 2021 21:49:45 GMT
ENV PG_SHA256=ea93e10390245f1ce461a54eb5f99a48d8cabd3a08ce4d652ec2169a357bc0cd
# Fri, 27 Aug 2021 21:53:51 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm11-dev clang g++ 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Fri, 27 Aug 2021 21:54:30 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample
# Fri, 27 Aug 2021 21:54:45 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 27 Aug 2021 21:54:51 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 27 Aug 2021 21:55:12 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 27 Aug 2021 21:55:19 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 27 Aug 2021 21:55:24 GMT
COPY file:ad28506adc606e446eefc263bc99d4cb809e608d4f550956143bf13c82c91f85 in /usr/local/bin/ 
# Fri, 27 Aug 2021 21:55:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 Aug 2021 21:55:37 GMT
STOPSIGNAL SIGINT
# Fri, 27 Aug 2021 21:55:44 GMT
EXPOSE 5432
# Fri, 27 Aug 2021 21:55:51 GMT
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
	-	`sha256:0dc04751ec342a016dbec67fd0a9377873dd8d7e78cbc937bd51f2274678d2a0`  
		Last Modified: Fri, 27 Aug 2021 22:18:32 GMT  
		Size: 77.9 MB (77910584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b64c74fcdb2c236be8cdcdf223af7c3e218991a466abc0fddfea5191d1addbce`  
		Last Modified: Fri, 27 Aug 2021 22:18:19 GMT  
		Size: 9.0 KB (9024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2aa4460735f47ad418b395e6bc80ef487b21fa63c9307f8d6ee61b07a08c2071`  
		Last Modified: Fri, 27 Aug 2021 22:18:19 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7311d71c34803f2c6669e38f3e60f650da1e415451fef4801b312db30318d09`  
		Last Modified: Fri, 27 Aug 2021 22:18:19 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23e67c1dc5a3b38fbaa1f150a08461c0efc5e0d9d37ea26cfd8db3bf621129e8`  
		Last Modified: Fri, 27 Aug 2021 22:18:19 GMT  
		Size: 4.4 KB (4408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:alpine` - linux; s390x

```console
$ docker pull postgres@sha256:6d3549180d1a140ab459d36b2a96b6585800a24104f312cd73efef16b537209f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.0 MB (77042999 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd86812b9110d0d3182b40e6206464f76e00fffeed5e2244e0210f2e7bc918ff`
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
# Sat, 28 Aug 2021 00:53:29 GMT
ENV PG_MAJOR=13
# Sat, 28 Aug 2021 00:53:29 GMT
ENV PG_VERSION=13.4
# Sat, 28 Aug 2021 00:53:29 GMT
ENV PG_SHA256=ea93e10390245f1ce461a54eb5f99a48d8cabd3a08ce4d652ec2169a357bc0cd
# Sat, 28 Aug 2021 00:56:44 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm11-dev clang g++ 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Sat, 28 Aug 2021 00:56:47 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample
# Sat, 28 Aug 2021 00:56:48 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Sat, 28 Aug 2021 00:56:48 GMT
ENV PGDATA=/var/lib/postgresql/data
# Sat, 28 Aug 2021 00:56:49 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Sat, 28 Aug 2021 00:56:49 GMT
VOLUME [/var/lib/postgresql/data]
# Sat, 28 Aug 2021 00:56:49 GMT
COPY file:ad28506adc606e446eefc263bc99d4cb809e608d4f550956143bf13c82c91f85 in /usr/local/bin/ 
# Sat, 28 Aug 2021 00:56:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 28 Aug 2021 00:56:50 GMT
STOPSIGNAL SIGINT
# Sat, 28 Aug 2021 00:56:50 GMT
EXPOSE 5432
# Sat, 28 Aug 2021 00:56:50 GMT
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
	-	`sha256:48b806db2b46fec8bd09e4feb96b260add385b642f6192b1ea474a1f7418af39`  
		Last Modified: Sat, 28 Aug 2021 01:20:05 GMT  
		Size: 74.4 MB (74424315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f51befec433c48adc36c6a71e4388acb88da68adec80aa9033e0814fac6d375`  
		Last Modified: Sat, 28 Aug 2021 01:19:55 GMT  
		Size: 9.0 KB (9028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1c1699615db7b6d7d061729231235df69526604942ec01bc0515c9f5b49b1aa`  
		Last Modified: Sat, 28 Aug 2021 01:19:55 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b5422fe64c303ed209900d3d3323ffb7013ae6163e6faa789f21e1859cd23bd`  
		Last Modified: Sat, 28 Aug 2021 01:19:56 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36d344d0fd327f36327417f0aadd63f42268129023189bfa62817bb33d744ff3`  
		Last Modified: Sat, 28 Aug 2021 01:19:55 GMT  
		Size: 4.4 KB (4403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
