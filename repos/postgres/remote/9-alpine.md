## `postgres:9-alpine`

```console
$ docker pull postgres@sha256:183f938cd1d47a7c8cc2b393e75605e44ae423f8fabcdc22436a3b99d5e0feac
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

### `postgres:9-alpine` - linux; amd64

```console
$ docker pull postgres@sha256:0c52ce5e2326abce52fbe7f3035552596846ca5ee7d029fd66a2ab516526d4b1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.6 MB (14590381 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:41217e3e2b3778e266219ab82e41e4de110d36ab600a9829028421b33f085eb8`
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
# Wed, 16 Jun 2021 22:35:42 GMT
ENV PG_MAJOR=9.6
# Wed, 16 Jun 2021 22:35:43 GMT
ENV PG_VERSION=9.6.22
# Wed, 16 Jun 2021 22:35:43 GMT
ENV PG_SHA256=3d32cd101025a0556813397c69feff3df3d63736adb8adeaf365c522f39f2930
# Fri, 25 Jun 2021 19:35:32 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Fri, 25 Jun 2021 19:35:33 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample
# Fri, 25 Jun 2021 19:35:34 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 25 Jun 2021 19:35:35 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 25 Jun 2021 19:35:36 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 25 Jun 2021 19:35:36 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 25 Jun 2021 19:35:36 GMT
COPY file:e881105b30bb0f1591c0f7f6dfe19bf5351d029d5babae597d2698e04a16ec8b in /usr/local/bin/ 
# Fri, 25 Jun 2021 19:35:37 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 25 Jun 2021 19:35:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Jun 2021 19:35:38 GMT
STOPSIGNAL SIGINT
# Fri, 25 Jun 2021 19:35:38 GMT
EXPOSE 5432
# Fri, 25 Jun 2021 19:35:38 GMT
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
	-	`sha256:434eb517987e6f3f78ed43bcc6b4473cd18417e65d18ca058ab143ef5a3e8112`  
		Last Modified: Fri, 25 Jun 2021 19:38:18 GMT  
		Size: 11.8 MB (11765048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c33bbcceee15c05951167a156b17fb5208c8c65520f185affdef0cd4fe7e280b`  
		Last Modified: Fri, 25 Jun 2021 19:38:13 GMT  
		Size: 7.5 KB (7536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16be0b17768e8fd4485404326ddb49e207e3200aad4e8bf44066fe2447490751`  
		Last Modified: Fri, 25 Jun 2021 19:38:13 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39b7a1255b684ce9fac6acb88e621c20acfc67ba347f136b34bc1d89cfd2aaf9`  
		Last Modified: Fri, 25 Jun 2021 19:38:13 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a6b676d6166316dd02b46def92c67f7138c3662cc5cb3d7b198adac9615f539`  
		Last Modified: Fri, 25 Jun 2021 19:38:13 GMT  
		Size: 4.4 KB (4411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e623573b72e3357aa4fdfa9396c09b2d9870a22d9b9e715667fb62fb984316c`  
		Last Modified: Fri, 25 Jun 2021 19:38:13 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:9-alpine` - linux; arm variant v6

```console
$ docker pull postgres@sha256:9959da32fb0008b46c4ab48582c1ab1e0e2d98e8f2abf4c57f2def7e36fb1e3e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.0 MB (14000745 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:869ef5c38739206c54f5ce782c1a95c9b0451b1aa225cfd10b6ea6fa3056a378`
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
# Tue, 22 Jun 2021 00:17:07 GMT
ENV PG_MAJOR=9.6
# Tue, 22 Jun 2021 00:17:07 GMT
ENV PG_VERSION=9.6.22
# Tue, 22 Jun 2021 00:17:08 GMT
ENV PG_SHA256=3d32cd101025a0556813397c69feff3df3d63736adb8adeaf365c522f39f2930
# Fri, 25 Jun 2021 19:32:23 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Fri, 25 Jun 2021 19:32:26 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample
# Fri, 25 Jun 2021 19:32:27 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 25 Jun 2021 19:32:28 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 25 Jun 2021 19:32:29 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 25 Jun 2021 19:32:30 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 25 Jun 2021 19:32:30 GMT
COPY file:e881105b30bb0f1591c0f7f6dfe19bf5351d029d5babae597d2698e04a16ec8b in /usr/local/bin/ 
# Fri, 25 Jun 2021 19:32:32 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 25 Jun 2021 19:32:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Jun 2021 19:32:33 GMT
STOPSIGNAL SIGINT
# Fri, 25 Jun 2021 19:32:33 GMT
EXPOSE 5432
# Fri, 25 Jun 2021 19:32:34 GMT
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
	-	`sha256:4cc28a58dfafbb6105e891d50d1097b3eb49b921d7035751dfdcb928f68473d7`  
		Last Modified: Fri, 25 Jun 2021 19:37:05 GMT  
		Size: 11.4 MB (11362520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00abb7cbf1986a96190e7c5cde0d0b8357fed599515f3c0a016fd41d2ca630b3`  
		Last Modified: Fri, 25 Jun 2021 19:36:55 GMT  
		Size: 7.5 KB (7531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6398d9814288300bafe53392b735bfa7278f05ff47b608ed1b1e8770af593371`  
		Last Modified: Fri, 25 Jun 2021 19:36:55 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cca26753c05b96e61e904ffcd3b93181bd9f34e5e26aba0ff66e81cae701e8ce`  
		Last Modified: Fri, 25 Jun 2021 19:36:55 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9722f9d39832d6ef2862daf1acfe584527342852873e41627c191fd1f90478e9`  
		Last Modified: Fri, 25 Jun 2021 19:36:55 GMT  
		Size: 4.4 KB (4406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1db16b47fb768481caffd5fc2f869a576fd6291fcad920723c592ff32e57e5e0`  
		Last Modified: Fri, 25 Jun 2021 19:36:55 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:9-alpine` - linux; arm variant v7

```console
$ docker pull postgres@sha256:207aa7fbac860d69fcad77c83e18eba163f871f0d63637365d00a8ee45fdf87f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.1 MB (13135401 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9cc3f08e68c9c622b66c1d7b9b013c21975c082852e05e76f82d20495941f186`
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
# Wed, 23 Jun 2021 22:43:28 GMT
ENV PG_MAJOR=9.6
# Wed, 23 Jun 2021 22:43:29 GMT
ENV PG_VERSION=9.6.22
# Wed, 23 Jun 2021 22:43:29 GMT
ENV PG_SHA256=3d32cd101025a0556813397c69feff3df3d63736adb8adeaf365c522f39f2930
# Fri, 25 Jun 2021 20:05:28 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Fri, 25 Jun 2021 20:05:29 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample
# Fri, 25 Jun 2021 20:05:31 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 25 Jun 2021 20:05:32 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 25 Jun 2021 20:05:33 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 25 Jun 2021 20:05:34 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 25 Jun 2021 20:05:34 GMT
COPY file:e881105b30bb0f1591c0f7f6dfe19bf5351d029d5babae597d2698e04a16ec8b in /usr/local/bin/ 
# Fri, 25 Jun 2021 20:05:36 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 25 Jun 2021 20:05:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Jun 2021 20:05:37 GMT
STOPSIGNAL SIGINT
# Fri, 25 Jun 2021 20:05:37 GMT
EXPOSE 5432
# Fri, 25 Jun 2021 20:05:38 GMT
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
	-	`sha256:bfb124eee8878199ef3a6c3c06e07b2c53750d0e0b17cebce5e946333ededcef`  
		Last Modified: Fri, 25 Jun 2021 20:13:00 GMT  
		Size: 10.7 MB (10693640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:649b6a42b9b3c6be297ab9e3194d61af11e541df50d30df88a19f518be112fd4`  
		Last Modified: Fri, 25 Jun 2021 20:12:51 GMT  
		Size: 7.5 KB (7531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76c9d63397595117fd8231f65f84438a112e83d400e28f3393275d3bd06288d2`  
		Last Modified: Fri, 25 Jun 2021 20:12:51 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8792814c6ea2afae809ea30e6d43bf8f873492497b347ef909f21d153dc595b7`  
		Last Modified: Fri, 25 Jun 2021 20:12:51 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56e6a57dabf82472360586956c5b8ea94843311bda32910a0eb523ed064f0704`  
		Last Modified: Fri, 25 Jun 2021 20:12:51 GMT  
		Size: 4.4 KB (4407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42067cd901dac59f9c4cbe6a9b734278850e409eb8de183235a5805b22f8bd79`  
		Last Modified: Fri, 25 Jun 2021 20:12:51 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:9-alpine` - linux; arm64 variant v8

```console
$ docker pull postgres@sha256:18cf77d0ca2807d60f433e73bd3a73d89097d95532f4de5fcbb72d82ba900f34
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.3 MB (14301229 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:22317d0ac485e9e99c8c5bcf435c4b8ac5507d92f812a9b9fda7a47105ff2b4d`
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
# Wed, 16 Jun 2021 23:45:17 GMT
ENV PG_MAJOR=9.6
# Wed, 16 Jun 2021 23:45:18 GMT
ENV PG_VERSION=9.6.22
# Wed, 16 Jun 2021 23:45:18 GMT
ENV PG_SHA256=3d32cd101025a0556813397c69feff3df3d63736adb8adeaf365c522f39f2930
# Fri, 25 Jun 2021 19:15:50 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Fri, 25 Jun 2021 19:15:51 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample
# Fri, 25 Jun 2021 19:15:52 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 25 Jun 2021 19:15:52 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 25 Jun 2021 19:15:53 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 25 Jun 2021 19:15:53 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 25 Jun 2021 19:15:53 GMT
COPY file:e881105b30bb0f1591c0f7f6dfe19bf5351d029d5babae597d2698e04a16ec8b in /usr/local/bin/ 
# Fri, 25 Jun 2021 19:15:54 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 25 Jun 2021 19:15:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Jun 2021 19:15:54 GMT
STOPSIGNAL SIGINT
# Fri, 25 Jun 2021 19:15:55 GMT
EXPOSE 5432
# Fri, 25 Jun 2021 19:15:55 GMT
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
	-	`sha256:019af10d1815050625cea3cc7b9169e7a73798d2556312d16729e3a9b24c9078`  
		Last Modified: Fri, 25 Jun 2021 19:19:39 GMT  
		Size: 11.6 MB (11577760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:517e7e657dfd5eeefe816d3dc3442a11e40f68bd1b4aec78bbcf9ebeb2f88cec`  
		Last Modified: Fri, 25 Jun 2021 19:19:34 GMT  
		Size: 7.5 KB (7529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7521441c621a6b697776d13619b1a08fbbfa388593a47aa9a510e2aefcc7cb0e`  
		Last Modified: Fri, 25 Jun 2021 19:19:34 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81e11ffcf6fd713ee5df34c34541a1565172fbaf006a74e8962c91f563a15858`  
		Last Modified: Fri, 25 Jun 2021 19:19:34 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9925f0eff914638b08016b51ec238b6d0415e355ed2af597c63b4d0663ed1504`  
		Last Modified: Fri, 25 Jun 2021 19:19:34 GMT  
		Size: 4.4 KB (4403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4b5135c7ef4f6d568cfdc64c18a31dc02254bb3bafe617219ba2706158ec9d6`  
		Last Modified: Fri, 25 Jun 2021 19:19:35 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:9-alpine` - linux; 386

```console
$ docker pull postgres@sha256:9ebfd431126f26e50d0aa304544e8a314c7205eeae0da9397bd9f026c661cea2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.2 MB (15221788 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1a3666c848571b2b59565a9b26d5e0e5b2613d2c68e91f64229beab71a1fd6e8`
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
# Wed, 16 Jun 2021 23:19:41 GMT
ENV PG_MAJOR=9.6
# Wed, 16 Jun 2021 23:19:41 GMT
ENV PG_VERSION=9.6.22
# Wed, 16 Jun 2021 23:19:42 GMT
ENV PG_SHA256=3d32cd101025a0556813397c69feff3df3d63736adb8adeaf365c522f39f2930
# Fri, 25 Jun 2021 19:29:23 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Fri, 25 Jun 2021 19:29:26 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample
# Fri, 25 Jun 2021 19:29:28 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 25 Jun 2021 19:29:28 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 25 Jun 2021 19:29:30 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 25 Jun 2021 19:29:30 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 25 Jun 2021 19:29:31 GMT
COPY file:e881105b30bb0f1591c0f7f6dfe19bf5351d029d5babae597d2698e04a16ec8b in /usr/local/bin/ 
# Fri, 25 Jun 2021 19:29:33 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 25 Jun 2021 19:29:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Jun 2021 19:29:34 GMT
STOPSIGNAL SIGINT
# Fri, 25 Jun 2021 19:29:34 GMT
EXPOSE 5432
# Fri, 25 Jun 2021 19:29:34 GMT
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
	-	`sha256:f5643ec086420c17072b8bb6fceafbc1cbc5152db2dfbd95650a4446feabce2d`  
		Last Modified: Fri, 25 Jun 2021 19:34:40 GMT  
		Size: 12.4 MB (12387233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70db1318c620eca5afa46861cd748822c681ab65cafba048482e1a75cbb6ec90`  
		Last Modified: Fri, 25 Jun 2021 19:34:34 GMT  
		Size: 7.5 KB (7525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ece006fca192836ab4a987d120f27ed43349574aae63cb2e368d19170b5fc2f4`  
		Last Modified: Fri, 25 Jun 2021 19:34:34 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0176d0e4027a119472b676f73683a8a5d7d5922ea75ece620cbf5c9a9846f63`  
		Last Modified: Fri, 25 Jun 2021 19:34:34 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e78adc6c3c82303efb1df6bdcbe0b1826afc87e0e3aca0c48d2d9db992d454ae`  
		Last Modified: Fri, 25 Jun 2021 19:34:34 GMT  
		Size: 4.4 KB (4406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c70c12b0c1365ee3b43829508417696fbbbd16b777356332aca4dc2686689b8`  
		Last Modified: Fri, 25 Jun 2021 19:34:34 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:9-alpine` - linux; ppc64le

```console
$ docker pull postgres@sha256:2100ee3067321289a76b6b433463d04b421aa6081226455e36c60b3499ac073e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.6 MB (15562067 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:99a4357172ba1e0ba609fccae8ac5b2db33bac1c6e900ca0ee766473ecc92759`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Wed, 14 Apr 2021 19:30:57 GMT
ADD file:52162c4413e3597dad4ccb790c379b67ef40d50c0d0659e8b6c65d833886b3af in / 
# Wed, 14 Apr 2021 19:31:02 GMT
CMD ["/bin/sh"]
# Thu, 15 Apr 2021 04:37:26 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 15 Apr 2021 04:37:29 GMT
ENV LANG=en_US.utf8
# Thu, 15 Apr 2021 04:37:35 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 15 Apr 2021 04:59:55 GMT
ENV PG_MAJOR=9.6
# Fri, 14 May 2021 20:48:47 GMT
ENV PG_VERSION=9.6.22
# Fri, 14 May 2021 20:48:55 GMT
ENV PG_SHA256=3d32cd101025a0556813397c69feff3df3d63736adb8adeaf365c522f39f2930
# Fri, 14 May 2021 20:51:48 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Fri, 14 May 2021 20:52:06 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Fri, 14 May 2021 20:52:29 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 14 May 2021 20:52:39 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 14 May 2021 20:53:13 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 14 May 2021 20:53:22 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 14 May 2021 20:53:29 GMT
COPY file:e881105b30bb0f1591c0f7f6dfe19bf5351d029d5babae597d2698e04a16ec8b in /usr/local/bin/ 
# Fri, 14 May 2021 20:54:12 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 14 May 2021 20:54:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 14 May 2021 20:55:11 GMT
STOPSIGNAL SIGINT
# Fri, 14 May 2021 20:55:32 GMT
EXPOSE 5432
# Fri, 14 May 2021 20:55:53 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:771d2590aa602a0d4a922e322f02b22cc9d193f8cd159d9d1a140cadf1f8b4d4`  
		Last Modified: Wed, 14 Apr 2021 19:32:33 GMT  
		Size: 2.8 MB (2813141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85f26f1d1b4701765dc7858aba1bef999c1ba3b78d85ae321be21792492595da`  
		Last Modified: Thu, 15 Apr 2021 05:08:21 GMT  
		Size: 1.3 KB (1277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c0eecc487c054210f70b7f1edd080c1373eb1ca361753079d68703ae4d81948`  
		Last Modified: Thu, 15 Apr 2021 05:08:20 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:793abb29a3df839089f8bb065a0eac58027e598a3d80efecbdf56322aa37655c`  
		Last Modified: Fri, 14 May 2021 21:08:01 GMT  
		Size: 12.7 MB (12735451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae62ca7da78a343ca54f17355e5e148544e5c20ee05b4c3a441a68eeec891d6a`  
		Last Modified: Fri, 14 May 2021 21:07:53 GMT  
		Size: 7.2 KB (7166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8a9a996e886a2da98918cd7bb7e31bb05d1456adce7d638d020a6d6402a1ab2`  
		Last Modified: Fri, 14 May 2021 21:07:53 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ada6f9eb1a8ffc719bd6435ce8820185b3256d0cdc83294869a7e9b031eeb18a`  
		Last Modified: Fri, 14 May 2021 21:07:53 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38e19ebf7fbce6fc3acbd339a157e76b8992b8f9687eb063b336d7e0ee310910`  
		Last Modified: Fri, 14 May 2021 21:07:53 GMT  
		Size: 4.4 KB (4406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebd8e9284e4a259cf79361e11b72fb59e54de1e29882c03ba49e04da6d1ffb27`  
		Last Modified: Fri, 14 May 2021 21:07:53 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:9-alpine` - linux; s390x

```console
$ docker pull postgres@sha256:3143ae545c90f424f4213e3a8f0013512cf640d379f8f281b99a09bf68782a56
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.2 MB (14224936 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1edd49465efa725e868627b60e4916564510a2b29cf5629219644acde7b4c90d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Wed, 14 Apr 2021 18:41:35 GMT
ADD file:c715fef757fe2b022ae1bbff71dbc58bddf5a858deb0aac5a6fbcf10d5f3111c in / 
# Wed, 14 Apr 2021 18:41:36 GMT
CMD ["/bin/sh"]
# Thu, 15 Apr 2021 02:35:26 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 15 Apr 2021 02:35:26 GMT
ENV LANG=en_US.utf8
# Thu, 15 Apr 2021 02:35:27 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 15 Apr 2021 02:50:28 GMT
ENV PG_MAJOR=9.6
# Fri, 14 May 2021 20:26:32 GMT
ENV PG_VERSION=9.6.22
# Fri, 14 May 2021 20:26:32 GMT
ENV PG_SHA256=3d32cd101025a0556813397c69feff3df3d63736adb8adeaf365c522f39f2930
# Fri, 14 May 2021 20:28:33 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Fri, 14 May 2021 20:28:34 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Fri, 14 May 2021 20:28:35 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 14 May 2021 20:28:35 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 14 May 2021 20:28:36 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 14 May 2021 20:28:36 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 14 May 2021 20:28:36 GMT
COPY file:e881105b30bb0f1591c0f7f6dfe19bf5351d029d5babae597d2698e04a16ec8b in /usr/local/bin/ 
# Fri, 14 May 2021 20:28:37 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 14 May 2021 20:28:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 14 May 2021 20:28:37 GMT
STOPSIGNAL SIGINT
# Fri, 14 May 2021 20:28:38 GMT
EXPOSE 5432
# Fri, 14 May 2021 20:28:38 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:afadee6ad6a38d3172beeeca818219604c782efbe93201ef4d39512f289b05ae`  
		Last Modified: Wed, 14 Apr 2021 18:42:16 GMT  
		Size: 2.6 MB (2602650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f539beccb9c12dbbd5eb5238188d7421b0e766e3e536f47e5a25dce4187b138f`  
		Last Modified: Thu, 15 Apr 2021 02:55:28 GMT  
		Size: 1.3 KB (1276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78639c932051e59362713e29f35ff376c4cd5627ea231422efbf7cf7b253ec7a`  
		Last Modified: Thu, 15 Apr 2021 02:55:28 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa90c0b5da19370b135ebaa0ca9968890a006bf74cccc27f6159dd2d34ef077a`  
		Last Modified: Fri, 14 May 2021 20:30:44 GMT  
		Size: 11.6 MB (11608814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5c3912af0aeaa61172d81a19cda28f85464ab07cbb71505c22b04598831a8ff`  
		Last Modified: Fri, 14 May 2021 20:30:40 GMT  
		Size: 7.2 KB (7167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4650c3a007cec5e575f6d00dd93b649a45f20e85940a6f35fdd9894857897a17`  
		Last Modified: Fri, 14 May 2021 20:30:41 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:802a01cd84403ebc1e42fdb38c4cb5068cd4c7fde3f42f96b5b94f76cea255f5`  
		Last Modified: Fri, 14 May 2021 20:30:41 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dd8ca94fd07cdc0b1b7fe925d1682569a12e70d8f8909e024b79c9d401bbbf8`  
		Last Modified: Fri, 14 May 2021 20:30:46 GMT  
		Size: 4.4 KB (4405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99efcb267e51915eb320cdc5ccb1921286e1e4d17d7b04d7c85cf2562c01e8fd`  
		Last Modified: Fri, 14 May 2021 20:30:41 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
