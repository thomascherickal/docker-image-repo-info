## `postgres:14beta2-alpine`

```console
$ docker pull postgres@sha256:65d709c4032154dc0df17ebc77eaa0f924137d4a5f4989595e778c3513e2996a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `postgres:14beta2-alpine` - linux; amd64

```console
$ docker pull postgres@sha256:dbcfabf699f6df33a81712716d0ef4e76961e5130159262c1099cdfe89107c73
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.3 MB (77309287 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a1be274409058e05b02d5b3b590aa2ea7f22606d660fd8bcd1f94139251f6cd6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 15 Jun 2021 22:19:37 GMT
ADD file:f278386b0cef68136129f5f58c52445590a417b624d62bca158d4dc926c340df in / 
# Tue, 15 Jun 2021 22:19:37 GMT
CMD ["/bin/sh"]
# Wed, 16 Jun 2021 22:24:56 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Wed, 16 Jun 2021 22:24:56 GMT
ENV LANG=en_US.utf8
# Wed, 16 Jun 2021 22:24:57 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 13 Jul 2021 18:40:04 GMT
ENV PG_MAJOR=14
# Tue, 13 Jul 2021 18:40:04 GMT
ENV PG_VERSION=14beta2
# Tue, 13 Jul 2021 18:40:04 GMT
ENV PG_SHA256=ffe64a76f50a2363443c1c9dc2195138933e931e351b74fb35a7935eae7c60a5
# Tue, 13 Jul 2021 18:46:12 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm11-dev clang g++ 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 		lz4-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 		--with-lz4 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Tue, 13 Jul 2021 18:46:15 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample
# Tue, 13 Jul 2021 18:46:18 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 13 Jul 2021 18:46:18 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 13 Jul 2021 18:46:20 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 13 Jul 2021 18:46:21 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 13 Jul 2021 18:46:21 GMT
COPY file:ad28506adc606e446eefc263bc99d4cb809e608d4f550956143bf13c82c91f85 in /usr/local/bin/ 
# Tue, 13 Jul 2021 18:46:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Jul 2021 18:46:22 GMT
STOPSIGNAL SIGINT
# Tue, 13 Jul 2021 18:46:23 GMT
EXPOSE 5432
# Tue, 13 Jul 2021 18:46:23 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:5843afab387455b37944e709ee8c78d7520df80f8d01cf7f861aae63beeddb6b`  
		Last Modified: Tue, 15 Jun 2021 22:20:04 GMT  
		Size: 2.8 MB (2811478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:525703b16f79bf722bb99ceb8d8e255d48302db2747d5f58db027abc3861c5ba`  
		Last Modified: Fri, 25 Jun 2021 19:36:39 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86f8340bd3d9f676a8b82d79fa7505af62500227d8991affdbacbdc428fb3c38`  
		Last Modified: Fri, 25 Jun 2021 19:36:38 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5a79fa0e97308dcac11f49c2a535b2267e0944910d0a09690a5f9564a911e1b`  
		Last Modified: Tue, 13 Jul 2021 18:49:28 GMT  
		Size: 74.5 MB (74482391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7122bd7e07c2156a0f776fee468935cb055db7fe0bc4d54d10513dd9fdbf9c0b`  
		Last Modified: Tue, 13 Jul 2021 18:49:15 GMT  
		Size: 9.2 KB (9229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9276c9b40429642fe2217c0c882950ae5e850852a6022ce902e1f222a911a32`  
		Last Modified: Tue, 13 Jul 2021 18:49:15 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5fb882dd5db870d1d066ab227ac968aff34a6a3e0887f6bb2b5c73638374b93`  
		Last Modified: Tue, 13 Jul 2021 18:49:15 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4533d0a6be2d198163b6d3e1ccbc4ba00f8472f9f823c53c9f778143dad63233`  
		Last Modified: Tue, 13 Jul 2021 18:49:15 GMT  
		Size: 4.4 KB (4402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:14beta2-alpine` - linux; arm variant v6

```console
$ docker pull postgres@sha256:bf217def6413b4ee96d8c3083df6637d55e6872a6216f36561f2d085998e2422
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.8 MB (75813650 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1db833338b08e7416993bb2cb6bb101b20fa01cd3a5d11c7b94caf6a41eaffba`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 15 Jun 2021 22:57:26 GMT
ADD file:c80bc2b093cbc0fc466582ef21cbed377de9fa874aedbf320079525ddacd1200 in / 
# Tue, 15 Jun 2021 22:57:26 GMT
CMD ["/bin/sh"]
# Mon, 21 Jun 2021 23:59:21 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Mon, 21 Jun 2021 23:59:22 GMT
ENV LANG=en_US.utf8
# Mon, 21 Jun 2021 23:59:23 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 13 Jul 2021 19:22:02 GMT
ENV PG_MAJOR=14
# Tue, 13 Jul 2021 19:22:02 GMT
ENV PG_VERSION=14beta2
# Tue, 13 Jul 2021 19:22:02 GMT
ENV PG_SHA256=ffe64a76f50a2363443c1c9dc2195138933e931e351b74fb35a7935eae7c60a5
# Tue, 13 Jul 2021 19:26:55 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm11-dev clang g++ 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 		lz4-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 		--with-lz4 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Tue, 13 Jul 2021 19:26:58 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample
# Tue, 13 Jul 2021 19:27:00 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 13 Jul 2021 19:27:00 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 13 Jul 2021 19:27:02 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 13 Jul 2021 19:27:02 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 13 Jul 2021 19:27:03 GMT
COPY file:ad28506adc606e446eefc263bc99d4cb809e608d4f550956143bf13c82c91f85 in /usr/local/bin/ 
# Tue, 13 Jul 2021 19:27:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Jul 2021 19:27:04 GMT
STOPSIGNAL SIGINT
# Tue, 13 Jul 2021 19:27:05 GMT
EXPOSE 5432
# Tue, 13 Jul 2021 19:27:05 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:b4c9a0924271af3466de27804af26420eb58da1466e7eaaba127d178b380fea3`  
		Last Modified: Tue, 15 Jun 2021 22:58:47 GMT  
		Size: 2.6 MB (2624382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf406c5d7ec791a51d8d15393de932c25f8dc5fe76a7c3dd40e254acd03f3ee5`  
		Last Modified: Fri, 25 Jun 2021 19:33:43 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ac4c25d65a7592994fa168d460c4333a15dc5e1e74fa8294e49a39625239f42`  
		Last Modified: Fri, 25 Jun 2021 19:33:42 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f57e0cfd89a429a1da39b3b34a69eb968941a4caa89702f55aad3e87923e8c8`  
		Last Modified: Tue, 13 Jul 2021 19:30:50 GMT  
		Size: 73.2 MB (73173843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92d4e19352c4d8922e23db62a3265ca4c235c9c8aae238d62cae2ccb9369b6e6`  
		Last Modified: Tue, 13 Jul 2021 19:30:07 GMT  
		Size: 9.2 KB (9232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c585c3d30a6e709525bcaf4613b6e34b78b77893c4818c80131a3b238e14ae3`  
		Last Modified: Tue, 13 Jul 2021 19:30:07 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9007a29d145309be3b821e71d6da3945eeba2e362e59b6994a0d8e84e9001326`  
		Last Modified: Tue, 13 Jul 2021 19:30:07 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bbb51e45362aa2089d6dea8754b36fef36441b98260ea7cff0bc26ace9e023a`  
		Last Modified: Tue, 13 Jul 2021 19:30:07 GMT  
		Size: 4.4 KB (4407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:14beta2-alpine` - linux; arm variant v7

```console
$ docker pull postgres@sha256:1295e0b964bce22ab48e8c6cc5aa3716afa49875f775effe5b61fb8eaa59e22d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.5 MB (71494262 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ef2077d209d4ec1481d4882aeb76556c2498ee55615b031b62b8fb0e7b2ae8c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 15 Jun 2021 23:15:05 GMT
ADD file:416a8b507abdc6bdcb22997a4be0a4170796c3f9f77e315b2dbff2b0a212bc68 in / 
# Tue, 15 Jun 2021 23:15:06 GMT
CMD ["/bin/sh"]
# Wed, 23 Jun 2021 19:33:12 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Wed, 23 Jun 2021 19:33:13 GMT
ENV LANG=en_US.utf8
# Wed, 23 Jun 2021 19:33:15 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 13 Jul 2021 19:27:32 GMT
ENV PG_MAJOR=14
# Tue, 13 Jul 2021 19:27:33 GMT
ENV PG_VERSION=14beta2
# Tue, 13 Jul 2021 19:27:33 GMT
ENV PG_SHA256=ffe64a76f50a2363443c1c9dc2195138933e931e351b74fb35a7935eae7c60a5
# Tue, 13 Jul 2021 19:32:08 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm11-dev clang g++ 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 		lz4-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 		--with-lz4 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Tue, 13 Jul 2021 19:32:11 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample
# Tue, 13 Jul 2021 19:32:12 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 13 Jul 2021 19:32:13 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 13 Jul 2021 19:32:15 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 13 Jul 2021 19:32:16 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 13 Jul 2021 19:32:17 GMT
COPY file:ad28506adc606e446eefc263bc99d4cb809e608d4f550956143bf13c82c91f85 in /usr/local/bin/ 
# Tue, 13 Jul 2021 19:32:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Jul 2021 19:32:18 GMT
STOPSIGNAL SIGINT
# Tue, 13 Jul 2021 19:32:18 GMT
EXPOSE 5432
# Tue, 13 Jul 2021 19:32:19 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:136482bf81d1fa351b424ebb8c7e34d15f2c5ed3fc0b66b544b8312bda3d52d9`  
		Last Modified: Tue, 15 Jun 2021 23:16:40 GMT  
		Size: 2.4 MB (2427917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de358c6e46472c219573fa1a55631af8c7bf91e9b1ea76d0f6d9180027b05b17`  
		Last Modified: Fri, 25 Jun 2021 20:09:13 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ab295b5804b0a6e29db014f413a57fc1655f93e692da751d046d79837cc0a4e`  
		Last Modified: Fri, 25 Jun 2021 20:09:13 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28e308eca6f27c001f4767d180794180982a5648cd962781dd34eddfd3f7d489`  
		Last Modified: Tue, 13 Jul 2021 19:40:28 GMT  
		Size: 69.1 MB (69050919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feff0f9b052a0dd547a7ad3becd2bab426fc34a7f6c1ecd052937664d2a3ea69`  
		Last Modified: Tue, 13 Jul 2021 19:39:51 GMT  
		Size: 9.2 KB (9234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:592d48cd43e4d6748c17b43f4255e71548a31d1a92f13677ed0e4e8fd0db6d1d`  
		Last Modified: Tue, 13 Jul 2021 19:39:51 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5665f5220f4b4f6fbd2c907ba3df746d5d3714e8d5022ff7720be06b7ad69c11`  
		Last Modified: Tue, 13 Jul 2021 19:39:51 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:366d5d54f21c9a1a0592aa5dfaf9175756804f0173dbd35df46ba71f598e1a90`  
		Last Modified: Tue, 13 Jul 2021 19:39:51 GMT  
		Size: 4.4 KB (4406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:14beta2-alpine` - linux; arm64 variant v8

```console
$ docker pull postgres@sha256:8c285a31f4f3d780b8e3e1cdde6bc37a6655732cd8d27870a6610f4e06f36fb3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.2 MB (76200158 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec93819499324620e87eda042c178b14544c28a343fa42f6d4f1273b3894d37c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 15 Jun 2021 21:44:56 GMT
ADD file:6797caacbfe41bfe44000b39ed017016c6fcc492b3d6557cdaba88536df6c876 in / 
# Tue, 15 Jun 2021 21:44:56 GMT
CMD ["/bin/sh"]
# Wed, 16 Jun 2021 23:08:22 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Wed, 16 Jun 2021 23:08:23 GMT
ENV LANG=en_US.utf8
# Wed, 16 Jun 2021 23:08:23 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 13 Jul 2021 18:43:26 GMT
ENV PG_MAJOR=14
# Tue, 13 Jul 2021 18:43:27 GMT
ENV PG_VERSION=14beta2
# Tue, 13 Jul 2021 18:43:27 GMT
ENV PG_SHA256=ffe64a76f50a2363443c1c9dc2195138933e931e351b74fb35a7935eae7c60a5
# Tue, 13 Jul 2021 18:47:57 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm11-dev clang g++ 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 		lz4-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 		--with-lz4 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Tue, 13 Jul 2021 18:47:58 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample
# Tue, 13 Jul 2021 18:47:59 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 13 Jul 2021 18:47:59 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 13 Jul 2021 18:48:00 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 13 Jul 2021 18:48:00 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 13 Jul 2021 18:48:00 GMT
COPY file:ad28506adc606e446eefc263bc99d4cb809e608d4f550956143bf13c82c91f85 in /usr/local/bin/ 
# Tue, 13 Jul 2021 18:48:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Jul 2021 18:48:00 GMT
STOPSIGNAL SIGINT
# Tue, 13 Jul 2021 18:48:01 GMT
EXPOSE 5432
# Tue, 13 Jul 2021 18:48:01 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:58ab47519297212468320b23b8100fc1b2b96e8d342040806ae509a778a0a07a`  
		Last Modified: Tue, 15 Jun 2021 21:46:03 GMT  
		Size: 2.7 MB (2709626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:014ca0527e174cf1bce26a8ba236f17ca0ffd4ebd97fd99b18dd76c382ea5bca`  
		Last Modified: Fri, 25 Jun 2021 19:17:39 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee9ed2adb5ac9aa385033227091a3f86d6ea0b74ea30e6ee625da34db4ca5a20`  
		Last Modified: Fri, 25 Jun 2021 19:17:39 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4070ab654ac519490abac73e08c5398c4360853f28d29f9f1f7f9bbcc7ec79ec`  
		Last Modified: Tue, 13 Jul 2021 18:51:51 GMT  
		Size: 73.5 MB (73475108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6346f6df0dadc1b536fc2e71424b5e8f9de96ed9c0efe5bdb3f383c4806f181`  
		Last Modified: Tue, 13 Jul 2021 18:51:40 GMT  
		Size: 9.2 KB (9227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62f23482ec32d2df6da72da30a2210a141c88203e4ac5193f3a191c46b91ba8d`  
		Last Modified: Tue, 13 Jul 2021 18:51:40 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6333e0a9a982cd3e59f25b752cf3fbbc53dba52659214bae84c0d14d10cdbc3`  
		Last Modified: Tue, 13 Jul 2021 18:51:40 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d2250b5b7eefcc150754cf6b64a7078377734350f1cbb4b86e4c2151a01b01c`  
		Last Modified: Tue, 13 Jul 2021 18:51:40 GMT  
		Size: 4.4 KB (4405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:14beta2-alpine` - linux; 386

```console
$ docker pull postgres@sha256:960d0304e4f935001221f5b70f8c598029df822d1973d4b45a19ed9f1a5cb697
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **82.1 MB (82081658 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e146a413a0d1142663aa808e585a4a57777f28fc054b3fc1bf643d5ae9cbc664`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 15 Jun 2021 21:38:30 GMT
ADD file:3b0fe1454491bb05e218b090fd461f2fd39546aa4a53eb3f953ee8eae149ac57 in / 
# Tue, 15 Jun 2021 21:38:30 GMT
CMD ["/bin/sh"]
# Wed, 16 Jun 2021 23:08:39 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Wed, 16 Jun 2021 23:08:39 GMT
ENV LANG=en_US.utf8
# Wed, 16 Jun 2021 23:08:40 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 13 Jul 2021 18:43:49 GMT
ENV PG_MAJOR=14
# Tue, 13 Jul 2021 18:43:50 GMT
ENV PG_VERSION=14beta2
# Tue, 13 Jul 2021 18:43:50 GMT
ENV PG_SHA256=ffe64a76f50a2363443c1c9dc2195138933e931e351b74fb35a7935eae7c60a5
# Tue, 13 Jul 2021 18:50:28 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm11-dev clang g++ 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 		lz4-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 		--with-lz4 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Tue, 13 Jul 2021 18:50:29 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample
# Tue, 13 Jul 2021 18:50:30 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 13 Jul 2021 18:50:30 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 13 Jul 2021 18:50:31 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 13 Jul 2021 18:50:31 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 13 Jul 2021 18:50:31 GMT
COPY file:ad28506adc606e446eefc263bc99d4cb809e608d4f550956143bf13c82c91f85 in /usr/local/bin/ 
# Tue, 13 Jul 2021 18:50:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Jul 2021 18:50:32 GMT
STOPSIGNAL SIGINT
# Tue, 13 Jul 2021 18:50:32 GMT
EXPOSE 5432
# Tue, 13 Jul 2021 18:50:32 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:be21df321efb39c5daf3151073ebff7688e15ea6cd5158878bc9559a5db76ac6`  
		Last Modified: Tue, 15 Jun 2021 21:39:16 GMT  
		Size: 2.8 MB (2820718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c53f1659e95a66231a1dc5b485721b25715f9ac8bd845eb152e34f662adad6d5`  
		Last Modified: Fri, 25 Jun 2021 19:32:06 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6739c4193b8d53cc791a1e1b0e06cb86b4dd9d32c22cb9437cb4a83579d6c38`  
		Last Modified: Fri, 25 Jun 2021 19:32:06 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a497cb41d8d3307b940facf15e6558c00231b7350e7f4cb038d8a9eff6f49cee`  
		Last Modified: Tue, 13 Jul 2021 18:54:32 GMT  
		Size: 79.2 MB (79245519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bc0684319092450263051af1c1458d140b7f495befd42e4e403cdb8a23b06dc`  
		Last Modified: Tue, 13 Jul 2021 18:54:18 GMT  
		Size: 9.2 KB (9230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef7e4ef85cfcc312f7d793e4e25962d9c7e036ede5953c717052c0b5001deeac`  
		Last Modified: Tue, 13 Jul 2021 18:54:18 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f248641279a72ad98eed465d958cdc00927ce91529a6dc0790e9abe1774f119`  
		Last Modified: Tue, 13 Jul 2021 18:54:18 GMT  
		Size: 192.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:153a3001a608206397c983b07e018f21c564c15c34054f8b292e21caa3644e2a`  
		Last Modified: Tue, 13 Jul 2021 18:54:18 GMT  
		Size: 4.4 KB (4408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
