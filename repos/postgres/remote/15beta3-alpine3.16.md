## `postgres:15beta3-alpine3.16`

```console
$ docker pull postgres@sha256:4742237cd17bd1ea9735ec4df216da2795622b142e06c84ea5a0aeb2f788d77d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; s390x

### `postgres:15beta3-alpine3.16` - linux; amd64

```console
$ docker pull postgres@sha256:7a5a0ffe97e3fa2009878f2f726c453568b1ff696d7fc2c486fa711530d93d40
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **85.5 MB (85542970 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:951bea73383bd8ba97f6cd9c314489eca26a196f282b18914502afb8e0134642`
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
# Fri, 12 Aug 2022 00:40:12 GMT
ENV PG_VERSION=15beta3
# Fri, 12 Aug 2022 00:40:13 GMT
ENV PG_SHA256=1a6e2a454b6bcdf76aa4e50573d2fa1ea8db2cdfaa3282a7538830bd285b27bf
# Fri, 12 Aug 2022 00:43:37 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm-dev clang g++ 		make 		openldap-dev 		openssl-dev 		perl-dev 		perl-ipc-run 		perl-utils 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		icu-dev 		lz4-dev 		zstd-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-krb5 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 		--with-lz4 		--with-zstd 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 		zstd 		icu-data-full 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Fri, 12 Aug 2022 00:43:38 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample
# Fri, 12 Aug 2022 00:43:39 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 12 Aug 2022 00:43:39 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 12 Aug 2022 00:43:39 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 12 Aug 2022 00:43:40 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 12 Aug 2022 00:43:40 GMT
COPY file:232dce6cf487afb0c0cc43d38932ff29614a74b57cd04557dc7398e6d2b93b8f in /usr/local/bin/ 
# Fri, 12 Aug 2022 00:43:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 12 Aug 2022 00:43:40 GMT
STOPSIGNAL SIGINT
# Fri, 12 Aug 2022 00:43:40 GMT
EXPOSE 5432
# Fri, 12 Aug 2022 00:43:40 GMT
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
	-	`sha256:334a2c4c22bef1417b5082ae639868f152d943c63ec503cbbec2d4e8d7add74f`  
		Last Modified: Fri, 12 Aug 2022 01:03:15 GMT  
		Size: 82.7 MB (82720959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dd531788ea938370b6a44cc18194e68575525efd729965074314287bf0c3a21`  
		Last Modified: Fri, 12 Aug 2022 01:03:04 GMT  
		Size: 9.5 KB (9465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93ee0a3ec73cdbdf15549f0b87c18fb4bccaeed508c8ac485e3456d30bf5d21f`  
		Last Modified: Fri, 12 Aug 2022 01:03:04 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eafb37abaebe29b363fdb16c066fd4462d100b8dd6ca18913edd268b9eb8259b`  
		Last Modified: Fri, 12 Aug 2022 01:03:04 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd4715dc84454e154ab30f2848bd471fc10f12de5533b2ea2a460c1eb5b7c5e3`  
		Last Modified: Fri, 12 Aug 2022 01:03:04 GMT  
		Size: 4.7 KB (4702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:15beta3-alpine3.16` - linux; arm variant v6

```console
$ docker pull postgres@sha256:0dbadb7fa838ed6a62cd236a1418f3d4292fbd3aed48b0b515ecf15a4ecb6229
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **83.7 MB (83671210 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:67d7054dad190bfe512a263349ef703268dfc4ee26a7d1fc41ee2cbadc05506f`
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
# Fri, 12 Aug 2022 00:19:04 GMT
ENV PG_VERSION=15beta3
# Fri, 12 Aug 2022 00:19:04 GMT
ENV PG_SHA256=1a6e2a454b6bcdf76aa4e50573d2fa1ea8db2cdfaa3282a7538830bd285b27bf
# Fri, 12 Aug 2022 00:36:12 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm-dev clang g++ 		make 		openldap-dev 		openssl-dev 		perl-dev 		perl-ipc-run 		perl-utils 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		icu-dev 		lz4-dev 		zstd-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-krb5 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 		--with-lz4 		--with-zstd 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 		zstd 		icu-data-full 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Fri, 12 Aug 2022 00:36:13 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample
# Fri, 12 Aug 2022 00:36:14 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 12 Aug 2022 00:36:14 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 12 Aug 2022 00:36:15 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 12 Aug 2022 00:36:15 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 12 Aug 2022 00:36:15 GMT
COPY file:232dce6cf487afb0c0cc43d38932ff29614a74b57cd04557dc7398e6d2b93b8f in /usr/local/bin/ 
# Fri, 12 Aug 2022 00:36:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 12 Aug 2022 00:36:16 GMT
STOPSIGNAL SIGINT
# Fri, 12 Aug 2022 00:36:16 GMT
EXPOSE 5432
# Fri, 12 Aug 2022 00:36:16 GMT
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
	-	`sha256:091d175d1cd0edbd8099dc26a67044425b96b729982fd834dbba2345dc9c31b8`  
		Last Modified: Fri, 12 Aug 2022 01:51:47 GMT  
		Size: 81.0 MB (81041280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c091334539b24057a5a026a4bf8ee120c47eeb84ad85aef23b3f048eda266b0`  
		Last Modified: Fri, 12 Aug 2022 01:51:23 GMT  
		Size: 9.5 KB (9466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16f23131ece3b1934a9dfae49e77cbe661a1feca28a0dca587e98a750d2b14fc`  
		Last Modified: Fri, 12 Aug 2022 01:51:23 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d01afe29add55c434e529e81a4c20311c7b0a4ccafad9cee27b981917da147db`  
		Last Modified: Fri, 12 Aug 2022 01:51:23 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e813461f6452e75d1dadf39b134f42f1570c9087aee81cc9f80344c97a64309`  
		Last Modified: Fri, 12 Aug 2022 01:51:23 GMT  
		Size: 4.7 KB (4708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:15beta3-alpine3.16` - linux; arm64 variant v8

```console
$ docker pull postgres@sha256:c7d3be7fa9419a4ee045427454b4422fc1d1e1eab4765a6cf35de1994a69765c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.4 MB (84379997 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:48f8fd75aa2fbf355ac8516b4a3961240c6a82740a9be8a377633bd7114b9f70`
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
# Thu, 11 Aug 2022 23:47:45 GMT
ENV PG_VERSION=15beta3
# Thu, 11 Aug 2022 23:47:46 GMT
ENV PG_SHA256=1a6e2a454b6bcdf76aa4e50573d2fa1ea8db2cdfaa3282a7538830bd285b27bf
# Thu, 11 Aug 2022 23:51:18 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm-dev clang g++ 		make 		openldap-dev 		openssl-dev 		perl-dev 		perl-ipc-run 		perl-utils 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		icu-dev 		lz4-dev 		zstd-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-krb5 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 		--with-lz4 		--with-zstd 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 		zstd 		icu-data-full 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Thu, 11 Aug 2022 23:51:19 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample
# Thu, 11 Aug 2022 23:51:20 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 11 Aug 2022 23:51:21 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 11 Aug 2022 23:51:22 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 11 Aug 2022 23:51:23 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 11 Aug 2022 23:51:25 GMT
COPY file:232dce6cf487afb0c0cc43d38932ff29614a74b57cd04557dc7398e6d2b93b8f in /usr/local/bin/ 
# Thu, 11 Aug 2022 23:51:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 11 Aug 2022 23:51:26 GMT
STOPSIGNAL SIGINT
# Thu, 11 Aug 2022 23:51:27 GMT
EXPOSE 5432
# Thu, 11 Aug 2022 23:51:28 GMT
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
	-	`sha256:76da40a90edf77ec2b06e08547ec77b865950d03924d5d761ab25bf61491c774`  
		Last Modified: Fri, 12 Aug 2022 00:13:31 GMT  
		Size: 81.7 MB (81656498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57f534f62a061a38dbefc530f1b366c9f41a8d9aad3d2f01bbaae2495c021c85`  
		Last Modified: Fri, 12 Aug 2022 00:13:20 GMT  
		Size: 9.5 KB (9464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4aca7edd1d6378f8b8e056b70ae9dc6aec17d0d825bffb7f747360d0fca73275`  
		Last Modified: Fri, 12 Aug 2022 00:13:20 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aa3798e7c3f716c259220617c653f00e63594c1e52bd911907a04805e83b952`  
		Last Modified: Fri, 12 Aug 2022 00:13:20 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1cf39226911bf39fdf8e159ada13fb0e636adeb2d1178c04ab9fbc49a6c1a70`  
		Last Modified: Fri, 12 Aug 2022 00:13:20 GMT  
		Size: 4.7 KB (4700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:15beta3-alpine3.16` - linux; 386

```console
$ docker pull postgres@sha256:ffa87c1a3285b37e67fae0c496b8f33242d8696ebee8263aac553ef84646345f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **90.9 MB (90899694 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f76854cdbbcbbe779d28aaa64a7f71e19a440d2904f72d1d06fabfd90a424d7`
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
# Thu, 11 Aug 2022 23:52:58 GMT
ENV PG_VERSION=15beta3
# Thu, 11 Aug 2022 23:52:59 GMT
ENV PG_SHA256=1a6e2a454b6bcdf76aa4e50573d2fa1ea8db2cdfaa3282a7538830bd285b27bf
# Thu, 11 Aug 2022 23:56:58 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm-dev clang g++ 		make 		openldap-dev 		openssl-dev 		perl-dev 		perl-ipc-run 		perl-utils 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		icu-dev 		lz4-dev 		zstd-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-krb5 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 		--with-lz4 		--with-zstd 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 		zstd 		icu-data-full 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Thu, 11 Aug 2022 23:56:59 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample
# Thu, 11 Aug 2022 23:57:00 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 11 Aug 2022 23:57:01 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 11 Aug 2022 23:57:02 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 11 Aug 2022 23:57:03 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 11 Aug 2022 23:57:05 GMT
COPY file:232dce6cf487afb0c0cc43d38932ff29614a74b57cd04557dc7398e6d2b93b8f in /usr/local/bin/ 
# Thu, 11 Aug 2022 23:57:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 11 Aug 2022 23:57:06 GMT
STOPSIGNAL SIGINT
# Thu, 11 Aug 2022 23:57:07 GMT
EXPOSE 5432
# Thu, 11 Aug 2022 23:57:08 GMT
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
	-	`sha256:60e226f19c5769d1252c450125a6b9aeae1c1bfde1bac1053b45c176f4346c0d`  
		Last Modified: Fri, 12 Aug 2022 01:19:17 GMT  
		Size: 88.1 MB (88076736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b54eda76641a885d37a540062fbf9939f6bef0c4783f85c72d31fd98c14bcb39`  
		Last Modified: Fri, 12 Aug 2022 01:19:06 GMT  
		Size: 9.5 KB (9464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86c2a2eeb9d654072ce26385c49123f8befe4bc314c6956325d7fa7c55899e6e`  
		Last Modified: Fri, 12 Aug 2022 01:19:06 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5eb60014eacfb1cb272b74d47594701b66abb0f578ea91f8e97fb2cb66ebea6`  
		Last Modified: Fri, 12 Aug 2022 01:19:07 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:579000a3464d9159e80bef3e43712716244c8a1fc4c3f0885bb10f73dfdd371f`  
		Last Modified: Fri, 12 Aug 2022 01:19:07 GMT  
		Size: 4.7 KB (4701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:15beta3-alpine3.16` - linux; s390x

```console
$ docker pull postgres@sha256:75197cd2d2bde99ece78fd4707048125193ec0801a663da016c20e084fb4fcd1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **86.8 MB (86778577 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:24725f803a4be8371a9d483d60c98dde6212036f68b169c0bd93906a350d6301`
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
# Thu, 11 Aug 2022 23:49:26 GMT
ENV PG_VERSION=15beta3
# Thu, 11 Aug 2022 23:49:26 GMT
ENV PG_SHA256=1a6e2a454b6bcdf76aa4e50573d2fa1ea8db2cdfaa3282a7538830bd285b27bf
# Thu, 11 Aug 2022 23:52:35 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm-dev clang g++ 		make 		openldap-dev 		openssl-dev 		perl-dev 		perl-ipc-run 		perl-utils 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		icu-dev 		lz4-dev 		zstd-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-krb5 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 		--with-lz4 		--with-zstd 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 		zstd 		icu-data-full 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Thu, 11 Aug 2022 23:52:38 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample
# Thu, 11 Aug 2022 23:52:39 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 11 Aug 2022 23:52:39 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 11 Aug 2022 23:52:39 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 11 Aug 2022 23:52:39 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 11 Aug 2022 23:52:39 GMT
COPY file:232dce6cf487afb0c0cc43d38932ff29614a74b57cd04557dc7398e6d2b93b8f in /usr/local/bin/ 
# Thu, 11 Aug 2022 23:52:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 11 Aug 2022 23:52:40 GMT
STOPSIGNAL SIGINT
# Thu, 11 Aug 2022 23:52:40 GMT
EXPOSE 5432
# Thu, 11 Aug 2022 23:52:40 GMT
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
	-	`sha256:c84724c05c5479f0d4257b3a8a0073dbf42c39a6ff90d5b6337f10f9992a297e`  
		Last Modified: Fri, 12 Aug 2022 01:05:27 GMT  
		Size: 84.2 MB (84172026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:661835f05f67bc2a6bb386115b59779ac5cf0514a0b5d7b10b75910711603eba`  
		Last Modified: Fri, 12 Aug 2022 01:05:17 GMT  
		Size: 9.5 KB (9463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebf61b50e59eb2096d1e451570924b24009c6497f365a557565b0b2e19426534`  
		Last Modified: Fri, 12 Aug 2022 01:05:17 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b35219d0a6908368397b78e872f45bd5ba55ceaf78861e75c419eb7e13e33fb9`  
		Last Modified: Fri, 12 Aug 2022 01:05:17 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d06ae97dedbad5363ede08c67f9a8683394d056141e71d095ac7a8bb78c18d5a`  
		Last Modified: Fri, 12 Aug 2022 01:05:17 GMT  
		Size: 4.7 KB (4703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
