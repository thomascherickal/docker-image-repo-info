## `postgres:10-alpine`

```console
$ docker pull postgres@sha256:9adf6d239d18cdcc8684990158d229ad6373d952c1fd7e0c0a800513d2922aa7
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

### `postgres:10-alpine` - linux; amd64

```console
$ docker pull postgres@sha256:2d0caf2510dd9236be7d9948a5343f2151a5191c2c64353fc48f250e2bba6b52
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.3 MB (30273873 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1713aedcfacda1824acf68266494bc494026a6c04179dee743f0c04f07027624`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Wed, 23 Mar 2022 15:21:21 GMT
ADD file:7386ad893672007cca2d73cec1862d582a69d581ca1d155d4599cb2aa54d5498 in / 
# Wed, 23 Mar 2022 15:21:21 GMT
CMD ["/bin/sh"]
# Wed, 23 Mar 2022 18:10:32 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Wed, 23 Mar 2022 18:10:32 GMT
ENV LANG=en_US.utf8
# Wed, 23 Mar 2022 18:10:32 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 23 Mar 2022 18:31:46 GMT
ENV PG_MAJOR=10
# Wed, 23 Mar 2022 18:31:46 GMT
ENV PG_VERSION=10.20
# Wed, 23 Mar 2022 18:31:46 GMT
ENV PG_SHA256=87de16d59bcfe42fa605c312c59be5e294e8a3e6acb655dd7ad47cbb930a659f
# Wed, 23 Mar 2022 18:35:07 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openldap-dev 		openssl-dev 		perl-dev 		perl-ipc-run 		perl-utils 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		zstd 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-krb5 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Wed, 23 Mar 2022 18:35:08 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample
# Wed, 23 Mar 2022 18:35:08 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Wed, 23 Mar 2022 18:35:08 GMT
ENV PGDATA=/var/lib/postgresql/data
# Wed, 23 Mar 2022 18:35:09 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Wed, 23 Mar 2022 18:35:09 GMT
VOLUME [/var/lib/postgresql/data]
# Wed, 23 Mar 2022 18:35:09 GMT
COPY file:e8928645623137de410cce68a2aa3b22f07a64e6391025598a60f3e461c606a3 in /usr/local/bin/ 
# Wed, 23 Mar 2022 18:35:09 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 23 Mar 2022 18:35:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 23 Mar 2022 18:35:10 GMT
STOPSIGNAL SIGINT
# Wed, 23 Mar 2022 18:35:10 GMT
EXPOSE 5432
# Wed, 23 Mar 2022 18:35:10 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:3aa4d0bbde192bfaba75f2d124d8cf2e6de452ae03e55d54105e46b06eb8127e`  
		Last Modified: Wed, 23 Mar 2022 15:21:44 GMT  
		Size: 2.8 MB (2812689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1446b5429bf64371b029f8d6f73453d7b4ac3780e6008783efe3c4da30428f76`  
		Last Modified: Wed, 23 Mar 2022 18:36:12 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9275bd2facbb6425a234a01c080390c933490d7ddff475390e8c245edf97cb3`  
		Last Modified: Wed, 23 Mar 2022 18:36:12 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6430e1d0db526eaf07624412dd71cbd423364b5ef02f0fccc90d23e6d3bd9c86`  
		Last Modified: Wed, 23 Mar 2022 18:38:14 GMT  
		Size: 27.4 MB (27446849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:365d2c8f4c54f498b444b75bd317d7c69cf38a06c5e557e7727152ca0c29c7a5`  
		Last Modified: Wed, 23 Mar 2022 18:38:08 GMT  
		Size: 7.7 KB (7728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05865676dbe552cc65ad239556c9ad83fe2cfabcb8e6d6554e831f04faf425eb`  
		Last Modified: Wed, 23 Mar 2022 18:38:08 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:640c280581183954fe5e7f662990f829d3814b1e6627b66896f0da40cc71abd9`  
		Last Modified: Wed, 23 Mar 2022 18:38:08 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:591367e235639e1af6f11a065e2229eed61474469ce949cab3c54fd0fd7b3666`  
		Last Modified: Wed, 23 Mar 2022 18:38:08 GMT  
		Size: 4.7 KB (4700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f400ee13cc3b71e7aece15781cb9f619bbe507b6c9ac4e9eebed3f4e49e85f7a`  
		Last Modified: Wed, 23 Mar 2022 18:38:08 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:10-alpine` - linux; arm variant v6

```console
$ docker pull postgres@sha256:78efdc2528b5941a2b30347983cef86208eb22f420d0965b4cab84ebe11bd3d4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.8 MB (29799096 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:27d3a9be6a62255dd5c30413faffc00a4dbb8693bce341183026b1cc1df56c31`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Wed, 23 Mar 2022 15:49:35 GMT
ADD file:fd7f6da4a48df653ae6dd18e6d5959008daf5ce429845c974982dc7d213342d9 in / 
# Wed, 23 Mar 2022 15:49:35 GMT
CMD ["/bin/sh"]
# Wed, 23 Mar 2022 23:21:07 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Wed, 23 Mar 2022 23:21:08 GMT
ENV LANG=en_US.utf8
# Wed, 23 Mar 2022 23:21:09 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 23 Mar 2022 23:42:54 GMT
ENV PG_MAJOR=10
# Wed, 23 Mar 2022 23:42:55 GMT
ENV PG_VERSION=10.20
# Wed, 23 Mar 2022 23:42:55 GMT
ENV PG_SHA256=87de16d59bcfe42fa605c312c59be5e294e8a3e6acb655dd7ad47cbb930a659f
# Tue, 29 Mar 2022 00:20:25 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openldap-dev 		openssl-dev 		perl-dev 		perl-ipc-run 		perl-utils 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-krb5 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 		zstd 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Tue, 29 Mar 2022 00:20:27 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample
# Tue, 29 Mar 2022 00:20:29 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 29 Mar 2022 00:20:29 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 29 Mar 2022 00:20:30 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 29 Mar 2022 00:20:31 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 29 Mar 2022 00:20:31 GMT
COPY file:e8928645623137de410cce68a2aa3b22f07a64e6391025598a60f3e461c606a3 in /usr/local/bin/ 
# Tue, 29 Mar 2022 00:20:33 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Tue, 29 Mar 2022 00:20:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 29 Mar 2022 00:20:34 GMT
STOPSIGNAL SIGINT
# Tue, 29 Mar 2022 00:20:34 GMT
EXPOSE 5432
# Tue, 29 Mar 2022 00:20:34 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:4e012d7cd81aa4570d9d209a75131b32f34a3533d5d449d23fd875513922588e`  
		Last Modified: Wed, 23 Mar 2022 15:51:07 GMT  
		Size: 2.6 MB (2624816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ed6ba2d9bf5eeeb6b35d630730e4c107c4d006f8ab5c27a66f84dbfb16b6e49`  
		Last Modified: Wed, 23 Mar 2022 23:48:37 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38dc3323f729ea15aeb7941aa1add794da08f0b2f0de89ae710c7de68145da50`  
		Last Modified: Wed, 23 Mar 2022 23:48:37 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dc9ca2ad3401d6fc6eef80fdb0f9a3a4cbba01b6c55b4d43163966e10b8846e`  
		Last Modified: Tue, 29 Mar 2022 00:27:05 GMT  
		Size: 27.2 MB (27159938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:328a9bdc4ac6508ec8905c489a2e306fb27a3d4ef5221ce3eedae674293bf11c`  
		Last Modified: Tue, 29 Mar 2022 00:26:47 GMT  
		Size: 7.7 KB (7736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f69e6d513a9f1c89f9156b483f469c2c74e437f796441642ce5b08d58a5f4cea`  
		Last Modified: Tue, 29 Mar 2022 00:26:47 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce2cf5a6a957f3a58471b738d24f866bf922a3b0be96a2b8e66177b38f0bfd00`  
		Last Modified: Tue, 29 Mar 2022 00:26:47 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52e340b816d025d7c1abe4f086918b192634c3b5517d855b53d62a64f228c277`  
		Last Modified: Tue, 29 Mar 2022 00:26:47 GMT  
		Size: 4.7 KB (4700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94505b5882a469156f0e64c830b8a0a8616cfb72e1ad929d9b6fe6a1b2405951`  
		Last Modified: Tue, 29 Mar 2022 00:26:47 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:10-alpine` - linux; arm variant v7

```console
$ docker pull postgres@sha256:e8df5e2bd2cd2e41b29a8e968b32c1192100e058efb92975a083e110a6605018
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.6 MB (28584399 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a3422de9b6df70d47d83f01a6fd096c7c97561c4df6d42e77314ac6000757f83`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Wed, 23 Mar 2022 15:57:29 GMT
ADD file:462f633d612f6502dcfa539fcfd8b1fc90da097b08ad6b984e485bc73e57bd41 in / 
# Wed, 23 Mar 2022 15:57:29 GMT
CMD ["/bin/sh"]
# Wed, 23 Mar 2022 23:28:38 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Wed, 23 Mar 2022 23:28:38 GMT
ENV LANG=en_US.utf8
# Wed, 23 Mar 2022 23:28:41 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 23 Mar 2022 23:50:15 GMT
ENV PG_MAJOR=10
# Wed, 23 Mar 2022 23:50:15 GMT
ENV PG_VERSION=10.20
# Wed, 23 Mar 2022 23:50:16 GMT
ENV PG_SHA256=87de16d59bcfe42fa605c312c59be5e294e8a3e6acb655dd7ad47cbb930a659f
# Tue, 29 Mar 2022 00:34:39 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openldap-dev 		openssl-dev 		perl-dev 		perl-ipc-run 		perl-utils 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-krb5 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 		zstd 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Tue, 29 Mar 2022 00:34:41 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample
# Tue, 29 Mar 2022 00:34:43 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 29 Mar 2022 00:34:43 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 29 Mar 2022 00:34:44 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 29 Mar 2022 00:34:45 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 29 Mar 2022 00:34:45 GMT
COPY file:e8928645623137de410cce68a2aa3b22f07a64e6391025598a60f3e461c606a3 in /usr/local/bin/ 
# Tue, 29 Mar 2022 00:34:47 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Tue, 29 Mar 2022 00:34:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 29 Mar 2022 00:34:47 GMT
STOPSIGNAL SIGINT
# Tue, 29 Mar 2022 00:34:48 GMT
EXPOSE 5432
# Tue, 29 Mar 2022 00:34:48 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:dfd6a1b07255bd60715939c7488b4714efdc3519f793d4d8b238b910091c1642`  
		Last Modified: Wed, 23 Mar 2022 15:58:58 GMT  
		Size: 2.4 MB (2427061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29c377d40d4b66501645a2ecdaea31e6ff505102f0fd40ab6a3c9727d9788de5`  
		Last Modified: Wed, 23 Mar 2022 23:57:33 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33165c008c29f279d33956ce2c18b152ce42e635b10180da72f5444a9033c890`  
		Last Modified: Wed, 23 Mar 2022 23:57:33 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04342d0c48954cebef0f544e4747cf65dd5d5b80fa10f7d986fca274541965b2`  
		Last Modified: Tue, 29 Mar 2022 00:43:13 GMT  
		Size: 26.1 MB (26142995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07fbaea2fd49b79513a8e39581276cf3979bf4baa561e4dfc0c3ac8b7c3756ca`  
		Last Modified: Tue, 29 Mar 2022 00:42:56 GMT  
		Size: 7.7 KB (7733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd843e5d90a48273d25cad70e79eb3011bd5181682c4b73413f863e5e169334e`  
		Last Modified: Tue, 29 Mar 2022 00:42:56 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ecc44dd292c09131e1243eae067a08038dad499aa8dc95694b5c9fe17b6b2df`  
		Last Modified: Tue, 29 Mar 2022 00:42:56 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56b983063117138bdb997abbd2a102b865e0eea4d69912d44c6dc7984d61079e`  
		Last Modified: Tue, 29 Mar 2022 00:42:56 GMT  
		Size: 4.7 KB (4701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1ced456dc042bd801de09d3ad71f5004de151e0aa509d019c8898f1bf0cb7f6`  
		Last Modified: Tue, 29 Mar 2022 00:42:56 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:10-alpine` - linux; arm64 variant v8

```console
$ docker pull postgres@sha256:dc57081314f92629a7f106a485256f61cfdce09e04e6496c6cf94750525c807f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.6 MB (30615891 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c10a4f7f76ddfd0df04808b22feb7b5428550793b60889952313b205d9caf35`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 24 Mar 2022 00:36:14 GMT
ADD file:30da1868f9f0555fb3e5223cd75cbf3c31760c1b6087f42d78abb08a8c5066ff in / 
# Thu, 24 Mar 2022 00:36:14 GMT
CMD ["/bin/sh"]
# Thu, 24 Mar 2022 07:07:43 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 24 Mar 2022 07:07:43 GMT
ENV LANG=en_US.utf8
# Thu, 24 Mar 2022 07:07:44 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 24 Mar 2022 07:22:00 GMT
ENV PG_MAJOR=10
# Thu, 24 Mar 2022 07:22:01 GMT
ENV PG_VERSION=10.20
# Thu, 24 Mar 2022 07:22:02 GMT
ENV PG_SHA256=87de16d59bcfe42fa605c312c59be5e294e8a3e6acb655dd7ad47cbb930a659f
# Tue, 29 Mar 2022 00:07:06 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openldap-dev 		openssl-dev 		perl-dev 		perl-ipc-run 		perl-utils 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-krb5 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 		zstd 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Tue, 29 Mar 2022 00:07:06 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample
# Tue, 29 Mar 2022 00:07:07 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 29 Mar 2022 00:07:08 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 29 Mar 2022 00:07:09 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 29 Mar 2022 00:07:10 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 29 Mar 2022 00:07:12 GMT
COPY file:e8928645623137de410cce68a2aa3b22f07a64e6391025598a60f3e461c606a3 in /usr/local/bin/ 
# Tue, 29 Mar 2022 00:07:12 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Tue, 29 Mar 2022 00:07:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 29 Mar 2022 00:07:14 GMT
STOPSIGNAL SIGINT
# Tue, 29 Mar 2022 00:07:15 GMT
EXPOSE 5432
# Tue, 29 Mar 2022 00:07:16 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:a5e44472bb1f0d721d23f82fa10a4c3d25994790238a173c1de950a649eb9a90`  
		Last Modified: Wed, 23 Mar 2022 20:10:33 GMT  
		Size: 2.7 MB (2714720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0496603e40846deae549baf83a9f56925a4a900fc46a434de84d2ac2c8514b35`  
		Last Modified: Thu, 24 Mar 2022 07:25:55 GMT  
		Size: 1.3 KB (1256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b9629142073a462cc28faaea8aff541e6bceb755d8646fabd3424e4ed0daa9d`  
		Last Modified: Thu, 24 Mar 2022 07:25:55 GMT  
		Size: 113.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98794691a97946d2a0e3862c3e9b3cc49c472b7da7c296c1566ddf54ffeedf6a`  
		Last Modified: Tue, 29 Mar 2022 00:11:23 GMT  
		Size: 27.9 MB (27886949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19fd3747b5676fdf0102638c1710d0a85d8dad4589e7f35126726245eb97164c`  
		Last Modified: Tue, 29 Mar 2022 00:11:17 GMT  
		Size: 7.7 KB (7728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b605275e525704a17a6c522e36914733c0dbb47e47fa57c350c972a806dbf719`  
		Last Modified: Tue, 29 Mar 2022 00:11:17 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5edd6a55918141567d745b19116f42d82c6f9238fa323c6572d571a7f4c33349`  
		Last Modified: Tue, 29 Mar 2022 00:11:17 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2129b40eb75063a37f12edeaa1c4f11ebbfbdab13202bfcaf424ad1be95c185b`  
		Last Modified: Tue, 29 Mar 2022 00:11:17 GMT  
		Size: 4.7 KB (4701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:007629ca7c2480be158342db84357bdeae771ff6d54ca33cdf82193f2a2ae7bc`  
		Last Modified: Tue, 29 Mar 2022 00:11:17 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:10-alpine` - linux; 386

```console
$ docker pull postgres@sha256:7c000584cf10da4255dded309b81b891930a70daed1f5ca31632fffdf5d7c057
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.9 MB (31924458 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f2c84fc67285faa99affa3dfd6d6fee5281da1065b7adda0247dbbc82570dadf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Wed, 23 Mar 2022 14:59:30 GMT
ADD file:b217fd5b9fc648f19dca9967ed10f2ac3b424f0d4d2f61e4582c965864f52d07 in / 
# Wed, 23 Mar 2022 14:59:31 GMT
CMD ["/bin/sh"]
# Wed, 23 Mar 2022 23:42:14 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Wed, 23 Mar 2022 23:42:15 GMT
ENV LANG=en_US.utf8
# Wed, 23 Mar 2022 23:42:16 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 24 Mar 2022 00:34:32 GMT
ENV PG_MAJOR=10
# Thu, 24 Mar 2022 00:34:33 GMT
ENV PG_VERSION=10.20
# Thu, 24 Mar 2022 00:34:34 GMT
ENV PG_SHA256=87de16d59bcfe42fa605c312c59be5e294e8a3e6acb655dd7ad47cbb930a659f
# Mon, 28 Mar 2022 23:55:39 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openldap-dev 		openssl-dev 		perl-dev 		perl-ipc-run 		perl-utils 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-krb5 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 		zstd 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Mon, 28 Mar 2022 23:55:39 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample
# Mon, 28 Mar 2022 23:55:40 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Mon, 28 Mar 2022 23:55:41 GMT
ENV PGDATA=/var/lib/postgresql/data
# Mon, 28 Mar 2022 23:55:42 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Mon, 28 Mar 2022 23:55:43 GMT
VOLUME [/var/lib/postgresql/data]
# Mon, 28 Mar 2022 23:55:45 GMT
COPY file:e8928645623137de410cce68a2aa3b22f07a64e6391025598a60f3e461c606a3 in /usr/local/bin/ 
# Mon, 28 Mar 2022 23:55:45 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Mon, 28 Mar 2022 23:55:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 28 Mar 2022 23:55:47 GMT
STOPSIGNAL SIGINT
# Mon, 28 Mar 2022 23:55:48 GMT
EXPOSE 5432
# Mon, 28 Mar 2022 23:55:49 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:b78004f8e08f3a114b1629885a10f66985c09b7d887608bb5fb1883c97b940ca`  
		Last Modified: Wed, 23 Mar 2022 15:00:33 GMT  
		Size: 2.8 MB (2821831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efecee9af9234dd45c1409faa1203d058b0c7f9e03b166aab0bd131570e4652c`  
		Last Modified: Thu, 24 Mar 2022 00:39:25 GMT  
		Size: 1.3 KB (1256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5dbf82ffafc4919ee4297954c00e6cc272e568e2c2e16cf7b525a7df603fcf3`  
		Last Modified: Thu, 24 Mar 2022 00:39:25 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dab9fc2f58e79f80d6e71beb889bff9ebb261c47f3eec8f43066e75d1f693f40`  
		Last Modified: Mon, 28 Mar 2022 23:59:54 GMT  
		Size: 29.1 MB (29088399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:beac8521b81d5c287b615fe7d31496ad77b732ab74da8d9bd50213492b67db9b`  
		Last Modified: Mon, 28 Mar 2022 23:59:47 GMT  
		Size: 7.7 KB (7733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f99661d77ed84a2f86a3737206c0f965cede55aee61f6f70149a2f10868c5e9`  
		Last Modified: Mon, 28 Mar 2022 23:59:47 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78fcae0d77afd323a548b5d5e293484161efa43cbaf8e3b05102d0608c7a89df`  
		Last Modified: Mon, 28 Mar 2022 23:59:47 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4df1670835e27ae7a10f069ad111ac9d05d3e6eaedf68603c531b51b48f58ed8`  
		Last Modified: Mon, 28 Mar 2022 23:59:47 GMT  
		Size: 4.7 KB (4701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d813d4c436a8122330d710c094d6fecef27682a2a528241e16c01638b2c343c6`  
		Last Modified: Mon, 28 Mar 2022 23:59:47 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:10-alpine` - linux; ppc64le

```console
$ docker pull postgres@sha256:d7c833252931c0ca3bf3724416e58749a75b12ad054f878d5bcf2db91a47371b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.7 MB (31656323 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f1533495c6b4985ee9924972f708682654f1101995f424b744aa7eb4df4684d9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Wed, 23 Mar 2022 15:24:30 GMT
ADD file:3392b3547a6a1366b9a6ada72065830d8886708bbfc70472c607e742dfd07994 in / 
# Wed, 23 Mar 2022 15:24:32 GMT
CMD ["/bin/sh"]
# Wed, 23 Mar 2022 23:03:58 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Wed, 23 Mar 2022 23:04:03 GMT
ENV LANG=en_US.utf8
# Wed, 23 Mar 2022 23:04:17 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 23 Mar 2022 23:28:44 GMT
ENV PG_MAJOR=10
# Wed, 23 Mar 2022 23:28:46 GMT
ENV PG_VERSION=10.20
# Wed, 23 Mar 2022 23:28:48 GMT
ENV PG_SHA256=87de16d59bcfe42fa605c312c59be5e294e8a3e6acb655dd7ad47cbb930a659f
# Wed, 23 Mar 2022 23:32:01 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openldap-dev 		openssl-dev 		perl-dev 		perl-ipc-run 		perl-utils 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		zstd 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-krb5 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Wed, 23 Mar 2022 23:32:12 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample
# Wed, 23 Mar 2022 23:32:20 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Wed, 23 Mar 2022 23:32:22 GMT
ENV PGDATA=/var/lib/postgresql/data
# Wed, 23 Mar 2022 23:32:27 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Wed, 23 Mar 2022 23:32:32 GMT
VOLUME [/var/lib/postgresql/data]
# Wed, 23 Mar 2022 23:32:35 GMT
COPY file:e8928645623137de410cce68a2aa3b22f07a64e6391025598a60f3e461c606a3 in /usr/local/bin/ 
# Wed, 23 Mar 2022 23:32:42 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 23 Mar 2022 23:32:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 23 Mar 2022 23:32:47 GMT
STOPSIGNAL SIGINT
# Wed, 23 Mar 2022 23:32:50 GMT
EXPOSE 5432
# Wed, 23 Mar 2022 23:32:55 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:58323f60457d1c04dce77185ce8c0377ac10135b55fdf4506e87d24e67780d7d`  
		Last Modified: Wed, 23 Mar 2022 15:25:23 GMT  
		Size: 2.8 MB (2814037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb9db94b880cf3a25ec4fa883c30a0984e0abdc6e2f3b9744f16714938eb3227`  
		Last Modified: Wed, 23 Mar 2022 23:34:40 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa868c9c77edbc6fac093b31efa86b5aad8f2fb0cbe4f519f0b5d65923854cdc`  
		Last Modified: Wed, 23 Mar 2022 23:34:40 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28e82d037ff6e7fa3facd49580451d20cef41d385d97021a69c47db689adcb47`  
		Last Modified: Wed, 23 Mar 2022 23:37:21 GMT  
		Size: 28.8 MB (28827956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6857ac8914d2eaf74235fbc17a093a2a8cf2caca5127e8505fe6102ca7771000`  
		Last Modified: Wed, 23 Mar 2022 23:37:12 GMT  
		Size: 7.7 KB (7728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:009e1329ba519a3e84956d01ac25352c35c985ec3d0f76c3ac4ceb9367f95b5a`  
		Last Modified: Wed, 23 Mar 2022 23:37:12 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c109670525900cfe05df58e389d4c5e6cfbc3968846cbf69daa1120123a2823`  
		Last Modified: Wed, 23 Mar 2022 23:37:12 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3bf966efd00da89e48c4b6461ac996bbcbcb4f24b2b0ab93e9ae34e7566be83`  
		Last Modified: Wed, 23 Mar 2022 23:37:12 GMT  
		Size: 4.7 KB (4697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aec4572e6379f15bfeac9a09e3ddbd1180998ee10a3d5872840e59a6f783b3d2`  
		Last Modified: Wed, 23 Mar 2022 23:37:12 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:10-alpine` - linux; s390x

```console
$ docker pull postgres@sha256:cc85d66c34bc8ad4d006a9a816ec247738e28f080267e465175ae4b4793ffa26
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.8 MB (30766236 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:835e31b318229773562c3fd09209775bacc9f038e46e0bc289a990c336897c4f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Wed, 23 Mar 2022 15:41:27 GMT
ADD file:c6fe4c8affcc912e0de86d8691aecb959ac828259f09843a569ec4e5714d6c6f in / 
# Wed, 23 Mar 2022 15:41:27 GMT
CMD ["/bin/sh"]
# Wed, 23 Mar 2022 19:40:12 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Wed, 23 Mar 2022 19:40:12 GMT
ENV LANG=en_US.utf8
# Wed, 23 Mar 2022 19:40:12 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 23 Mar 2022 19:52:20 GMT
ENV PG_MAJOR=10
# Wed, 23 Mar 2022 19:52:20 GMT
ENV PG_VERSION=10.20
# Wed, 23 Mar 2022 19:52:20 GMT
ENV PG_SHA256=87de16d59bcfe42fa605c312c59be5e294e8a3e6acb655dd7ad47cbb930a659f
# Mon, 28 Mar 2022 23:57:01 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openldap-dev 		openssl-dev 		perl-dev 		perl-ipc-run 		perl-utils 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-krb5 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 		zstd 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Mon, 28 Mar 2022 23:57:02 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample
# Mon, 28 Mar 2022 23:57:03 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Mon, 28 Mar 2022 23:57:03 GMT
ENV PGDATA=/var/lib/postgresql/data
# Mon, 28 Mar 2022 23:57:03 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Mon, 28 Mar 2022 23:57:03 GMT
VOLUME [/var/lib/postgresql/data]
# Mon, 28 Mar 2022 23:57:03 GMT
COPY file:e8928645623137de410cce68a2aa3b22f07a64e6391025598a60f3e461c606a3 in /usr/local/bin/ 
# Mon, 28 Mar 2022 23:57:04 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Mon, 28 Mar 2022 23:57:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 28 Mar 2022 23:57:04 GMT
STOPSIGNAL SIGINT
# Mon, 28 Mar 2022 23:57:04 GMT
EXPOSE 5432
# Mon, 28 Mar 2022 23:57:04 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:cf2f18c21a46b2d59a7a34a051c9c289710e89cdef47cc582fdb9d65a1e68e44`  
		Last Modified: Wed, 23 Mar 2022 15:42:18 GMT  
		Size: 2.6 MB (2601698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dc5c78150f738a40107a8e5ac8f6a74b8f71fe899133c9d5d1751b4ec198e2f`  
		Last Modified: Wed, 23 Mar 2022 19:55:47 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:110c012f282f5f0ea397ea685e89820379da8545d4dafac0008c8171127f49a4`  
		Last Modified: Wed, 23 Mar 2022 19:55:47 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63d1b1cf5896a1773b54f5b101024a103381f60d741bf4587e8b0b40cbc07865`  
		Last Modified: Tue, 29 Mar 2022 00:11:49 GMT  
		Size: 28.2 MB (28150205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65b02b242274dad0d2427462985cf119b9869a8427cabdd647a10ce4e32d1f45`  
		Last Modified: Tue, 29 Mar 2022 00:11:19 GMT  
		Size: 7.7 KB (7731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a219bd9f84a0f543a790444fcb4b27bb2cb384fe170ddb24f59ff4206fe9079b`  
		Last Modified: Tue, 29 Mar 2022 00:11:23 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c752b417c6639a4e67d1388652a0782cf2308e1922ad5e2cc330d12d7a86ab8`  
		Last Modified: Tue, 29 Mar 2022 00:11:19 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02d40569b1efb95dad6c88b3882f0df9069a9b74ae3556f15b78b551a16d9105`  
		Last Modified: Tue, 29 Mar 2022 00:11:19 GMT  
		Size: 4.7 KB (4696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35e8bde55eb9541399f966867edc985a841638e7acc8715ae769b342dfebacc4`  
		Last Modified: Tue, 29 Mar 2022 00:11:19 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
