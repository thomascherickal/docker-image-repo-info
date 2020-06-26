## `postgres:13-beta2-alpine`

```console
$ docker pull postgres@sha256:b3a4ebdb37b892696a7bd7e05763b938345f29a7327fc17049c7148c03ff6a92
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

### `postgres:13-beta2-alpine` - linux; amd64

```console
$ docker pull postgres@sha256:70a72c8ce1d1841351b21bad80ff69a0c0f863ec1e0b3b51289a13a12fc75457
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.0 MB (61994028 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cac2ee40fa5a40f0abe53e0138033fe7a9bcee28e7fb6c9eaac4d3a2076b1a86`
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
# Thu, 11 Jun 2020 22:46:49 GMT
ENV PG_MAJOR=13
# Fri, 26 Jun 2020 20:34:53 GMT
ENV PG_VERSION=13beta2
# Fri, 26 Jun 2020 20:34:53 GMT
ENV PG_SHA256=51b8c64f4c354728555144a7bfbdced96afb86e5cfa80a26b5e96a1d9081ee9f
# Fri, 26 Jun 2020 20:41:35 GMT
RUN set -ex 		&& wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2" 	&& echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c - 	&& mkdir -p /usr/src/postgresql 	&& tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	&& rm postgresql.tar.bz2 		&& apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm10-dev clang g++ 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 		&& cd /usr/src/postgresql 	&& awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new 	&& grep '/var/run/postgresql' src/include/pg_config_manual.h.new 	&& mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& ./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	&& make -j "$(nproc)" world 	&& make install-world 	&& make -C contrib install 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	&& apk del --no-network .build-deps 	&& cd / 	&& rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	&& find /usr/local -name '*.a' -delete
# Fri, 26 Jun 2020 20:41:37 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Fri, 26 Jun 2020 20:41:38 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 26 Jun 2020 20:41:39 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 26 Jun 2020 20:41:40 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 26 Jun 2020 20:41:41 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 26 Jun 2020 20:41:41 GMT
COPY file:33e6fc6ab9ea2b87183e496ad72f1df7f682913ffd781b1451fd178b0c7d745a in /usr/local/bin/ 
# Fri, 26 Jun 2020 20:41:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Jun 2020 20:41:42 GMT
EXPOSE 5432
# Fri, 26 Jun 2020 20:41:42 GMT
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
	-	`sha256:da0b7e87acdc03695b63c05aad631243c40fd1eb5243bf99108e48aba5e678c9`  
		Last Modified: Fri, 26 Jun 2020 21:14:40 GMT  
		Size: 59.2 MB (59182057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3efaff8ea7fde151d6d624ad111e9e3bde11fadbaa57c0bb195c2d6bdc0f69a5`  
		Last Modified: Fri, 26 Jun 2020 21:14:29 GMT  
		Size: 8.5 KB (8515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f9b11b9547510e2bbf87566ea10bf95e99a72403acb34951a2b0e12276b2df1`  
		Last Modified: Fri, 26 Jun 2020 21:14:29 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a19443a69ae4021d32a7c3b44932b1fa81375a60bd2b2fd4fe5e74632b33f5c5`  
		Last Modified: Fri, 26 Jun 2020 21:14:30 GMT  
		Size: 164.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cfa04de1a1f6f4f70f20799afc4589b6e24f4ced65aeea0531680b507ae8628`  
		Last Modified: Fri, 26 Jun 2020 21:14:29 GMT  
		Size: 4.3 KB (4259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:13-beta2-alpine` - linux; arm variant v6

```console
$ docker pull postgres@sha256:7aea04cd9fe5f506bcd8e8ea87832cb58c2a5a08755bef03b56ed8b3b0d34b16
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.2 MB (60214088 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3d38384ca39bd5f8cc7012590959b10e0f4de1152fd71e7117c579982b5ad18f`
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
# Thu, 11 Jun 2020 20:27:31 GMT
ENV PG_MAJOR=13
# Fri, 26 Jun 2020 19:33:03 GMT
ENV PG_VERSION=13beta2
# Fri, 26 Jun 2020 19:33:03 GMT
ENV PG_SHA256=51b8c64f4c354728555144a7bfbdced96afb86e5cfa80a26b5e96a1d9081ee9f
# Fri, 26 Jun 2020 19:37:36 GMT
RUN set -ex 		&& wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2" 	&& echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c - 	&& mkdir -p /usr/src/postgresql 	&& tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	&& rm postgresql.tar.bz2 		&& apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm10-dev clang g++ 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 		&& cd /usr/src/postgresql 	&& awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new 	&& grep '/var/run/postgresql' src/include/pg_config_manual.h.new 	&& mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& ./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	&& make -j "$(nproc)" world 	&& make install-world 	&& make -C contrib install 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	&& apk del --no-network .build-deps 	&& cd / 	&& rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	&& find /usr/local -name '*.a' -delete
# Fri, 26 Jun 2020 19:37:40 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Fri, 26 Jun 2020 19:37:41 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 26 Jun 2020 19:37:42 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 26 Jun 2020 19:37:44 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 26 Jun 2020 19:37:44 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 26 Jun 2020 19:37:45 GMT
COPY file:33e6fc6ab9ea2b87183e496ad72f1df7f682913ffd781b1451fd178b0c7d745a in /usr/local/bin/ 
# Fri, 26 Jun 2020 19:37:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Jun 2020 19:37:46 GMT
EXPOSE 5432
# Fri, 26 Jun 2020 19:37:47 GMT
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
	-	`sha256:3057ce4d5dbf198d29b09971727a488647c4a99394e35c386ae3439b36072f3f`  
		Last Modified: Fri, 26 Jun 2020 19:58:19 GMT  
		Size: 57.6 MB (57596235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30e691b4dc479af080e012f6ba32259fad89261722dff549d05aecbc4ee02bd1`  
		Last Modified: Fri, 26 Jun 2020 19:58:01 GMT  
		Size: 8.5 KB (8523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d538ebe9ab59c0e73e6e94e470a83b57c4590b4ad875646251ce9fa5ab883ad9`  
		Last Modified: Fri, 26 Jun 2020 19:58:01 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bb1ea925f4fbb760c3e866774487d27ee80b1782541a20e557a8e0aa9dd5ff8`  
		Last Modified: Fri, 26 Jun 2020 19:58:01 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b60d2e10bbc746dfba4374261616681880a7f24960cc00d94227afdb2dc5a23`  
		Last Modified: Fri, 26 Jun 2020 19:58:01 GMT  
		Size: 4.3 KB (4261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:13-beta2-alpine` - linux; arm variant v7

```console
$ docker pull postgres@sha256:e1e2e05a7b4a8ad3871cf699ccead68d1a699326347e2584dbf1f8e251b418ed
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.3 MB (57315682 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e0b694ceee15f215afd07e2c812cc0600ee8c2b806aa3bc88141ba99447037c2`
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
# Thu, 11 Jun 2020 20:44:02 GMT
ENV PG_MAJOR=13
# Fri, 26 Jun 2020 19:25:25 GMT
ENV PG_VERSION=13beta2
# Fri, 26 Jun 2020 19:25:27 GMT
ENV PG_SHA256=51b8c64f4c354728555144a7bfbdced96afb86e5cfa80a26b5e96a1d9081ee9f
# Fri, 26 Jun 2020 19:28:33 GMT
RUN set -ex 		&& wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2" 	&& echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c - 	&& mkdir -p /usr/src/postgresql 	&& tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	&& rm postgresql.tar.bz2 		&& apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm10-dev clang g++ 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 		&& cd /usr/src/postgresql 	&& awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new 	&& grep '/var/run/postgresql' src/include/pg_config_manual.h.new 	&& mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& ./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	&& make -j "$(nproc)" world 	&& make install-world 	&& make -C contrib install 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	&& apk del --no-network .build-deps 	&& cd / 	&& rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	&& find /usr/local -name '*.a' -delete
# Fri, 26 Jun 2020 19:28:36 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Fri, 26 Jun 2020 19:28:38 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 26 Jun 2020 19:28:39 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 26 Jun 2020 19:28:44 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 26 Jun 2020 19:28:46 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 26 Jun 2020 19:28:48 GMT
COPY file:33e6fc6ab9ea2b87183e496ad72f1df7f682913ffd781b1451fd178b0c7d745a in /usr/local/bin/ 
# Fri, 26 Jun 2020 19:28:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Jun 2020 19:28:52 GMT
EXPOSE 5432
# Fri, 26 Jun 2020 19:28:53 GMT
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
	-	`sha256:154d65a446363bdb3ed9c31ced1db30b1ed72869d9411116692c224486e3dfec`  
		Last Modified: Fri, 26 Jun 2020 19:48:13 GMT  
		Size: 54.9 MB (54894361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ff5d8edb8ac5db69dd1419d6d5559be808253a17cf326827ad5dc0e96dbdaac`  
		Last Modified: Fri, 26 Jun 2020 19:47:59 GMT  
		Size: 8.5 KB (8518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11930a89308b36e119e6e290855d2903daec6749e8caf59fec0cd2ac9fb6ed37`  
		Last Modified: Fri, 26 Jun 2020 19:47:59 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c6095624b2ea90b4391308874f11bab7c71f36a2b116420aa33b1a457968884`  
		Last Modified: Fri, 26 Jun 2020 19:47:59 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ec24005972af16e015d38099dd538c1d652e1d4c7b97df0b9d32e4d05f99cd3`  
		Last Modified: Fri, 26 Jun 2020 19:47:58 GMT  
		Size: 4.3 KB (4261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:13-beta2-alpine` - linux; arm64 variant v8

```console
$ docker pull postgres@sha256:a54347b91604b7029f7c0631519b618fe2503b1d8290555fcdf93ffc1a90de25
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.5 MB (61532541 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a39e7c2f452920d4231a3e4c2061daad3c1dd37b534b81c5a8b3be6cfda106c0`
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
# Thu, 11 Jun 2020 21:06:17 GMT
ENV PG_MAJOR=13
# Fri, 26 Jun 2020 20:39:50 GMT
ENV PG_VERSION=13beta2
# Fri, 26 Jun 2020 20:39:51 GMT
ENV PG_SHA256=51b8c64f4c354728555144a7bfbdced96afb86e5cfa80a26b5e96a1d9081ee9f
# Fri, 26 Jun 2020 20:43:31 GMT
RUN set -ex 		&& wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2" 	&& echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c - 	&& mkdir -p /usr/src/postgresql 	&& tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	&& rm postgresql.tar.bz2 		&& apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm10-dev clang g++ 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 		&& cd /usr/src/postgresql 	&& awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new 	&& grep '/var/run/postgresql' src/include/pg_config_manual.h.new 	&& mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& ./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	&& make -j "$(nproc)" world 	&& make install-world 	&& make -C contrib install 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	&& apk del --no-network .build-deps 	&& cd / 	&& rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	&& find /usr/local -name '*.a' -delete
# Fri, 26 Jun 2020 20:43:34 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Fri, 26 Jun 2020 20:43:36 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 26 Jun 2020 20:43:37 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 26 Jun 2020 20:43:40 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 26 Jun 2020 20:43:40 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 26 Jun 2020 20:43:41 GMT
COPY file:33e6fc6ab9ea2b87183e496ad72f1df7f682913ffd781b1451fd178b0c7d745a in /usr/local/bin/ 
# Fri, 26 Jun 2020 20:43:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Jun 2020 20:43:43 GMT
EXPOSE 5432
# Fri, 26 Jun 2020 20:43:44 GMT
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
	-	`sha256:8e7c8c36168cf3c66239a08ad0b99ea913465d2aece63ccadacc4d732c19b4a9`  
		Last Modified: Fri, 26 Jun 2020 21:02:22 GMT  
		Size: 58.8 MB (58810010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:452d7bcd2adf8c2f3f6803474ec371e57517affda2ba4f6b308c791633718e0a`  
		Last Modified: Fri, 26 Jun 2020 21:02:06 GMT  
		Size: 8.5 KB (8522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d138454106f81e2066051008db8ca1e4389f5019ce4c37de68e2d2d7aa61c7c0`  
		Last Modified: Fri, 26 Jun 2020 21:02:06 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1458c338a98cf780876309f80e9a83065c185ff09b93211ec59a6493e9c88cd1`  
		Last Modified: Fri, 26 Jun 2020 21:02:06 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90c69370fa0fb581e0ec76ea3960f30d7ef5b338aeed1d018e98f70b3c4b9aff`  
		Last Modified: Fri, 26 Jun 2020 21:02:06 GMT  
		Size: 4.3 KB (4262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:13-beta2-alpine` - linux; 386

```console
$ docker pull postgres@sha256:f6c73f969e77245103340e0b5ffd2e51f0b2bb64f7593c6dda97026e38f9b9ba
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.5 MB (65534099 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb2a05330b035cf7a99d35556e143fc5112ec7ead644014df7459465e12f7052`
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
# Thu, 11 Jun 2020 23:02:23 GMT
ENV PG_MAJOR=13
# Fri, 26 Jun 2020 22:07:21 GMT
ENV PG_VERSION=13beta2
# Fri, 26 Jun 2020 22:07:21 GMT
ENV PG_SHA256=51b8c64f4c354728555144a7bfbdced96afb86e5cfa80a26b5e96a1d9081ee9f
# Fri, 26 Jun 2020 22:18:39 GMT
RUN set -ex 		&& wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2" 	&& echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c - 	&& mkdir -p /usr/src/postgresql 	&& tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	&& rm postgresql.tar.bz2 		&& apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm10-dev clang g++ 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 		&& cd /usr/src/postgresql 	&& awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new 	&& grep '/var/run/postgresql' src/include/pg_config_manual.h.new 	&& mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& ./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	&& make -j "$(nproc)" world 	&& make install-world 	&& make -C contrib install 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	&& apk del --no-network .build-deps 	&& cd / 	&& rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	&& find /usr/local -name '*.a' -delete
# Fri, 26 Jun 2020 22:18:41 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Fri, 26 Jun 2020 22:18:42 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 26 Jun 2020 22:18:43 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 26 Jun 2020 22:18:44 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 26 Jun 2020 22:18:44 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 26 Jun 2020 22:18:45 GMT
COPY file:33e6fc6ab9ea2b87183e496ad72f1df7f682913ffd781b1451fd178b0c7d745a in /usr/local/bin/ 
# Fri, 26 Jun 2020 22:18:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Jun 2020 22:18:46 GMT
EXPOSE 5432
# Fri, 26 Jun 2020 22:18:46 GMT
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
	-	`sha256:eae00009b72c29b80f0430aa3202dadef8ac811c1522267218baba4e0a62ca65`  
		Last Modified: Fri, 26 Jun 2020 22:53:55 GMT  
		Size: 62.7 MB (62727363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fbebc83c8e3ff79e3f23f7c5f667de21ed7972d16365be6724e6f6772fb1ceb`  
		Last Modified: Fri, 26 Jun 2020 22:53:39 GMT  
		Size: 8.5 KB (8519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bea7cc78a78d41743ac9deb75ae4aff4f1f0da1b980beab6220d337c640387da`  
		Last Modified: Fri, 26 Jun 2020 22:53:38 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02582b20490479f0855c9851074b3bb0b4fbe38e65c9f4ca926cc7b58c042a5e`  
		Last Modified: Fri, 26 Jun 2020 22:53:38 GMT  
		Size: 164.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72dbe9e55fc8c1e2b6e0c7dbf667f4db2ef02a5d90d43635e51b1cbc445fa291`  
		Last Modified: Fri, 26 Jun 2020 22:53:39 GMT  
		Size: 4.3 KB (4263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:13-beta2-alpine` - linux; ppc64le

```console
$ docker pull postgres@sha256:84026a3907ecb1024929e9596a3dce645f5e17c780ee555f86a81355159eabed
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.3 MB (64314656 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:44f07c77e6f639f2a2c89463cc3e300427914c1b6d7789b5c9036d140396a724`
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
# Thu, 11 Jun 2020 21:41:02 GMT
ENV PG_MAJOR=13
# Fri, 26 Jun 2020 20:18:12 GMT
ENV PG_VERSION=13beta2
# Fri, 26 Jun 2020 20:18:16 GMT
ENV PG_SHA256=51b8c64f4c354728555144a7bfbdced96afb86e5cfa80a26b5e96a1d9081ee9f
# Fri, 26 Jun 2020 20:22:07 GMT
RUN set -ex 		&& wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2" 	&& echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c - 	&& mkdir -p /usr/src/postgresql 	&& tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	&& rm postgresql.tar.bz2 		&& apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm10-dev clang g++ 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 		&& cd /usr/src/postgresql 	&& awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new 	&& grep '/var/run/postgresql' src/include/pg_config_manual.h.new 	&& mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& ./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	&& make -j "$(nproc)" world 	&& make install-world 	&& make -C contrib install 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	&& apk del --no-network .build-deps 	&& cd / 	&& rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	&& find /usr/local -name '*.a' -delete
# Fri, 26 Jun 2020 20:22:19 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Fri, 26 Jun 2020 20:22:25 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 26 Jun 2020 20:22:33 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 26 Jun 2020 20:22:39 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 26 Jun 2020 20:22:42 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 26 Jun 2020 20:22:44 GMT
COPY file:33e6fc6ab9ea2b87183e496ad72f1df7f682913ffd781b1451fd178b0c7d745a in /usr/local/bin/ 
# Fri, 26 Jun 2020 20:22:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Jun 2020 20:22:49 GMT
EXPOSE 5432
# Fri, 26 Jun 2020 20:22:54 GMT
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
	-	`sha256:c08afd44423f41502ace0e72e413807e34eeb4963da421f691c5e0092769ced9`  
		Last Modified: Fri, 26 Jun 2020 20:45:28 GMT  
		Size: 61.5 MB (61494892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6420477d0f1c2669e1c4bb9dc93b2f18795827c7621423880a5cda47ab776a5`  
		Last Modified: Fri, 26 Jun 2020 20:45:16 GMT  
		Size: 8.5 KB (8520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20ceb49cb714da449a6689daf5eb30c03fc2b831a4056ad74724a643a3162ae1`  
		Last Modified: Fri, 26 Jun 2020 20:45:16 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9b94b3ed30f423289729fe11d8ac20bc29ee9ec6211b428094ab6b63022c9e3`  
		Last Modified: Fri, 26 Jun 2020 20:45:15 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c689f37363d927b6ee404922dd03b26223de66d9dfeea86931d1c36514d787a`  
		Last Modified: Fri, 26 Jun 2020 20:45:16 GMT  
		Size: 4.3 KB (4260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:13-beta2-alpine` - linux; s390x

```console
$ docker pull postgres@sha256:b6da0462c4692bf2d5e0000e06bd1d0e88b6aba72b2f3d7a9d1ed06b0236f225
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.4 MB (64449190 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:81a6dccd05ee13ad0ed62d433aa8ddd4784a164ffd395d35c58c20b8dc303f02`
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
# Thu, 11 Jun 2020 19:51:57 GMT
ENV PG_MAJOR=13
# Fri, 26 Jun 2020 19:51:31 GMT
ENV PG_VERSION=13beta2
# Fri, 26 Jun 2020 19:51:31 GMT
ENV PG_SHA256=51b8c64f4c354728555144a7bfbdced96afb86e5cfa80a26b5e96a1d9081ee9f
# Fri, 26 Jun 2020 19:54:45 GMT
RUN set -ex 		&& wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2" 	&& echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c - 	&& mkdir -p /usr/src/postgresql 	&& tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	&& rm postgresql.tar.bz2 		&& apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm10-dev clang g++ 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 		&& cd /usr/src/postgresql 	&& awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new 	&& grep '/var/run/postgresql' src/include/pg_config_manual.h.new 	&& mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& ./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	&& make -j "$(nproc)" world 	&& make install-world 	&& make -C contrib install 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	&& apk del --no-network .build-deps 	&& cd / 	&& rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	&& find /usr/local -name '*.a' -delete
# Fri, 26 Jun 2020 19:54:48 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Fri, 26 Jun 2020 19:54:49 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 26 Jun 2020 19:54:49 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 26 Jun 2020 19:54:49 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 26 Jun 2020 19:54:50 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 26 Jun 2020 19:54:50 GMT
COPY file:33e6fc6ab9ea2b87183e496ad72f1df7f682913ffd781b1451fd178b0c7d745a in /usr/local/bin/ 
# Fri, 26 Jun 2020 19:54:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Jun 2020 19:54:50 GMT
EXPOSE 5432
# Fri, 26 Jun 2020 19:54:50 GMT
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
	-	`sha256:9909d6a0d579793581879ddca4c2a127f8a5cf2559de06e83c1c29d43a97ee75`  
		Last Modified: Fri, 26 Jun 2020 20:07:52 GMT  
		Size: 61.9 MB (61868441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fa00840cb9b74b84f5475600e91e28c24b0d161097b546c45ce65e15002aaa1`  
		Last Modified: Fri, 26 Jun 2020 20:07:59 GMT  
		Size: 8.5 KB (8519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b764bb43495a1cdea12534888e8b0ae2680445a773839445423cd7a1a3a60ce`  
		Last Modified: Fri, 26 Jun 2020 20:07:59 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1722b94a9cc207a84a143686ea44336f57f63b9c476d3a7cd89e8a4c0994e5be`  
		Last Modified: Fri, 26 Jun 2020 20:07:59 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f56b12336933dd7b7bd80a28ca6196ef9d933e7ed6b76c6f6ad102d91f3a221c`  
		Last Modified: Fri, 26 Jun 2020 20:07:59 GMT  
		Size: 4.3 KB (4261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
