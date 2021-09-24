## `postgres:14rc1-alpine3.14`

```console
$ docker pull postgres@sha256:bc9f311be96786db94457efd89be66c0dc5bdc95414e9a2d4d8ce6fff13292a3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `postgres:14rc1-alpine3.14` - linux; amd64

```console
$ docker pull postgres@sha256:a02683ad721245bdabc26a43b7d3080631e89ae8a65f3417b745756bcbd7d20d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.3 MB (77325268 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:db69b5fbfccfee090f7af8132d507d14d1e1468f7a694ad39115e8c1269f0a3f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Fri, 27 Aug 2021 22:48:02 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Fri, 27 Aug 2021 22:48:02 GMT
ENV LANG=en_US.utf8
# Fri, 27 Aug 2021 22:48:03 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 27 Aug 2021 22:48:03 GMT
ENV PG_MAJOR=14
# Thu, 23 Sep 2021 23:49:39 GMT
ENV PG_VERSION=14rc1
# Thu, 23 Sep 2021 23:49:39 GMT
ENV PG_SHA256=586a816cb7811985f474eda0d4926fabd2378f0f6d5659d12fba421d38a07616
# Thu, 23 Sep 2021 23:55:59 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm11-dev clang g++ 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 		lz4-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 		--with-lz4 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Thu, 23 Sep 2021 23:56:00 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample
# Thu, 23 Sep 2021 23:56:01 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 23 Sep 2021 23:56:01 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 23 Sep 2021 23:56:02 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 23 Sep 2021 23:56:02 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 23 Sep 2021 23:56:02 GMT
COPY file:ad28506adc606e446eefc263bc99d4cb809e608d4f550956143bf13c82c91f85 in /usr/local/bin/ 
# Thu, 23 Sep 2021 23:56:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Sep 2021 23:56:03 GMT
STOPSIGNAL SIGINT
# Thu, 23 Sep 2021 23:56:03 GMT
EXPOSE 5432
# Thu, 23 Sep 2021 23:56:03 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:a0d0a0d46f8b52473982a3c466318f479767577551a53ffc9074c9fa7035982e`  
		Last Modified: Fri, 27 Aug 2021 17:20:13 GMT  
		Size: 2.8 MB (2814446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5034a66b99e67db609bf6b4f82bea915e39a42e6f03d11889f7406b4de9e99da`  
		Last Modified: Fri, 27 Aug 2021 23:28:20 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82e9eb77798bd506a06a9adab733c822c718be829c54d514b5789b07c0f1c164`  
		Last Modified: Fri, 27 Aug 2021 23:28:20 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6c79b0bf8c1639cb6c4065897d78b8e1e831d2169b4772653042529e26e4d96`  
		Last Modified: Fri, 24 Sep 2021 00:00:44 GMT  
		Size: 74.5 MB (74495422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2010d088b52d37cec7d2fd31266ce947691811c917e3dc50e6ba2a44cd9e1a07`  
		Last Modified: Fri, 24 Sep 2021 00:00:34 GMT  
		Size: 9.2 KB (9208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7d0064b53f1788c84f703b6c0f8ab11109a0c5b0d66c8c2da6f9bdf00b5cd78`  
		Last Modified: Fri, 24 Sep 2021 00:00:34 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cf4097bdf301bd1d19e433a48e70c190a10bc499ac4906890e75928e50bf63e`  
		Last Modified: Fri, 24 Sep 2021 00:00:34 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84cbd7f80baf38ba6fb27a15dafe704ac43d3a9721923435ff272d11259ca773`  
		Last Modified: Fri, 24 Sep 2021 00:00:34 GMT  
		Size: 4.4 KB (4406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:14rc1-alpine3.14` - linux; arm variant v6

```console
$ docker pull postgres@sha256:98a4191e9d61a6c19ff496d281f14b96fc98e4f8a0b339320ef205ff3d21892f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.8 MB (75838473 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:00174041ac6372cd54a3b4fef9af28d05ad054f43bc4db1083c106f828ba9b7d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Fri, 27 Aug 2021 17:49:29 GMT
ADD file:1c1c4520d49cb6e8f795f3b953d1ed3c3c77868b98b53a455169c254fcec5acd in / 
# Fri, 27 Aug 2021 17:49:30 GMT
CMD ["/bin/sh"]
# Fri, 27 Aug 2021 22:04:28 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Fri, 27 Aug 2021 22:04:29 GMT
ENV LANG=en_US.utf8
# Fri, 27 Aug 2021 22:04:33 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 27 Aug 2021 22:04:34 GMT
ENV PG_MAJOR=14
# Thu, 23 Sep 2021 23:31:50 GMT
ENV PG_VERSION=14rc1
# Thu, 23 Sep 2021 23:31:51 GMT
ENV PG_SHA256=586a816cb7811985f474eda0d4926fabd2378f0f6d5659d12fba421d38a07616
# Thu, 23 Sep 2021 23:36:44 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm11-dev clang g++ 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 		lz4-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 		--with-lz4 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Thu, 23 Sep 2021 23:36:46 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample
# Thu, 23 Sep 2021 23:36:48 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 23 Sep 2021 23:36:49 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 23 Sep 2021 23:36:51 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 23 Sep 2021 23:36:51 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 23 Sep 2021 23:36:52 GMT
COPY file:ad28506adc606e446eefc263bc99d4cb809e608d4f550956143bf13c82c91f85 in /usr/local/bin/ 
# Thu, 23 Sep 2021 23:36:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Sep 2021 23:36:52 GMT
STOPSIGNAL SIGINT
# Thu, 23 Sep 2021 23:36:53 GMT
EXPOSE 5432
# Thu, 23 Sep 2021 23:36:53 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:2e78c0f86ba9a1fed30df20cb48c9cc73e9626399f12749d36b892ff99c0ecf5`  
		Last Modified: Fri, 27 Aug 2021 17:50:55 GMT  
		Size: 2.6 MB (2627447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a768a51394fb89d634086ed31a7649653823611d054a16603974b9148da6f5b`  
		Last Modified: Fri, 27 Aug 2021 22:36:22 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e44aa70cad34222b58a50860314f35128c905e3265d6d7bf08054f3c70daeb3d`  
		Last Modified: Fri, 27 Aug 2021 22:36:22 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28bfc37c7dd2c5fdecf7ea4e78da6d192b2ea683190f9161388a7ce4d3cf8479`  
		Last Modified: Thu, 23 Sep 2021 23:40:38 GMT  
		Size: 73.2 MB (73195627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66ab6673c5d2e5e848aaa7105be836d0bdfd0e7cd6efb0a8257b9617b9734a33`  
		Last Modified: Thu, 23 Sep 2021 23:39:55 GMT  
		Size: 9.2 KB (9202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac708e924e1fdca5a8035aa2f9e4a5f84a30ff35e6eba6ef397072036759a3e2`  
		Last Modified: Thu, 23 Sep 2021 23:39:55 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6069f40005e1a1b1f955ab0688b6073579717eeff183251a35898e4e2ab5af5`  
		Last Modified: Thu, 23 Sep 2021 23:39:55 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6762cf3cad5e41ec457bfa640b545ed666c95e6261dc80274dcd2b34afc2cc28`  
		Last Modified: Thu, 23 Sep 2021 23:39:56 GMT  
		Size: 4.4 KB (4408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:14rc1-alpine3.14` - linux; arm64 variant v8

```console
$ docker pull postgres@sha256:28a18c1a3f8449bd5490d53adbaf681c909fb90fb680181bcbf9a3d1483676af
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.2 MB (76217328 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b8c13f3f083baabab28a2b5d35671ccf8897877854b54f1b03addae6cb75b03`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Fri, 27 Aug 2021 17:39:33 GMT
ADD file:dc8af9c7bfe9f9541e1db38dea01c4201609f3075b31e108f2073ffed8c5e4b9 in / 
# Fri, 27 Aug 2021 17:39:33 GMT
CMD ["/bin/sh"]
# Sat, 28 Aug 2021 00:44:21 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Sat, 28 Aug 2021 00:44:21 GMT
ENV LANG=en_US.utf8
# Sat, 28 Aug 2021 00:44:22 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 28 Aug 2021 00:44:22 GMT
ENV PG_MAJOR=14
# Fri, 24 Sep 2021 01:22:55 GMT
ENV PG_VERSION=14rc1
# Fri, 24 Sep 2021 01:22:56 GMT
ENV PG_SHA256=586a816cb7811985f474eda0d4926fabd2378f0f6d5659d12fba421d38a07616
# Fri, 24 Sep 2021 01:27:27 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm11-dev clang g++ 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 		lz4-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 		--with-lz4 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Fri, 24 Sep 2021 01:27:29 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample
# Fri, 24 Sep 2021 01:27:29 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 24 Sep 2021 01:27:29 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 24 Sep 2021 01:27:30 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 24 Sep 2021 01:27:30 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 24 Sep 2021 01:27:30 GMT
COPY file:ad28506adc606e446eefc263bc99d4cb809e608d4f550956143bf13c82c91f85 in /usr/local/bin/ 
# Fri, 24 Sep 2021 01:27:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Sep 2021 01:27:31 GMT
STOPSIGNAL SIGINT
# Fri, 24 Sep 2021 01:27:31 GMT
EXPOSE 5432
# Fri, 24 Sep 2021 01:27:31 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:552d1f2373af9bfe12033568ebbfb0ccbb0de11279f9a415a29207e264d7f4d9`  
		Last Modified: Fri, 27 Aug 2021 17:40:18 GMT  
		Size: 2.7 MB (2711827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7e9520c37213002780ab811214a7b664b01adbff78712b200a8ad6dac8f6ecb`  
		Last Modified: Sat, 28 Aug 2021 01:11:06 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e16841d04e832ad38f955594481fd7205810db3379719d35e62c344f12dc0ff`  
		Last Modified: Sat, 28 Aug 2021 01:11:06 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daa96d8477a738240ba70773ba43917d6c36f1a6ad4cedafefbdb8873e398a3f`  
		Last Modified: Fri, 24 Sep 2021 01:33:11 GMT  
		Size: 73.5 MB (73490106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b64f6146c486d4823bb1270051661a3426a09986c3fe9ea6132158bba5fd9f8`  
		Last Modified: Fri, 24 Sep 2021 01:33:01 GMT  
		Size: 9.2 KB (9200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c6f5139bdabf2d8f8f3a4230b6565702ab7243e7c3b342f549b26e864388bcc`  
		Last Modified: Fri, 24 Sep 2021 01:33:01 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e9c42ff81e2cd421927e31fcaea50690a516947cb3fc6001a9d6cd643461a10`  
		Last Modified: Fri, 24 Sep 2021 01:33:01 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27e03163aa661dba041442bc2668ab2025fe2caebad5228a4a6e6f0753975b6c`  
		Last Modified: Fri, 24 Sep 2021 01:33:01 GMT  
		Size: 4.4 KB (4405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:14rc1-alpine3.14` - linux; 386

```console
$ docker pull postgres@sha256:ce711ce88dbd9fb2c5d603d5ece6ac418352c7dd72ebf5e345cc9f9b6ed56ed1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **82.1 MB (82098039 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9934dedbdba4b4d2346f401745a3855e97f9403a27794a9f31d7b865d557a91c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Fri, 27 Aug 2021 17:38:29 GMT
ADD file:42a7bc5a08b546b47049dd0f89ae4e7a8c86342f87000f39ade3ff52916a6c2e in / 
# Fri, 27 Aug 2021 17:38:30 GMT
CMD ["/bin/sh"]
# Fri, 27 Aug 2021 21:55:05 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Fri, 27 Aug 2021 21:55:05 GMT
ENV LANG=en_US.utf8
# Fri, 27 Aug 2021 21:55:06 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 27 Aug 2021 21:55:06 GMT
ENV PG_MAJOR=14
# Thu, 23 Sep 2021 23:12:58 GMT
ENV PG_VERSION=14rc1
# Thu, 23 Sep 2021 23:12:58 GMT
ENV PG_SHA256=586a816cb7811985f474eda0d4926fabd2378f0f6d5659d12fba421d38a07616
# Thu, 23 Sep 2021 23:19:21 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm11-dev clang g++ 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 		lz4-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 		--with-lz4 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Thu, 23 Sep 2021 23:19:22 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample
# Thu, 23 Sep 2021 23:19:23 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 23 Sep 2021 23:19:23 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 23 Sep 2021 23:19:24 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 23 Sep 2021 23:19:24 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 23 Sep 2021 23:19:25 GMT
COPY file:ad28506adc606e446eefc263bc99d4cb809e608d4f550956143bf13c82c91f85 in /usr/local/bin/ 
# Thu, 23 Sep 2021 23:19:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Sep 2021 23:19:25 GMT
STOPSIGNAL SIGINT
# Thu, 23 Sep 2021 23:19:25 GMT
EXPOSE 5432
# Thu, 23 Sep 2021 23:19:26 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:b11ae9fc5d8a106cfed3a6f6c75e5b5b5797c566fac4411622b4055df6541286`  
		Last Modified: Fri, 27 Aug 2021 17:39:18 GMT  
		Size: 2.8 MB (2822857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b976c7cea63cd0c42b035f2167b42952bfe4b4c5c26d5c1828e46ccf08b16dd9`  
		Last Modified: Fri, 27 Aug 2021 22:41:30 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b58324ac0c0139295582dea67f31b819f305cd721ba1189ab4e66fbb574de652`  
		Last Modified: Fri, 27 Aug 2021 22:41:30 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22227e5fb47f4df8c176739fb3c3304a62cd318f91708854dc70406793dc85e0`  
		Last Modified: Fri, 24 Sep 2021 00:33:33 GMT  
		Size: 79.3 MB (79259786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:672d485a47334b9556f21a10af89a01b50e4c78df4bfc6c6bfd912f18ffb141f`  
		Last Modified: Fri, 24 Sep 2021 00:33:10 GMT  
		Size: 9.2 KB (9202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc1c63919f5fc41b83c30232633fb66a413ecdb264b1461cd21d217d21fceebd`  
		Last Modified: Fri, 24 Sep 2021 00:33:11 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70258a98a540820a7f3c88a07139ff4e5619915151314711f5c2b91115713d08`  
		Last Modified: Fri, 24 Sep 2021 00:33:11 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ae6d596b78151f01e43405159ca28dc1c7a7e4b8adf2971cea12afeecf823d8`  
		Last Modified: Fri, 24 Sep 2021 00:33:11 GMT  
		Size: 4.4 KB (4404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:14rc1-alpine3.14` - linux; ppc64le

```console
$ docker pull postgres@sha256:c733637afdf22d6edba27c2d3d48557a976cd72382c66da766cc29c4dce5190f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **82.3 MB (82348083 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:599920bc14c9bc3dad455e88b1f9ec70ef81893ae41fc84ad577eec45a39efb4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Fri, 27 Aug 2021 19:39:54 GMT
ADD file:d213c56ffc24a5051e8060fd0fec1a0520367c10d88ab16321c36336b6c66098 in / 
# Fri, 27 Aug 2021 19:39:59 GMT
CMD ["/bin/sh"]
# Fri, 27 Aug 2021 21:43:37 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Fri, 27 Aug 2021 21:43:39 GMT
ENV LANG=en_US.utf8
# Fri, 27 Aug 2021 21:43:48 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 27 Aug 2021 21:43:53 GMT
ENV PG_MAJOR=14
# Fri, 24 Sep 2021 06:47:49 GMT
ENV PG_VERSION=14rc1
# Fri, 24 Sep 2021 06:47:58 GMT
ENV PG_SHA256=586a816cb7811985f474eda0d4926fabd2378f0f6d5659d12fba421d38a07616
# Fri, 24 Sep 2021 06:52:33 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm11-dev clang g++ 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 		lz4-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 		--with-lz4 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Fri, 24 Sep 2021 06:53:04 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample
# Fri, 24 Sep 2021 06:53:18 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 24 Sep 2021 06:53:24 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 24 Sep 2021 06:53:41 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 24 Sep 2021 06:53:48 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 24 Sep 2021 06:53:53 GMT
COPY file:ad28506adc606e446eefc263bc99d4cb809e608d4f550956143bf13c82c91f85 in /usr/local/bin/ 
# Fri, 24 Sep 2021 06:53:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Sep 2021 06:54:02 GMT
STOPSIGNAL SIGINT
# Fri, 24 Sep 2021 06:54:14 GMT
EXPOSE 5432
# Fri, 24 Sep 2021 06:54:20 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:63da8ca98f7b4b94381aed56862a60aecf355d9428b9aeb7c61d5bd017100c18`  
		Last Modified: Fri, 27 Aug 2021 19:41:06 GMT  
		Size: 2.8 MB (2812284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51b84363c8c0f2373e8b665451df1c6a11a9415fd4f1c773e8ce7aaafa836248`  
		Last Modified: Fri, 27 Aug 2021 22:17:39 GMT  
		Size: 1.3 KB (1287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7f2722689cf013f5f6333bf25f2c1fa26b298e09468166e2cbade7a81c0817c`  
		Last Modified: Fri, 27 Aug 2021 22:17:38 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d87d8d422ab251a9396956aa6d524feff46dafb3b3ef8d1233e476d8c70f9618`  
		Last Modified: Fri, 24 Sep 2021 07:20:05 GMT  
		Size: 79.5 MB (79520392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ca34b9544a81ed813cc66415709cf8520f076ce95a43b54f6b2c2c0fb0538e9`  
		Last Modified: Fri, 24 Sep 2021 07:19:52 GMT  
		Size: 9.2 KB (9210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfd9029a4978df685af3a4298c2aed99fc69ca5b84533909e1c00aff684c7000`  
		Last Modified: Fri, 24 Sep 2021 07:19:51 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09c8a20fa1297c49b74d06db5f42299554327b262bec618d8a7b33cb9e457952`  
		Last Modified: Fri, 24 Sep 2021 07:19:51 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1a1f10e04bc0f992eb3de9bcff2252ba7cfc451c9ab1d3cca8c9a264ff42456`  
		Last Modified: Fri, 24 Sep 2021 07:19:51 GMT  
		Size: 4.4 KB (4406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:14rc1-alpine3.14` - linux; s390x

```console
$ docker pull postgres@sha256:2da66594ded5f426c1761650e9d21192086ef5975bb580b7920e2cf233210b06
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **78.6 MB (78603571 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4508fcea87221cfd046799dbea4d013f8a86a184d13d2e5da0229eb32b8ace00`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Fri, 27 Aug 2021 17:41:29 GMT
ADD file:9b40ee281e8797067fb2ae207c406084cb81593090338a8b7cb09ade52168daa in / 
# Fri, 27 Aug 2021 17:41:30 GMT
CMD ["/bin/sh"]
# Sat, 28 Aug 2021 00:49:31 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Sat, 28 Aug 2021 00:49:32 GMT
ENV LANG=en_US.utf8
# Sat, 28 Aug 2021 00:49:32 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 28 Aug 2021 00:49:32 GMT
ENV PG_MAJOR=14
# Thu, 23 Sep 2021 22:50:59 GMT
ENV PG_VERSION=14rc1
# Thu, 23 Sep 2021 22:50:59 GMT
ENV PG_SHA256=586a816cb7811985f474eda0d4926fabd2378f0f6d5659d12fba421d38a07616
# Thu, 23 Sep 2021 22:53:46 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm11-dev clang g++ 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 		lz4-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 		--with-lz4 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Thu, 23 Sep 2021 22:53:49 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample
# Thu, 23 Sep 2021 22:53:50 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 23 Sep 2021 22:53:50 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 23 Sep 2021 22:53:51 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 23 Sep 2021 22:53:51 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 23 Sep 2021 22:53:51 GMT
COPY file:ad28506adc606e446eefc263bc99d4cb809e608d4f550956143bf13c82c91f85 in /usr/local/bin/ 
# Thu, 23 Sep 2021 22:53:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Sep 2021 22:53:51 GMT
STOPSIGNAL SIGINT
# Thu, 23 Sep 2021 22:53:51 GMT
EXPOSE 5432
# Thu, 23 Sep 2021 22:53:51 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:da14cb6b6dc946dbb2d84386bcaca84e2d46f650767cd11bdb3331ec9d623988`  
		Last Modified: Fri, 27 Aug 2021 17:42:25 GMT  
		Size: 2.6 MB (2603464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31510cc6ab297041382a23f3ee5b4a7cf8e1a650f86836260bfcb82cbd35f7eb`  
		Last Modified: Sat, 28 Aug 2021 01:19:34 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a5c23a40fbc63d8bd8713694dbda49900c3198d4156a8b8ca18ccc15b793399`  
		Last Modified: Sat, 28 Aug 2021 01:19:33 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e553da16a5d90a76a41b979a429bab341b28dc1bbad36d8421ba661180e0d7a`  
		Last Modified: Thu, 23 Sep 2021 23:35:32 GMT  
		Size: 76.0 MB (75984715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2543df2fc5f15d9399e85951251b20134246cc74134e3f81c425e592373e0a6`  
		Last Modified: Thu, 23 Sep 2021 23:35:23 GMT  
		Size: 9.2 KB (9200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82a59cc3ed5e3e1ccba7c82e7a482d54b0cb39f88b9a09ec455d14a17e2b2b34`  
		Last Modified: Thu, 23 Sep 2021 23:35:23 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc13bbba2eca7795c0c2ed48f770b1aaa6bdf7382089f71f33cf4016ad8ef02a`  
		Last Modified: Thu, 23 Sep 2021 23:35:23 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0055cc2c63413511f46f39b03adef9ec61a7cf7ed8788969b30981abfbe05166`  
		Last Modified: Thu, 23 Sep 2021 23:35:23 GMT  
		Size: 4.4 KB (4404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
