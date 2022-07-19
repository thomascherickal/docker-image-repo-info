## `postgres:15beta2-alpine3.16`

```console
$ docker pull postgres@sha256:f0c9b02959d56e186a0c4ad69e8f8134e8da05b1276d70d4c1b6d8582232b0f5
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

### `postgres:15beta2-alpine3.16` - linux; amd64

```console
$ docker pull postgres@sha256:e02e2708d5966029d4618855f889d0f8d74adfe71c71592cdb55252589050cc5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **85.5 MB (85542554 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f3c8bf75c81922885d97e15f1b4e8e88b7348b93e41535fcad550e5514387ca`
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
# Tue, 19 Jul 2022 01:37:19 GMT
ENV PG_MAJOR=15
# Tue, 19 Jul 2022 01:37:19 GMT
ENV PG_VERSION=15beta2
# Tue, 19 Jul 2022 01:37:19 GMT
ENV PG_SHA256=2fedbc58b370f30e5f59fb0dcc8128a2ef9a922b50fa931b442e4fa27ca98830
# Tue, 19 Jul 2022 01:40:55 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm-dev clang g++ 		make 		openldap-dev 		openssl-dev 		perl-dev 		perl-ipc-run 		perl-utils 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		icu-dev 		lz4-dev 		zstd-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-krb5 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 		--with-lz4 		--with-zstd 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 		zstd 		icu-data-full 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Tue, 19 Jul 2022 01:40:56 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample
# Tue, 19 Jul 2022 01:40:57 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 19 Jul 2022 01:40:57 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 19 Jul 2022 01:40:57 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 19 Jul 2022 01:40:58 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 19 Jul 2022 01:40:58 GMT
COPY file:232dce6cf487afb0c0cc43d38932ff29614a74b57cd04557dc7398e6d2b93b8f in /usr/local/bin/ 
# Tue, 19 Jul 2022 01:40:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 19 Jul 2022 01:40:58 GMT
STOPSIGNAL SIGINT
# Tue, 19 Jul 2022 01:40:58 GMT
EXPOSE 5432
# Tue, 19 Jul 2022 01:40:58 GMT
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
	-	`sha256:7d921115293d11f6e49321b1947bb3aa3924810674df56f42d1505e0f44dbb74`  
		Last Modified: Tue, 19 Jul 2022 01:58:55 GMT  
		Size: 82.7 MB (82727796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f31ad885612e4dbdbe2c944b73e524ffe36a8591272b7c16da4ebd68ee27868c`  
		Last Modified: Tue, 19 Jul 2022 01:58:44 GMT  
		Size: 9.5 KB (9458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f7a050dd8e411b164d7e4fb615dd8fd79c9bd50c33a16b25f951b28d776540b`  
		Last Modified: Tue, 19 Jul 2022 01:58:44 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3835832cb206024806d8af13c6360a5ec03bb9c4d3867b7c8dc016351744a59`  
		Last Modified: Tue, 19 Jul 2022 01:58:44 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cab478ee290cf8321a2b6c5db927449a21476bdad4283ebd9ad55843548ddab1`  
		Last Modified: Tue, 19 Jul 2022 01:58:44 GMT  
		Size: 4.7 KB (4703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:15beta2-alpine3.16` - linux; arm variant v6

```console
$ docker pull postgres@sha256:4f9b01c23453641796e433544658331c259bc12a8b827b3f95461d879efc39eb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **83.6 MB (83641295 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12a0712ef860b6e91cd8b22b07a7de934a13820173fff7dc10e4875e84da1746`
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
# Mon, 18 Jul 2022 21:06:38 GMT
ENV PG_MAJOR=15
# Mon, 18 Jul 2022 21:06:38 GMT
ENV PG_VERSION=15beta2
# Mon, 18 Jul 2022 21:06:39 GMT
ENV PG_SHA256=2fedbc58b370f30e5f59fb0dcc8128a2ef9a922b50fa931b442e4fa27ca98830
# Mon, 18 Jul 2022 21:13:02 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm-dev clang g++ 		make 		openldap-dev 		openssl-dev 		perl-dev 		perl-ipc-run 		perl-utils 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		icu-dev 		lz4-dev 		zstd-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-krb5 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 		--with-lz4 		--with-zstd 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 		zstd 		icu-data-full 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Mon, 18 Jul 2022 21:13:04 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample
# Mon, 18 Jul 2022 21:13:06 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Mon, 18 Jul 2022 21:13:06 GMT
ENV PGDATA=/var/lib/postgresql/data
# Mon, 18 Jul 2022 21:13:08 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Mon, 18 Jul 2022 21:13:08 GMT
VOLUME [/var/lib/postgresql/data]
# Mon, 18 Jul 2022 21:13:09 GMT
COPY file:232dce6cf487afb0c0cc43d38932ff29614a74b57cd04557dc7398e6d2b93b8f in /usr/local/bin/ 
# Mon, 18 Jul 2022 21:13:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 18 Jul 2022 21:13:09 GMT
STOPSIGNAL SIGINT
# Mon, 18 Jul 2022 21:13:10 GMT
EXPOSE 5432
# Mon, 18 Jul 2022 21:13:10 GMT
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
	-	`sha256:6b90e83ffafd65b52949a6d598a2250a913e5d30d6f40265052ae754df110f9f`  
		Last Modified: Mon, 18 Jul 2022 21:44:52 GMT  
		Size: 81.0 MB (81018904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ac8f58b562b3a7f3fad81b20f2fec1750f30e9054fbce99e008a6c3ea00d9ec`  
		Last Modified: Mon, 18 Jul 2022 21:44:05 GMT  
		Size: 9.5 KB (9464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:363db02263dd084c8c1e5e28770d314b51c3ae3929c85fc954b8f49f7e6af226`  
		Last Modified: Mon, 18 Jul 2022 21:44:05 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e3cf208cec18027f86257ddc089a2a1bc247cf08dbc86019198b3623c59840c`  
		Last Modified: Mon, 18 Jul 2022 21:44:05 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:580031eb76f29331bec12507b778f65a6aa32811fb54103a9c12036187b1a814`  
		Last Modified: Mon, 18 Jul 2022 21:44:05 GMT  
		Size: 4.7 KB (4707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:15beta2-alpine3.16` - linux; arm variant v7

```console
$ docker pull postgres@sha256:b97163de49765226474c771421bdbd9f5f55c4171010e55b239a8c4f71f30142
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **79.9 MB (79895085 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b2a514fb0326423a1b9fc5a8273a98c7f818dc1419f990678958c00b56d47a9`
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
# Wed, 25 May 2022 20:19:30 GMT
ENV PG_MAJOR=15
# Fri, 01 Jul 2022 02:50:47 GMT
ENV PG_VERSION=15beta2
# Fri, 01 Jul 2022 02:50:48 GMT
ENV PG_SHA256=2fedbc58b370f30e5f59fb0dcc8128a2ef9a922b50fa931b442e4fa27ca98830
# Fri, 01 Jul 2022 02:56:53 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm-dev clang g++ 		make 		openldap-dev 		openssl-dev 		perl-dev 		perl-ipc-run 		perl-utils 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		icu-dev 		lz4-dev 		zstd-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-krb5 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 		--with-lz4 		--with-zstd 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 		zstd 		icu-data-full 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Fri, 01 Jul 2022 02:56:55 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample
# Fri, 01 Jul 2022 02:56:57 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 01 Jul 2022 02:56:57 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 01 Jul 2022 02:56:59 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 01 Jul 2022 02:56:59 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 01 Jul 2022 02:57:00 GMT
COPY file:232dce6cf487afb0c0cc43d38932ff29614a74b57cd04557dc7398e6d2b93b8f in /usr/local/bin/ 
# Fri, 01 Jul 2022 02:57:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 01 Jul 2022 02:57:00 GMT
STOPSIGNAL SIGINT
# Fri, 01 Jul 2022 02:57:01 GMT
EXPOSE 5432
# Fri, 01 Jul 2022 02:57:01 GMT
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
	-	`sha256:6e4a4a8d3b4d53ad0324eb14d65f6cfc6cb9fe1a56d2695db561a48aa87b5ea2`  
		Last Modified: Fri, 01 Jul 2022 03:04:55 GMT  
		Size: 77.5 MB (77467479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9ba3af8eaf74b6eacd90a0a4f24a4fa8cbf919245178f23679b371904ec854b`  
		Last Modified: Fri, 01 Jul 2022 03:04:13 GMT  
		Size: 9.5 KB (9463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed94ed45236235f744839badea63240b1fd2403b86ddef45732f110aae2523f4`  
		Last Modified: Fri, 01 Jul 2022 03:04:13 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a9343213cf33373173b4aa395f05268de882c0589a95988710245214b7ae4c4`  
		Last Modified: Fri, 01 Jul 2022 03:04:13 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5d81151035a4b2ab842b15d379cd6e6c2896fb1bf3e4aad3f55675017d71ca2`  
		Last Modified: Fri, 01 Jul 2022 03:04:13 GMT  
		Size: 4.7 KB (4702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:15beta2-alpine3.16` - linux; arm64 variant v8

```console
$ docker pull postgres@sha256:bf44c08f894a915806ad1ac408bf602b11cfb981a671b645e62d4020a9a3bca3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.4 MB (84369792 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a4fc9a3ecc24b3968b308bb60b3cba6478a0733d046c6a9b1ce46ff09d9c05f`
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
# Tue, 19 Jul 2022 01:26:40 GMT
ENV PG_MAJOR=15
# Tue, 19 Jul 2022 01:26:41 GMT
ENV PG_VERSION=15beta2
# Tue, 19 Jul 2022 01:26:42 GMT
ENV PG_SHA256=2fedbc58b370f30e5f59fb0dcc8128a2ef9a922b50fa931b442e4fa27ca98830
# Tue, 19 Jul 2022 01:30:18 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm-dev clang g++ 		make 		openldap-dev 		openssl-dev 		perl-dev 		perl-ipc-run 		perl-utils 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		icu-dev 		lz4-dev 		zstd-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-krb5 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 		--with-lz4 		--with-zstd 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 		zstd 		icu-data-full 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Tue, 19 Jul 2022 01:30:19 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample
# Tue, 19 Jul 2022 01:30:20 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 19 Jul 2022 01:30:21 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 19 Jul 2022 01:30:22 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 19 Jul 2022 01:30:23 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 19 Jul 2022 01:30:25 GMT
COPY file:232dce6cf487afb0c0cc43d38932ff29614a74b57cd04557dc7398e6d2b93b8f in /usr/local/bin/ 
# Tue, 19 Jul 2022 01:30:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 19 Jul 2022 01:30:26 GMT
STOPSIGNAL SIGINT
# Tue, 19 Jul 2022 01:30:27 GMT
EXPOSE 5432
# Tue, 19 Jul 2022 01:30:28 GMT
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
	-	`sha256:9baeb91f3108fee25fe44dcc2800fdab9786a2c67c7514d07b6db0a917fd0998`  
		Last Modified: Tue, 19 Jul 2022 01:49:30 GMT  
		Size: 81.7 MB (81659244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef1c6e957c2451725fc0ef626369ca8b913f8fa8616851baeb23b81b4c9f5909`  
		Last Modified: Tue, 19 Jul 2022 01:49:19 GMT  
		Size: 9.5 KB (9455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d3dbc04ad0a04c38e5f14f14c61f7c7783375c0d32a09232f662e27db532024`  
		Last Modified: Tue, 19 Jul 2022 01:49:19 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90ef6a5d69036261252e345b8551bf662db30cfbd40a5825fb315622d38ee96d`  
		Last Modified: Tue, 19 Jul 2022 01:49:19 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc0b52c1ea64dfe2bcc7d99595ce3fd8c4517849b18cc2ce0a3277cf89db8d2e`  
		Last Modified: Tue, 19 Jul 2022 01:49:19 GMT  
		Size: 4.7 KB (4700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:15beta2-alpine3.16` - linux; 386

```console
$ docker pull postgres@sha256:cda53e0fad458ad656262b06d0f68c5d79b6258184391637728ad2cbf3803113
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **90.9 MB (90888780 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b2cfa15db3917d8fca053eb911cebea38de2733e465adbf57a58c9e9e045d39c`
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
# Mon, 18 Jul 2022 22:52:19 GMT
ENV PG_MAJOR=15
# Mon, 18 Jul 2022 22:52:20 GMT
ENV PG_VERSION=15beta2
# Mon, 18 Jul 2022 22:52:21 GMT
ENV PG_SHA256=2fedbc58b370f30e5f59fb0dcc8128a2ef9a922b50fa931b442e4fa27ca98830
# Mon, 18 Jul 2022 22:56:22 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm-dev clang g++ 		make 		openldap-dev 		openssl-dev 		perl-dev 		perl-ipc-run 		perl-utils 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		icu-dev 		lz4-dev 		zstd-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-krb5 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 		--with-lz4 		--with-zstd 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 		zstd 		icu-data-full 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Mon, 18 Jul 2022 22:56:23 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample
# Mon, 18 Jul 2022 22:56:23 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Mon, 18 Jul 2022 22:56:24 GMT
ENV PGDATA=/var/lib/postgresql/data
# Mon, 18 Jul 2022 22:56:25 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Mon, 18 Jul 2022 22:56:26 GMT
VOLUME [/var/lib/postgresql/data]
# Mon, 18 Jul 2022 22:56:28 GMT
COPY file:232dce6cf487afb0c0cc43d38932ff29614a74b57cd04557dc7398e6d2b93b8f in /usr/local/bin/ 
# Mon, 18 Jul 2022 22:56:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 18 Jul 2022 22:56:29 GMT
STOPSIGNAL SIGINT
# Mon, 18 Jul 2022 22:56:30 GMT
EXPOSE 5432
# Mon, 18 Jul 2022 22:56:31 GMT
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
	-	`sha256:2718fd8b59d6143c1bca83bef3aa71dd1f1bdaf4d3a8b9cff5d85caa26a33b29`  
		Last Modified: Mon, 18 Jul 2022 23:17:30 GMT  
		Size: 88.1 MB (88070617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26985507281ac12cc8287ec6dbef58a23375c875712b0ca3fa5f8d522427c689`  
		Last Modified: Mon, 18 Jul 2022 23:17:19 GMT  
		Size: 9.5 KB (9457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a91e6f2b6be45787370ca52c275c1ab7e78d4e85b891ecbe60050bdc1c6f81d`  
		Last Modified: Mon, 18 Jul 2022 23:17:19 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:444302d14d4a9946a0908b2476a6df0f944b5c5fd22df4bbb84ad07bdbd91c4f`  
		Last Modified: Mon, 18 Jul 2022 23:17:19 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:698fa2ea89574fce7854fd333cfa482a583d5280c3b675a4b720c92a9df835b8`  
		Last Modified: Mon, 18 Jul 2022 23:17:19 GMT  
		Size: 4.7 KB (4702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:15beta2-alpine3.16` - linux; ppc64le

```console
$ docker pull postgres@sha256:cd7534be45d32e5b6b1bb312193ace9eba52c55d926318f97104997ba8b39bec
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.8 MB (91827311 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d5d1c459161cf236cfbef46b44fb10446662e33c61f2f44040ed373567c2aa1e`
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
# Tue, 19 Jul 2022 05:02:47 GMT
ENV PG_MAJOR=15
# Tue, 19 Jul 2022 05:02:51 GMT
ENV PG_VERSION=15beta2
# Tue, 19 Jul 2022 05:02:54 GMT
ENV PG_SHA256=2fedbc58b370f30e5f59fb0dcc8128a2ef9a922b50fa931b442e4fa27ca98830
# Tue, 19 Jul 2022 05:07:24 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm-dev clang g++ 		make 		openldap-dev 		openssl-dev 		perl-dev 		perl-ipc-run 		perl-utils 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		icu-dev 		lz4-dev 		zstd-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-krb5 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 		--with-lz4 		--with-zstd 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 		zstd 		icu-data-full 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Tue, 19 Jul 2022 05:07:34 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample
# Tue, 19 Jul 2022 05:07:39 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 19 Jul 2022 05:07:42 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 19 Jul 2022 05:07:46 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 19 Jul 2022 05:07:48 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 19 Jul 2022 05:07:49 GMT
COPY file:232dce6cf487afb0c0cc43d38932ff29614a74b57cd04557dc7398e6d2b93b8f in /usr/local/bin/ 
# Tue, 19 Jul 2022 05:07:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 19 Jul 2022 05:07:54 GMT
STOPSIGNAL SIGINT
# Tue, 19 Jul 2022 05:07:56 GMT
EXPOSE 5432
# Tue, 19 Jul 2022 05:07:59 GMT
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
	-	`sha256:f6451148188196a7e0cf9c1c0e3ad92b3b36b16a84520fab61ce8146d3c45319`  
		Last Modified: Tue, 19 Jul 2022 05:34:34 GMT  
		Size: 89.0 MB (89021429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea03c73df6cf283cba536bbc096ea2937595b4bd1afc71412647a947ab16b03e`  
		Last Modified: Tue, 19 Jul 2022 05:34:20 GMT  
		Size: 9.5 KB (9458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:395090df6ef2a1daa7920696fdd9649bca4fbfb96bfd4ec63b849ccde4b89b1e`  
		Last Modified: Tue, 19 Jul 2022 05:34:20 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77bd8043251e19123dc6bd1eec9ddafa8214b177276b272850ecf5bf9ca186a6`  
		Last Modified: Tue, 19 Jul 2022 05:34:20 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17eddae60d72e131d4860f699bdc83a1ff9f9cae5a2f69b102a811134563a253`  
		Last Modified: Tue, 19 Jul 2022 05:34:20 GMT  
		Size: 4.7 KB (4705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:15beta2-alpine3.16` - linux; s390x

```console
$ docker pull postgres@sha256:0c371c204306955692ba48654adec3f876027c71960bd3fbdf61f05c8d2f8e88
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **86.8 MB (86752295 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:54cf593d1108c997e0c8b6bb0c7ec3e7ed5ff776caa396be2f519d0c304a804d`
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
# Tue, 19 Jul 2022 03:37:57 GMT
ENV PG_MAJOR=15
# Tue, 19 Jul 2022 03:37:57 GMT
ENV PG_VERSION=15beta2
# Tue, 19 Jul 2022 03:37:58 GMT
ENV PG_SHA256=2fedbc58b370f30e5f59fb0dcc8128a2ef9a922b50fa931b442e4fa27ca98830
# Tue, 19 Jul 2022 03:42:40 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm-dev clang g++ 		make 		openldap-dev 		openssl-dev 		perl-dev 		perl-ipc-run 		perl-utils 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		icu-dev 		lz4-dev 		zstd-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-krb5 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 		--with-lz4 		--with-zstd 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 		zstd 		icu-data-full 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Tue, 19 Jul 2022 03:42:53 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample
# Tue, 19 Jul 2022 03:42:55 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 19 Jul 2022 03:42:55 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 19 Jul 2022 03:42:57 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 19 Jul 2022 03:42:58 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 19 Jul 2022 03:42:58 GMT
COPY file:232dce6cf487afb0c0cc43d38932ff29614a74b57cd04557dc7398e6d2b93b8f in /usr/local/bin/ 
# Tue, 19 Jul 2022 03:42:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 19 Jul 2022 03:42:59 GMT
STOPSIGNAL SIGINT
# Tue, 19 Jul 2022 03:43:00 GMT
EXPOSE 5432
# Tue, 19 Jul 2022 03:43:00 GMT
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
	-	`sha256:9eb39de721e58404070ef6431eb254a2db15b94ffc1cfadcbfde4035e37571e7`  
		Last Modified: Tue, 19 Jul 2022 04:06:07 GMT  
		Size: 84.2 MB (84155546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93e4231040ce23abe1d7691184a0877ea359c2596cf7129875c4a67cf44fbbd7`  
		Last Modified: Tue, 19 Jul 2022 04:05:58 GMT  
		Size: 9.5 KB (9459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb1e778b2b1ea828e6f1a80d52237c1bcf2dc0c51d0d371de8767bc1efce949f`  
		Last Modified: Tue, 19 Jul 2022 04:05:57 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0d3dba656849d96178aeb3fdb46d7610b9cd129e66dcbeca672e95eaa496cd1`  
		Last Modified: Tue, 19 Jul 2022 04:05:57 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f79e10a6853e79b59aad0576ffbd91b89999166b38aacfbb40ef179936215a2`  
		Last Modified: Tue, 19 Jul 2022 04:05:57 GMT  
		Size: 4.7 KB (4702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
