## `postgres:13-alpine3.15`

```console
$ docker pull postgres@sha256:816e8a48deff56ecc585908c5117888b469f70b4cb7d3eddf55aaab21caa8cdf
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
$ docker pull postgres@sha256:06665316da2c856d3c0f1c57d7ecab15b743a7c207826f8c8c6858d8fcf65d3e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **78.3 MB (78285414 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c05347dd6fd6d159a5cc5f8a4f2560776e026143c8205e4a30c8d22d91fafef`
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
# Wed, 23 Mar 2022 23:31:47 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm-dev clang g++ 		make 		openldap-dev 		openssl-dev 		perl-dev 		perl-ipc-run 		perl-utils 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		zstd 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-krb5 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Wed, 23 Mar 2022 23:31:49 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample
# Wed, 23 Mar 2022 23:31:51 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Wed, 23 Mar 2022 23:31:51 GMT
ENV PGDATA=/var/lib/postgresql/data
# Wed, 23 Mar 2022 23:31:53 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Wed, 23 Mar 2022 23:31:53 GMT
VOLUME [/var/lib/postgresql/data]
# Wed, 23 Mar 2022 23:31:54 GMT
COPY file:e8928645623137de410cce68a2aa3b22f07a64e6391025598a60f3e461c606a3 in /usr/local/bin/ 
# Wed, 23 Mar 2022 23:31:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 23 Mar 2022 23:31:54 GMT
STOPSIGNAL SIGINT
# Wed, 23 Mar 2022 23:31:55 GMT
EXPOSE 5432
# Wed, 23 Mar 2022 23:31:55 GMT
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
	-	`sha256:6331c6ec370b79c3f958c9715e7c808876bb4b437fc3b712e92d944c64118c29`  
		Last Modified: Wed, 23 Mar 2022 23:50:28 GMT  
		Size: 75.6 MB (75645083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21a8535c5f11d90b77a4a8f705f034f84a0bd5829f0ba92c25c28315991d8660`  
		Last Modified: Wed, 23 Mar 2022 23:49:44 GMT  
		Size: 9.0 KB (9030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0524f9bff6d3b2ec5843d4dc8a459f978a2d824b5fe47229f4cbe6fe64740cff`  
		Last Modified: Wed, 23 Mar 2022 23:49:44 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ae0e9af86d412d9af9b3076fdd086defb8514650020f670b5773b13a049d7bd`  
		Last Modified: Wed, 23 Mar 2022 23:49:44 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:987bbab36d6ae2d9919c7e992abe1f1a43c94af12147481cfa0cd6b85775ecbd`  
		Last Modified: Wed, 23 Mar 2022 23:49:44 GMT  
		Size: 4.7 KB (4701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:13-alpine3.15` - linux; arm variant v7

```console
$ docker pull postgres@sha256:9b341943ad97a5e6488da991955c3b9642b381f45be6a0bbc48df4aeaa87f62d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.7 MB (73664969 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:795779ae8630df8c8ec48201a41010c721c7c752513d9b711a97fd73e22caaef`
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
# Wed, 23 Mar 2022 23:38:54 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm-dev clang g++ 		make 		openldap-dev 		openssl-dev 		perl-dev 		perl-ipc-run 		perl-utils 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		zstd 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-krb5 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Wed, 23 Mar 2022 23:38:57 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample
# Wed, 23 Mar 2022 23:38:59 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Wed, 23 Mar 2022 23:38:59 GMT
ENV PGDATA=/var/lib/postgresql/data
# Wed, 23 Mar 2022 23:39:02 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Wed, 23 Mar 2022 23:39:02 GMT
VOLUME [/var/lib/postgresql/data]
# Wed, 23 Mar 2022 23:39:03 GMT
COPY file:e8928645623137de410cce68a2aa3b22f07a64e6391025598a60f3e461c606a3 in /usr/local/bin/ 
# Wed, 23 Mar 2022 23:39:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 23 Mar 2022 23:39:04 GMT
STOPSIGNAL SIGINT
# Wed, 23 Mar 2022 23:39:05 GMT
EXPOSE 5432
# Wed, 23 Mar 2022 23:39:06 GMT
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
	-	`sha256:ff84007c01eaffd174aeda75620a5887999ae8247c659ec18f62f4c49b0298c6`  
		Last Modified: Wed, 23 Mar 2022 23:59:22 GMT  
		Size: 71.2 MB (71222396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:707786052f1647b14e8835471a62f6597bd70e5ccf01e3fd6d802be718025b38`  
		Last Modified: Wed, 23 Mar 2022 23:58:44 GMT  
		Size: 9.0 KB (9025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ae0bf511c0bc2c365d6e03a48b4f2186894c2a556ec1c085a59c2f105a48817`  
		Last Modified: Wed, 23 Mar 2022 23:58:44 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30399ee291fdb4f0a085563d3294cb11dcb2d48d8f41fb333262ce34529a5dfb`  
		Last Modified: Wed, 23 Mar 2022 23:58:44 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8a92286f07f371b7350f785895396b76ba7e23148da9d8bd171a1fb53f1b0c8`  
		Last Modified: Wed, 23 Mar 2022 23:58:44 GMT  
		Size: 4.7 KB (4699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:13-alpine3.15` - linux; arm64 variant v8

```console
$ docker pull postgres@sha256:d842fbc183ff96e64070dd44e1d8d7cec60e4e00038fd56d4bc96751f4d197e6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **79.1 MB (79138606 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f8a495fd7c136240d997136098ddd2e131e022531710e95f8a9fc661fef0e2af`
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
# Thu, 24 Mar 2022 07:14:34 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm-dev clang g++ 		make 		openldap-dev 		openssl-dev 		perl-dev 		perl-ipc-run 		perl-utils 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		zstd 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-krb5 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Thu, 24 Mar 2022 07:14:35 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample
# Thu, 24 Mar 2022 07:14:36 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 24 Mar 2022 07:14:37 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 24 Mar 2022 07:14:38 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 24 Mar 2022 07:14:39 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 24 Mar 2022 07:14:41 GMT
COPY file:e8928645623137de410cce68a2aa3b22f07a64e6391025598a60f3e461c606a3 in /usr/local/bin/ 
# Thu, 24 Mar 2022 07:14:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 24 Mar 2022 07:14:42 GMT
STOPSIGNAL SIGINT
# Thu, 24 Mar 2022 07:14:43 GMT
EXPOSE 5432
# Thu, 24 Mar 2022 07:14:44 GMT
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
	-	`sha256:99c28636303469a4ed1a0135e5c131a84d9b48ef4a862f41a9b2e04d69f717ef`  
		Last Modified: Thu, 24 Mar 2022 07:26:40 GMT  
		Size: 76.4 MB (76408496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd3bf1f868a811249b30f90b94479e070ec841acf302204a3d104bf825224bc7`  
		Last Modified: Thu, 24 Mar 2022 07:26:30 GMT  
		Size: 9.0 KB (9022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17367be588f3c65861dd317109a0c3469d14fa70dcbd6c2096065a506e46100c`  
		Last Modified: Thu, 24 Mar 2022 07:26:30 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecd6c8076f18b406bf63bda301eb3752ada62670e79712f077f7465d5d170216`  
		Last Modified: Thu, 24 Mar 2022 07:26:30 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07631b7c63d88ef2013d10393502eeea527907c5a1e22aa11e602689e6f398cd`  
		Last Modified: Thu, 24 Mar 2022 07:26:30 GMT  
		Size: 4.7 KB (4700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:13-alpine3.15` - linux; 386

```console
$ docker pull postgres@sha256:9a5351baf47832b0d27dc7410163b659e95bd2bb3be9c47b8084b80b375baf52
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **85.2 MB (85190237 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f5d9e901dac62b287c0d8a8eb043537cafda2353c3802330965d7a0d88cdae7`
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
# Thu, 24 Mar 2022 00:02:16 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm-dev clang g++ 		make 		openldap-dev 		openssl-dev 		perl-dev 		perl-ipc-run 		perl-utils 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		zstd 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-krb5 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Thu, 24 Mar 2022 00:02:16 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample
# Thu, 24 Mar 2022 00:02:17 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 24 Mar 2022 00:02:18 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 24 Mar 2022 00:02:19 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 24 Mar 2022 00:02:20 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 24 Mar 2022 00:02:22 GMT
COPY file:e8928645623137de410cce68a2aa3b22f07a64e6391025598a60f3e461c606a3 in /usr/local/bin/ 
# Thu, 24 Mar 2022 00:02:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 24 Mar 2022 00:02:23 GMT
STOPSIGNAL SIGINT
# Thu, 24 Mar 2022 00:02:24 GMT
EXPOSE 5432
# Thu, 24 Mar 2022 00:02:25 GMT
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
	-	`sha256:030d024a9707a070ef36dd71e346842c801846f97f7411dc0f989cb35ebafafe`  
		Last Modified: Thu, 24 Mar 2022 00:40:46 GMT  
		Size: 82.4 MB (82353009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62e32e68b7e7445bdebaa724c5ca8ddd2920aa166624cef1d147c4a6a84da52d`  
		Last Modified: Thu, 24 Mar 2022 00:40:36 GMT  
		Size: 9.0 KB (9025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a7c23c1e2086169019d5fc1dcc7ede2cfefc38c6e9831d41727a5a02113f388`  
		Last Modified: Thu, 24 Mar 2022 00:40:36 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d4cb931bd2786d26372ebee2d2416de3c067075852b36de8719d5f4adc2a2a6`  
		Last Modified: Thu, 24 Mar 2022 00:40:38 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c9cafe4daa864fcad39a6a40cc637eae48e551956dea182b8a5bcd947d79108`  
		Last Modified: Thu, 24 Mar 2022 00:40:36 GMT  
		Size: 4.7 KB (4701 bytes)  
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
$ docker pull postgres@sha256:383518a01f747fd111c3915dbdf7b3c6efbf5354d1320a260bf270c1a1094ba1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.6 MB (81632773 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dc0fb36cd8b51d51a54461fb76ac735b1a7772a9d7d31f1651145e80329a1d03`
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
# Wed, 23 Mar 2022 19:46:07 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm-dev clang g++ 		make 		openldap-dev 		openssl-dev 		perl-dev 		perl-ipc-run 		perl-utils 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		zstd 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-krb5 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Wed, 23 Mar 2022 19:46:10 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample
# Wed, 23 Mar 2022 19:46:11 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Wed, 23 Mar 2022 19:46:11 GMT
ENV PGDATA=/var/lib/postgresql/data
# Wed, 23 Mar 2022 19:46:11 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Wed, 23 Mar 2022 19:46:12 GMT
VOLUME [/var/lib/postgresql/data]
# Wed, 23 Mar 2022 19:46:12 GMT
COPY file:e8928645623137de410cce68a2aa3b22f07a64e6391025598a60f3e461c606a3 in /usr/local/bin/ 
# Wed, 23 Mar 2022 19:46:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 23 Mar 2022 19:46:12 GMT
STOPSIGNAL SIGINT
# Wed, 23 Mar 2022 19:46:12 GMT
EXPOSE 5432
# Wed, 23 Mar 2022 19:46:12 GMT
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
	-	`sha256:17061158ba2b88f40476eb61f0b1f79f1be823168a5a22a56552a022421371e5`  
		Last Modified: Wed, 23 Mar 2022 19:56:23 GMT  
		Size: 79.0 MB (79015563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42ecde9b3f81d1c2bd58ef263e102b5fe9914a87072049c17be0433b69a35626`  
		Last Modified: Wed, 23 Mar 2022 19:56:14 GMT  
		Size: 9.0 KB (9027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb32687f0c676d44dcaf6066f2318f95c3dc1274994c4236eb403dd77cabfe9f`  
		Last Modified: Wed, 23 Mar 2022 19:56:14 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:893b1ab74ecb0639c98074dea038faca8062e46dd5b4291441c8db488e08185c`  
		Last Modified: Wed, 23 Mar 2022 19:56:14 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63bb5a362cbcc5f187613741dd22da28146f9af8240756c52b5383026bbd9e87`  
		Last Modified: Wed, 23 Mar 2022 19:56:14 GMT  
		Size: 4.7 KB (4700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
