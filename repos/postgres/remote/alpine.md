## `postgres:alpine`

```console
$ docker pull postgres@sha256:fe79e56c374441f03569370e8be4b33f3308e5b9be25b976ad9735488cc9b5e5
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

### `postgres:alpine` - linux; amd64

```console
$ docker pull postgres@sha256:024c97d18e5060ef48ce20ea96550506a137403b0aaf1d2fd56b1483d40b89fe
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.1 MB (62145522 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6415f604ebf8e32158a07426205cd3882c6a36cb955c16bd26cdebe006cbeb20`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Fri, 11 Dec 2020 02:04:06 GMT
ADD file:62a1e09319acb6d1bad91ef1c35aabdc7e5e19883a77f30f1951ccfffc812124 in / 
# Fri, 11 Dec 2020 02:04:07 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 12:24:09 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Fri, 11 Dec 2020 12:24:10 GMT
ENV LANG=en_US.utf8
# Fri, 11 Dec 2020 12:24:11 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 11 Dec 2020 12:24:11 GMT
ENV PG_MAJOR=13
# Fri, 11 Dec 2020 12:24:11 GMT
ENV PG_VERSION=13.1
# Fri, 11 Dec 2020 12:24:11 GMT
ENV PG_SHA256=12345c83b89aa29808568977f5200d6da00f88a035517f925293355432ffe61f
# Fri, 11 Dec 2020 12:32:56 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm10-dev clang g++ 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Fri, 11 Dec 2020 12:32:57 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Fri, 11 Dec 2020 12:32:58 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 11 Dec 2020 12:32:58 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 11 Dec 2020 12:32:59 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 11 Dec 2020 12:32:59 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 11 Dec 2020 12:32:59 GMT
COPY file:8f542efd076b9b67ef64928f3c0185ed50bfcbbc3572436a7222e879810d747f in /usr/local/bin/ 
# Fri, 11 Dec 2020 12:32:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 12:33:00 GMT
STOPSIGNAL SIGINT
# Fri, 11 Dec 2020 12:33:00 GMT
EXPOSE 5432
# Fri, 11 Dec 2020 12:33:00 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:05e7bc50f07f000e9993ec0d264b9ffcbb9a01a4d69c68f556d25e9811a8f7f4`  
		Last Modified: Fri, 11 Dec 2020 02:04:37 GMT  
		Size: 2.8 MB (2796945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b05eb41eecb97b89919d2eacdc86aa1332e168aa4ff3750c35c41525c333054c`  
		Last Modified: Fri, 11 Dec 2020 13:07:48 GMT  
		Size: 1.2 KB (1247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a37c8fecb6acc85d913b4779946759124998986425d194ff748d6c12dabb1e7`  
		Last Modified: Fri, 11 Dec 2020 13:07:49 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccad999f964e7c828cdee085845e59f29f98768d0343b6fa79cc78182cdc03b0`  
		Last Modified: Fri, 11 Dec 2020 13:07:58 GMT  
		Size: 59.3 MB (59334116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2ca942b5238b87b226bd0d43f4134cdf523f1f9462b3c7a4e16f2433a85f06a`  
		Last Modified: Fri, 11 Dec 2020 13:07:47 GMT  
		Size: 8.5 KB (8542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b39228c90d11faa13d7c611a64be2eb100593a6a72950bb70e103c915b580c0e`  
		Last Modified: Fri, 11 Dec 2020 13:07:48 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0be8ebd0ef6225a8e0c5a7727301b0f965f8fcce134a03f06c33419bfcc12c52`  
		Last Modified: Fri, 11 Dec 2020 13:07:48 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:976c32ae61dcebf4a7eb670fa2d3af155efd4b45368eb9f027d8b87456e526ae`  
		Last Modified: Fri, 11 Dec 2020 13:07:47 GMT  
		Size: 4.3 KB (4264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:alpine` - linux; arm variant v6

```console
$ docker pull postgres@sha256:eba55b99485ce49573c4f70661a6509e14a926e0301dfe06cabd07439e92050c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.3 MB (60322259 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:49665089da4cf5f0969ab5bbc35c99057912b2483eaac38e2309a7870ac04763`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Fri, 11 Dec 2020 02:17:15 GMT
ADD file:1a9c0a67560d338c0c0e7005d8915d998fc9cf3e9f53bfd7e42e8391f0a39bce in / 
# Fri, 11 Dec 2020 02:17:15 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 03:19:10 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Fri, 11 Dec 2020 03:19:11 GMT
ENV LANG=en_US.utf8
# Fri, 11 Dec 2020 03:19:14 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 11 Dec 2020 03:19:15 GMT
ENV PG_MAJOR=13
# Fri, 11 Dec 2020 03:19:18 GMT
ENV PG_VERSION=13.1
# Fri, 11 Dec 2020 03:19:21 GMT
ENV PG_SHA256=12345c83b89aa29808568977f5200d6da00f88a035517f925293355432ffe61f
# Fri, 11 Dec 2020 03:23:42 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm10-dev clang g++ 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Fri, 11 Dec 2020 03:23:45 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Fri, 11 Dec 2020 03:23:47 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 11 Dec 2020 03:23:48 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 11 Dec 2020 03:23:50 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 11 Dec 2020 03:23:51 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 11 Dec 2020 03:23:52 GMT
COPY file:8f542efd076b9b67ef64928f3c0185ed50bfcbbc3572436a7222e879810d747f in /usr/local/bin/ 
# Fri, 11 Dec 2020 03:23:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 03:23:54 GMT
STOPSIGNAL SIGINT
# Fri, 11 Dec 2020 03:23:57 GMT
EXPOSE 5432
# Fri, 11 Dec 2020 03:23:58 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:f1c16df8fee33d421d08790b17ca2af67a3fe49e77b6b991dd0c30631f5d1baf`  
		Last Modified: Fri, 11 Dec 2020 02:17:57 GMT  
		Size: 2.6 MB (2601992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76b7015842cf54dcea68acedc8c878eb3e85df19eea729780caf5876a68ea886`  
		Last Modified: Fri, 11 Dec 2020 03:44:54 GMT  
		Size: 1.3 KB (1279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4750e2c99e48f7325df4f7ed77a0bfab419f5470d2747d50f891b372583e7f3`  
		Last Modified: Fri, 11 Dec 2020 03:44:54 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6739c463a64e1ba2de9978f12a29e634502f8b0bbb5f43ad220fd9aef1091c63`  
		Last Modified: Fri, 11 Dec 2020 03:45:10 GMT  
		Size: 57.7 MB (57705676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa1e3e79cf2265e449a48df98433e3616a6878964d6eefc446d517675860e701`  
		Last Modified: Fri, 11 Dec 2020 03:44:52 GMT  
		Size: 8.5 KB (8544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5ccfeea641b10f4e1f314111ca76b2ea36d0ec69c190b2e6769b8edf91a3974`  
		Last Modified: Fri, 11 Dec 2020 03:44:52 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3667bb6b9e8867f58e858755efd4c5daf17cfac9c6867e73882ec6eb82b99eb8`  
		Last Modified: Fri, 11 Dec 2020 03:44:52 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29a79af5f1b23747ab257dd9a6fff5534f09ec055afc09942fc4210cc72bc77f`  
		Last Modified: Fri, 11 Dec 2020 03:44:52 GMT  
		Size: 4.3 KB (4263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:alpine` - linux; arm variant v7

```console
$ docker pull postgres@sha256:92ab37fed27ef76a9c85bb8ee8733c882318757a71315dfe4e76360bdd8fa94e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.4 MB (57429973 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:18b5139b6ddda79cddee3ed7483fba2575c20b9b2366d09dea9b1fecd1ceb0cc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Fri, 11 Dec 2020 02:20:33 GMT
ADD file:0e85952ec585d17378d9bb15a94ddc10c3ed8f766f275cf50fb36be1126f35d2 in / 
# Fri, 11 Dec 2020 02:20:34 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 09:57:30 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Fri, 11 Dec 2020 09:57:32 GMT
ENV LANG=en_US.utf8
# Fri, 11 Dec 2020 09:57:35 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 11 Dec 2020 09:57:36 GMT
ENV PG_MAJOR=13
# Fri, 11 Dec 2020 09:57:37 GMT
ENV PG_VERSION=13.1
# Fri, 11 Dec 2020 09:57:38 GMT
ENV PG_SHA256=12345c83b89aa29808568977f5200d6da00f88a035517f925293355432ffe61f
# Fri, 11 Dec 2020 10:00:41 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm10-dev clang g++ 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Fri, 11 Dec 2020 10:01:02 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Fri, 11 Dec 2020 10:01:16 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 11 Dec 2020 10:01:21 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 11 Dec 2020 10:01:31 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 11 Dec 2020 10:01:32 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 11 Dec 2020 10:01:35 GMT
COPY file:8f542efd076b9b67ef64928f3c0185ed50bfcbbc3572436a7222e879810d747f in /usr/local/bin/ 
# Fri, 11 Dec 2020 10:01:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 10:01:40 GMT
STOPSIGNAL SIGINT
# Fri, 11 Dec 2020 10:01:41 GMT
EXPOSE 5432
# Fri, 11 Dec 2020 10:01:42 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:f70c74f2e22556cebd0cbbff78c03d4f0560d76979bf799d67730340a639aa57`  
		Last Modified: Fri, 11 Dec 2020 02:21:18 GMT  
		Size: 2.4 MB (2405692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7cd8806bcb86432eb337ebed64a71a663101cfc12c9785018615d82142fa33e`  
		Last Modified: Fri, 11 Dec 2020 11:57:38 GMT  
		Size: 1.3 KB (1278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f047e2e411e97b34b2928ccf0fac2f48025ef6bed64ce781c283e6774473eccc`  
		Last Modified: Fri, 11 Dec 2020 11:57:38 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b4e92821679070236ae9cc9fc725af4fbe5566ac98258ce1f9c9f51e6f5b93c`  
		Last Modified: Fri, 11 Dec 2020 11:57:50 GMT  
		Size: 55.0 MB (55009688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95a1626656e1ee9f3533e83fa51ef1e5fd74f30ba43cabb87e653c515e901112`  
		Last Modified: Fri, 11 Dec 2020 11:57:35 GMT  
		Size: 8.5 KB (8545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7629915f169e02de65665844832867ed2a9b789a8ed255dfb6c807e765fe28de`  
		Last Modified: Fri, 11 Dec 2020 11:57:35 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e8e797dad6fb5f273fd5b60b2c1a047e154e2f926be70f9cfb201abf6909f31`  
		Last Modified: Fri, 11 Dec 2020 11:57:36 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d64f3eb7a848024a286491ae460df55614c3543273e3101acb68cc1a389b2883`  
		Last Modified: Fri, 11 Dec 2020 11:57:36 GMT  
		Size: 4.3 KB (4264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:alpine` - linux; arm64 variant v8

```console
$ docker pull postgres@sha256:16f03c45030dd4008055026c29a34c37685d12372b3d6e3c99ba0399f203453a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.7 MB (61682612 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:69a4fc29ae45005c298b0125c601d60ea9f8c5445824e985955050977a1d8949`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Fri, 11 Dec 2020 02:42:58 GMT
ADD file:a1a6d0f8dffb9bc75438921cdb5c04d2f2f49400a7526dcf3d8dff9238e3235a in / 
# Fri, 11 Dec 2020 02:43:00 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 07:43:01 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Fri, 11 Dec 2020 07:43:04 GMT
ENV LANG=en_US.utf8
# Fri, 11 Dec 2020 07:43:08 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 11 Dec 2020 07:43:10 GMT
ENV PG_MAJOR=13
# Fri, 11 Dec 2020 07:43:12 GMT
ENV PG_VERSION=13.1
# Fri, 11 Dec 2020 07:43:13 GMT
ENV PG_SHA256=12345c83b89aa29808568977f5200d6da00f88a035517f925293355432ffe61f
# Fri, 11 Dec 2020 07:46:36 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm10-dev clang g++ 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Fri, 11 Dec 2020 07:46:47 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Fri, 11 Dec 2020 07:46:54 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 11 Dec 2020 07:46:56 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 11 Dec 2020 07:47:06 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 11 Dec 2020 07:47:08 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 11 Dec 2020 07:47:11 GMT
COPY file:8f542efd076b9b67ef64928f3c0185ed50bfcbbc3572436a7222e879810d747f in /usr/local/bin/ 
# Fri, 11 Dec 2020 07:47:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 07:47:16 GMT
STOPSIGNAL SIGINT
# Fri, 11 Dec 2020 07:47:19 GMT
EXPOSE 5432
# Fri, 11 Dec 2020 07:47:22 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:a3cc7d3b244e0bac4f32b7529f804d1ab735b088ea432061c3949b2a890b919f`  
		Last Modified: Fri, 11 Dec 2020 02:43:46 GMT  
		Size: 2.7 MB (2706619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ea427249dae13c957e3db1b95561e7c5d8ac8f15eaf4746e4cbc00d20040bf4`  
		Last Modified: Fri, 11 Dec 2020 09:28:07 GMT  
		Size: 1.3 KB (1277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed90029c1f1e4312c5204f01900ecfb18c7511758bf218f91a37ce56fb893f56`  
		Last Modified: Fri, 11 Dec 2020 09:28:08 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb49b04d063b9ec2fb39df7db3456b032bb8a3b39804fd530964516471c85d0d`  
		Last Modified: Fri, 11 Dec 2020 09:28:19 GMT  
		Size: 59.0 MB (58961420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ced4bdbdacff50e9371b97d16ff37e71e51109b64b5fbcb0fc67ee8c5601634`  
		Last Modified: Fri, 11 Dec 2020 09:28:05 GMT  
		Size: 8.5 KB (8536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f645fa2ac36df69dbd1852acc37f47d546ed5a01f74004161d25aed04691e31`  
		Last Modified: Fri, 11 Dec 2020 09:28:05 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53298960ec6a0f9b90a512ec91fb0e075b22ef5f18793595ea9814c5b1e64958`  
		Last Modified: Fri, 11 Dec 2020 09:28:05 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:823764e6ab93256397f951bc406f544eca693aae09ea00600fa8e1997ccaa3d9`  
		Last Modified: Fri, 11 Dec 2020 09:28:06 GMT  
		Size: 4.3 KB (4256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:alpine` - linux; 386

```console
$ docker pull postgres@sha256:aaab473b1c9c6837cee306d07a41f862c8170773e18560301a9ed8db03bbe3df
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.7 MB (65735797 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ed002bec1bd12ae59b5335f628712bb3872d20303a845e292813e31c56097d2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Fri, 11 Dec 2020 02:01:14 GMT
ADD file:8812e502f26af2dc4efdfb7387f8bf99f2a098b6c95b9f6abf900df2ce74e3da in / 
# Fri, 11 Dec 2020 02:01:14 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 11:28:37 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Fri, 11 Dec 2020 11:28:37 GMT
ENV LANG=en_US.utf8
# Fri, 11 Dec 2020 11:28:38 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 11 Dec 2020 11:28:39 GMT
ENV PG_MAJOR=13
# Fri, 11 Dec 2020 11:28:39 GMT
ENV PG_VERSION=13.1
# Fri, 11 Dec 2020 11:28:39 GMT
ENV PG_SHA256=12345c83b89aa29808568977f5200d6da00f88a035517f925293355432ffe61f
# Fri, 11 Dec 2020 11:40:17 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm10-dev clang g++ 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Fri, 11 Dec 2020 11:40:18 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Fri, 11 Dec 2020 11:40:19 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 11 Dec 2020 11:40:19 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 11 Dec 2020 11:40:20 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 11 Dec 2020 11:40:20 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 11 Dec 2020 11:40:20 GMT
COPY file:8f542efd076b9b67ef64928f3c0185ed50bfcbbc3572436a7222e879810d747f in /usr/local/bin/ 
# Fri, 11 Dec 2020 11:40:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 11:40:20 GMT
STOPSIGNAL SIGINT
# Fri, 11 Dec 2020 11:40:21 GMT
EXPOSE 5432
# Fri, 11 Dec 2020 11:40:21 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:b62269920a7a62a905817c7c1b33f33b6e658121e9a054715ff052a23f7de3a0`  
		Last Modified: Fri, 11 Dec 2020 02:01:43 GMT  
		Size: 2.8 MB (2791504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21318200c9ffca0d89785f9d6133303f6c170c0b6c4b194668806cb6de2493a2`  
		Last Modified: Fri, 11 Dec 2020 12:20:11 GMT  
		Size: 1.2 KB (1248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bfd14765d20bb204499946368aa573d0a3fec716ac647c4515c067ac51be203`  
		Last Modified: Fri, 11 Dec 2020 12:20:10 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b82f7d2e38a5ebc50d04c53b65361d4d22c129ff49746611c81dfff3e012ee0`  
		Last Modified: Fri, 11 Dec 2020 12:20:25 GMT  
		Size: 62.9 MB (62929835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b5a7b3e7f1e53f92722ed0e7cada8e43423ae5959321d3b904365fcad033563`  
		Last Modified: Fri, 11 Dec 2020 12:20:08 GMT  
		Size: 8.5 KB (8541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2add4eaf1036a38ab9bd23558751bb08161ecdae9efd20528059285e800cd375`  
		Last Modified: Fri, 11 Dec 2020 12:20:08 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ba32f7f04b2f774eaf4537f6a073b476bdd275bb9733d2996d9c9552a653d63`  
		Last Modified: Fri, 11 Dec 2020 12:20:09 GMT  
		Size: 164.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8a81fbf175305fbba265c5e1734952624b4fb74e69189a3ca744331f00c5849`  
		Last Modified: Fri, 11 Dec 2020 12:20:09 GMT  
		Size: 4.3 KB (4261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:alpine` - linux; ppc64le

```console
$ docker pull postgres@sha256:5d15265326367f308605ecbdf056d0ec005d18b2a266ab5887fd4aaaa98f0c2d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.5 MB (64544553 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c9b5507dc4c2fddce9f9491c4ee490e178c3eef427c46bd0d879327f6e3dff97`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Fri, 11 Dec 2020 03:30:29 GMT
ADD file:9b4b44ee9eaddedc13f114bb55c9abeabceff6abd47f4a660734e431d22fcdce in / 
# Fri, 11 Dec 2020 03:30:32 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 13:06:42 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Fri, 11 Dec 2020 13:06:51 GMT
ENV LANG=en_US.utf8
# Fri, 11 Dec 2020 13:07:03 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 11 Dec 2020 13:07:08 GMT
ENV PG_MAJOR=13
# Fri, 11 Dec 2020 13:07:10 GMT
ENV PG_VERSION=13.1
# Fri, 11 Dec 2020 13:07:13 GMT
ENV PG_SHA256=12345c83b89aa29808568977f5200d6da00f88a035517f925293355432ffe61f
# Fri, 11 Dec 2020 13:11:11 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm10-dev clang g++ 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Fri, 11 Dec 2020 13:11:23 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Fri, 11 Dec 2020 13:11:35 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 11 Dec 2020 13:11:37 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 11 Dec 2020 13:11:46 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 11 Dec 2020 13:11:53 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 11 Dec 2020 13:11:55 GMT
COPY file:8f542efd076b9b67ef64928f3c0185ed50bfcbbc3572436a7222e879810d747f in /usr/local/bin/ 
# Fri, 11 Dec 2020 13:11:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 13:12:02 GMT
STOPSIGNAL SIGINT
# Fri, 11 Dec 2020 13:12:06 GMT
EXPOSE 5432
# Fri, 11 Dec 2020 13:12:10 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:ed596bc4dd0a0c7ff1952005f6cae53a061e1c7998282289586bbfc17a2fd6db`  
		Last Modified: Fri, 11 Dec 2020 03:31:06 GMT  
		Size: 2.8 MB (2803424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35c3e2488105b3059115519bba7a91ba6672f0a1ebe7b539a91ed11db94fc128`  
		Last Modified: Fri, 11 Dec 2020 13:38:46 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41c86b351a0401b8358294a6e6bef969f710f500c7780654b9f1dfbc33e21e2b`  
		Last Modified: Fri, 11 Dec 2020 13:38:47 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27954c6873484b44e77c6cd3b2ff63c73c32d46b0876eea4b4fd882d3c427c57`  
		Last Modified: Fri, 11 Dec 2020 13:38:56 GMT  
		Size: 61.7 MB (61726540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57b2d675f8a0272f85437e16179df3a3c6ad5b5ba911dc6ea2066c91a99114cd`  
		Last Modified: Fri, 11 Dec 2020 13:38:42 GMT  
		Size: 8.5 KB (8540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c2e31d22475d10ca546b0bdbd7b80b3324815b04dd9bf64faf636eecd0e9506`  
		Last Modified: Fri, 11 Dec 2020 13:38:44 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63ba6163759b9cc4140e09103a027a00b6a27e8ae5851000ccf8c856d29bba08`  
		Last Modified: Fri, 11 Dec 2020 13:38:43 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ac4fb973e0b28c7d2f9d9c41c0096236ee9955d55222504e20d22c4621572ae`  
		Last Modified: Fri, 11 Dec 2020 13:38:44 GMT  
		Size: 4.3 KB (4264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:alpine` - linux; s390x

```console
$ docker pull postgres@sha256:2fb40a98c77785ec8f4c3212d49ed6fdd23575ad7cff8e456e618efffe98b5be
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.6 MB (64603192 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4143f93e7c71741aef38704a99766895ebc23e4f89a7b5d80276671890098161`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Fri, 11 Dec 2020 02:09:52 GMT
ADD file:c9395a36a4e03768aabd282eb1f31705cc00181d3147222d9c940eaa5a8fd511 in / 
# Fri, 11 Dec 2020 02:09:53 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 06:15:38 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Fri, 11 Dec 2020 06:15:39 GMT
ENV LANG=en_US.utf8
# Fri, 11 Dec 2020 06:15:41 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 11 Dec 2020 06:15:41 GMT
ENV PG_MAJOR=13
# Fri, 11 Dec 2020 06:15:42 GMT
ENV PG_VERSION=13.1
# Fri, 11 Dec 2020 06:15:42 GMT
ENV PG_SHA256=12345c83b89aa29808568977f5200d6da00f88a035517f925293355432ffe61f
# Fri, 11 Dec 2020 06:19:20 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm10-dev clang g++ 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Fri, 11 Dec 2020 06:19:28 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Fri, 11 Dec 2020 06:19:29 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 11 Dec 2020 06:19:30 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 11 Dec 2020 06:19:31 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 11 Dec 2020 06:19:31 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 11 Dec 2020 06:19:31 GMT
COPY file:8f542efd076b9b67ef64928f3c0185ed50bfcbbc3572436a7222e879810d747f in /usr/local/bin/ 
# Fri, 11 Dec 2020 06:19:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 06:19:32 GMT
STOPSIGNAL SIGINT
# Fri, 11 Dec 2020 06:19:33 GMT
EXPOSE 5432
# Fri, 11 Dec 2020 06:19:33 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:7c2470fe3d16cb70fca0826168095a96838b1322a8cd1502b28284ee8561b491`  
		Last Modified: Fri, 11 Dec 2020 02:10:27 GMT  
		Size: 2.6 MB (2565988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2280b68a5b744783bcdf6324c96fa72156c9296f68b3241b1b5465abc2569ec5`  
		Last Modified: Fri, 11 Dec 2020 06:45:08 GMT  
		Size: 1.3 KB (1277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7a46b2e5e2d8452c04a96097d4e63f442c22347ff9ec33ad63d59c2b8a6110c`  
		Last Modified: Fri, 11 Dec 2020 06:45:08 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cafc4da20bcb281b1a3e4005e2d062fafeb563c14cf70bd1f9a4cd0eb1d2a68`  
		Last Modified: Fri, 11 Dec 2020 06:45:14 GMT  
		Size: 62.0 MB (62022617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc7ee46b1663fa72817d0e88360ec0d5cd6f82ea3ddfcfd0c70571d1155e551f`  
		Last Modified: Fri, 11 Dec 2020 06:45:06 GMT  
		Size: 8.5 KB (8542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:449feb728f58f8c381bc72d8f51f2c09eef8d0707f6aafd88fb57e6d99f6a5d7`  
		Last Modified: Fri, 11 Dec 2020 06:45:06 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23859d9953fea05ff92d6db390cc9e98bcd47f53434d6cc156d96664bada1595`  
		Last Modified: Fri, 11 Dec 2020 06:45:06 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99262ee21175f7f5771861fbff00c1461f5403fa7b06524398ac0c29b15d057c`  
		Last Modified: Fri, 11 Dec 2020 06:45:06 GMT  
		Size: 4.3 KB (4264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
