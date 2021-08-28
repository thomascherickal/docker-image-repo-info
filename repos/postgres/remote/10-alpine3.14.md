## `postgres:10-alpine3.14`

```console
$ docker pull postgres@sha256:5450449112486d392b231a7bcfcd7e61a2d2882fb3e9546939d1d0f12d520e53
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

### `postgres:10-alpine3.14` - linux; amd64

```console
$ docker pull postgres@sha256:9ce18fb55e6e141b9193beeca644edf36ddd757b302b6bbde0d7b6f414f83bc8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.7 MB (28660684 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:17ec9988ae216f69d9e6528aae17a9fce29a2b7951313de9a34802528116f2eb`
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
# Fri, 27 Aug 2021 23:17:09 GMT
ENV PG_MAJOR=10
# Fri, 27 Aug 2021 23:17:09 GMT
ENV PG_VERSION=10.18
# Fri, 27 Aug 2021 23:17:09 GMT
ENV PG_SHA256=57477c2edc82c3f86a74747707b3babc1f301f389315ae14e819e025c0ba3801
# Fri, 27 Aug 2021 23:21:58 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Fri, 27 Aug 2021 23:21:59 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample
# Fri, 27 Aug 2021 23:22:01 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 27 Aug 2021 23:22:01 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 27 Aug 2021 23:22:03 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 27 Aug 2021 23:22:03 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 27 Aug 2021 23:22:03 GMT
COPY file:ad28506adc606e446eefc263bc99d4cb809e608d4f550956143bf13c82c91f85 in /usr/local/bin/ 
# Fri, 27 Aug 2021 23:22:04 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 27 Aug 2021 23:22:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 Aug 2021 23:22:04 GMT
STOPSIGNAL SIGINT
# Fri, 27 Aug 2021 23:22:05 GMT
EXPOSE 5432
# Fri, 27 Aug 2021 23:22:05 GMT
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
	-	`sha256:c0911b5b83247bf778b746ca1cdb75ff9f135705b4f6644ea7adb654ceb88a37`  
		Last Modified: Fri, 27 Aug 2021 23:30:22 GMT  
		Size: 25.8 MB (25832193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11ce96790b22a67b27bcbc09bb5bca0383e1a7eb99c0cc3ed628715df3b38377`  
		Last Modified: Fri, 27 Aug 2021 23:30:15 GMT  
		Size: 7.7 KB (7732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:638c20c41c011133224b810081d40db4184d92eccfe9602109dbe86b372f279e`  
		Last Modified: Fri, 27 Aug 2021 23:30:15 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84d4ffed5e4e0d32baf7a7584df616495b44807557944f240ca5770b3218da51`  
		Last Modified: Fri, 27 Aug 2021 23:30:15 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a91ec44e1b4b874dbdb702d8c5a3c037908db9d679288b20038bdf53b94b6dac`  
		Last Modified: Fri, 27 Aug 2021 23:30:15 GMT  
		Size: 4.4 KB (4405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d2fbc558f889d7c8fdbcc955cc4c4e412cc4525754dfa246e88f85af78982c4`  
		Last Modified: Fri, 27 Aug 2021 23:30:15 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:10-alpine3.14` - linux; arm variant v6

```console
$ docker pull postgres@sha256:ed51adfc59c9bc52c333148ec1d02c71ad196a942820fe0097ae6735390412bb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.8 MB (27803074 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:740a81c446eaf1b828e7aad45168c6bddb04e431149d0d1106649fca958e1c45`
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
# Fri, 27 Aug 2021 22:26:22 GMT
ENV PG_MAJOR=10
# Fri, 27 Aug 2021 22:26:23 GMT
ENV PG_VERSION=10.18
# Fri, 27 Aug 2021 22:26:23 GMT
ENV PG_SHA256=57477c2edc82c3f86a74747707b3babc1f301f389315ae14e819e025c0ba3801
# Fri, 27 Aug 2021 22:29:57 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Fri, 27 Aug 2021 22:29:59 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample
# Fri, 27 Aug 2021 22:30:00 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 27 Aug 2021 22:30:01 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 27 Aug 2021 22:30:02 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 27 Aug 2021 22:30:03 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 27 Aug 2021 22:30:03 GMT
COPY file:ad28506adc606e446eefc263bc99d4cb809e608d4f550956143bf13c82c91f85 in /usr/local/bin/ 
# Fri, 27 Aug 2021 22:30:05 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 27 Aug 2021 22:30:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 Aug 2021 22:30:06 GMT
STOPSIGNAL SIGINT
# Fri, 27 Aug 2021 22:30:06 GMT
EXPOSE 5432
# Fri, 27 Aug 2021 22:30:07 GMT
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
	-	`sha256:8911da316502b4326712a4303b621e5b7c101e6e764500fc669ada2cc3101c2c`  
		Last Modified: Fri, 27 Aug 2021 22:40:42 GMT  
		Size: 25.2 MB (25161581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b022f7f87311be7935fce408e384441dc2eccca19c29a14afa25b0fcd01dde9`  
		Last Modified: Fri, 27 Aug 2021 22:40:28 GMT  
		Size: 7.7 KB (7732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7fcb3231daec06a8789e75236e5b28bf9ed7369b6145d4d2b05c54e8089b950`  
		Last Modified: Fri, 27 Aug 2021 22:40:28 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6cb572b73011a307351ece4ceb2567635649560af15c5bb8b582f60d3dc8662`  
		Last Modified: Fri, 27 Aug 2021 22:40:28 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7826799e242dd8fbccb25a4beb2a945afbac958649e6769f34869c2cd73dff7b`  
		Last Modified: Fri, 27 Aug 2021 22:40:28 GMT  
		Size: 4.4 KB (4404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1efe6be15cd3275b8d95778d4be545df37733862d074ef2588cccdb6ba69f40b`  
		Last Modified: Fri, 27 Aug 2021 22:40:28 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:10-alpine3.14` - linux; arm variant v7

```console
$ docker pull postgres@sha256:290c62d14497dc0f4371cae3984e41095296f055f7687bce4ccd8ce92854a444
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.7 MB (26728367 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:62b2b2a36df444702520de30c39a6e5132ebb0aaf344f88e137de11624e6abb9`
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
# Sat, 28 Aug 2021 00:29:03 GMT
ENV PG_MAJOR=10
# Sat, 28 Aug 2021 00:29:04 GMT
ENV PG_VERSION=10.18
# Sat, 28 Aug 2021 00:29:04 GMT
ENV PG_SHA256=57477c2edc82c3f86a74747707b3babc1f301f389315ae14e819e025c0ba3801
# Sat, 28 Aug 2021 00:32:39 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Sat, 28 Aug 2021 00:32:41 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample
# Sat, 28 Aug 2021 00:32:43 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Sat, 28 Aug 2021 00:32:43 GMT
ENV PGDATA=/var/lib/postgresql/data
# Sat, 28 Aug 2021 00:32:45 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Sat, 28 Aug 2021 00:32:46 GMT
VOLUME [/var/lib/postgresql/data]
# Sat, 28 Aug 2021 00:32:46 GMT
COPY file:ad28506adc606e446eefc263bc99d4cb809e608d4f550956143bf13c82c91f85 in /usr/local/bin/ 
# Sat, 28 Aug 2021 00:32:48 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 28 Aug 2021 00:32:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 28 Aug 2021 00:32:49 GMT
STOPSIGNAL SIGINT
# Sat, 28 Aug 2021 00:32:49 GMT
EXPOSE 5432
# Sat, 28 Aug 2021 00:32:50 GMT
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
	-	`sha256:d4675de674617d4e8e7ac84d0aebbff11eb5279b88b375cb95467b4a0d8a9627`  
		Last Modified: Sat, 28 Aug 2021 00:46:00 GMT  
		Size: 24.3 MB (24283907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b43780aead6fc736103cc3b6f317aedc790e586920d1500f8b21fa9d4b8efec`  
		Last Modified: Sat, 28 Aug 2021 00:45:43 GMT  
		Size: 7.7 KB (7728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04efef4cfc81f8c225d296b9ead639777b74a2d7c01a71c6a816e25fa2cd6d9f`  
		Last Modified: Sat, 28 Aug 2021 00:45:43 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c32cadad93dae5bb47ea8da38cc948c2829cd452ed74db62ba1498b9c8828dd1`  
		Last Modified: Sat, 28 Aug 2021 00:45:43 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce42818901a4416097b0f071cab2622de9d2be9f746c66ec0a537d8e062a7bd9`  
		Last Modified: Sat, 28 Aug 2021 00:45:43 GMT  
		Size: 4.4 KB (4404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a839ad45f4c3aae6e1c5d4a75640ed21ada21308d3c7e6f993bef4faac666b7`  
		Last Modified: Sat, 28 Aug 2021 00:45:43 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:10-alpine3.14` - linux; arm64 variant v8

```console
$ docker pull postgres@sha256:a00c5f8a5f1f3b202981f9590cba06102024b853df77b6752f056143d9833c9e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.4 MB (28363470 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ebec86614ea56ed08d92e143c3e6604d0daf18fd9122b5fe4a7fd1b6ee56e9a`
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
# Sat, 28 Aug 2021 01:02:42 GMT
ENV PG_MAJOR=10
# Sat, 28 Aug 2021 01:02:43 GMT
ENV PG_VERSION=10.18
# Sat, 28 Aug 2021 01:02:43 GMT
ENV PG_SHA256=57477c2edc82c3f86a74747707b3babc1f301f389315ae14e819e025c0ba3801
# Sat, 28 Aug 2021 01:05:36 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Sat, 28 Aug 2021 01:05:37 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample
# Sat, 28 Aug 2021 01:05:37 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Sat, 28 Aug 2021 01:05:37 GMT
ENV PGDATA=/var/lib/postgresql/data
# Sat, 28 Aug 2021 01:05:38 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Sat, 28 Aug 2021 01:05:38 GMT
VOLUME [/var/lib/postgresql/data]
# Sat, 28 Aug 2021 01:05:38 GMT
COPY file:ad28506adc606e446eefc263bc99d4cb809e608d4f550956143bf13c82c91f85 in /usr/local/bin/ 
# Sat, 28 Aug 2021 01:05:39 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 28 Aug 2021 01:05:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 28 Aug 2021 01:05:39 GMT
STOPSIGNAL SIGINT
# Sat, 28 Aug 2021 01:05:40 GMT
EXPOSE 5432
# Sat, 28 Aug 2021 01:05:40 GMT
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
	-	`sha256:3c164b47491dd335b8dc4e36208af9e95cf19077b1b305bb77390c7ae549229b`  
		Last Modified: Sat, 28 Aug 2021 01:13:23 GMT  
		Size: 25.6 MB (25637600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77a37d4c1769f0045039c6df70ad426e9477688e9c361f72e1dc62442a370b47`  
		Last Modified: Sat, 28 Aug 2021 01:13:16 GMT  
		Size: 7.7 KB (7728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d75bfa882706c340e87f3dca8adc91f2d5a0ef7de0c95e138fa1cbcbe3e3a0a`  
		Last Modified: Sat, 28 Aug 2021 01:13:16 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d306665154b5281c9e05ed39deca8eff940d871a065d1c0e8dc165e0f9092bc`  
		Last Modified: Sat, 28 Aug 2021 01:13:16 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11d98f366af14998aae1ff1614e4f2e95f1e01f898c701c8e33768e55750ace8`  
		Last Modified: Sat, 28 Aug 2021 01:13:17 GMT  
		Size: 4.4 KB (4403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36672cce533ab2dbcce8312d96a18b6ba63b31560efc989a57ed02eaa47cc5b7`  
		Last Modified: Sat, 28 Aug 2021 01:13:16 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:10-alpine3.14` - linux; 386

```console
$ docker pull postgres@sha256:72f599385c93aa4eab6b4d111f85974b0ca9e1b1a8d7efbdb088f158fa73ebaf
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.6 MB (29561033 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:244c0f36ac3e4ba42cf41df31e1b4400278fccb605b174b5c139ee6c4c08c3d0`
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
# Fri, 27 Aug 2021 22:28:56 GMT
ENV PG_MAJOR=10
# Fri, 27 Aug 2021 22:28:56 GMT
ENV PG_VERSION=10.18
# Fri, 27 Aug 2021 22:28:57 GMT
ENV PG_SHA256=57477c2edc82c3f86a74747707b3babc1f301f389315ae14e819e025c0ba3801
# Fri, 27 Aug 2021 22:34:53 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Fri, 27 Aug 2021 22:34:54 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample
# Fri, 27 Aug 2021 22:34:55 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 27 Aug 2021 22:34:55 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 27 Aug 2021 22:34:56 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 27 Aug 2021 22:34:56 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 27 Aug 2021 22:34:56 GMT
COPY file:ad28506adc606e446eefc263bc99d4cb809e608d4f550956143bf13c82c91f85 in /usr/local/bin/ 
# Fri, 27 Aug 2021 22:34:57 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 27 Aug 2021 22:34:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 Aug 2021 22:34:58 GMT
STOPSIGNAL SIGINT
# Fri, 27 Aug 2021 22:34:58 GMT
EXPOSE 5432
# Fri, 27 Aug 2021 22:34:58 GMT
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
	-	`sha256:3f68196b133ba0e7fe6c0c32f447e5cbce26274e48b8438830cfd0be7edfa446`  
		Last Modified: Fri, 27 Aug 2021 22:44:05 GMT  
		Size: 26.7 MB (26724130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2d6f55f0182605724e6a3f7d3f3c21bc03bb8f6c38512e17f44d9733c1154d3`  
		Last Modified: Fri, 27 Aug 2021 22:43:57 GMT  
		Size: 7.7 KB (7730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c11246dd5da6bb6cac6885e20694a0155132868b4713642a69577d846e681e64`  
		Last Modified: Fri, 27 Aug 2021 22:43:58 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dccd27bcfbf81628ea3bcf3999ba6e0bec52039881bf917c6c5f03c8e9c5dc61`  
		Last Modified: Fri, 27 Aug 2021 22:43:57 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06796b004172b19be0b344390c925f638f877d64bf3053178361a07f3681a3e5`  
		Last Modified: Fri, 27 Aug 2021 22:43:57 GMT  
		Size: 4.4 KB (4405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:601d24b3fb6fc5044bd038e45350874e0dd5e85a0565d21ddbfac5bf1fd14c62`  
		Last Modified: Fri, 27 Aug 2021 22:43:57 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:10-alpine3.14` - linux; ppc64le

```console
$ docker pull postgres@sha256:814fda38341a820c20838c17820afc99ec7739fe197d669dc1e69d51653c70ef
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.0 MB (29954520 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2ae2c0d1b06dc7d43e173579f0dccbe4c6caf404094158329378c6095f31c969`
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
# Fri, 27 Aug 2021 22:06:41 GMT
ENV PG_MAJOR=10
# Fri, 27 Aug 2021 22:06:48 GMT
ENV PG_VERSION=10.18
# Fri, 27 Aug 2021 22:06:50 GMT
ENV PG_SHA256=57477c2edc82c3f86a74747707b3babc1f301f389315ae14e819e025c0ba3801
# Fri, 27 Aug 2021 22:09:41 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Fri, 27 Aug 2021 22:10:02 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample
# Fri, 27 Aug 2021 22:10:12 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 27 Aug 2021 22:10:14 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 27 Aug 2021 22:10:24 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 27 Aug 2021 22:10:27 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 27 Aug 2021 22:10:29 GMT
COPY file:ad28506adc606e446eefc263bc99d4cb809e608d4f550956143bf13c82c91f85 in /usr/local/bin/ 
# Fri, 27 Aug 2021 22:10:35 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 27 Aug 2021 22:10:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 Aug 2021 22:10:47 GMT
STOPSIGNAL SIGINT
# Fri, 27 Aug 2021 22:10:50 GMT
EXPOSE 5432
# Fri, 27 Aug 2021 22:10:53 GMT
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
	-	`sha256:03b84332d3d34d7f08aa919d5379efa4dbd647b4f835b7dfa70233348860906b`  
		Last Modified: Fri, 27 Aug 2021 22:20:21 GMT  
		Size: 27.1 MB (27128193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e614185e68541f9e49724707d654203e7145f41401c75f558c20ef5ab312cd0`  
		Last Modified: Fri, 27 Aug 2021 22:20:13 GMT  
		Size: 7.7 KB (7727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a569484b87b578d2f296bc37da7e959106c330d7404d87d8a3fe2b00ceb257e`  
		Last Modified: Fri, 27 Aug 2021 22:20:13 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67a6bfa76ef7461f578511ef5f5be546d3edd650ec161577f5a41c19f1aae43a`  
		Last Modified: Fri, 27 Aug 2021 22:20:13 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a11a33a1048c61baee3ebe43f20b134527940665f04dbe94f41953f1da36026e`  
		Last Modified: Fri, 27 Aug 2021 22:20:13 GMT  
		Size: 4.4 KB (4404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c44dccb6db59831f8e770e635c4e2f8d98881d7d6a84e5fb7fc15fd0508e6816`  
		Last Modified: Fri, 27 Aug 2021 22:20:13 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:10-alpine3.14` - linux; s390x

```console
$ docker pull postgres@sha256:409a400de60d874296a0345be226ccdce64f89b5de3225fa2c4e951d2d91079d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.5 MB (28504593 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:edf2c292fc302c286d18ae57dbc3de6661a8c19bd01582780f070eac72f29bb5`
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
# Sat, 28 Aug 2021 01:08:36 GMT
ENV PG_MAJOR=10
# Sat, 28 Aug 2021 01:08:36 GMT
ENV PG_VERSION=10.18
# Sat, 28 Aug 2021 01:08:36 GMT
ENV PG_SHA256=57477c2edc82c3f86a74747707b3babc1f301f389315ae14e819e025c0ba3801
# Sat, 28 Aug 2021 01:12:39 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Sat, 28 Aug 2021 01:12:44 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample
# Sat, 28 Aug 2021 01:12:46 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Sat, 28 Aug 2021 01:12:46 GMT
ENV PGDATA=/var/lib/postgresql/data
# Sat, 28 Aug 2021 01:12:48 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Sat, 28 Aug 2021 01:12:48 GMT
VOLUME [/var/lib/postgresql/data]
# Sat, 28 Aug 2021 01:12:49 GMT
COPY file:ad28506adc606e446eefc263bc99d4cb809e608d4f550956143bf13c82c91f85 in /usr/local/bin/ 
# Sat, 28 Aug 2021 01:12:51 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 28 Aug 2021 01:12:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 28 Aug 2021 01:12:52 GMT
STOPSIGNAL SIGINT
# Sat, 28 Aug 2021 01:12:53 GMT
EXPOSE 5432
# Sat, 28 Aug 2021 01:12:53 GMT
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
	-	`sha256:c27947a6719db6f12c7d9a53034a6368f1e166b03ba37720a5c7d59cc92b22cd`  
		Last Modified: Sat, 28 Aug 2021 01:21:31 GMT  
		Size: 25.9 MB (25887083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d879e9d994ed31a4f6e94db8ded8e0b61926f0421f0b1157b2cac09445e874c8`  
		Last Modified: Sat, 28 Aug 2021 01:21:25 GMT  
		Size: 7.7 KB (7732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ca39cb772d32ed541304b257500962e5193419e201f7b99f4e79ac84ab531fc`  
		Last Modified: Sat, 28 Aug 2021 01:21:25 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47d44267ba0ff9348e20a3469b96368d3129a3059a9ace567b4bac3cd3264c9d`  
		Last Modified: Sat, 28 Aug 2021 01:21:25 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fa95fb9e50d25257f016b40ce626713d63d86bf3d0fa92c48af22e9e9390e88`  
		Last Modified: Sat, 28 Aug 2021 01:21:25 GMT  
		Size: 4.4 KB (4405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76d57cfb4311bab69de5329850e207f390ad0466b18ddd85ba73b9dea9e93535`  
		Last Modified: Sat, 28 Aug 2021 01:21:26 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
