## `postgres:11-alpine3.15`

```console
$ docker pull postgres@sha256:5e79f844764a374a0c6797ed46449966cde0e227ca707fa0bf5bfd279e388bbf
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

### `postgres:11-alpine3.15` - linux; amd64

```console
$ docker pull postgres@sha256:96fae2fddad1a3d0c17741bf01cad0a47819f243985e94570f672dd050555339
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **78.5 MB (78537978 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a11773c76b9b3dd774577928cbcbfd95cc6ef610817968df4032c70cb821244c`
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
# Wed, 23 Mar 2022 18:26:49 GMT
ENV PG_MAJOR=11
# Wed, 23 Mar 2022 18:26:49 GMT
ENV PG_VERSION=11.15
# Wed, 23 Mar 2022 18:26:49 GMT
ENV PG_SHA256=c8f58e8ebd4f4567f4f9ba1032eb3e99e0251d87cbe3e564b485590e37a879e3
# Wed, 23 Mar 2022 18:31:29 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm-dev clang g++ 		make 		openldap-dev 		openssl-dev 		perl-dev 		perl-ipc-run 		perl-utils 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		zstd 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-krb5 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Wed, 23 Mar 2022 18:31:30 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample
# Wed, 23 Mar 2022 18:31:30 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Wed, 23 Mar 2022 18:31:30 GMT
ENV PGDATA=/var/lib/postgresql/data
# Wed, 23 Mar 2022 18:31:31 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Wed, 23 Mar 2022 18:31:31 GMT
VOLUME [/var/lib/postgresql/data]
# Wed, 23 Mar 2022 18:31:31 GMT
COPY file:e8928645623137de410cce68a2aa3b22f07a64e6391025598a60f3e461c606a3 in /usr/local/bin/ 
# Wed, 23 Mar 2022 18:31:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 23 Mar 2022 18:31:31 GMT
STOPSIGNAL SIGINT
# Wed, 23 Mar 2022 18:31:31 GMT
EXPOSE 5432
# Wed, 23 Mar 2022 18:31:32 GMT
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
	-	`sha256:c07b69f0798d7f9c634e22436947893198390e99a13ed6636eea839383c07bd6`  
		Last Modified: Wed, 23 Mar 2022 18:37:51 GMT  
		Size: 75.7 MB (75710810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a10f4c865cff12c286453f6bcb581f8f887c86a2de4a687c47eeed7076f2202`  
		Last Modified: Wed, 23 Mar 2022 18:37:41 GMT  
		Size: 8.0 KB (7991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85ffb522b3b9deb40750dd935af28b91f8a5add67619a01792cde65f743bc05a`  
		Last Modified: Wed, 23 Mar 2022 18:37:41 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fa93a1e09be60f7fcb5787f6c027fe4edf2cb306412235ac8ebbe18caca2668`  
		Last Modified: Wed, 23 Mar 2022 18:37:41 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fa9ff5345bb059b29102f663e90de34be8828cc571e07f4c8c9b7894959b9cb`  
		Last Modified: Wed, 23 Mar 2022 18:37:41 GMT  
		Size: 4.7 KB (4702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:11-alpine3.15` - linux; arm variant v6

```console
$ docker pull postgres@sha256:0bf73b27aaccc88aaa05c24f7cc48b10ad7c5cd05e28348e5b954557022d7bce
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.5 MB (76539318 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:853fcab88f435852b5bd9e2b0d2530304b494d374716f979b1c73448757fbc4f`
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
# Wed, 23 Mar 2022 23:37:31 GMT
ENV PG_MAJOR=11
# Wed, 23 Mar 2022 23:37:32 GMT
ENV PG_VERSION=11.15
# Wed, 23 Mar 2022 23:37:32 GMT
ENV PG_SHA256=c8f58e8ebd4f4567f4f9ba1032eb3e99e0251d87cbe3e564b485590e37a879e3
# Wed, 23 Mar 2022 23:42:25 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm-dev clang g++ 		make 		openldap-dev 		openssl-dev 		perl-dev 		perl-ipc-run 		perl-utils 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		zstd 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-krb5 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Wed, 23 Mar 2022 23:42:27 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample
# Wed, 23 Mar 2022 23:42:28 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Wed, 23 Mar 2022 23:42:29 GMT
ENV PGDATA=/var/lib/postgresql/data
# Wed, 23 Mar 2022 23:42:30 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Wed, 23 Mar 2022 23:42:31 GMT
VOLUME [/var/lib/postgresql/data]
# Wed, 23 Mar 2022 23:42:31 GMT
COPY file:e8928645623137de410cce68a2aa3b22f07a64e6391025598a60f3e461c606a3 in /usr/local/bin/ 
# Wed, 23 Mar 2022 23:42:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 23 Mar 2022 23:42:32 GMT
STOPSIGNAL SIGINT
# Wed, 23 Mar 2022 23:42:32 GMT
EXPOSE 5432
# Wed, 23 Mar 2022 23:42:33 GMT
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
	-	`sha256:09cd2d7be948e50af61d0bde7c62d0daa7556728233daab3fdb1bdbba2d6ab51`  
		Last Modified: Thu, 24 Mar 2022 01:33:25 GMT  
		Size: 73.9 MB (73900022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a94b2b80e17c24271efc01af9dee17043a024efc4fa96069334b71853903c9c`  
		Last Modified: Thu, 24 Mar 2022 01:32:41 GMT  
		Size: 8.0 KB (7992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5455a7c4f1e2b541b4dd0812989a0b6ef720e79c4644df7dbd2d83a67568c558`  
		Last Modified: Thu, 24 Mar 2022 01:32:42 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a85ff1e3ad7be0086b17bf8ca2d2ebdc4b25ea0e406995b83dc5da21f7afcb3`  
		Last Modified: Thu, 24 Mar 2022 01:32:41 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:573b90c4226dea3094bbcb37f74f59dcf84b39bc76d17bc5706a34ffb6dca6e5`  
		Last Modified: Thu, 24 Mar 2022 01:32:41 GMT  
		Size: 4.7 KB (4702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:11-alpine3.15` - linux; arm variant v7

```console
$ docker pull postgres@sha256:a8c10b550dd8c8affdfc633a42c34b63e51a363d6d22d482545f8bdcc915a4f8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.0 MB (72006623 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:46a2a2f17fb01a34041fc41f75186c24f032249e1d7869d8183dff14a5ae23ee`
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
# Wed, 23 Mar 2022 23:45:01 GMT
ENV PG_MAJOR=11
# Wed, 23 Mar 2022 23:45:01 GMT
ENV PG_VERSION=11.15
# Wed, 23 Mar 2022 23:45:02 GMT
ENV PG_SHA256=c8f58e8ebd4f4567f4f9ba1032eb3e99e0251d87cbe3e564b485590e37a879e3
# Wed, 23 Mar 2022 23:49:30 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm-dev clang g++ 		make 		openldap-dev 		openssl-dev 		perl-dev 		perl-ipc-run 		perl-utils 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		zstd 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-krb5 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Wed, 23 Mar 2022 23:49:32 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample
# Wed, 23 Mar 2022 23:49:33 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Wed, 23 Mar 2022 23:49:34 GMT
ENV PGDATA=/var/lib/postgresql/data
# Wed, 23 Mar 2022 23:49:35 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Wed, 23 Mar 2022 23:49:36 GMT
VOLUME [/var/lib/postgresql/data]
# Wed, 23 Mar 2022 23:49:36 GMT
COPY file:e8928645623137de410cce68a2aa3b22f07a64e6391025598a60f3e461c606a3 in /usr/local/bin/ 
# Wed, 23 Mar 2022 23:49:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 23 Mar 2022 23:49:37 GMT
STOPSIGNAL SIGINT
# Wed, 23 Mar 2022 23:49:37 GMT
EXPOSE 5432
# Wed, 23 Mar 2022 23:49:38 GMT
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
	-	`sha256:b4bb949bd5932a930e78b091eef4ff0038839e9fd4df5998d4fe712385d2636f`  
		Last Modified: Thu, 24 Mar 2022 00:01:32 GMT  
		Size: 69.6 MB (69565089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19b5b395693316fdaa31769b5e59fdcfd729598980601a7ba75678cf975fa556`  
		Last Modified: Thu, 24 Mar 2022 00:00:56 GMT  
		Size: 8.0 KB (7988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:565a17f98ccc12d8e8d661c671daedfa9fea05e89e3e7d196236d2b123270afa`  
		Last Modified: Thu, 24 Mar 2022 00:00:55 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a088634f53cfaedcb874e70a868e34bfda3ec241689ef275b957bb669729c50`  
		Last Modified: Thu, 24 Mar 2022 00:00:55 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:126f6d808f01f817a88dad8e17a49b558839cabcf4c7fcf06d1e7598f72898e6`  
		Last Modified: Thu, 24 Mar 2022 00:00:55 GMT  
		Size: 4.7 KB (4696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:11-alpine3.15` - linux; arm64 variant v8

```console
$ docker pull postgres@sha256:6be45562e4fed9c0af430eb1e66ebc4ea2d78343d01cf482d4964fcfe6997bf5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.4 MB (77405412 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1a8efca559a73a28ad5acba73d72fe15474c68fa24f9e15a4cca6a9881143208`
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
# Thu, 24 Mar 2022 07:18:38 GMT
ENV PG_MAJOR=11
# Thu, 24 Mar 2022 07:18:39 GMT
ENV PG_VERSION=11.15
# Thu, 24 Mar 2022 07:18:40 GMT
ENV PG_SHA256=c8f58e8ebd4f4567f4f9ba1032eb3e99e0251d87cbe3e564b485590e37a879e3
# Thu, 24 Mar 2022 07:21:36 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm-dev clang g++ 		make 		openldap-dev 		openssl-dev 		perl-dev 		perl-ipc-run 		perl-utils 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		zstd 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-krb5 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Thu, 24 Mar 2022 07:21:37 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample
# Thu, 24 Mar 2022 07:21:37 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 24 Mar 2022 07:21:38 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 24 Mar 2022 07:21:39 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 24 Mar 2022 07:21:40 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 24 Mar 2022 07:21:42 GMT
COPY file:e8928645623137de410cce68a2aa3b22f07a64e6391025598a60f3e461c606a3 in /usr/local/bin/ 
# Thu, 24 Mar 2022 07:21:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 24 Mar 2022 07:21:43 GMT
STOPSIGNAL SIGINT
# Thu, 24 Mar 2022 07:21:44 GMT
EXPOSE 5432
# Thu, 24 Mar 2022 07:21:45 GMT
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
	-	`sha256:169c57f86301b1dd5da7c9d0b11ce22f6e28ca2d20c51a4d8910da0c341fc459`  
		Last Modified: Thu, 24 Mar 2022 07:27:42 GMT  
		Size: 74.7 MB (74676336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbc7552a0e44e8e33824b9b6807ca4b06f1629a0ead7e8702fd8d99b828f5e86`  
		Last Modified: Thu, 24 Mar 2022 07:27:31 GMT  
		Size: 8.0 KB (7988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99d1f0d03461184ff19d6a1b694788faf17740f0da716bcdfe1386bac63a23ec`  
		Last Modified: Thu, 24 Mar 2022 07:27:31 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:082057d93b6f059567d1198570bff2394aacc3b6b022f8f2ef0c0c4a451da9d7`  
		Last Modified: Thu, 24 Mar 2022 07:27:32 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d94131173a3625ffe8252a58b88101de4da719395d1158993293d1edec95d81c`  
		Last Modified: Thu, 24 Mar 2022 07:27:31 GMT  
		Size: 4.7 KB (4701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:11-alpine3.15` - linux; 386

```console
$ docker pull postgres@sha256:287910d3e2a0699117e836046645f12c75a37714a611474918033cc0f26d6971
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **83.3 MB (83275286 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b83af3c75d53c1988a2a8780c80837b0d9b37ce9e2ca76c558048fa44c86aac9`
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
# Thu, 24 Mar 2022 00:21:29 GMT
ENV PG_MAJOR=11
# Thu, 24 Mar 2022 00:21:30 GMT
ENV PG_VERSION=11.15
# Thu, 24 Mar 2022 00:21:31 GMT
ENV PG_SHA256=c8f58e8ebd4f4567f4f9ba1032eb3e99e0251d87cbe3e564b485590e37a879e3
# Thu, 24 Mar 2022 00:24:35 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm-dev clang g++ 		make 		openldap-dev 		openssl-dev 		perl-dev 		perl-ipc-run 		perl-utils 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		zstd 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-krb5 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Thu, 24 Mar 2022 00:24:36 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample
# Thu, 24 Mar 2022 00:24:37 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 24 Mar 2022 00:24:38 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 24 Mar 2022 00:24:39 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 24 Mar 2022 00:24:40 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 24 Mar 2022 00:24:42 GMT
COPY file:e8928645623137de410cce68a2aa3b22f07a64e6391025598a60f3e461c606a3 in /usr/local/bin/ 
# Thu, 24 Mar 2022 00:24:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 24 Mar 2022 00:24:43 GMT
STOPSIGNAL SIGINT
# Thu, 24 Mar 2022 00:24:44 GMT
EXPOSE 5432
# Thu, 24 Mar 2022 00:24:45 GMT
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
	-	`sha256:7867c085eda5880fe7c947233aca58837ac0d223a61c1d3efb67889ab2fd533c`  
		Last Modified: Thu, 24 Mar 2022 00:42:38 GMT  
		Size: 80.4 MB (80439102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9a615a9809419c3f1351a778dd4aa6122641adce63306ed7eec42003edd37dd`  
		Last Modified: Thu, 24 Mar 2022 00:42:29 GMT  
		Size: 8.0 KB (7985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29c97b69e9889638aa311b39780572c5588bbb2f8ee589e98df176796a2a9c28`  
		Last Modified: Thu, 24 Mar 2022 00:42:29 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:726517bdcbe93d2091f4ef155d09750ed06a54c15eafabf574cf009d8af42bb4`  
		Last Modified: Thu, 24 Mar 2022 00:42:29 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40d44a87ede10a41715afcc95793cd524921047532c7a0d8ebc92855e70a3de0`  
		Last Modified: Thu, 24 Mar 2022 00:42:29 GMT  
		Size: 4.7 KB (4699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:11-alpine3.15` - linux; ppc64le

```console
$ docker pull postgres@sha256:cc3e1b48e8a3d637c45a1d97ffc11bf06270c0dcc777b4e953c00f816eb47b6c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **83.7 MB (83740403 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:95b8a64f2c0da2feb5fa4f9e94c2c1420589a614cf57604ef41607bfede83a01`
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
# Wed, 23 Mar 2022 23:22:59 GMT
ENV PG_MAJOR=11
# Wed, 23 Mar 2022 23:23:03 GMT
ENV PG_VERSION=11.15
# Wed, 23 Mar 2022 23:23:05 GMT
ENV PG_SHA256=c8f58e8ebd4f4567f4f9ba1032eb3e99e0251d87cbe3e564b485590e37a879e3
# Wed, 23 Mar 2022 23:27:31 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm-dev clang g++ 		make 		openldap-dev 		openssl-dev 		perl-dev 		perl-ipc-run 		perl-utils 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		zstd 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-krb5 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Wed, 23 Mar 2022 23:27:45 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample
# Wed, 23 Mar 2022 23:27:56 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Wed, 23 Mar 2022 23:28:01 GMT
ENV PGDATA=/var/lib/postgresql/data
# Wed, 23 Mar 2022 23:28:13 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Wed, 23 Mar 2022 23:28:16 GMT
VOLUME [/var/lib/postgresql/data]
# Wed, 23 Mar 2022 23:28:19 GMT
COPY file:e8928645623137de410cce68a2aa3b22f07a64e6391025598a60f3e461c606a3 in /usr/local/bin/ 
# Wed, 23 Mar 2022 23:28:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 23 Mar 2022 23:28:24 GMT
STOPSIGNAL SIGINT
# Wed, 23 Mar 2022 23:28:28 GMT
EXPOSE 5432
# Wed, 23 Mar 2022 23:28:30 GMT
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
	-	`sha256:78b67a161dffab4c55f96e4193403125bef7658fe0dec9d21c551d4fa6a84604`  
		Last Modified: Wed, 23 Mar 2022 23:36:49 GMT  
		Size: 80.9 MB (80911886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aae599bb388f55dd0aad554afae3f08c197ecc76fc23feabbf128eed63a0f610`  
		Last Modified: Wed, 23 Mar 2022 23:36:36 GMT  
		Size: 8.0 KB (7994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa31bb235f25000269fc286c8cf641f0e54189680e5814c8f2dbdcbf9f74dbf8`  
		Last Modified: Wed, 23 Mar 2022 23:36:36 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:254bb382ead8463cee898c2caef6986f5b11b5bc5347093f42f858f671572790`  
		Last Modified: Wed, 23 Mar 2022 23:36:36 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b52de5bfc4beeee7f5407c060c205958101b9a0a6e46501a6ee4854b95496a5f`  
		Last Modified: Wed, 23 Mar 2022 23:36:36 GMT  
		Size: 4.7 KB (4702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:11-alpine3.15` - linux; s390x

```console
$ docker pull postgres@sha256:db15a9659cb753bf62e12925dff362aeb511ad767b225d56af02b4873716be5e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **79.7 MB (79701040 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8d2f213dcf2f2c798e47177f8a4c636fc328543861b4e40cf4960fd9f1a2817d`
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
# Wed, 23 Mar 2022 19:49:24 GMT
ENV PG_MAJOR=11
# Wed, 23 Mar 2022 19:49:24 GMT
ENV PG_VERSION=11.15
# Wed, 23 Mar 2022 19:49:24 GMT
ENV PG_SHA256=c8f58e8ebd4f4567f4f9ba1032eb3e99e0251d87cbe3e564b485590e37a879e3
# Wed, 23 Mar 2022 19:52:00 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm-dev clang g++ 		make 		openldap-dev 		openssl-dev 		perl-dev 		perl-ipc-run 		perl-utils 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		zstd 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-krb5 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Wed, 23 Mar 2022 19:52:03 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample
# Wed, 23 Mar 2022 19:52:03 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Wed, 23 Mar 2022 19:52:03 GMT
ENV PGDATA=/var/lib/postgresql/data
# Wed, 23 Mar 2022 19:52:04 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Wed, 23 Mar 2022 19:52:04 GMT
VOLUME [/var/lib/postgresql/data]
# Wed, 23 Mar 2022 19:52:04 GMT
COPY file:e8928645623137de410cce68a2aa3b22f07a64e6391025598a60f3e461c606a3 in /usr/local/bin/ 
# Wed, 23 Mar 2022 19:52:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 23 Mar 2022 19:52:04 GMT
STOPSIGNAL SIGINT
# Wed, 23 Mar 2022 19:52:04 GMT
EXPOSE 5432
# Wed, 23 Mar 2022 19:52:04 GMT
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
	-	`sha256:5bfc278ca7f152b3de3cf4d84e6275671119e3c0932176492e3cfbd9e520d9a5`  
		Last Modified: Wed, 23 Mar 2022 19:57:08 GMT  
		Size: 77.1 MB (77084867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:178ba6735f8ad270ab08f11ecad7a991f0d4651e4b9b6babfd6ac4fbb5862da5`  
		Last Modified: Wed, 23 Mar 2022 19:56:59 GMT  
		Size: 8.0 KB (7987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6bd155285a36aae62296c2d95444f8d1410f91dbf7698d4fa99acc767b392f5`  
		Last Modified: Wed, 23 Mar 2022 19:56:59 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba40999c22844124bd3ba491878aa685f9f097de9d7382644b2c1c62b76c9fe6`  
		Last Modified: Wed, 23 Mar 2022 19:56:59 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcebfd148424ee0afded46244db4504bbab49b09d197c69865d03dbf067022c4`  
		Last Modified: Wed, 23 Mar 2022 19:56:59 GMT  
		Size: 4.7 KB (4700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
