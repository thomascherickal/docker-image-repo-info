## `postgres:14-alpine3.15`

```console
$ docker pull postgres@sha256:fe1c5562ba5e7e79efd4b8f2fce4454d4bfe9420a3ef6804119c3fc1144dddba
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

### `postgres:14-alpine3.15` - linux; amd64

```console
$ docker pull postgres@sha256:6d6308441b7d1e3cfc2ac86f6b2b1f6d7bd290fb6d38e565fabb4ffb280b63d9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.8 MB (81822585 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4133e917a82d9442795494de700670f7626a3b15008abfbb5f9d8023544420d4`
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
# Wed, 23 Mar 2022 18:10:32 GMT
ENV PG_MAJOR=14
# Wed, 23 Mar 2022 18:10:32 GMT
ENV PG_VERSION=14.2
# Wed, 23 Mar 2022 18:10:32 GMT
ENV PG_SHA256=2cf78b2e468912f8101d695db5340cf313c2e9f68a612fb71427524e8c9a977a
# Wed, 23 Mar 2022 18:15:36 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm-dev clang g++ 		make 		openldap-dev 		openssl-dev 		perl-dev 		perl-ipc-run 		perl-utils 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		zstd 		icu-dev 		lz4-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-krb5 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 		--with-lz4 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Wed, 23 Mar 2022 18:15:37 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample
# Wed, 23 Mar 2022 18:15:37 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Wed, 23 Mar 2022 18:15:37 GMT
ENV PGDATA=/var/lib/postgresql/data
# Wed, 23 Mar 2022 18:15:38 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Wed, 23 Mar 2022 18:15:38 GMT
VOLUME [/var/lib/postgresql/data]
# Wed, 23 Mar 2022 18:15:38 GMT
COPY file:e8928645623137de410cce68a2aa3b22f07a64e6391025598a60f3e461c606a3 in /usr/local/bin/ 
# Wed, 23 Mar 2022 18:15:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 23 Mar 2022 18:15:38 GMT
STOPSIGNAL SIGINT
# Wed, 23 Mar 2022 18:15:38 GMT
EXPOSE 5432
# Wed, 23 Mar 2022 18:15:38 GMT
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
	-	`sha256:57d3903eeac00ece26e0cfccc0279cf988f33613f3903b333340d236ab38d538`  
		Last Modified: Wed, 23 Mar 2022 18:36:20 GMT  
		Size: 79.0 MB (78994207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58fc8cab17b31b55f16c7ed2042d42770cb4f9544ff08c2192b53cc922577304`  
		Last Modified: Wed, 23 Mar 2022 18:36:09 GMT  
		Size: 9.2 KB (9209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:800a0137a38c9f916ee2fb937a427170b0cec5958209f9b3ce03d1364e761f40`  
		Last Modified: Wed, 23 Mar 2022 18:36:09 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2fc2df72960281a7b932bb6b14ebe52b8e2fd3ca7bc8fbf4c5570bea081e79c`  
		Last Modified: Wed, 23 Mar 2022 18:36:09 GMT  
		Size: 192.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10e3eb856b87b58385554cbb5fcd22835585e1926f6a52bfb3a7bbc7d7c3732c`  
		Last Modified: Wed, 23 Mar 2022 18:36:09 GMT  
		Size: 4.7 KB (4698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:14-alpine3.15` - linux; arm variant v6

```console
$ docker pull postgres@sha256:3ec83a482a07403a58338bc063b09c6693a15dea9e88d70c8637336b62224ec4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **80.2 MB (80234861 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:32a0fb018738674b1247443b3909c8624d51c7246a3f670c4df3ad0403908508`
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
# Wed, 23 Mar 2022 23:21:10 GMT
ENV PG_MAJOR=14
# Wed, 23 Mar 2022 23:21:10 GMT
ENV PG_VERSION=14.2
# Wed, 23 Mar 2022 23:21:11 GMT
ENV PG_SHA256=2cf78b2e468912f8101d695db5340cf313c2e9f68a612fb71427524e8c9a977a
# Tue, 29 Mar 2022 00:00:20 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm-dev clang g++ 		make 		openldap-dev 		openssl-dev 		perl-dev 		perl-ipc-run 		perl-utils 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		icu-dev 		lz4-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-krb5 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 		--with-lz4 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 		zstd 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Tue, 29 Mar 2022 00:00:22 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample
# Tue, 29 Mar 2022 00:00:23 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 29 Mar 2022 00:00:24 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 29 Mar 2022 00:00:25 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 29 Mar 2022 00:00:26 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 29 Mar 2022 00:00:26 GMT
COPY file:e8928645623137de410cce68a2aa3b22f07a64e6391025598a60f3e461c606a3 in /usr/local/bin/ 
# Tue, 29 Mar 2022 00:00:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 29 Mar 2022 00:00:27 GMT
STOPSIGNAL SIGINT
# Tue, 29 Mar 2022 00:00:27 GMT
EXPOSE 5432
# Tue, 29 Mar 2022 00:00:28 GMT
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
	-	`sha256:66372237b61be9d2aa070852e1c10d47f6777a160218837e2ed61b4181f4398f`  
		Last Modified: Tue, 29 Mar 2022 00:23:09 GMT  
		Size: 77.6 MB (77594354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d0e54e77f2eb28f837567ee05d8fb47b5c3417c3555385e98f5799b1839b760`  
		Last Modified: Tue, 29 Mar 2022 00:22:29 GMT  
		Size: 9.2 KB (9208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02312ebc57eb41e15ff990f7801c49d0ee71b53d02ff767f8c18aece11c05ea9`  
		Last Modified: Tue, 29 Mar 2022 00:22:30 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76efa35f3e96a82fbb9243b12b39298b2039fac1e55b690042286be6eb151a56`  
		Last Modified: Tue, 29 Mar 2022 00:22:29 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d224d918e5585cdadf9c46f20288fd6b8f12879892cb00213cd6eea12fbc24d9`  
		Last Modified: Tue, 29 Mar 2022 00:22:29 GMT  
		Size: 4.7 KB (4701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:14-alpine3.15` - linux; arm variant v7

```console
$ docker pull postgres@sha256:dcee41f3397e874d69aaf3bcf7eae3f13f63c2544b7d04dfc82bfba48642a376
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.5 MB (75528717 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b4ae47ef9b95e47e4ea80a1d185a7d8d10bba5a4088c10555efdab36c5008416`
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
# Wed, 23 Mar 2022 23:28:41 GMT
ENV PG_MAJOR=14
# Wed, 23 Mar 2022 23:28:42 GMT
ENV PG_VERSION=14.2
# Wed, 23 Mar 2022 23:28:42 GMT
ENV PG_SHA256=2cf78b2e468912f8101d695db5340cf313c2e9f68a612fb71427524e8c9a977a
# Tue, 29 Mar 2022 00:14:45 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm-dev clang g++ 		make 		openldap-dev 		openssl-dev 		perl-dev 		perl-ipc-run 		perl-utils 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		icu-dev 		lz4-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-krb5 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 		--with-lz4 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 		zstd 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Tue, 29 Mar 2022 00:14:47 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample
# Tue, 29 Mar 2022 00:14:49 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 29 Mar 2022 00:14:49 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 29 Mar 2022 00:14:51 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 29 Mar 2022 00:14:51 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 29 Mar 2022 00:14:52 GMT
COPY file:e8928645623137de410cce68a2aa3b22f07a64e6391025598a60f3e461c606a3 in /usr/local/bin/ 
# Tue, 29 Mar 2022 00:14:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 29 Mar 2022 00:14:53 GMT
STOPSIGNAL SIGINT
# Tue, 29 Mar 2022 00:14:53 GMT
EXPOSE 5432
# Tue, 29 Mar 2022 00:14:53 GMT
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
	-	`sha256:3e1c57102a7f9b33ea7c2414f00fa339f82b2a30b55dc94c9333f69930793a2b`  
		Last Modified: Tue, 29 Mar 2022 00:39:04 GMT  
		Size: 73.1 MB (73085959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8547c1653efaba3ed78a629a7c98fc5734c82e8d44cc6e3130f0ff0f86447e4`  
		Last Modified: Tue, 29 Mar 2022 00:38:25 GMT  
		Size: 9.2 KB (9209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7678c16b866b9da0bf540d71239e9c2d9f9025953cc52d7cd81922420b64a30a`  
		Last Modified: Tue, 29 Mar 2022 00:38:25 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed0287fca8565c142bde7753c20eab84ec1aabafa6e4cae777ab0e2c425dc181`  
		Last Modified: Tue, 29 Mar 2022 00:38:25 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:333c8348a104d3ce967256f88f7f49b484298d9ad43a460f32bf7aa5a3558c9f`  
		Last Modified: Tue, 29 Mar 2022 00:38:25 GMT  
		Size: 4.7 KB (4699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:14-alpine3.15` - linux; arm64 variant v8

```console
$ docker pull postgres@sha256:94b98458d61b787eda137625d07c3a22446e3b289cbe9254f3f11d08931ffa06
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.3 MB (81272980 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eeb792ede2247cf821267791be266536745c9493602b02be39e3cf8d1ccb7143`
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
# Thu, 24 Mar 2022 07:07:45 GMT
ENV PG_MAJOR=14
# Thu, 24 Mar 2022 07:07:46 GMT
ENV PG_VERSION=14.2
# Thu, 24 Mar 2022 07:07:47 GMT
ENV PG_SHA256=2cf78b2e468912f8101d695db5340cf313c2e9f68a612fb71427524e8c9a977a
# Mon, 28 Mar 2022 23:46:10 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm-dev clang g++ 		make 		openldap-dev 		openssl-dev 		perl-dev 		perl-ipc-run 		perl-utils 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		icu-dev 		lz4-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-krb5 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 		--with-lz4 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 		zstd 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Mon, 28 Mar 2022 23:46:11 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample
# Mon, 28 Mar 2022 23:46:11 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Mon, 28 Mar 2022 23:46:12 GMT
ENV PGDATA=/var/lib/postgresql/data
# Mon, 28 Mar 2022 23:46:13 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Mon, 28 Mar 2022 23:46:14 GMT
VOLUME [/var/lib/postgresql/data]
# Mon, 28 Mar 2022 23:46:16 GMT
COPY file:e8928645623137de410cce68a2aa3b22f07a64e6391025598a60f3e461c606a3 in /usr/local/bin/ 
# Mon, 28 Mar 2022 23:46:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 28 Mar 2022 23:46:17 GMT
STOPSIGNAL SIGINT
# Mon, 28 Mar 2022 23:46:18 GMT
EXPOSE 5432
# Mon, 28 Mar 2022 23:46:19 GMT
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
	-	`sha256:445c2cd430ec12713e0aef144aaaecf3357c15bd51221524885d16f351d8fac8`  
		Last Modified: Tue, 29 Mar 2022 00:09:14 GMT  
		Size: 78.5 MB (78542686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41d82ae99ce4a75e60987290b191f09e57cb68b6c5ca4eaf4ceb4f648f15cc03`  
		Last Modified: Tue, 29 Mar 2022 00:09:04 GMT  
		Size: 9.2 KB (9199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbb65b98c1542ed30a908d2c25820b26ab63bc2eb660bf3bc044a24a9ecab895`  
		Last Modified: Tue, 29 Mar 2022 00:09:04 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:257a2e2f54c812fd63612ce5426dd48ef2fba3b66ab6e5e67451ed1ec8394708`  
		Last Modified: Tue, 29 Mar 2022 00:09:04 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e029406de6fd0834f1f36bf1c8e01d2cbfa301086ac6a16cf67ae5f83d43af4`  
		Last Modified: Tue, 29 Mar 2022 00:09:04 GMT  
		Size: 4.7 KB (4703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:14-alpine3.15` - linux; 386

```console
$ docker pull postgres@sha256:469ae313ec5bb31f68825bae9ec873e5536c34c1bd56ea1312eb2176ad32ff27
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.3 MB (87346469 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa52a74d75682733b008e68179c357ff85ed203cbae034d4f79c09245b156d19`
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
# Wed, 23 Mar 2022 23:42:17 GMT
ENV PG_MAJOR=14
# Wed, 23 Mar 2022 23:42:18 GMT
ENV PG_VERSION=14.2
# Wed, 23 Mar 2022 23:42:19 GMT
ENV PG_SHA256=2cf78b2e468912f8101d695db5340cf313c2e9f68a612fb71427524e8c9a977a
# Mon, 28 Mar 2022 23:42:22 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm-dev clang g++ 		make 		openldap-dev 		openssl-dev 		perl-dev 		perl-ipc-run 		perl-utils 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		icu-dev 		lz4-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-krb5 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 		--with-lz4 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 		zstd 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Mon, 28 Mar 2022 23:42:22 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample
# Mon, 28 Mar 2022 23:42:23 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Mon, 28 Mar 2022 23:42:24 GMT
ENV PGDATA=/var/lib/postgresql/data
# Mon, 28 Mar 2022 23:42:25 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Mon, 28 Mar 2022 23:42:26 GMT
VOLUME [/var/lib/postgresql/data]
# Mon, 28 Mar 2022 23:42:28 GMT
COPY file:e8928645623137de410cce68a2aa3b22f07a64e6391025598a60f3e461c606a3 in /usr/local/bin/ 
# Mon, 28 Mar 2022 23:42:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 28 Mar 2022 23:42:29 GMT
STOPSIGNAL SIGINT
# Mon, 28 Mar 2022 23:42:30 GMT
EXPOSE 5432
# Mon, 28 Mar 2022 23:42:31 GMT
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
	-	`sha256:7f5cf66d1eef8714823dac3b5fc8784c308690656640a86aeb27da7bdec5a1bb`  
		Last Modified: Mon, 28 Mar 2022 23:57:45 GMT  
		Size: 84.5 MB (84509060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c5de047c174131eb5ec54bd1490952e0a07c0dd72b61ff2b26bd1a81a25880e`  
		Last Modified: Mon, 28 Mar 2022 23:57:34 GMT  
		Size: 9.2 KB (9206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cd4f7d5a1ecf1e119f3f902b5ac12bac344f52c1603bd30885c33bbd7f68c40`  
		Last Modified: Mon, 28 Mar 2022 23:57:34 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c712e930812b7d290548b0386eb8d1e1ad36c55753ed21c42590d96896717a76`  
		Last Modified: Mon, 28 Mar 2022 23:57:34 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da50fb181a9f291d83c3b610b699fa859128e9f8dcfbb84518d06f85cdec9212`  
		Last Modified: Mon, 28 Mar 2022 23:57:34 GMT  
		Size: 4.7 KB (4701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:14-alpine3.15` - linux; ppc64le

```console
$ docker pull postgres@sha256:c7fb94d925ff71ca4cedd243f26fd338124196f756d9e8b8966f2d8e50d30c9a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.2 MB (87205446 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3fcffccde51d289db86753fb4a78b9c8f9d4d39e9169d75e2e0edc00ddff383f`
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
# Wed, 23 Mar 2022 23:04:25 GMT
ENV PG_MAJOR=14
# Wed, 23 Mar 2022 23:04:28 GMT
ENV PG_VERSION=14.2
# Wed, 23 Mar 2022 23:04:41 GMT
ENV PG_SHA256=2cf78b2e468912f8101d695db5340cf313c2e9f68a612fb71427524e8c9a977a
# Wed, 23 Mar 2022 23:09:19 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm-dev clang g++ 		make 		openldap-dev 		openssl-dev 		perl-dev 		perl-ipc-run 		perl-utils 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		zstd 		icu-dev 		lz4-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-krb5 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 		--with-lz4 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Wed, 23 Mar 2022 23:09:29 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample
# Wed, 23 Mar 2022 23:09:34 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Wed, 23 Mar 2022 23:09:37 GMT
ENV PGDATA=/var/lib/postgresql/data
# Wed, 23 Mar 2022 23:09:43 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Wed, 23 Mar 2022 23:09:48 GMT
VOLUME [/var/lib/postgresql/data]
# Wed, 23 Mar 2022 23:09:50 GMT
COPY file:e8928645623137de410cce68a2aa3b22f07a64e6391025598a60f3e461c606a3 in /usr/local/bin/ 
# Wed, 23 Mar 2022 23:09:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 23 Mar 2022 23:09:58 GMT
STOPSIGNAL SIGINT
# Wed, 23 Mar 2022 23:10:03 GMT
EXPOSE 5432
# Wed, 23 Mar 2022 23:10:07 GMT
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
	-	`sha256:fff623461d9ef9f730f36b1d5c9b466da0655f1ad9df769096c05b7019f71e4a`  
		Last Modified: Wed, 23 Mar 2022 23:34:52 GMT  
		Size: 84.4 MB (84375718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4818856db2607f772bd7473a24a56ab5f0a5b94e5edb2385165e71e422658550`  
		Last Modified: Wed, 23 Mar 2022 23:34:38 GMT  
		Size: 9.2 KB (9204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5d0dc8eef40fe844dbfcbc90e8a0a2b8c6acaa617c711fb7b62edcafa24e22a`  
		Last Modified: Wed, 23 Mar 2022 23:34:38 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:defedf53a02886f37f78b905294630129c1a9cf25a0dbabc3981c0141d3f645e`  
		Last Modified: Wed, 23 Mar 2022 23:34:38 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:918ada37a4afa5b0ae726294c6e251b2852aaa06227faed4576dc8e0589cb615`  
		Last Modified: Wed, 23 Mar 2022 23:34:38 GMT  
		Size: 4.7 KB (4700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:14-alpine3.15` - linux; s390x

```console
$ docker pull postgres@sha256:d2c6645af917dcd01b27db9bbb93194a60224773767d512864998e6f4bb3f929
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **83.8 MB (83759960 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ebd3e966ff658aa0ab9e727463b7bc859d6a90aae4ba42e61e07e4653f54ef83`
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
# Wed, 23 Mar 2022 19:40:12 GMT
ENV PG_MAJOR=14
# Wed, 23 Mar 2022 19:40:12 GMT
ENV PG_VERSION=14.2
# Wed, 23 Mar 2022 19:40:12 GMT
ENV PG_SHA256=2cf78b2e468912f8101d695db5340cf313c2e9f68a612fb71427524e8c9a977a
# Mon, 28 Mar 2022 23:45:10 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm-dev clang g++ 		make 		openldap-dev 		openssl-dev 		perl-dev 		perl-ipc-run 		perl-utils 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		icu-dev 		lz4-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-krb5 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 		--with-lz4 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 		zstd 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Mon, 28 Mar 2022 23:45:13 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample
# Mon, 28 Mar 2022 23:45:14 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Mon, 28 Mar 2022 23:45:14 GMT
ENV PGDATA=/var/lib/postgresql/data
# Mon, 28 Mar 2022 23:45:14 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Mon, 28 Mar 2022 23:45:15 GMT
VOLUME [/var/lib/postgresql/data]
# Mon, 28 Mar 2022 23:45:15 GMT
COPY file:e8928645623137de410cce68a2aa3b22f07a64e6391025598a60f3e461c606a3 in /usr/local/bin/ 
# Mon, 28 Mar 2022 23:45:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 28 Mar 2022 23:45:15 GMT
STOPSIGNAL SIGINT
# Mon, 28 Mar 2022 23:45:15 GMT
EXPOSE 5432
# Mon, 28 Mar 2022 23:45:15 GMT
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
	-	`sha256:1eb2f61cd5730625d581a37845e8e1b3340f5e317004ed0189128d4bbe7b5c6f`  
		Last Modified: Mon, 28 Mar 2022 23:59:19 GMT  
		Size: 81.1 MB (81142578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5fdf461e95636f15ccc2d84f5851ea70eb5a9017794436fda23e441966fa3d7`  
		Last Modified: Mon, 28 Mar 2022 23:59:11 GMT  
		Size: 9.2 KB (9204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ba05f0d9c1675ed4778db804f43d1ac096cdf757cb980e77e6a86a74e442a8a`  
		Last Modified: Mon, 28 Mar 2022 23:59:07 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acf58878040b743bdf1e737b23b73adf8256c7ebb3df4b223e81cb5a9b57c645`  
		Last Modified: Mon, 28 Mar 2022 23:59:06 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39cd6433e4ef473f9f529c0e6dc2bb8b50c0ae8caab078f5af51be57b2efef44`  
		Last Modified: Mon, 28 Mar 2022 23:59:11 GMT  
		Size: 4.7 KB (4696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
