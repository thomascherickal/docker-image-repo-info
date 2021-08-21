## `postgres:14beta3-alpine3.14`

```console
$ docker pull postgres@sha256:e6a89e27cd26103d516ac4863fa2dd5f828972170f849af2f948a19fee21dfc9
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
$ docker pull postgres@sha256:b523df7927dcd52758e10a73bc0c1d4d54dce58570836f9b92d4a122f5211303
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.3 MB (77319348 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:99403d705ab07a5b48eaada50150fc6fadf7faae892ffe1156cdafebbcf0cc90`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Fri, 06 Aug 2021 17:19:45 GMT
ADD file:34eb5c40aa00028921a224d1764ae1b1f3ef710d191e4dfc7df55e0594aa7217 in / 
# Fri, 06 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Fri, 06 Aug 2021 20:09:36 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Fri, 06 Aug 2021 20:09:36 GMT
ENV LANG=en_US.utf8
# Fri, 06 Aug 2021 20:09:37 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 06 Aug 2021 20:09:37 GMT
ENV PG_MAJOR=14
# Thu, 12 Aug 2021 20:35:51 GMT
ENV PG_VERSION=14beta3
# Thu, 12 Aug 2021 20:35:51 GMT
ENV PG_SHA256=2ea265980193db70106576201a2fee5b2d72bf9890d3911ddd374d4830624bfa
# Thu, 12 Aug 2021 20:40:59 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm11-dev clang g++ 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 		lz4-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 		--with-lz4 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Thu, 12 Aug 2021 20:41:01 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample
# Thu, 12 Aug 2021 20:41:02 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 12 Aug 2021 20:41:02 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 12 Aug 2021 20:41:04 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 12 Aug 2021 20:41:04 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 12 Aug 2021 20:41:05 GMT
COPY file:ad28506adc606e446eefc263bc99d4cb809e608d4f550956143bf13c82c91f85 in /usr/local/bin/ 
# Thu, 12 Aug 2021 20:41:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 12 Aug 2021 20:41:05 GMT
STOPSIGNAL SIGINT
# Thu, 12 Aug 2021 20:41:05 GMT
EXPOSE 5432
# Thu, 12 Aug 2021 20:41:06 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:29291e31a76a7e560b9b7ad3cada56e8c18d50a96cca8a2573e4f4689d7aca77`  
		Last Modified: Thu, 05 Aug 2021 15:56:25 GMT  
		Size: 2.8 MB (2813006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7f8a1ea71cb44639c871a69f095baa1737555205a3ea7ce92b116c1462ffc37`  
		Last Modified: Fri, 06 Aug 2021 20:49:45 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64d8912b293dcd54c830c025ee7d3c1e3774037bc917800fc4db4a04959855ca`  
		Last Modified: Fri, 06 Aug 2021 20:49:45 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c35e60d05ec4dd04b41bef185fb97cc8d212d6aa77eb0fee6c6d66a0a3cc264a`  
		Last Modified: Thu, 12 Aug 2021 21:20:49 GMT  
		Size: 74.5 MB (74490946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0ee631531d661dd21ab686a2f9713484a37e52d867471bd4b33aee5bdc55f68`  
		Last Modified: Thu, 12 Aug 2021 21:20:35 GMT  
		Size: 9.2 KB (9205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e08351986c4d2a102c349078ffdb4e6e4a465c50d85b052607572d20263ed017`  
		Last Modified: Thu, 12 Aug 2021 21:20:35 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a51da03b0c6c6dc5fabf8f622d4a8d44657032f76952c903c29ad1a4cea85a7f`  
		Last Modified: Thu, 12 Aug 2021 21:20:35 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22628c5c63625961f3c23d9884770f0b9686f2db5ab210ccf48f15345981bc91`  
		Last Modified: Thu, 12 Aug 2021 21:20:35 GMT  
		Size: 4.4 KB (4404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:14beta3-alpine3.14` - linux; arm variant v6

```console
$ docker pull postgres@sha256:d0494340d04ccf4a040fc446bb7bc03e0834aa50df104c1a2081d23d22690cea
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.8 MB (75832529 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e5436e40f9b5dfd8d613b0a7f20f69b4cdf4354cc21fb40ad1d679091b0b9cee`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Fri, 06 Aug 2021 17:49:32 GMT
ADD file:7f2c7deda009eabdcbbdccb11e854043d32c498e64e7e1ca02165d7bb4261d39 in / 
# Fri, 06 Aug 2021 17:49:32 GMT
CMD ["/bin/sh"]
# Fri, 06 Aug 2021 21:34:10 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Fri, 06 Aug 2021 21:34:11 GMT
ENV LANG=en_US.utf8
# Fri, 06 Aug 2021 21:34:12 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 06 Aug 2021 21:34:13 GMT
ENV PG_MAJOR=14
# Thu, 12 Aug 2021 23:29:05 GMT
ENV PG_VERSION=14beta3
# Thu, 12 Aug 2021 23:29:06 GMT
ENV PG_SHA256=2ea265980193db70106576201a2fee5b2d72bf9890d3911ddd374d4830624bfa
# Thu, 12 Aug 2021 23:34:23 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm11-dev clang g++ 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 		lz4-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 		--with-lz4 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Thu, 12 Aug 2021 23:34:25 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample
# Thu, 12 Aug 2021 23:34:26 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 12 Aug 2021 23:34:27 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 12 Aug 2021 23:34:28 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 12 Aug 2021 23:34:29 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 12 Aug 2021 23:34:29 GMT
COPY file:ad28506adc606e446eefc263bc99d4cb809e608d4f550956143bf13c82c91f85 in /usr/local/bin/ 
# Thu, 12 Aug 2021 23:34:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 12 Aug 2021 23:34:30 GMT
STOPSIGNAL SIGINT
# Thu, 12 Aug 2021 23:34:31 GMT
EXPOSE 5432
# Thu, 12 Aug 2021 23:34:31 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:f465bb3e9fcd0c42f936ecc566c6e40353c00f3089b2b2c2ea1663c30f89d3ab`  
		Last Modified: Fri, 06 Aug 2021 17:51:00 GMT  
		Size: 2.6 MB (2626350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9894594f46e7a2d9314f2f96a83a8a4d069c1c3d3bd1f20f7378ea4a36eb000`  
		Last Modified: Fri, 06 Aug 2021 22:05:03 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1d885209ac2857981e19ce7ccfb1852b335ed57fd0d8020badbc76323c3a5c3`  
		Last Modified: Fri, 06 Aug 2021 22:05:04 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:050e53bb72b69e5678796a8707230a5abe9ede9e1190f3a22bb0f59d4365e567`  
		Last Modified: Fri, 13 Aug 2021 00:04:50 GMT  
		Size: 73.2 MB (73190778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dbcbfc979ea62874ba8ca05ad234468313c45314b2738c8c889cab2f5466f2b`  
		Last Modified: Fri, 13 Aug 2021 00:04:11 GMT  
		Size: 9.2 KB (9207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e345c771eff08c9351814a256d6b95dd82cf78f871bd7a5fe822940a3471f23`  
		Last Modified: Fri, 13 Aug 2021 00:04:11 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:462a5604679f15ed234cc2852988bfcb08d427784f43b8285a3fa2b7f420a962`  
		Last Modified: Fri, 13 Aug 2021 00:04:11 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64340cb2f7819162f58285597ea724c2edf57bf591bbb093adbdbb957306eba5`  
		Last Modified: Fri, 13 Aug 2021 00:04:11 GMT  
		Size: 4.4 KB (4406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:14beta3-alpine3.14` - linux; arm variant v7

```console
$ docker pull postgres@sha256:3ea56c87588a946937bff38c62844241c2b0dde2d4bb2be8e2b7a56ff79b8ee1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.5 MB (71513183 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:30204bf17347982625b5f1d9c7d6b1e0fd9b2ca9dab364c4d356e48b8dd0022f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Fri, 06 Aug 2021 17:57:32 GMT
ADD file:3a35ff3ac0d80289d419a4d6d8319610c38e1936d296addafb9aaf506946230f in / 
# Fri, 06 Aug 2021 17:57:32 GMT
CMD ["/bin/sh"]
# Sat, 07 Aug 2021 01:08:14 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Sat, 07 Aug 2021 01:08:14 GMT
ENV LANG=en_US.utf8
# Sat, 07 Aug 2021 01:08:16 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 07 Aug 2021 01:08:16 GMT
ENV PG_MAJOR=14
# Fri, 13 Aug 2021 01:15:55 GMT
ENV PG_VERSION=14beta3
# Fri, 13 Aug 2021 01:15:56 GMT
ENV PG_SHA256=2ea265980193db70106576201a2fee5b2d72bf9890d3911ddd374d4830624bfa
# Fri, 13 Aug 2021 01:20:40 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm11-dev clang g++ 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 		lz4-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 		--with-lz4 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Fri, 13 Aug 2021 01:20:42 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample
# Fri, 13 Aug 2021 01:20:44 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 13 Aug 2021 01:20:44 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 13 Aug 2021 01:20:46 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 13 Aug 2021 01:20:46 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 13 Aug 2021 01:20:47 GMT
COPY file:ad28506adc606e446eefc263bc99d4cb809e608d4f550956143bf13c82c91f85 in /usr/local/bin/ 
# Fri, 13 Aug 2021 01:20:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 13 Aug 2021 01:20:48 GMT
STOPSIGNAL SIGINT
# Fri, 13 Aug 2021 01:20:48 GMT
EXPOSE 5432
# Fri, 13 Aug 2021 01:20:49 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:4ee0caa23b369b04827640a4be298bf4ff7bacd030c77e915f5d7fb8f987594a`  
		Last Modified: Fri, 06 Aug 2021 17:58:57 GMT  
		Size: 2.4 MB (2429359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cef58414db85950184ccfaaf047c5260d938c1ed132eb394e7dcc08e421dc3e`  
		Last Modified: Sat, 07 Aug 2021 01:40:44 GMT  
		Size: 1.3 KB (1283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d99a5114dc9bd4eaae87d214120cfd9ac233204ed1fdf161fad160f52db1439a`  
		Last Modified: Sat, 07 Aug 2021 01:40:44 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12270d8a7a48598590b22e79361d15e7813beeceb9614c25cab4d540c0fb8cd9`  
		Last Modified: Fri, 13 Aug 2021 05:12:06 GMT  
		Size: 69.1 MB (69068425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42130c53e43e248c8311cde1bcc0ac747186519ead60b0fb58cb11aa69492e70`  
		Last Modified: Fri, 13 Aug 2021 05:11:29 GMT  
		Size: 9.2 KB (9204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8adfd8a425675c6c6e6595ce13f706c913765dd50a90d4cbce1d43973dae3b22`  
		Last Modified: Fri, 13 Aug 2021 05:11:29 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29b9f03fdb4d3acbaf72bd359373fb3f62a17fcca65ae781a8734662aeecea7d`  
		Last Modified: Fri, 13 Aug 2021 05:11:29 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a1a2b8656bb103ddb8f266292494fe78b5589c18b8e66afd31d4bc42ce8c672`  
		Last Modified: Fri, 13 Aug 2021 05:11:29 GMT  
		Size: 4.4 KB (4407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:14beta3-alpine3.14` - linux; arm64 variant v8

```console
$ docker pull postgres@sha256:e1269d740b41aa152b89163d729a14f049c80b3cd062717a2dc03a6f66f59060
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.2 MB (76214664 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb00e7f8e637fc520f9b8a6caa7a2e333ebb99b9446e41add6894b884c16a8dd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Fri, 06 Aug 2021 17:39:26 GMT
ADD file:1a8fd1066485e1261462e689c1a072f010c1d3be904b73ef2b84128fac652951 in / 
# Fri, 06 Aug 2021 17:39:27 GMT
CMD ["/bin/sh"]
# Sat, 07 Aug 2021 00:19:26 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Sat, 07 Aug 2021 00:19:26 GMT
ENV LANG=en_US.utf8
# Sat, 07 Aug 2021 00:19:27 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 07 Aug 2021 00:19:27 GMT
ENV PG_MAJOR=14
# Fri, 13 Aug 2021 03:07:44 GMT
ENV PG_VERSION=14beta3
# Fri, 13 Aug 2021 03:07:44 GMT
ENV PG_SHA256=2ea265980193db70106576201a2fee5b2d72bf9890d3911ddd374d4830624bfa
# Fri, 13 Aug 2021 03:12:36 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm11-dev clang g++ 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 		lz4-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 		--with-lz4 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Fri, 13 Aug 2021 03:12:37 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample
# Fri, 13 Aug 2021 03:12:38 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 13 Aug 2021 03:12:38 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 13 Aug 2021 03:12:38 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 13 Aug 2021 03:12:39 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 13 Aug 2021 03:12:39 GMT
COPY file:ad28506adc606e446eefc263bc99d4cb809e608d4f550956143bf13c82c91f85 in /usr/local/bin/ 
# Fri, 13 Aug 2021 03:12:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 13 Aug 2021 03:12:39 GMT
STOPSIGNAL SIGINT
# Fri, 13 Aug 2021 03:12:39 GMT
EXPOSE 5432
# Fri, 13 Aug 2021 03:12:39 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:fd3acdcea5682abced546ec19fb6ebee725c5184e5d91614c469c0a79e67f2d0`  
		Last Modified: Fri, 06 Aug 2021 17:40:12 GMT  
		Size: 2.7 MB (2710613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba97523f916fd8acc76ccd9aaafa6ef7f9adf2d2ae821e4b8c2a4a3ce78db610`  
		Last Modified: Sat, 07 Aug 2021 00:46:45 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef888e85bfc8313834349d662d946b19b67e6a6fb705c484d91b83be6a9b76d8`  
		Last Modified: Sat, 07 Aug 2021 00:46:45 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17ee98358deae1f3e38be94414c1b48fc44e9132e6b7b5dab0adb1c75b40f300`  
		Last Modified: Fri, 13 Aug 2021 04:06:30 GMT  
		Size: 73.5 MB (73488651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7faf3afd79ec270a7ab39dee90bbabdb232b519aea0f89f52f4e26abb9d440f2`  
		Last Modified: Fri, 13 Aug 2021 04:06:20 GMT  
		Size: 9.2 KB (9206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42c0d85fac987b3f3df250a36d4cd399fc18f8f537c5ff1323f97b25204c8013`  
		Last Modified: Fri, 13 Aug 2021 04:06:20 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:639f8df6cbcd9fd4d253fe39a0d65ddbf586ffbe01b7a9efb7d42e4f0632f96a`  
		Last Modified: Fri, 13 Aug 2021 04:06:20 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0586522a34bc9d5958fd93a8270986969cddbc4e70aa9d16bd3333a01f846cf8`  
		Last Modified: Fri, 13 Aug 2021 04:06:20 GMT  
		Size: 4.4 KB (4404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:14beta3-alpine3.14` - linux; 386

```console
$ docker pull postgres@sha256:2727a8906b09aabf24944cbee002965c107eca62e1abe6644adc9fda8a6fc5b6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **82.1 MB (82096747 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e04601002d41a4d9e41d8808ce623cb4a8ba9d35ef97fdc58e858a44098577d3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Fri, 06 Aug 2021 17:38:26 GMT
ADD file:bafaec4a54d6cef99b5f3660d074a3d2251e4d4bd09df9ea65f33e9bffb7d88d in / 
# Fri, 06 Aug 2021 17:38:26 GMT
CMD ["/bin/sh"]
# Fri, 06 Aug 2021 21:44:56 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Fri, 06 Aug 2021 21:44:57 GMT
ENV LANG=en_US.utf8
# Fri, 06 Aug 2021 21:44:57 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 06 Aug 2021 21:44:58 GMT
ENV PG_MAJOR=14
# Thu, 12 Aug 2021 20:40:17 GMT
ENV PG_VERSION=14beta3
# Thu, 12 Aug 2021 20:40:17 GMT
ENV PG_SHA256=2ea265980193db70106576201a2fee5b2d72bf9890d3911ddd374d4830624bfa
# Thu, 12 Aug 2021 20:48:38 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm11-dev clang g++ 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 		lz4-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 		--with-lz4 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Thu, 12 Aug 2021 20:48:40 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample
# Thu, 12 Aug 2021 20:48:41 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 12 Aug 2021 20:48:41 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 12 Aug 2021 20:48:42 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 12 Aug 2021 20:48:42 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 12 Aug 2021 20:48:43 GMT
COPY file:ad28506adc606e446eefc263bc99d4cb809e608d4f550956143bf13c82c91f85 in /usr/local/bin/ 
# Thu, 12 Aug 2021 20:48:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 12 Aug 2021 20:48:43 GMT
STOPSIGNAL SIGINT
# Thu, 12 Aug 2021 20:48:43 GMT
EXPOSE 5432
# Thu, 12 Aug 2021 20:48:44 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:935703e1179e32e201e4a36d5664d58299dc8e7bcac197b70c295c0a59216db1`  
		Last Modified: Fri, 06 Aug 2021 17:39:15 GMT  
		Size: 2.8 MB (2821910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7c05efe598158ae45c83841ac5ec7934faa5d733f5fcfe85b0261cf9c987262`  
		Last Modified: Fri, 06 Aug 2021 22:25:16 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bf37feeefc8b50739451550bcd2f9738e9369d3eea1e7c8fe5fbd0ee22ba530`  
		Last Modified: Fri, 06 Aug 2021 22:25:15 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb228de3a1fabe90c8499036d3b1d70519f959d917eb325e3f3b0a6dd0e660b1`  
		Last Modified: Thu, 12 Aug 2021 21:30:14 GMT  
		Size: 79.3 MB (79259440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bffbe567b2e640efbefd1033c3861f2c54618558682de59c82e0c68f8bb76221`  
		Last Modified: Thu, 12 Aug 2021 21:29:59 GMT  
		Size: 9.2 KB (9202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdbd5ce413000d0a173e2698e01f11c3cc255d802ea8c1b1a254b4d3650429b0`  
		Last Modified: Thu, 12 Aug 2021 21:29:59 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9bcb26cd53b8c2df6a849dc71f90b964d160b453dabf47d6beeccc7bb314190`  
		Last Modified: Thu, 12 Aug 2021 21:29:59 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17167a2ad0acfe845d3c2264a346d59c1bbe4f6be80501c2a3497b3c5903a812`  
		Last Modified: Thu, 12 Aug 2021 21:29:59 GMT  
		Size: 4.4 KB (4406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:14beta3-alpine3.14` - linux; ppc64le

```console
$ docker pull postgres@sha256:08cfb5ee7bca339ba28a6b74cc616a7fdb0295d95d573d8df16e7acf372ccd15
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **82.3 MB (82346866 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92347c2b33212b9a01538d5d8f4676867e97c6a9ecf2a98835f9876da60dcbf5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Fri, 06 Aug 2021 18:28:28 GMT
ADD file:40f3b617d7ff269d92f0ffcf8aad561b5f2c0626ef519a7f584f1ba0182b3188 in / 
# Fri, 06 Aug 2021 18:28:35 GMT
CMD ["/bin/sh"]
# Sat, 07 Aug 2021 00:39:16 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Sat, 07 Aug 2021 00:39:27 GMT
ENV LANG=en_US.utf8
# Sat, 07 Aug 2021 00:39:50 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 07 Aug 2021 00:39:54 GMT
ENV PG_MAJOR=14
# Fri, 13 Aug 2021 00:09:24 GMT
ENV PG_VERSION=14beta3
# Fri, 13 Aug 2021 00:09:30 GMT
ENV PG_SHA256=2ea265980193db70106576201a2fee5b2d72bf9890d3911ddd374d4830624bfa
# Fri, 13 Aug 2021 00:13:43 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm11-dev clang g++ 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 		lz4-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 		--with-lz4 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Fri, 13 Aug 2021 00:14:00 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample
# Fri, 13 Aug 2021 00:14:07 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 13 Aug 2021 00:14:11 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 13 Aug 2021 00:14:18 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 13 Aug 2021 00:14:22 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 13 Aug 2021 00:14:24 GMT
COPY file:ad28506adc606e446eefc263bc99d4cb809e608d4f550956143bf13c82c91f85 in /usr/local/bin/ 
# Fri, 13 Aug 2021 00:14:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 13 Aug 2021 00:14:30 GMT
STOPSIGNAL SIGINT
# Fri, 13 Aug 2021 00:14:36 GMT
EXPOSE 5432
# Fri, 13 Aug 2021 00:14:41 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:0ff902055236f70c4694c806877243e1dd52c513825a2a3ecc7eba8f5202acc8`  
		Last Modified: Fri, 06 Aug 2021 18:29:33 GMT  
		Size: 2.8 MB (2811152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0171836c388de004e05625d2d3ef11aca08f84a644c0e3556f407e3faa45b35b`  
		Last Modified: Sat, 07 Aug 2021 01:13:13 GMT  
		Size: 1.3 KB (1283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f2c96cc7a2637602e04a8006bc17a2ef71621e55b1d19adb54611e9ae383651`  
		Last Modified: Sat, 07 Aug 2021 01:13:13 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7db2a108a2f3d39e35ccc2921572e58e6cb39c4d75616da4ca81e4f4226975c0`  
		Last Modified: Fri, 13 Aug 2021 01:02:33 GMT  
		Size: 79.5 MB (79520319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb29043e9ea225d32f81bb2459d4f2a8f5b5822dbfb67be39327c147c9cd8ddd`  
		Last Modified: Fri, 13 Aug 2021 01:02:20 GMT  
		Size: 9.2 KB (9204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cff0389e9b8ca2cfb79c224a86a025947617504a5ce8c8e64c46d0f1c173fb6`  
		Last Modified: Fri, 13 Aug 2021 01:02:20 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82399d6635b1d83c90784e14f5865e7adf73efe4443e949f40ccdbee044a472b`  
		Last Modified: Fri, 13 Aug 2021 01:02:20 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4f8e7a6626654ad059ec96a65b3f008272712e58862339c2090f890bd810d0e`  
		Last Modified: Fri, 13 Aug 2021 01:02:20 GMT  
		Size: 4.4 KB (4404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:14beta3-alpine3.14` - linux; s390x

```console
$ docker pull postgres@sha256:b884eafbdd985e6de7b86204af7be4e38000ad7df182346e1ce7cc561af73f56
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **78.6 MB (78601882 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89c299d5024e30932cadb95e5f2729aca8937916ab11bb491ca101698b514734`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Fri, 06 Aug 2021 17:41:30 GMT
ADD file:bdf19d63e9f8600d2fbe02435279b8df06fbcb5105e6b8eea778d8ef928e219a in / 
# Fri, 06 Aug 2021 17:41:31 GMT
CMD ["/bin/sh"]
# Fri, 06 Aug 2021 19:47:03 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Fri, 06 Aug 2021 19:47:03 GMT
ENV LANG=en_US.utf8
# Fri, 06 Aug 2021 19:47:05 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 06 Aug 2021 19:47:05 GMT
ENV PG_MAJOR=14
# Fri, 13 Aug 2021 00:40:45 GMT
ENV PG_VERSION=14beta3
# Fri, 13 Aug 2021 00:40:46 GMT
ENV PG_SHA256=2ea265980193db70106576201a2fee5b2d72bf9890d3911ddd374d4830624bfa
# Sat, 21 Aug 2021 03:17:50 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm11-dev clang g++ 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 		lz4-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 		--with-lz4 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Sat, 21 Aug 2021 03:17:56 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample
# Sat, 21 Aug 2021 03:17:56 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Sat, 21 Aug 2021 03:17:57 GMT
ENV PGDATA=/var/lib/postgresql/data
# Sat, 21 Aug 2021 03:17:58 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Sat, 21 Aug 2021 03:17:58 GMT
VOLUME [/var/lib/postgresql/data]
# Sat, 21 Aug 2021 03:17:58 GMT
COPY file:ad28506adc606e446eefc263bc99d4cb809e608d4f550956143bf13c82c91f85 in /usr/local/bin/ 
# Sat, 21 Aug 2021 03:17:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 21 Aug 2021 03:17:59 GMT
STOPSIGNAL SIGINT
# Sat, 21 Aug 2021 03:17:59 GMT
EXPOSE 5432
# Sat, 21 Aug 2021 03:17:59 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:625f57562315453466f73bc9d8c96e678f8d4ea436b462d06c60fb217c6b3d38`  
		Last Modified: Fri, 06 Aug 2021 17:42:42 GMT  
		Size: 2.6 MB (2602036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6feee749ba385a97a7ab1fd9cb3de25413708670d74258e8b54ae7b4f1b8ffbe`  
		Last Modified: Sat, 21 Aug 2021 03:40:07 GMT  
		Size: 1.3 KB (1283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba322904a726e4ccf5081d028fd5bc093f22c97b09b32c5a9e894ef2f66dbbc8`  
		Last Modified: Sat, 21 Aug 2021 03:40:07 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba3d1661cb3c4259caf276e05dcb846c9be8351dbcdeb37253c1bf817bcd1244`  
		Last Modified: Sat, 21 Aug 2021 03:40:15 GMT  
		Size: 76.0 MB (75984448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2e4ff312c8dd3a8b4d4c401d7b98717427c99dba998b5f9230bb6e0d2c98a38`  
		Last Modified: Sat, 21 Aug 2021 03:40:05 GMT  
		Size: 9.2 KB (9204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51c524b7ae16efb835540c652806d86f573b993a639612c61ee736510ec8c02e`  
		Last Modified: Sat, 21 Aug 2021 03:40:06 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eaf0bc137bd3e9276b819d02a35d5db4b9a127fddd57d808c3ad88d5f6618fbf`  
		Last Modified: Sat, 21 Aug 2021 03:40:05 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f077a642044bb7376b869fa95aadb732f550351c9a0966999a37bf669c7f59c`  
		Last Modified: Sat, 21 Aug 2021 03:40:05 GMT  
		Size: 4.4 KB (4408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
