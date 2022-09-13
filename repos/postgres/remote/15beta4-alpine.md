## `postgres:15beta4-alpine`

```console
$ docker pull postgres@sha256:90d350c999096350497a46339614f2cf6d0ea7e3f11d4120ce5338ee630635d8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; s390x

### `postgres:15beta4-alpine` - linux; amd64

```console
$ docker pull postgres@sha256:04ffc78fb8731da85b5be783de68c6ecbd18b9694bed8d836d816d40281ebcef
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **85.3 MB (85346549 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:24cad2537b26b6c6ee7cf473be63e58c1f8a6df76d4b1803cc189cfc60512be2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 23:10:36 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Tue, 09 Aug 2022 23:10:37 GMT
ENV LANG=en_US.utf8
# Tue, 09 Aug 2022 23:10:37 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 09 Aug 2022 23:10:37 GMT
ENV PG_MAJOR=15
# Mon, 12 Sep 2022 22:45:55 GMT
ENV PG_VERSION=15beta4
# Mon, 12 Sep 2022 22:45:55 GMT
ENV PG_SHA256=d84d18ef26a64e76f189b7efb05179920eb0e8ae5d68cdbdbbe966305aee4416
# Mon, 12 Sep 2022 22:49:14 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm-dev clang g++ 		make 		openldap-dev 		openssl-dev 		perl-dev 		perl-ipc-run 		perl-utils 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		icu-dev 		lz4-dev 		zstd-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-krb5 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 		--with-lz4 		--with-zstd 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 		zstd 		icu-data-full 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Mon, 12 Sep 2022 22:49:15 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample
# Mon, 12 Sep 2022 22:49:15 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Mon, 12 Sep 2022 22:49:15 GMT
ENV PGDATA=/var/lib/postgresql/data
# Mon, 12 Sep 2022 22:49:16 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Mon, 12 Sep 2022 22:49:16 GMT
VOLUME [/var/lib/postgresql/data]
# Mon, 12 Sep 2022 22:49:16 GMT
COPY file:232dce6cf487afb0c0cc43d38932ff29614a74b57cd04557dc7398e6d2b93b8f in /usr/local/bin/ 
# Mon, 12 Sep 2022 22:49:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 12 Sep 2022 22:49:16 GMT
STOPSIGNAL SIGINT
# Mon, 12 Sep 2022 22:49:16 GMT
EXPOSE 5432
# Mon, 12 Sep 2022 22:49:16 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85c3ef7cf9a6beeec8ff5b757e39ad71347ec77e891ad4d7784b14019583b223`  
		Last Modified: Tue, 09 Aug 2022 23:30:37 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac29cc04759ac7a5bf2b2df30b2272ec2eddee0feb4eedd6b50afe7056c3194b`  
		Last Modified: Tue, 09 Aug 2022 23:30:38 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1950f9c3a969767b204eb4bd4e6b5f1e43ec724df884562373c62119b6709a60`  
		Last Modified: Mon, 12 Sep 2022 22:51:00 GMT  
		Size: 82.5 MB (82524538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:999e28db1dcd20dae056985ad65da3aa9599f356003697459db8e7431dabfb4d`  
		Last Modified: Mon, 12 Sep 2022 22:50:50 GMT  
		Size: 9.5 KB (9465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec5d470746e094fd03d6a44c65e17009cc1a32f280560e96452b1eacdf37a691`  
		Last Modified: Mon, 12 Sep 2022 22:50:50 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4639ff61ae283ddd8dc4c7bdb7b5b0a7e0ce44015d3529cc9d227eae68bb9301`  
		Last Modified: Mon, 12 Sep 2022 22:50:50 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:838e9dccfaa3d5e11ca204ad905069f45c622b662713dfbe1950a4f7117b9734`  
		Last Modified: Mon, 12 Sep 2022 22:50:50 GMT  
		Size: 4.7 KB (4703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:15beta4-alpine` - linux; arm variant v6

```console
$ docker pull postgres@sha256:963f868c1dbdaac45f319dc6a29f9d0044c619ff0e5beaf17727339b972b9f2c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **83.5 MB (83468146 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b49a94d056e7e27e718653344099c645fba5d87ee612e60d0ff2ddd282c5ae76`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:22 GMT
ADD file:e8733e8cc0a81e15ca4041760b6e27392c34171512d34405a9b262b1fff5c687 in / 
# Tue, 09 Aug 2022 17:49:22 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 16:32:48 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Wed, 10 Aug 2022 16:32:48 GMT
ENV LANG=en_US.utf8
# Wed, 10 Aug 2022 16:32:49 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 10 Aug 2022 16:32:49 GMT
ENV PG_MAJOR=15
# Tue, 13 Sep 2022 01:07:07 GMT
ENV PG_VERSION=15beta4
# Tue, 13 Sep 2022 01:07:08 GMT
ENV PG_SHA256=d84d18ef26a64e76f189b7efb05179920eb0e8ae5d68cdbdbbe966305aee4416
# Tue, 13 Sep 2022 01:18:58 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm-dev clang g++ 		make 		openldap-dev 		openssl-dev 		perl-dev 		perl-ipc-run 		perl-utils 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		icu-dev 		lz4-dev 		zstd-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-krb5 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 		--with-lz4 		--with-zstd 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 		zstd 		icu-data-full 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Tue, 13 Sep 2022 01:18:59 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample
# Tue, 13 Sep 2022 01:18:59 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 13 Sep 2022 01:19:00 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 13 Sep 2022 01:19:00 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 13 Sep 2022 01:19:00 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 13 Sep 2022 01:19:00 GMT
COPY file:232dce6cf487afb0c0cc43d38932ff29614a74b57cd04557dc7398e6d2b93b8f in /usr/local/bin/ 
# Tue, 13 Sep 2022 01:19:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Sep 2022 01:19:01 GMT
STOPSIGNAL SIGINT
# Tue, 13 Sep 2022 01:19:01 GMT
EXPOSE 5432
# Tue, 13 Sep 2022 01:19:01 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:9506b835437abb4d8ba1683e00c500b8f77e1975e930b356fbb72f2dbdc274d9`  
		Last Modified: Tue, 09 Aug 2022 17:50:33 GMT  
		Size: 2.6 MB (2613965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2041638875c51a479e6eebba8c0987b5ffc3afbb9ae0e025c925dae805209f8`  
		Last Modified: Wed, 10 Aug 2022 17:36:09 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6486fdaa1c6892370bf2f055a3d2aab714affd6d377828de930664fb1ba8358`  
		Last Modified: Wed, 10 Aug 2022 17:36:09 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cfaf2fdc8742977f5578c5022be945bc11c824e19b43062ed2a7995cf5c520c`  
		Last Modified: Tue, 13 Sep 2022 01:21:03 GMT  
		Size: 80.8 MB (80838217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:704c24825effffcb0965e03fdd5372d2ef98f41ec452465e4256b7e816781132`  
		Last Modified: Tue, 13 Sep 2022 01:20:42 GMT  
		Size: 9.5 KB (9470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd0307314439bc47497f606c3e245ea8985d696b0bc18a8992669cde7a597271`  
		Last Modified: Tue, 13 Sep 2022 01:20:42 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00a6136b064ce923b4d05987db8a06bec9df70af5492af917cf6ae34ba3960ae`  
		Last Modified: Tue, 13 Sep 2022 01:20:42 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8a9092631c31690a50cd4d7ca8bbda9bc87c22a7908f37c2fcb342b8184d6b2`  
		Last Modified: Tue, 13 Sep 2022 01:20:42 GMT  
		Size: 4.7 KB (4704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:15beta4-alpine` - linux; arm variant v7

```console
$ docker pull postgres@sha256:c486cb734d7338e4ffc5d8140d9ff65460b6cc1a10a758e52bce7358ef3af944
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **78.6 MB (78562544 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a57655a5fc4ba16a7260896df1c626dcaf25109285925cfd6611e9fee10ce12`
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
# Mon, 12 Sep 2022 22:14:45 GMT
ENV PG_VERSION=15beta4
# Mon, 12 Sep 2022 22:14:45 GMT
ENV PG_SHA256=d84d18ef26a64e76f189b7efb05179920eb0e8ae5d68cdbdbbe966305aee4416
# Mon, 12 Sep 2022 22:21:19 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm-dev clang g++ 		make 		openldap-dev 		openssl-dev 		perl-dev 		perl-ipc-run 		perl-utils 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		icu-dev 		lz4-dev 		zstd-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-krb5 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 		--with-lz4 		--with-zstd 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 		zstd 		icu-data-full 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Mon, 12 Sep 2022 22:21:20 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample
# Mon, 12 Sep 2022 22:21:21 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Mon, 12 Sep 2022 22:21:21 GMT
ENV PGDATA=/var/lib/postgresql/data
# Mon, 12 Sep 2022 22:21:21 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Mon, 12 Sep 2022 22:21:21 GMT
VOLUME [/var/lib/postgresql/data]
# Mon, 12 Sep 2022 22:21:21 GMT
COPY file:232dce6cf487afb0c0cc43d38932ff29614a74b57cd04557dc7398e6d2b93b8f in /usr/local/bin/ 
# Mon, 12 Sep 2022 22:21:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 12 Sep 2022 22:21:21 GMT
STOPSIGNAL SIGINT
# Mon, 12 Sep 2022 22:21:22 GMT
EXPOSE 5432
# Mon, 12 Sep 2022 22:21:22 GMT
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
	-	`sha256:f36d07182de39b98e593b23723b4a5cb4a9e53348da8e35c6333b19e63c5b871`  
		Last Modified: Mon, 12 Sep 2022 22:24:45 GMT  
		Size: 76.1 MB (76129514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90ab79d433f7271a9d948db8e79348f82f4a0d87a59cec38009cd0e7e4669199`  
		Last Modified: Mon, 12 Sep 2022 22:24:36 GMT  
		Size: 9.5 KB (9469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59662b1a6fabd8f5cc5abe1d9e99997958540c541ab211dba1b5badbf01a1c52`  
		Last Modified: Mon, 12 Sep 2022 22:24:36 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e29d1e5c322aafed075588f456905d3fd1a1e5c0e2c3f3d8ba77b5e65415f957`  
		Last Modified: Mon, 12 Sep 2022 22:24:35 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95980eb3b3b6b7a750037126f0c520b3d17c4c11a973b52b95b116e172347cc0`  
		Last Modified: Mon, 12 Sep 2022 22:24:36 GMT  
		Size: 4.7 KB (4705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:15beta4-alpine` - linux; arm64 variant v8

```console
$ docker pull postgres@sha256:bed1a697a46d2be1766f4e90f260e8c728d65141ea3047302ad7a3abed769e1f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.2 MB (84186135 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d027751601fd24d8dc183c51ba13c289365d05321872e127c28c39851a12bed`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Tue, 09 Aug 2022 17:39:42 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 02:26:39 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Wed, 10 Aug 2022 02:26:40 GMT
ENV LANG=en_US.utf8
# Wed, 10 Aug 2022 02:26:41 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 10 Aug 2022 02:26:42 GMT
ENV PG_MAJOR=15
# Mon, 12 Sep 2022 23:26:11 GMT
ENV PG_VERSION=15beta4
# Mon, 12 Sep 2022 23:26:12 GMT
ENV PG_SHA256=d84d18ef26a64e76f189b7efb05179920eb0e8ae5d68cdbdbbe966305aee4416
# Mon, 12 Sep 2022 23:29:39 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm-dev clang g++ 		make 		openldap-dev 		openssl-dev 		perl-dev 		perl-ipc-run 		perl-utils 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		icu-dev 		lz4-dev 		zstd-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-krb5 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 		--with-lz4 		--with-zstd 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 		zstd 		icu-data-full 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Mon, 12 Sep 2022 23:29:40 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample
# Mon, 12 Sep 2022 23:29:41 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Mon, 12 Sep 2022 23:29:42 GMT
ENV PGDATA=/var/lib/postgresql/data
# Mon, 12 Sep 2022 23:29:43 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Mon, 12 Sep 2022 23:29:44 GMT
VOLUME [/var/lib/postgresql/data]
# Mon, 12 Sep 2022 23:29:46 GMT
COPY file:232dce6cf487afb0c0cc43d38932ff29614a74b57cd04557dc7398e6d2b93b8f in /usr/local/bin/ 
# Mon, 12 Sep 2022 23:29:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 12 Sep 2022 23:29:47 GMT
STOPSIGNAL SIGINT
# Mon, 12 Sep 2022 23:29:48 GMT
EXPOSE 5432
# Mon, 12 Sep 2022 23:29:49 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75aada9edfc58771473e8896a13640c97ada8da22ee2296fb12338c45d0ab8d7`  
		Last Modified: Wed, 10 Aug 2022 02:49:40 GMT  
		Size: 1.3 KB (1255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8207736937506f07b9ceed008216a1acbd1e12c8e770a48463266154eea5a296`  
		Last Modified: Wed, 10 Aug 2022 02:49:39 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:170807296ce68ea980120556b586c3e10939fcb788888b47415355ba9273203c`  
		Last Modified: Mon, 12 Sep 2022 23:32:35 GMT  
		Size: 81.5 MB (81462631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7e7e2130eccaf2ae1f00bb770bcff9ec8ce316f95ca8c4a4cdfd3fd1a6316cf`  
		Last Modified: Mon, 12 Sep 2022 23:32:24 GMT  
		Size: 9.5 KB (9466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc6e0dc7a87fae679697315132a2c0d71feab8a028c73b759c2a6dc5fe14b877`  
		Last Modified: Mon, 12 Sep 2022 23:32:24 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f763c220a2a9cd96e5bbb877ad4ef4e8eb3819a7fb523512418b52593b78290e`  
		Last Modified: Mon, 12 Sep 2022 23:32:24 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29fac81c5ad3fcb1d8afd6c1005db6e1d4f6a78c8a792ca32b2a135053beb5bd`  
		Last Modified: Mon, 12 Sep 2022 23:32:24 GMT  
		Size: 4.7 KB (4704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:15beta4-alpine` - linux; 386

```console
$ docker pull postgres@sha256:3ee140ae255d0d2729b7ff8fe7b14ec16d3d436cb7f05711ad9713f350f5b0ee
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **90.7 MB (90689725 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:85f0f56037af96ddcd26573f8de007acb1467f6770fb7d019678dec0e12f591e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 09 Aug 2022 17:38:39 GMT
ADD file:b828bc14bc5ff03c8f7310fe0aed6ac5df19a393622d5d1d779a523234d07c0a in / 
# Tue, 09 Aug 2022 17:38:39 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 20:53:15 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Tue, 09 Aug 2022 20:53:16 GMT
ENV LANG=en_US.utf8
# Tue, 09 Aug 2022 20:53:17 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 09 Aug 2022 20:53:18 GMT
ENV PG_MAJOR=15
# Mon, 12 Sep 2022 23:00:30 GMT
ENV PG_VERSION=15beta4
# Mon, 12 Sep 2022 23:00:31 GMT
ENV PG_SHA256=d84d18ef26a64e76f189b7efb05179920eb0e8ae5d68cdbdbbe966305aee4416
# Mon, 12 Sep 2022 23:04:26 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm-dev clang g++ 		make 		openldap-dev 		openssl-dev 		perl-dev 		perl-ipc-run 		perl-utils 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		icu-dev 		lz4-dev 		zstd-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-krb5 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 		--with-lz4 		--with-zstd 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 		zstd 		icu-data-full 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Mon, 12 Sep 2022 23:04:26 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample
# Mon, 12 Sep 2022 23:04:27 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Mon, 12 Sep 2022 23:04:28 GMT
ENV PGDATA=/var/lib/postgresql/data
# Mon, 12 Sep 2022 23:04:29 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Mon, 12 Sep 2022 23:04:30 GMT
VOLUME [/var/lib/postgresql/data]
# Mon, 12 Sep 2022 23:04:32 GMT
COPY file:232dce6cf487afb0c0cc43d38932ff29614a74b57cd04557dc7398e6d2b93b8f in /usr/local/bin/ 
# Mon, 12 Sep 2022 23:04:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 12 Sep 2022 23:04:33 GMT
STOPSIGNAL SIGINT
# Mon, 12 Sep 2022 23:04:34 GMT
EXPOSE 5432
# Mon, 12 Sep 2022 23:04:35 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:6c0d3b419d848ea31ca748254611d5d5ce3b76e3d7bba520fd87400fbb75f3b9`  
		Last Modified: Tue, 09 Aug 2022 17:39:33 GMT  
		Size: 2.8 MB (2807121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08c28e75c4cf92ef72dba94a55ce482cf503fbc49400e209e8c7f918c4c3b738`  
		Last Modified: Tue, 09 Aug 2022 21:18:35 GMT  
		Size: 1.3 KB (1255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ec2f418c543a35f5a9bd4622f8333170308c8bfc39d60776c46f8cd414f6218`  
		Last Modified: Tue, 09 Aug 2022 21:18:35 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c601a67746c6c14c946cdb4105e7bf19fdac9926130072578da7c8e8567b44f4`  
		Last Modified: Mon, 12 Sep 2022 23:07:31 GMT  
		Size: 87.9 MB (87866761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fecf15b2a2fb865a2909406b967447c88c1dbb3cc4cbb751b5bba152db52e6b7`  
		Last Modified: Mon, 12 Sep 2022 23:07:20 GMT  
		Size: 9.5 KB (9470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1068a9a6441e2bb08ceb6df212f8a5f3664d41c0931a59546d64190331138e17`  
		Last Modified: Mon, 12 Sep 2022 23:07:20 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d236cc05eb83e1b32738858f522976688ff91887f155c9cdd4242d002f33ac6b`  
		Last Modified: Mon, 12 Sep 2022 23:07:20 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51d57eb81aaad31b505843361004c0bb72161efd4151b7f188656a7d7fd75288`  
		Last Modified: Mon, 12 Sep 2022 23:07:20 GMT  
		Size: 4.7 KB (4701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:15beta4-alpine` - linux; s390x

```console
$ docker pull postgres@sha256:d2010726634164262da2bb5a61291304a664e505f9d717d5ef8c85df22385aa6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **86.6 MB (86555642 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f130c4a755e697df9ab495e496cd556b2142f840adeb5b0c6fd6ca7b11fe92ef`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 09 Aug 2022 17:41:46 GMT
ADD file:b43a065471bc4711415d3c67cd5b6559b0c48ee7ffe9761530477cf457a6dc34 in / 
# Tue, 09 Aug 2022 17:41:46 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 02:38:11 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Wed, 10 Aug 2022 02:38:12 GMT
ENV LANG=en_US.utf8
# Wed, 10 Aug 2022 02:38:12 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 10 Aug 2022 02:38:13 GMT
ENV PG_MAJOR=15
# Mon, 12 Sep 2022 22:59:31 GMT
ENV PG_VERSION=15beta4
# Mon, 12 Sep 2022 22:59:31 GMT
ENV PG_SHA256=d84d18ef26a64e76f189b7efb05179920eb0e8ae5d68cdbdbbe966305aee4416
# Mon, 12 Sep 2022 23:02:44 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm-dev clang g++ 		make 		openldap-dev 		openssl-dev 		perl-dev 		perl-ipc-run 		perl-utils 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		icu-dev 		lz4-dev 		zstd-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-krb5 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 		--with-lz4 		--with-zstd 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 		zstd 		icu-data-full 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Mon, 12 Sep 2022 23:02:51 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample
# Mon, 12 Sep 2022 23:02:52 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Mon, 12 Sep 2022 23:02:52 GMT
ENV PGDATA=/var/lib/postgresql/data
# Mon, 12 Sep 2022 23:02:53 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Mon, 12 Sep 2022 23:02:53 GMT
VOLUME [/var/lib/postgresql/data]
# Mon, 12 Sep 2022 23:02:53 GMT
COPY file:232dce6cf487afb0c0cc43d38932ff29614a74b57cd04557dc7398e6d2b93b8f in /usr/local/bin/ 
# Mon, 12 Sep 2022 23:02:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 12 Sep 2022 23:02:54 GMT
STOPSIGNAL SIGINT
# Mon, 12 Sep 2022 23:02:54 GMT
EXPOSE 5432
# Mon, 12 Sep 2022 23:02:54 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:790c84f1f3409eab952345157df7fa804ba6b5f06d4ceb6f2dfa3c6de2064397`  
		Last Modified: Tue, 09 Aug 2022 17:42:45 GMT  
		Size: 2.6 MB (2590597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e37954570c3339ca3dbd0ab6914f9cc51c3e566c430fccfcf138af422bec41fb`  
		Last Modified: Wed, 10 Aug 2022 03:08:51 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fb11cf4d23618d019e95519ca11f8b63235cbb4e6ce8e456c44b98728c74962`  
		Last Modified: Wed, 10 Aug 2022 03:08:51 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:288d278ef3457dfbd9f472536d248db2a4e5a8f7767ae0cb519b5758819b1483`  
		Last Modified: Mon, 12 Sep 2022 23:15:36 GMT  
		Size: 83.9 MB (83949090 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8991ac5cbf8b5a9b225decfd4d7748de73e87a2d1c78416c6db251a146ec48f9`  
		Last Modified: Mon, 12 Sep 2022 23:15:27 GMT  
		Size: 9.5 KB (9465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:555266da95cc3bdbf6b6e887c1e35db721ac264576a0fba6a895c8a73566cdc2`  
		Last Modified: Mon, 12 Sep 2022 23:15:27 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29ad2115d63b99c4aeafec98a2e65530add699b1397f162a3530f00e6902cd73`  
		Last Modified: Mon, 12 Sep 2022 23:15:27 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fd8f7467ed5c9cb28ef2420724f6d3abf7e6ccb00e27637c8d1470c2b8c2f15`  
		Last Modified: Mon, 12 Sep 2022 23:15:27 GMT  
		Size: 4.7 KB (4701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
