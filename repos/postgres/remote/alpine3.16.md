## `postgres:alpine3.16`

```console
$ docker pull postgres@sha256:9f7112adc1aa44c0129fd4535a0ccf237dcabadbcbd3cf3c2bf5dbf551ddd788
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

### `postgres:alpine3.16` - linux; amd64

```console
$ docker pull postgres@sha256:7d6403121b12c9d29c13c9873bc0f76da8ff51f6c89fae10b99dc890807e27ae
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.7 MB (84683553 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:41cd24e8c51bfe2a56fbe1577c41f5160692de3092d7ba0f2e0a622c57724fc3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Mon, 18 Jul 2022 21:00:15 GMT
ADD file:a2648378045615c3785c752423b1afc8dc1c2b213393344f4d0ca17e7255c1cb in / 
# Mon, 18 Jul 2022 21:00:15 GMT
CMD ["/bin/sh"]
# Tue, 19 Jul 2022 01:37:18 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Tue, 19 Jul 2022 01:37:18 GMT
ENV LANG=en_US.utf8
# Tue, 19 Jul 2022 01:37:19 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 19 Jul 2022 01:41:13 GMT
ENV PG_MAJOR=14
# Tue, 19 Jul 2022 01:41:13 GMT
ENV PG_VERSION=14.4
# Tue, 19 Jul 2022 01:41:14 GMT
ENV PG_SHA256=c23b6237c5231c791511bdc79098617d6852e9e3bdf360efd8b5d15a1a3d8f6a
# Tue, 19 Jul 2022 01:44:39 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm-dev clang g++ 		make 		openldap-dev 		openssl-dev 		perl-dev 		perl-ipc-run 		perl-utils 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		icu-dev 		lz4-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-krb5 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 		--with-lz4 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 		zstd 		icu-data-full 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Tue, 19 Jul 2022 01:44:40 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample
# Tue, 19 Jul 2022 01:44:41 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 19 Jul 2022 01:44:41 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 19 Jul 2022 01:44:41 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 19 Jul 2022 01:44:41 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 19 Jul 2022 01:44:42 GMT
COPY file:232dce6cf487afb0c0cc43d38932ff29614a74b57cd04557dc7398e6d2b93b8f in /usr/local/bin/ 
# Tue, 19 Jul 2022 01:44:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 19 Jul 2022 01:44:42 GMT
STOPSIGNAL SIGINT
# Tue, 19 Jul 2022 01:44:42 GMT
EXPOSE 5432
# Tue, 19 Jul 2022 01:44:42 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:530afca65e2ea04227630ae746e0c85b2bd1a179379cbf2b6501b49c4cab2ccc`  
		Last Modified: Mon, 18 Jul 2022 19:09:35 GMT  
		Size: 2.8 MB (2798806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:915bf02ec4105a810e064257cd9ce9cbf90be2ec069bf0f87d12f98038d07c56`  
		Last Modified: Tue, 19 Jul 2022 01:58:47 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b026a0cf3c97e00c74281e123e212ce0517eee48fbd9a1086027c4684f6f5517`  
		Last Modified: Tue, 19 Jul 2022 01:58:46 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88659e2107f6c19018c4e187da12c1d25804ea415012db2800349a24303c3f58`  
		Last Modified: Tue, 19 Jul 2022 01:59:19 GMT  
		Size: 81.9 MB (81869047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33960a1e9871a67fd4cdc90215bb1e3002ec7fac9e5ffa3d9729f1632f659f91`  
		Last Modified: Tue, 19 Jul 2022 01:59:07 GMT  
		Size: 9.2 KB (9204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9bbc907277f07d68b85d7eab8d131447831f84eaac4d1bf2421ff2e6139ea7c`  
		Last Modified: Tue, 19 Jul 2022 01:59:07 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e545c6230ec7e1d72b3d7fdfae81ebfa9d1ee7ab1fb165b956202376cafe277`  
		Last Modified: Tue, 19 Jul 2022 01:59:07 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba5428d6e942832c77d8b941f2a66f721abc27bb010a93d9a60a933df9e51dc4`  
		Last Modified: Tue, 19 Jul 2022 01:59:07 GMT  
		Size: 4.7 KB (4704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:alpine3.16` - linux; arm variant v6

```console
$ docker pull postgres@sha256:56d258a75a7862cb319cfd52cc3bf174f78b9f4d242cfdd98cfbe78c1a506ca6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **82.8 MB (82779681 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba42fabb5665ba1fc8b66d76e712164047f5115a59208c01facc932ca6986a8d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Mon, 18 Jul 2022 19:49:37 GMT
ADD file:7a20333469e71664904a0cb8f61613250f2bd092b4a27bfa7bbae1dc7e21b7ed in / 
# Mon, 18 Jul 2022 19:49:37 GMT
CMD ["/bin/sh"]
# Mon, 18 Jul 2022 21:06:36 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Mon, 18 Jul 2022 21:06:36 GMT
ENV LANG=en_US.utf8
# Mon, 18 Jul 2022 21:06:38 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Mon, 18 Jul 2022 21:13:22 GMT
ENV PG_MAJOR=14
# Mon, 18 Jul 2022 21:13:22 GMT
ENV PG_VERSION=14.4
# Mon, 18 Jul 2022 21:13:23 GMT
ENV PG_SHA256=c23b6237c5231c791511bdc79098617d6852e9e3bdf360efd8b5d15a1a3d8f6a
# Mon, 18 Jul 2022 21:19:11 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm-dev clang g++ 		make 		openldap-dev 		openssl-dev 		perl-dev 		perl-ipc-run 		perl-utils 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		icu-dev 		lz4-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-krb5 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 		--with-lz4 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 		zstd 		icu-data-full 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Mon, 18 Jul 2022 21:19:13 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample
# Mon, 18 Jul 2022 21:19:14 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Mon, 18 Jul 2022 21:19:15 GMT
ENV PGDATA=/var/lib/postgresql/data
# Mon, 18 Jul 2022 21:19:16 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Mon, 18 Jul 2022 21:19:16 GMT
VOLUME [/var/lib/postgresql/data]
# Mon, 18 Jul 2022 21:19:17 GMT
COPY file:232dce6cf487afb0c0cc43d38932ff29614a74b57cd04557dc7398e6d2b93b8f in /usr/local/bin/ 
# Mon, 18 Jul 2022 21:19:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 18 Jul 2022 21:19:18 GMT
STOPSIGNAL SIGINT
# Mon, 18 Jul 2022 21:19:18 GMT
EXPOSE 5432
# Mon, 18 Jul 2022 21:19:19 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:b7885075fcd06a866d12dfd56eb704045eaadbd22dc03a224cd98715be566677`  
		Last Modified: Mon, 18 Jul 2022 19:08:42 GMT  
		Size: 2.6 MB (2606431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33ee135ac0bb04d40f0640b49a624bd7ee2aefe8bfbfc103e187bc2ec33604b8`  
		Last Modified: Mon, 18 Jul 2022 21:44:07 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21f9e567f61e29fde27226359cb09450d6888364eedb70b1144acc08642e6ade`  
		Last Modified: Mon, 18 Jul 2022 21:44:07 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3ab543b24bb036ab693847b178b8ac49a86ca0c46cf043f5125e473cb054c9e`  
		Last Modified: Mon, 18 Jul 2022 21:45:51 GMT  
		Size: 80.2 MB (80157550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7714019fc6f25e85b1bcce6fe19b344aa5c200dd2c223434dce112d7ac62c778`  
		Last Modified: Mon, 18 Jul 2022 21:45:04 GMT  
		Size: 9.2 KB (9204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c9aaf9a842af3493df009b39d0dbd1703bfb1d564e4f9ec3f00253fe1f7c18e`  
		Last Modified: Mon, 18 Jul 2022 21:45:04 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d60d60f7f3a4c5ae5af3478752f58a20ff3d65fd3aaf59011ea4591f17f6809`  
		Last Modified: Mon, 18 Jul 2022 21:45:04 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9f0ae825c0023c72b789af79a5d0c080acfb555ce21e70bd10c57089a26ea30`  
		Last Modified: Mon, 18 Jul 2022 21:45:04 GMT  
		Size: 4.7 KB (4706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:alpine3.16` - linux; arm variant v7

```console
$ docker pull postgres@sha256:ba80799d6b68f46d92de059b19cac927d18ea063fbc48e017860601a27797355
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.9 MB (77895947 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:491e25db1f0560af6f6a74b72a4895de8a0f6ed20acf388ae93607442bbb80f2`
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
# Wed, 25 May 2022 20:26:17 GMT
ENV PG_MAJOR=14
# Wed, 22 Jun 2022 00:34:00 GMT
ENV PG_VERSION=14.4
# Wed, 22 Jun 2022 00:34:01 GMT
ENV PG_SHA256=c23b6237c5231c791511bdc79098617d6852e9e3bdf360efd8b5d15a1a3d8f6a
# Wed, 22 Jun 2022 00:39:38 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm-dev clang g++ 		make 		openldap-dev 		openssl-dev 		perl-dev 		perl-ipc-run 		perl-utils 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		icu-dev 		lz4-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-krb5 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 		--with-lz4 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 		zstd 		icu-data-full 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Wed, 22 Jun 2022 00:39:40 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample
# Wed, 22 Jun 2022 00:39:42 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Wed, 22 Jun 2022 00:39:42 GMT
ENV PGDATA=/var/lib/postgresql/data
# Wed, 22 Jun 2022 00:39:44 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Wed, 22 Jun 2022 00:39:44 GMT
VOLUME [/var/lib/postgresql/data]
# Wed, 22 Jun 2022 00:39:44 GMT
COPY file:232dce6cf487afb0c0cc43d38932ff29614a74b57cd04557dc7398e6d2b93b8f in /usr/local/bin/ 
# Wed, 22 Jun 2022 00:39:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 22 Jun 2022 00:39:45 GMT
STOPSIGNAL SIGINT
# Wed, 22 Jun 2022 00:39:46 GMT
EXPOSE 5432
# Wed, 22 Jun 2022 00:39:46 GMT
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
	-	`sha256:ccac1bcc88876fb9421f37f653be47466d667c902b56cefeb082c9a48dadb273`  
		Last Modified: Wed, 22 Jun 2022 00:48:45 GMT  
		Size: 75.5 MB (75468600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c291aa3d92577753a78e06574217605a42e6864cf247d0c431d138a974a552de`  
		Last Modified: Wed, 22 Jun 2022 00:48:05 GMT  
		Size: 9.2 KB (9204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdf64d30d3289d10f31bd5cbf8ef90a3a1e9c13b5460aff04bb870e55a23b0d4`  
		Last Modified: Wed, 22 Jun 2022 00:48:05 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f09695acd9a33cc5d1e4ace1505caca2424afbccce0fb4b834de7b2e06f70f0`  
		Last Modified: Wed, 22 Jun 2022 00:48:05 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b293f610eaeeb539249f7fba0c5b2bb74b676c58479f587d43729a455e0c798c`  
		Last Modified: Wed, 22 Jun 2022 00:48:05 GMT  
		Size: 4.7 KB (4703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:alpine3.16` - linux; arm64 variant v8

```console
$ docker pull postgres@sha256:033ba1b6dfd128e81008e98229b1b6d715352f13a14f3ae58539677b9cc79ef8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **83.5 MB (83524809 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:054113da34d97ccba36ed9c08e21d2f6e6dd7bf5950aae1e9981b96c3c56c71c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Mon, 18 Jul 2022 21:57:05 GMT
ADD file:9ccb70abba88b6de789b29f17770246f765ffbb072fe598580bfc29ce3213f1c in / 
# Mon, 18 Jul 2022 21:57:05 GMT
CMD ["/bin/sh"]
# Tue, 19 Jul 2022 01:26:38 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Tue, 19 Jul 2022 01:26:38 GMT
ENV LANG=en_US.utf8
# Tue, 19 Jul 2022 01:26:39 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 19 Jul 2022 01:30:40 GMT
ENV PG_MAJOR=14
# Tue, 19 Jul 2022 01:30:41 GMT
ENV PG_VERSION=14.4
# Tue, 19 Jul 2022 01:30:42 GMT
ENV PG_SHA256=c23b6237c5231c791511bdc79098617d6852e9e3bdf360efd8b5d15a1a3d8f6a
# Tue, 19 Jul 2022 01:34:03 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm-dev clang g++ 		make 		openldap-dev 		openssl-dev 		perl-dev 		perl-ipc-run 		perl-utils 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		icu-dev 		lz4-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-krb5 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 		--with-lz4 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 		zstd 		icu-data-full 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Tue, 19 Jul 2022 01:34:04 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample
# Tue, 19 Jul 2022 01:34:05 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 19 Jul 2022 01:34:06 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 19 Jul 2022 01:34:07 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 19 Jul 2022 01:34:08 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 19 Jul 2022 01:34:10 GMT
COPY file:232dce6cf487afb0c0cc43d38932ff29614a74b57cd04557dc7398e6d2b93b8f in /usr/local/bin/ 
# Tue, 19 Jul 2022 01:34:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 19 Jul 2022 01:34:11 GMT
STOPSIGNAL SIGINT
# Tue, 19 Jul 2022 01:34:12 GMT
EXPOSE 5432
# Tue, 19 Jul 2022 01:34:13 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:f97344484467e4c4ebb85aae724170073799295a3442c50ab532e249bd27b412`  
		Last Modified: Mon, 18 Jul 2022 19:08:29 GMT  
		Size: 2.7 MB (2694720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:204fa37ad79b6fbdaa6b71115fab75d702735b2da767ca79a34f9ae33d35e456`  
		Last Modified: Tue, 19 Jul 2022 01:49:22 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a550a0032f8399648b092e8dac43bb9b5ac5fd50d67cd74bfe0ad094ba2a535`  
		Last Modified: Tue, 19 Jul 2022 01:49:22 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb34ecb999918a9201680eaf8c70e6269e8c0d72fa05748ed276eace84fe76e3`  
		Last Modified: Tue, 19 Jul 2022 01:49:56 GMT  
		Size: 80.8 MB (80814513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9a2e68b08765d3a07190c21adfc150b2087aff7f3deada0a605d6e455025f92`  
		Last Modified: Tue, 19 Jul 2022 01:49:46 GMT  
		Size: 9.2 KB (9202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13dfed150d08c79c112befc24b7668800f0b4c5082871984779d6f824a8255f0`  
		Last Modified: Tue, 19 Jul 2022 01:49:46 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac01d50c1b9b4a340eb93f4f32028c3d16273851c63f4274e12bfb12a5c83171`  
		Last Modified: Tue, 19 Jul 2022 01:49:46 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5590d83d2d1740deaede85637af992e32009b5a0fdbcb63280c0a89feda1a37a`  
		Last Modified: Tue, 19 Jul 2022 01:49:46 GMT  
		Size: 4.7 KB (4704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:alpine3.16` - linux; 386

```console
$ docker pull postgres@sha256:74d434c2369e8b5385ac18a78b794e8e1e7556bec6c553041cc7395ee2db5fc7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **90.0 MB (89980358 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:53f3bd2ed51eb12fc15f38767f50e0a1b461555f21f633f2c85b4e8032d5cbce`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Mon, 18 Jul 2022 20:38:19 GMT
ADD file:be69b7550bf861d8fb12bdbe1edf3a0d2519a6a4da61bd04858b6258ffbf48a7 in / 
# Mon, 18 Jul 2022 20:38:19 GMT
CMD ["/bin/sh"]
# Mon, 18 Jul 2022 22:52:16 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Mon, 18 Jul 2022 22:52:17 GMT
ENV LANG=en_US.utf8
# Mon, 18 Jul 2022 22:52:18 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Mon, 18 Jul 2022 22:56:48 GMT
ENV PG_MAJOR=14
# Mon, 18 Jul 2022 22:56:49 GMT
ENV PG_VERSION=14.4
# Mon, 18 Jul 2022 22:56:50 GMT
ENV PG_SHA256=c23b6237c5231c791511bdc79098617d6852e9e3bdf360efd8b5d15a1a3d8f6a
# Mon, 18 Jul 2022 23:00:39 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm-dev clang g++ 		make 		openldap-dev 		openssl-dev 		perl-dev 		perl-ipc-run 		perl-utils 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		icu-dev 		lz4-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-krb5 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 		--with-lz4 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 		zstd 		icu-data-full 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Mon, 18 Jul 2022 23:00:39 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample
# Mon, 18 Jul 2022 23:00:40 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Mon, 18 Jul 2022 23:00:41 GMT
ENV PGDATA=/var/lib/postgresql/data
# Mon, 18 Jul 2022 23:00:42 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Mon, 18 Jul 2022 23:00:43 GMT
VOLUME [/var/lib/postgresql/data]
# Mon, 18 Jul 2022 23:00:45 GMT
COPY file:232dce6cf487afb0c0cc43d38932ff29614a74b57cd04557dc7398e6d2b93b8f in /usr/local/bin/ 
# Mon, 18 Jul 2022 23:00:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 18 Jul 2022 23:00:46 GMT
STOPSIGNAL SIGINT
# Mon, 18 Jul 2022 23:00:47 GMT
EXPOSE 5432
# Mon, 18 Jul 2022 23:00:48 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:5d7f927419794ebb7496ac38b0659686317b2d2fac7252a4a0d40d43d5fdd662`  
		Last Modified: Mon, 18 Jul 2022 19:09:22 GMT  
		Size: 2.8 MB (2802334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f036c9eaa88b40b78cc122e866baceacb64ada92934099e016b91314f8dbce0`  
		Last Modified: Mon, 18 Jul 2022 23:17:21 GMT  
		Size: 1.3 KB (1256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7db490d377bb031a749799fe3786fd2199b749c4c22e7aad3bf8feffdaea4ec`  
		Last Modified: Mon, 18 Jul 2022 23:17:21 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a9dbb26b5c8d648c24bb6c671781127a94d20fd282df790cb58dd1dbca1a4ce`  
		Last Modified: Mon, 18 Jul 2022 23:17:56 GMT  
		Size: 87.2 MB (87162447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c0024c87e79b4181b0384672e77e6d4a21012e181b44b6fbd0970466095e097`  
		Last Modified: Mon, 18 Jul 2022 23:17:45 GMT  
		Size: 9.2 KB (9203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11710c017a1f86f48c279a2e51b76633fbaf55e5da147366fda061ecf25d4227`  
		Last Modified: Mon, 18 Jul 2022 23:17:45 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fd727bbeddcae569c806bd50f409e57b2f5dbb954d09e4e123ac79a7d86ca7a`  
		Last Modified: Mon, 18 Jul 2022 23:17:45 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07b67696fdddb3a8b523585b7885d8125f634f2abff7ccd0430c20fb1837bff2`  
		Last Modified: Mon, 18 Jul 2022 23:17:45 GMT  
		Size: 4.7 KB (4705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:alpine3.16` - linux; ppc64le

```console
$ docker pull postgres@sha256:3e4b0b2526e743285f8d16bc90080210aa40def18244d64a7b4762457743afad
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **90.9 MB (90926182 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:04dec6547896817557a09c0075a51e30a6ea5347106754066b92b516104cb857`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Mon, 18 Jul 2022 21:29:30 GMT
ADD file:69e4080f15f54e2d8f8aa25fdcba9c01dde149d43592edd5023106675e54a769 in / 
# Mon, 18 Jul 2022 21:29:31 GMT
CMD ["/bin/sh"]
# Tue, 19 Jul 2022 05:02:34 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Tue, 19 Jul 2022 05:02:36 GMT
ENV LANG=en_US.utf8
# Tue, 19 Jul 2022 05:02:43 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 19 Jul 2022 05:08:15 GMT
ENV PG_MAJOR=14
# Tue, 19 Jul 2022 05:08:17 GMT
ENV PG_VERSION=14.4
# Tue, 19 Jul 2022 05:08:19 GMT
ENV PG_SHA256=c23b6237c5231c791511bdc79098617d6852e9e3bdf360efd8b5d15a1a3d8f6a
# Tue, 19 Jul 2022 05:12:30 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm-dev clang g++ 		make 		openldap-dev 		openssl-dev 		perl-dev 		perl-ipc-run 		perl-utils 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		icu-dev 		lz4-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-krb5 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 		--with-lz4 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 		zstd 		icu-data-full 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Tue, 19 Jul 2022 05:12:38 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample
# Tue, 19 Jul 2022 05:12:43 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 19 Jul 2022 05:12:44 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 19 Jul 2022 05:12:50 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 19 Jul 2022 05:12:52 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 19 Jul 2022 05:12:53 GMT
COPY file:232dce6cf487afb0c0cc43d38932ff29614a74b57cd04557dc7398e6d2b93b8f in /usr/local/bin/ 
# Tue, 19 Jul 2022 05:12:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 19 Jul 2022 05:12:56 GMT
STOPSIGNAL SIGINT
# Tue, 19 Jul 2022 05:12:58 GMT
EXPOSE 5432
# Tue, 19 Jul 2022 05:13:00 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:602896d442490cd3fbb6599f0f862d3673b7cd58eca3ac842b8e09bf8d012443`  
		Last Modified: Mon, 18 Jul 2022 19:09:09 GMT  
		Size: 2.8 MB (2789923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bea11e69809984567de191b5236f9f9412dd5e355bc134e106ad159f8301136`  
		Last Modified: Tue, 19 Jul 2022 05:34:23 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64e883d9bbf6af75c81f2d96c627e68d5520c1c80d8fd131f96423df163a6133`  
		Last Modified: Tue, 19 Jul 2022 05:34:23 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:144d3c642eb80c409f1c537495c0837343437f4df98f04237735453bdff43c1d`  
		Last Modified: Tue, 19 Jul 2022 05:35:07 GMT  
		Size: 88.1 MB (88120551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f17f7b3bf08317860dc8bf6458fe311e97634ab33a12beb82a11e8495dc74239`  
		Last Modified: Tue, 19 Jul 2022 05:34:53 GMT  
		Size: 9.2 KB (9204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:795cb4a263ffa63cbd40ce1e9646a4d15d908bf7e73bd503cfd63e0a120054db`  
		Last Modified: Tue, 19 Jul 2022 05:34:52 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b8f01fb21d3e7ebe6af6e5cf0aeac7e26e0f1a633ef678d94e58368bdff7d51`  
		Last Modified: Tue, 19 Jul 2022 05:34:52 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:899439f5b533079b59c6a3cd2bfdaa52cb99a60c5954e618237dacdf40219772`  
		Last Modified: Tue, 19 Jul 2022 05:34:52 GMT  
		Size: 4.7 KB (4705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:alpine3.16` - linux; s390x

```console
$ docker pull postgres@sha256:a1985a4a2aad2a90ff6cc53178a72cb90f75ab842a51a995202d6a30eea0c7c1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **85.9 MB (85875682 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:04d6a3b8376393a718c8d60048cded77c8ed709a67a18f62c64f9ada71e58861`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Mon, 18 Jul 2022 20:41:35 GMT
ADD file:deaa573cd61e07709846a5300fb627a8610e9754129c085ed483ff8897d0c002 in / 
# Mon, 18 Jul 2022 20:41:36 GMT
CMD ["/bin/sh"]
# Tue, 19 Jul 2022 03:37:54 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Tue, 19 Jul 2022 03:37:55 GMT
ENV LANG=en_US.utf8
# Tue, 19 Jul 2022 03:37:56 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 19 Jul 2022 03:43:25 GMT
ENV PG_MAJOR=14
# Tue, 19 Jul 2022 03:43:25 GMT
ENV PG_VERSION=14.4
# Tue, 19 Jul 2022 03:43:25 GMT
ENV PG_SHA256=c23b6237c5231c791511bdc79098617d6852e9e3bdf360efd8b5d15a1a3d8f6a
# Tue, 19 Jul 2022 03:47:42 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm-dev clang g++ 		make 		openldap-dev 		openssl-dev 		perl-dev 		perl-ipc-run 		perl-utils 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		icu-dev 		lz4-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-krb5 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 		--with-lz4 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 		zstd 		icu-data-full 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Tue, 19 Jul 2022 03:47:59 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample
# Tue, 19 Jul 2022 03:48:01 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 19 Jul 2022 03:48:02 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 19 Jul 2022 03:48:03 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 19 Jul 2022 03:48:04 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 19 Jul 2022 03:48:04 GMT
COPY file:232dce6cf487afb0c0cc43d38932ff29614a74b57cd04557dc7398e6d2b93b8f in /usr/local/bin/ 
# Tue, 19 Jul 2022 03:48:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 19 Jul 2022 03:48:05 GMT
STOPSIGNAL SIGINT
# Tue, 19 Jul 2022 03:48:06 GMT
EXPOSE 5432
# Tue, 19 Jul 2022 03:48:07 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:5f1840d5bacf4162a87f497e22d94bce946e660bdfce8eeefcbf7bd0beb193f3`  
		Last Modified: Mon, 18 Jul 2022 20:42:36 GMT  
		Size: 2.6 MB (2580798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef21d7303e7cec444c557678d1d82ed1093485abfa43d752e3b9b3f8ced44c5c`  
		Last Modified: Tue, 19 Jul 2022 04:05:59 GMT  
		Size: 1.3 KB (1287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c3215cc8466384c4108c3bfa65989864020c0a98faaca380239e0de7da5e115`  
		Last Modified: Tue, 19 Jul 2022 04:05:59 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6b7cc8ffc5ecc93be39fc895e6c7c4e8315283abed324e51938a90310e7d5c5`  
		Last Modified: Tue, 19 Jul 2022 04:06:31 GMT  
		Size: 83.3 MB (83279184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97f5a6b233a34c7f2b4d03d5a9aea31c02f1b1212204c46e5f29c9c4877ce098`  
		Last Modified: Tue, 19 Jul 2022 04:06:21 GMT  
		Size: 9.2 KB (9205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3c36d666f826f07a748646cdcf65d144ea0478b35ef440063f36c836d17413c`  
		Last Modified: Tue, 19 Jul 2022 04:06:21 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d90aa99a8cda997999a882a409df260316471859eeddc94d19e7debbbff8beb`  
		Last Modified: Tue, 19 Jul 2022 04:06:21 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e0eb26ecd529be727e1ba740d9fe0937671a32df1da185f7e9da4e56de649b0`  
		Last Modified: Tue, 19 Jul 2022 04:06:21 GMT  
		Size: 4.7 KB (4703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
