## `postgres:15rc1-alpine`

```console
$ docker pull postgres@sha256:a565aa880a08838742b2ee86ecfc702277551e4191ebd1f39de1277519c6ac74
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

### `postgres:15rc1-alpine` - linux; amd64

```console
$ docker pull postgres@sha256:061ec9753b1f97d9724538b6e2acf60b6079612ec71e5d3ba27529acc4106ec2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **85.4 MB (85350007 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1e08f51cf3a4384ff937b6590ce1dca2c5ae6fa4dc53b35b01f6f10b6d450abd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 01:10:45 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Fri, 07 Oct 2022 01:10:45 GMT
ENV LANG=en_US.utf8
# Fri, 07 Oct 2022 01:10:45 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 07 Oct 2022 01:10:45 GMT
ENV PG_MAJOR=15
# Fri, 07 Oct 2022 01:10:46 GMT
ENV PG_VERSION=15rc1
# Fri, 07 Oct 2022 01:10:46 GMT
ENV PG_SHA256=576476fab0d49f05f27625e1d6ed433e6e1358fabba92ae41780421e65fa7ad4
# Fri, 07 Oct 2022 01:14:04 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm-dev clang g++ 		make 		openldap-dev 		openssl-dev 		perl-dev 		perl-ipc-run 		perl-utils 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		icu-dev 		lz4-dev 		zstd-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-krb5 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 		--with-lz4 		--with-zstd 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 		zstd 		icu-data-full 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Fri, 07 Oct 2022 01:14:05 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample
# Fri, 07 Oct 2022 01:14:06 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 07 Oct 2022 01:14:06 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 07 Oct 2022 01:14:07 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 07 Oct 2022 01:14:07 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 07 Oct 2022 01:14:07 GMT
COPY file:232dce6cf487afb0c0cc43d38932ff29614a74b57cd04557dc7398e6d2b93b8f in /usr/local/bin/ 
# Fri, 07 Oct 2022 01:14:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 07 Oct 2022 01:14:07 GMT
STOPSIGNAL SIGINT
# Fri, 07 Oct 2022 01:14:07 GMT
EXPOSE 5432
# Fri, 07 Oct 2022 01:14:07 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40ab741cca09cae3efd0bccbe57183973b177cda2b7f65d67078454dc1d97ba7`  
		Last Modified: Fri, 07 Oct 2022 01:30:44 GMT  
		Size: 1.3 KB (1287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3636f308d36c203f3f75f1c294814f647b4641fc980b708edb341400491e6fc`  
		Last Modified: Fri, 07 Oct 2022 01:30:44 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cb4be8375c6f90481d5aa9cbfae45eb4e52c125886620d4738f47a96c7afdfd`  
		Last Modified: Fri, 07 Oct 2022 01:30:53 GMT  
		Size: 82.5 MB (82527990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcaeaebb2dbd74d6e1d70c7ce16aa489f249dc78af0b075754a3d993aa5975c2`  
		Last Modified: Fri, 07 Oct 2022 01:30:42 GMT  
		Size: 9.5 KB (9470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:604718d61ea725a2eee95d66ee203e7baa81771e96e9dce74051d195408b1f49`  
		Last Modified: Fri, 07 Oct 2022 01:30:42 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fea6d1741dba8e0620b07eb627a3b1201c82c1e2b6e30096f6d3364607530a9`  
		Last Modified: Fri, 07 Oct 2022 01:30:42 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffe61a2b3c94e440ac1fa8a2cd8d53e775e5e8b609f310e4588e61f288f11777`  
		Last Modified: Fri, 07 Oct 2022 01:30:43 GMT  
		Size: 4.7 KB (4700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:15rc1-alpine` - linux; arm variant v6

```console
$ docker pull postgres@sha256:791cc8c3d2f15c09df4ead4cfc9a133d54869243a156758d118d20b934e1a5ab
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **83.5 MB (83470328 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:48df0cde0862596e94046d56a7c7e608c8c12f98c8aafbdb531d45370c879d6b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:22 GMT
ADD file:e8733e8cc0a81e15ca4041760b6e27392c34171512d34405a9b262b1fff5c687 in / 
# Tue, 09 Aug 2022 17:49:22 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 15:56:27 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Fri, 07 Oct 2022 15:56:28 GMT
ENV LANG=en_US.utf8
# Fri, 07 Oct 2022 15:56:28 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 07 Oct 2022 15:56:28 GMT
ENV PG_MAJOR=15
# Fri, 07 Oct 2022 15:56:28 GMT
ENV PG_VERSION=15rc1
# Fri, 07 Oct 2022 15:56:29 GMT
ENV PG_SHA256=576476fab0d49f05f27625e1d6ed433e6e1358fabba92ae41780421e65fa7ad4
# Fri, 07 Oct 2022 16:08:44 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm-dev clang g++ 		make 		openldap-dev 		openssl-dev 		perl-dev 		perl-ipc-run 		perl-utils 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		icu-dev 		lz4-dev 		zstd-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-krb5 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 		--with-lz4 		--with-zstd 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 		zstd 		icu-data-full 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Fri, 07 Oct 2022 16:08:45 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample
# Fri, 07 Oct 2022 16:08:46 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 07 Oct 2022 16:08:46 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 07 Oct 2022 16:08:47 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 07 Oct 2022 16:08:47 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 07 Oct 2022 16:08:47 GMT
COPY file:232dce6cf487afb0c0cc43d38932ff29614a74b57cd04557dc7398e6d2b93b8f in /usr/local/bin/ 
# Fri, 07 Oct 2022 16:08:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 07 Oct 2022 16:08:47 GMT
STOPSIGNAL SIGINT
# Fri, 07 Oct 2022 16:08:48 GMT
EXPOSE 5432
# Fri, 07 Oct 2022 16:08:48 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:9506b835437abb4d8ba1683e00c500b8f77e1975e930b356fbb72f2dbdc274d9`  
		Last Modified: Tue, 09 Aug 2022 17:50:33 GMT  
		Size: 2.6 MB (2613965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4a97f44d5468b1977fffbbe13f6ea3bd6c5e69dd42ec5115a4c24e3269e14d1`  
		Last Modified: Fri, 07 Oct 2022 17:03:33 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:369971d6642d8d215945973b41cf0d2d39bcc95648a5615067e1453a0b350063`  
		Last Modified: Fri, 07 Oct 2022 17:03:32 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00160c9c1a0c4adfdfcba0336d57677540d100a8c8c55bca6084a8d2162da1f6`  
		Last Modified: Fri, 07 Oct 2022 17:03:48 GMT  
		Size: 80.8 MB (80840402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f935f59531da0db2dec1db1317d8e7b173c3627590f7f735f25af7e7a651932`  
		Last Modified: Fri, 07 Oct 2022 17:03:30 GMT  
		Size: 9.5 KB (9462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d655d2c1064eacfe2e09285a217456ed1b60890ad4ad8a63ca266e6e86fc805f`  
		Last Modified: Fri, 07 Oct 2022 17:03:30 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73a35dba5711da3dd696962992af66bcb1f8ecfb6da2d3990c132d0bf47ac6b0`  
		Last Modified: Fri, 07 Oct 2022 17:03:30 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84773400480a3ec65ca37fdcca638ba6a81687f44b0a990bb20cedd3215f46ad`  
		Last Modified: Fri, 07 Oct 2022 17:03:30 GMT  
		Size: 4.7 KB (4707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:15rc1-alpine` - linux; arm variant v7

```console
$ docker pull postgres@sha256:648d33573fde8c1e018698af08cd31ef6decb6cd85906ca60e1ad92cf6b0711a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **78.6 MB (78566778 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f62b4887eba117cad27c470e9a7eeac2a18953bb4e0e0a55c0634639b9ff000`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 09 Aug 2022 16:57:44 GMT
ADD file:75521fe16320b193092588f6f31052c85e736965ceb11673de18bd14965a45e6 in / 
# Tue, 09 Aug 2022 16:57:44 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 19:31:18 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Wed, 10 Aug 2022 19:31:18 GMT
ENV LANG=en_US.utf8
# Wed, 10 Aug 2022 19:31:19 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 10 Aug 2022 19:31:19 GMT
ENV PG_MAJOR=15
# Fri, 30 Sep 2022 19:27:32 GMT
ENV PG_VERSION=15rc1
# Fri, 30 Sep 2022 19:27:32 GMT
ENV PG_SHA256=576476fab0d49f05f27625e1d6ed433e6e1358fabba92ae41780421e65fa7ad4
# Fri, 30 Sep 2022 19:34:09 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm-dev clang g++ 		make 		openldap-dev 		openssl-dev 		perl-dev 		perl-ipc-run 		perl-utils 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		icu-dev 		lz4-dev 		zstd-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-krb5 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 		--with-lz4 		--with-zstd 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 		zstd 		icu-data-full 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Fri, 30 Sep 2022 19:34:09 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample
# Fri, 30 Sep 2022 19:34:10 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 30 Sep 2022 19:34:10 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 30 Sep 2022 19:34:11 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 30 Sep 2022 19:34:11 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 30 Sep 2022 19:34:11 GMT
COPY file:232dce6cf487afb0c0cc43d38932ff29614a74b57cd04557dc7398e6d2b93b8f in /usr/local/bin/ 
# Fri, 30 Sep 2022 19:34:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 30 Sep 2022 19:34:11 GMT
STOPSIGNAL SIGINT
# Fri, 30 Sep 2022 19:34:11 GMT
EXPOSE 5432
# Fri, 30 Sep 2022 19:34:11 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:c6556b3b6858c6fa1e328377cc2c4becdc9cd1bc3e7302aa7299936522cf93ba`  
		Last Modified: Tue, 09 Aug 2022 16:58:55 GMT  
		Size: 2.4 MB (2417065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8a738b39479fd8f48817ac98870f37b48f1856fe7db240c151ca31d02c8dc99`  
		Last Modified: Wed, 10 Aug 2022 20:36:55 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03b8cd076cdce07e25ab5ecddc7b199911583628b53f4fd34d24488968b80d8b`  
		Last Modified: Wed, 10 Aug 2022 20:36:55 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0500eae4e14c3ae4fb2d0bfb57ccb393a4ba4dcb11c21f38bfd13c29415b707`  
		Last Modified: Fri, 30 Sep 2022 19:49:07 GMT  
		Size: 76.1 MB (76133752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8b43648aa68c45dd5ca8d62469bf5a892e1bb5289162a280a604d76f8dd1d5e`  
		Last Modified: Fri, 30 Sep 2022 19:48:57 GMT  
		Size: 9.5 KB (9463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc30dd89feadc89cb3c95c6afb2fde88743ef1dfcfdca85f474fa83f66fc9ce9`  
		Last Modified: Fri, 30 Sep 2022 19:48:57 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:976603f8733db86556163d74c4b98202e6788393c31af213a987d9072c424cfd`  
		Last Modified: Fri, 30 Sep 2022 19:48:57 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4791984b2c20f09c1ec9b87ab65365766e95dbe16a5a8bac1e6849c494c1a7a0`  
		Last Modified: Fri, 30 Sep 2022 19:48:57 GMT  
		Size: 4.7 KB (4702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:15rc1-alpine` - linux; arm64 variant v8

```console
$ docker pull postgres@sha256:ed9b5055fb97825c14493d050f6783397265588959fc33625a00faf185ed572c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.2 MB (84192706 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a1f1262cb8d8b2ebe199a4af069ac8a00b4b8d8ce69808ce035b6f6d3b5a3aa`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Tue, 09 Aug 2022 17:39:42 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 04:05:38 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Fri, 07 Oct 2022 04:05:39 GMT
ENV LANG=en_US.utf8
# Fri, 07 Oct 2022 04:05:40 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 07 Oct 2022 04:05:41 GMT
ENV PG_MAJOR=15
# Fri, 07 Oct 2022 04:05:42 GMT
ENV PG_VERSION=15rc1
# Fri, 07 Oct 2022 04:05:43 GMT
ENV PG_SHA256=576476fab0d49f05f27625e1d6ed433e6e1358fabba92ae41780421e65fa7ad4
# Fri, 07 Oct 2022 04:09:07 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm-dev clang g++ 		make 		openldap-dev 		openssl-dev 		perl-dev 		perl-ipc-run 		perl-utils 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		icu-dev 		lz4-dev 		zstd-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-krb5 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 		--with-lz4 		--with-zstd 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 		zstd 		icu-data-full 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Fri, 07 Oct 2022 04:09:08 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample
# Fri, 07 Oct 2022 04:09:08 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 07 Oct 2022 04:09:09 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 07 Oct 2022 04:09:10 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 07 Oct 2022 04:09:11 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 07 Oct 2022 04:09:13 GMT
COPY file:232dce6cf487afb0c0cc43d38932ff29614a74b57cd04557dc7398e6d2b93b8f in /usr/local/bin/ 
# Fri, 07 Oct 2022 04:09:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 07 Oct 2022 04:09:14 GMT
STOPSIGNAL SIGINT
# Fri, 07 Oct 2022 04:09:15 GMT
EXPOSE 5432
# Fri, 07 Oct 2022 04:09:16 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5ac05eb62a0d312c6a5077cc54b5bca58a2c51aec7a337f3339c7084aaf153c`  
		Last Modified: Fri, 07 Oct 2022 04:28:06 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fbbc8b450549bfae843e4365be3315e577270effad7c627affbd83b95e98bad`  
		Last Modified: Fri, 07 Oct 2022 04:28:06 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc3f51735b9c1505858c965ad4547b0f2f7a2fd85de93ab1cd2d0f83d84818ff`  
		Last Modified: Fri, 07 Oct 2022 04:28:15 GMT  
		Size: 81.5 MB (81469200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c58a1b99f9f9bcebe0cb75a12c54130a32edf40c97a1d0172df544da1ee191f9`  
		Last Modified: Fri, 07 Oct 2022 04:28:04 GMT  
		Size: 9.5 KB (9465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75fffe2dbd3457a46c73b167b372947dab54503a9fa4f95bd5da7ac6752ea400`  
		Last Modified: Fri, 07 Oct 2022 04:28:04 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1b9ef12a389fce4308d036a6fe39808794373997abc52263c2347e17b2136da`  
		Last Modified: Fri, 07 Oct 2022 04:28:04 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49e041e522ce38e0bd6c4005e33a904f4dc2ef498e00bc955b19d76ff1e815a3`  
		Last Modified: Fri, 07 Oct 2022 04:28:04 GMT  
		Size: 4.7 KB (4704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:15rc1-alpine` - linux; 386

```console
$ docker pull postgres@sha256:93569f0bb3b1fd7c46fec84c74aa8ff91b734c4996cd90307e043b4920cb3e9e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **90.7 MB (90689658 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:72216e86da3269646a13a2f7776a7b85cd4290d67643eb0cdfa2dc8af60f0b9e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 09 Aug 2022 17:38:39 GMT
ADD file:b828bc14bc5ff03c8f7310fe0aed6ac5df19a393622d5d1d779a523234d07c0a in / 
# Tue, 09 Aug 2022 17:38:39 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 22:58:32 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 06 Oct 2022 22:58:33 GMT
ENV LANG=en_US.utf8
# Thu, 06 Oct 2022 22:58:34 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 06 Oct 2022 22:58:35 GMT
ENV PG_MAJOR=15
# Thu, 06 Oct 2022 22:58:36 GMT
ENV PG_VERSION=15rc1
# Thu, 06 Oct 2022 22:58:37 GMT
ENV PG_SHA256=576476fab0d49f05f27625e1d6ed433e6e1358fabba92ae41780421e65fa7ad4
# Thu, 06 Oct 2022 23:02:34 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm-dev clang g++ 		make 		openldap-dev 		openssl-dev 		perl-dev 		perl-ipc-run 		perl-utils 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		icu-dev 		lz4-dev 		zstd-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-krb5 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 		--with-lz4 		--with-zstd 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 		zstd 		icu-data-full 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Thu, 06 Oct 2022 23:02:35 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample
# Thu, 06 Oct 2022 23:02:36 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 06 Oct 2022 23:02:37 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 06 Oct 2022 23:02:38 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 06 Oct 2022 23:02:39 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 06 Oct 2022 23:02:41 GMT
COPY file:232dce6cf487afb0c0cc43d38932ff29614a74b57cd04557dc7398e6d2b93b8f in /usr/local/bin/ 
# Thu, 06 Oct 2022 23:02:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 06 Oct 2022 23:02:42 GMT
STOPSIGNAL SIGINT
# Thu, 06 Oct 2022 23:02:43 GMT
EXPOSE 5432
# Thu, 06 Oct 2022 23:02:44 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:6c0d3b419d848ea31ca748254611d5d5ce3b76e3d7bba520fd87400fbb75f3b9`  
		Last Modified: Tue, 09 Aug 2022 17:39:33 GMT  
		Size: 2.8 MB (2807121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcc0a2d06c52831b717922c82a177581313d43ff48fa82da49ed9fe0bf8002d8`  
		Last Modified: Thu, 06 Oct 2022 23:23:50 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3642389f32b5996f507baab5859e392131d7bce3768326935a4dfb51d4932b5a`  
		Last Modified: Thu, 06 Oct 2022 23:23:50 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ceef4e0c1ee03cc4185669ae46fc0bfd292a1f9fe750d91af0ced2148e09daa`  
		Last Modified: Thu, 06 Oct 2022 23:23:59 GMT  
		Size: 87.9 MB (87866698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:035405de074d739f5dd83786d4c284e3644a618da09cf2eed9bdf4126535b635`  
		Last Modified: Thu, 06 Oct 2022 23:23:48 GMT  
		Size: 9.5 KB (9463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bd48f581bd6daf130df58e5a596dd56a14b3aaab009e7171effa23062f0063c`  
		Last Modified: Thu, 06 Oct 2022 23:23:49 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7b8a958844a6fafd54ac2b54035a6f21d2bb47ba0721766d2b120965b9dac5e`  
		Last Modified: Thu, 06 Oct 2022 23:23:48 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a18537a55de9e2084475313b5830a744300002ce13724d38bda70a5c621f532`  
		Last Modified: Thu, 06 Oct 2022 23:23:48 GMT  
		Size: 4.7 KB (4701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:15rc1-alpine` - linux; ppc64le

```console
$ docker pull postgres@sha256:03b5752e867bfe65278ca76d970664b43561df8bc5f8bcc39c7c20582351eb0a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.6 MB (91648827 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a3d869823e42ddd08bdeb7f418a16c5f5feeea4695b7c9edc9571580ad4359a2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 09 Aug 2022 17:17:09 GMT
ADD file:66b351666e41834033d334aeb3dc6998dea77aa22e8e254028c923fee67a41a8 in / 
# Tue, 09 Aug 2022 17:17:10 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 02:25:58 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Fri, 07 Oct 2022 02:25:59 GMT
ENV LANG=en_US.utf8
# Fri, 07 Oct 2022 02:26:00 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 07 Oct 2022 02:26:00 GMT
ENV PG_MAJOR=15
# Fri, 07 Oct 2022 02:26:01 GMT
ENV PG_VERSION=15rc1
# Fri, 07 Oct 2022 02:26:01 GMT
ENV PG_SHA256=576476fab0d49f05f27625e1d6ed433e6e1358fabba92ae41780421e65fa7ad4
# Fri, 07 Oct 2022 02:30:28 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm-dev clang g++ 		make 		openldap-dev 		openssl-dev 		perl-dev 		perl-ipc-run 		perl-utils 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		icu-dev 		lz4-dev 		zstd-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-krb5 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 		--with-lz4 		--with-zstd 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 		zstd 		icu-data-full 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Fri, 07 Oct 2022 02:30:32 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample
# Fri, 07 Oct 2022 02:30:33 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 07 Oct 2022 02:30:33 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 07 Oct 2022 02:30:34 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 07 Oct 2022 02:30:34 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 07 Oct 2022 02:30:35 GMT
COPY file:232dce6cf487afb0c0cc43d38932ff29614a74b57cd04557dc7398e6d2b93b8f in /usr/local/bin/ 
# Fri, 07 Oct 2022 02:30:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 07 Oct 2022 02:30:35 GMT
STOPSIGNAL SIGINT
# Fri, 07 Oct 2022 02:30:36 GMT
EXPOSE 5432
# Fri, 07 Oct 2022 02:30:36 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:c79e5d1a8c89b87020a754c8a5c8370faaa37bfb5bca1d8af66770d522ef1caf`  
		Last Modified: Tue, 09 Aug 2022 17:18:26 GMT  
		Size: 2.8 MB (2803320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c9886199ad194bb654781346f2cd4cce2905c90d143f8d77e5869dada1864c5`  
		Last Modified: Fri, 07 Oct 2022 02:54:28 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dca1982ca555c7b16501b90c9ee856d6d3a531258352fd09a5db82ef45f9984`  
		Last Modified: Fri, 07 Oct 2022 02:54:27 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cde9e4bf10d8474203d44c8470b3ce721de695814a3957bacc0c7b42613b17f`  
		Last Modified: Fri, 07 Oct 2022 02:54:45 GMT  
		Size: 88.8 MB (88829540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71b523db6a281275ad717c6271abcd5bf4af87ce50ca7d11fa589ee245347c38`  
		Last Modified: Fri, 07 Oct 2022 02:54:26 GMT  
		Size: 9.5 KB (9469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6cb525e544a24496ed0a305793647c8ee0c7711f59367853438c5049125a403`  
		Last Modified: Fri, 07 Oct 2022 02:54:25 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c697ac378cde5779a4c6d79142db6463724718538c16ed620da0b3297737b08f`  
		Last Modified: Fri, 07 Oct 2022 02:54:25 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:391ae7e103c4bcf9bccef38dc5c2bf237f25700bafefc3e4c19ed0c383c4e745`  
		Last Modified: Fri, 07 Oct 2022 02:54:25 GMT  
		Size: 4.7 KB (4705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:15rc1-alpine` - linux; s390x

```console
$ docker pull postgres@sha256:0bd49b872f433198a343e686415ba9abda10fce50e5c9bb1206874572d66e486
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **86.6 MB (86563565 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2037dd795a00ce2c18ce13ca4a8a23800fadc7e49537ccbf03012be367010c03`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 09 Aug 2022 17:41:46 GMT
ADD file:b43a065471bc4711415d3c67cd5b6559b0c48ee7ffe9761530477cf457a6dc34 in / 
# Tue, 09 Aug 2022 17:41:46 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 03:35:39 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Fri, 07 Oct 2022 03:35:39 GMT
ENV LANG=en_US.utf8
# Fri, 07 Oct 2022 03:35:41 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 07 Oct 2022 03:35:41 GMT
ENV PG_MAJOR=15
# Fri, 07 Oct 2022 03:35:41 GMT
ENV PG_VERSION=15rc1
# Fri, 07 Oct 2022 03:35:42 GMT
ENV PG_SHA256=576476fab0d49f05f27625e1d6ed433e6e1358fabba92ae41780421e65fa7ad4
# Fri, 07 Oct 2022 03:39:52 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm-dev clang g++ 		make 		openldap-dev 		openssl-dev 		perl-dev 		perl-ipc-run 		perl-utils 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		icu-dev 		lz4-dev 		zstd-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-krb5 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 		--with-lz4 		--with-zstd 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 		zstd 		icu-data-full 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Fri, 07 Oct 2022 03:40:02 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample
# Fri, 07 Oct 2022 03:40:03 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 07 Oct 2022 03:40:03 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 07 Oct 2022 03:40:04 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 07 Oct 2022 03:40:05 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 07 Oct 2022 03:40:05 GMT
COPY file:232dce6cf487afb0c0cc43d38932ff29614a74b57cd04557dc7398e6d2b93b8f in /usr/local/bin/ 
# Fri, 07 Oct 2022 03:40:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 07 Oct 2022 03:40:05 GMT
STOPSIGNAL SIGINT
# Fri, 07 Oct 2022 03:40:06 GMT
EXPOSE 5432
# Fri, 07 Oct 2022 03:40:06 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:790c84f1f3409eab952345157df7fa804ba6b5f06d4ceb6f2dfa3c6de2064397`  
		Last Modified: Tue, 09 Aug 2022 17:42:45 GMT  
		Size: 2.6 MB (2590597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e890de774640a358825541264ef983fef765c29d72f21038ede1ac41c85e6fd`  
		Last Modified: Fri, 07 Oct 2022 04:02:51 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:310de1aaaef21df2d67997a7dfe754c704ddf70ece33ada85f4f2dd0a4e02359`  
		Last Modified: Fri, 07 Oct 2022 04:02:51 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5cfa7675041abe02577686daaff10071e243460dca0fe9ca2b9a6a62ee20bcb`  
		Last Modified: Fri, 07 Oct 2022 04:03:00 GMT  
		Size: 84.0 MB (83957005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:370604c1af8483417520cca9857ca1e2701b04b598b3a9f683e053f95e67f222`  
		Last Modified: Fri, 07 Oct 2022 04:02:50 GMT  
		Size: 9.5 KB (9466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bc6181bb67428db23fdf12597dd3b405e7317124fb9d5849782a8af6f5cca37`  
		Last Modified: Fri, 07 Oct 2022 04:02:50 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:335e2aae832612cecc16dd923cdc1771209d498633ceefa7a28ab9688f88f3ab`  
		Last Modified: Fri, 07 Oct 2022 04:02:50 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fad49f5a4fde7424385dbd2852f95af4a794695f3e4273cbaa4519ea52009b1d`  
		Last Modified: Fri, 07 Oct 2022 04:02:50 GMT  
		Size: 4.7 KB (4704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
