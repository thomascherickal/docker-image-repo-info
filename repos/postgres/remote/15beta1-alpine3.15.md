## `postgres:15beta1-alpine3.15`

```console
$ docker pull postgres@sha256:b0d8db2b68d7a795a475036476b9b79c32ea31898369c7a372b25b2ff445a44e
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

### `postgres:15beta1-alpine3.15` - linux; amd64

```console
$ docker pull postgres@sha256:b81d966a616365177a55530eb9afafa6606a07a15bf4db0b7d87d3f42e511934
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.8 MB (84823603 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d9b4e2a8d550f34db1b76841becbe3bdd46a4c229147887d0735b8e37d9c1fd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 05 Apr 2022 00:19:59 GMT
ADD file:5d673d25da3a14ce1f6cf66e4c7fd4f4b85a3759a9d93efb3fd9ff852b5b56e4 in / 
# Tue, 05 Apr 2022 00:19:59 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 07:24:39 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Tue, 05 Apr 2022 07:24:39 GMT
ENV LANG=en_US.utf8
# Tue, 05 Apr 2022 07:24:40 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 24 May 2022 19:28:50 GMT
ENV PG_MAJOR=15
# Tue, 24 May 2022 19:28:50 GMT
ENV PG_VERSION=15beta1
# Tue, 24 May 2022 19:28:50 GMT
ENV PG_SHA256=5dd8a466fb0c9eca11f10b1275524fc8f38d1699cac6a689780b49eac878f7af
# Tue, 24 May 2022 19:32:13 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm-dev clang g++ 		make 		openldap-dev 		openssl-dev 		perl-dev 		perl-ipc-run 		perl-utils 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		icu-dev 		lz4-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-krb5 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 		--with-lz4 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 		zstd 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Tue, 24 May 2022 19:32:14 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample
# Tue, 24 May 2022 19:32:14 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 24 May 2022 19:32:14 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 24 May 2022 19:32:15 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 24 May 2022 19:32:15 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 24 May 2022 19:32:15 GMT
COPY file:e8928645623137de410cce68a2aa3b22f07a64e6391025598a60f3e461c606a3 in /usr/local/bin/ 
# Tue, 24 May 2022 19:32:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 24 May 2022 19:32:15 GMT
STOPSIGNAL SIGINT
# Tue, 24 May 2022 19:32:15 GMT
EXPOSE 5432
# Tue, 24 May 2022 19:32:15 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:df9b9388f04ad6279a7410b85cedfdcb2208c0a003da7ab5613af71079148139`  
		Last Modified: Mon, 04 Apr 2022 19:10:16 GMT  
		Size: 2.8 MB (2814559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7902437d3a1288bbe38562c760e4e6b155617991e782f33ddd81da3f4f88305a`  
		Last Modified: Tue, 05 Apr 2022 07:48:12 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:709e2267bc988471d02df06f7a9f133dd3195af6da61c0869b0555f72f0c1e4e`  
		Last Modified: Tue, 05 Apr 2022 07:48:12 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eae4c3b8f10d5daa58724da7a323be1601f4014df22ce134db98a816eafb2229`  
		Last Modified: Tue, 24 May 2022 19:34:11 GMT  
		Size: 82.0 MB (81993102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbaa13105591befa90a9c4159c7130eca863b926f83ff418bd927e8213a11da3`  
		Last Modified: Tue, 24 May 2022 19:34:00 GMT  
		Size: 9.5 KB (9457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e9d5c02d6249ac982cfcac63700f0629b2a9929eafae39444fca72ae6e88fc1`  
		Last Modified: Tue, 24 May 2022 19:34:00 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2035c234b030694c337d1b09d15e48848a5f3e6ed8ed91cfc65d8768d091d7e`  
		Last Modified: Tue, 24 May 2022 19:34:00 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98699342f160b24110e8d1e9fa426b587cf15058c5d689314a9dddc96282926b`  
		Last Modified: Tue, 24 May 2022 19:34:00 GMT  
		Size: 4.7 KB (4697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:15beta1-alpine3.15` - linux; arm variant v6

```console
$ docker pull postgres@sha256:7d0a6c4ecfdf05698870d1ca428a001f6ae60891b92c48e9b411b764a2b32764
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **82.3 MB (82336854 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:04654b2a8cc8947964f31bf856bc4dafd8a61c4e7b82c7a210dfe9da478dfdde`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Mon, 04 Apr 2022 23:49:42 GMT
ADD file:159dcddaab900372df882a4e94615ed84250e9cea3e74bc0479d98280342f596 in / 
# Mon, 04 Apr 2022 23:49:42 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 06:44:13 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Tue, 05 Apr 2022 06:44:13 GMT
ENV LANG=en_US.utf8
# Tue, 05 Apr 2022 06:44:15 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 24 May 2022 20:04:37 GMT
ENV PG_MAJOR=15
# Tue, 24 May 2022 20:04:38 GMT
ENV PG_VERSION=15beta1
# Tue, 24 May 2022 20:04:38 GMT
ENV PG_SHA256=5dd8a466fb0c9eca11f10b1275524fc8f38d1699cac6a689780b49eac878f7af
# Tue, 24 May 2022 20:10:07 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm-dev clang g++ 		make 		openldap-dev 		openssl-dev 		perl-dev 		perl-ipc-run 		perl-utils 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		icu-dev 		lz4-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-krb5 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 		--with-lz4 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 		zstd 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Tue, 24 May 2022 20:10:10 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample
# Tue, 24 May 2022 20:10:11 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 24 May 2022 20:10:11 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 24 May 2022 20:10:13 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 24 May 2022 20:10:13 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 24 May 2022 20:10:14 GMT
COPY file:e8928645623137de410cce68a2aa3b22f07a64e6391025598a60f3e461c606a3 in /usr/local/bin/ 
# Tue, 24 May 2022 20:10:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 24 May 2022 20:10:15 GMT
STOPSIGNAL SIGINT
# Tue, 24 May 2022 20:10:15 GMT
EXPOSE 5432
# Tue, 24 May 2022 20:10:15 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:c319b1fc4ed70b8241a7ce6ac0c4015d354bf5cf8c01eb73c50b6709c0c46e49`  
		Last Modified: Mon, 04 Apr 2022 19:09:22 GMT  
		Size: 2.6 MB (2621972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cb8e77db967e9917c31ab0acb275de8ef6e22c214dfe4e99c2f6aeb9c10b299`  
		Last Modified: Tue, 05 Apr 2022 07:11:18 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d6281d8a0ebe004d81faf000876292bc4f792eb730ac75d51aaeca917db6eb0`  
		Last Modified: Tue, 05 Apr 2022 07:11:18 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68d986262d49f33a3e37f755ef04d914e9423d365cbdd8a39119b6519b3b1266`  
		Last Modified: Tue, 24 May 2022 20:13:52 GMT  
		Size: 79.7 MB (79698936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8606cc0fe50a9a22d037fd1c658dd90986621a1fa7e46b2795598b16d166e370`  
		Last Modified: Tue, 24 May 2022 20:13:05 GMT  
		Size: 9.5 KB (9458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3a9e533cf747f8655cb938757ab33848867c817676ea11f929b6f378f22fb75`  
		Last Modified: Tue, 24 May 2022 20:13:05 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:765fbcc8ac8322095c73ca29c0eccc3b2536a3fe0de72f5a1903c00071bc8102`  
		Last Modified: Tue, 24 May 2022 20:13:05 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69a4cb64c1fd83d1d0cd429645b3c3daeb1f1876b4bfca28d55bd048a93b73ae`  
		Last Modified: Tue, 24 May 2022 20:13:05 GMT  
		Size: 4.7 KB (4702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:15beta1-alpine3.15` - linux; arm variant v7

```console
$ docker pull postgres@sha256:6dce253da96d99568c1817b3a407951f51982d906032dcd4e4cb280c2cbaceea
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.5 MB (77541108 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dbe12c4c0b527896e47c579c0fe51cf900f05ecf3e139f44a7fc911e13b3a6cb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Mon, 04 Apr 2022 23:57:34 GMT
ADD file:20f8cdddc53a4a8bd78945fc32fe08e9f80ab3b16dc20a9aa4ba73b79f2bc71c in / 
# Mon, 04 Apr 2022 23:57:35 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 10:40:04 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Tue, 05 Apr 2022 10:40:05 GMT
ENV LANG=en_US.utf8
# Tue, 05 Apr 2022 10:40:06 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 24 May 2022 23:41:55 GMT
ENV PG_MAJOR=15
# Tue, 24 May 2022 23:41:56 GMT
ENV PG_VERSION=15beta1
# Tue, 24 May 2022 23:41:56 GMT
ENV PG_SHA256=5dd8a466fb0c9eca11f10b1275524fc8f38d1699cac6a689780b49eac878f7af
# Tue, 24 May 2022 23:47:02 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm-dev clang g++ 		make 		openldap-dev 		openssl-dev 		perl-dev 		perl-ipc-run 		perl-utils 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		icu-dev 		lz4-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-krb5 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 		--with-lz4 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 		zstd 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Tue, 24 May 2022 23:47:04 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample
# Tue, 24 May 2022 23:47:06 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 24 May 2022 23:47:06 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 24 May 2022 23:47:08 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 24 May 2022 23:47:08 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 24 May 2022 23:47:09 GMT
COPY file:e8928645623137de410cce68a2aa3b22f07a64e6391025598a60f3e461c606a3 in /usr/local/bin/ 
# Tue, 24 May 2022 23:47:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 24 May 2022 23:47:09 GMT
STOPSIGNAL SIGINT
# Tue, 24 May 2022 23:47:10 GMT
EXPOSE 5432
# Tue, 24 May 2022 23:47:10 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:57fb4b5f1a47c953ca5703f0f81ce14e5d01cf23aa79558b5adb961cc526e320`  
		Last Modified: Mon, 04 Apr 2022 19:09:36 GMT  
		Size: 2.4 MB (2424323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a73a72bdda5eae4bf93e48ab5614ce664c8d55a850cc23684a669ac50d7c562`  
		Last Modified: Tue, 05 Apr 2022 11:08:51 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:900cc3f9e3fa7beceaf45b2dd8fd89c500fa73defa872eeafea1769d75770d73`  
		Last Modified: Tue, 05 Apr 2022 11:08:51 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be79e0c8545b6a5ff9e72da7b964a229aaad271e94b4a3368a7990a715181d5e`  
		Last Modified: Tue, 24 May 2022 23:55:07 GMT  
		Size: 75.1 MB (75100838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25cdc97203399897b42c2e985e3669a12dad932bc66b3a15c720cce0973457d3`  
		Last Modified: Tue, 24 May 2022 23:54:30 GMT  
		Size: 9.5 KB (9459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:317e2805a232ece20af303123f4b843cfcbee1dda20488ff4410a73d6c46919a`  
		Last Modified: Tue, 24 May 2022 23:54:30 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08b402813b65bcd64ecf3da83c8676a3fb60807c2bb5e60d335be2b746b04691`  
		Last Modified: Tue, 24 May 2022 23:54:30 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60f8663016eac0d00a0829dd56b28c676f6c3cc632bcdb629fca71a89f1b65ab`  
		Last Modified: Tue, 24 May 2022 23:54:30 GMT  
		Size: 4.7 KB (4699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:15beta1-alpine3.15` - linux; arm64 variant v8

```console
$ docker pull postgres@sha256:b6af482a1d084a368dae9a366b364d96a2e39564f7b14be3d046c8e33036ee4a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **83.5 MB (83497693 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f355b230360a3cd7d66ed835b57e4b5ab46e140e1ac9fda669d58568bb01f30f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:31 GMT
ADD file:90e56af13188c7f0283d244a0d70b853d8bef8587a41f1da8eac3a2aba8964ef in / 
# Mon, 04 Apr 2022 23:39:31 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 04:22:00 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Tue, 05 Apr 2022 04:22:01 GMT
ENV LANG=en_US.utf8
# Tue, 05 Apr 2022 04:22:02 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 24 May 2022 20:14:43 GMT
ENV PG_MAJOR=15
# Tue, 24 May 2022 20:14:44 GMT
ENV PG_VERSION=15beta1
# Tue, 24 May 2022 20:14:45 GMT
ENV PG_SHA256=5dd8a466fb0c9eca11f10b1275524fc8f38d1699cac6a689780b49eac878f7af
# Tue, 24 May 2022 20:20:38 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm-dev clang g++ 		make 		openldap-dev 		openssl-dev 		perl-dev 		perl-ipc-run 		perl-utils 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		icu-dev 		lz4-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-krb5 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 		--with-lz4 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 		zstd 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Tue, 24 May 2022 20:20:39 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample
# Tue, 24 May 2022 20:20:40 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 24 May 2022 20:20:41 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 24 May 2022 20:20:42 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 24 May 2022 20:20:43 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 24 May 2022 20:20:45 GMT
COPY file:e8928645623137de410cce68a2aa3b22f07a64e6391025598a60f3e461c606a3 in /usr/local/bin/ 
# Tue, 24 May 2022 20:20:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 24 May 2022 20:20:46 GMT
STOPSIGNAL SIGINT
# Tue, 24 May 2022 20:20:47 GMT
EXPOSE 5432
# Tue, 24 May 2022 20:20:48 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:9981e73032c8833e387a8f96986e560edbed12c38119e0edb0439c9c2234eac9`  
		Last Modified: Mon, 04 Apr 2022 19:09:10 GMT  
		Size: 2.7 MB (2716477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9998735be53b82d4d93cc72813622118271d565b9576e178c1cf196b949b56de`  
		Last Modified: Tue, 05 Apr 2022 04:40:33 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51338f5c9ae13e18e64d58b7ceacd16d0004c01ea9a50e77307e9c26794559a5`  
		Last Modified: Tue, 05 Apr 2022 04:40:32 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b52601062474ee739f0d6643e63bcb26f3beae8e28d69fdc61a62c7768217fa`  
		Last Modified: Tue, 24 May 2022 20:24:05 GMT  
		Size: 80.8 MB (80765382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32de514a232b254d88ab4b619dad7507689514f1a1e15bb455a6474d50a41637`  
		Last Modified: Tue, 24 May 2022 20:23:54 GMT  
		Size: 9.5 KB (9457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd7f0b90711221493cf78aa83223c8a19e21494c3bac5727e79e7e18ee85761e`  
		Last Modified: Tue, 24 May 2022 20:23:54 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c27c162f60408e914dcafb5f322a2222b5cfc20f4280c6644b53b8307530d415`  
		Last Modified: Tue, 24 May 2022 20:23:54 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e94ca4e72b705fbf5025fad408417cb7ec78e90842682844ab7cd8b1029588c`  
		Last Modified: Tue, 24 May 2022 20:23:54 GMT  
		Size: 4.7 KB (4703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:15beta1-alpine3.15` - linux; 386

```console
$ docker pull postgres@sha256:1ac76e56e8d2f1b418d2268042264d092a72aad8f2727b0bb05509485ee6a15a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **89.7 MB (89742433 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c9d4f2468867263f2d4dfd7161de92f907bf2d895a7459208514dcfc98663752`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Mon, 04 Apr 2022 23:38:25 GMT
ADD file:7d51a0f8691eb78c9062fd31984423a93d276a67b4ed5d1a706e1c2cd9fea23a in / 
# Mon, 04 Apr 2022 23:38:25 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 04:18:33 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Tue, 05 Apr 2022 04:18:34 GMT
ENV LANG=en_US.utf8
# Tue, 05 Apr 2022 04:18:35 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 24 May 2022 20:05:02 GMT
ENV PG_MAJOR=15
# Tue, 24 May 2022 20:05:03 GMT
ENV PG_VERSION=15beta1
# Tue, 24 May 2022 20:05:04 GMT
ENV PG_SHA256=5dd8a466fb0c9eca11f10b1275524fc8f38d1699cac6a689780b49eac878f7af
# Tue, 24 May 2022 20:08:40 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm-dev clang g++ 		make 		openldap-dev 		openssl-dev 		perl-dev 		perl-ipc-run 		perl-utils 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		icu-dev 		lz4-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-krb5 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 		--with-lz4 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 		zstd 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Tue, 24 May 2022 20:08:41 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample
# Tue, 24 May 2022 20:08:41 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 24 May 2022 20:08:42 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 24 May 2022 20:08:43 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 24 May 2022 20:08:44 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 24 May 2022 20:08:46 GMT
COPY file:e8928645623137de410cce68a2aa3b22f07a64e6391025598a60f3e461c606a3 in /usr/local/bin/ 
# Tue, 24 May 2022 20:08:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 24 May 2022 20:08:47 GMT
STOPSIGNAL SIGINT
# Tue, 24 May 2022 20:08:48 GMT
EXPOSE 5432
# Tue, 24 May 2022 20:08:49 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:73b28a5955ec7fb46f2cf0434e4901a889f7dda3f8c9ec496300feb256c7eda8`  
		Last Modified: Mon, 04 Apr 2022 19:10:03 GMT  
		Size: 2.8 MB (2818974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:440ad7c551279d9f14743cb1f9d3d9c5e5c62431537e922e055ad3d5a9e98ddd`  
		Last Modified: Tue, 05 Apr 2022 04:38:01 GMT  
		Size: 1.3 KB (1256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58f96dc8fa9ed931f47d352471b5f575a1bc1895361bfa37f9b002333ca26c1b`  
		Last Modified: Tue, 05 Apr 2022 04:38:00 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:907b6f10f16c330211e5d7c97f1ada2d4d3193e096d985fdcbc969c6ab6b1677`  
		Last Modified: Tue, 24 May 2022 20:12:26 GMT  
		Size: 86.9 MB (86907628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8efff91aab4ab5394260cd9b4efd5fc09a73fdc0dfc297e76c80ef883f5262c0`  
		Last Modified: Tue, 24 May 2022 20:12:10 GMT  
		Size: 9.5 KB (9456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:955e004994c632afa861e9312b0c76c87273727093126ae60dde3876afb26d08`  
		Last Modified: Tue, 24 May 2022 20:12:10 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd36fba764106f307053751b027be016cb09a8e70fb027a1a155a2c8899a5a1d`  
		Last Modified: Tue, 24 May 2022 20:12:10 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91fa65c006186d151d2dd07d246a756eb7abc99cf4ae29d27b822e8876b659c1`  
		Last Modified: Tue, 24 May 2022 20:12:10 GMT  
		Size: 4.7 KB (4701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:15beta1-alpine3.15` - linux; ppc64le

```console
$ docker pull postgres@sha256:a4e04ff5b2213cc1ab08f28dbd3713a6085d86d06097847bb619b02ca1f3a474
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **90.2 MB (90197211 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0073c61b1f1eba89eb42b0bc6bbcff0dd09f0fa2458b23bd8c7b76271dc95d92`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 05 Apr 2022 00:23:30 GMT
ADD file:960cf6f9d3d1cfcb36c2d67dd4c3eaba7db1d0c7afe97968512248d7f234ad47 in / 
# Tue, 05 Apr 2022 00:23:32 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 10:15:26 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Tue, 05 Apr 2022 10:15:31 GMT
ENV LANG=en_US.utf8
# Tue, 05 Apr 2022 10:15:41 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 24 May 2022 19:39:04 GMT
ENV PG_MAJOR=15
# Tue, 24 May 2022 19:39:06 GMT
ENV PG_VERSION=15beta1
# Tue, 24 May 2022 19:39:09 GMT
ENV PG_SHA256=5dd8a466fb0c9eca11f10b1275524fc8f38d1699cac6a689780b49eac878f7af
# Tue, 24 May 2022 19:44:18 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm-dev clang g++ 		make 		openldap-dev 		openssl-dev 		perl-dev 		perl-ipc-run 		perl-utils 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		icu-dev 		lz4-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-krb5 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 		--with-lz4 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 		zstd 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Tue, 24 May 2022 19:44:34 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample
# Tue, 24 May 2022 19:44:41 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 24 May 2022 19:44:43 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 24 May 2022 19:44:51 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 24 May 2022 19:44:53 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 24 May 2022 19:44:54 GMT
COPY file:e8928645623137de410cce68a2aa3b22f07a64e6391025598a60f3e461c606a3 in /usr/local/bin/ 
# Tue, 24 May 2022 19:44:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 24 May 2022 19:44:59 GMT
STOPSIGNAL SIGINT
# Tue, 24 May 2022 19:45:03 GMT
EXPOSE 5432
# Tue, 24 May 2022 19:45:07 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:1877acf2d48ed8bcb5bd9756a95aca0c077457be7cf4fcef25807f4e9be88db1`  
		Last Modified: Mon, 04 Apr 2022 19:09:49 GMT  
		Size: 2.8 MB (2811186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31d11c39eb8c6d4d061062b829221f428b3acf12369b01b6c042d6a713031c39`  
		Last Modified: Tue, 05 Apr 2022 10:45:10 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf0ff1d52fa2dd7453fce38e8e17b53514b2e104f4e6275e00196f88415a4398`  
		Last Modified: Tue, 05 Apr 2022 10:45:10 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:990183e8c84a4b939e4f0f54a389824a4a8a025d3a9f52169db79aa62a94fd53`  
		Last Modified: Tue, 24 May 2022 19:48:51 GMT  
		Size: 87.4 MB (87370066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd62f117777a73876cde85cd057a21844a7925c5611d7661e14f070a8419d8d0`  
		Last Modified: Tue, 24 May 2022 19:48:36 GMT  
		Size: 9.5 KB (9465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed0dcc1f8c54c9654e7639961b5af385fbad261fd39e346e4507d4754857f215`  
		Last Modified: Tue, 24 May 2022 19:48:36 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d97195e31cdcb570d38dc1d3196b65016bba8af19a37ae8efebe6376da11161`  
		Last Modified: Tue, 24 May 2022 19:48:36 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87bb31b3482f8e9dc9acb7e84ca26307d03c41448382e7477f1702f87a47e147`  
		Last Modified: Tue, 24 May 2022 19:48:36 GMT  
		Size: 4.7 KB (4701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:15beta1-alpine3.15` - linux; s390x

```console
$ docker pull postgres@sha256:27e78fa5d77a5858b746fe22261c4214c309029da221815db61c9954e973c891
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **85.9 MB (85855567 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f5be8c35ee253e5f95b2a520f24c2f1fec9d953e6faebc660f5c71ee72b79926`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Mon, 04 Apr 2022 23:41:39 GMT
ADD file:f22e4b2be87d3c59c8c609acf79015938dc1fba0b26d7c1b59bd0fc36d63a906 in / 
# Mon, 04 Apr 2022 23:41:39 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 06:55:28 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Tue, 05 Apr 2022 06:55:28 GMT
ENV LANG=en_US.utf8
# Tue, 05 Apr 2022 06:55:29 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 24 May 2022 20:08:35 GMT
ENV PG_MAJOR=15
# Tue, 24 May 2022 20:08:36 GMT
ENV PG_VERSION=15beta1
# Tue, 24 May 2022 20:08:36 GMT
ENV PG_SHA256=5dd8a466fb0c9eca11f10b1275524fc8f38d1699cac6a689780b49eac878f7af
# Tue, 24 May 2022 20:12:26 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm-dev clang g++ 		make 		openldap-dev 		openssl-dev 		perl-dev 		perl-ipc-run 		perl-utils 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		icu-dev 		lz4-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-krb5 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 		--with-lz4 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 		zstd 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Tue, 24 May 2022 20:12:31 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample
# Tue, 24 May 2022 20:12:32 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 24 May 2022 20:12:32 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 24 May 2022 20:12:33 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 24 May 2022 20:12:33 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 24 May 2022 20:12:33 GMT
COPY file:e8928645623137de410cce68a2aa3b22f07a64e6391025598a60f3e461c606a3 in /usr/local/bin/ 
# Tue, 24 May 2022 20:12:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 24 May 2022 20:12:34 GMT
STOPSIGNAL SIGINT
# Tue, 24 May 2022 20:12:34 GMT
EXPOSE 5432
# Tue, 24 May 2022 20:12:34 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:a27b630f446c3da376a30cf610e4bfa6847f8b87c83702c29e72b986f4e52d28`  
		Last Modified: Mon, 04 Apr 2022 23:42:37 GMT  
		Size: 2.6 MB (2600375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:101f526f514773cdbd93dcd2746d73e8dff7395f41467133c139fc629c7b8db0`  
		Last Modified: Tue, 05 Apr 2022 07:11:42 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc452154c8b825654930b9dae70ac27b9d54bbae8d0ff8bacc09468465e28a3a`  
		Last Modified: Tue, 05 Apr 2022 07:11:42 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfb33095fda8969a7f83e21e5fb32ad447aba6d8f6923e83e2e1b82b8e9ba170`  
		Last Modified: Tue, 24 May 2022 20:15:48 GMT  
		Size: 83.2 MB (83239247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd6726c775e4d524f4f64dc1881d68d898092f3b210d2aca9991f1fa54653842`  
		Last Modified: Tue, 24 May 2022 20:15:38 GMT  
		Size: 9.5 KB (9455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:556d72f0a71a110aee5df8634631473e3eb7c70039e8a521887a52dd4b0d7d42`  
		Last Modified: Tue, 24 May 2022 20:15:38 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d749bda3147c9b23bb406590132f1160b93965e900a9d0683767b435fea0ada7`  
		Last Modified: Tue, 24 May 2022 20:15:38 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:353bc5725cbbff6c42270554f68223c906b1d5c94849ac6916db91eb4151ae32`  
		Last Modified: Tue, 24 May 2022 20:15:38 GMT  
		Size: 4.7 KB (4703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
