## `postgres:12-alpine`

```console
$ docker pull postgres@sha256:62747237d799896f5b00b28f0e97e91396f938571090ded2416ade833a9b9d44
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
$ docker pull postgres@sha256:045d92032908a2ecf58e7ef97332ba00d3d7a7920cc30ab3eb22e50809c96e44
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.1 MB (81124473 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7df59d7559417b0916d4716d43a3c6035182f28e533d0e35cdd4406b5aaff4b7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Wed, 24 Nov 2021 20:19:40 GMT
ADD file:9233f6f2237d79659a9521f7e390df217cec49f1a8aa3a12147bbca1956acdb9 in / 
# Wed, 24 Nov 2021 20:19:40 GMT
CMD ["/bin/sh"]
# Tue, 30 Nov 2021 04:59:34 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Tue, 30 Nov 2021 04:59:34 GMT
ENV LANG=en_US.utf8
# Tue, 30 Nov 2021 04:59:35 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 30 Nov 2021 05:17:44 GMT
ENV PG_MAJOR=12
# Sat, 12 Feb 2022 00:44:04 GMT
ENV PG_VERSION=12.10
# Sat, 12 Feb 2022 00:44:05 GMT
ENV PG_SHA256=83dd192e6034951192b9a86dc19cf3717a8b82120e2f11a0a36723c820d2b257
# Tue, 08 Mar 2022 19:53:08 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm-dev clang g++ 		make 		openldap-dev 		openssl-dev 		perl-dev 		perl-ipc-run 		perl-utils 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		zstd 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-krb5 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Tue, 08 Mar 2022 19:53:09 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample
# Tue, 08 Mar 2022 19:53:10 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 08 Mar 2022 19:53:10 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 08 Mar 2022 19:53:11 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 08 Mar 2022 19:53:11 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 08 Mar 2022 19:53:11 GMT
COPY file:e8928645623137de410cce68a2aa3b22f07a64e6391025598a60f3e461c606a3 in /usr/local/bin/ 
# Tue, 08 Mar 2022 19:53:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 08 Mar 2022 19:53:11 GMT
STOPSIGNAL SIGINT
# Tue, 08 Mar 2022 19:53:11 GMT
EXPOSE 5432
# Tue, 08 Mar 2022 19:53:11 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:59bf1c3509f33515622619af21ed55bbe26d24913cedbca106468a5fb37a50c3`  
		Last Modified: Wed, 24 Nov 2021 20:20:05 GMT  
		Size: 2.8 MB (2818413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c50e01d57241cf7ef93a91060f5eb0b895a4b443f20dc1ce5e77d441184a6dc2`  
		Last Modified: Tue, 30 Nov 2021 05:48:55 GMT  
		Size: 1.3 KB (1279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0646b0f1eadaf0cd3fdb4c4490a69c4c7aed9b7ae10b24eb9005c59aa0b6e57`  
		Last Modified: Tue, 30 Nov 2021 05:48:55 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dbee45775c73a9c1d94c3d8a8e1a66af92d493c15664fd729b5b97fed9ee095`  
		Last Modified: Tue, 08 Mar 2022 20:09:44 GMT  
		Size: 78.3 MB (78290887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2932c92dbef1148d8ae90b3b81e9569399d67455eff312b80fca0ba03622f24f`  
		Last Modified: Tue, 08 Mar 2022 20:09:30 GMT  
		Size: 8.7 KB (8692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dadbb4cc7169aec30ade3d05948f0ceb87b1741bc2ae893d7b5f333b00b44c0e`  
		Last Modified: Tue, 08 Mar 2022 20:09:30 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:642e4d09e075b6c14545087a5256cb4d4af895d5c442886bb9816cf771453524`  
		Last Modified: Tue, 08 Mar 2022 20:09:30 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c73c0e429d659ea70cb71dbc93bed068046b8aff512c581e42e828af1579ebe4`  
		Last Modified: Tue, 08 Mar 2022 20:09:30 GMT  
		Size: 4.7 KB (4697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:12-alpine` - linux; arm variant v6

```console
$ docker pull postgres@sha256:ff0bbf7ad0b8d22896cf4fbfe2ea8d3dad54f8d968b4c0a2e477e213f6971c18
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.7 MB (77686650 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b43a863885c7d17b06f11429fe4e36b13196dfcadd96c760bde92f1e3d4f9a6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 17 Mar 2022 02:26:45 GMT
ADD file:9c8618405ef54d562132919ffe49c862d014b402e0e4813b87bf01574fa04c0e in / 
# Thu, 17 Mar 2022 02:26:45 GMT
CMD ["/bin/sh"]
# Thu, 17 Mar 2022 09:33:37 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 17 Mar 2022 09:33:37 GMT
ENV LANG=en_US.utf8
# Thu, 17 Mar 2022 09:33:38 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 17 Mar 2022 09:44:38 GMT
ENV PG_MAJOR=12
# Thu, 17 Mar 2022 09:44:38 GMT
ENV PG_VERSION=12.10
# Thu, 17 Mar 2022 09:44:38 GMT
ENV PG_SHA256=83dd192e6034951192b9a86dc19cf3717a8b82120e2f11a0a36723c820d2b257
# Thu, 17 Mar 2022 09:49:33 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm-dev clang g++ 		make 		openldap-dev 		openssl-dev 		perl-dev 		perl-ipc-run 		perl-utils 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		zstd 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-krb5 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Thu, 17 Mar 2022 09:49:36 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample
# Thu, 17 Mar 2022 09:49:37 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 17 Mar 2022 09:49:37 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 17 Mar 2022 09:49:39 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 17 Mar 2022 09:49:39 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 17 Mar 2022 09:49:40 GMT
COPY file:e8928645623137de410cce68a2aa3b22f07a64e6391025598a60f3e461c606a3 in /usr/local/bin/ 
# Thu, 17 Mar 2022 09:49:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Mar 2022 09:49:41 GMT
STOPSIGNAL SIGINT
# Thu, 17 Mar 2022 09:49:41 GMT
EXPOSE 5432
# Thu, 17 Mar 2022 09:49:42 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:787f016efa9bc7812361be134f731e845b97fba19169cf3615e7048c0412380e`  
		Last Modified: Thu, 17 Mar 2022 02:28:24 GMT  
		Size: 2.6 MB (2624973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf8357a39915fb976ee53735630d407cf3039a8804160e32ecd63d7206dd0e49`  
		Last Modified: Thu, 17 Mar 2022 10:00:50 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d68a50d25506682f9d05b7bf766ef5cf0bddb6785e086d10c03f83e050fea12b`  
		Last Modified: Thu, 17 Mar 2022 10:00:50 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edc8e9e0a03b5a4dbf4295bd4e4bd2294d5abe3f6ba4ffa246efde0746b9c6ef`  
		Last Modified: Thu, 17 Mar 2022 10:03:49 GMT  
		Size: 75.0 MB (75046496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f2fb4191937bdfdd4d9bf03c17a98db038176089672e8a4382e690434154188`  
		Last Modified: Thu, 17 Mar 2022 10:03:04 GMT  
		Size: 8.7 KB (8692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73b8428508ba99ff432ed5821e9f8dc4c109548e13ef30011babc4ae9988a2b3`  
		Last Modified: Thu, 17 Mar 2022 10:03:04 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acb6e228765742d1aaff6aea96b1306a21e7034dc7717dfe32ae67a1aad2f18d`  
		Last Modified: Thu, 17 Mar 2022 10:03:04 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b861f4759b9be1295e97c330daa710caa72f7c37edf1fbc5c921efe898dc7cf`  
		Last Modified: Thu, 17 Mar 2022 10:03:05 GMT  
		Size: 4.7 KB (4700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:12-alpine` - linux; arm variant v7

```console
$ docker pull postgres@sha256:d9dcfa8bcfcc70e3ea568020ac0aa377b80828838c7a652ad1c0d90ae228dce4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.3 MB (74275902 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e5822fc0484924640fce68b3b4b34bd84294d40e26b2398c1b69a7863f6993a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Wed, 24 Nov 2021 21:42:11 GMT
ADD file:ca436da5b0bfc9c0e2fc685533c6628918000c8fff109fe9a8da625b9a798002 in / 
# Wed, 24 Nov 2021 21:42:11 GMT
CMD ["/bin/sh"]
# Tue, 30 Nov 2021 07:45:15 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Tue, 30 Nov 2021 07:45:15 GMT
ENV LANG=en_US.utf8
# Tue, 30 Nov 2021 07:45:17 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 30 Nov 2021 09:00:39 GMT
ENV PG_MAJOR=12
# Sat, 12 Feb 2022 00:58:42 GMT
ENV PG_VERSION=12.10
# Sat, 12 Feb 2022 00:58:43 GMT
ENV PG_SHA256=83dd192e6034951192b9a86dc19cf3717a8b82120e2f11a0a36723c820d2b257
# Tue, 08 Mar 2022 22:08:09 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm-dev clang g++ 		make 		openldap-dev 		openssl-dev 		perl-dev 		perl-ipc-run 		perl-utils 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		zstd 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-krb5 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Tue, 08 Mar 2022 22:08:11 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample
# Tue, 08 Mar 2022 22:08:12 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 08 Mar 2022 22:08:13 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 08 Mar 2022 22:08:14 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 08 Mar 2022 22:08:15 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 08 Mar 2022 22:08:15 GMT
COPY file:e8928645623137de410cce68a2aa3b22f07a64e6391025598a60f3e461c606a3 in /usr/local/bin/ 
# Tue, 08 Mar 2022 22:08:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 08 Mar 2022 22:08:16 GMT
STOPSIGNAL SIGINT
# Tue, 08 Mar 2022 22:08:17 GMT
EXPOSE 5432
# Tue, 08 Mar 2022 22:08:17 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:5480d2ca1740c20ce17652e01ed2265cdc914458acd41256a2b1ccff28f2762c`  
		Last Modified: Wed, 24 Nov 2021 21:43:40 GMT  
		Size: 2.4 MB (2434764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8f681d006162b865bd7dca8476d129c7fa1193b246ad8a598d27eb28769a6ac`  
		Last Modified: Tue, 30 Nov 2021 12:10:30 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c74eb577cd41aefd27e490e1cbe04812996920ee2af42f358c659d1bb8a40230`  
		Last Modified: Tue, 30 Nov 2021 12:10:30 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f55ea977a63d69ac61f786eaa8e90606ca5d221c88fa65a8039b498c56900d29`  
		Last Modified: Wed, 09 Mar 2022 00:07:40 GMT  
		Size: 71.8 MB (71825955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a85b61bee2b35be3ccfaa86301337f6806cab5f5f2a98c3a6c6b2b0ab85c1da3`  
		Last Modified: Wed, 09 Mar 2022 00:07:03 GMT  
		Size: 8.7 KB (8696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78411dbbb7faad1cec6293d013b0664063887ac9b54cc8f3d2ce6c5ba47caceb`  
		Last Modified: Wed, 09 Mar 2022 00:07:03 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:396cb6d6344c9bec0a7dc02e9f6b3a131c18f4a3b72bddaf2f4bc5099cb8de7a`  
		Last Modified: Wed, 09 Mar 2022 00:07:03 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3771ac1dfdb5db677ee60c4059424f3624ddcfcf254e4a3b24af89f9ffc964f`  
		Last Modified: Wed, 09 Mar 2022 00:07:03 GMT  
		Size: 4.7 KB (4701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:12-alpine` - linux; arm64 variant v8

```console
$ docker pull postgres@sha256:407b2d52058ff7d92b6c1ed17cd6539c4eacf19e0b1befe7be82650a89cb4b92
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **79.9 MB (79866388 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:98303717e8b31270bf379db105379e920167ffef55b7cca4da0d852b6be09aa4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Wed, 24 Nov 2021 20:39:20 GMT
ADD file:df53811312284306901fdaaff0a357a4bf40d631e662fe9ce6d342442e494b6c in / 
# Wed, 24 Nov 2021 20:39:20 GMT
CMD ["/bin/sh"]
# Tue, 30 Nov 2021 04:27:18 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Tue, 30 Nov 2021 04:27:19 GMT
ENV LANG=en_US.utf8
# Tue, 30 Nov 2021 04:27:20 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 30 Nov 2021 04:36:07 GMT
ENV PG_MAJOR=12
# Sat, 12 Feb 2022 00:57:27 GMT
ENV PG_VERSION=12.10
# Sat, 12 Feb 2022 00:57:28 GMT
ENV PG_SHA256=83dd192e6034951192b9a86dc19cf3717a8b82120e2f11a0a36723c820d2b257
# Tue, 08 Mar 2022 20:06:50 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm-dev clang g++ 		make 		openldap-dev 		openssl-dev 		perl-dev 		perl-ipc-run 		perl-utils 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		zstd 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-krb5 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Tue, 08 Mar 2022 20:06:50 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample
# Tue, 08 Mar 2022 20:06:51 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 08 Mar 2022 20:06:52 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 08 Mar 2022 20:06:53 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 08 Mar 2022 20:06:54 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 08 Mar 2022 20:06:56 GMT
COPY file:e8928645623137de410cce68a2aa3b22f07a64e6391025598a60f3e461c606a3 in /usr/local/bin/ 
# Tue, 08 Mar 2022 20:06:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 08 Mar 2022 20:06:57 GMT
STOPSIGNAL SIGINT
# Tue, 08 Mar 2022 20:06:58 GMT
EXPOSE 5432
# Tue, 08 Mar 2022 20:06:59 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:9b3977197b4f2147bdd31e1271f811319dcd5c2fc595f14e81f5351ab6275b99`  
		Last Modified: Wed, 24 Nov 2021 20:39:59 GMT  
		Size: 2.7 MB (2715434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:995a68b04f2b01f2160f500ef732a967a427af5da712fac9029eeecbc80af73d`  
		Last Modified: Tue, 30 Nov 2021 05:22:34 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8a8bdf2ee5e8b95fdba44140b8595c955b8639595bcf5c0f15841330176d8e5`  
		Last Modified: Tue, 30 Nov 2021 05:22:35 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ccb985ae41b688cb4a6da77ab6c8189ed539af4ef839fd7648054bef8f9bc0b`  
		Last Modified: Tue, 08 Mar 2022 20:38:42 GMT  
		Size: 77.1 MB (77135889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c4ff93a6cfddb6e9e1527c0bec08b7775e4f3e52733b42d3e07ee6deebb1688`  
		Last Modified: Tue, 08 Mar 2022 20:38:28 GMT  
		Size: 8.7 KB (8695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16222f12c27bf8d570bca6f1915177ac75bf301a98673bbb9f82f3caaf82a32a`  
		Last Modified: Tue, 08 Mar 2022 20:38:28 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:665170a351ea1145db062de6bdae68a5d5db75b021b54fcd47f06a44794b3141`  
		Last Modified: Tue, 08 Mar 2022 20:38:28 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9789fa7f4eb7e9fb1f928a55cbdd45ef8a1799681000f2c096f273bde375514`  
		Last Modified: Tue, 08 Mar 2022 20:38:29 GMT  
		Size: 4.7 KB (4695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:12-alpine` - linux; 386

```console
$ docker pull postgres@sha256:3e6c0642400c74bd55e8d6efb07e8fe493e5a340148a9fbe25fd5ffa33ae53bd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **86.0 MB (85955377 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:88bcb461510be7a9b341020e04988a922c6f8ad219b113e1809358cb19756007`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Wed, 24 Nov 2021 20:53:48 GMT
ADD file:b9a17131c440053f2f67e127b447645f25fd7de2d6caca42f569cafab6291855 in / 
# Wed, 24 Nov 2021 20:53:48 GMT
CMD ["/bin/sh"]
# Tue, 30 Nov 2021 02:41:28 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Tue, 30 Nov 2021 02:41:28 GMT
ENV LANG=en_US.utf8
# Tue, 30 Nov 2021 02:41:29 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 30 Nov 2021 03:32:23 GMT
ENV PG_MAJOR=12
# Sat, 12 Feb 2022 00:05:11 GMT
ENV PG_VERSION=12.10
# Sat, 12 Feb 2022 00:05:11 GMT
ENV PG_SHA256=83dd192e6034951192b9a86dc19cf3717a8b82120e2f11a0a36723c820d2b257
# Tue, 08 Mar 2022 20:41:10 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm-dev clang g++ 		make 		openldap-dev 		openssl-dev 		perl-dev 		perl-ipc-run 		perl-utils 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		zstd 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-krb5 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Tue, 08 Mar 2022 20:41:11 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample
# Tue, 08 Mar 2022 20:41:12 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 08 Mar 2022 20:41:12 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 08 Mar 2022 20:41:12 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 08 Mar 2022 20:41:13 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 08 Mar 2022 20:41:13 GMT
COPY file:e8928645623137de410cce68a2aa3b22f07a64e6391025598a60f3e461c606a3 in /usr/local/bin/ 
# Tue, 08 Mar 2022 20:41:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 08 Mar 2022 20:41:13 GMT
STOPSIGNAL SIGINT
# Tue, 08 Mar 2022 20:41:13 GMT
EXPOSE 5432
# Tue, 08 Mar 2022 20:41:13 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:e6889e0d66307a4b916fc844f2dcbc03245c63bc4189dd3e88126d9dcf2f9231`  
		Last Modified: Wed, 24 Nov 2021 20:54:48 GMT  
		Size: 2.8 MB (2827117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3af56146d51f459d9baa843fcf88ab0b80c1c9de99248bc2163f19197ba95d05`  
		Last Modified: Tue, 30 Nov 2021 04:43:41 GMT  
		Size: 1.3 KB (1279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87a14412d0e45405abe51e591c8467d465e5f91db0600bf8b9120d9c6f15217c`  
		Last Modified: Tue, 30 Nov 2021 04:43:41 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3f7f98482b149a4f117bbc79774a9d9aafddab8c46a0420b754763101c9e2d7`  
		Last Modified: Tue, 08 Mar 2022 21:21:07 GMT  
		Size: 83.1 MB (83113087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:036dd1d064f39dfbd2083fed5a0d5ae1e984eade98582a581c4406d0fb05ecde`  
		Last Modified: Tue, 08 Mar 2022 21:20:53 GMT  
		Size: 8.7 KB (8693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8502287f851a59874a0d010b14815ec8f65ce671cbee3a07f68c90859c719db`  
		Last Modified: Tue, 08 Mar 2022 21:20:53 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ae9f9fa248bf1815dd38b41c12974e51b2ce1fe789e451796c03c3de9e1adf8`  
		Last Modified: Tue, 08 Mar 2022 21:20:53 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c924cb50a6452dd6b44f4ce73cbb16102c327b70c92f385a9f7a7884993d14bd`  
		Last Modified: Tue, 08 Mar 2022 21:20:53 GMT  
		Size: 4.7 KB (4698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:12-alpine` - linux; ppc64le

```console
$ docker pull postgres@sha256:b432cbf90682a127d728476520ec3bed9253198215f81d3bbd30a9c1e1d7f6f1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **86.3 MB (86296971 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa827e10b5210644e7e3c89d0d3ec993a9b5aa6e59f5643a68dbe40168842579`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Wed, 24 Nov 2021 20:20:16 GMT
ADD file:57115dca2eb707f46b6301e75174e6aa316fb02ac28643b91429b75be51bd8c8 in / 
# Wed, 24 Nov 2021 20:20:20 GMT
CMD ["/bin/sh"]
# Tue, 30 Nov 2021 04:26:49 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Tue, 30 Nov 2021 04:26:53 GMT
ENV LANG=en_US.utf8
# Tue, 30 Nov 2021 04:27:03 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 30 Nov 2021 04:43:10 GMT
ENV PG_MAJOR=12
# Sat, 12 Feb 2022 00:18:18 GMT
ENV PG_VERSION=12.10
# Sat, 12 Feb 2022 00:18:20 GMT
ENV PG_SHA256=83dd192e6034951192b9a86dc19cf3717a8b82120e2f11a0a36723c820d2b257
# Tue, 08 Mar 2022 20:48:05 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm-dev clang g++ 		make 		openldap-dev 		openssl-dev 		perl-dev 		perl-ipc-run 		perl-utils 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		zstd 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-krb5 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Tue, 08 Mar 2022 20:48:16 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample
# Tue, 08 Mar 2022 20:48:28 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 08 Mar 2022 20:48:29 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 08 Mar 2022 20:48:40 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 08 Mar 2022 20:48:43 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 08 Mar 2022 20:48:44 GMT
COPY file:e8928645623137de410cce68a2aa3b22f07a64e6391025598a60f3e461c606a3 in /usr/local/bin/ 
# Tue, 08 Mar 2022 20:48:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 08 Mar 2022 20:48:48 GMT
STOPSIGNAL SIGINT
# Tue, 08 Mar 2022 20:48:51 GMT
EXPOSE 5432
# Tue, 08 Mar 2022 20:48:54 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:159b5dcb1717c815c76ff5ea1db730e18e8609c9090238e43282856db9e71f47`  
		Last Modified: Wed, 24 Nov 2021 20:21:14 GMT  
		Size: 2.8 MB (2814780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f21143ce0a44ab602b12471d2a1cf95c5dcbc9d805bd8ede00e2766f24d295b5`  
		Last Modified: Tue, 30 Nov 2021 05:10:51 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5c45529781f9e932a9022851fca78ba53022920657aa14e0479b195cac40189`  
		Last Modified: Tue, 30 Nov 2021 05:10:51 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5aaed242006ee1c71626defa5d78433fd85d804277a83b1c355f7d6ff128a8b`  
		Last Modified: Tue, 08 Mar 2022 21:11:45 GMT  
		Size: 83.5 MB (83467015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12cf3559c0cb459c33f67a8e74364845c5e6227130218dfd3bfa0fb87e1d0f78`  
		Last Modified: Tue, 08 Mar 2022 21:11:31 GMT  
		Size: 8.7 KB (8689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:758974d95f6dc32aaa2a4cafd137e18a2cb3c601eb50d5062d79bd712172269f`  
		Last Modified: Tue, 08 Mar 2022 21:11:31 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f44821bd679b64e876dba4646e4f9797525ef688a789b82d77ee8ea80ccd92e`  
		Last Modified: Tue, 08 Mar 2022 21:11:31 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b215b4039b7a5e401731a8ca5adfccc381116744e0fa88ac742df95796155b0`  
		Last Modified: Tue, 08 Mar 2022 21:11:31 GMT  
		Size: 4.7 KB (4699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:12-alpine` - linux; s390x

```console
$ docker pull postgres@sha256:0d08a54768ca3f018ffae4eb4250028bce57ca550add0db1ec13656465dced30
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **82.1 MB (82144864 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c7949ee92d04289fbc30db5ac184125c1f9f394e90922b6019efafe71993b0b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Wed, 24 Nov 2021 20:41:23 GMT
ADD file:cd24c711a2ef431b3ff94f9a02bfc42f159bc60de1d0eceecafea4e8af02441d in / 
# Wed, 24 Nov 2021 20:41:23 GMT
CMD ["/bin/sh"]
# Tue, 30 Nov 2021 08:50:09 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Tue, 30 Nov 2021 08:50:09 GMT
ENV LANG=en_US.utf8
# Tue, 30 Nov 2021 08:50:10 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 30 Nov 2021 09:12:05 GMT
ENV PG_MAJOR=12
# Sat, 12 Feb 2022 00:10:11 GMT
ENV PG_VERSION=12.10
# Sat, 12 Feb 2022 00:10:11 GMT
ENV PG_SHA256=83dd192e6034951192b9a86dc19cf3717a8b82120e2f11a0a36723c820d2b257
# Tue, 08 Mar 2022 20:22:27 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm-dev clang g++ 		make 		openldap-dev 		openssl-dev 		perl-dev 		perl-ipc-run 		perl-utils 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		zstd 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-krb5 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Tue, 08 Mar 2022 20:22:30 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample
# Tue, 08 Mar 2022 20:22:31 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 08 Mar 2022 20:22:31 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 08 Mar 2022 20:22:31 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 08 Mar 2022 20:22:32 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 08 Mar 2022 20:22:32 GMT
COPY file:e8928645623137de410cce68a2aa3b22f07a64e6391025598a60f3e461c606a3 in /usr/local/bin/ 
# Tue, 08 Mar 2022 20:22:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 08 Mar 2022 20:22:32 GMT
STOPSIGNAL SIGINT
# Tue, 08 Mar 2022 20:22:32 GMT
EXPOSE 5432
# Tue, 08 Mar 2022 20:22:32 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:d6baca485f3d0f7c77221be60fbef5db014a5ef9d8f53db4a310c947c690d189`  
		Last Modified: Wed, 24 Nov 2021 20:42:15 GMT  
		Size: 2.6 MB (2605944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96844042cfb587d09e525bf6890e267412ad5971e27ece4faa02e82f6fda3c87`  
		Last Modified: Tue, 30 Nov 2021 09:46:44 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:826ee6a78ec06ec30a73acc9c0f2337f744b77da2931a6e0c1d3efb35d76cfe6`  
		Last Modified: Tue, 30 Nov 2021 09:46:44 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5b3a65415921b3d90103a6670fd9d22ffd06a61977aa7cee14a796c8e2ff69e`  
		Last Modified: Tue, 08 Mar 2022 20:46:05 GMT  
		Size: 79.5 MB (79523740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38829c0ce8434a9068b99c94601fa39c1243d2bad27f9915a0503f3a67608efd`  
		Last Modified: Tue, 08 Mar 2022 20:45:56 GMT  
		Size: 8.7 KB (8697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c54077196f50c2a012505bd1ccee3eb71a6a0dd2e6ebcf34c93ca4bdaceff73b`  
		Last Modified: Tue, 08 Mar 2022 20:45:56 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b8ef7a1de21e344e4de8b19e8362e1ba823f312e20851d54034f1dfaf8ee617`  
		Last Modified: Tue, 08 Mar 2022 20:45:56 GMT  
		Size: 192.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aeb8d1e90e7f823ce3de22aee622741785054da5f8d5b3debc61283ae5750cc`  
		Last Modified: Tue, 08 Mar 2022 20:45:56 GMT  
		Size: 4.7 KB (4699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
