## `postgres:9-alpine3.13`

```console
$ docker pull postgres@sha256:e3c0e48f4bd741049af55afb8d368c4178d80390c46bc15e67e50df4976ddafa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `postgres:9-alpine3.13` - linux; amd64

```console
$ docker pull postgres@sha256:0fceaf685127b0b557a1ed84f6d6fbba22f2101c1bf7cc0410fba13cd7618000
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.5 MB (14547466 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:60d950d0004d074b3428080181976e3450ab885e7d23f673473242c7e6d3d970`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Thu, 15 Apr 2021 03:44:32 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 15 Apr 2021 03:44:32 GMT
ENV LANG=en_US.utf8
# Thu, 15 Apr 2021 03:44:33 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 15 Apr 2021 04:12:22 GMT
ENV PG_MAJOR=9.6
# Fri, 14 May 2021 20:04:08 GMT
ENV PG_VERSION=9.6.22
# Fri, 14 May 2021 20:04:08 GMT
ENV PG_SHA256=3d32cd101025a0556813397c69feff3df3d63736adb8adeaf365c522f39f2930
# Fri, 14 May 2021 20:09:32 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Fri, 14 May 2021 20:09:34 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Fri, 14 May 2021 20:09:37 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 14 May 2021 20:09:37 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 14 May 2021 20:09:39 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 14 May 2021 20:09:40 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 14 May 2021 20:09:40 GMT
COPY file:e881105b30bb0f1591c0f7f6dfe19bf5351d029d5babae597d2698e04a16ec8b in /usr/local/bin/ 
# Fri, 14 May 2021 20:09:42 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 14 May 2021 20:09:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 14 May 2021 20:09:43 GMT
STOPSIGNAL SIGINT
# Fri, 14 May 2021 20:09:43 GMT
EXPOSE 5432
# Fri, 14 May 2021 20:09:43 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3cb73039552ea36b22e7ea1fabf738b87f83b2c9347901ce77b79c790389bb7`  
		Last Modified: Thu, 15 Apr 2021 04:21:20 GMT  
		Size: 1.3 KB (1277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39855706e49a3eeebf4c28a2ff3d706c5cdbe7bb1726d272188f08e91a46bfb8`  
		Last Modified: Thu, 15 Apr 2021 04:21:19 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caacf3a6c4e30b29f55a45ebab958805b2742fa2692a5c3b9e744ad7044fffde`  
		Last Modified: Fri, 14 May 2021 20:14:18 GMT  
		Size: 11.7 MB (11722022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a43e10552cb913a2435fb3a5f2c86756bb9de36d3770a19d370aeb0a56d3d399`  
		Last Modified: Fri, 14 May 2021 20:14:13 GMT  
		Size: 7.2 KB (7165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ad27a20815a176dfc2b7070cf2cd703d14a1fc96b4ff24d129fb2a219af4e0f`  
		Last Modified: Fri, 14 May 2021 20:14:13 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dabb4cf8dc15cd435b4fc897977218f65e44a163c4da61e4453ef359de0701b5`  
		Last Modified: Fri, 14 May 2021 20:14:13 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:817e5c24ebbc37820e6b901b48212e0c499c49c73ad71b54b97d90c9cbdf0657`  
		Last Modified: Fri, 14 May 2021 20:14:13 GMT  
		Size: 4.4 KB (4408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71f8cfbd522dcb11f4ff846acdb10bf2e7beae0173475f8ad5e2b37d627d9e6a`  
		Last Modified: Fri, 14 May 2021 20:14:13 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:9-alpine3.13` - linux; arm variant v6

```console
$ docker pull postgres@sha256:72d3c7727aaeb6b1adb99a971a2db2cb68a420356bcdb22ce5faded0d11b51c3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.3 MB (14324937 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:622e3278963a2043ab663fe2aacdbc56575b616ae6fc2f306adb6339bdd9b0ce`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 15 Jun 2021 22:57:34 GMT
ADD file:4479f0a51530e039edf231d87201896dcff908aa542a613cdccb015f93dda8a3 in / 
# Tue, 15 Jun 2021 22:57:34 GMT
CMD ["/bin/sh"]
# Mon, 12 Jul 2021 23:17:05 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Mon, 12 Jul 2021 23:17:06 GMT
ENV LANG=en_US.utf8
# Mon, 12 Jul 2021 23:17:07 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Mon, 12 Jul 2021 23:36:51 GMT
ENV PG_MAJOR=9.6
# Mon, 12 Jul 2021 23:36:52 GMT
ENV PG_VERSION=9.6.22
# Mon, 12 Jul 2021 23:36:52 GMT
ENV PG_SHA256=3d32cd101025a0556813397c69feff3df3d63736adb8adeaf365c522f39f2930
# Mon, 12 Jul 2021 23:40:08 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Mon, 12 Jul 2021 23:40:10 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Mon, 12 Jul 2021 23:40:13 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Mon, 12 Jul 2021 23:40:13 GMT
ENV PGDATA=/var/lib/postgresql/data
# Mon, 12 Jul 2021 23:40:15 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Mon, 12 Jul 2021 23:40:16 GMT
VOLUME [/var/lib/postgresql/data]
# Mon, 12 Jul 2021 23:40:16 GMT
COPY file:e881105b30bb0f1591c0f7f6dfe19bf5351d029d5babae597d2698e04a16ec8b in /usr/local/bin/ 
# Mon, 12 Jul 2021 23:40:19 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Mon, 12 Jul 2021 23:40:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 12 Jul 2021 23:40:20 GMT
STOPSIGNAL SIGINT
# Mon, 12 Jul 2021 23:40:20 GMT
EXPOSE 5432
# Mon, 12 Jul 2021 23:40:21 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:740c950346cf39c85b52576998695c9b909c24a58a8bb1b64cce91fda3ef1d3a`  
		Last Modified: Wed, 14 Apr 2021 18:50:30 GMT  
		Size: 2.6 MB (2622131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:957b1aca16cb7c58365877da0bd1faee5e1ffb47a865ee837514aae66d5897d8`  
		Last Modified: Mon, 12 Jul 2021 23:44:17 GMT  
		Size: 1.3 KB (1278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83b82e52d6594d4fbeddc069e45000bf8a43379127bb1958a008ad747756e4cd`  
		Last Modified: Mon, 12 Jul 2021 23:44:17 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa4f66dfa8453c4eb16cd4c00aa3ffda47e8e9311486d61b682d6a1194c89a08`  
		Last Modified: Mon, 12 Jul 2021 23:47:31 GMT  
		Size: 11.7 MB (11689328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7886b3a56a192d5307ef5ada4689ed0c4b4932c08b41aa6e9c8fcb5ba520472`  
		Last Modified: Mon, 12 Jul 2021 23:47:21 GMT  
		Size: 7.2 KB (7168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da8f1c0e14cc94d16ff7b5d62005a7922879aad22b08daa60f1daae8b4025ab9`  
		Last Modified: Mon, 12 Jul 2021 23:47:21 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:288e6057418a14f55afd7c692eda362d7066f55dd345be0e9b0f4ca6c58f4b11`  
		Last Modified: Mon, 12 Jul 2021 23:47:21 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:924d6945040d07576e3d0bff67c0e829ef9603562bfe93642731701f1fdd435c`  
		Last Modified: Mon, 12 Jul 2021 23:47:21 GMT  
		Size: 4.4 KB (4407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e135595c81523d5b1d845f1cb2fe6966a5b547961a9d1f691eb877652fb161e4`  
		Last Modified: Mon, 12 Jul 2021 23:47:21 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:9-alpine3.13` - linux; arm64 variant v8

```console
$ docker pull postgres@sha256:eb77322ba0528c57ab326cc49d86746abde8302a39a3c6460acec9175be4b10a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.7 MB (14664283 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:45a4c842b66ae6115163fec3eee6f6965a12dd9d1b37be7e25320d803153e13f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 15 Jun 2021 21:45:03 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Tue, 15 Jun 2021 21:45:04 GMT
CMD ["/bin/sh"]
# Wed, 16 Jun 2021 08:34:51 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Wed, 16 Jun 2021 08:34:51 GMT
ENV LANG=en_US.utf8
# Wed, 16 Jun 2021 08:34:52 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 16 Jun 2021 09:22:00 GMT
ENV PG_MAJOR=9.6
# Wed, 16 Jun 2021 09:22:00 GMT
ENV PG_VERSION=9.6.22
# Wed, 16 Jun 2021 09:22:00 GMT
ENV PG_SHA256=3d32cd101025a0556813397c69feff3df3d63736adb8adeaf365c522f39f2930
# Wed, 16 Jun 2021 09:24:40 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Wed, 16 Jun 2021 09:24:41 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Wed, 16 Jun 2021 09:24:42 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Wed, 16 Jun 2021 09:24:42 GMT
ENV PGDATA=/var/lib/postgresql/data
# Wed, 16 Jun 2021 09:24:43 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Wed, 16 Jun 2021 09:24:43 GMT
VOLUME [/var/lib/postgresql/data]
# Wed, 16 Jun 2021 09:24:43 GMT
COPY file:e881105b30bb0f1591c0f7f6dfe19bf5351d029d5babae597d2698e04a16ec8b in /usr/local/bin/ 
# Wed, 16 Jun 2021 09:24:44 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 16 Jun 2021 09:24:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Jun 2021 09:24:44 GMT
STOPSIGNAL SIGINT
# Wed, 16 Jun 2021 09:24:45 GMT
EXPOSE 5432
# Wed, 16 Jun 2021 09:24:45 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f371db7316b44874c3c018d3dbc2dacb013ac75a8807c03dcb87219ef26fd1e3`  
		Last Modified: Wed, 16 Jun 2021 09:26:22 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f098f183ff9fed325c5e1fbbf197648d3666d7d79d33dd7a33a076862ec5b222`  
		Last Modified: Wed, 16 Jun 2021 09:26:22 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b863b421c9bebc8d4bfb3ffe964397bdb827aaf8cd909c64c50fd91163ca0356`  
		Last Modified: Wed, 16 Jun 2021 09:29:34 GMT  
		Size: 11.9 MB (11938781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55179377c183b72c400f1893061173453c4cb9b8b54c686264a691a808ad3865`  
		Last Modified: Wed, 16 Jun 2021 09:29:30 GMT  
		Size: 7.2 KB (7164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adefb8b37f08e6db52212de6a3731cc9ded4f0231321147a90497fa98b254cc0`  
		Last Modified: Wed, 16 Jun 2021 09:29:30 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbe3b4397e1f9522a74a2b559d37f8aca6f433fac20193445a8d898a6cd05990`  
		Last Modified: Wed, 16 Jun 2021 09:29:30 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:141933f20ce990e46478a4cc87c30c0ec3bc845ec30d3294ccca089773d55427`  
		Last Modified: Wed, 16 Jun 2021 09:29:30 GMT  
		Size: 4.4 KB (4403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:510732c44a3ad4430931a40277e8f578ed6520546caed591d48844505ede43e7`  
		Last Modified: Wed, 16 Jun 2021 09:29:30 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:9-alpine3.13` - linux; 386

```console
$ docker pull postgres@sha256:665aa3d8831964cbf33b914c7b3624f39d0c50d5409c58550fabebbdcd8f60a1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.2 MB (15189872 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c4f872b8eafeededb104e102ad6d238fad6f0a8d2c7d18394d62e7c12a25a65d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Wed, 14 Apr 2021 18:38:29 GMT
ADD file:36634145ad6ec95a6b1a4f8d875f48719357c7a90f9b4906f8ce74f71b28c19d in / 
# Wed, 14 Apr 2021 18:38:29 GMT
CMD ["/bin/sh"]
# Thu, 15 Apr 2021 06:08:09 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 15 Apr 2021 06:08:09 GMT
ENV LANG=en_US.utf8
# Thu, 15 Apr 2021 06:08:10 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 15 Apr 2021 06:29:18 GMT
ENV PG_MAJOR=9.6
# Fri, 14 May 2021 20:24:09 GMT
ENV PG_VERSION=9.6.22
# Fri, 14 May 2021 20:24:09 GMT
ENV PG_SHA256=3d32cd101025a0556813397c69feff3df3d63736adb8adeaf365c522f39f2930
# Fri, 14 May 2021 20:27:28 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Fri, 14 May 2021 20:27:29 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Fri, 14 May 2021 20:27:30 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 14 May 2021 20:27:30 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 14 May 2021 20:27:31 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 14 May 2021 20:27:31 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 14 May 2021 20:27:32 GMT
COPY file:e881105b30bb0f1591c0f7f6dfe19bf5351d029d5babae597d2698e04a16ec8b in /usr/local/bin/ 
# Fri, 14 May 2021 20:27:33 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 14 May 2021 20:27:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 14 May 2021 20:27:33 GMT
STOPSIGNAL SIGINT
# Fri, 14 May 2021 20:27:33 GMT
EXPOSE 5432
# Fri, 14 May 2021 20:27:34 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:31b7e7ccca9e17fd08b39c9a4ffd3ded380b62816c489d6c3758c9bb5a632430`  
		Last Modified: Wed, 14 Apr 2021 18:39:24 GMT  
		Size: 2.8 MB (2818900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5d598db5bdb56bc14bf75398a61d3a0d982e72260a1108a46665627a73212d0`  
		Last Modified: Thu, 15 Apr 2021 06:36:56 GMT  
		Size: 1.3 KB (1277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc60ee1989b27c3c75961dc0e2a874021e7626fcaf8c4e289d05df49a78c40cd`  
		Last Modified: Thu, 15 Apr 2021 06:36:56 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cde3a40b8a061ba3e9749dea181e4f839593ead2cd387ce26258bb606e8d2e06`  
		Last Modified: Fri, 14 May 2021 20:33:25 GMT  
		Size: 12.4 MB (12357492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cc025483ae5fa4095e5dc09c0e14148a98b3adab2ebe5bebf40a0b63e1446b9`  
		Last Modified: Fri, 14 May 2021 20:33:19 GMT  
		Size: 7.2 KB (7171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:048a441a2fb9380bc5dc2aef2109568c82e70805fdbbcd8daba54a88dfe79583`  
		Last Modified: Fri, 14 May 2021 20:33:20 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1e423bb266a8f1fb1029b062704351dbd656175c3b791d1ffefa7d76045aba1`  
		Last Modified: Fri, 14 May 2021 20:33:20 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d0cca3a8c25046825cac8ba69043fe6ec51df6129fb3e551fb5548193ab3f29`  
		Last Modified: Fri, 14 May 2021 20:33:20 GMT  
		Size: 4.4 KB (4407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e9a74d30132bc58b418c4e1a565e7d95dfc3a7c4864167d91d863bbf1580f18`  
		Last Modified: Fri, 14 May 2021 20:33:20 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:9-alpine3.13` - linux; ppc64le

```console
$ docker pull postgres@sha256:75e2fd2bc85f8e7927e67e16331c3ee1ddf01787a4f84cb16ca72fef83d95840
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.0 MB (15953464 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba46a8135c8064b6553d617230b9fe9b2938eb701db5831ad5fa05c7c49e5595`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Wed, 14 Apr 2021 19:30:57 GMT
ADD file:52162c4413e3597dad4ccb790c379b67ef40d50c0d0659e8b6c65d833886b3af in / 
# Wed, 14 Apr 2021 19:31:02 GMT
CMD ["/bin/sh"]
# Mon, 12 Jul 2021 22:58:30 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Mon, 12 Jul 2021 22:58:33 GMT
ENV LANG=en_US.utf8
# Mon, 12 Jul 2021 22:58:44 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Mon, 12 Jul 2021 23:23:35 GMT
ENV PG_MAJOR=9.6
# Mon, 12 Jul 2021 23:23:43 GMT
ENV PG_VERSION=9.6.22
# Mon, 12 Jul 2021 23:23:50 GMT
ENV PG_SHA256=3d32cd101025a0556813397c69feff3df3d63736adb8adeaf365c522f39f2930
# Mon, 12 Jul 2021 23:26:33 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Mon, 12 Jul 2021 23:26:50 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Mon, 12 Jul 2021 23:27:01 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Mon, 12 Jul 2021 23:27:05 GMT
ENV PGDATA=/var/lib/postgresql/data
# Mon, 12 Jul 2021 23:27:18 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Mon, 12 Jul 2021 23:27:26 GMT
VOLUME [/var/lib/postgresql/data]
# Mon, 12 Jul 2021 23:27:31 GMT
COPY file:e881105b30bb0f1591c0f7f6dfe19bf5351d029d5babae597d2698e04a16ec8b in /usr/local/bin/ 
# Mon, 12 Jul 2021 23:27:46 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Mon, 12 Jul 2021 23:27:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 12 Jul 2021 23:27:55 GMT
STOPSIGNAL SIGINT
# Mon, 12 Jul 2021 23:27:58 GMT
EXPOSE 5432
# Mon, 12 Jul 2021 23:28:03 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:771d2590aa602a0d4a922e322f02b22cc9d193f8cd159d9d1a140cadf1f8b4d4`  
		Last Modified: Wed, 14 Apr 2021 19:32:33 GMT  
		Size: 2.8 MB (2813141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd6b1fdf45ba85b0eec3c08346703770c6fa8461aef0f1e5d92e80dee81f5ec3`  
		Last Modified: Mon, 12 Jul 2021 23:32:30 GMT  
		Size: 1.3 KB (1283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d1656ac6a93b634ef3d1f29404d2402168b6548155466e1e19413124692abee`  
		Last Modified: Mon, 12 Jul 2021 23:32:30 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78cd30d3633378ebc7457c87edad17cf66a2799052034a582bb8f49bf604eb1a`  
		Last Modified: Mon, 12 Jul 2021 23:34:15 GMT  
		Size: 13.1 MB (13126838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a91e085347a038c25733fc98c6b6af09f17d4514f358cfc6d4bf07ebfb0b078`  
		Last Modified: Mon, 12 Jul 2021 23:34:09 GMT  
		Size: 7.2 KB (7170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee305b5c254c6302809d0b545ad61d21a8bde0988e557cec9084235f12d26a9d`  
		Last Modified: Mon, 12 Jul 2021 23:34:09 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:160aefbeadccb5347570df13a8c6205fcc0967d9a039ad3c4f8cf866025fded7`  
		Last Modified: Mon, 12 Jul 2021 23:34:09 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef2915a029015078ee6ef0d58a829890ec451a70c481da586bfd67127be138d2`  
		Last Modified: Mon, 12 Jul 2021 23:34:09 GMT  
		Size: 4.4 KB (4407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5905e1b12abfa9b98f58c55a97d81bfabc1e79186653317fda91eb8c793af36`  
		Last Modified: Mon, 12 Jul 2021 23:34:09 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:9-alpine3.13` - linux; s390x

```console
$ docker pull postgres@sha256:97be8e142ae2633893ce8cab389a1fbea49c83278d026c2b11144f4e7f091f9f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.6 MB (14625355 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:94fbf3beb45d9db4fbb10bddaf8f254bcaa99e8b8fb8943b1e567d284cd98288`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Wed, 14 Apr 2021 18:41:35 GMT
ADD file:c715fef757fe2b022ae1bbff71dbc58bddf5a858deb0aac5a6fbcf10d5f3111c in / 
# Wed, 14 Apr 2021 18:41:36 GMT
CMD ["/bin/sh"]
# Tue, 13 Jul 2021 00:11:26 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Tue, 13 Jul 2021 00:11:27 GMT
ENV LANG=en_US.utf8
# Tue, 13 Jul 2021 00:11:29 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 13 Jul 2021 00:39:28 GMT
ENV PG_MAJOR=9.6
# Tue, 13 Jul 2021 00:39:29 GMT
ENV PG_VERSION=9.6.22
# Tue, 13 Jul 2021 00:39:29 GMT
ENV PG_SHA256=3d32cd101025a0556813397c69feff3df3d63736adb8adeaf365c522f39f2930
# Tue, 13 Jul 2021 00:43:24 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Tue, 13 Jul 2021 00:43:27 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Tue, 13 Jul 2021 00:43:29 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 13 Jul 2021 00:43:30 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 13 Jul 2021 00:43:31 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 13 Jul 2021 00:43:32 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 13 Jul 2021 00:43:32 GMT
COPY file:e881105b30bb0f1591c0f7f6dfe19bf5351d029d5babae597d2698e04a16ec8b in /usr/local/bin/ 
# Tue, 13 Jul 2021 00:43:34 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Tue, 13 Jul 2021 00:43:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Jul 2021 00:43:35 GMT
STOPSIGNAL SIGINT
# Tue, 13 Jul 2021 00:43:35 GMT
EXPOSE 5432
# Tue, 13 Jul 2021 00:43:36 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:afadee6ad6a38d3172beeeca818219604c782efbe93201ef4d39512f289b05ae`  
		Last Modified: Wed, 14 Apr 2021 18:42:16 GMT  
		Size: 2.6 MB (2602650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68fdd2776568e1159ee997287cceca0dd324bb559ef0509f32a74925763e09e1`  
		Last Modified: Tue, 13 Jul 2021 00:46:41 GMT  
		Size: 1.3 KB (1278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:611359463d48c1036be3e5dcedbab576bc0a6c53d504d5d41010406c7854baab`  
		Last Modified: Tue, 13 Jul 2021 00:46:41 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abf8b26379df16616a893658848ed1297bbaf5d3bec82ad31c8704422bcc216a`  
		Last Modified: Tue, 13 Jul 2021 00:48:21 GMT  
		Size: 12.0 MB (12009234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c81c694eb7c7265305170af10909acdac6479aeb14501c021084d42f22e47833`  
		Last Modified: Tue, 13 Jul 2021 00:48:17 GMT  
		Size: 7.2 KB (7162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e45c6fbdc34d908dd9a7026da996d3902bc2f7dab7f7218cad07d78a0eb17ce4`  
		Last Modified: Tue, 13 Jul 2021 00:48:17 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1250175f89a3f4fa0a0286802fe1a93a725b8d52f14d0cfa47da6ef2ea5ec1f2`  
		Last Modified: Tue, 13 Jul 2021 00:48:17 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:724a1a253e50639ed86738d5b8a6d7b21c690fa4a693fe8f0f6732ad62c8402e`  
		Last Modified: Tue, 13 Jul 2021 00:48:17 GMT  
		Size: 4.4 KB (4406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7db10f9030d070fdc580195047abd9634bf13d405f35d7b4eda58438de2c65f4`  
		Last Modified: Tue, 13 Jul 2021 00:48:17 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
