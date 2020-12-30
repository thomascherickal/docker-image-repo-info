## `postgres:10-alpine`

```console
$ docker pull postgres@sha256:668e8d23299266b570978d95d498c4f40b4c2038dda208b009ffb2968e76b994
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
$ docker pull postgres@sha256:432d0edc17d031f7ad51f839d017be598313223351cd17da7f41a2f405d03200
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.5 MB (28509068 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bec9f481115c600b7a89684d6c7df852c8a3044106593bc780152fc8e864f36e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:41 GMT
ADD file:ec475c2abb2d46435286b5ae5efacf5b50b1a9e3b6293b69db3c0172b5b9658b in / 
# Thu, 17 Dec 2020 00:19:42 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 00:59:48 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 17 Dec 2020 00:59:49 GMT
ENV LANG=en_US.utf8
# Thu, 17 Dec 2020 00:59:50 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 17 Dec 2020 01:22:04 GMT
ENV PG_MAJOR=10
# Thu, 17 Dec 2020 01:22:04 GMT
ENV PG_VERSION=10.15
# Thu, 17 Dec 2020 01:22:04 GMT
ENV PG_SHA256=5956bce0becffa77883c41594c95a23110b94f10cd66a1157e373c3575921f7e
# Thu, 17 Dec 2020 01:25:26 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Thu, 17 Dec 2020 01:25:27 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Thu, 17 Dec 2020 01:25:28 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 17 Dec 2020 01:25:28 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 17 Dec 2020 01:25:29 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 17 Dec 2020 01:25:29 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 17 Dec 2020 01:25:30 GMT
COPY file:8f542efd076b9b67ef64928f3c0185ed50bfcbbc3572436a7222e879810d747f in /usr/local/bin/ 
# Thu, 17 Dec 2020 01:25:31 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 17 Dec 2020 01:25:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Dec 2020 01:25:31 GMT
STOPSIGNAL SIGINT
# Thu, 17 Dec 2020 01:25:31 GMT
EXPOSE 5432
# Thu, 17 Dec 2020 01:25:31 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:801bfaa63ef2094d770c809815b9e2b9c1194728e5e754ef7bc764030e140cea`  
		Last Modified: Wed, 16 Dec 2020 19:34:50 GMT  
		Size: 2.8 MB (2799066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8392b19747a95c5f0945f923608970a15320af8654f0a299a0fc345f7d2aa926`  
		Last Modified: Thu, 17 Dec 2020 01:35:47 GMT  
		Size: 1.2 KB (1249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae408abf9c34442cb63539f6995aa2f7a7f934c7671d59879da83a8a0d936c6d`  
		Last Modified: Thu, 17 Dec 2020 01:35:45 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ed79f1313c19ef66aa147f598c4960373652fd98eb7864868d2e66da327f4f8`  
		Last Modified: Thu, 17 Dec 2020 01:36:58 GMT  
		Size: 25.7 MB (25696614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32293377c51db721fd491a57a280dfbc822f982ae1edf1f2fee5291c7b3a07ba`  
		Last Modified: Thu, 17 Dec 2020 01:36:51 GMT  
		Size: 7.4 KB (7351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb8522ebd752fa2d6cffba81c3926ae3581095e862a3454ebd3346d166f3e0b8`  
		Last Modified: Thu, 17 Dec 2020 01:36:52 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75cb175eed12b2d1e5c8ffadf454d3f66904f75e2f2d0cf33ba93cdfca3c9218`  
		Last Modified: Thu, 17 Dec 2020 01:36:51 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca03df5a634c593f57fee9bbfe5d5de37d11c0ebf730267e36acd9fb1ef092d2`  
		Last Modified: Thu, 17 Dec 2020 01:36:52 GMT  
		Size: 4.3 KB (4260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:910cfd7e122f93812e753b7c27e3bf82ffff12b1bdfc64cc8bd92bfe58a7f402`  
		Last Modified: Thu, 17 Dec 2020 01:36:51 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:10-alpine` - linux; arm variant v6

```console
$ docker pull postgres@sha256:c5ea68a339670824084a5663e792de79528a9beab0c05c2da8a68973eb74bd53
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.6 MB (27611582 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f0bd36892b4744de1b5bb83c3cc11b81e6cffb6981ca7ecebbb7ba0482dcf036`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Wed, 16 Dec 2020 23:49:43 GMT
ADD file:0a16715e2d0e5811c3c578945d618db0e269847a799340248f9ba8d393c9eec2 in / 
# Wed, 16 Dec 2020 23:49:45 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 05:45:15 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 17 Dec 2020 05:45:16 GMT
ENV LANG=en_US.utf8
# Thu, 17 Dec 2020 05:45:18 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 17 Dec 2020 06:00:23 GMT
ENV PG_MAJOR=10
# Thu, 17 Dec 2020 06:00:23 GMT
ENV PG_VERSION=10.15
# Thu, 17 Dec 2020 06:00:24 GMT
ENV PG_SHA256=5956bce0becffa77883c41594c95a23110b94f10cd66a1157e373c3575921f7e
# Fri, 18 Dec 2020 20:41:02 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Fri, 18 Dec 2020 20:41:05 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Fri, 18 Dec 2020 20:41:06 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 18 Dec 2020 20:41:07 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 18 Dec 2020 20:41:09 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 18 Dec 2020 20:41:09 GMT
VOLUME [/var/lib/postgresql/data]
# Wed, 30 Dec 2020 00:55:32 GMT
COPY file:f937c0ee3ab8736d7adeefe3108ce546c352d85751a620058fb9427c3648a82c in /usr/local/bin/ 
# Wed, 30 Dec 2020 00:55:35 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 30 Dec 2020 00:55:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 30 Dec 2020 00:55:38 GMT
STOPSIGNAL SIGINT
# Wed, 30 Dec 2020 00:55:40 GMT
EXPOSE 5432
# Wed, 30 Dec 2020 00:55:42 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:93247449aef3c56eb4f7ab7b3fed95743c974b823def6dd86ec84008126e7903`  
		Last Modified: Wed, 16 Dec 2020 23:50:24 GMT  
		Size: 2.6 MB (2604163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8281cbd4bde01cbf0ed0e8ecf5550798d848c1d7d2d642a0416759d8df635f3`  
		Last Modified: Thu, 17 Dec 2020 06:08:22 GMT  
		Size: 1.3 KB (1276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eae834cabab68fcc6ee1f251914773d8111eba34640f8849961845844a4f4681`  
		Last Modified: Thu, 17 Dec 2020 06:08:22 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ad8020dbf3ca99d19f18d4c74f20d772013ff958e21487f0afd379e0dab8c4a`  
		Last Modified: Fri, 18 Dec 2020 20:48:13 GMT  
		Size: 25.0 MB (24993774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46e8c58f6550f444ea1fc3a255287fe9fec9cb07b601ad8a59c884a26d82e98a`  
		Last Modified: Fri, 18 Dec 2020 20:48:03 GMT  
		Size: 7.4 KB (7355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09c3c12c953acffb31bd0818c5f2de1722ec938c39467a4508ead7559280cfd1`  
		Last Modified: Fri, 18 Dec 2020 20:48:03 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0039cdb7cf97c955b1fae739c051ffcb18bb958a39545849508005703d742a0c`  
		Last Modified: Fri, 18 Dec 2020 20:48:03 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f92b73b8242e1f0ffaf5b0771d24edfe6cefb312218d5129b8b4f0adf962cba7`  
		Last Modified: Wed, 30 Dec 2020 00:57:05 GMT  
		Size: 4.4 KB (4391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:beacb8b285674c4be7c2581f59fc9665ad5647b321e5717c0b2a01b5a7438031`  
		Last Modified: Wed, 30 Dec 2020 00:57:05 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:10-alpine` - linux; arm variant v7

```console
$ docker pull postgres@sha256:e936644ba6039c2211682b66148faefe075a7e90fa076e1091da3182a42414c1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.6 MB (26558364 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:10689478ceb997bfa059e721e5c5c575fe52ccbd1ac2a79c513b16fed8604437`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Wed, 16 Dec 2020 23:58:14 GMT
ADD file:bd07f77a2b2741ca6bda80d9203be9c7274cf73145bff778cf000db0d8d4e903 in / 
# Wed, 16 Dec 2020 23:58:15 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 05:35:59 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 17 Dec 2020 05:36:01 GMT
ENV LANG=en_US.utf8
# Thu, 17 Dec 2020 05:36:05 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 17 Dec 2020 05:47:34 GMT
ENV PG_MAJOR=10
# Thu, 17 Dec 2020 05:47:36 GMT
ENV PG_VERSION=10.15
# Thu, 17 Dec 2020 05:47:39 GMT
ENV PG_SHA256=5956bce0becffa77883c41594c95a23110b94f10cd66a1157e373c3575921f7e
# Thu, 17 Dec 2020 05:50:25 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Thu, 17 Dec 2020 05:50:32 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Thu, 17 Dec 2020 05:50:36 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 17 Dec 2020 05:50:37 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 17 Dec 2020 05:50:41 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 17 Dec 2020 05:50:43 GMT
VOLUME [/var/lib/postgresql/data]
# Wed, 30 Dec 2020 01:03:00 GMT
COPY file:f937c0ee3ab8736d7adeefe3108ce546c352d85751a620058fb9427c3648a82c in /usr/local/bin/ 
# Wed, 30 Dec 2020 01:03:02 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 30 Dec 2020 01:03:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 30 Dec 2020 01:03:06 GMT
STOPSIGNAL SIGINT
# Wed, 30 Dec 2020 01:03:08 GMT
EXPOSE 5432
# Wed, 30 Dec 2020 01:03:10 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:c58e8a26a8407acc3ead776f6526efa889fda03270a8d05109208d9f59159420`  
		Last Modified: Wed, 16 Dec 2020 23:58:59 GMT  
		Size: 2.4 MB (2407555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81fd93cc6a1e39bdb8121ae35ee402c25416b317da7efd7e27a38a4af80710b7`  
		Last Modified: Thu, 17 Dec 2020 05:58:49 GMT  
		Size: 1.3 KB (1277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9fc827812b79452d91ced463793937316b84ae0d091f1be8f633999b998bf4b`  
		Last Modified: Thu, 17 Dec 2020 05:58:48 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3542d42495843bc963a255be1401b985c82d4bc0280f98fdbd64ff043796261e`  
		Last Modified: Thu, 17 Dec 2020 06:00:22 GMT  
		Size: 24.1 MB (24137157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b42815488bf74222c6c200312fd0b38f46ae0126ba2d87ef3b7607f10fcf482`  
		Last Modified: Thu, 17 Dec 2020 06:00:13 GMT  
		Size: 7.4 KB (7353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ea4664b16480afafbb948b0cd72ab1aee191a5c1ab1f06d7e712295a106f3bb`  
		Last Modified: Thu, 17 Dec 2020 06:00:14 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c3a40a4df7ca462d5c4ab70150ef724ac4a4e673340386950d3697a6bb4bccd`  
		Last Modified: Thu, 17 Dec 2020 06:00:13 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ec68f0b66ae8b746c9ae6e281ef7e3c721f714cdeb372387c47402835748c67`  
		Last Modified: Wed, 30 Dec 2020 01:05:50 GMT  
		Size: 4.4 KB (4397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:419d28c527af1b7779659d53e6dcdd2bf7f2aed3d71ceec07f7adcd3b19df5c1`  
		Last Modified: Wed, 30 Dec 2020 01:05:50 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:10-alpine` - linux; arm64 variant v8

```console
$ docker pull postgres@sha256:6c6bd2b7a6bc9ab02632cd30f764d02cd333a6d187195233d087f44f0ab8c845
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.3 MB (28283222 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:02bfa6655612561c12bccb28af704388827e13a8ce0fdb8ba1b10f2ad36f5e61`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Wed, 16 Dec 2020 23:40:26 GMT
ADD file:a4845c3840a3fd0e41e4635a179cce20c81afc6c02e34e3fd5bd2d535698918b in / 
# Wed, 16 Dec 2020 23:40:29 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 04:01:11 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 17 Dec 2020 04:01:19 GMT
ENV LANG=en_US.utf8
# Thu, 17 Dec 2020 04:01:28 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 17 Dec 2020 04:15:23 GMT
ENV PG_MAJOR=10
# Thu, 17 Dec 2020 04:15:30 GMT
ENV PG_VERSION=10.15
# Thu, 17 Dec 2020 04:15:35 GMT
ENV PG_SHA256=5956bce0becffa77883c41594c95a23110b94f10cd66a1157e373c3575921f7e
# Thu, 17 Dec 2020 04:18:51 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Thu, 17 Dec 2020 04:18:57 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Thu, 17 Dec 2020 04:19:09 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 17 Dec 2020 04:19:12 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 17 Dec 2020 04:19:20 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 17 Dec 2020 04:19:23 GMT
VOLUME [/var/lib/postgresql/data]
# Wed, 30 Dec 2020 00:44:49 GMT
COPY file:f937c0ee3ab8736d7adeefe3108ce546c352d85751a620058fb9427c3648a82c in /usr/local/bin/ 
# Wed, 30 Dec 2020 00:44:52 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 30 Dec 2020 00:44:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 30 Dec 2020 00:44:59 GMT
STOPSIGNAL SIGINT
# Wed, 30 Dec 2020 00:45:02 GMT
EXPOSE 5432
# Wed, 30 Dec 2020 00:45:06 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:159e5727ea618dfe8b08811112e2c51f5bd2b9ae7db9eb214914a65249f70ca0`  
		Last Modified: Wed, 16 Dec 2020 23:41:08 GMT  
		Size: 2.7 MB (2709048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d20223af9aac4511a0a9a78463ff758585620e621be0678319eba90176b7e615`  
		Last Modified: Thu, 17 Dec 2020 04:28:04 GMT  
		Size: 1.3 KB (1283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2482f57ac4ab8ff038d0589f0507eea54d56adf3da98ff95df25c6beb575c1e4`  
		Last Modified: Thu, 17 Dec 2020 04:28:04 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2ccc0e04504a424f63a1feac951b10de52ad101a5e7ad0b3e194812c533a0b6`  
		Last Modified: Thu, 17 Dec 2020 04:29:39 GMT  
		Size: 25.6 MB (25560514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7546b1ff93283ee302258aac08b4c95c585bcd0188146bc0a7882742c91dc418`  
		Last Modified: Thu, 17 Dec 2020 04:29:31 GMT  
		Size: 7.4 KB (7357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fe0fb2eac3a3663f1750eed83a61176783474ee0fc554e911686c26f982aa0a`  
		Last Modified: Thu, 17 Dec 2020 04:29:31 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee397dcc6e12f257e3e7ffa146f136eb35e8e906a18913cc08803ae16a6579f2`  
		Last Modified: Thu, 17 Dec 2020 04:29:30 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc3a843aea85d6ff7402cbcc3bff7c1f81004f9f018f2a3ec6e671d5aaab03a0`  
		Last Modified: Wed, 30 Dec 2020 00:48:25 GMT  
		Size: 4.4 KB (4395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:877d25b332c9bb7a134cd7a32eb33ebc656282d323fd02173a0f8380dd950bef`  
		Last Modified: Wed, 30 Dec 2020 00:48:25 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:10-alpine` - linux; 386

```console
$ docker pull postgres@sha256:0e6c566bca6e1ff159f35cd79ac3d30e1467159a032b41b6f14111c90c37a5c2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.4 MB (29429117 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f3140a9b76430644e0584dfc9c0abeeaa5b1d01a82d56721c2e0bb1c8e5e652`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 17 Dec 2020 00:38:32 GMT
ADD file:de33fda50a142403e842620d20bc4404e66fc4ace16edc6946c4539e8a797458 in / 
# Thu, 17 Dec 2020 00:38:32 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 05:49:55 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 17 Dec 2020 05:49:56 GMT
ENV LANG=en_US.utf8
# Thu, 17 Dec 2020 05:49:56 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 17 Dec 2020 06:02:47 GMT
ENV PG_MAJOR=10
# Thu, 17 Dec 2020 06:02:47 GMT
ENV PG_VERSION=10.15
# Thu, 17 Dec 2020 06:02:47 GMT
ENV PG_SHA256=5956bce0becffa77883c41594c95a23110b94f10cd66a1157e373c3575921f7e
# Fri, 18 Dec 2020 20:45:56 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Fri, 18 Dec 2020 20:45:57 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Fri, 18 Dec 2020 20:45:58 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 18 Dec 2020 20:45:58 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 18 Dec 2020 20:45:59 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 18 Dec 2020 20:45:59 GMT
VOLUME [/var/lib/postgresql/data]
# Wed, 30 Dec 2020 00:41:44 GMT
COPY file:f937c0ee3ab8736d7adeefe3108ce546c352d85751a620058fb9427c3648a82c in /usr/local/bin/ 
# Wed, 30 Dec 2020 00:41:45 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 30 Dec 2020 00:41:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 30 Dec 2020 00:41:45 GMT
STOPSIGNAL SIGINT
# Wed, 30 Dec 2020 00:41:45 GMT
EXPOSE 5432
# Wed, 30 Dec 2020 00:41:46 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:455793c72b878001f0905634ed52a2524ba51796e7377bf00683a85123f7dce9`  
		Last Modified: Thu, 17 Dec 2020 00:39:18 GMT  
		Size: 2.8 MB (2794130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5305178ae8cb85c448e0963870f5425a527c36dae59155568c8da341f4173b82`  
		Last Modified: Thu, 17 Dec 2020 06:07:45 GMT  
		Size: 1.2 KB (1247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f3614159f507682c618782d96e8e35ed8b175b4dff44e39ef793184e39ba180`  
		Last Modified: Thu, 17 Dec 2020 06:07:45 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc4a8bf472bb0e3f06e5b1ca43a6036bca34b7cb8138c57cde3a6a7184c21109`  
		Last Modified: Fri, 18 Dec 2020 20:56:02 GMT  
		Size: 26.6 MB (26621470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4a37f4d1a499c7929c49a6ed120194ed3a6cf96e54e9e86c9af6248dec1b983`  
		Last Modified: Fri, 18 Dec 2020 20:55:53 GMT  
		Size: 7.4 KB (7352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0596f458ed821737966f01a2e22da2531f7d870d9ecf0a4cd3a3a2f983be8aac`  
		Last Modified: Fri, 18 Dec 2020 20:55:53 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:317a89ea78d7d7eafd4f706bbdd51c71205d0e48022372ef963135d8aad269c1`  
		Last Modified: Fri, 18 Dec 2020 20:55:53 GMT  
		Size: 164.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcf969266cdc98bfbc35fdc6116700201b6e48ddd6541f6dc479dccdb4190e86`  
		Last Modified: Wed, 30 Dec 2020 00:43:22 GMT  
		Size: 4.4 KB (4390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6335acfa984d9b847af4c4c6af9c2020a18e2499a17119c22eb46e060d814c4c`  
		Last Modified: Wed, 30 Dec 2020 00:43:23 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:10-alpine` - linux; ppc64le

```console
$ docker pull postgres@sha256:a90ea86e64bcf1fb1faf5e9fa148db9aaaa9285dbe5635cfce799d6ba10bccfc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.7 MB (29673792 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:22024ec0d02583e4e24ee307471c1987ad93c4f33492ec41cc231ad06c32aca2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 17 Dec 2020 00:20:42 GMT
ADD file:0a38c9b4955f8faa79627c166fca80ef342e443a16ce2925a30eeae317bbd786 in / 
# Thu, 17 Dec 2020 00:20:48 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 08:27:05 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 17 Dec 2020 08:27:07 GMT
ENV LANG=en_US.utf8
# Thu, 17 Dec 2020 08:27:16 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 17 Dec 2020 08:43:27 GMT
ENV PG_MAJOR=10
# Thu, 17 Dec 2020 08:43:33 GMT
ENV PG_VERSION=10.15
# Thu, 17 Dec 2020 08:43:37 GMT
ENV PG_SHA256=5956bce0becffa77883c41594c95a23110b94f10cd66a1157e373c3575921f7e
# Thu, 17 Dec 2020 08:46:18 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Thu, 17 Dec 2020 08:46:25 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Thu, 17 Dec 2020 08:46:32 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 17 Dec 2020 08:46:33 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 17 Dec 2020 08:46:41 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 17 Dec 2020 08:46:43 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 17 Dec 2020 08:46:44 GMT
COPY file:8f542efd076b9b67ef64928f3c0185ed50bfcbbc3572436a7222e879810d747f in /usr/local/bin/ 
# Thu, 17 Dec 2020 08:46:51 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 17 Dec 2020 08:46:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Dec 2020 08:47:03 GMT
STOPSIGNAL SIGINT
# Thu, 17 Dec 2020 08:47:10 GMT
EXPOSE 5432
# Thu, 17 Dec 2020 08:47:12 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:a9d343b7bcc225fe7ac17d96a81329510ab7f31a50472311cafe7168d3107317`  
		Last Modified: Thu, 17 Dec 2020 00:21:33 GMT  
		Size: 2.8 MB (2805226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9020dece47a455612905a0f9d5608b39b5cfa68bf304d4473bbbee3f085dce3e`  
		Last Modified: Thu, 17 Dec 2020 08:55:18 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fd7a09fca54bf573268df0318667b22454de76b77537ce6968b9a9e3a5bd2b7`  
		Last Modified: Thu, 17 Dec 2020 08:55:17 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90c6c3331ee1777fcfbe4649379b3202522f5101a1fc43a603dc47e65d37f565`  
		Last Modified: Thu, 17 Dec 2020 08:56:52 GMT  
		Size: 26.9 MB (26855044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:405e59062775a6ceb355d6f1f93a2577a44f639219c8fcd77e481807ce50797b`  
		Last Modified: Thu, 17 Dec 2020 08:56:45 GMT  
		Size: 7.4 KB (7355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:922ebee47b59a2691e8085a7f69e2f22527f414c0080aa7c535df919ab816b8f`  
		Last Modified: Thu, 17 Dec 2020 08:56:44 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d88ec0f13dca77304d617c726f5e8410a29d4e0ef490b3af8d1cbd2eed08758`  
		Last Modified: Thu, 17 Dec 2020 08:56:44 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c40e2207e1963aa86213186f0bc02bdf80833db764144c630e01fa34066b93c`  
		Last Modified: Thu, 17 Dec 2020 08:56:47 GMT  
		Size: 4.3 KB (4259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f7b45e0e171c19342e4b05512148c70665a9da0f78a3fb5e0fb2cb2fb39567f`  
		Last Modified: Thu, 17 Dec 2020 08:56:44 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:10-alpine` - linux; s390x

```console
$ docker pull postgres@sha256:f8d163b3523f259bb51382ab6a87d905da622b3edde3cb6ce25106c8ccb9167f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.3 MB (28271988 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5766add58380ad3776176ed4e557ff5aa2ab9af67266a0aa1b720e1109a3a102`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Wed, 16 Dec 2020 23:41:37 GMT
ADD file:3ad3856d165e8760af85574a8ffa75ca44b7e1b97b64d1d6d4608445efa4b860 in / 
# Wed, 16 Dec 2020 23:41:37 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 09:43:56 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 17 Dec 2020 09:43:57 GMT
ENV LANG=en_US.utf8
# Thu, 17 Dec 2020 09:43:58 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 17 Dec 2020 09:59:53 GMT
ENV PG_MAJOR=10
# Thu, 17 Dec 2020 09:59:53 GMT
ENV PG_VERSION=10.15
# Thu, 17 Dec 2020 09:59:54 GMT
ENV PG_SHA256=5956bce0becffa77883c41594c95a23110b94f10cd66a1157e373c3575921f7e
# Fri, 18 Dec 2020 22:57:52 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Fri, 18 Dec 2020 22:57:57 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Fri, 18 Dec 2020 22:57:59 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 18 Dec 2020 22:58:00 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 18 Dec 2020 22:58:01 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 18 Dec 2020 22:58:02 GMT
VOLUME [/var/lib/postgresql/data]
# Wed, 30 Dec 2020 00:46:17 GMT
COPY file:f937c0ee3ab8736d7adeefe3108ce546c352d85751a620058fb9427c3648a82c in /usr/local/bin/ 
# Wed, 30 Dec 2020 00:46:19 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 30 Dec 2020 00:46:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 30 Dec 2020 00:46:20 GMT
STOPSIGNAL SIGINT
# Wed, 30 Dec 2020 00:46:20 GMT
EXPOSE 5432
# Wed, 30 Dec 2020 00:46:21 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:ee52640a49e15b8b7c8edb66c2d048b26abdee8d828d6e5ef4e10a28cb15a84f`  
		Last Modified: Wed, 16 Dec 2020 23:42:15 GMT  
		Size: 2.6 MB (2567018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec909f7d148e1f5c76f40f0fe4cec25c8a0f55dee05e382db0c692d59f7c084f`  
		Last Modified: Fri, 18 Dec 2020 23:05:49 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fadc63f7954f50d02abf819a5f8693cf92f86873d00c4dd5108f7dbbf5e0c48`  
		Last Modified: Fri, 18 Dec 2020 23:05:48 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95a7337716874753e800a53f4fc1f0be725b3252579a61d2880dd8d23bc5926f`  
		Last Modified: Fri, 18 Dec 2020 23:07:10 GMT  
		Size: 25.7 MB (25691320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f4f4e6818a62a384684299d2e64de0357ebe727f6026da7874ee4a2cbb55366`  
		Last Modified: Fri, 18 Dec 2020 23:07:04 GMT  
		Size: 7.3 KB (7347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d81fc5562ba0439d6de7e23fbc94b0548daba5b453a6a58d482f925062be6132`  
		Last Modified: Fri, 18 Dec 2020 23:07:04 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5d22eedf153df7464433321e6d991f7324dad7d1c1f62cf13ba59c908ae27f1`  
		Last Modified: Fri, 18 Dec 2020 23:07:04 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4eff8a6a94e29574e2ce8e3245fb6d0a957fd5c7f288f96a63b273b106d3da1c`  
		Last Modified: Wed, 30 Dec 2020 00:48:18 GMT  
		Size: 4.4 KB (4395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34350ec438d6f046da1ae62facbf3a5fefe2e9450cd1e38a64567293af20d4ab`  
		Last Modified: Wed, 30 Dec 2020 00:48:18 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
