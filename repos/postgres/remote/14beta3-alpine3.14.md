## `postgres:14beta3-alpine3.14`

```console
$ docker pull postgres@sha256:fc1f6462526d86523bb2a9d1d5a3305fc453fb6687e42d8462b406ea9bc06074
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

### `postgres:14beta3-alpine3.14` - linux; amd64

```console
$ docker pull postgres@sha256:f09659f13a844643394013e36d2c24fde67648f75928fceb39385a4079ffa7f0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.3 MB (77320888 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:429af77d04e230cbcd57f75651cbf3ede7b8a4dd25efbc73006822a55d96ce55`
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
# Fri, 27 Aug 2021 22:48:03 GMT
ENV PG_MAJOR=14
# Fri, 27 Aug 2021 22:48:04 GMT
ENV PG_VERSION=14beta3
# Fri, 27 Aug 2021 22:48:04 GMT
ENV PG_SHA256=2ea265980193db70106576201a2fee5b2d72bf9890d3911ddd374d4830624bfa
# Fri, 27 Aug 2021 22:54:41 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm11-dev clang g++ 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 		lz4-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 		--with-lz4 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Fri, 27 Aug 2021 22:54:42 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample
# Fri, 27 Aug 2021 22:54:43 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 27 Aug 2021 22:54:43 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 27 Aug 2021 22:54:44 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 27 Aug 2021 22:54:44 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 27 Aug 2021 22:54:44 GMT
COPY file:ad28506adc606e446eefc263bc99d4cb809e608d4f550956143bf13c82c91f85 in /usr/local/bin/ 
# Fri, 27 Aug 2021 22:54:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 Aug 2021 22:54:44 GMT
STOPSIGNAL SIGINT
# Fri, 27 Aug 2021 22:54:45 GMT
EXPOSE 5432
# Fri, 27 Aug 2021 22:54:45 GMT
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
	-	`sha256:c2306860552496fb9a83f67b39ee50fb7d3cf9204bb835c309b5740f00a8c9bb`  
		Last Modified: Fri, 27 Aug 2021 23:28:28 GMT  
		Size: 74.5 MB (74491047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a63ccf89bce168b7fa490646c096cbd2e3ba3169aaf2035b0e70a8965494fa6`  
		Last Modified: Fri, 27 Aug 2021 23:28:17 GMT  
		Size: 9.2 KB (9204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3dbe99abe7d69e1622373957826eb1ba46e95f22a4d77b2f5db6d622d8b9374`  
		Last Modified: Fri, 27 Aug 2021 23:28:17 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5397f06ed4f5fea67bdbf4710cf71a591d4f08cc33095b24a56560c30f0bb125`  
		Last Modified: Fri, 27 Aug 2021 23:28:17 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57c459d6b3d2376df61e8100f598bc722bccd1233a08bb4f9a7de34dddd9bd47`  
		Last Modified: Fri, 27 Aug 2021 23:28:17 GMT  
		Size: 4.4 KB (4404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:14beta3-alpine3.14` - linux; arm variant v6

```console
$ docker pull postgres@sha256:6be52cc61b109ae7bae2804c3843cfad360db769b30fd78b46f846a0040caa6d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.8 MB (75833652 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:72fe9ce069721bd07ea4795c23533b48cccd5c71666d52697418f377065a3af7`
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
# Fri, 27 Aug 2021 22:04:34 GMT
ENV PG_MAJOR=14
# Fri, 27 Aug 2021 22:04:35 GMT
ENV PG_VERSION=14beta3
# Fri, 27 Aug 2021 22:04:36 GMT
ENV PG_SHA256=2ea265980193db70106576201a2fee5b2d72bf9890d3911ddd374d4830624bfa
# Fri, 27 Aug 2021 22:10:41 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm11-dev clang g++ 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 		lz4-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 		--with-lz4 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Fri, 27 Aug 2021 22:10:43 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample
# Fri, 27 Aug 2021 22:10:44 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 27 Aug 2021 22:10:45 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 27 Aug 2021 22:10:46 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 27 Aug 2021 22:10:47 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 27 Aug 2021 22:10:47 GMT
COPY file:ad28506adc606e446eefc263bc99d4cb809e608d4f550956143bf13c82c91f85 in /usr/local/bin/ 
# Fri, 27 Aug 2021 22:10:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 Aug 2021 22:10:48 GMT
STOPSIGNAL SIGINT
# Fri, 27 Aug 2021 22:10:49 GMT
EXPOSE 5432
# Fri, 27 Aug 2021 22:10:49 GMT
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
	-	`sha256:6e5710218bbe3f26f092a90864baa3651b547ccbccb4af8bdd6103082dab05b3`  
		Last Modified: Fri, 27 Aug 2021 22:37:02 GMT  
		Size: 73.2 MB (73190808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cdc0c3f831694d649aacd35be7c2b230d76600745724c2ec2e0898bfc6e462a`  
		Last Modified: Fri, 27 Aug 2021 22:36:20 GMT  
		Size: 9.2 KB (9204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8f3d2ff03a53a1af1c4768f2a44accb1e8e036c6ac9bb2a396bf6fde3616fce`  
		Last Modified: Fri, 27 Aug 2021 22:36:20 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af15e91f302b2dee44b67f8ef1714d081b3c243c6dac1b0f31581609c8547946`  
		Last Modified: Fri, 27 Aug 2021 22:36:20 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98695eaea7c70f888f3cfe78a116b3f3fea1a4673c08db54ddbb54d51172ef43`  
		Last Modified: Fri, 27 Aug 2021 22:36:20 GMT  
		Size: 4.4 KB (4404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:14beta3-alpine3.14` - linux; arm variant v7

```console
$ docker pull postgres@sha256:51a7dc701e4d6a75e273a680109e796d2675107c569ad4a5e970a9b86651d04a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.5 MB (71514092 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b88daa3f2fafc503ce4362f3151be9afdd1f81ba2c6a6415435be4b21a188f7d`
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
# Sat, 28 Aug 2021 00:08:10 GMT
ENV PG_MAJOR=14
# Sat, 28 Aug 2021 00:08:10 GMT
ENV PG_VERSION=14beta3
# Sat, 28 Aug 2021 00:08:11 GMT
ENV PG_SHA256=2ea265980193db70106576201a2fee5b2d72bf9890d3911ddd374d4830624bfa
# Sat, 28 Aug 2021 00:12:52 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm11-dev clang g++ 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 		lz4-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 		--with-lz4 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Sat, 28 Aug 2021 00:12:55 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample
# Sat, 28 Aug 2021 00:12:56 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Sat, 28 Aug 2021 00:12:57 GMT
ENV PGDATA=/var/lib/postgresql/data
# Sat, 28 Aug 2021 00:12:59 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Sat, 28 Aug 2021 00:12:59 GMT
VOLUME [/var/lib/postgresql/data]
# Sat, 28 Aug 2021 00:13:00 GMT
COPY file:ad28506adc606e446eefc263bc99d4cb809e608d4f550956143bf13c82c91f85 in /usr/local/bin/ 
# Sat, 28 Aug 2021 00:13:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 28 Aug 2021 00:13:01 GMT
STOPSIGNAL SIGINT
# Sat, 28 Aug 2021 00:13:01 GMT
EXPOSE 5432
# Sat, 28 Aug 2021 00:13:02 GMT
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
	-	`sha256:76c13460735d96c6e78b9c9ac128511874c487071af09922e7c8edfc04091b3d`  
		Last Modified: Sat, 28 Aug 2021 00:41:55 GMT  
		Size: 69.1 MB (69068272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c2e696aabcef242c0e0778ce5a5dd341660be37dab374c7d5b50ab37bbb3662`  
		Last Modified: Sat, 28 Aug 2021 00:41:19 GMT  
		Size: 9.2 KB (9208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd229b5c2a0e70d9d3af8b1f2897c5ba8d5f178598e8a37463d523c0ff3d7b29`  
		Last Modified: Sat, 28 Aug 2021 00:41:19 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62c44d9496bfcd57a877c09b964284a13e8928e3f44d2610d222a534f98c9560`  
		Last Modified: Sat, 28 Aug 2021 00:41:19 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c577d174895c02dae197fb35d41d0053373bd3cfb83f99e501ee74211b899ec`  
		Last Modified: Sat, 28 Aug 2021 00:41:19 GMT  
		Size: 4.4 KB (4405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:14beta3-alpine3.14` - linux; arm64 variant v8

```console
$ docker pull postgres@sha256:162f6f821c0f71b4ca91c3ae69f5cfd9ce45418abec65129e2eccae3ea14b0a0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.2 MB (76215826 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b28ebe81a1575a2d4b9d646ab63e7346385574451e72667831c4435d716b9d4`
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
# Sat, 28 Aug 2021 00:44:22 GMT
ENV PG_MAJOR=14
# Sat, 28 Aug 2021 00:44:22 GMT
ENV PG_VERSION=14beta3
# Sat, 28 Aug 2021 00:44:22 GMT
ENV PG_SHA256=2ea265980193db70106576201a2fee5b2d72bf9890d3911ddd374d4830624bfa
# Sat, 28 Aug 2021 00:48:48 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm11-dev clang g++ 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 		lz4-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 		--with-lz4 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Sat, 28 Aug 2021 00:48:49 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample
# Sat, 28 Aug 2021 00:48:49 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Sat, 28 Aug 2021 00:48:50 GMT
ENV PGDATA=/var/lib/postgresql/data
# Sat, 28 Aug 2021 00:48:50 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Sat, 28 Aug 2021 00:48:50 GMT
VOLUME [/var/lib/postgresql/data]
# Sat, 28 Aug 2021 00:48:51 GMT
COPY file:ad28506adc606e446eefc263bc99d4cb809e608d4f550956143bf13c82c91f85 in /usr/local/bin/ 
# Sat, 28 Aug 2021 00:48:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 28 Aug 2021 00:48:51 GMT
STOPSIGNAL SIGINT
# Sat, 28 Aug 2021 00:48:51 GMT
EXPOSE 5432
# Sat, 28 Aug 2021 00:48:51 GMT
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
	-	`sha256:33ac35981c87445ebf1c982ebf8b7edd8d7fe7c6a013676091fdb766d6f889a8`  
		Last Modified: Sat, 28 Aug 2021 01:11:14 GMT  
		Size: 73.5 MB (73488602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:056243e2b97bf19c409542221aa3b621a9aa6c7235d98d9e67041ce3796dffd0`  
		Last Modified: Sat, 28 Aug 2021 01:11:03 GMT  
		Size: 9.2 KB (9199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89a1ee4cf750a13120ab956158b73a42702ac8d513311ee392aef14e5278b4ad`  
		Last Modified: Sat, 28 Aug 2021 01:11:03 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbbb5f3a7e0a0575640f97c1c052ce0e7121590780904c03e02d896b68e1b144`  
		Last Modified: Sat, 28 Aug 2021 01:11:04 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ff55d55c760d78edd76fa177a6c9c2de3ba25a9fa57b8f4c72b7a1efa06a1b6`  
		Last Modified: Sat, 28 Aug 2021 01:11:03 GMT  
		Size: 4.4 KB (4406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:14beta3-alpine3.14` - linux; 386

```console
$ docker pull postgres@sha256:d3a223160dea07039cd198d37284e41fb9b5ce0e710b35f1048b9094492d40f8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **82.1 MB (82097515 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c579ff7f2ad373630be1f164c378bfdf7d0b11247db8289c1751e62cf4f80c92`
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
# Fri, 27 Aug 2021 21:55:06 GMT
ENV PG_MAJOR=14
# Fri, 27 Aug 2021 21:55:06 GMT
ENV PG_VERSION=14beta3
# Fri, 27 Aug 2021 21:55:06 GMT
ENV PG_SHA256=2ea265980193db70106576201a2fee5b2d72bf9890d3911ddd374d4830624bfa
# Fri, 27 Aug 2021 22:04:24 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm11-dev clang g++ 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 		lz4-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 		--with-lz4 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Fri, 27 Aug 2021 22:04:26 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample
# Fri, 27 Aug 2021 22:04:27 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 27 Aug 2021 22:04:27 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 27 Aug 2021 22:04:28 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 27 Aug 2021 22:04:28 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 27 Aug 2021 22:04:29 GMT
COPY file:ad28506adc606e446eefc263bc99d4cb809e608d4f550956143bf13c82c91f85 in /usr/local/bin/ 
# Fri, 27 Aug 2021 22:04:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 Aug 2021 22:04:29 GMT
STOPSIGNAL SIGINT
# Fri, 27 Aug 2021 22:04:29 GMT
EXPOSE 5432
# Fri, 27 Aug 2021 22:04:30 GMT
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
	-	`sha256:afe82d87e901346f7780e2f7e2a3d1df75490be7cb082dac0ef4a9302e846d22`  
		Last Modified: Fri, 27 Aug 2021 22:41:42 GMT  
		Size: 79.3 MB (79259265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c77687b257cb68df33b4c797a9625e3d0c90e3e82b2859be994f625d4b96aeeb`  
		Last Modified: Fri, 27 Aug 2021 22:41:27 GMT  
		Size: 9.2 KB (9202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3519394581e99a0440b84be579e7bb280ccc4b7cf6f2b91e633ad6dfc102c6c2`  
		Last Modified: Fri, 27 Aug 2021 22:41:27 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e162c52e3d7d90390916d64fce588a5889efaa31893113da41c6f4dae268f4cf`  
		Last Modified: Fri, 27 Aug 2021 22:41:27 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82bb9b984bb81034002e1b2a81d43e5b71e03e9bf922d6342d3d2024b55bee99`  
		Last Modified: Fri, 27 Aug 2021 22:41:27 GMT  
		Size: 4.4 KB (4404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:14beta3-alpine3.14` - linux; ppc64le

```console
$ docker pull postgres@sha256:4d827b23294508f444bf39f4944d918d85a23698c600968c5a34de3ac1620ff4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **82.3 MB (82347954 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc9dc818357453b47a6576f3b84a8b5247d9f97640013c7d17d7361a0709fbcf`
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
# Fri, 27 Aug 2021 21:43:53 GMT
ENV PG_MAJOR=14
# Fri, 27 Aug 2021 21:43:57 GMT
ENV PG_VERSION=14beta3
# Fri, 27 Aug 2021 21:43:59 GMT
ENV PG_SHA256=2ea265980193db70106576201a2fee5b2d72bf9890d3911ddd374d4830624bfa
# Fri, 27 Aug 2021 21:48:15 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm11-dev clang g++ 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 		lz4-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 		--with-lz4 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Fri, 27 Aug 2021 21:48:28 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample
# Fri, 27 Aug 2021 21:48:37 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 27 Aug 2021 21:48:42 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 27 Aug 2021 21:48:52 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 27 Aug 2021 21:49:02 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 27 Aug 2021 21:49:05 GMT
COPY file:ad28506adc606e446eefc263bc99d4cb809e608d4f550956143bf13c82c91f85 in /usr/local/bin/ 
# Fri, 27 Aug 2021 21:49:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 Aug 2021 21:49:11 GMT
STOPSIGNAL SIGINT
# Fri, 27 Aug 2021 21:49:14 GMT
EXPOSE 5432
# Fri, 27 Aug 2021 21:49:18 GMT
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
	-	`sha256:99147b644513abfe0ef9b702a7cb3c148f004e14e63934d1c30a7806261f355f`  
		Last Modified: Fri, 27 Aug 2021 22:18:01 GMT  
		Size: 79.5 MB (79520268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af3dd777258e9ab9b1c49bdf8c0a4518e7ed73096e9b93753f8785b6265cd9ff`  
		Last Modified: Fri, 27 Aug 2021 22:17:34 GMT  
		Size: 9.2 KB (9203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57f7060aa44f7d5cc77d46a11387e1ec573ff212a61e19129cf8a953bd18984d`  
		Last Modified: Fri, 27 Aug 2021 22:17:34 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edf9134880081d5de28684776960d5325f7d5b69cc8ec97ba40c06cf85e3c76e`  
		Last Modified: Fri, 27 Aug 2021 22:17:34 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8eb03bd1913a6131ec9480a5d0060e67d57b6771d47277c81951b99737b9cfb6`  
		Last Modified: Fri, 27 Aug 2021 22:17:34 GMT  
		Size: 4.4 KB (4405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:14beta3-alpine3.14` - linux; s390x

```console
$ docker pull postgres@sha256:fb8550d9895df989a91c15009ac01e9586e3f985152fb30507ced08661a796bd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **78.6 MB (78603436 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fd586d1d67935c8e9cc1b5eaf8a2c299ccb24a03e79d136cc6227ea8cf164376`
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
# Sat, 28 Aug 2021 00:49:32 GMT
ENV PG_MAJOR=14
# Sat, 28 Aug 2021 00:49:33 GMT
ENV PG_VERSION=14beta3
# Sat, 28 Aug 2021 00:49:33 GMT
ENV PG_SHA256=2ea265980193db70106576201a2fee5b2d72bf9890d3911ddd374d4830624bfa
# Sat, 28 Aug 2021 00:52:54 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm11-dev clang g++ 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 		lz4-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 		--with-lz4 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Sat, 28 Aug 2021 00:52:59 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample
# Sat, 28 Aug 2021 00:52:59 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Sat, 28 Aug 2021 00:52:59 GMT
ENV PGDATA=/var/lib/postgresql/data
# Sat, 28 Aug 2021 00:53:00 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Sat, 28 Aug 2021 00:53:01 GMT
VOLUME [/var/lib/postgresql/data]
# Sat, 28 Aug 2021 00:53:01 GMT
COPY file:ad28506adc606e446eefc263bc99d4cb809e608d4f550956143bf13c82c91f85 in /usr/local/bin/ 
# Sat, 28 Aug 2021 00:53:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 28 Aug 2021 00:53:02 GMT
STOPSIGNAL SIGINT
# Sat, 28 Aug 2021 00:53:02 GMT
EXPOSE 5432
# Sat, 28 Aug 2021 00:53:02 GMT
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
	-	`sha256:c0755d1060476fc6e2d0edb9f4793e95554d1a23484870b2c5d8296ad736492b`  
		Last Modified: Sat, 28 Aug 2021 01:19:40 GMT  
		Size: 76.0 MB (75984576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04344ec486ae3ecca94701b5631ef757c27dff3ed9a13a588930fb5a8e82fe69`  
		Last Modified: Sat, 28 Aug 2021 01:19:31 GMT  
		Size: 9.2 KB (9204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f145056b6b82fdd78465869f91e33c18ec284db59e64833f02b59c1b290814c6`  
		Last Modified: Sat, 28 Aug 2021 01:19:31 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c9046e4c9e9a5907805747c3b320b807f17f1634f656a59693e5e5b1b81c1b4`  
		Last Modified: Sat, 28 Aug 2021 01:19:31 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d41f6a60bd173cd536a2eaf40d6cc22b0e949819caba756fc8bab4914336a84`  
		Last Modified: Sat, 28 Aug 2021 01:19:31 GMT  
		Size: 4.4 KB (4403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
