## `postgres:11-alpine3.13`

```console
$ docker pull postgres@sha256:09014c82a269ca6ebeb62e837db8e16837bb8f9a0d587763ff4d6d0983dad147
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `postgres:11-alpine3.13` - linux; amd64

```console
$ docker pull postgres@sha256:7970b18d3c5384fd9c04a86bd5e035f8d3609d15b7efeeb7ec8458f0d66c184d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.5 MB (60548214 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a0c1cd75a1885c37a89245286a9907cd7be1cdcfcbca8888cd850f715e783e19`
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
# Thu, 15 Apr 2021 03:59:20 GMT
ENV PG_MAJOR=11
# Fri, 14 May 2021 19:51:21 GMT
ENV PG_VERSION=11.12
# Fri, 14 May 2021 19:51:21 GMT
ENV PG_SHA256=87f9d8b16b2b8ef71586f2ec76beac844819f64734b07fa33986755c2f53cb04
# Fri, 14 May 2021 19:58:05 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm10-dev clang g++ 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Fri, 14 May 2021 19:58:08 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Fri, 14 May 2021 19:58:10 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 14 May 2021 19:58:10 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 14 May 2021 19:58:12 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 14 May 2021 19:58:13 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 14 May 2021 19:58:13 GMT
COPY file:ad28506adc606e446eefc263bc99d4cb809e608d4f550956143bf13c82c91f85 in /usr/local/bin/ 
# Fri, 14 May 2021 19:58:15 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 14 May 2021 19:58:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 14 May 2021 19:58:16 GMT
STOPSIGNAL SIGINT
# Fri, 14 May 2021 19:58:16 GMT
EXPOSE 5432
# Fri, 14 May 2021 19:58:17 GMT
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
	-	`sha256:4ccfb61ea6ebc5a2888aa7464f1712f2000a4a1ee3482321943c3ee545586c6c`  
		Last Modified: Fri, 14 May 2021 20:12:54 GMT  
		Size: 57.7 MB (57722359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89c24901cc6d507b187c209882b9d349e5d462361b44846bac83e6a49420017f`  
		Last Modified: Fri, 14 May 2021 20:12:43 GMT  
		Size: 7.6 KB (7576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aa245525deeaec9e688ba7b8bd33e7958cd4d7c90ed1bad3ebc02bea68725c0`  
		Last Modified: Fri, 14 May 2021 20:12:43 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:628cda073dfb732ce47e4d071c88be596d970ad3be9c207f82be47cc563feefb`  
		Last Modified: Fri, 14 May 2021 20:12:43 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9440d7d0a587c9b5173f7afe16e433a46bf80f5b25f488742ca8cd89e3e7f46b`  
		Last Modified: Fri, 14 May 2021 20:12:43 GMT  
		Size: 4.4 KB (4408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f9f6bef65f135b0823c18591873a423ecc411a21fe15d489d84fa2b5f9f5a8d`  
		Last Modified: Fri, 14 May 2021 20:12:43 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:11-alpine3.13` - linux; arm variant v6

```console
$ docker pull postgres@sha256:e06ea831245e1a931be8419cee01b17325cc13921f748abce0417b5a7a089a75
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.3 MB (59258953 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ff464397eb98be3ae89a960267ffbbaf5fea6caa9bb9a5f0898d1a8cbf9d94ea`
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
# Mon, 12 Jul 2021 23:27:28 GMT
ENV PG_MAJOR=11
# Mon, 12 Jul 2021 23:27:29 GMT
ENV PG_VERSION=11.12
# Mon, 12 Jul 2021 23:27:30 GMT
ENV PG_SHA256=87f9d8b16b2b8ef71586f2ec76beac844819f64734b07fa33986755c2f53cb04
# Mon, 12 Jul 2021 23:32:21 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm10-dev clang g++ 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Mon, 12 Jul 2021 23:32:24 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Mon, 12 Jul 2021 23:32:25 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Mon, 12 Jul 2021 23:32:26 GMT
ENV PGDATA=/var/lib/postgresql/data
# Mon, 12 Jul 2021 23:32:27 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Mon, 12 Jul 2021 23:32:28 GMT
VOLUME [/var/lib/postgresql/data]
# Mon, 12 Jul 2021 23:32:28 GMT
COPY file:ad28506adc606e446eefc263bc99d4cb809e608d4f550956143bf13c82c91f85 in /usr/local/bin/ 
# Mon, 12 Jul 2021 23:32:30 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Mon, 12 Jul 2021 23:32:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 12 Jul 2021 23:32:31 GMT
STOPSIGNAL SIGINT
# Mon, 12 Jul 2021 23:32:31 GMT
EXPOSE 5432
# Mon, 12 Jul 2021 23:32:32 GMT
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
	-	`sha256:aea13cfcec141562261f3041e38c5b9847f91f87793d1d0ac6cd4aa5d7b48410`  
		Last Modified: Mon, 12 Jul 2021 23:46:37 GMT  
		Size: 56.6 MB (56622937 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0c55861fcb22729c5eb48b483c3b854472a0c515a5d6813816a4308af25f480`  
		Last Modified: Mon, 12 Jul 2021 23:46:00 GMT  
		Size: 7.6 KB (7579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01ad3140819d3a5a6d8f787f1c17fdc6069a04dfaecfd1fc5f16a9fd8443aa4e`  
		Last Modified: Mon, 12 Jul 2021 23:45:59 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ddde2a0fc087e6774cd7683ff7f0026c850a086379536668b5c04eb01c40f57`  
		Last Modified: Mon, 12 Jul 2021 23:45:59 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b47a23f2dda8de17473b3427b7bb73e8f301658d7ac250e8c741d71842a18a6`  
		Last Modified: Mon, 12 Jul 2021 23:45:59 GMT  
		Size: 4.4 KB (4404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a8cc9a50c1f254e4df6f821a531cc2c18cd413d5f2fe90f377689c17e395c32`  
		Last Modified: Mon, 12 Jul 2021 23:46:00 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:11-alpine3.13` - linux; arm64 variant v8

```console
$ docker pull postgres@sha256:e758449fcc02aad6f21c0e2d5bb25d998cd61240f2fe2724f267fa0b27abe3d9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.2 MB (60231744 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3cd53751d4c5693767e427f0b680ddd52285d8c5370087419222b6494a90c8a6`
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
# Wed, 16 Jun 2021 08:55:04 GMT
ENV PG_MAJOR=11
# Wed, 16 Jun 2021 08:55:04 GMT
ENV PG_VERSION=11.12
# Wed, 16 Jun 2021 08:55:04 GMT
ENV PG_SHA256=87f9d8b16b2b8ef71586f2ec76beac844819f64734b07fa33986755c2f53cb04
# Wed, 16 Jun 2021 08:59:32 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm10-dev clang g++ 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Wed, 16 Jun 2021 08:59:33 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Wed, 16 Jun 2021 08:59:34 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Wed, 16 Jun 2021 08:59:34 GMT
ENV PGDATA=/var/lib/postgresql/data
# Wed, 16 Jun 2021 08:59:35 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Wed, 16 Jun 2021 08:59:35 GMT
VOLUME [/var/lib/postgresql/data]
# Wed, 16 Jun 2021 08:59:35 GMT
COPY file:ad28506adc606e446eefc263bc99d4cb809e608d4f550956143bf13c82c91f85 in /usr/local/bin/ 
# Wed, 16 Jun 2021 08:59:36 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 16 Jun 2021 08:59:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Jun 2021 08:59:36 GMT
STOPSIGNAL SIGINT
# Wed, 16 Jun 2021 08:59:37 GMT
EXPOSE 5432
# Wed, 16 Jun 2021 08:59:37 GMT
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
	-	`sha256:aee675bbb742caa9848d887fc693513c37bdbf2bb6ccc1d95bef913d1934c178`  
		Last Modified: Wed, 16 Jun 2021 09:28:12 GMT  
		Size: 57.5 MB (57505834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb9bf392b5a0f2efe09cce2f390fa6fdea2aa16c1612269df73b4aac6b122d50`  
		Last Modified: Wed, 16 Jun 2021 09:28:00 GMT  
		Size: 7.6 KB (7577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf116ed66368d6a0e94da2cca2f110270f4bffb473fa4a01d64c821b1e370b60`  
		Last Modified: Wed, 16 Jun 2021 09:28:00 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24dba7bb14c7ff01b5870635fdee12cfe0b60d1e894ae7f378781d98571b3b6a`  
		Last Modified: Wed, 16 Jun 2021 09:28:00 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fc29dc55f9974af827ffa5e7f533665e5d2342178a10e4a49a8b88c7a6f6914`  
		Last Modified: Wed, 16 Jun 2021 09:28:00 GMT  
		Size: 4.4 KB (4401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:045c67a79e3aefccddf104f71e6d6818c6913f4b459ffb1bb33597457b17bc54`  
		Last Modified: Wed, 16 Jun 2021 09:28:00 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:11-alpine3.13` - linux; 386

```console
$ docker pull postgres@sha256:bb1fb76cd817427894e7e63f09e1ed368b59d5c99f8e3576a5a9cb1e2ca9ce8d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.0 MB (63989201 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:25049fe256dd0a2fc8f474cb24a8da0fc075357923a73a04dee56cc31d3f0639`
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
# Thu, 15 Apr 2021 06:19:58 GMT
ENV PG_MAJOR=11
# Fri, 14 May 2021 20:12:40 GMT
ENV PG_VERSION=11.12
# Fri, 14 May 2021 20:12:40 GMT
ENV PG_SHA256=87f9d8b16b2b8ef71586f2ec76beac844819f64734b07fa33986755c2f53cb04
# Fri, 14 May 2021 20:18:40 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm10-dev clang g++ 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Fri, 14 May 2021 20:18:42 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Fri, 14 May 2021 20:18:43 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 14 May 2021 20:18:43 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 14 May 2021 20:18:44 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 14 May 2021 20:18:44 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 14 May 2021 20:18:44 GMT
COPY file:ad28506adc606e446eefc263bc99d4cb809e608d4f550956143bf13c82c91f85 in /usr/local/bin/ 
# Fri, 14 May 2021 20:18:45 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 14 May 2021 20:18:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 14 May 2021 20:18:46 GMT
STOPSIGNAL SIGINT
# Fri, 14 May 2021 20:18:46 GMT
EXPOSE 5432
# Fri, 14 May 2021 20:18:46 GMT
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
	-	`sha256:cdf576df562089eb7ed17f8b4e44d34b9039233509b11e073f31b9e8aa583590`  
		Last Modified: Fri, 14 May 2021 20:31:54 GMT  
		Size: 61.2 MB (61156413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecdec80ec7804d02d085966b721d11cb57981d80bdd2fd14d5ac89911bd656cc`  
		Last Modified: Fri, 14 May 2021 20:31:39 GMT  
		Size: 7.6 KB (7582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:079059085f7344697bea9b85181937e1c85087cfa6a0e6b49cc5172b138cd361`  
		Last Modified: Fri, 14 May 2021 20:31:39 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c81c7cfcdd7ff89ad4c33072ecb2ec57dd26423d0f7b9a4422dea934503693e`  
		Last Modified: Fri, 14 May 2021 20:31:39 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8ea928a4e0fbc3e0f5ea1cb298177a59d60cc7556302b4e9e2e87203ec274b7`  
		Last Modified: Fri, 14 May 2021 20:31:39 GMT  
		Size: 4.4 KB (4405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb8dae001223c72a2bd7a072931358a3765d0c5138df17db43ec42a96a9c3f5e`  
		Last Modified: Fri, 14 May 2021 20:31:39 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:11-alpine3.13` - linux; ppc64le

```console
$ docker pull postgres@sha256:0cea2ea1640b5d32fb7839ec4566e14b9c9cc64baed517c95049d7d5899fd59a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.3 MB (63253824 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a21c5876edff9b19fe2960aef0164640270ace56abb187591539f4003497326b`
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
# Mon, 12 Jul 2021 23:11:36 GMT
ENV PG_MAJOR=11
# Mon, 12 Jul 2021 23:11:40 GMT
ENV PG_VERSION=11.12
# Mon, 12 Jul 2021 23:11:44 GMT
ENV PG_SHA256=87f9d8b16b2b8ef71586f2ec76beac844819f64734b07fa33986755c2f53cb04
# Mon, 12 Jul 2021 23:16:07 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm10-dev clang g++ 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Mon, 12 Jul 2021 23:16:30 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Mon, 12 Jul 2021 23:16:43 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Mon, 12 Jul 2021 23:16:50 GMT
ENV PGDATA=/var/lib/postgresql/data
# Mon, 12 Jul 2021 23:17:00 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Mon, 12 Jul 2021 23:17:03 GMT
VOLUME [/var/lib/postgresql/data]
# Mon, 12 Jul 2021 23:17:05 GMT
COPY file:ad28506adc606e446eefc263bc99d4cb809e608d4f550956143bf13c82c91f85 in /usr/local/bin/ 
# Mon, 12 Jul 2021 23:17:21 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Mon, 12 Jul 2021 23:17:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 12 Jul 2021 23:17:34 GMT
STOPSIGNAL SIGINT
# Mon, 12 Jul 2021 23:17:40 GMT
EXPOSE 5432
# Mon, 12 Jul 2021 23:17:45 GMT
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
	-	`sha256:8d30c0eecc22b0fc39194c7c53e085be1e42c1617670d2ba213065d1d96edca7`  
		Last Modified: Mon, 12 Jul 2021 23:33:36 GMT  
		Size: 60.4 MB (60426791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4af1c8715437ac2d0248635d144058999778d354821f778602a30c04c3e1c0cc`  
		Last Modified: Mon, 12 Jul 2021 23:33:21 GMT  
		Size: 7.6 KB (7580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9a758d8cc8af40b3cc153ccbf4db3acaf5795df1e04e9b58d2213e3b58ee917`  
		Last Modified: Mon, 12 Jul 2021 23:33:21 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bd818625a9092d922c97a4d2d456dbc747ae944cab2db46f655cf57e3d77c5e`  
		Last Modified: Mon, 12 Jul 2021 23:33:21 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1571c07c80a5d2f7c8080637758609a5bed1bddd8badd5412705aa0d05a89a15`  
		Last Modified: Mon, 12 Jul 2021 23:33:21 GMT  
		Size: 4.4 KB (4405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88e4c87ecc187655cbc91a0ba0b122b7c3a58c6dd18c463c621a611defc71f91`  
		Last Modified: Mon, 12 Jul 2021 23:33:22 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:11-alpine3.13` - linux; s390x

```console
$ docker pull postgres@sha256:3db2198d950e737424ac13390af06f88f00fc4c16de4c02bfedb6e4c5965e5b4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.2 MB (63242986 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e5981ee8fd0befc4c9132e7e3db9f4c99f5567fda99aafd11b4d95cf4bf0e36`
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
# Tue, 13 Jul 2021 00:27:16 GMT
ENV PG_MAJOR=11
# Tue, 13 Jul 2021 00:27:16 GMT
ENV PG_VERSION=11.12
# Tue, 13 Jul 2021 00:27:17 GMT
ENV PG_SHA256=87f9d8b16b2b8ef71586f2ec76beac844819f64734b07fa33986755c2f53cb04
# Tue, 13 Jul 2021 00:33:54 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm10-dev clang g++ 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Tue, 13 Jul 2021 00:34:03 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Tue, 13 Jul 2021 00:34:06 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 13 Jul 2021 00:34:07 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 13 Jul 2021 00:34:08 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 13 Jul 2021 00:34:09 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 13 Jul 2021 00:34:10 GMT
COPY file:ad28506adc606e446eefc263bc99d4cb809e608d4f550956143bf13c82c91f85 in /usr/local/bin/ 
# Tue, 13 Jul 2021 00:34:12 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Tue, 13 Jul 2021 00:34:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Jul 2021 00:34:13 GMT
STOPSIGNAL SIGINT
# Tue, 13 Jul 2021 00:34:14 GMT
EXPOSE 5432
# Tue, 13 Jul 2021 00:34:15 GMT
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
	-	`sha256:3d798ffba162e36f99b48922e931add32d54941d690a31e06f6fc843cedb4b07`  
		Last Modified: Tue, 13 Jul 2021 00:47:53 GMT  
		Size: 60.6 MB (60626449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6238a4962f4dfbc8ef3d0b5f29a8dc8c9636f98c0a1a58fb1e54d7a62b54d9fa`  
		Last Modified: Tue, 13 Jul 2021 00:47:42 GMT  
		Size: 7.6 KB (7580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a4eb6bcd1df0f6153897b6727a5211efac0c6c19cee8567e6592410bb6a54ac`  
		Last Modified: Tue, 13 Jul 2021 00:47:42 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a6d6433ef05b682ca8ccb5ce120b6a40960c62180410f178b6b3ce194a74602`  
		Last Modified: Tue, 13 Jul 2021 00:47:42 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55474f2225acf9bc4d591a67cbce21fce0e79f6f736451b3595f2f45348e4d2e`  
		Last Modified: Tue, 13 Jul 2021 00:47:42 GMT  
		Size: 4.4 KB (4404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7ccb6f9d6f9ee2cbccb67f1e9429ba41a75c8de92aabb9bfbe897bfffcf759b`  
		Last Modified: Tue, 13 Jul 2021 00:47:42 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
