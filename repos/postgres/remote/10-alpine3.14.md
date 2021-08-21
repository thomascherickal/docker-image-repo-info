## `postgres:10-alpine3.14`

```console
$ docker pull postgres@sha256:1d14e8c879a8121bc2eeeca989529de5a76eebc01257038ed662dbe9dfcd1f51
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
$ docker pull postgres@sha256:a0b7ab218ec0e916665eb1ce7856ec602091a9a0bb42df386f61f7b0722ce7ed
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.7 MB (28659293 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f97ea1dd5c1684f08c2869442e90e8f5af9090727e4124ec95332a407ccee73a`
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
# Fri, 06 Aug 2021 20:38:34 GMT
ENV PG_MAJOR=10
# Thu, 12 Aug 2021 21:08:49 GMT
ENV PG_VERSION=10.18
# Thu, 12 Aug 2021 21:08:49 GMT
ENV PG_SHA256=57477c2edc82c3f86a74747707b3babc1f301f389315ae14e819e025c0ba3801
# Thu, 12 Aug 2021 21:13:38 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Thu, 12 Aug 2021 21:13:40 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample
# Thu, 12 Aug 2021 21:13:42 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 12 Aug 2021 21:13:42 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 12 Aug 2021 21:13:44 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 12 Aug 2021 21:13:45 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 12 Aug 2021 21:13:45 GMT
COPY file:ad28506adc606e446eefc263bc99d4cb809e608d4f550956143bf13c82c91f85 in /usr/local/bin/ 
# Thu, 12 Aug 2021 21:13:47 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 12 Aug 2021 21:13:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 12 Aug 2021 21:13:48 GMT
STOPSIGNAL SIGINT
# Thu, 12 Aug 2021 21:13:48 GMT
EXPOSE 5432
# Thu, 12 Aug 2021 21:13:48 GMT
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
	-	`sha256:79460b2651a17ba27c94ac5a8cf9cb00c8e49e0d09c722a8e3f69fe59ad7742b`  
		Last Modified: Thu, 12 Aug 2021 21:25:26 GMT  
		Size: 25.8 MB (25832241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbd3892bb03543e5a6fa21e75419015b465651382f6645026cf7b60f9e3e4119`  
		Last Modified: Thu, 12 Aug 2021 21:25:19 GMT  
		Size: 7.7 KB (7732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e926b47ceb70f58dc48d173e04be1d7027653f2267b6dfcd317f63329b4996b`  
		Last Modified: Thu, 12 Aug 2021 21:25:19 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d458f5836c117d14c2506420058d004f7dedee1f282efc9f74177c5e144f5275`  
		Last Modified: Thu, 12 Aug 2021 21:25:19 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8456db1d837f9c5b13597ac57989538e89f9bf8b7a887802e394f5eddab3d69c`  
		Last Modified: Thu, 12 Aug 2021 21:25:19 GMT  
		Size: 4.4 KB (4405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfbc1767106480ec0f6ca47c612eb6c526bbafe9478fae27a31f880044280909`  
		Last Modified: Thu, 12 Aug 2021 21:25:19 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:10-alpine3.14` - linux; arm variant v6

```console
$ docker pull postgres@sha256:6058fd6db44a2fbfa69698bbaae1cad3d60c5030e16e2251849a83daedd165c8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.8 MB (27802003 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4fe2f1700030cb00c5a5cf6b8475fa2ea456d9188849efd1308b1a725396dea4`
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
# Fri, 06 Aug 2021 21:55:17 GMT
ENV PG_MAJOR=10
# Thu, 12 Aug 2021 23:52:47 GMT
ENV PG_VERSION=10.18
# Thu, 12 Aug 2021 23:52:47 GMT
ENV PG_SHA256=57477c2edc82c3f86a74747707b3babc1f301f389315ae14e819e025c0ba3801
# Thu, 12 Aug 2021 23:56:56 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Thu, 12 Aug 2021 23:56:59 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample
# Thu, 12 Aug 2021 23:57:04 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 12 Aug 2021 23:57:05 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 12 Aug 2021 23:57:08 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 12 Aug 2021 23:57:09 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 12 Aug 2021 23:57:11 GMT
COPY file:ad28506adc606e446eefc263bc99d4cb809e608d4f550956143bf13c82c91f85 in /usr/local/bin/ 
# Thu, 12 Aug 2021 23:57:15 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 12 Aug 2021 23:57:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 12 Aug 2021 23:57:16 GMT
STOPSIGNAL SIGINT
# Thu, 12 Aug 2021 23:57:18 GMT
EXPOSE 5432
# Thu, 12 Aug 2021 23:57:19 GMT
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
	-	`sha256:c16eca58f45b2e481e3cb2b89136fbcb893d3553a5877ff0bdf2594ad3dbcc87`  
		Last Modified: Fri, 13 Aug 2021 00:08:36 GMT  
		Size: 25.2 MB (25161605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8172bac02c8635308fad1099bcd8ccb8d90ad814c0d9251d741d3a1939f464b`  
		Last Modified: Fri, 13 Aug 2021 00:08:18 GMT  
		Size: 7.7 KB (7732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e38ac356b23a03818091e242c051e1219351471f1933b32b6fe69bfe94a4984`  
		Last Modified: Fri, 13 Aug 2021 00:08:18 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41ae60c8a48fc3927cf6a5bfd9af001eead463f0e378408ca8ca3bc552b8fd4a`  
		Last Modified: Fri, 13 Aug 2021 00:08:18 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a02ba41ffd4fae2273dfca624d274d05635102376e8d5c7a0bc0506e9524380e`  
		Last Modified: Fri, 13 Aug 2021 00:08:18 GMT  
		Size: 4.4 KB (4406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72143bb504e3401dc34b8c06a5a8c73e21684b4e2f9fb784eb820ce04a4d6e68`  
		Last Modified: Fri, 13 Aug 2021 00:08:18 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:10-alpine3.14` - linux; arm variant v7

```console
$ docker pull postgres@sha256:ab619d147ad54a415fd1abcb2a0a41bb5dc29f926dbf6ed2bd2ba44fbeeacf01
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.7 MB (26727439 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d177a9b7fbf42af211b7647c730e91acda62d6d6d3b650ed8ea0cb56c9260ba7`
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
# Sat, 07 Aug 2021 01:28:55 GMT
ENV PG_MAJOR=10
# Fri, 13 Aug 2021 04:14:21 GMT
ENV PG_VERSION=10.18
# Fri, 13 Aug 2021 04:14:22 GMT
ENV PG_SHA256=57477c2edc82c3f86a74747707b3babc1f301f389315ae14e819e025c0ba3801
# Fri, 13 Aug 2021 04:17:56 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Fri, 13 Aug 2021 04:17:58 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample
# Fri, 13 Aug 2021 04:18:00 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 13 Aug 2021 04:18:00 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 13 Aug 2021 04:18:02 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 13 Aug 2021 04:18:02 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 13 Aug 2021 04:18:03 GMT
COPY file:ad28506adc606e446eefc263bc99d4cb809e608d4f550956143bf13c82c91f85 in /usr/local/bin/ 
# Fri, 13 Aug 2021 04:18:04 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 13 Aug 2021 04:18:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 13 Aug 2021 04:18:05 GMT
STOPSIGNAL SIGINT
# Fri, 13 Aug 2021 04:18:06 GMT
EXPOSE 5432
# Fri, 13 Aug 2021 04:18:06 GMT
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
	-	`sha256:053948a232f8220d6b3b8366f5451b46a297e60c6a53362f0a8ad756a8e63450`  
		Last Modified: Fri, 13 Aug 2021 05:21:04 GMT  
		Size: 24.3 MB (24284036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f61aecca702ed78e55a136d8fbf25019d1f4e31617b8d9e09d7bb32c3ee455df`  
		Last Modified: Fri, 13 Aug 2021 05:20:47 GMT  
		Size: 7.7 KB (7730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f6115e62dc8b8699c64df8d58b6d09a1462f76709e30d504c295eeb2da5bb8c`  
		Last Modified: Fri, 13 Aug 2021 05:20:47 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd044ff71f4295bc626640ca8ce4ef53dec250d2a00082ec0fda58a58a53d892`  
		Last Modified: Fri, 13 Aug 2021 05:20:47 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e83720ae7adc37ac16794a03c8a3ba07ed0d69fb31cc1088866646d42b78a32f`  
		Last Modified: Fri, 13 Aug 2021 05:20:47 GMT  
		Size: 4.4 KB (4405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4df4a56f809ad8a31a9f0d16a082d1f63c3e69234a8873194f1b94455b262fb`  
		Last Modified: Fri, 13 Aug 2021 05:20:47 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:10-alpine3.14` - linux; arm64 variant v8

```console
$ docker pull postgres@sha256:39a516c43d65c492826dee037bf3fae034ad35f298a70badc16dfc7bf066ae11
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.4 MB (28362215 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9240700402e75a8961e84071b1f50dc95827e58ae6aefd5970cb521229f6ea60`
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
# Sat, 07 Aug 2021 00:38:06 GMT
ENV PG_MAJOR=10
# Fri, 13 Aug 2021 03:47:27 GMT
ENV PG_VERSION=10.18
# Fri, 13 Aug 2021 03:47:27 GMT
ENV PG_SHA256=57477c2edc82c3f86a74747707b3babc1f301f389315ae14e819e025c0ba3801
# Fri, 13 Aug 2021 03:50:34 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Fri, 13 Aug 2021 03:50:35 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample
# Fri, 13 Aug 2021 03:50:35 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 13 Aug 2021 03:50:36 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 13 Aug 2021 03:50:36 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 13 Aug 2021 03:50:37 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 13 Aug 2021 03:50:37 GMT
COPY file:ad28506adc606e446eefc263bc99d4cb809e608d4f550956143bf13c82c91f85 in /usr/local/bin/ 
# Fri, 13 Aug 2021 03:50:37 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 13 Aug 2021 03:50:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 13 Aug 2021 03:50:38 GMT
STOPSIGNAL SIGINT
# Fri, 13 Aug 2021 03:50:38 GMT
EXPOSE 5432
# Fri, 13 Aug 2021 03:50:38 GMT
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
	-	`sha256:009949f52d6714541cc540e26575dc82ab05eb6ed44ed2b5b3674e31ba74b4e9`  
		Last Modified: Fri, 13 Aug 2021 04:11:14 GMT  
		Size: 25.6 MB (25637559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f47a66ae0cf6063afa840e6d76c17ebafe83c94d177400073d3a4e139ebcc2e`  
		Last Modified: Fri, 13 Aug 2021 04:11:07 GMT  
		Size: 7.7 KB (7730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29a60b61a06df67c064c11cc4521c6d9f3f742d688185606ab1b1e39f9293a43`  
		Last Modified: Fri, 13 Aug 2021 04:11:07 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0f2a8f65fda79c9658dde6cea16d286d612966a2332ad3ed9cd6145f34fc4e5`  
		Last Modified: Fri, 13 Aug 2021 04:11:07 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9837acdeb334de7c57be7d4074a18c1f13e74d146db475722c89a878d72145b1`  
		Last Modified: Fri, 13 Aug 2021 04:11:07 GMT  
		Size: 4.4 KB (4403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:908d55eb9ac3ec51694f35b21d2eb898bc12c9908d6d26989fbf709f83858e61`  
		Last Modified: Fri, 13 Aug 2021 04:11:07 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:10-alpine3.14` - linux; 386

```console
$ docker pull postgres@sha256:b065d7b19b6044a1fd434d9c7fd71edfdb2e256473fae928c1cebed8e6279100
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.6 MB (29560058 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:afb4f32cc8608b425bb56ff0da6b166b42c5a036c6ec63594fd53b1292e7ddce`
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
# Fri, 06 Aug 2021 22:12:59 GMT
ENV PG_MAJOR=10
# Thu, 12 Aug 2021 21:18:35 GMT
ENV PG_VERSION=10.18
# Thu, 12 Aug 2021 21:18:35 GMT
ENV PG_SHA256=57477c2edc82c3f86a74747707b3babc1f301f389315ae14e819e025c0ba3801
# Thu, 12 Aug 2021 21:22:23 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Thu, 12 Aug 2021 21:22:24 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample
# Thu, 12 Aug 2021 21:22:24 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 12 Aug 2021 21:22:25 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 12 Aug 2021 21:22:26 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 12 Aug 2021 21:22:26 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 12 Aug 2021 21:22:26 GMT
COPY file:ad28506adc606e446eefc263bc99d4cb809e608d4f550956143bf13c82c91f85 in /usr/local/bin/ 
# Thu, 12 Aug 2021 21:22:27 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 12 Aug 2021 21:22:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 12 Aug 2021 21:22:27 GMT
STOPSIGNAL SIGINT
# Thu, 12 Aug 2021 21:22:27 GMT
EXPOSE 5432
# Thu, 12 Aug 2021 21:22:28 GMT
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
	-	`sha256:dd580d09385f6216ee84421f4b951c8526b6684bd27bfc89f35c54e98a8b8ff5`  
		Last Modified: Thu, 12 Aug 2021 21:35:53 GMT  
		Size: 26.7 MB (26724102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:074dd0a8e574d6634fbe4e1d062902d3123d8babc6b6e614d0e13e8cc97b8554`  
		Last Modified: Thu, 12 Aug 2021 21:35:45 GMT  
		Size: 7.7 KB (7732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32324d5b8e53eb995533b1ba543fb0b95b44ff45dedf514f30b65054f643d66f`  
		Last Modified: Thu, 12 Aug 2021 21:35:45 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b13a0a819c22b4a34edeabcef4b690dc16ac80b34efb9a48d99fbd152fcaddcf`  
		Last Modified: Thu, 12 Aug 2021 21:35:45 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c0369dca87dc6227edc6ac1022324150cb8504729a7283e4d343517350bb92e`  
		Last Modified: Thu, 12 Aug 2021 21:35:45 GMT  
		Size: 4.4 KB (4404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b6d651e017a5cd0fc12090a45436dabd6331d92ae7beb3782ca6a614a532f55`  
		Last Modified: Thu, 12 Aug 2021 21:35:45 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:10-alpine3.14` - linux; ppc64le

```console
$ docker pull postgres@sha256:ba249f2ec06a85040bb69113f59e39df9215097c639d4a3c99466546311e0aba
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.0 MB (29953441 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0b779b0cc2a1f882f1c61f4cd92841a012e645d9d93fae2f11c6fc42856d635`
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
# Sat, 07 Aug 2021 01:03:08 GMT
ENV PG_MAJOR=10
# Fri, 13 Aug 2021 00:47:05 GMT
ENV PG_VERSION=10.18
# Fri, 13 Aug 2021 00:47:12 GMT
ENV PG_SHA256=57477c2edc82c3f86a74747707b3babc1f301f389315ae14e819e025c0ba3801
# Fri, 13 Aug 2021 00:50:05 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Fri, 13 Aug 2021 00:50:14 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample
# Fri, 13 Aug 2021 00:50:21 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 13 Aug 2021 00:50:31 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 13 Aug 2021 00:50:40 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 13 Aug 2021 00:50:43 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 13 Aug 2021 00:50:46 GMT
COPY file:ad28506adc606e446eefc263bc99d4cb809e608d4f550956143bf13c82c91f85 in /usr/local/bin/ 
# Fri, 13 Aug 2021 00:50:55 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 13 Aug 2021 00:51:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 13 Aug 2021 00:51:08 GMT
STOPSIGNAL SIGINT
# Fri, 13 Aug 2021 00:51:13 GMT
EXPOSE 5432
# Fri, 13 Aug 2021 00:51:17 GMT
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
	-	`sha256:0ec9a5efccea9fcdebc47c4dde19bc224429f07e6f4734c60cf2abd237c25c39`  
		Last Modified: Fri, 13 Aug 2021 01:06:50 GMT  
		Size: 27.1 MB (27128250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83cce1c7e318a2e08ba9f6c8f9242c387013fe2b59c3e083fac5a77913b8d82c`  
		Last Modified: Fri, 13 Aug 2021 01:06:42 GMT  
		Size: 7.7 KB (7731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76d954781f96e9323b85541d3bbccf96b53caa62ef5b4c21a825fec7d26e64a6`  
		Last Modified: Fri, 13 Aug 2021 01:06:42 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:453f816235499318e0c01e163be4c12efb43dd0bb2039ec1df4293bd2c33b172`  
		Last Modified: Fri, 13 Aug 2021 01:06:42 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b321056c8055109fc52ec9c05553c1f3a280d50e87ef50ad31c4479b3c6b4f1`  
		Last Modified: Fri, 13 Aug 2021 01:06:42 GMT  
		Size: 4.4 KB (4402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffda10fb728be89f32c5e8586d0b554b22989fe93657e2a8f9506aa36e6aec8e`  
		Last Modified: Fri, 13 Aug 2021 01:06:41 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:10-alpine3.14` - linux; s390x

```console
$ docker pull postgres@sha256:8fe4c2558e1798a52746d96eca254398169bf9f03a4ff209e42a19987767590a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.5 MB (28503092 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8a56e1b451f6eac221094deeefa643366969f8755df07ee22f1b73bb2186e1f`
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
# Fri, 06 Aug 2021 20:04:04 GMT
ENV PG_MAJOR=10
# Fri, 13 Aug 2021 01:38:52 GMT
ENV PG_VERSION=10.18
# Fri, 13 Aug 2021 01:38:52 GMT
ENV PG_SHA256=57477c2edc82c3f86a74747707b3babc1f301f389315ae14e819e025c0ba3801
# Sat, 21 Aug 2021 03:33:38 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Sat, 21 Aug 2021 03:33:43 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample
# Sat, 21 Aug 2021 03:33:45 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Sat, 21 Aug 2021 03:33:45 GMT
ENV PGDATA=/var/lib/postgresql/data
# Sat, 21 Aug 2021 03:33:46 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Sat, 21 Aug 2021 03:33:47 GMT
VOLUME [/var/lib/postgresql/data]
# Sat, 21 Aug 2021 03:33:47 GMT
COPY file:ad28506adc606e446eefc263bc99d4cb809e608d4f550956143bf13c82c91f85 in /usr/local/bin/ 
# Sat, 21 Aug 2021 03:33:48 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 21 Aug 2021 03:33:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 21 Aug 2021 03:33:49 GMT
STOPSIGNAL SIGINT
# Sat, 21 Aug 2021 03:33:50 GMT
EXPOSE 5432
# Sat, 21 Aug 2021 03:33:50 GMT
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
	-	`sha256:430d1e0e612fee4757857c1b26231ce2a16cff2e0928d358d9603511f3557717`  
		Last Modified: Sat, 21 Aug 2021 03:41:56 GMT  
		Size: 25.9 MB (25887021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:894d6c0c5fe027723cbfe5af0d158078c09d3b96dc8c6ec339e3d5c7da29f7f6`  
		Last Modified: Sat, 21 Aug 2021 03:41:51 GMT  
		Size: 7.7 KB (7724 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f9c7f3779f07abd5d121e260c5c55c2a902a7ef0d6508a92782bba3be8c0896`  
		Last Modified: Sat, 21 Aug 2021 03:41:51 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d67f6dde02ff7b1b127139a4e19f144d45ade8bf23c5d9f258602919793a792c`  
		Last Modified: Sat, 21 Aug 2021 03:41:51 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d16e306179eb80146c607dc71bab09b9a32504c5a336f7ae0ddbb4f8c90ed42`  
		Last Modified: Sat, 21 Aug 2021 03:41:51 GMT  
		Size: 4.4 KB (4404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e54a323925795bf347e06d5f6617ec6d3748a624d6fa1110dc58d8ea6914886`  
		Last Modified: Sat, 21 Aug 2021 03:41:51 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
