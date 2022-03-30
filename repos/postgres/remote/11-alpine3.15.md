## `postgres:11-alpine3.15`

```console
$ docker pull postgres@sha256:4e3313956a3d88fc13a7d3786c25d67dd034bd921459958819832f0769a33e3a
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
$ docker pull postgres@sha256:a36dfe5c51b29470e4c90e511001a73f51522d53636dd3beb89210c38fb66400
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **79.1 MB (79124161 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7942142a9c5038376a98b46858f25c5ea0d5ff31b2e2fe7ec86fb6e908ad63e2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 29 Mar 2022 00:19:36 GMT
ADD file:3b5a33c96fd3c10d0c438d907ce172903f7b2bde0f4e5107831e135ddf111b19 in / 
# Tue, 29 Mar 2022 00:19:36 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 04:35:10 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Tue, 29 Mar 2022 04:35:10 GMT
ENV LANG=en_US.utf8
# Tue, 29 Mar 2022 04:35:11 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 29 Mar 2022 04:52:44 GMT
ENV PG_MAJOR=11
# Tue, 29 Mar 2022 04:52:44 GMT
ENV PG_VERSION=11.15
# Tue, 29 Mar 2022 04:52:44 GMT
ENV PG_SHA256=c8f58e8ebd4f4567f4f9ba1032eb3e99e0251d87cbe3e564b485590e37a879e3
# Tue, 29 Mar 2022 04:57:11 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm-dev clang g++ 		make 		openldap-dev 		openssl-dev 		perl-dev 		perl-ipc-run 		perl-utils 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-krb5 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 		zstd 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Tue, 29 Mar 2022 04:57:12 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample
# Tue, 29 Mar 2022 04:57:13 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 29 Mar 2022 04:57:13 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 29 Mar 2022 04:57:14 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 29 Mar 2022 04:57:14 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 29 Mar 2022 04:57:14 GMT
COPY file:e8928645623137de410cce68a2aa3b22f07a64e6391025598a60f3e461c606a3 in /usr/local/bin/ 
# Tue, 29 Mar 2022 04:57:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 29 Mar 2022 04:57:14 GMT
STOPSIGNAL SIGINT
# Tue, 29 Mar 2022 04:57:14 GMT
EXPOSE 5432
# Tue, 29 Mar 2022 04:57:14 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:40e059520d199e1a1a259089077f2a0c879951c9a4540490bad3a0d7714c6ae7`  
		Last Modified: Mon, 28 Mar 2022 23:30:57 GMT  
		Size: 2.8 MB (2814512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7cb04fc09966f66dad51ce1cf7300e8aae1694099ab28b11896563195c0308d`  
		Last Modified: Tue, 29 Mar 2022 05:02:50 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd3fde6b0ba8b972cc7040ff216b6b54600806651e1103d4dcdf3e36afdd25e7`  
		Last Modified: Tue, 29 Mar 2022 05:02:50 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb9d19de46b0b4226456ccc2e8c3a895ccd62f967c28fb56031840b0c993fb0b`  
		Last Modified: Tue, 29 Mar 2022 05:06:11 GMT  
		Size: 76.3 MB (76295169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b29c7398245ef8618e20bfce9ed8a9887b4df391a241be579b9b216c0cd0c89`  
		Last Modified: Tue, 29 Mar 2022 05:06:00 GMT  
		Size: 8.0 KB (7990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7619f74396f0f12587a24a79286c6e7f0947813e5f2da5a5ca58a74466d2744f`  
		Last Modified: Tue, 29 Mar 2022 05:06:00 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:105f2276fc643a389cdea81ba11d20eb33bacd57590cdcb839f0b886dcc7403a`  
		Last Modified: Tue, 29 Mar 2022 05:06:00 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c118d9d80c2c543e4fe06a0e4d94b9ae4ff4ef07cd659cdc8c31f085fd8b8161`  
		Last Modified: Tue, 29 Mar 2022 05:06:00 GMT  
		Size: 4.7 KB (4700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:11-alpine3.15` - linux; arm variant v6

```console
$ docker pull postgres@sha256:e4f344866bf10ce7136adf4606ce95ed9e98de0e788e939956b33eed93c51014
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.0 MB (76953920 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:effc3b1bc9075f8fc89b9f2e4d59622c7dae18ba3a6ed386c1aee829d3810877`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 29 Mar 2022 00:49:32 GMT
ADD file:44acf536d487bec7f7bf16561f4ec90e60d4447b3cbabfeca66953c4491aabeb in / 
# Tue, 29 Mar 2022 00:49:33 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 08:35:52 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Tue, 29 Mar 2022 08:35:53 GMT
ENV LANG=en_US.utf8
# Tue, 29 Mar 2022 08:35:54 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 29 Mar 2022 08:53:01 GMT
ENV PG_MAJOR=11
# Tue, 29 Mar 2022 08:53:01 GMT
ENV PG_VERSION=11.15
# Tue, 29 Mar 2022 08:53:02 GMT
ENV PG_SHA256=c8f58e8ebd4f4567f4f9ba1032eb3e99e0251d87cbe3e564b485590e37a879e3
# Tue, 29 Mar 2022 08:57:45 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm-dev clang g++ 		make 		openldap-dev 		openssl-dev 		perl-dev 		perl-ipc-run 		perl-utils 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-krb5 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 		zstd 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Tue, 29 Mar 2022 08:57:48 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample
# Tue, 29 Mar 2022 08:57:50 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 29 Mar 2022 08:57:50 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 29 Mar 2022 08:57:52 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 29 Mar 2022 08:57:53 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 29 Mar 2022 08:57:53 GMT
COPY file:e8928645623137de410cce68a2aa3b22f07a64e6391025598a60f3e461c606a3 in /usr/local/bin/ 
# Tue, 29 Mar 2022 08:57:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 29 Mar 2022 08:57:54 GMT
STOPSIGNAL SIGINT
# Tue, 29 Mar 2022 08:57:55 GMT
EXPOSE 5432
# Tue, 29 Mar 2022 08:57:55 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:84f033dabe5013c0dfae4263abd951011719d0a15adc3c7312c5be994deff030`  
		Last Modified: Tue, 29 Mar 2022 00:51:25 GMT  
		Size: 2.6 MB (2621943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7748deb378b52b01d1210ccde1068b8232a159d4e67dacfcb351d00e5d4e652d`  
		Last Modified: Tue, 29 Mar 2022 09:03:50 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:757a14ba8cbb07c226f75e0a623339c0306a0b11de115bf4d73d7eab0abddeba`  
		Last Modified: Tue, 29 Mar 2022 09:03:50 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66e9893d1870dcff5f218c26a1df8d80dad699fa98495d7e16025abab984ffca`  
		Last Modified: Tue, 29 Mar 2022 09:07:41 GMT  
		Size: 74.3 MB (74317503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df713b733a62bd07a0ee1d47a8706ac97af06df417ce685043be4a6b9f8c9490`  
		Last Modified: Tue, 29 Mar 2022 09:06:57 GMT  
		Size: 8.0 KB (7989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7871754bccf6a99e538f835c5c8ac5853089ffc4a71d4f3cb489008fb91c045`  
		Last Modified: Tue, 29 Mar 2022 09:06:57 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b4d7c4c8ba63b3b2fa189dd16e36f39e14297f4cf87722b96bd3e95dc123b29`  
		Last Modified: Tue, 29 Mar 2022 09:06:57 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:690d50daa7aa7fcb491dc0cc2b25a98617563937c29a481edad3c4c4c6d2feea`  
		Last Modified: Tue, 29 Mar 2022 09:06:57 GMT  
		Size: 4.7 KB (4697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:11-alpine3.15` - linux; arm variant v7

```console
$ docker pull postgres@sha256:d51a786ec04e57ef9ca3cb431c022e7bf8e7b4eba3e73eb2c2fe1993bcd37299
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.4 MB (72377879 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d9c3472cd05f38f6250bf4694e14333c5eb4b5085919b1e9dd3df24bda70768d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 29 Mar 2022 02:13:28 GMT
ADD file:8c959b80e3661beea7b3468017b88897d981bf52ed43c074e7c87ecb753e9059 in / 
# Tue, 29 Mar 2022 02:13:28 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 03:21:41 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Tue, 29 Mar 2022 03:21:41 GMT
ENV LANG=en_US.utf8
# Tue, 29 Mar 2022 03:21:43 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 29 Mar 2022 05:38:57 GMT
ENV PG_MAJOR=11
# Tue, 29 Mar 2022 05:38:58 GMT
ENV PG_VERSION=11.15
# Tue, 29 Mar 2022 05:38:58 GMT
ENV PG_SHA256=c8f58e8ebd4f4567f4f9ba1032eb3e99e0251d87cbe3e564b485590e37a879e3
# Tue, 29 Mar 2022 05:43:27 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm-dev clang g++ 		make 		openldap-dev 		openssl-dev 		perl-dev 		perl-ipc-run 		perl-utils 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-krb5 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 		zstd 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Tue, 29 Mar 2022 05:43:29 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample
# Tue, 29 Mar 2022 05:43:30 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 29 Mar 2022 05:43:31 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 29 Mar 2022 05:43:32 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 29 Mar 2022 05:43:33 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 29 Mar 2022 05:43:33 GMT
COPY file:e8928645623137de410cce68a2aa3b22f07a64e6391025598a60f3e461c606a3 in /usr/local/bin/ 
# Tue, 29 Mar 2022 05:43:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 29 Mar 2022 05:43:34 GMT
STOPSIGNAL SIGINT
# Tue, 29 Mar 2022 05:43:34 GMT
EXPOSE 5432
# Tue, 29 Mar 2022 05:43:35 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:22b1e5a07a97d7af6fdc335e3b3a975b73908fa19b084289c408a00814da0398`  
		Last Modified: Tue, 29 Mar 2022 02:15:28 GMT  
		Size: 2.4 MB (2424303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6efa95512275c1dc3e2e9d61d2034aeea997b464fe3a7f3f8ff67c360d7780d4`  
		Last Modified: Tue, 29 Mar 2022 06:37:26 GMT  
		Size: 1.3 KB (1283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5c20db44a9534da25352d3b2d6c0153f75b99cded4f03763d17d210642eeb29`  
		Last Modified: Tue, 29 Mar 2022 06:37:26 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:584231895171104513fbe36514612de00b1ffcaa013348459dcaa131458aa9a7`  
		Last Modified: Tue, 29 Mar 2022 06:45:17 GMT  
		Size: 69.9 MB (69939105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e3a5bd3a74c70c21168ab9f2386139b5df6b9d05d428a92a79d496297300555`  
		Last Modified: Tue, 29 Mar 2022 06:44:39 GMT  
		Size: 8.0 KB (7983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ced7a1aa0a0dc719a711f8605a754780631f4984f7621a3baec01fe0fa8285e7`  
		Last Modified: Tue, 29 Mar 2022 06:44:39 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2eb727733faffcd678a9fbc391346c8fb0353e9e6bc6392ef61aab09424b8ef`  
		Last Modified: Tue, 29 Mar 2022 06:44:39 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:808500e7f8c3aa71d7690402d42f1374519dd8a8e438fb5b7c49fb80a93038b4`  
		Last Modified: Tue, 29 Mar 2022 06:44:40 GMT  
		Size: 4.7 KB (4702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:11-alpine3.15` - linux; arm64 variant v8

```console
$ docker pull postgres@sha256:5501efb85fec34e3572c79049e34e3a43ed69907e9c1e1d68aa8729ef7072bca
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **78.0 MB (77976922 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cecbb13f758f487050c528ead616357c2e1368692bd46d8a8bba96f766f84ed0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 29 Mar 2022 00:40:05 GMT
ADD file:24e8b04304ef91bbf949674909ccaf2c66e3dcd096c3c307a0510569eadf576f in / 
# Tue, 29 Mar 2022 00:40:05 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 12:32:20 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Tue, 29 Mar 2022 12:32:21 GMT
ENV LANG=en_US.utf8
# Tue, 29 Mar 2022 12:32:22 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 29 Mar 2022 13:04:05 GMT
ENV PG_MAJOR=11
# Tue, 29 Mar 2022 13:04:06 GMT
ENV PG_VERSION=11.15
# Tue, 29 Mar 2022 13:04:07 GMT
ENV PG_SHA256=c8f58e8ebd4f4567f4f9ba1032eb3e99e0251d87cbe3e564b485590e37a879e3
# Tue, 29 Mar 2022 13:09:11 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm-dev clang g++ 		make 		openldap-dev 		openssl-dev 		perl-dev 		perl-ipc-run 		perl-utils 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-krb5 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 		zstd 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Tue, 29 Mar 2022 13:09:12 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample
# Tue, 29 Mar 2022 13:09:13 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 29 Mar 2022 13:09:14 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 29 Mar 2022 13:09:15 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 29 Mar 2022 13:09:16 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 29 Mar 2022 13:09:18 GMT
COPY file:e8928645623137de410cce68a2aa3b22f07a64e6391025598a60f3e461c606a3 in /usr/local/bin/ 
# Tue, 29 Mar 2022 13:09:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 29 Mar 2022 13:09:19 GMT
STOPSIGNAL SIGINT
# Tue, 29 Mar 2022 13:09:20 GMT
EXPOSE 5432
# Tue, 29 Mar 2022 13:09:21 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:80fa7f07ec7b717ec5f8e2717b91e3d659e129052ec3def2570a5674322688d9`  
		Last Modified: Tue, 29 Mar 2022 00:41:08 GMT  
		Size: 2.7 MB (2716347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b439f782e5aee029ecc24d7332fd55b1d41b1853148bfa9f8e2de3471cf12f0`  
		Last Modified: Tue, 29 Mar 2022 13:27:49 GMT  
		Size: 1.3 KB (1256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7d60a8ccf71b5d8b05839b27e56f69040a1c957686702919c4986826949d2fb`  
		Last Modified: Tue, 29 Mar 2022 13:27:49 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a6eefdea8b48472a2e9ad9ca2796f6e9db914e8f7be2c29b5299cb02799c180`  
		Last Modified: Tue, 29 Mar 2022 13:31:29 GMT  
		Size: 75.2 MB (75246213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b397912a89d36ec7865ce369f042e9cc1ec14c63552d63a3d8e66cdba6c61062`  
		Last Modified: Tue, 29 Mar 2022 13:31:19 GMT  
		Size: 8.0 KB (7989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1862c41adb5bc97353391272971e518fe9db17e192c050fb4c59362ea062e3d`  
		Last Modified: Tue, 29 Mar 2022 13:31:19 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e75828846962b4d27086bcdf55deae3270a182ff0acfee939379db4da83e4120`  
		Last Modified: Tue, 29 Mar 2022 13:31:19 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b83dc53493889216b5f201b6fe697f6e2db1c04096881d0dbe2a18a8102309ab`  
		Last Modified: Tue, 29 Mar 2022 13:31:20 GMT  
		Size: 4.7 KB (4701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:11-alpine3.15` - linux; 386

```console
$ docker pull postgres@sha256:a628c8fe83389b5670bb131bb44c0edbcb5945c92975d1d048b12c81ccd949bc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **83.8 MB (83833733 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d41e817a9b6a59dad75e4903efe67c9425aff2a5c58e3e01807655a0b761b2f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 29 Mar 2022 00:38:32 GMT
ADD file:8d3b249cd4cd9b2fb1888f3efcc06d39c2f56b4c25257ecee645c1be0146f7fd in / 
# Tue, 29 Mar 2022 00:38:33 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 11:32:27 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Tue, 29 Mar 2022 11:32:28 GMT
ENV LANG=en_US.utf8
# Tue, 29 Mar 2022 11:32:29 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 29 Mar 2022 12:22:46 GMT
ENV PG_MAJOR=11
# Tue, 29 Mar 2022 12:22:47 GMT
ENV PG_VERSION=11.15
# Tue, 29 Mar 2022 12:22:48 GMT
ENV PG_SHA256=c8f58e8ebd4f4567f4f9ba1032eb3e99e0251d87cbe3e564b485590e37a879e3
# Tue, 29 Mar 2022 12:25:53 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm-dev clang g++ 		make 		openldap-dev 		openssl-dev 		perl-dev 		perl-ipc-run 		perl-utils 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-krb5 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 		zstd 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Tue, 29 Mar 2022 12:25:53 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample
# Tue, 29 Mar 2022 12:25:54 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 29 Mar 2022 12:25:55 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 29 Mar 2022 12:25:56 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 29 Mar 2022 12:25:57 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 29 Mar 2022 12:25:59 GMT
COPY file:e8928645623137de410cce68a2aa3b22f07a64e6391025598a60f3e461c606a3 in /usr/local/bin/ 
# Tue, 29 Mar 2022 12:25:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 29 Mar 2022 12:26:00 GMT
STOPSIGNAL SIGINT
# Tue, 29 Mar 2022 12:26:01 GMT
EXPOSE 5432
# Tue, 29 Mar 2022 12:26:02 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:134f45dc6b904419acf27b9807970f271117691bc67b963b86de8965db932175`  
		Last Modified: Tue, 29 Mar 2022 00:39:35 GMT  
		Size: 2.8 MB (2818926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f945fcbf5171d3e4e6e2ab1f12d733ed4f9c6c8d1715b476d8febaf9dd28f57`  
		Last Modified: Tue, 29 Mar 2022 12:40:38 GMT  
		Size: 1.3 KB (1254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb32ff4ea2172e863b81903a0d2e9f2dab0a281bff200bbf38a227fa42c2a1da`  
		Last Modified: Tue, 29 Mar 2022 12:40:38 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b65d5b849c3e70909069075c21ef0ce5bdc30e8a085feffb44052f87d5c2d7ce`  
		Last Modified: Tue, 29 Mar 2022 12:44:26 GMT  
		Size: 81.0 MB (81000453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4153371a49b4d3591ef0d74372c16971199b42dee6c8cf45c291bee48fa05c9`  
		Last Modified: Tue, 29 Mar 2022 12:44:16 GMT  
		Size: 8.0 KB (7987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78ff5dfb969a48510db4fa95d398eebb5f17b629b7f99f23aae5d105291eedc8`  
		Last Modified: Tue, 29 Mar 2022 12:44:16 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae96d183efc46e36cac9d739d0787ef1d9cd3102c4a4af0ac53e22b4489a9438`  
		Last Modified: Tue, 29 Mar 2022 12:44:16 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bb81df37fa828e72e6a677857d057bbdfe0f18338dae37354201505f6d78fd0`  
		Last Modified: Tue, 29 Mar 2022 12:44:16 GMT  
		Size: 4.7 KB (4698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:11-alpine3.15` - linux; ppc64le

```console
$ docker pull postgres@sha256:90f1e534e031c9fd0a95d98827c6587d6e21249002d0ea8d60f87e1809dbd59e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.4 MB (84354219 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9abdbfe30c99ba22ddd0c7833a03fc37fbbb613a3ba1fc6ece8a0c7e35c81da9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 29 Mar 2022 00:16:52 GMT
ADD file:9e7b65a431d59070abaadae56d9c3fc59c899af881939e4353b1f524b2bd5185 in / 
# Tue, 29 Mar 2022 00:16:55 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 05:31:20 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Tue, 29 Mar 2022 05:31:22 GMT
ENV LANG=en_US.utf8
# Tue, 29 Mar 2022 05:31:28 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 29 Mar 2022 05:55:04 GMT
ENV PG_MAJOR=11
# Tue, 29 Mar 2022 05:55:07 GMT
ENV PG_VERSION=11.15
# Tue, 29 Mar 2022 05:55:10 GMT
ENV PG_SHA256=c8f58e8ebd4f4567f4f9ba1032eb3e99e0251d87cbe3e564b485590e37a879e3
# Tue, 29 Mar 2022 05:59:43 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm-dev clang g++ 		make 		openldap-dev 		openssl-dev 		perl-dev 		perl-ipc-run 		perl-utils 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-krb5 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 		zstd 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Tue, 29 Mar 2022 05:59:59 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample
# Tue, 29 Mar 2022 06:00:08 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 29 Mar 2022 06:00:11 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 29 Mar 2022 06:00:20 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 29 Mar 2022 06:00:22 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 29 Mar 2022 06:00:25 GMT
COPY file:e8928645623137de410cce68a2aa3b22f07a64e6391025598a60f3e461c606a3 in /usr/local/bin/ 
# Tue, 29 Mar 2022 06:00:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 29 Mar 2022 06:00:38 GMT
STOPSIGNAL SIGINT
# Tue, 29 Mar 2022 06:00:44 GMT
EXPOSE 5432
# Tue, 29 Mar 2022 06:00:49 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:1c611bca4fa49cac5bc1e3826ad53fee85ed659d24bffcccd86c3f04be07339a`  
		Last Modified: Tue, 29 Mar 2022 00:18:26 GMT  
		Size: 2.8 MB (2811009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0270fd1b7d407719c8c12f907a2ee08b355530920c5b0735fd2c5f92c5ac0ff7`  
		Last Modified: Tue, 29 Mar 2022 06:11:36 GMT  
		Size: 1.3 KB (1283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62ce97e0c46a6dc8604b20f4c3da1f09ca7f224554227f87dc8fa14735c15a48`  
		Last Modified: Tue, 29 Mar 2022 06:11:36 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e63a30590523b5000005b645a304239cfab0594fc5e2787568f7a1d4d37307f`  
		Last Modified: Tue, 29 Mar 2022 06:15:21 GMT  
		Size: 81.5 MB (81528730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87c90b3bc55e008ebf35b57884641c5a52241fe343f7da38c3e1c192aea9f4fb`  
		Last Modified: Tue, 29 Mar 2022 06:15:08 GMT  
		Size: 8.0 KB (7992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:377402d7cc0de812cdb15017ad4ac2e067f172fac70c5e96c83fc80d30e6b15e`  
		Last Modified: Tue, 29 Mar 2022 06:15:08 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b61631271125b7c50768a85a3b345cbd84e464f30b87e5bb5d05f750d721f600`  
		Last Modified: Tue, 29 Mar 2022 06:15:07 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38afbafd6abd08528ddc76ddf1a75b1205522fb71369cee1bc2da8c09e058dfa`  
		Last Modified: Tue, 29 Mar 2022 06:15:07 GMT  
		Size: 4.7 KB (4701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:11-alpine3.15` - linux; s390x

```console
$ docker pull postgres@sha256:137b5d957a08d16641f98ea7e5e430553c48afd4a9e055443b66b978fc62a10b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **80.3 MB (80250105 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0397110378f8d140a35c6a013c646396262e8cae0474129c40325dd0fd96ec5a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 29 Mar 2022 00:41:32 GMT
ADD file:75e6f1cb0cdf63de14d99f8419ce47d61e295300299c18b08bd484dff0da4e93 in / 
# Tue, 29 Mar 2022 00:41:32 GMT
CMD ["/bin/sh"]
# Wed, 30 Mar 2022 01:14:17 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Wed, 30 Mar 2022 01:14:17 GMT
ENV LANG=en_US.utf8
# Wed, 30 Mar 2022 01:14:17 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 30 Mar 2022 01:43:04 GMT
ENV PG_MAJOR=11
# Wed, 30 Mar 2022 01:43:04 GMT
ENV PG_VERSION=11.15
# Wed, 30 Mar 2022 01:43:04 GMT
ENV PG_SHA256=c8f58e8ebd4f4567f4f9ba1032eb3e99e0251d87cbe3e564b485590e37a879e3
# Wed, 30 Mar 2022 01:45:49 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm-dev clang g++ 		make 		openldap-dev 		openssl-dev 		perl-dev 		perl-ipc-run 		perl-utils 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-krb5 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 		zstd 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Wed, 30 Mar 2022 01:45:52 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample
# Wed, 30 Mar 2022 01:45:53 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Wed, 30 Mar 2022 01:45:53 GMT
ENV PGDATA=/var/lib/postgresql/data
# Wed, 30 Mar 2022 01:45:53 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Wed, 30 Mar 2022 01:45:54 GMT
VOLUME [/var/lib/postgresql/data]
# Wed, 30 Mar 2022 01:45:54 GMT
COPY file:e8928645623137de410cce68a2aa3b22f07a64e6391025598a60f3e461c606a3 in /usr/local/bin/ 
# Wed, 30 Mar 2022 01:45:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 30 Mar 2022 01:45:54 GMT
STOPSIGNAL SIGINT
# Wed, 30 Mar 2022 01:45:54 GMT
EXPOSE 5432
# Wed, 30 Mar 2022 01:45:54 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:2c33ece150b7a4954636e49b807bdf240c422de7a78f45728d2fcdb7c96d14a3`  
		Last Modified: Tue, 29 Mar 2022 00:44:03 GMT  
		Size: 2.6 MB (2600441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a977e9a14327d2f9d58d48da2e6b40ecf90262550e09f1807463da67e769ee6e`  
		Last Modified: Wed, 30 Mar 2022 02:02:15 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c461439424786a4630870245f5df1cfc7bc047d0e9637fb1daf72f4036aa17e`  
		Last Modified: Wed, 30 Mar 2022 02:02:15 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1022708dbb4a19eb1da9823edb6148c92b4d525d810f2bc157df684a4adf60d6`  
		Last Modified: Wed, 30 Mar 2022 02:15:30 GMT  
		Size: 77.6 MB (77635183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a96650f0c8c2591b8a88c8de0687b850295200901040d15fcf4601bc0fd8b68d`  
		Last Modified: Wed, 30 Mar 2022 02:15:26 GMT  
		Size: 8.0 KB (7992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c876ff7fe7749e45c874184b777abf53789f3d0b0fda6fb0aec0467c887bebc0`  
		Last Modified: Wed, 30 Mar 2022 02:15:21 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18222ecbe682e1f2e0eb0a1504c6ab28266ffcfbdc3052e85f8b649c2626d87c`  
		Last Modified: Wed, 30 Mar 2022 02:15:26 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ccbc46181eee6d16c01adf3bfdc1905883c5b0f7e598f36f3056272ba3af5ea`  
		Last Modified: Wed, 30 Mar 2022 02:15:21 GMT  
		Size: 4.7 KB (4702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
