## `postgres:12-alpine`

```console
$ docker pull postgres@sha256:cd3d70d16d29f1e08b9371986ce16cd21bdd774c562e8917a3ac2eefb200ca15
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

### `postgres:12-alpine` - linux; amd64

```console
$ docker pull postgres@sha256:c8b6b4807ada769b0fb46d1e52fb9b307129c2425a468bc46045d69365a61334
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.6 MB (61615400 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a58cf5527d368041890279fbe3e9c4ab460f5fd168c66639d3a5d5d2b3141e44`
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
# Thu, 15 Apr 2021 03:52:19 GMT
ENV PG_MAJOR=12
# Fri, 14 May 2021 19:44:33 GMT
ENV PG_VERSION=12.7
# Fri, 14 May 2021 19:44:33 GMT
ENV PG_SHA256=8490741f47c88edc8b6624af009ce19fda4dc9b31c4469ce2551d84075d5d995
# Fri, 14 May 2021 19:50:36 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm10-dev clang g++ 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Fri, 14 May 2021 19:50:37 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Fri, 14 May 2021 19:50:38 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 14 May 2021 19:50:38 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 14 May 2021 19:50:39 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 14 May 2021 19:50:40 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 14 May 2021 19:50:40 GMT
COPY file:ad28506adc606e446eefc263bc99d4cb809e608d4f550956143bf13c82c91f85 in /usr/local/bin/ 
# Fri, 14 May 2021 19:50:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 14 May 2021 19:50:40 GMT
STOPSIGNAL SIGINT
# Fri, 14 May 2021 19:50:40 GMT
EXPOSE 5432
# Fri, 14 May 2021 19:50:41 GMT
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
	-	`sha256:3f0f1a7f7d33afbd9e9dd6b8fec8ba01048df807f4bbe67bdf80b776ee82d3f0`  
		Last Modified: Fri, 14 May 2021 20:12:03 GMT  
		Size: 58.8 MB (58788997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f65e3924365741b930da376a9b40c240bcf61531f76aa3b06f7de030d279a46`  
		Last Modified: Fri, 14 May 2021 20:11:55 GMT  
		Size: 8.2 KB (8247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44817ec3b5bbe3b2455c5103409da192c8a74a17741d67574cddf8e7b1d636f0`  
		Last Modified: Fri, 14 May 2021 20:11:54 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:310cea271e8973c592bf81368fadbb5b706fc940213774bcfed0b95bd3cf9259`  
		Last Modified: Fri, 14 May 2021 20:11:55 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:717b5444b286b70ae9faed00103216a34f9ba6a2dfdb8297c2f531bec86c3ff3`  
		Last Modified: Fri, 14 May 2021 20:11:54 GMT  
		Size: 4.4 KB (4405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:12-alpine` - linux; arm variant v6

```console
$ docker pull postgres@sha256:555551264cc6293ba7be62d24547730f45ddb7c39b564d44580ebd6f233bc00f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.0 MB (60003543 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1017971bbaf8002577df540f58e3e156bc419f0bf18bea5a64c9c489c7e380c1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Wed, 14 Apr 2021 18:49:39 GMT
ADD file:4479f0a51530e039edf231d87201896dcff908aa542a613cdccb015f93dda8a3 in / 
# Wed, 14 Apr 2021 18:49:40 GMT
CMD ["/bin/sh"]
# Thu, 15 Apr 2021 02:39:44 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 15 Apr 2021 02:39:45 GMT
ENV LANG=en_US.utf8
# Thu, 15 Apr 2021 02:39:48 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 15 Apr 2021 02:47:59 GMT
ENV PG_MAJOR=12
# Fri, 14 May 2021 20:15:40 GMT
ENV PG_VERSION=12.7
# Fri, 14 May 2021 20:15:42 GMT
ENV PG_SHA256=8490741f47c88edc8b6624af009ce19fda4dc9b31c4469ce2551d84075d5d995
# Fri, 14 May 2021 20:19:28 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm10-dev clang g++ 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Fri, 14 May 2021 20:19:34 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Fri, 14 May 2021 20:19:38 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 14 May 2021 20:19:38 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 14 May 2021 20:19:41 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 14 May 2021 20:19:42 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 14 May 2021 20:19:44 GMT
COPY file:ad28506adc606e446eefc263bc99d4cb809e608d4f550956143bf13c82c91f85 in /usr/local/bin/ 
# Fri, 14 May 2021 20:19:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 14 May 2021 20:19:47 GMT
STOPSIGNAL SIGINT
# Fri, 14 May 2021 20:19:47 GMT
EXPOSE 5432
# Fri, 14 May 2021 20:19:48 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:740c950346cf39c85b52576998695c9b909c24a58a8bb1b64cce91fda3ef1d3a`  
		Last Modified: Wed, 14 Apr 2021 18:50:30 GMT  
		Size: 2.6 MB (2622131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb015ae0de556d839b1cce178f0d7aac974efbf85f07dae41e1cb18f4704b7f2`  
		Last Modified: Thu, 15 Apr 2021 03:12:23 GMT  
		Size: 1.3 KB (1278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce063f2d27607cdd3336512bf1e2cdeb8caa1488efded3002dcaf4c6c267a296`  
		Last Modified: Thu, 15 Apr 2021 03:12:23 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f924948cdf26ec61b02d1bba986d70c2a676db544fb1890b1f240d3aad87fb3`  
		Last Modified: Fri, 14 May 2021 20:31:50 GMT  
		Size: 57.4 MB (57366974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf2c58f441e904dbdcc13497f28e18a4bb375c1c9f7a5d343eb9313a0e406c40`  
		Last Modified: Fri, 14 May 2021 20:31:33 GMT  
		Size: 8.3 KB (8251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62def16f2d7a39009c2a267586486d1f5847429507f7e721fb50849d7edaaf75`  
		Last Modified: Fri, 14 May 2021 20:31:33 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a16df48e26042b75b55147c11b3509e275f5a688cad0baf6a8366911892cae9f`  
		Last Modified: Fri, 14 May 2021 20:31:33 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c04bb9a5b45e22d1026f8e9156a4eb71a54c5a2379f6a6cc9319585605d4571`  
		Last Modified: Fri, 14 May 2021 20:31:33 GMT  
		Size: 4.4 KB (4404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:12-alpine` - linux; arm variant v7

```console
$ docker pull postgres@sha256:def47edb1ff4eb75a44de30be8efc4ccb6444e2ff6352fe39b8e01c8d40310f5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.1 MB (57055449 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66b7a9e45239f1d7b2223de1fe09d995cca6c3311687a69c0bea31859b039e7d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Wed, 14 Apr 2021 18:57:39 GMT
ADD file:028c5b473d862250586e174c5dd19b37f8fc3bffbc02d888e72df30f32fd6129 in / 
# Wed, 14 Apr 2021 18:57:39 GMT
CMD ["/bin/sh"]
# Thu, 15 Apr 2021 03:45:28 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 15 Apr 2021 03:45:30 GMT
ENV LANG=en_US.utf8
# Thu, 15 Apr 2021 03:45:35 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 15 Apr 2021 03:50:36 GMT
ENV PG_MAJOR=12
# Fri, 14 May 2021 21:04:43 GMT
ENV PG_VERSION=12.7
# Fri, 14 May 2021 21:04:44 GMT
ENV PG_SHA256=8490741f47c88edc8b6624af009ce19fda4dc9b31c4469ce2551d84075d5d995
# Fri, 14 May 2021 21:08:03 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm10-dev clang g++ 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Fri, 14 May 2021 21:08:11 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Fri, 14 May 2021 21:08:19 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 14 May 2021 21:08:20 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 14 May 2021 21:08:28 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 14 May 2021 21:08:30 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 14 May 2021 21:08:32 GMT
COPY file:ad28506adc606e446eefc263bc99d4cb809e608d4f550956143bf13c82c91f85 in /usr/local/bin/ 
# Fri, 14 May 2021 21:08:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 14 May 2021 21:08:35 GMT
STOPSIGNAL SIGINT
# Fri, 14 May 2021 21:08:36 GMT
EXPOSE 5432
# Fri, 14 May 2021 21:08:37 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:e160e00eb35d5bc2373770873fbc9c8f5706045b0b06bfd1c364fcf69f02e9fe`  
		Last Modified: Wed, 14 Apr 2021 18:58:36 GMT  
		Size: 2.4 MB (2424145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d289031c7f8e86cc05ec575d7c122bc6d615e827ae76e96bca00fd9b0bba9dfb`  
		Last Modified: Thu, 15 Apr 2021 04:10:49 GMT  
		Size: 1.3 KB (1275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65b79752b7fbad651a271862e12e829d3ce7258cfa9386e5945f7c4232008d57`  
		Last Modified: Thu, 15 Apr 2021 04:10:49 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fcbc67f3d3cb46b7af6cc138179976337228e7ef33341e0f41d04ca13527ec2`  
		Last Modified: Fri, 14 May 2021 22:19:39 GMT  
		Size: 54.6 MB (54616869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc875b5e6dccb9d8b2168dbdfc8e7743bd14eb92967645fda5aa0ac92e088f70`  
		Last Modified: Fri, 14 May 2021 22:19:20 GMT  
		Size: 8.3 KB (8252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1d581280869c44166ad9baac707258546fa94766c02db3eb1a9e12154453b08`  
		Last Modified: Fri, 14 May 2021 22:19:19 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d0394f8ab5ed2d22c62ec885798ea248cf3f58cc18327923a2d2edf747dc88e`  
		Last Modified: Fri, 14 May 2021 22:19:19 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3d2eca38d744a32c6ea6dfaf14d2519f78df143dad15a8a17979e00feffd9d3`  
		Last Modified: Fri, 14 May 2021 22:19:19 GMT  
		Size: 4.4 KB (4406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:12-alpine` - linux; arm64 variant v8

```console
$ docker pull postgres@sha256:4e016a23c8ee655e85b85248d0c65568f3edc7dac424fae1c1fcbc68700b879c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.3 MB (61317806 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb7dbe557017fa6a27fc01b561e408a16a179a75b38be238c1bf1794daa74e57`
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
# Wed, 16 Jun 2021 08:40:20 GMT
ENV PG_MAJOR=12
# Wed, 16 Jun 2021 08:40:20 GMT
ENV PG_VERSION=12.7
# Wed, 16 Jun 2021 08:40:21 GMT
ENV PG_SHA256=8490741f47c88edc8b6624af009ce19fda4dc9b31c4469ce2551d84075d5d995
# Wed, 16 Jun 2021 08:44:52 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm10-dev clang g++ 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Wed, 16 Jun 2021 08:44:53 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Wed, 16 Jun 2021 08:44:54 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Wed, 16 Jun 2021 08:44:54 GMT
ENV PGDATA=/var/lib/postgresql/data
# Wed, 16 Jun 2021 08:44:55 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Wed, 16 Jun 2021 08:44:55 GMT
VOLUME [/var/lib/postgresql/data]
# Wed, 16 Jun 2021 08:44:55 GMT
COPY file:ad28506adc606e446eefc263bc99d4cb809e608d4f550956143bf13c82c91f85 in /usr/local/bin/ 
# Wed, 16 Jun 2021 08:44:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Jun 2021 08:44:55 GMT
STOPSIGNAL SIGINT
# Wed, 16 Jun 2021 08:44:56 GMT
EXPOSE 5432
# Wed, 16 Jun 2021 08:44:56 GMT
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
	-	`sha256:5723b6efc7a1d6c271ff21951f51b906d59e6035ad6746f695a9e4606442da3d`  
		Last Modified: Wed, 16 Jun 2021 09:27:27 GMT  
		Size: 58.6 MB (58591339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46f643894e88238cd3c80652882cf867c02dfa228f96b4eefb1d506fa5f1bdc6`  
		Last Modified: Wed, 16 Jun 2021 09:27:16 GMT  
		Size: 8.2 KB (8250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56c7961a07aea568c36de399b8ea0b4775e6a9ca552383c44073fab3cc36b6b4`  
		Last Modified: Wed, 16 Jun 2021 09:27:16 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1aa822a6d14bb4a0bdb8c688013446505b6181bae69342d1d01e16cb0e908fc6`  
		Last Modified: Wed, 16 Jun 2021 09:27:17 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:837a81400b07190de6fab5d51dfc92de92af2ff864f093c79d596fae7b687424`  
		Last Modified: Wed, 16 Jun 2021 09:27:16 GMT  
		Size: 4.4 KB (4406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:12-alpine` - linux; 386

```console
$ docker pull postgres@sha256:94e69f810277fb96d1ee48886d194a5250c9513b433004a3ec8a62ef21ceb181
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.2 MB (65170064 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f9e0c0820fe259b645b2b49429528f08ca87a5c2a6daa6da95a5d6b6914adbc4`
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
# Thu, 15 Apr 2021 06:14:11 GMT
ENV PG_MAJOR=12
# Fri, 14 May 2021 20:03:42 GMT
ENV PG_VERSION=12.7
# Fri, 14 May 2021 20:03:42 GMT
ENV PG_SHA256=8490741f47c88edc8b6624af009ce19fda4dc9b31c4469ce2551d84075d5d995
# Fri, 14 May 2021 20:11:39 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm10-dev clang g++ 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Fri, 14 May 2021 20:11:40 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Fri, 14 May 2021 20:11:41 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 14 May 2021 20:11:42 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 14 May 2021 20:11:42 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 14 May 2021 20:11:43 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 14 May 2021 20:11:43 GMT
COPY file:ad28506adc606e446eefc263bc99d4cb809e608d4f550956143bf13c82c91f85 in /usr/local/bin/ 
# Fri, 14 May 2021 20:11:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 14 May 2021 20:11:43 GMT
STOPSIGNAL SIGINT
# Fri, 14 May 2021 20:11:43 GMT
EXPOSE 5432
# Fri, 14 May 2021 20:11:44 GMT
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
	-	`sha256:32c4297f502a98a47ce91450471db573f05946795cd8e67f1951f72efc127d7c`  
		Last Modified: Fri, 14 May 2021 20:30:56 GMT  
		Size: 62.3 MB (62336730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb9132cb643517cd8e4580d69d07ed55f7e7ed0606eb4eee62064c6a2e825fef`  
		Last Modified: Fri, 14 May 2021 20:30:44 GMT  
		Size: 8.2 KB (8249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaf425f810065b19930f4b6a903f87bbdfb0df0ac334bfd6919af63842861416`  
		Last Modified: Fri, 14 May 2021 20:30:45 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3060b61bf406da942cfc42d6c2e79e9256435e961e1f396b7f91ab1c27a1a627`  
		Last Modified: Fri, 14 May 2021 20:30:44 GMT  
		Size: 192.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:115e99259b9e33ecf3eabd7152ab13652929d4536ee18f36f6db6cb8e61e5c57`  
		Last Modified: Fri, 14 May 2021 20:30:44 GMT  
		Size: 4.4 KB (4406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:12-alpine` - linux; ppc64le

```console
$ docker pull postgres@sha256:f78f9956eb182a092b5f570a4dbf09aebdbe8d8ef91fc46030bdea3ca07ac310
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.0 MB (64017579 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1fca45427c2abfaa2d78de5951801bd4c9df0e6c5169dbdb082b58c5e1e8df13`
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
# Thu, 15 Apr 2021 04:43:46 GMT
ENV PG_MAJOR=12
# Fri, 14 May 2021 20:23:01 GMT
ENV PG_VERSION=12.7
# Fri, 14 May 2021 20:23:17 GMT
ENV PG_SHA256=8490741f47c88edc8b6624af009ce19fda4dc9b31c4469ce2551d84075d5d995
# Fri, 14 May 2021 20:28:04 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm10-dev clang g++ 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Fri, 14 May 2021 20:28:35 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Fri, 14 May 2021 20:29:12 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 14 May 2021 20:29:51 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 14 May 2021 20:30:18 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 14 May 2021 20:30:29 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 14 May 2021 20:30:32 GMT
COPY file:ad28506adc606e446eefc263bc99d4cb809e608d4f550956143bf13c82c91f85 in /usr/local/bin/ 
# Fri, 14 May 2021 20:30:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 14 May 2021 20:30:47 GMT
STOPSIGNAL SIGINT
# Fri, 14 May 2021 20:30:58 GMT
EXPOSE 5432
# Fri, 14 May 2021 20:31:08 GMT
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
	-	`sha256:623374fe97d0d9b5f56538d7ba6e4d446edb20431d5071ce34e34015b3d59404`  
		Last Modified: Fri, 14 May 2021 21:06:38 GMT  
		Size: 61.2 MB (61189996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bbe81da92e6cb8941121fde31a0c7c8d82cf96487b279c0b159f7885dfbf54b`  
		Last Modified: Fri, 14 May 2021 21:05:40 GMT  
		Size: 8.3 KB (8254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3adbcfb3ea811a3455a55d95476f859749aa30123ab668f01c8f512e07ea2944`  
		Last Modified: Fri, 14 May 2021 21:05:40 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcc27891f80a31dc0ac58ea491c2a8110d755a9dc597630e44b7a6740b3539e2`  
		Last Modified: Fri, 14 May 2021 21:05:41 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d572140e9910189aa35c5efe16900a24db3876989a305f5d9c62e873c68551a`  
		Last Modified: Fri, 14 May 2021 21:05:41 GMT  
		Size: 4.4 KB (4406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:12-alpine` - linux; s390x

```console
$ docker pull postgres@sha256:1682771b158921892a5cca1b08089661099848897db1390c86caafbd95d53a42
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.2 MB (64242199 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:20a7b425a3e8cd4bc4750150aeaaf509043cb14c8c1c8bc856235edccd064a2c`
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
# Thu, 15 Apr 2021 02:39:22 GMT
ENV PG_MAJOR=12
# Fri, 14 May 2021 20:16:18 GMT
ENV PG_VERSION=12.7
# Fri, 14 May 2021 20:16:18 GMT
ENV PG_SHA256=8490741f47c88edc8b6624af009ce19fda4dc9b31c4469ce2551d84075d5d995
# Fri, 14 May 2021 20:20:04 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm10-dev clang g++ 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Fri, 14 May 2021 20:20:07 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Fri, 14 May 2021 20:20:08 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 14 May 2021 20:20:08 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 14 May 2021 20:20:09 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 14 May 2021 20:20:09 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 14 May 2021 20:20:09 GMT
COPY file:ad28506adc606e446eefc263bc99d4cb809e608d4f550956143bf13c82c91f85 in /usr/local/bin/ 
# Fri, 14 May 2021 20:20:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 14 May 2021 20:20:10 GMT
STOPSIGNAL SIGINT
# Fri, 14 May 2021 20:20:10 GMT
EXPOSE 5432
# Fri, 14 May 2021 20:20:10 GMT
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
	-	`sha256:158601a14e3fa49f4fb44652e653c8fc8efcbc22eab7ef13b6a72f3b5bb6614d`  
		Last Modified: Fri, 14 May 2021 20:30:07 GMT  
		Size: 61.6 MB (61625119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6d215edfb59559d049735cf1bc25c1ec4257da2a476b2db27d7b65b147aba4a`  
		Last Modified: Fri, 14 May 2021 20:29:59 GMT  
		Size: 8.2 KB (8247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5939afff9e1ee5dd537c8eb52492d0d745e3bcd0060a25ac23cb469014f57256`  
		Last Modified: Fri, 14 May 2021 20:29:59 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a62ad57be056a6774dd712d34fc33a4d6c46a579e59608d87ed614f310ce1858`  
		Last Modified: Fri, 14 May 2021 20:29:59 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fffebdb1951dde65518f8b00382ddf1533ece423ea7d06d6bbd5457714b832c`  
		Last Modified: Fri, 14 May 2021 20:29:59 GMT  
		Size: 4.4 KB (4404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
