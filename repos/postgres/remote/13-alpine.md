## `postgres:13-alpine`

```console
$ docker pull postgres@sha256:28e7ddf9f137b6cff7234bd57027f69e4e7a9e421615ead38c1bba0b94e8ac9e
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

### `postgres:13-alpine` - linux; amd64

```console
$ docker pull postgres@sha256:188f89f47973de8b730e505da50c15bbbb2a0949169546c9bbdd47d3c42f9d56
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.0 MB (61999811 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:329922c3c1c1b165f98fd458643012a423fbe16fface40b98cfbf5512cfb2e36`
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
# Fri, 14 Aug 2020 17:20:56 GMT
ENV PG_VERSION=13beta3
# Fri, 14 Aug 2020 17:20:56 GMT
ENV PG_SHA256=863e33ee9d1099e2a0f1cab6dbd015789b2c2af75cfbad814a3acdf7c8eeaf9d
# Fri, 14 Aug 2020 17:26:27 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm10-dev clang g++ 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 	find /usr/local -name '*.a' -delete; 		postgres --version
# Fri, 14 Aug 2020 17:26:28 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Fri, 14 Aug 2020 17:26:28 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 14 Aug 2020 17:26:29 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 14 Aug 2020 17:26:29 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 14 Aug 2020 17:26:29 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 14 Aug 2020 17:26:30 GMT
COPY file:33e6fc6ab9ea2b87183e496ad72f1df7f682913ffd781b1451fd178b0c7d745a in /usr/local/bin/ 
# Fri, 14 Aug 2020 17:26:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 14 Aug 2020 17:26:30 GMT
EXPOSE 5432
# Fri, 14 Aug 2020 17:26:30 GMT
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
	-	`sha256:e1cd7a27b77a9e18018a2a48f1d36ba919490fe005826cf16fda939a4b827012`  
		Last Modified: Fri, 14 Aug 2020 17:56:11 GMT  
		Size: 59.2 MB (59187817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d664703aecf17f1c561bb75b28144ed4be15f7cb5a913a863131c7ac9ee502b2`  
		Last Modified: Fri, 14 Aug 2020 17:55:47 GMT  
		Size: 8.5 KB (8535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d0f9e022a76286bbf81deb71a81865f04eaa02224ae42fd5fab8a3f50579fbe`  
		Last Modified: Fri, 14 Aug 2020 17:55:47 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99d39193700b759b051268add99b614a34083f08318792a0b9470e9184b4cfad`  
		Last Modified: Fri, 14 Aug 2020 17:55:47 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f442b720b44a51559804d17f405dc86459a251b65c090a4e879a712fbb68d80b`  
		Last Modified: Fri, 14 Aug 2020 17:55:47 GMT  
		Size: 4.3 KB (4264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:13-alpine` - linux; arm variant v6

```console
$ docker pull postgres@sha256:9d8b5975b1fccb329ea5d68290254464c588cd2476621d0188d5444b59bb422e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.2 MB (60219372 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b1f48884be0f6bb26b59f0579af7343678ea43dc3163f643d0922c9e2274736f`
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
# Fri, 14 Aug 2020 16:50:59 GMT
ENV PG_VERSION=13beta3
# Fri, 14 Aug 2020 16:50:59 GMT
ENV PG_SHA256=863e33ee9d1099e2a0f1cab6dbd015789b2c2af75cfbad814a3acdf7c8eeaf9d
# Fri, 14 Aug 2020 16:55:12 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm10-dev clang g++ 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 	find /usr/local -name '*.a' -delete; 		postgres --version
# Fri, 14 Aug 2020 16:55:15 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Fri, 14 Aug 2020 16:55:17 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 14 Aug 2020 16:55:17 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 14 Aug 2020 16:55:19 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 14 Aug 2020 16:55:20 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 14 Aug 2020 16:55:20 GMT
COPY file:33e6fc6ab9ea2b87183e496ad72f1df7f682913ffd781b1451fd178b0c7d745a in /usr/local/bin/ 
# Fri, 14 Aug 2020 16:55:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 14 Aug 2020 16:55:21 GMT
EXPOSE 5432
# Fri, 14 Aug 2020 16:55:22 GMT
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
	-	`sha256:e15640ed6898b15f4d475da40f9bba8ea99b8457a87a4e194c3a7c8dfee6096c`  
		Last Modified: Fri, 14 Aug 2020 17:14:14 GMT  
		Size: 57.6 MB (57601515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2465cbe4a54442e8f0741663d78a69f32e3dc05b87353034d11a9066acb84ae6`  
		Last Modified: Fri, 14 Aug 2020 17:13:57 GMT  
		Size: 8.5 KB (8532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20a9a8a86bf0f5fc9bf1b74e46fd2614bf05eb4e079c2cb8c62261c92008e1b8`  
		Last Modified: Fri, 14 Aug 2020 17:13:57 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e14e76485116772f4e8836729b76b53226908c7bcbf60a0737c59129eca6801`  
		Last Modified: Fri, 14 Aug 2020 17:13:58 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbe505a0beae65af4d1a5792113a31f09d463a9507c557a0ac586908fe39112c`  
		Last Modified: Fri, 14 Aug 2020 17:13:57 GMT  
		Size: 4.3 KB (4257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:13-alpine` - linux; arm variant v7

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

### `postgres:13-alpine` - linux; arm64 variant v8

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

### `postgres:13-alpine` - linux; 386

```console
$ docker pull postgres@sha256:0c499e45440e50eba54d97bea1b91f588d2816ac3a6dbcacaf2ebb38ce2e24c7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.5 MB (65543647 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af154bb0a8fe019b3229c2447e039c30acde6281a86948c4905d8c2aff31a4b2`
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
# Fri, 14 Aug 2020 17:39:13 GMT
ENV PG_VERSION=13beta3
# Fri, 14 Aug 2020 17:39:13 GMT
ENV PG_SHA256=863e33ee9d1099e2a0f1cab6dbd015789b2c2af75cfbad814a3acdf7c8eeaf9d
# Fri, 14 Aug 2020 17:50:23 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm10-dev clang g++ 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 	find /usr/local -name '*.a' -delete; 		postgres --version
# Fri, 14 Aug 2020 17:50:24 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Fri, 14 Aug 2020 17:50:24 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 14 Aug 2020 17:50:25 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 14 Aug 2020 17:50:25 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 14 Aug 2020 17:50:26 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 14 Aug 2020 17:50:26 GMT
COPY file:33e6fc6ab9ea2b87183e496ad72f1df7f682913ffd781b1451fd178b0c7d745a in /usr/local/bin/ 
# Fri, 14 Aug 2020 17:50:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 14 Aug 2020 17:50:26 GMT
EXPOSE 5432
# Fri, 14 Aug 2020 17:50:27 GMT
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
	-	`sha256:3bec1a529f3d60bd7225aebaca88322f3bdae52f14586d14c418ba7d4f0d673f`  
		Last Modified: Fri, 14 Aug 2020 18:21:49 GMT  
		Size: 62.7 MB (62736898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac9c932a6814e192bf834e9ddade7da4363d1a60ad59fff9e5ca6d04356337ef`  
		Last Modified: Fri, 14 Aug 2020 18:21:35 GMT  
		Size: 8.5 KB (8538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60f4a8e4dba58f2b3b6b6e0b5a38de351676b3d7323b1f80b57eef16f00956b8`  
		Last Modified: Fri, 14 Aug 2020 18:21:35 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f0d9e4cc68ffffa329ba88bdac6d72e37aed219a9e0870714ab8d2d7536ab39`  
		Last Modified: Fri, 14 Aug 2020 18:21:35 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4ef976ea42835f6928ec9b4daf915ef87c5d9f82c41263dbfa6bd7921fd01e2`  
		Last Modified: Fri, 14 Aug 2020 18:21:35 GMT  
		Size: 4.3 KB (4259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:13-alpine` - linux; ppc64le

```console
$ docker pull postgres@sha256:cd9d558a59f1cc79087a33dffdfac97d1ed3defe32e52e4eadceeb7ee8e39c32
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.3 MB (64321049 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:945d6ee8463134f6b263d16a68c267eaaae9e74547c3266c50aec2f745b6f2ab`
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
# Fri, 14 Aug 2020 17:23:00 GMT
ENV PG_VERSION=13beta3
# Fri, 14 Aug 2020 17:23:06 GMT
ENV PG_SHA256=863e33ee9d1099e2a0f1cab6dbd015789b2c2af75cfbad814a3acdf7c8eeaf9d
# Fri, 14 Aug 2020 17:27:24 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm10-dev clang g++ 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 	find /usr/local -name '*.a' -delete; 		postgres --version
# Fri, 14 Aug 2020 17:27:41 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Fri, 14 Aug 2020 17:27:50 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 14 Aug 2020 17:27:56 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 14 Aug 2020 17:28:11 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 14 Aug 2020 17:28:14 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 14 Aug 2020 17:28:15 GMT
COPY file:33e6fc6ab9ea2b87183e496ad72f1df7f682913ffd781b1451fd178b0c7d745a in /usr/local/bin/ 
# Fri, 14 Aug 2020 17:28:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 14 Aug 2020 17:28:22 GMT
EXPOSE 5432
# Fri, 14 Aug 2020 17:28:27 GMT
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
	-	`sha256:c3a6eeb714101c243171a1c74c3019775ca197647499d45ea6d5063dd094a54d`  
		Last Modified: Fri, 14 Aug 2020 18:11:09 GMT  
		Size: 61.5 MB (61501262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17a53b8808689393d1688389e455cedc110b22ec7db36fbbbfa2d2bee84d45f3`  
		Last Modified: Fri, 14 Aug 2020 18:10:58 GMT  
		Size: 8.5 KB (8541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03a0eabcb048bcdf7fc68062bb7fb18eaad0f4d1371fbd9af5c1793db96449d7`  
		Last Modified: Fri, 14 Aug 2020 18:10:56 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd18bfb9cf9e33d5d99620c194e4b62130bc303ead66e6c3d94498951b90e171`  
		Last Modified: Fri, 14 Aug 2020 18:10:58 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0066f455006bdebba6f493c65c52aa4bcc9c81d3f00cf33f05014cd1294b1a7e`  
		Last Modified: Fri, 14 Aug 2020 18:10:57 GMT  
		Size: 4.3 KB (4262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:13-alpine` - linux; s390x

```console
$ docker pull postgres@sha256:8fb60c7efc98da1286986709605c094de769e96908ef7b8326e9d3960277b289
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.5 MB (64456334 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2be6cf69ed71c04435e6b18332fd0994c4428248a8b0b452888cf5343b9b48f7`
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
# Fri, 14 Aug 2020 17:51:05 GMT
ENV PG_VERSION=13beta3
# Fri, 14 Aug 2020 17:51:05 GMT
ENV PG_SHA256=863e33ee9d1099e2a0f1cab6dbd015789b2c2af75cfbad814a3acdf7c8eeaf9d
# Fri, 14 Aug 2020 17:54:42 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm10-dev clang g++ 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 	find /usr/local -name '*.a' -delete; 		postgres --version
# Fri, 14 Aug 2020 17:54:45 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Fri, 14 Aug 2020 17:54:46 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 14 Aug 2020 17:54:46 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 14 Aug 2020 17:54:47 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 14 Aug 2020 17:54:47 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 14 Aug 2020 17:54:47 GMT
COPY file:33e6fc6ab9ea2b87183e496ad72f1df7f682913ffd781b1451fd178b0c7d745a in /usr/local/bin/ 
# Fri, 14 Aug 2020 17:54:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 14 Aug 2020 17:54:48 GMT
EXPOSE 5432
# Fri, 14 Aug 2020 17:54:48 GMT
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
	-	`sha256:8d51af78a06ac0bbc2bf5e4bc0c19654de0967a180b5c6b187a939989a3438bf`  
		Last Modified: Fri, 14 Aug 2020 18:20:31 GMT  
		Size: 61.9 MB (61875561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20cdab784661a149a298344704e07d1cc6e6cc6d35a056142650193fbf3db347`  
		Last Modified: Fri, 14 Aug 2020 18:20:23 GMT  
		Size: 8.5 KB (8541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:023233d76b7e2ccaa19c83853f3f4a3cdca5e56f983d8c4d9ad8c715c8334953`  
		Last Modified: Fri, 14 Aug 2020 18:20:23 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25ab2fcdddf1487d2e3b63572a7c17895ff697ab615f048cc383bf47a3d55175`  
		Last Modified: Fri, 14 Aug 2020 18:20:23 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1bfccf1f73435ff7e79b6102347bd3cf277104318cf2c86f978b35c81138ba5`  
		Last Modified: Fri, 14 Aug 2020 18:20:23 GMT  
		Size: 4.3 KB (4260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
