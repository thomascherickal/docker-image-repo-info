## `postgres:9-alpine`

```console
$ docker pull postgres@sha256:131cfc4e14ecef822986d8d0942406ca1cef3402119829f8c00739647668da34
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

### `postgres:9-alpine` - linux; amd64

```console
$ docker pull postgres@sha256:24160e1a469d3ec7254986c50640d59585e57ef13c0a583cf724656cfb9c3ada
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.6 MB (14588466 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a42c67bd1f54cded75cdc55800e59fff15cf06730b1c4cf9b2d7d45a9525d7c7`
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
# Thu, 11 Jun 2020 23:18:52 GMT
ENV PG_MAJOR=9.6
# Fri, 14 Aug 2020 17:45:20 GMT
ENV PG_VERSION=9.6.19
# Fri, 14 Aug 2020 17:45:21 GMT
ENV PG_SHA256=61f93a94ccddbe0b2d1afaf03f04ba605d8af5b774ff9b830e5adeb50ab55cb0
# Fri, 14 Aug 2020 17:49:48 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 	find /usr/local -name '*.a' -delete; 		postgres --version
# Fri, 14 Aug 2020 17:49:50 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Fri, 14 Aug 2020 17:49:51 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 14 Aug 2020 17:49:52 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 14 Aug 2020 17:49:53 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 14 Aug 2020 17:49:53 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 14 Aug 2020 17:49:54 GMT
COPY file:8241ba12b253167d267d2d8aba237bf478f6de0a6f29aa61515376f105626d03 in /usr/local/bin/ 
# Fri, 14 Aug 2020 17:49:55 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 14 Aug 2020 17:49:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 14 Aug 2020 17:49:56 GMT
EXPOSE 5432
# Fri, 14 Aug 2020 17:49:56 GMT
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
	-	`sha256:beef23c1d21656c00d133b8108620e8385a0bea08381a291fca69032e7f44246`  
		Last Modified: Fri, 14 Aug 2020 17:58:34 GMT  
		Size: 11.8 MB (11777726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4d63fb7eb68aaa9022377ac9974e088ba2ef42118e494f7ad2706185d9c1c6d`  
		Last Modified: Fri, 14 Aug 2020 17:58:30 GMT  
		Size: 7.2 KB (7156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b0f095a3ae38fe7a0129114f926873db204cedcb637967a73f7d5db99a0b4be`  
		Last Modified: Fri, 14 Aug 2020 17:58:30 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:978a844a01a6668e3fb90a4b293eb76a9966a06e4745c5dad6c83e56b005bf9a`  
		Last Modified: Fri, 14 Aug 2020 17:58:30 GMT  
		Size: 164.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8a2d2c5867211e44165b3d63b33a7f77e4d3d93fc8d726643ee70ca3deb0f6c`  
		Last Modified: Fri, 14 Aug 2020 17:58:30 GMT  
		Size: 4.3 KB (4266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13e4b747d566f4ef2e3e87b062687ff2b0fd29076c80b94eb72ea5d81f6aeb1f`  
		Last Modified: Fri, 14 Aug 2020 17:58:30 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:9-alpine` - linux; arm variant v6

```console
$ docker pull postgres@sha256:7199982f05d9aedf2a95128dce44df7001bc685665636f5e05cd3f37cb48eb8a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.0 MB (13971769 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba00ce09d5432791e4a63ff21579314a01233947e41b8049c422ce03b22a025b`
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
# Thu, 11 Jun 2020 20:44:59 GMT
ENV PG_MAJOR=9.6
# Fri, 14 Aug 2020 17:08:10 GMT
ENV PG_VERSION=9.6.19
# Fri, 14 Aug 2020 17:08:10 GMT
ENV PG_SHA256=61f93a94ccddbe0b2d1afaf03f04ba605d8af5b774ff9b830e5adeb50ab55cb0
# Fri, 14 Aug 2020 17:10:40 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 	find /usr/local -name '*.a' -delete; 		postgres --version
# Fri, 14 Aug 2020 17:10:43 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Fri, 14 Aug 2020 17:10:44 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 14 Aug 2020 17:10:45 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 14 Aug 2020 17:10:48 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 14 Aug 2020 17:10:48 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 14 Aug 2020 17:10:49 GMT
COPY file:8241ba12b253167d267d2d8aba237bf478f6de0a6f29aa61515376f105626d03 in /usr/local/bin/ 
# Fri, 14 Aug 2020 17:10:51 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 14 Aug 2020 17:10:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 14 Aug 2020 17:10:52 GMT
EXPOSE 5432
# Fri, 14 Aug 2020 17:10:53 GMT
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
	-	`sha256:08633820479a5e63021c112150c88b01e671b1d1be8f4dea93adf7b392f071f8`  
		Last Modified: Fri, 14 Aug 2020 17:15:30 GMT  
		Size: 11.4 MB (11355161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbed7f0bf08dd37f182ed3e2a5782ea9716eb193b20d625847622a012104144b`  
		Last Modified: Fri, 14 Aug 2020 17:15:25 GMT  
		Size: 7.2 KB (7160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e58109fcafbf4a30847c8c154d71a717ba2e94545d38b4aa777eb91787d4dda9`  
		Last Modified: Fri, 14 Aug 2020 17:15:25 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa0f4cc182dc66682b21fb61d7e969939aa4760e2a04d43c82a97c5a08d9e35f`  
		Last Modified: Fri, 14 Aug 2020 17:15:25 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3f8107bde569618e724b4c854dcf04e424d8a46407d88822102b2fc3ace7fbd`  
		Last Modified: Fri, 14 Aug 2020 17:15:25 GMT  
		Size: 4.3 KB (4257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b12533c009ce3b9db130e1836920e6c16f484753faf5576c7a136110c3e51b5e`  
		Last Modified: Fri, 14 Aug 2020 17:15:26 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:9-alpine` - linux; arm variant v7

```console
$ docker pull postgres@sha256:4b3d132ba62eea492b9f1855113e67283542d3229a01ccabe398b8984f35d367
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.1 MB (13104663 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ff20237da194abb270f7a3efcd2f24a325112dd93288dc6a33c09331b91eb1e5`
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
# Thu, 11 Jun 2020 20:59:17 GMT
ENV PG_MAJOR=9.6
# Thu, 11 Jun 2020 20:59:20 GMT
ENV PG_VERSION=9.6.18
# Thu, 11 Jun 2020 20:59:26 GMT
ENV PG_SHA256=517ec282b785e6d22f360c30ba0c5e2a506fca5ca07dcc545427511d94c89999
# Fri, 26 Jun 2020 19:42:51 GMT
RUN set -ex 		&& wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2" 	&& echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c - 	&& mkdir -p /usr/src/postgresql 	&& tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	&& rm postgresql.tar.bz2 		&& apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		&& cd /usr/src/postgresql 	&& awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new 	&& grep '/var/run/postgresql' src/include/pg_config_manual.h.new 	&& mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& ./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 	&& make -j "$(nproc)" world 	&& make install-world 	&& make -C contrib install 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	&& apk del --no-network .build-deps 	&& cd / 	&& rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	&& find /usr/local -name '*.a' -delete
# Fri, 26 Jun 2020 19:42:58 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Fri, 26 Jun 2020 19:43:06 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 26 Jun 2020 19:43:08 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 26 Jun 2020 19:43:12 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 26 Jun 2020 19:43:13 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 26 Jun 2020 19:43:14 GMT
COPY file:8241ba12b253167d267d2d8aba237bf478f6de0a6f29aa61515376f105626d03 in /usr/local/bin/ 
# Fri, 26 Jun 2020 19:43:19 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 26 Jun 2020 19:43:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Jun 2020 19:43:23 GMT
EXPOSE 5432
# Fri, 26 Jun 2020 19:43:24 GMT
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
	-	`sha256:878f6b6b32ac29f29f80649f0f524e9f9c8fb88ea92c5ee881647c04f60a542a`  
		Last Modified: Fri, 26 Jun 2020 19:49:27 GMT  
		Size: 10.7 MB (10684579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3a1acbc000342e8a8a2585fa5ebf6a200afba2ae7fdba1908384c723c39c0f3`  
		Last Modified: Fri, 26 Jun 2020 19:49:22 GMT  
		Size: 7.2 KB (7156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72ee0ad71a4067772ec65b754818077891d9b3695d608dee6d19116de8911297`  
		Last Modified: Fri, 26 Jun 2020 19:49:22 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:788686e17c7edb82028e24cca893d5243a19351d101ba7cb88ba92dd893d00d5`  
		Last Modified: Fri, 26 Jun 2020 19:49:22 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:850b367cd47d9c63c723ff25a3471218e5a44903b62e896513ac0c195b68393a`  
		Last Modified: Fri, 26 Jun 2020 19:49:22 GMT  
		Size: 4.3 KB (4265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05d0cc24ea7796aea97d68eabad8df201c8d882ca74fd297f64ad9b92cfffbba`  
		Last Modified: Fri, 26 Jun 2020 19:49:23 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:9-alpine` - linux; arm64 variant v8

```console
$ docker pull postgres@sha256:a359dc223d9a1e815323e0c04e50f80fb934f4fbce0a34ce9b602a1bed8a52dd
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.3 MB (14345160 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0d6dbb27c1d8405bd733aa31fdf266b33edb5f4e69bca9b3e95d07eda95c283d`
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
# Thu, 11 Jun 2020 21:34:57 GMT
ENV PG_MAJOR=9.6
# Thu, 11 Jun 2020 21:34:58 GMT
ENV PG_VERSION=9.6.18
# Thu, 11 Jun 2020 21:34:58 GMT
ENV PG_SHA256=517ec282b785e6d22f360c30ba0c5e2a506fca5ca07dcc545427511d94c89999
# Fri, 26 Jun 2020 20:57:32 GMT
RUN set -ex 		&& wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2" 	&& echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c - 	&& mkdir -p /usr/src/postgresql 	&& tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	&& rm postgresql.tar.bz2 		&& apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		&& cd /usr/src/postgresql 	&& awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new 	&& grep '/var/run/postgresql' src/include/pg_config_manual.h.new 	&& mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& ./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 	&& make -j "$(nproc)" world 	&& make install-world 	&& make -C contrib install 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	&& apk del --no-network .build-deps 	&& cd / 	&& rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	&& find /usr/local -name '*.a' -delete
# Fri, 26 Jun 2020 20:57:38 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Fri, 26 Jun 2020 20:57:41 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 26 Jun 2020 20:57:42 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 26 Jun 2020 20:57:46 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 26 Jun 2020 20:57:48 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 26 Jun 2020 20:57:49 GMT
COPY file:8241ba12b253167d267d2d8aba237bf478f6de0a6f29aa61515376f105626d03 in /usr/local/bin/ 
# Fri, 26 Jun 2020 20:57:51 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 26 Jun 2020 20:57:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Jun 2020 20:57:53 GMT
EXPOSE 5432
# Fri, 26 Jun 2020 20:57:55 GMT
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
	-	`sha256:93b9f304949af753967afb0d6a53cc0e94ce5bc3825ffc1f1032f312249b73ba`  
		Last Modified: Fri, 26 Jun 2020 21:03:34 GMT  
		Size: 11.6 MB (11623871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ad7a8831513abd5ec8d11f81a44a0a2cad63d200112b7db4a9f7ccab6918a6d`  
		Last Modified: Fri, 26 Jun 2020 21:03:29 GMT  
		Size: 7.2 KB (7159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e44a3db62d4404d0cf3a0689aac4dd3088cea56f85b23430ddd8e19ba178623d`  
		Last Modified: Fri, 26 Jun 2020 21:03:29 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b00fdd860128578be3e9437e7c3e1d3d3ee6a66a94d2b2077916427af6ab6b5`  
		Last Modified: Fri, 26 Jun 2020 21:03:29 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22fce9f3f22e0cd11544a69f199a944bf4cdf172e9e2a52d8c18697969e3af85`  
		Last Modified: Fri, 26 Jun 2020 21:03:29 GMT  
		Size: 4.3 KB (4261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b854d4d4f27e9a77d8430134d72c947ee831c8b4b51e1c2f0b7e8b1161226d5`  
		Last Modified: Fri, 26 Jun 2020 21:03:30 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:9-alpine` - linux; 386

```console
$ docker pull postgres@sha256:05fb406fd481a6c452a1836ef1fe9605267333719a2667fae104c955b28ef139
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.2 MB (15188511 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:39c305da8404c81c7c5ecab27fa2d2ea5f1b5797a26a14e90c107312b37a4e36`
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
# Thu, 11 Jun 2020 23:41:59 GMT
ENV PG_MAJOR=9.6
# Fri, 14 Aug 2020 18:12:55 GMT
ENV PG_VERSION=9.6.19
# Fri, 14 Aug 2020 18:12:55 GMT
ENV PG_SHA256=61f93a94ccddbe0b2d1afaf03f04ba605d8af5b774ff9b830e5adeb50ab55cb0
# Fri, 14 Aug 2020 18:16:28 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 	find /usr/local -name '*.a' -delete; 		postgres --version
# Fri, 14 Aug 2020 18:16:29 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Fri, 14 Aug 2020 18:16:29 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 14 Aug 2020 18:16:29 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 14 Aug 2020 18:16:30 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 14 Aug 2020 18:16:30 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 14 Aug 2020 18:16:31 GMT
COPY file:8241ba12b253167d267d2d8aba237bf478f6de0a6f29aa61515376f105626d03 in /usr/local/bin/ 
# Fri, 14 Aug 2020 18:16:31 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 14 Aug 2020 18:16:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 14 Aug 2020 18:16:32 GMT
EXPOSE 5432
# Fri, 14 Aug 2020 18:16:32 GMT
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
	-	`sha256:c960cc9da1c64bb641687fa25d00962aa29a2c1e6168121edf14029aef35e890`  
		Last Modified: Fri, 14 Aug 2020 18:24:05 GMT  
		Size: 12.4 MB (12383015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45eb203094af5d3dd8f9d4de1efbd7f37dfe7dea1834449d4cc112b3b1e54541`  
		Last Modified: Fri, 14 Aug 2020 18:24:01 GMT  
		Size: 7.2 KB (7163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61c74e7abe4bb1ae5d20d0ba135e4cb48c0f81a3d478917139755b9c9b86521b`  
		Last Modified: Fri, 14 Aug 2020 18:24:01 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed9b305ec79fc170e064c349902a820321ff36b6795cb198245978f31930fc7b`  
		Last Modified: Fri, 14 Aug 2020 18:24:01 GMT  
		Size: 164.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4793c75028209905694bccaa10142ce8a44bf6f3075db07ca284d403e84e77e`  
		Last Modified: Fri, 14 Aug 2020 18:24:01 GMT  
		Size: 4.3 KB (4259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bb162ac2f6ac4cf8324ff292d9f5df6a673e4088e246b44db68613ad8cab985`  
		Last Modified: Fri, 14 Aug 2020 18:24:01 GMT  
		Size: 119.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:9-alpine` - linux; ppc64le

```console
$ docker pull postgres@sha256:5e6d9a8c51a3eb540f4623fa294f25483c4d6cec49f4a6ccc6b110e1ad3a059e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.5 MB (15494192 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:babbd1b43dc8498489ddfeb7aff98fe668a97f5e02333f83b9c55661779ac8b7`
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
# Thu, 11 Jun 2020 21:59:04 GMT
ENV PG_MAJOR=9.6
# Fri, 14 Aug 2020 17:58:31 GMT
ENV PG_VERSION=9.6.19
# Fri, 14 Aug 2020 17:58:38 GMT
ENV PG_SHA256=61f93a94ccddbe0b2d1afaf03f04ba605d8af5b774ff9b830e5adeb50ab55cb0
# Fri, 14 Aug 2020 18:02:11 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 	find /usr/local -name '*.a' -delete; 		postgres --version
# Fri, 14 Aug 2020 18:02:36 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Fri, 14 Aug 2020 18:02:56 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 14 Aug 2020 18:03:03 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 14 Aug 2020 18:03:26 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 14 Aug 2020 18:03:34 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 14 Aug 2020 18:03:37 GMT
COPY file:8241ba12b253167d267d2d8aba237bf478f6de0a6f29aa61515376f105626d03 in /usr/local/bin/ 
# Fri, 14 Aug 2020 18:04:00 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 14 Aug 2020 18:04:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 14 Aug 2020 18:04:13 GMT
EXPOSE 5432
# Fri, 14 Aug 2020 18:04:20 GMT
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
	-	`sha256:3de99203242fcdf4204f0ab945cf7c5b28997f78989bb33dc43944c75c96370b`  
		Last Modified: Fri, 14 Aug 2020 18:13:25 GMT  
		Size: 12.7 MB (12675668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d6e0bca9d9fd1480671729f8915d5e707abc093056963c87729f03720695792`  
		Last Modified: Fri, 14 Aug 2020 18:13:18 GMT  
		Size: 7.2 KB (7155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:127853bbcddd69de4421eaec819b088009611b4fadd9a904cf07d77d5b5aa516`  
		Last Modified: Fri, 14 Aug 2020 18:13:18 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5e32b3b8c1922ee2e5f38925abd8d500a10dced780fd6b79a67d91ba4700bfa`  
		Last Modified: Fri, 14 Aug 2020 18:13:18 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e1408a0e3efcb3abd05b155cc9247fe2167c5c45c72f8fa68260ce3fc84635f`  
		Last Modified: Fri, 14 Aug 2020 18:13:18 GMT  
		Size: 4.3 KB (4264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd2253f729e22a3a0676d20559ec483271cf5f7b783e8617f23c969dd7097fbb`  
		Last Modified: Fri, 14 Aug 2020 18:13:18 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:9-alpine` - linux; s390x

```console
$ docker pull postgres@sha256:08acbd1d90d2e1f954de06b0647e0e41df5efb99c7d69741cb19d89b88963549
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.2 MB (14184914 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:113a5536d3705981f6ec10e2817725669fad407d85e3e847a836dd1223be811b`
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
# Thu, 11 Jun 2020 20:07:42 GMT
ENV PG_MAJOR=9.6
# Fri, 14 Aug 2020 18:14:36 GMT
ENV PG_VERSION=9.6.19
# Fri, 14 Aug 2020 18:14:37 GMT
ENV PG_SHA256=61f93a94ccddbe0b2d1afaf03f04ba605d8af5b774ff9b830e5adeb50ab55cb0
# Fri, 14 Aug 2020 18:16:08 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 	find /usr/local -name '*.a' -delete; 		postgres --version
# Fri, 14 Aug 2020 18:16:10 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Fri, 14 Aug 2020 18:16:10 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 14 Aug 2020 18:16:11 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 14 Aug 2020 18:16:11 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 14 Aug 2020 18:16:11 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 14 Aug 2020 18:16:12 GMT
COPY file:8241ba12b253167d267d2d8aba237bf478f6de0a6f29aa61515376f105626d03 in /usr/local/bin/ 
# Fri, 14 Aug 2020 18:16:12 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 14 Aug 2020 18:16:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 14 Aug 2020 18:16:13 GMT
EXPOSE 5432
# Fri, 14 Aug 2020 18:16:13 GMT
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
	-	`sha256:28b25708bc5d5a98348bd08d10e18e5e9daff2b468c9f55f964044d36d6861ba`  
		Last Modified: Fri, 14 Aug 2020 18:21:46 GMT  
		Size: 11.6 MB (11605407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd94b19c933438ae7eab4f2150c73f313830601f1b6d979918d053f896fd9b96`  
		Last Modified: Fri, 14 Aug 2020 18:21:42 GMT  
		Size: 7.2 KB (7157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8e9dd4dba79c7da4d9d0b133367847ca68c0552e3ba879a8848b7470c888506`  
		Last Modified: Fri, 14 Aug 2020 18:21:42 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2eaa69c0fc76f0de474961dca67964c030ec42f06a13cc354f3604f34fe78f3b`  
		Last Modified: Fri, 14 Aug 2020 18:21:42 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e90be655de6384d86d83f71f81ece2a4621f0c01912a0fe60dbc825a09fa4254`  
		Last Modified: Fri, 14 Aug 2020 18:21:42 GMT  
		Size: 4.3 KB (4256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:862878ee73ad43a422e5603fd82a9dd8f061bffc385a10a001e3fccb9e4ab2c5`  
		Last Modified: Fri, 14 Aug 2020 18:21:42 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
