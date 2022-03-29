## `postgres:13-alpine3.15`

```console
$ docker pull postgres@sha256:f8ad68094852d61ef06510d22c1e2293cc9e7fd108aaf3b28a5c18ef9cfdda97
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

### `postgres:13-alpine3.15` - linux; amd64

```console
$ docker pull postgres@sha256:cdba8efb3127d1a3e7988a0ae72ef1b31ea075864ca5e335f4b856aada86acd2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **80.3 MB (80309465 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:414f0d09598496988acb2437a87e2865d79d21ceb60abd8ef4f3bceaaf2f6bc3`
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
# Wed, 23 Mar 2022 18:15:56 GMT
ENV PG_MAJOR=13
# Wed, 23 Mar 2022 18:15:56 GMT
ENV PG_VERSION=13.6
# Wed, 23 Mar 2022 18:15:56 GMT
ENV PG_SHA256=bafc7fa3d9d4da8fe71b84c63ba8bdfe8092935c30c0aa85c24b2c08508f67fc
# Wed, 23 Mar 2022 18:20:43 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm-dev clang g++ 		make 		openldap-dev 		openssl-dev 		perl-dev 		perl-ipc-run 		perl-utils 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		zstd 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-krb5 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Wed, 23 Mar 2022 18:20:44 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample
# Wed, 23 Mar 2022 18:20:44 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Wed, 23 Mar 2022 18:20:44 GMT
ENV PGDATA=/var/lib/postgresql/data
# Wed, 23 Mar 2022 18:20:45 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Wed, 23 Mar 2022 18:20:45 GMT
VOLUME [/var/lib/postgresql/data]
# Wed, 23 Mar 2022 18:20:45 GMT
COPY file:e8928645623137de410cce68a2aa3b22f07a64e6391025598a60f3e461c606a3 in /usr/local/bin/ 
# Wed, 23 Mar 2022 18:20:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 23 Mar 2022 18:20:45 GMT
STOPSIGNAL SIGINT
# Wed, 23 Mar 2022 18:20:45 GMT
EXPOSE 5432
# Wed, 23 Mar 2022 18:20:45 GMT
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
	-	`sha256:171825a3cd502106bc74cfcead9a4774203366ca98eeb468d7c2b96f4704c7f3`  
		Last Modified: Wed, 23 Mar 2022 18:36:52 GMT  
		Size: 77.5 MB (77481269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d012376224aacc740c30e62350a4bcb7a424c93f8d2d5ad2ccf25e222636d9a8`  
		Last Modified: Wed, 23 Mar 2022 18:36:42 GMT  
		Size: 9.0 KB (9023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:763b88b0622f090da0cce219735435e9428c4c8ed4156910849f56210ccbbfff`  
		Last Modified: Wed, 23 Mar 2022 18:36:42 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d36d4a5610eea8be4916e25589a56c1e5b0fc24d257bfc644a13c10e8329f17`  
		Last Modified: Wed, 23 Mar 2022 18:36:42 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e951de7b28b14b4f3b22b8dca85d7e7b61e362c0774a94dfddc0cf8dc08e7f9c`  
		Last Modified: Wed, 23 Mar 2022 18:36:42 GMT  
		Size: 4.7 KB (4700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:13-alpine3.15` - linux; arm variant v6

```console
$ docker pull postgres@sha256:0f00997e6ea042b219da3f2b496b52618dd7070a5c83d883fb9a86f53d3f9bf8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **78.7 MB (78736308 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:63f08efa0243d0aa188a2448055efbda28b31c7edc9b435b72db52575c6f338b`
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
# Wed, 23 Mar 2022 23:26:44 GMT
ENV PG_MAJOR=13
# Wed, 23 Mar 2022 23:26:44 GMT
ENV PG_VERSION=13.6
# Wed, 23 Mar 2022 23:26:45 GMT
ENV PG_SHA256=bafc7fa3d9d4da8fe71b84c63ba8bdfe8092935c30c0aa85c24b2c08508f67fc
# Tue, 29 Mar 2022 00:05:36 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm-dev clang g++ 		make 		openldap-dev 		openssl-dev 		perl-dev 		perl-ipc-run 		perl-utils 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-krb5 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 		zstd 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Tue, 29 Mar 2022 00:05:38 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample
# Tue, 29 Mar 2022 00:05:40 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 29 Mar 2022 00:05:40 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 29 Mar 2022 00:05:42 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 29 Mar 2022 00:05:42 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 29 Mar 2022 00:05:43 GMT
COPY file:e8928645623137de410cce68a2aa3b22f07a64e6391025598a60f3e461c606a3 in /usr/local/bin/ 
# Tue, 29 Mar 2022 00:05:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 29 Mar 2022 00:05:43 GMT
STOPSIGNAL SIGINT
# Tue, 29 Mar 2022 00:05:44 GMT
EXPOSE 5432
# Tue, 29 Mar 2022 00:05:44 GMT
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
	-	`sha256:9e8a5dd0af40e4298cc4a4ff95d89f97b7eb5c7686e89e4b20f95d587c79a615`  
		Last Modified: Tue, 29 Mar 2022 00:24:20 GMT  
		Size: 76.1 MB (76095977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9b87fd4a8d23290e28c72838b4df4ca1edae4560bfb32b6b19ad91bf59b1b83`  
		Last Modified: Tue, 29 Mar 2022 00:23:37 GMT  
		Size: 9.0 KB (9026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c918d58b64e0558c701e5e1edc3043fec1e93a99c23fa5b1c29734dda53df99a`  
		Last Modified: Tue, 29 Mar 2022 00:23:37 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:157d5a1a79f28f1d24cb67d71eae5404a0fd4bf98d6f8c50aff113f79bcd284d`  
		Last Modified: Tue, 29 Mar 2022 00:23:37 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8c71b82b83ccb8f0f90672313484b5ae838efd48e31d31cef7838d73630e7b6`  
		Last Modified: Tue, 29 Mar 2022 00:23:37 GMT  
		Size: 4.7 KB (4702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:13-alpine3.15` - linux; arm variant v7

```console
$ docker pull postgres@sha256:e786718fb4f7bd31a712bedd0b8726d571e18e395a1bb743f76783ef0c283d25
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.1 MB (74072234 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a1c323057988e95060acd5e4075b487ad4b1c46341e88aafcdf7ae77e36ceae`
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
# Wed, 23 Mar 2022 23:34:11 GMT
ENV PG_MAJOR=13
# Wed, 23 Mar 2022 23:34:12 GMT
ENV PG_VERSION=13.6
# Wed, 23 Mar 2022 23:34:12 GMT
ENV PG_SHA256=bafc7fa3d9d4da8fe71b84c63ba8bdfe8092935c30c0aa85c24b2c08508f67fc
# Tue, 29 Mar 2022 00:20:01 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm-dev clang g++ 		make 		openldap-dev 		openssl-dev 		perl-dev 		perl-ipc-run 		perl-utils 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-krb5 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 		zstd 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Tue, 29 Mar 2022 00:20:03 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample
# Tue, 29 Mar 2022 00:20:05 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 29 Mar 2022 00:20:05 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 29 Mar 2022 00:20:07 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 29 Mar 2022 00:20:07 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 29 Mar 2022 00:20:08 GMT
COPY file:e8928645623137de410cce68a2aa3b22f07a64e6391025598a60f3e461c606a3 in /usr/local/bin/ 
# Tue, 29 Mar 2022 00:20:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 29 Mar 2022 00:20:09 GMT
STOPSIGNAL SIGINT
# Tue, 29 Mar 2022 00:20:09 GMT
EXPOSE 5432
# Tue, 29 Mar 2022 00:20:10 GMT
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
	-	`sha256:7edc15a292b153fc0dc4af6a9c879ce62c19ee6c9854cba205b0e26e274af9bb`  
		Last Modified: Tue, 29 Mar 2022 00:40:16 GMT  
		Size: 71.6 MB (71629659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e481e3e8a062e649bb5f9a9a0c5312eac058b4d4f9e793016eed1b72d8eaf6f0`  
		Last Modified: Tue, 29 Mar 2022 00:39:38 GMT  
		Size: 9.0 KB (9025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a276f355b71063ecb6a8d66e13e532ebec14d6ff122155204fd56c9da1c8095`  
		Last Modified: Tue, 29 Mar 2022 00:39:38 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:553581abba0f878ec9eb5a939f876b8da2bdeb2e6880d4a5f1e1e9da231c019a`  
		Last Modified: Tue, 29 Mar 2022 00:39:38 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92dc863fbe678583f285023d9d946e26f76f10b72c1291801bedcb773d0a57c0`  
		Last Modified: Tue, 29 Mar 2022 00:39:38 GMT  
		Size: 4.7 KB (4700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:13-alpine3.15` - linux; arm64 variant v8

```console
$ docker pull postgres@sha256:e06a9a98f6d3193e173801aa0d3a3b3adf38e0ea72771889207b248e34ea8045
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **79.8 MB (79762617 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7c201fd823066157e7f9c8879e41f3d7495460b82c110904aae9f6900c49f1e`
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
# Thu, 24 Mar 2022 07:11:29 GMT
ENV PG_MAJOR=13
# Thu, 24 Mar 2022 07:11:30 GMT
ENV PG_VERSION=13.6
# Thu, 24 Mar 2022 07:11:31 GMT
ENV PG_SHA256=bafc7fa3d9d4da8fe71b84c63ba8bdfe8092935c30c0aa85c24b2c08508f67fc
# Mon, 28 Mar 2022 23:51:48 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm-dev clang g++ 		make 		openldap-dev 		openssl-dev 		perl-dev 		perl-ipc-run 		perl-utils 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-krb5 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 		zstd 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Mon, 28 Mar 2022 23:51:49 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample
# Mon, 28 Mar 2022 23:51:50 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Mon, 28 Mar 2022 23:51:51 GMT
ENV PGDATA=/var/lib/postgresql/data
# Mon, 28 Mar 2022 23:51:52 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Mon, 28 Mar 2022 23:51:53 GMT
VOLUME [/var/lib/postgresql/data]
# Mon, 28 Mar 2022 23:51:55 GMT
COPY file:e8928645623137de410cce68a2aa3b22f07a64e6391025598a60f3e461c606a3 in /usr/local/bin/ 
# Mon, 28 Mar 2022 23:51:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 28 Mar 2022 23:51:56 GMT
STOPSIGNAL SIGINT
# Mon, 28 Mar 2022 23:51:57 GMT
EXPOSE 5432
# Mon, 28 Mar 2022 23:51:58 GMT
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
	-	`sha256:1c6e2317551abdd05d9b805ed3308dd9e5781b47ad604f36da138bb67b7676b0`  
		Last Modified: Tue, 29 Mar 2022 00:09:50 GMT  
		Size: 77.0 MB (77032508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6468eb974783e329e0c09195c99bef7eb23980ed8844c8c0add8caa4b0cf4051`  
		Last Modified: Tue, 29 Mar 2022 00:09:41 GMT  
		Size: 9.0 KB (9019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:558e2382614d330df4b6dd886563012390357daeb1a38d0f04e20f5c223ef23e`  
		Last Modified: Tue, 29 Mar 2022 00:09:41 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cabbd548c014351bf1599de76a57670ad0879a26152b2d7f7446ae374e8f0d88`  
		Last Modified: Tue, 29 Mar 2022 00:09:40 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a70407d68ebe6d54ca5afb5e7c885bc896e2c3e586dbda47b95f5b1c092f9df7`  
		Last Modified: Tue, 29 Mar 2022 00:09:41 GMT  
		Size: 4.7 KB (4700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:13-alpine3.15` - linux; 386

```console
$ docker pull postgres@sha256:389a5abf64e76c77d3e22496da30432ec8eb943643b974cfb89491fa690bcbc0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **85.8 MB (85805521 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:daab364ff1104b130cb917ed20073dfa16eb90f37fd2c0fc28f76acf0f762795`
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
# Wed, 23 Mar 2022 23:58:57 GMT
ENV PG_MAJOR=13
# Wed, 23 Mar 2022 23:58:58 GMT
ENV PG_VERSION=13.6
# Wed, 23 Mar 2022 23:58:59 GMT
ENV PG_SHA256=bafc7fa3d9d4da8fe71b84c63ba8bdfe8092935c30c0aa85c24b2c08508f67fc
# Mon, 28 Mar 2022 23:45:57 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm-dev clang g++ 		make 		openldap-dev 		openssl-dev 		perl-dev 		perl-ipc-run 		perl-utils 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-krb5 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 		zstd 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Mon, 28 Mar 2022 23:45:58 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample
# Mon, 28 Mar 2022 23:45:58 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Mon, 28 Mar 2022 23:45:59 GMT
ENV PGDATA=/var/lib/postgresql/data
# Mon, 28 Mar 2022 23:46:00 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Mon, 28 Mar 2022 23:46:01 GMT
VOLUME [/var/lib/postgresql/data]
# Mon, 28 Mar 2022 23:46:03 GMT
COPY file:e8928645623137de410cce68a2aa3b22f07a64e6391025598a60f3e461c606a3 in /usr/local/bin/ 
# Mon, 28 Mar 2022 23:46:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 28 Mar 2022 23:46:04 GMT
STOPSIGNAL SIGINT
# Mon, 28 Mar 2022 23:46:05 GMT
EXPOSE 5432
# Mon, 28 Mar 2022 23:46:06 GMT
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
	-	`sha256:2ce4d922be25b6f5e3405af4ce89952dc02bbc1fa4a4a06af4d1f7c6cd09459d`  
		Last Modified: Mon, 28 Mar 2022 23:58:22 GMT  
		Size: 83.0 MB (82968292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02697625e4810b57b4ad0eb9187325b4d9e0e731412a9b501b668811a08ea535`  
		Last Modified: Mon, 28 Mar 2022 23:58:12 GMT  
		Size: 9.0 KB (9023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db143ddcb0dc34d217821a3a5af2b5d093bd97da3f883fffeb9da5e71f7c70e0`  
		Last Modified: Mon, 28 Mar 2022 23:58:13 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:225b9e800af499ef55121cc06fe9d0887f262cbd2eaf7162c4f6581e748e16c3`  
		Last Modified: Mon, 28 Mar 2022 23:58:12 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac97b65cf3be3d8a3a6bffa7d3a8d6b4664a54cda5027d28baabd9d0b6ce0675`  
		Last Modified: Mon, 28 Mar 2022 23:58:12 GMT  
		Size: 4.7 KB (4702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:13-alpine3.15` - linux; ppc64le

```console
$ docker pull postgres@sha256:cbbcbc8923c1a49d7fcbf041c439a412be0e7c52ae776832e23b6723ba118676
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **85.6 MB (85597550 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:45e32595309aecb72f0cdc46f267fdcd9d7ac12c40d9ddf91a6a3b5a7e1a5f47`
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
# Wed, 23 Mar 2022 23:10:44 GMT
ENV PG_MAJOR=13
# Wed, 23 Mar 2022 23:11:00 GMT
ENV PG_VERSION=13.6
# Wed, 23 Mar 2022 23:11:12 GMT
ENV PG_SHA256=bafc7fa3d9d4da8fe71b84c63ba8bdfe8092935c30c0aa85c24b2c08508f67fc
# Wed, 23 Mar 2022 23:15:42 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm-dev clang g++ 		make 		openldap-dev 		openssl-dev 		perl-dev 		perl-ipc-run 		perl-utils 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		zstd 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-krb5 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Wed, 23 Mar 2022 23:15:54 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample
# Wed, 23 Mar 2022 23:16:03 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Wed, 23 Mar 2022 23:16:05 GMT
ENV PGDATA=/var/lib/postgresql/data
# Wed, 23 Mar 2022 23:16:11 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Wed, 23 Mar 2022 23:16:15 GMT
VOLUME [/var/lib/postgresql/data]
# Wed, 23 Mar 2022 23:16:17 GMT
COPY file:e8928645623137de410cce68a2aa3b22f07a64e6391025598a60f3e461c606a3 in /usr/local/bin/ 
# Wed, 23 Mar 2022 23:16:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 23 Mar 2022 23:16:26 GMT
STOPSIGNAL SIGINT
# Wed, 23 Mar 2022 23:16:34 GMT
EXPOSE 5432
# Wed, 23 Mar 2022 23:16:37 GMT
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
	-	`sha256:79626f7d272ad2c323979c6f4f50c70996c036ac1a620d4f1ca5627d6a21b9cb`  
		Last Modified: Wed, 23 Mar 2022 23:35:36 GMT  
		Size: 82.8 MB (82768001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:216074f3496765ba0f83beb36f3b98343017d6338f914d569bb822ebdc59925b`  
		Last Modified: Wed, 23 Mar 2022 23:35:23 GMT  
		Size: 9.0 KB (9027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42c2d5b064216972380003c2644a4da4c4c763a3adb0a2cf1063590be369b284`  
		Last Modified: Wed, 23 Mar 2022 23:35:23 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9837d612ba93351bba4831b7caa743bac07b1fe7ea5c53c80efb0a2afa08303c`  
		Last Modified: Wed, 23 Mar 2022 23:35:23 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8f836a155fab2c408f86fb1beb9fc599690b9287595ee4d7e9b5fdedcb092a9`  
		Last Modified: Wed, 23 Mar 2022 23:35:23 GMT  
		Size: 4.7 KB (4701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:13-alpine3.15` - linux; s390x

```console
$ docker pull postgres@sha256:339d895d6d0e3d80a21d8e5c869f94519fcea965475205bf20bb021c48c84b55
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **82.2 MB (82233664 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab8a90b40fd57f545ba399256ba726af109430c7d17f6a2256f7740b86215623`
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
# Wed, 23 Mar 2022 19:43:24 GMT
ENV PG_MAJOR=13
# Wed, 23 Mar 2022 19:43:24 GMT
ENV PG_VERSION=13.6
# Wed, 23 Mar 2022 19:43:24 GMT
ENV PG_SHA256=bafc7fa3d9d4da8fe71b84c63ba8bdfe8092935c30c0aa85c24b2c08508f67fc
# Mon, 28 Mar 2022 23:48:20 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm-dev clang g++ 		make 		openldap-dev 		openssl-dev 		perl-dev 		perl-ipc-run 		perl-utils 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-krb5 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 		zstd 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Mon, 28 Mar 2022 23:48:23 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample
# Mon, 28 Mar 2022 23:48:24 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Mon, 28 Mar 2022 23:48:24 GMT
ENV PGDATA=/var/lib/postgresql/data
# Mon, 28 Mar 2022 23:48:24 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Mon, 28 Mar 2022 23:48:25 GMT
VOLUME [/var/lib/postgresql/data]
# Mon, 28 Mar 2022 23:48:25 GMT
COPY file:e8928645623137de410cce68a2aa3b22f07a64e6391025598a60f3e461c606a3 in /usr/local/bin/ 
# Mon, 28 Mar 2022 23:48:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 28 Mar 2022 23:48:25 GMT
STOPSIGNAL SIGINT
# Mon, 28 Mar 2022 23:48:25 GMT
EXPOSE 5432
# Mon, 28 Mar 2022 23:48:25 GMT
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
	-	`sha256:63854c0856d06025686ad5a442f45c11a6a7547896ccfd165ec740785266a147`  
		Last Modified: Tue, 29 Mar 2022 00:02:57 GMT  
		Size: 79.6 MB (79616458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2462bf2b1795534972f36fd39575def272b93f9cb3b1da233fcab4a0a6d9d1c`  
		Last Modified: Tue, 29 Mar 2022 00:02:53 GMT  
		Size: 9.0 KB (9024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:024c01f13db7524f03b8d9e43c08e21973f9667522d159d2bae63ba3fdb2b8b1`  
		Last Modified: Tue, 29 Mar 2022 00:02:53 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04b960ef877191fb585725ea8551c04a05dd3a5f4391ebebb6cea7f5a4d16550`  
		Last Modified: Tue, 29 Mar 2022 00:02:53 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2306ef655cad1f33bf5c10283647fc17d64371e9542a28f84a06d6d97b03b9b`  
		Last Modified: Tue, 29 Mar 2022 00:02:48 GMT  
		Size: 4.7 KB (4700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
