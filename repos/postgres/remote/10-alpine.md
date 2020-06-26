## `postgres:10-alpine`

```console
$ docker pull postgres@sha256:3bb8275aaf7704cdde352ebf29675799cbf6a8391b1fbace057eea7f33d52162
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `postgres:10-alpine` - linux; amd64

```console
$ docker pull postgres@sha256:ad8e2879d680e47002add46152fd81d30790f54841b994399153fefb9c0d613a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.5 MB (28520472 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1adeb2c0300781b7805b15763e9b0bcc5a6ca4d407e98078a949faeabf548c11`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Fri, 29 May 2020 21:19:46 GMT
ADD file:c92c248239f8c7b9b3c067650954815f391b7bcb09023f984972c082ace2a8d0 in / 
# Fri, 29 May 2020 21:19:46 GMT
CMD ["/bin/sh"]
# Thu, 11 Jun 2020 22:46:48 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 11 Jun 2020 22:46:48 GMT
ENV LANG=en_US.utf8
# Thu, 11 Jun 2020 22:46:49 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 11 Jun 2020 23:13:43 GMT
ENV PG_MAJOR=10
# Thu, 11 Jun 2020 23:13:43 GMT
ENV PG_VERSION=10.13
# Thu, 11 Jun 2020 23:13:43 GMT
ENV PG_SHA256=4d701f450cd92ffb123cf6c296e9656abbc2ab7ea6507894ff1e2475ae0754e1
# Fri, 26 Jun 2020 21:04:31 GMT
RUN set -ex 		&& wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2" 	&& echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c - 	&& mkdir -p /usr/src/postgresql 	&& tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	&& rm postgresql.tar.bz2 		&& apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 		&& cd /usr/src/postgresql 	&& awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new 	&& grep '/var/run/postgresql' src/include/pg_config_manual.h.new 	&& mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& ./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 	&& make -j "$(nproc)" world 	&& make install-world 	&& make -C contrib install 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	&& apk del --no-network .build-deps 	&& cd / 	&& rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	&& find /usr/local -name '*.a' -delete
# Fri, 26 Jun 2020 21:04:32 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Fri, 26 Jun 2020 21:04:32 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 26 Jun 2020 21:04:33 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 26 Jun 2020 21:04:33 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 26 Jun 2020 21:04:33 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 26 Jun 2020 21:04:34 GMT
COPY file:33e6fc6ab9ea2b87183e496ad72f1df7f682913ffd781b1451fd178b0c7d745a in /usr/local/bin/ 
# Fri, 26 Jun 2020 21:04:34 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 26 Jun 2020 21:04:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Jun 2020 21:04:35 GMT
EXPOSE 5432
# Fri, 26 Jun 2020 21:04:35 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:df20fa9351a15782c64e6dddb2d4a6f50bf6d3688060a34c4014b0d9a752eb4c`  
		Last Modified: Fri, 29 May 2020 21:20:06 GMT  
		Size: 2.8 MB (2797541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:600cd4e17445b526dc093ca716d204a866349e5c7228251e31178e81371c47ff`  
		Last Modified: Thu, 11 Jun 2020 23:28:47 GMT  
		Size: 1.2 KB (1248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04c8eedc9a7657acd81498f6619dffcb88d9a150879f9ec0cc358834aa84aaf7`  
		Last Modified: Thu, 11 Jun 2020 23:28:47 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b767fa5ba60657f4381645772d60704611a9a164f9a979b1139a9866a2b2d11c`  
		Last Modified: Fri, 26 Jun 2020 21:15:50 GMT  
		Size: 25.7 MB (25709539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:accbaf05ced2c12b410418767be906368fa2b027a4acc8683311f0248930490a`  
		Last Modified: Fri, 26 Jun 2020 21:15:43 GMT  
		Size: 7.4 KB (7355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7be7413903a779d87bce5df9afc4175917016da43f9b6a1baa8ddf311f90cf40`  
		Last Modified: Fri, 26 Jun 2020 21:15:43 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:574f51692c839b23027d4e96ea581f151c67e79a9c491e3acf593a7d443d726c`  
		Last Modified: Fri, 26 Jun 2020 21:15:43 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1ab0e63265492b870d0f8d59906f80440f6e8b093dcd85210fec4c85617d221`  
		Last Modified: Fri, 26 Jun 2020 21:15:43 GMT  
		Size: 4.3 KB (4261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22d3ba89c4f27af12b18b007472b0866ee574479aebb923163d1e616a797d7e0`  
		Last Modified: Fri, 26 Jun 2020 21:15:43 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:10-alpine` - linux; arm variant v6

```console
$ docker pull postgres@sha256:0f4cfdf50bf8fba92bca4c7644b99ccb60261a53b762aba788af7534971681aa
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.6 MB (27639005 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6ebdb4791b97854ea0f4ba96526f42806f1bacfaa9ae1e534526cbf4b8b8f68b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Fri, 29 May 2020 21:50:55 GMT
ADD file:f46e997a56849423db17e5fc9f0249ab6c73b155245927dba5fcb9dfd65f622f in / 
# Fri, 29 May 2020 21:50:56 GMT
CMD ["/bin/sh"]
# Thu, 11 Jun 2020 20:27:27 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 11 Jun 2020 20:27:28 GMT
ENV LANG=en_US.utf8
# Thu, 11 Jun 2020 20:27:30 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 11 Jun 2020 20:41:34 GMT
ENV PG_MAJOR=10
# Thu, 11 Jun 2020 20:41:35 GMT
ENV PG_VERSION=10.13
# Thu, 11 Jun 2020 20:41:35 GMT
ENV PG_SHA256=4d701f450cd92ffb123cf6c296e9656abbc2ab7ea6507894ff1e2475ae0754e1
# Fri, 26 Jun 2020 19:50:49 GMT
RUN set -ex 		&& wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2" 	&& echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c - 	&& mkdir -p /usr/src/postgresql 	&& tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	&& rm postgresql.tar.bz2 		&& apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 		&& cd /usr/src/postgresql 	&& awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new 	&& grep '/var/run/postgresql' src/include/pg_config_manual.h.new 	&& mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& ./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 	&& make -j "$(nproc)" world 	&& make install-world 	&& make -C contrib install 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	&& apk del --no-network .build-deps 	&& cd / 	&& rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	&& find /usr/local -name '*.a' -delete
# Fri, 26 Jun 2020 19:50:52 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Fri, 26 Jun 2020 19:50:54 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 26 Jun 2020 19:50:55 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 26 Jun 2020 19:50:57 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 26 Jun 2020 19:50:58 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 26 Jun 2020 19:50:59 GMT
COPY file:33e6fc6ab9ea2b87183e496ad72f1df7f682913ffd781b1451fd178b0c7d745a in /usr/local/bin/ 
# Fri, 26 Jun 2020 19:51:02 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 26 Jun 2020 19:51:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Jun 2020 19:51:05 GMT
EXPOSE 5432
# Fri, 26 Jun 2020 19:51:06 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:b4b72e716706d29f5d2351709c20bf737b94f876a5472a43ff1b6e203c65d27f`  
		Last Modified: Fri, 29 May 2020 21:51:30 GMT  
		Size: 2.6 MB (2603286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e0c6822b30b82f1bf3837b7d730cf7d68d7101602023fc38fb839cf826a5bd6`  
		Last Modified: Thu, 11 Jun 2020 20:52:06 GMT  
		Size: 1.3 KB (1279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcc1c5a5bbcba93ab5809dbcc58c6042d7a9983681f6a6f951d947b0d4d0c3b5`  
		Last Modified: Thu, 11 Jun 2020 20:52:06 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd194797cc7b995d0c92cc8b48f23c526c3c25c5dc75c3676869e9920f371af0`  
		Last Modified: Fri, 26 Jun 2020 19:59:31 GMT  
		Size: 25.0 MB (25022196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a20f9f4d5135e3bdf950e029a52bc89d252b49505e41dcf532f2512996ae018`  
		Last Modified: Fri, 26 Jun 2020 19:59:21 GMT  
		Size: 7.4 KB (7357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a076223af14de2bc9614897fbaad2b7a9a23315c7997b10288248ba4f116019`  
		Last Modified: Fri, 26 Jun 2020 19:59:21 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74f85781bd820de607a61886a5c2b9d075ba593e1e9b6154fa222d99937259c5`  
		Last Modified: Fri, 26 Jun 2020 19:59:21 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecb74ae10e42eba0c8eaa9cf4fa842cd280a28a83eb323244cf8f68011923c00`  
		Last Modified: Fri, 26 Jun 2020 19:59:22 GMT  
		Size: 4.3 KB (4261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f4962327583146068708d04fd532d46397275f4a2050b3ea14a43361f6ec3b4`  
		Last Modified: Fri, 26 Jun 2020 19:59:21 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:10-alpine` - linux; arm variant v7

```console
$ docker pull postgres@sha256:1b6e8a6cda4548a97b50d43e9a6f2c1c2c6c7eefe64f3b77e51d670150154d48
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.6 MB (26583697 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c400f1d3e02bee90de47bf50791385f7decfa8a4cad2a4f53b85520ae37b79f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Fri, 29 May 2020 21:02:07 GMT
ADD file:e97bf0d217846312b19a9f7264604851aedd125c23b4d291eed4c69b880dce26 in / 
# Fri, 29 May 2020 21:02:08 GMT
CMD ["/bin/sh"]
# Thu, 11 Jun 2020 20:43:57 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 11 Jun 2020 20:43:58 GMT
ENV LANG=en_US.utf8
# Thu, 11 Jun 2020 20:44:01 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 11 Jun 2020 20:55:49 GMT
ENV PG_MAJOR=10
# Thu, 11 Jun 2020 20:55:57 GMT
ENV PG_VERSION=10.13
# Thu, 11 Jun 2020 20:56:00 GMT
ENV PG_SHA256=4d701f450cd92ffb123cf6c296e9656abbc2ab7ea6507894ff1e2475ae0754e1
# Fri, 26 Jun 2020 19:39:06 GMT
RUN set -ex 		&& wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2" 	&& echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c - 	&& mkdir -p /usr/src/postgresql 	&& tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	&& rm postgresql.tar.bz2 		&& apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 		&& cd /usr/src/postgresql 	&& awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new 	&& grep '/var/run/postgresql' src/include/pg_config_manual.h.new 	&& mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& ./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 	&& make -j "$(nproc)" world 	&& make install-world 	&& make -C contrib install 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	&& apk del --no-network .build-deps 	&& cd / 	&& rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	&& find /usr/local -name '*.a' -delete
# Fri, 26 Jun 2020 19:39:15 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Fri, 26 Jun 2020 19:39:23 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 26 Jun 2020 19:39:25 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 26 Jun 2020 19:39:33 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 26 Jun 2020 19:39:38 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 26 Jun 2020 19:39:41 GMT
COPY file:33e6fc6ab9ea2b87183e496ad72f1df7f682913ffd781b1451fd178b0c7d745a in /usr/local/bin/ 
# Fri, 26 Jun 2020 19:39:50 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 26 Jun 2020 19:39:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Jun 2020 19:39:54 GMT
EXPOSE 5432
# Fri, 26 Jun 2020 19:39:57 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:52278dd8e57993669c5b72a9620e89bebdc098f2af2379caaa8945f7403f77a2`  
		Last Modified: Fri, 29 May 2020 21:02:38 GMT  
		Size: 2.4 MB (2406763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcd3f931b2a724d22b1f76af233e84a5d592aa2a21caad88700c700ef28bec95`  
		Last Modified: Thu, 11 Jun 2020 21:05:18 GMT  
		Size: 1.3 KB (1274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19f754b96158415f11b928d9d9e9f98a8cd305f2a033ef0b4c6e7bfe6645b508`  
		Last Modified: Thu, 11 Jun 2020 21:05:18 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cf88a03da08a155f6bd3436b760f129a0ecfceb10461ebf0922d71669ac18f9`  
		Last Modified: Fri, 26 Jun 2020 19:49:16 GMT  
		Size: 24.2 MB (24163415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d99d91e06c1cf65aa875d9d3bfeba4ea9ebee72335198a9d795f3b39712d914e`  
		Last Modified: Fri, 26 Jun 2020 19:49:08 GMT  
		Size: 7.4 KB (7357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd497c1f723440e6facd32c29d859c748ca913844d07dac022330b6897363b67`  
		Last Modified: Fri, 26 Jun 2020 19:49:08 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aab4deb78c734ffc512c9c123eb0c978a572ee1f3e37f660086fafc9ce27badc`  
		Last Modified: Fri, 26 Jun 2020 19:49:08 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:744827c13f06e814481921c384b30815e64123b035e667c40de61ef3bb320688`  
		Last Modified: Fri, 26 Jun 2020 19:49:08 GMT  
		Size: 4.3 KB (4260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d08e2b701362d7adb0f5b31c9599dbd31e489a500e1e9135af423ed168f9cfc7`  
		Last Modified: Fri, 26 Jun 2020 19:49:08 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:10-alpine` - linux; arm64 variant v8

```console
$ docker pull postgres@sha256:7daf62c36e1af8e83ebdaacc596b12a841019383df114fae021ce085cdf53de5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.3 MB (28286269 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c337116dd0ec79d96ef5a38e0512fac5654a97c6196f10597b89b5959cad5b4d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Fri, 29 May 2020 21:43:19 GMT
ADD file:7574aee4e37a85460ab889212d52912723a9b30dda1c060548f0deb4a05fc398 in / 
# Fri, 29 May 2020 21:43:20 GMT
CMD ["/bin/sh"]
# Thu, 11 Jun 2020 21:06:12 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 11 Jun 2020 21:06:13 GMT
ENV LANG=en_US.utf8
# Thu, 11 Jun 2020 21:06:16 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 11 Jun 2020 21:31:48 GMT
ENV PG_MAJOR=10
# Thu, 11 Jun 2020 21:31:49 GMT
ENV PG_VERSION=10.13
# Thu, 11 Jun 2020 21:31:50 GMT
ENV PG_SHA256=4d701f450cd92ffb123cf6c296e9656abbc2ab7ea6507894ff1e2475ae0754e1
# Fri, 26 Jun 2020 20:54:30 GMT
RUN set -ex 		&& wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2" 	&& echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c - 	&& mkdir -p /usr/src/postgresql 	&& tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	&& rm postgresql.tar.bz2 		&& apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 		&& cd /usr/src/postgresql 	&& awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new 	&& grep '/var/run/postgresql' src/include/pg_config_manual.h.new 	&& mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& ./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 	&& make -j "$(nproc)" world 	&& make install-world 	&& make -C contrib install 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	&& apk del --no-network .build-deps 	&& cd / 	&& rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	&& find /usr/local -name '*.a' -delete
# Fri, 26 Jun 2020 20:54:33 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Fri, 26 Jun 2020 20:54:36 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 26 Jun 2020 20:54:37 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 26 Jun 2020 20:54:40 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 26 Jun 2020 20:54:42 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 26 Jun 2020 20:54:43 GMT
COPY file:33e6fc6ab9ea2b87183e496ad72f1df7f682913ffd781b1451fd178b0c7d745a in /usr/local/bin/ 
# Fri, 26 Jun 2020 20:54:45 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 26 Jun 2020 20:54:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Jun 2020 20:54:47 GMT
EXPOSE 5432
# Fri, 26 Jun 2020 20:54:48 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:b538f80385f9b48122e3da068c932a96ea5018afa3c7be79da00437414bd18cd`  
		Last Modified: Fri, 29 May 2020 21:43:57 GMT  
		Size: 2.7 MB (2707964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9d4833cc285b7342c1d7bab9159e04f3cb6d84914e4a6376bd605ef138613aa`  
		Last Modified: Thu, 11 Jun 2020 21:41:31 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bf1f783f6dc9622807ab9414bb09346699c6eea41fd6260efcfe679699f206d`  
		Last Modified: Thu, 11 Jun 2020 21:41:31 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd46bfb4fe09c2238640344050b2a3054a237cf59eb4116e3b60cca99af10709`  
		Last Modified: Fri, 26 Jun 2020 21:03:23 GMT  
		Size: 25.6 MB (25564781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:833d201925497de1bfc3e4e2d8c65f8d065c4d5c99c6b6a0ce0da2595423618c`  
		Last Modified: Fri, 26 Jun 2020 21:03:15 GMT  
		Size: 7.4 KB (7353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9063d2f23decd2d3386d9973164d5012800dba6027a94d329a6635a7adcf769c`  
		Last Modified: Fri, 26 Jun 2020 21:03:14 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b526f26791f36543bd5db4f565abb38b0435282b92ea97abc2d65ce6aa105c8`  
		Last Modified: Fri, 26 Jun 2020 21:03:14 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cccf499adf1a34623dfc930a8f76f3e4515afaec1c560c89503f68a9898286a6`  
		Last Modified: Fri, 26 Jun 2020 21:03:14 GMT  
		Size: 4.3 KB (4264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe082d273977ed59b78b542e8babf171efcd5440ea6582a417df540cb1f09327`  
		Last Modified: Fri, 26 Jun 2020 21:03:14 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:10-alpine` - linux; 386

```console
$ docker pull postgres@sha256:c397de2337ecb265bf88bffd502cfa8097a8cd4db40d5c256e74a13f2a424f78
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.4 MB (29396078 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dc0d7645e9e8d242b64871c839c87d54539c146924fb154fa11bdff29d1b543d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Fri, 29 May 2020 21:38:33 GMT
ADD file:5624441d97aca5eeb82a582941efc3586397098b8391227a9040ebe434cc1d6b in / 
# Fri, 29 May 2020 21:38:33 GMT
CMD ["/bin/sh"]
# Thu, 11 Jun 2020 23:02:21 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 11 Jun 2020 23:02:22 GMT
ENV LANG=en_US.utf8
# Thu, 11 Jun 2020 23:02:23 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 11 Jun 2020 23:35:36 GMT
ENV PG_MAJOR=10
# Thu, 11 Jun 2020 23:35:37 GMT
ENV PG_VERSION=10.13
# Thu, 11 Jun 2020 23:35:37 GMT
ENV PG_SHA256=4d701f450cd92ffb123cf6c296e9656abbc2ab7ea6507894ff1e2475ae0754e1
# Fri, 26 Jun 2020 22:43:10 GMT
RUN set -ex 		&& wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2" 	&& echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c - 	&& mkdir -p /usr/src/postgresql 	&& tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	&& rm postgresql.tar.bz2 		&& apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 		&& cd /usr/src/postgresql 	&& awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new 	&& grep '/var/run/postgresql' src/include/pg_config_manual.h.new 	&& mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& ./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 	&& make -j "$(nproc)" world 	&& make install-world 	&& make -C contrib install 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	&& apk del --no-network .build-deps 	&& cd / 	&& rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	&& find /usr/local -name '*.a' -delete
# Fri, 26 Jun 2020 22:43:11 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Fri, 26 Jun 2020 22:43:12 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 26 Jun 2020 22:43:12 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 26 Jun 2020 22:43:13 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 26 Jun 2020 22:43:13 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 26 Jun 2020 22:43:14 GMT
COPY file:33e6fc6ab9ea2b87183e496ad72f1df7f682913ffd781b1451fd178b0c7d745a in /usr/local/bin/ 
# Fri, 26 Jun 2020 22:43:14 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 26 Jun 2020 22:43:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Jun 2020 22:43:15 GMT
EXPOSE 5432
# Fri, 26 Jun 2020 22:43:15 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:0625b4155e2a59f647ece47c0cd77ed3196b1f84454fa64ce80cad90e2b9b79e`  
		Last Modified: Fri, 29 May 2020 21:38:53 GMT  
		Size: 2.8 MB (2792298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c748d368bf108a32daf0810b28e1996f37eca0dfed0dac7c8c2598e6c6029748`  
		Last Modified: Thu, 11 Jun 2020 23:54:07 GMT  
		Size: 1.2 KB (1249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b0010b2123bc87ca763bce1e85a2350a168ce13065a7ae9b47e6ed49fa4b72d`  
		Last Modified: Thu, 11 Jun 2020 23:54:07 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd58e8f2ee4d2520d670d3e662865632f1fd36deec830ec6f6d748f74d1afeb8`  
		Last Modified: Fri, 26 Jun 2020 22:54:49 GMT  
		Size: 26.6 MB (26590388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3290046d870d63a7c0754e849a0a67d160d06e16d63b3391d056a9f09c08ea0`  
		Last Modified: Fri, 26 Jun 2020 22:54:41 GMT  
		Size: 7.4 KB (7352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bef1d7bf6178be04545283a10df7aaf44526969e6ffa38a83ae0d99d5d8f425`  
		Last Modified: Fri, 26 Jun 2020 22:54:41 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9b47cb70a83e083024ff169692c4c0d604018c452bc0f2358be332a1959c3fd`  
		Last Modified: Fri, 26 Jun 2020 22:54:41 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7daf05657b3e25eea9eb290e9f173db35817f8adbdb8f03ddf9dcfab7fe34282`  
		Last Modified: Fri, 26 Jun 2020 22:54:41 GMT  
		Size: 4.3 KB (4263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:674c82e37e165b6939b27a731da76a72955b5a218f014da8a8d3a8f1abf68f0d`  
		Last Modified: Fri, 26 Jun 2020 22:54:41 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:10-alpine` - linux; ppc64le

```console
$ docker pull postgres@sha256:fd35b083c317a3deef16263877d2a52d4b381a857b4c75e54d76abcce078e2b9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.6 MB (29615110 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2cafc8d8f341ba8c4b5854ec633a97999a6191b811c5773d79dafd48ed5a4b57`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Fri, 29 May 2020 21:23:03 GMT
ADD file:8194808a812370fd2202d80d1667f851bd9eac4c560d69d347fe1964f54343de in / 
# Fri, 29 May 2020 21:23:06 GMT
CMD ["/bin/sh"]
# Thu, 11 Jun 2020 21:40:53 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 11 Jun 2020 21:40:56 GMT
ENV LANG=en_US.utf8
# Thu, 11 Jun 2020 21:41:01 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 11 Jun 2020 21:54:59 GMT
ENV PG_MAJOR=10
# Thu, 11 Jun 2020 21:55:01 GMT
ENV PG_VERSION=10.13
# Thu, 11 Jun 2020 21:55:03 GMT
ENV PG_SHA256=4d701f450cd92ffb123cf6c296e9656abbc2ab7ea6507894ff1e2475ae0754e1
# Fri, 26 Jun 2020 20:35:38 GMT
RUN set -ex 		&& wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2" 	&& echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c - 	&& mkdir -p /usr/src/postgresql 	&& tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	&& rm postgresql.tar.bz2 		&& apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 		&& cd /usr/src/postgresql 	&& awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new 	&& grep '/var/run/postgresql' src/include/pg_config_manual.h.new 	&& mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& ./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 	&& make -j "$(nproc)" world 	&& make install-world 	&& make -C contrib install 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	&& apk del --no-network .build-deps 	&& cd / 	&& rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	&& find /usr/local -name '*.a' -delete
# Fri, 26 Jun 2020 20:35:47 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Fri, 26 Jun 2020 20:35:55 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 26 Jun 2020 20:35:57 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 26 Jun 2020 20:36:05 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 26 Jun 2020 20:36:08 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 26 Jun 2020 20:36:09 GMT
COPY file:33e6fc6ab9ea2b87183e496ad72f1df7f682913ffd781b1451fd178b0c7d745a in /usr/local/bin/ 
# Fri, 26 Jun 2020 20:36:17 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 26 Jun 2020 20:36:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Jun 2020 20:36:24 GMT
EXPOSE 5432
# Fri, 26 Jun 2020 20:36:30 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:5077f8601dceb5744d875d7740ebc203f674b108a0188f3a31e292b21a4bee64`  
		Last Modified: Fri, 29 May 2020 21:23:37 GMT  
		Size: 2.8 MB (2805199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a9f72d45e54d4dd62def75147b46a533078a8d2923214d24a8e89d83d426c84`  
		Last Modified: Thu, 11 Jun 2020 22:06:29 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d870eff785c52b89df973046311ce60ebdc465c597c3268e41f87f0e4e645ef`  
		Last Modified: Thu, 11 Jun 2020 22:06:29 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90a7d9842232016adda21238ac484d0f956d09b15413e983817fced1e9ca0410`  
		Last Modified: Fri, 26 Jun 2020 20:46:59 GMT  
		Size: 26.8 MB (26796389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63e3e7d996ef802ef6409fed1d1eded745de90376f89fd726576ea221fea3019`  
		Last Modified: Fri, 26 Jun 2020 20:46:51 GMT  
		Size: 7.4 KB (7354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:538b7667f7a0d439e27aee546dd792c64d86fcbf3a053c190a7ebd9d62b28c51`  
		Last Modified: Fri, 26 Jun 2020 20:46:51 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd5ba2ea1922ab70aa33a13d985beae4bee75b7378192fc5d5eb297e80134085`  
		Last Modified: Fri, 26 Jun 2020 20:46:51 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3cb5d88a76eee920ed7c1e447941f1d06c00f9e80765572a53cf829ff6da08e`  
		Last Modified: Fri, 26 Jun 2020 20:46:51 GMT  
		Size: 4.3 KB (4259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aad2e740d29a6555d38fb484a0b8989fca70a0040ec50e9172a4241e866e07d`  
		Last Modified: Fri, 26 Jun 2020 20:46:51 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:10-alpine` - linux; s390x

```console
$ docker pull postgres@sha256:665c414d159a66708fe78deda0d28c4ad191f2da8d4f56e86c9ffdae737b5bef
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.3 MB (28254706 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ad31612cf4ae701c93857be9074cf6d75f4c6490e28a749f0b25330041d7386`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Fri, 29 May 2020 21:41:39 GMT
ADD file:9799ce3b2f782a28e10b1846cd9b3db827fa99c9bc601feb268456195856814e in / 
# Fri, 29 May 2020 21:41:39 GMT
CMD ["/bin/sh"]
# Thu, 11 Jun 2020 19:51:55 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 11 Jun 2020 19:51:56 GMT
ENV LANG=en_US.utf8
# Thu, 11 Jun 2020 19:51:57 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 11 Jun 2020 20:05:03 GMT
ENV PG_MAJOR=10
# Thu, 11 Jun 2020 20:05:03 GMT
ENV PG_VERSION=10.13
# Thu, 11 Jun 2020 20:05:03 GMT
ENV PG_SHA256=4d701f450cd92ffb123cf6c296e9656abbc2ab7ea6507894ff1e2475ae0754e1
# Fri, 26 Jun 2020 20:03:13 GMT
RUN set -ex 		&& wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2" 	&& echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c - 	&& mkdir -p /usr/src/postgresql 	&& tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	&& rm postgresql.tar.bz2 		&& apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 		&& cd /usr/src/postgresql 	&& awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new 	&& grep '/var/run/postgresql' src/include/pg_config_manual.h.new 	&& mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& ./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 	&& make -j "$(nproc)" world 	&& make install-world 	&& make -C contrib install 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	&& apk del --no-network .build-deps 	&& cd / 	&& rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	&& find /usr/local -name '*.a' -delete
# Fri, 26 Jun 2020 20:03:15 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Fri, 26 Jun 2020 20:03:15 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 26 Jun 2020 20:03:16 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 26 Jun 2020 20:03:16 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 26 Jun 2020 20:03:17 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 26 Jun 2020 20:03:17 GMT
COPY file:33e6fc6ab9ea2b87183e496ad72f1df7f682913ffd781b1451fd178b0c7d745a in /usr/local/bin/ 
# Fri, 26 Jun 2020 20:03:17 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 26 Jun 2020 20:03:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Jun 2020 20:03:18 GMT
EXPOSE 5432
# Fri, 26 Jun 2020 20:03:18 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:8fb3d41b2e9a59630b51745f257cd2561f96bcd15cf309fcc20120d5fcee8c5b`  
		Last Modified: Fri, 29 May 2020 21:42:03 GMT  
		Size: 2.6 MB (2566189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9066740685f109ff5f6b8d3a76bf92f0a147fc0c2c7a12e60fdc44c49e476f9d`  
		Last Modified: Thu, 11 Jun 2020 20:12:40 GMT  
		Size: 1.3 KB (1277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8b44ce9d8f58aeaceb2528f4511ad9c56f557e0951ea9cf22b452d5e2f8bbf0`  
		Last Modified: Thu, 11 Jun 2020 20:12:39 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a82e49fe629e25d23d3f0d08a75ef3129ff9b1fe33baeab4b1a783c130d51a09`  
		Last Modified: Fri, 26 Jun 2020 20:08:44 GMT  
		Size: 25.7 MB (25675001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d6a4dbb3f5a782f2081b84f88f9c2135114f408e9aff3a0418c056f37ae00a3`  
		Last Modified: Fri, 26 Jun 2020 20:08:39 GMT  
		Size: 7.4 KB (7355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e93e2586cd3826569e993c7934ac74b133169ad3f577b6b4fcc5c2425b8749ac`  
		Last Modified: Fri, 26 Jun 2020 20:08:40 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42f86523665a127252eb81c1a2ba496b1d795c2e01b45e5a9ca9301033948426`  
		Last Modified: Fri, 26 Jun 2020 20:08:40 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07497ba3e16f2bd6197a1d13fc71bb22ede42c1e64c5f3972fd51c5614e79a18`  
		Last Modified: Fri, 26 Jun 2020 20:08:40 GMT  
		Size: 4.3 KB (4258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af9433e1d7df65eba07f26c20978cfecaf2482d25281abae1fa165b4e32ffeb6`  
		Last Modified: Fri, 26 Jun 2020 20:08:45 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
