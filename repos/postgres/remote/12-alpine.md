## `postgres:12-alpine`

```console
$ docker pull postgres@sha256:73afca2e2f0593d1d08b692161880b4fe0ee8c224f7d747e116c32bda0e71ada
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

### `postgres:12-alpine` - linux; amd64

```console
$ docker pull postgres@sha256:c5efe5f512dcf259e7ae5a4611bc9094630538942806f4d9c576b9d921222135
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **82.5 MB (82520689 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3496e5bc48fb8ba14bcf5ff1c1f7b9ed408efb820f880e74cf4769310a7029aa`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Mon, 23 May 2022 19:19:30 GMT
ADD file:8e81116368669ed3dd361bc898d61bff249f524139a239fdaf3ec46869a39921 in / 
# Mon, 23 May 2022 19:19:31 GMT
CMD ["/bin/sh"]
# Wed, 25 May 2022 20:33:22 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Wed, 25 May 2022 20:33:22 GMT
ENV LANG=en_US.utf8
# Wed, 25 May 2022 20:33:23 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 25 May 2022 20:44:22 GMT
ENV PG_MAJOR=12
# Wed, 25 May 2022 20:44:22 GMT
ENV PG_VERSION=12.11
# Wed, 25 May 2022 20:44:22 GMT
ENV PG_SHA256=1026248a5fd2beeaf43e4c7236ac817e56d58b681a335856465dfbc75b3e8302
# Mon, 06 Jun 2022 22:11:16 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm-dev clang g++ 		make 		openldap-dev 		openssl-dev 		perl-dev 		perl-ipc-run 		perl-utils 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-krb5 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 		zstd 		icu-data-full 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Mon, 06 Jun 2022 22:11:16 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample
# Mon, 06 Jun 2022 22:11:17 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Mon, 06 Jun 2022 22:11:17 GMT
ENV PGDATA=/var/lib/postgresql/data
# Mon, 06 Jun 2022 22:11:18 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Mon, 06 Jun 2022 22:11:18 GMT
VOLUME [/var/lib/postgresql/data]
# Mon, 06 Jun 2022 22:11:18 GMT
COPY file:e8928645623137de410cce68a2aa3b22f07a64e6391025598a60f3e461c606a3 in /usr/local/bin/ 
# Mon, 06 Jun 2022 22:11:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 06 Jun 2022 22:11:18 GMT
STOPSIGNAL SIGINT
# Mon, 06 Jun 2022 22:11:18 GMT
EXPOSE 5432
# Mon, 06 Jun 2022 22:11:18 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:2408cc74d12b6cd092bb8b516ba7d5e290f485d3eb9672efc00f0583730179e8`  
		Last Modified: Mon, 23 May 2022 19:09:38 GMT  
		Size: 2.8 MB (2798889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cde4337df78db353166be0e52015f790ef243152b9e250db922937c6c4435943`  
		Last Modified: Wed, 25 May 2022 20:54:14 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55ba5f4947805e5929e7a1bc92a0d59a6aac5ef362202d33f26391fa79e09df9`  
		Last Modified: Wed, 25 May 2022 20:54:14 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a72993f7bb68e179d59f7eb7a2419f31c76dfe47c75386959c8dfa9824d2447c`  
		Last Modified: Mon, 06 Jun 2022 22:19:40 GMT  
		Size: 79.7 MB (79706617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f67ea1d3a2006285259f4bdeab18214396d50069e83c8034fbe96ea75e1662c`  
		Last Modified: Mon, 06 Jun 2022 22:19:29 GMT  
		Size: 8.7 KB (8696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26df0bc07c8a93062b960344cca32d9e11f216216b57f2f5179f67b7d93099d3`  
		Last Modified: Mon, 06 Jun 2022 22:19:29 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a975a6711bdbc3a5bdbe72291d6a8a9273226b9f648081e6f2deb5b9a5dfcce`  
		Last Modified: Mon, 06 Jun 2022 22:19:29 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1273c2f89d31f7719d3dc683fdef0769653cfcdc3191a40be4c8ce5b5d940b0`  
		Last Modified: Mon, 06 Jun 2022 22:19:29 GMT  
		Size: 4.7 KB (4698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:12-alpine` - linux; arm variant v6

```console
$ docker pull postgres@sha256:1edcab643809aa9d3fb481b6fca097332fab126a05273934f34c1643269ced60
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **80.7 MB (80684148 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:acdd237f5c1839dee40e57cde8dfe7e9325b7c1ea469e0355af7e528a87276e0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Mon, 23 May 2022 19:49:32 GMT
ADD file:f7cee617575b5e5a7672d298a519bb8d8b5098efb90aa2a5d7b0510003457d52 in / 
# Mon, 23 May 2022 19:49:33 GMT
CMD ["/bin/sh"]
# Wed, 25 May 2022 22:54:04 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Wed, 25 May 2022 22:54:04 GMT
ENV LANG=en_US.utf8
# Wed, 25 May 2022 22:54:06 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 25 May 2022 23:13:31 GMT
ENV PG_MAJOR=12
# Wed, 25 May 2022 23:13:31 GMT
ENV PG_VERSION=12.11
# Wed, 25 May 2022 23:13:32 GMT
ENV PG_SHA256=1026248a5fd2beeaf43e4c7236ac817e56d58b681a335856465dfbc75b3e8302
# Mon, 06 Jun 2022 21:55:56 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm-dev clang g++ 		make 		openldap-dev 		openssl-dev 		perl-dev 		perl-ipc-run 		perl-utils 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-krb5 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 		zstd 		icu-data-full 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Mon, 06 Jun 2022 21:55:58 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample
# Mon, 06 Jun 2022 21:56:00 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Mon, 06 Jun 2022 21:56:00 GMT
ENV PGDATA=/var/lib/postgresql/data
# Mon, 06 Jun 2022 21:56:01 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Mon, 06 Jun 2022 21:56:02 GMT
VOLUME [/var/lib/postgresql/data]
# Mon, 06 Jun 2022 21:56:02 GMT
COPY file:e8928645623137de410cce68a2aa3b22f07a64e6391025598a60f3e461c606a3 in /usr/local/bin/ 
# Mon, 06 Jun 2022 21:56:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 06 Jun 2022 21:56:03 GMT
STOPSIGNAL SIGINT
# Mon, 06 Jun 2022 21:56:04 GMT
EXPOSE 5432
# Mon, 06 Jun 2022 21:56:04 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:79a25ccaf940855872635c06e7614d9b27dd38ffb5a8adfdb9274dfdc0ea0d87`  
		Last Modified: Mon, 23 May 2022 19:08:47 GMT  
		Size: 2.6 MB (2606142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68ce185d2eacd6b0f61082b66474ba45a2f13ff27bbae2c58ee0b2da085db2db`  
		Last Modified: Wed, 25 May 2022 23:32:05 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c88d0d1f7487195d34ca2fb5493567418f60bf6dc33e0a43e6c3338928710e5`  
		Last Modified: Wed, 25 May 2022 23:32:06 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:717225a02ae87ed1fe2ab43e79c3d89a233cb34255ad4e5320baf5328bedc63b`  
		Last Modified: Mon, 06 Jun 2022 22:13:43 GMT  
		Size: 78.1 MB (78062827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11b5c704036141ea02fdc5e6327e2dfdf9505bc354582a26a06bf58b047696c1`  
		Last Modified: Mon, 06 Jun 2022 22:13:16 GMT  
		Size: 8.7 KB (8692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1674a4bead5044cb28094803c91a7036a0a88db7f55fec96706ac5a3e55663b`  
		Last Modified: Mon, 06 Jun 2022 22:13:16 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:426d97632d943abc11dad2232ad4babeb8cc1a1add8d1b27f2c463953634027f`  
		Last Modified: Mon, 06 Jun 2022 22:13:16 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dad98ab61100499b5e40c32e39d3f05f6a8abc4b4377abcf2c50506681e908c4`  
		Last Modified: Mon, 06 Jun 2022 22:13:16 GMT  
		Size: 4.7 KB (4698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:12-alpine` - linux; arm variant v7

```console
$ docker pull postgres@sha256:25eb6e952d0ef5ae9e5bb48810dd03cb1a546da3b29b3049b01f7d4b59f5d527
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.3 MB (64326508 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1a28cbfc5f6ac40071b910acf089c627f765340739906c9ba542cc0ca9f39133`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Mon, 23 May 2022 18:57:46 GMT
ADD file:72698cc08524b911ebaacf992490707e5a951ddd2fe6edb3fb598e9dc7155049 in / 
# Mon, 23 May 2022 18:57:47 GMT
CMD ["/bin/sh"]
# Wed, 25 May 2022 20:19:26 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Wed, 25 May 2022 20:19:27 GMT
ENV LANG=en_US.utf8
# Wed, 25 May 2022 20:19:29 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 25 May 2022 20:38:47 GMT
ENV PG_MAJOR=12
# Wed, 25 May 2022 20:38:48 GMT
ENV PG_VERSION=12.11
# Wed, 25 May 2022 20:38:48 GMT
ENV PG_SHA256=1026248a5fd2beeaf43e4c7236ac817e56d58b681a335856465dfbc75b3e8302
# Wed, 25 May 2022 20:44:06 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm-dev clang g++ 		make 		openldap-dev 		openssl-dev 		perl-dev 		perl-ipc-run 		perl-utils 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-krb5 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 		zstd 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Wed, 25 May 2022 20:44:08 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample
# Wed, 25 May 2022 20:44:10 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Wed, 25 May 2022 20:44:10 GMT
ENV PGDATA=/var/lib/postgresql/data
# Wed, 25 May 2022 20:44:11 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Wed, 25 May 2022 20:44:12 GMT
VOLUME [/var/lib/postgresql/data]
# Wed, 25 May 2022 20:44:12 GMT
COPY file:e8928645623137de410cce68a2aa3b22f07a64e6391025598a60f3e461c606a3 in /usr/local/bin/ 
# Wed, 25 May 2022 20:44:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 25 May 2022 20:44:13 GMT
STOPSIGNAL SIGINT
# Wed, 25 May 2022 20:44:14 GMT
EXPOSE 5432
# Wed, 25 May 2022 20:44:14 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:6366ba92f08e2418e90171f1e34bd86ecd50fdc95953b3f33b8943c143518eca`  
		Last Modified: Mon, 23 May 2022 18:59:17 GMT  
		Size: 2.4 MB (2411648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1485f2527978c240fce79b602a9c26b17948e5d60d3d518958be1069f0b225e6`  
		Last Modified: Wed, 25 May 2022 20:59:20 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ea3978d0b81cea51a1d3359988fc1b1b202c9020e43fd938e6bbc7611ac1bb5`  
		Last Modified: Wed, 25 May 2022 20:59:20 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88e4cde843b920c898aa968c68f4388103ebbc3cf912f8a08db612d168a43839`  
		Last Modified: Wed, 25 May 2022 21:02:53 GMT  
		Size: 61.9 MB (61899679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9301c7aaab5fda4787d705f10398233b5e40fd71d61457af9236da5ac6dfd8e`  
		Last Modified: Wed, 25 May 2022 21:02:20 GMT  
		Size: 8.7 KB (8691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ce3f5c17cb19f06559182366bbd02eaa037db192cf1599b0748487115edc43f`  
		Last Modified: Wed, 25 May 2022 21:02:20 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb08d33858348e3e0f1fafdbaa9b7a3f6d47b2be9bd95692f0c0a4c47ede1ad4`  
		Last Modified: Wed, 25 May 2022 21:02:20 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25b2391ae2f0772066eb2418a265e8d03dc249ba59b2f7b74bf2ffc7fd6fa5df`  
		Last Modified: Wed, 25 May 2022 21:02:20 GMT  
		Size: 4.7 KB (4699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:12-alpine` - linux; arm64 variant v8

```console
$ docker pull postgres@sha256:d0458a4b6a5ecb9d4e2537d646202ba2b58c54c5d0cff39c832d2f12cf270573
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.4 MB (81409689 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6db3c34c181bfef2e11ec5225f571914d353d8f52f6a458e5ad2b101f29151fa`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Mon, 23 May 2022 19:39:22 GMT
ADD file:3ae36c6c4a1fc43157692da97c6c4fa6c3d0189ba82e2bef7f5aaf4a5e083f18 in / 
# Mon, 23 May 2022 19:39:22 GMT
CMD ["/bin/sh"]
# Wed, 25 May 2022 21:33:04 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Wed, 25 May 2022 21:33:05 GMT
ENV LANG=en_US.utf8
# Wed, 25 May 2022 21:33:06 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 25 May 2022 21:44:26 GMT
ENV PG_MAJOR=12
# Wed, 25 May 2022 21:44:27 GMT
ENV PG_VERSION=12.11
# Wed, 25 May 2022 21:44:28 GMT
ENV PG_SHA256=1026248a5fd2beeaf43e4c7236ac817e56d58b681a335856465dfbc75b3e8302
# Tue, 07 Jun 2022 01:13:39 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm-dev clang g++ 		make 		openldap-dev 		openssl-dev 		perl-dev 		perl-ipc-run 		perl-utils 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-krb5 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 		zstd 		icu-data-full 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Tue, 07 Jun 2022 01:13:40 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample
# Tue, 07 Jun 2022 01:13:40 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 07 Jun 2022 01:13:41 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 07 Jun 2022 01:13:42 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 07 Jun 2022 01:13:43 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 07 Jun 2022 01:13:45 GMT
COPY file:e8928645623137de410cce68a2aa3b22f07a64e6391025598a60f3e461c606a3 in /usr/local/bin/ 
# Tue, 07 Jun 2022 01:13:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 07 Jun 2022 01:13:46 GMT
STOPSIGNAL SIGINT
# Tue, 07 Jun 2022 01:13:47 GMT
EXPOSE 5432
# Tue, 07 Jun 2022 01:13:48 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:b3c136eddcbf2003d3180787cef00f39d46b9fd9e4623178282ad6a8d63ad3b0`  
		Last Modified: Mon, 23 May 2022 19:08:34 GMT  
		Size: 2.7 MB (2694464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:428d3642719badb326ee04030ea97839d69d5a82b8306924e5ebcf3a65b191dc`  
		Last Modified: Wed, 25 May 2022 21:55:55 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bd66d73c4e4594a6a582481c08b74269a6bda983845fb5018e8ff8e00fb5ec1`  
		Last Modified: Wed, 25 May 2022 21:55:56 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6f6da2b61eeff71e25f6ff9ee9303a4008e46a7e4dcefa553cf199c497ce64f`  
		Last Modified: Tue, 07 Jun 2022 01:23:40 GMT  
		Size: 78.7 MB (78700161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfe2abf5227180248968bd533681fb4d8e4d5bca0c797ae5c13e40780c8c82df`  
		Last Modified: Tue, 07 Jun 2022 01:23:29 GMT  
		Size: 8.7 KB (8689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c071944e89db95dd25b0eedce1edf878b165985672bb1bced521be85076aff7`  
		Last Modified: Tue, 07 Jun 2022 01:23:29 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96619c125fd4ddbb93e7bc84a5d6dddf89bc78fa6e6054fa5f94375ff5c04045`  
		Last Modified: Tue, 07 Jun 2022 01:23:29 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9045b01a8028a4c701d86d05bfff9275a4e077965b6f32188fbca2f3e9995be0`  
		Last Modified: Tue, 07 Jun 2022 01:23:29 GMT  
		Size: 4.7 KB (4700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:12-alpine` - linux; 386

```console
$ docker pull postgres@sha256:5d848e2ad45e08ad3486fe5b03c8991f8efd5eea5dff2d461bc07d8ec7a13c64
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.8 MB (87779325 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e083cd2cab2735317b32369f1667bf7efc755c3f8fdfacf23ddf839d2634a6b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Mon, 23 May 2022 19:38:20 GMT
ADD file:1750ccfabfe93636015070d51a6e824cbd738056223421c69d8aaabc38041b18 in / 
# Mon, 23 May 2022 19:38:20 GMT
CMD ["/bin/sh"]
# Wed, 25 May 2022 22:22:31 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Wed, 25 May 2022 22:22:32 GMT
ENV LANG=en_US.utf8
# Wed, 25 May 2022 22:22:33 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 25 May 2022 22:35:25 GMT
ENV PG_MAJOR=12
# Wed, 25 May 2022 22:35:25 GMT
ENV PG_VERSION=12.11
# Wed, 25 May 2022 22:35:26 GMT
ENV PG_SHA256=1026248a5fd2beeaf43e4c7236ac817e56d58b681a335856465dfbc75b3e8302
# Mon, 06 Jun 2022 21:06:24 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm-dev clang g++ 		make 		openldap-dev 		openssl-dev 		perl-dev 		perl-ipc-run 		perl-utils 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-krb5 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 		zstd 		icu-data-full 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Mon, 06 Jun 2022 21:06:24 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample
# Mon, 06 Jun 2022 21:06:25 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Mon, 06 Jun 2022 21:06:26 GMT
ENV PGDATA=/var/lib/postgresql/data
# Mon, 06 Jun 2022 21:06:27 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Mon, 06 Jun 2022 21:06:28 GMT
VOLUME [/var/lib/postgresql/data]
# Mon, 06 Jun 2022 21:06:30 GMT
COPY file:e8928645623137de410cce68a2aa3b22f07a64e6391025598a60f3e461c606a3 in /usr/local/bin/ 
# Mon, 06 Jun 2022 21:06:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 06 Jun 2022 21:06:31 GMT
STOPSIGNAL SIGINT
# Mon, 06 Jun 2022 21:06:32 GMT
EXPOSE 5432
# Mon, 06 Jun 2022 21:06:33 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:bb638a3869eed698f88775c7a48f36f8e22e7c6bbaa98fa1d5678966b619b859`  
		Last Modified: Mon, 23 May 2022 19:09:25 GMT  
		Size: 2.8 MB (2801887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa6b536300ebf44ca3d811d15e76a960dacddafea21867a310b2bc9d308d382e`  
		Last Modified: Wed, 25 May 2022 22:48:02 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c973fe6785aafb3f812e17ca4088d67ed9081ac155d8340dfbfb27e6af6fd4f1`  
		Last Modified: Wed, 25 May 2022 22:48:02 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e65719fe00503c10b79698e708943169ca8cd61b9a3e27e5cd0b1b49432f97d4`  
		Last Modified: Mon, 06 Jun 2022 21:17:24 GMT  
		Size: 85.0 MB (84962378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2c4caf6381e0a43878ea5fcb79d743f38191db3d1ee06a3f9afcb127e71f42b`  
		Last Modified: Mon, 06 Jun 2022 21:17:13 GMT  
		Size: 8.7 KB (8691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7bdcf2d309be40c7ebb4460951eabd67ba5a8120f51cf06e3ab1c507d70c249`  
		Last Modified: Mon, 06 Jun 2022 21:17:13 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65a4f85534d72052227af40db9e8c80bf0f8c80a41c1ffb7d53b26e4c2173535`  
		Last Modified: Mon, 06 Jun 2022 21:17:13 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c391987f7abd8a4a09b8023232ba4ce0aa7edc0e095330dd875ed1b5b319cb0`  
		Last Modified: Mon, 06 Jun 2022 21:17:13 GMT  
		Size: 4.7 KB (4695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:12-alpine` - linux; ppc64le

```console
$ docker pull postgres@sha256:436e72491af6dc8d37f101842e1f8e6edf555ae3b0b3759e23b6b3e83746fdce
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.1 MB (77071258 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:64539e722211b46766296262e1cee0dc721c9e17b4f90689fb2ce5c9a3cf3c87`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Mon, 23 May 2022 19:16:51 GMT
ADD file:6a5450c8a7cee3ceda59e7cb350c54df4139b0f7b7cf49c8b31bb9c01646c3cd in / 
# Mon, 23 May 2022 19:16:53 GMT
CMD ["/bin/sh"]
# Wed, 25 May 2022 21:15:49 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Wed, 25 May 2022 21:15:52 GMT
ENV LANG=en_US.utf8
# Wed, 25 May 2022 21:16:03 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 25 May 2022 21:32:04 GMT
ENV PG_MAJOR=12
# Wed, 25 May 2022 21:32:06 GMT
ENV PG_VERSION=12.11
# Wed, 25 May 2022 21:32:08 GMT
ENV PG_SHA256=1026248a5fd2beeaf43e4c7236ac817e56d58b681a335856465dfbc75b3e8302
# Wed, 25 May 2022 21:36:12 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm-dev clang g++ 		make 		openldap-dev 		openssl-dev 		perl-dev 		perl-ipc-run 		perl-utils 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-krb5 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 		zstd 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Wed, 25 May 2022 21:36:22 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample
# Wed, 25 May 2022 21:36:28 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Wed, 25 May 2022 21:36:31 GMT
ENV PGDATA=/var/lib/postgresql/data
# Wed, 25 May 2022 21:36:35 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Wed, 25 May 2022 21:36:38 GMT
VOLUME [/var/lib/postgresql/data]
# Wed, 25 May 2022 21:36:41 GMT
COPY file:e8928645623137de410cce68a2aa3b22f07a64e6391025598a60f3e461c606a3 in /usr/local/bin/ 
# Wed, 25 May 2022 21:36:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 25 May 2022 21:36:48 GMT
STOPSIGNAL SIGINT
# Wed, 25 May 2022 21:36:54 GMT
EXPOSE 5432
# Wed, 25 May 2022 21:36:57 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:d3deabf2a506ef6f5fa7c2a68bf27047574cef9908b30a97ff2d01ae539b089a`  
		Last Modified: Mon, 23 May 2022 19:09:13 GMT  
		Size: 2.8 MB (2789745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81e62f323795c1329627761f005a9830616ff5334a265f968c101d69c1c0269a`  
		Last Modified: Wed, 25 May 2022 21:48:19 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:071dfcedb35d03138067dfd4563efbfe985d93db17eea877655db88cd18ea7d9`  
		Last Modified: Wed, 25 May 2022 21:48:19 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdd62e20f9db512dbde8fd5f86ce7b622b141c1ca21904032b1127852348ef9e`  
		Last Modified: Wed, 25 May 2022 21:50:33 GMT  
		Size: 74.3 MB (74266325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d9be98704c9c1e3b3798ab6f5e793ae16cb87a076ced40f6b3396da8f9ab9af`  
		Last Modified: Wed, 25 May 2022 21:50:21 GMT  
		Size: 8.7 KB (8693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29dc97255fa714dc322d0b98c79ecc0647bcff114b8851d5c3e4a25089472101`  
		Last Modified: Wed, 25 May 2022 21:50:20 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fb6ca142f9084c592834d462f94c05ce225aa77ac9189857c37257ac57cbd03`  
		Last Modified: Wed, 25 May 2022 21:50:21 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9835349b5d7add3ab5f694d5b86f4512370dedacfe224a5084a0782558af59bb`  
		Last Modified: Wed, 25 May 2022 21:50:20 GMT  
		Size: 4.7 KB (4702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:12-alpine` - linux; s390x

```console
$ docker pull postgres@sha256:efd1a85a98c264b173a2b0b703930138d94b863f00bc8ee1b3d3ceac42c2e498
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **83.6 MB (83617433 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4859503e776d7aeee10e956711dea25e0a069db7b5b50c265540260a9fc85b4b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Mon, 23 May 2022 19:41:59 GMT
ADD file:e1852d8ef555a0d3ef6d0b74a898720c82bb9f491430b06a0dd0499497ce118e in / 
# Mon, 23 May 2022 19:42:10 GMT
CMD ["/bin/sh"]
# Wed, 25 May 2022 21:18:55 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Wed, 25 May 2022 21:18:56 GMT
ENV LANG=en_US.utf8
# Wed, 25 May 2022 21:18:57 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 25 May 2022 21:32:59 GMT
ENV PG_MAJOR=12
# Wed, 25 May 2022 21:32:59 GMT
ENV PG_VERSION=12.11
# Wed, 25 May 2022 21:33:00 GMT
ENV PG_SHA256=1026248a5fd2beeaf43e4c7236ac817e56d58b681a335856465dfbc75b3e8302
# Tue, 07 Jun 2022 03:52:23 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm-dev clang g++ 		make 		openldap-dev 		openssl-dev 		perl-dev 		perl-ipc-run 		perl-utils 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-krb5 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 		zstd 		icu-data-full 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Tue, 07 Jun 2022 03:52:31 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample
# Tue, 07 Jun 2022 03:52:33 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 07 Jun 2022 03:52:33 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 07 Jun 2022 03:52:34 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 07 Jun 2022 03:52:34 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 07 Jun 2022 03:52:34 GMT
COPY file:e8928645623137de410cce68a2aa3b22f07a64e6391025598a60f3e461c606a3 in /usr/local/bin/ 
# Tue, 07 Jun 2022 03:52:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 07 Jun 2022 03:52:35 GMT
STOPSIGNAL SIGINT
# Tue, 07 Jun 2022 03:52:35 GMT
EXPOSE 5432
# Tue, 07 Jun 2022 03:52:35 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:af1ac1a73384e058591d04d19bc05a06781cc32d52d4593b468d6cb95eda9858`  
		Last Modified: Mon, 23 May 2022 19:43:36 GMT  
		Size: 2.6 MB (2580494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e39251492e62d811aa94961c8e28a32e2d839aff833e8cb7d038d68cfa1b31b1`  
		Last Modified: Wed, 25 May 2022 21:48:40 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c159c69cfc44c287422fdef78cc8dbc8c6a88fd4f24d04b8efc313da9b72eda0`  
		Last Modified: Wed, 25 May 2022 21:48:39 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4849ad38dfa40241f20d4d782a934e4a0d87c1301cc247bebec61f364808374d`  
		Last Modified: Tue, 07 Jun 2022 04:03:14 GMT  
		Size: 81.0 MB (81021761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee7842c704199d12e471bcfdbda7ba59d1a315fb2e27e5093747df19746288e3`  
		Last Modified: Tue, 07 Jun 2022 04:03:04 GMT  
		Size: 8.7 KB (8692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb8bef70c1c608944d062825261c096ba0332847825bdb1086e813ba0ea62b82`  
		Last Modified: Tue, 07 Jun 2022 04:03:03 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd274862130ad8d18e54748d5e12deb8d9fa129a4475304fea2a0a0ec8619efd`  
		Last Modified: Tue, 07 Jun 2022 04:03:03 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dc7661c8af440693e5a98fbd7b2f64ae412ff0965028d233da74bbbec23df0e`  
		Last Modified: Tue, 07 Jun 2022 04:03:03 GMT  
		Size: 4.7 KB (4698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
