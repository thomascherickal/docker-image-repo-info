## `postgres:12-alpine`

```console
$ docker pull postgres@sha256:e2f4a5b7c3173ac9ab9aa97e5fb82631d7beb719f4c74cd26cee0cc1ed8881ee
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `postgres:12-alpine` - linux; amd64

```console
$ docker pull postgres@sha256:eee6f89fab183ebae62ad976722e3c2c1d201e73916af664d6c8fbfe9fe071fd
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.5 MB (61498214 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4f5f2240c9a49d71b52db92d591e10dd16ba228c129e81029f775daca8d9e648`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:41 GMT
ADD file:ec475c2abb2d46435286b5ae5efacf5b50b1a9e3b6293b69db3c0172b5b9658b in / 
# Thu, 17 Dec 2020 00:19:42 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 00:59:48 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 17 Dec 2020 00:59:49 GMT
ENV LANG=en_US.utf8
# Thu, 17 Dec 2020 00:59:50 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 17 Dec 2020 01:07:43 GMT
ENV PG_MAJOR=12
# Thu, 17 Dec 2020 01:07:44 GMT
ENV PG_VERSION=12.5
# Thu, 17 Dec 2020 01:07:44 GMT
ENV PG_SHA256=bd0d25341d9578b5473c9506300022de26370879581f5fddd243a886ce79ff95
# Thu, 17 Dec 2020 01:14:35 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm10-dev clang g++ 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Thu, 17 Dec 2020 01:14:37 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Thu, 17 Dec 2020 01:14:38 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 17 Dec 2020 01:14:38 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 17 Dec 2020 01:14:39 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 17 Dec 2020 01:14:40 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 17 Dec 2020 01:14:40 GMT
COPY file:8f542efd076b9b67ef64928f3c0185ed50bfcbbc3572436a7222e879810d747f in /usr/local/bin/ 
# Thu, 17 Dec 2020 01:14:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Dec 2020 01:14:40 GMT
STOPSIGNAL SIGINT
# Thu, 17 Dec 2020 01:14:40 GMT
EXPOSE 5432
# Thu, 17 Dec 2020 01:14:40 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:801bfaa63ef2094d770c809815b9e2b9c1194728e5e754ef7bc764030e140cea`  
		Last Modified: Wed, 16 Dec 2020 19:34:50 GMT  
		Size: 2.8 MB (2799066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8392b19747a95c5f0945f923608970a15320af8654f0a299a0fc345f7d2aa926`  
		Last Modified: Thu, 17 Dec 2020 01:35:47 GMT  
		Size: 1.2 KB (1249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae408abf9c34442cb63539f6995aa2f7a7f934c7671d59879da83a8a0d936c6d`  
		Last Modified: Thu, 17 Dec 2020 01:35:45 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47c4a28307fc51ef32aca7e0256bc157dd83bf552c1a5618bfe1e5937cf2db9f`  
		Last Modified: Thu, 17 Dec 2020 01:36:22 GMT  
		Size: 58.7 MB (58685021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e39140439913c5ee6d62199bc37338f02ad6f582ebc0f857d24600d969f6710`  
		Last Modified: Thu, 17 Dec 2020 01:36:10 GMT  
		Size: 8.2 KB (8213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f64e51a82d10a441cd5432fe9fbd6e4486d6df087081a0f0c3c00573821879af`  
		Last Modified: Thu, 17 Dec 2020 01:36:09 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ceaa4d24e193d4c327e7419e46c00cfe0ef57be2fe8ad36c53a06c586adaa6d`  
		Last Modified: Thu, 17 Dec 2020 01:36:09 GMT  
		Size: 164.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d92928e7b8c5641ae358590041322f03aa750a83a4c23a65183fc9b06ec52ddd`  
		Last Modified: Thu, 17 Dec 2020 01:36:10 GMT  
		Size: 4.3 KB (4258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:12-alpine` - linux; arm variant v6

```console
$ docker pull postgres@sha256:c88b8bf0b26a3200d89d4d7a28351a9b64d46cdd9ae526f7652a468c26bfe3ff
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.7 MB (59742004 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0de1acb41ecbd6c13df952213b9a5d4714ae26cf567a319a02f0d1551495d3a4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Wed, 16 Dec 2020 23:49:43 GMT
ADD file:0a16715e2d0e5811c3c578945d618db0e269847a799340248f9ba8d393c9eec2 in / 
# Wed, 16 Dec 2020 23:49:45 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 05:45:15 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 17 Dec 2020 05:45:16 GMT
ENV LANG=en_US.utf8
# Thu, 17 Dec 2020 05:45:18 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 17 Dec 2020 05:50:37 GMT
ENV PG_MAJOR=12
# Thu, 17 Dec 2020 05:50:39 GMT
ENV PG_VERSION=12.5
# Thu, 17 Dec 2020 05:50:40 GMT
ENV PG_SHA256=bd0d25341d9578b5473c9506300022de26370879581f5fddd243a886ce79ff95
# Thu, 17 Dec 2020 05:55:01 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm10-dev clang g++ 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Thu, 17 Dec 2020 05:55:05 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Thu, 17 Dec 2020 05:55:07 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 17 Dec 2020 05:55:08 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 17 Dec 2020 05:55:11 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 17 Dec 2020 05:55:12 GMT
VOLUME [/var/lib/postgresql/data]
# Wed, 30 Dec 2020 00:55:08 GMT
COPY file:f937c0ee3ab8736d7adeefe3108ce546c352d85751a620058fb9427c3648a82c in /usr/local/bin/ 
# Wed, 30 Dec 2020 00:55:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 30 Dec 2020 00:55:09 GMT
STOPSIGNAL SIGINT
# Wed, 30 Dec 2020 00:55:10 GMT
EXPOSE 5432
# Wed, 30 Dec 2020 00:55:10 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:93247449aef3c56eb4f7ab7b3fed95743c974b823def6dd86ec84008126e7903`  
		Last Modified: Wed, 16 Dec 2020 23:50:24 GMT  
		Size: 2.6 MB (2604163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8281cbd4bde01cbf0ed0e8ecf5550798d848c1d7d2d642a0416759d8df635f3`  
		Last Modified: Thu, 17 Dec 2020 06:08:22 GMT  
		Size: 1.3 KB (1276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eae834cabab68fcc6ee1f251914773d8111eba34640f8849961845844a4f4681`  
		Last Modified: Thu, 17 Dec 2020 06:08:22 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94ee3946e1b14118f46f9caa5792d044e45400f80b2fc7d17a97531f78b9f144`  
		Last Modified: Thu, 17 Dec 2020 06:08:48 GMT  
		Size: 57.1 MB (57123454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69d3f28f62712e489734b7685b75d37373005e16249673996c336f75ffcf2e37`  
		Last Modified: Thu, 17 Dec 2020 06:08:32 GMT  
		Size: 8.2 KB (8215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52ec9bc11b92f83b75189a71d0fdaf5cfe2625f3727a51dab6f547b0943e3ade`  
		Last Modified: Thu, 17 Dec 2020 06:08:31 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f81606619864685a37a5c8d493691ae6606e6810d70c7685f842eaf9e784eca`  
		Last Modified: Thu, 17 Dec 2020 06:08:31 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1425268980731d786b05be0d1f9a56237eb3dbfbc15897d91f3bdbb1c434d139`  
		Last Modified: Wed, 30 Dec 2020 00:56:46 GMT  
		Size: 4.4 KB (4393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:12-alpine` - linux; arm variant v7

```console
$ docker pull postgres@sha256:54fddcfa4ab57116b88fc96e876f61f7e40063426f43d48c60f5f370b3a9505c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.9 MB (56874262 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5cee9948c339467ed30b01e8edc121925ab29375f1687e730929764ade6f6f9c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Wed, 16 Dec 2020 23:58:14 GMT
ADD file:bd07f77a2b2741ca6bda80d9203be9c7274cf73145bff778cf000db0d8d4e903 in / 
# Wed, 16 Dec 2020 23:58:15 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 05:35:59 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 17 Dec 2020 05:36:01 GMT
ENV LANG=en_US.utf8
# Thu, 17 Dec 2020 05:36:05 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 17 Dec 2020 05:39:51 GMT
ENV PG_MAJOR=12
# Thu, 17 Dec 2020 05:39:52 GMT
ENV PG_VERSION=12.5
# Thu, 17 Dec 2020 05:39:53 GMT
ENV PG_SHA256=bd0d25341d9578b5473c9506300022de26370879581f5fddd243a886ce79ff95
# Thu, 17 Dec 2020 05:42:48 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm10-dev clang g++ 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Thu, 17 Dec 2020 05:42:50 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Thu, 17 Dec 2020 05:42:52 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 17 Dec 2020 05:42:53 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 17 Dec 2020 05:42:55 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 17 Dec 2020 05:42:56 GMT
VOLUME [/var/lib/postgresql/data]
# Wed, 30 Dec 2020 01:02:07 GMT
COPY file:f937c0ee3ab8736d7adeefe3108ce546c352d85751a620058fb9427c3648a82c in /usr/local/bin/ 
# Wed, 30 Dec 2020 01:02:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 30 Dec 2020 01:02:08 GMT
STOPSIGNAL SIGINT
# Wed, 30 Dec 2020 01:02:09 GMT
EXPOSE 5432
# Wed, 30 Dec 2020 01:02:10 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:c58e8a26a8407acc3ead776f6526efa889fda03270a8d05109208d9f59159420`  
		Last Modified: Wed, 16 Dec 2020 23:58:59 GMT  
		Size: 2.4 MB (2407555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81fd93cc6a1e39bdb8121ae35ee402c25416b317da7efd7e27a38a4af80710b7`  
		Last Modified: Thu, 17 Dec 2020 05:58:49 GMT  
		Size: 1.3 KB (1277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9fc827812b79452d91ced463793937316b84ae0d091f1be8f633999b998bf4b`  
		Last Modified: Thu, 17 Dec 2020 05:58:48 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdd53e87812e9495e0af28503a9bbbd86872047bb29a15ca57da39bbea4f35ec`  
		Last Modified: Thu, 17 Dec 2020 05:59:33 GMT  
		Size: 54.5 MB (54452316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df0f44c46aaf1dc95a159b360c97457c746764bbf07308eda0c45c75386bf85f`  
		Last Modified: Thu, 17 Dec 2020 05:59:16 GMT  
		Size: 8.2 KB (8212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0bd795650194138c943cf4c2f105529bf90a5d2af42ae8ce28ed262fa5dc296`  
		Last Modified: Thu, 17 Dec 2020 05:59:15 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf836abdd6a5d6bddfb9e1fb774d0dff1e2b0a984aab806a9b082354f15bbd48`  
		Last Modified: Thu, 17 Dec 2020 05:59:15 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d90b728d4ee31f2a99cba9d78dd3f97407b43649926dd89d0a5b9238c8510478`  
		Last Modified: Wed, 30 Dec 2020 01:05:14 GMT  
		Size: 4.4 KB (4396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:12-alpine` - linux; arm64 variant v8

```console
$ docker pull postgres@sha256:e204667c5ea1021c9c7723a3c4f79ae04615f9c976de13f786fe974adc234c9e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.1 MB (61060213 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4f0b38348599d952ec2be4f5f9282ef96a9c84c15c085cbefaeb25618aae3643`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Wed, 16 Dec 2020 23:40:26 GMT
ADD file:a4845c3840a3fd0e41e4635a179cce20c81afc6c02e34e3fd5bd2d535698918b in / 
# Wed, 16 Dec 2020 23:40:29 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 04:01:11 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 17 Dec 2020 04:01:19 GMT
ENV LANG=en_US.utf8
# Thu, 17 Dec 2020 04:01:28 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 17 Dec 2020 04:06:22 GMT
ENV PG_MAJOR=12
# Thu, 17 Dec 2020 04:06:23 GMT
ENV PG_VERSION=12.5
# Thu, 17 Dec 2020 04:06:24 GMT
ENV PG_SHA256=bd0d25341d9578b5473c9506300022de26370879581f5fddd243a886ce79ff95
# Thu, 17 Dec 2020 04:09:56 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm10-dev clang g++ 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Thu, 17 Dec 2020 04:10:01 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Thu, 17 Dec 2020 04:10:04 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 17 Dec 2020 04:10:05 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 17 Dec 2020 04:10:09 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 17 Dec 2020 04:10:10 GMT
VOLUME [/var/lib/postgresql/data]
# Wed, 30 Dec 2020 00:43:19 GMT
COPY file:f937c0ee3ab8736d7adeefe3108ce546c352d85751a620058fb9427c3648a82c in /usr/local/bin/ 
# Wed, 30 Dec 2020 00:43:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 30 Dec 2020 00:43:25 GMT
STOPSIGNAL SIGINT
# Wed, 30 Dec 2020 00:43:27 GMT
EXPOSE 5432
# Wed, 30 Dec 2020 00:43:28 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:159e5727ea618dfe8b08811112e2c51f5bd2b9ae7db9eb214914a65249f70ca0`  
		Last Modified: Wed, 16 Dec 2020 23:41:08 GMT  
		Size: 2.7 MB (2709048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d20223af9aac4511a0a9a78463ff758585620e621be0678319eba90176b7e615`  
		Last Modified: Thu, 17 Dec 2020 04:28:04 GMT  
		Size: 1.3 KB (1283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2482f57ac4ab8ff038d0589f0507eea54d56adf3da98ff95df25c6beb575c1e4`  
		Last Modified: Thu, 17 Dec 2020 04:28:04 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3b1070dc40ee338bd6257ddfa0d2d403e8c59d1e93e912398459f8b3bdbbfa7`  
		Last Modified: Thu, 17 Dec 2020 04:28:49 GMT  
		Size: 58.3 MB (58336781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c135f1cdc71946c0716d2d7a287fb3af839f7a9e3d36a27ec78f56c66b54bbe6`  
		Last Modified: Thu, 17 Dec 2020 04:28:33 GMT  
		Size: 8.2 KB (8210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4960e60c6080d84c754535b97a8a5e332d1d216a89ae97551f187d04a94777f7`  
		Last Modified: Thu, 17 Dec 2020 04:28:33 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fdd3497cfd7214469427ad6b1dac72dbfcb2eaeb51006ae8f38048ef7fb421f`  
		Last Modified: Thu, 17 Dec 2020 04:28:33 GMT  
		Size: 192.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74eac3f07a62a18f58b8314da858419b34d5fb43618a78a256d1203f69db3aa8`  
		Last Modified: Wed, 30 Dec 2020 00:47:50 GMT  
		Size: 4.4 KB (4390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:12-alpine` - linux; 386

```console
$ docker pull postgres@sha256:0b1306be1cbbd795086524a9a42417a87e99aebae7997a7332c92690a52a3fc9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.1 MB (65050769 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b8f90cfe3298a3fd56034391a0fd24f0e022a2dfd749ebf13c41d7984b664d0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 17 Dec 2020 00:38:32 GMT
ADD file:de33fda50a142403e842620d20bc4404e66fc4ace16edc6946c4539e8a797458 in / 
# Thu, 17 Dec 2020 00:38:32 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 05:49:55 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 17 Dec 2020 05:49:56 GMT
ENV LANG=en_US.utf8
# Thu, 17 Dec 2020 05:49:56 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 17 Dec 2020 05:57:20 GMT
ENV PG_MAJOR=12
# Thu, 17 Dec 2020 05:57:20 GMT
ENV PG_VERSION=12.5
# Thu, 17 Dec 2020 05:57:20 GMT
ENV PG_SHA256=bd0d25341d9578b5473c9506300022de26370879581f5fddd243a886ce79ff95
# Fri, 18 Dec 2020 20:33:40 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm10-dev clang g++ 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Fri, 18 Dec 2020 20:33:41 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Fri, 18 Dec 2020 20:33:41 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 18 Dec 2020 20:33:42 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 18 Dec 2020 20:33:42 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 18 Dec 2020 20:33:42 GMT
VOLUME [/var/lib/postgresql/data]
# Wed, 30 Dec 2020 00:41:22 GMT
COPY file:f937c0ee3ab8736d7adeefe3108ce546c352d85751a620058fb9427c3648a82c in /usr/local/bin/ 
# Wed, 30 Dec 2020 00:41:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 30 Dec 2020 00:41:22 GMT
STOPSIGNAL SIGINT
# Wed, 30 Dec 2020 00:41:22 GMT
EXPOSE 5432
# Wed, 30 Dec 2020 00:41:23 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:455793c72b878001f0905634ed52a2524ba51796e7377bf00683a85123f7dce9`  
		Last Modified: Thu, 17 Dec 2020 00:39:18 GMT  
		Size: 2.8 MB (2794130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5305178ae8cb85c448e0963870f5425a527c36dae59155568c8da341f4173b82`  
		Last Modified: Thu, 17 Dec 2020 06:07:45 GMT  
		Size: 1.2 KB (1247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f3614159f507682c618782d96e8e35ed8b175b4dff44e39ef793184e39ba180`  
		Last Modified: Thu, 17 Dec 2020 06:07:45 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6ecc241f765a804fa84df1b0e3b9af034bd382606d710a3c233efc65df50567`  
		Last Modified: Fri, 18 Dec 2020 20:55:21 GMT  
		Size: 62.2 MB (62242389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9d9b4ad52ed0ea50c0cbeba808cfc61180f4f3a39bb9edaae859feb8845e13d`  
		Last Modified: Fri, 18 Dec 2020 20:55:05 GMT  
		Size: 8.2 KB (8207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0e8a5ff13514a225a2632b9b5e610333fa256750ba0b4380ceeda6155c0544d`  
		Last Modified: Fri, 18 Dec 2020 20:55:05 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a86c044ac0a7868073a4ab33f917d6be043ec161c9b777a52c279fd17224a6aa`  
		Last Modified: Fri, 18 Dec 2020 20:55:05 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c15cd0662b3ac44b1edb485b990a9ba37fa9a308a82a90584ef64e37533505c0`  
		Last Modified: Wed, 30 Dec 2020 00:43:02 GMT  
		Size: 4.4 KB (4391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:12-alpine` - linux; ppc64le

```console
$ docker pull postgres@sha256:9c33b3d498bd302370586f6db78563a2f076b9479ce5c5cc8ba164a268b046d3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.9 MB (63861306 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:26c4ef1e162ba9a2544d44017587e6e5e62cdf791bdce48f33f36a215330820b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 17 Dec 2020 00:20:42 GMT
ADD file:0a38c9b4955f8faa79627c166fca80ef342e443a16ce2925a30eeae317bbd786 in / 
# Thu, 17 Dec 2020 00:20:48 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 08:27:05 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 17 Dec 2020 08:27:07 GMT
ENV LANG=en_US.utf8
# Thu, 17 Dec 2020 08:27:16 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 17 Dec 2020 08:32:32 GMT
ENV PG_MAJOR=12
# Thu, 17 Dec 2020 08:32:41 GMT
ENV PG_VERSION=12.5
# Thu, 17 Dec 2020 08:32:48 GMT
ENV PG_SHA256=bd0d25341d9578b5473c9506300022de26370879581f5fddd243a886ce79ff95
# Thu, 17 Dec 2020 08:36:35 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm10-dev clang g++ 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Thu, 17 Dec 2020 08:36:52 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Thu, 17 Dec 2020 08:37:02 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 17 Dec 2020 08:37:06 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 17 Dec 2020 08:37:20 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 17 Dec 2020 08:37:21 GMT
VOLUME [/var/lib/postgresql/data]
# Wed, 30 Dec 2020 01:19:32 GMT
COPY file:f937c0ee3ab8736d7adeefe3108ce546c352d85751a620058fb9427c3648a82c in /usr/local/bin/ 
# Wed, 30 Dec 2020 01:19:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 30 Dec 2020 01:19:41 GMT
STOPSIGNAL SIGINT
# Wed, 30 Dec 2020 01:19:44 GMT
EXPOSE 5432
# Wed, 30 Dec 2020 01:19:47 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:a9d343b7bcc225fe7ac17d96a81329510ab7f31a50472311cafe7168d3107317`  
		Last Modified: Thu, 17 Dec 2020 00:21:33 GMT  
		Size: 2.8 MB (2805226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9020dece47a455612905a0f9d5608b39b5cfa68bf304d4473bbbee3f085dce3e`  
		Last Modified: Thu, 17 Dec 2020 08:55:18 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fd7a09fca54bf573268df0318667b22454de76b77537ce6968b9a9e3a5bd2b7`  
		Last Modified: Thu, 17 Dec 2020 08:55:17 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7708f8f88744af32a21db4f105e90c96989cc81785a3d05e4d2bac4fc838adc7`  
		Last Modified: Thu, 17 Dec 2020 08:55:54 GMT  
		Size: 61.0 MB (61041697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82eb8129c7cf36466698dead333e85a707cd430acec54b23b3ac3d7e700fa221`  
		Last Modified: Thu, 17 Dec 2020 08:55:41 GMT  
		Size: 8.2 KB (8209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bf899db54e2325843c2bfc6e0ab085f111f24e6b137d83d6fa17b318dcbc571`  
		Last Modified: Thu, 17 Dec 2020 08:55:41 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad2a4cd83fed38136166fe6cf40f13a564bcf7bf58346cbcf8dd99ed4425283f`  
		Last Modified: Thu, 17 Dec 2020 08:55:41 GMT  
		Size: 192.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a63b062fdc5ba40de9e8f78a9585ecc1ecfff45a6181c7c2bdf8526e58056427`  
		Last Modified: Wed, 30 Dec 2020 01:23:03 GMT  
		Size: 4.4 KB (4389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:12-alpine` - linux; s390x

```console
$ docker pull postgres@sha256:951a7ade41a9f6f21da15cf0d75d9976f08f04ae35d3bbc32016734ede220518
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.8 MB (63821364 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:036acc97b9fbf19cdcc1347e6adbb3cfb6a8f71299c2c3407819aff3d9c72d11`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Wed, 16 Dec 2020 23:41:37 GMT
ADD file:3ad3856d165e8760af85574a8ffa75ca44b7e1b97b64d1d6d4608445efa4b860 in / 
# Wed, 16 Dec 2020 23:41:37 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 09:43:56 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 17 Dec 2020 09:43:57 GMT
ENV LANG=en_US.utf8
# Thu, 17 Dec 2020 09:43:58 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 17 Dec 2020 09:47:08 GMT
ENV PG_MAJOR=12
# Thu, 17 Dec 2020 09:47:09 GMT
ENV PG_VERSION=12.5
# Thu, 17 Dec 2020 09:47:09 GMT
ENV PG_SHA256=bd0d25341d9578b5473c9506300022de26370879581f5fddd243a886ce79ff95
# Fri, 18 Dec 2020 22:48:37 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm10-dev clang g++ 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Fri, 18 Dec 2020 22:48:47 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Fri, 18 Dec 2020 22:48:49 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 18 Dec 2020 22:48:49 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 18 Dec 2020 22:48:51 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 18 Dec 2020 22:48:51 GMT
VOLUME [/var/lib/postgresql/data]
# Wed, 30 Dec 2020 00:46:01 GMT
COPY file:f937c0ee3ab8736d7adeefe3108ce546c352d85751a620058fb9427c3648a82c in /usr/local/bin/ 
# Wed, 30 Dec 2020 00:46:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 30 Dec 2020 00:46:02 GMT
STOPSIGNAL SIGINT
# Wed, 30 Dec 2020 00:46:02 GMT
EXPOSE 5432
# Wed, 30 Dec 2020 00:46:03 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:ee52640a49e15b8b7c8edb66c2d048b26abdee8d828d6e5ef4e10a28cb15a84f`  
		Last Modified: Wed, 16 Dec 2020 23:42:15 GMT  
		Size: 2.6 MB (2567018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec909f7d148e1f5c76f40f0fe4cec25c8a0f55dee05e382db0c692d59f7c084f`  
		Last Modified: Fri, 18 Dec 2020 23:05:49 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fadc63f7954f50d02abf819a5f8693cf92f86873d00c4dd5108f7dbbf5e0c48`  
		Last Modified: Fri, 18 Dec 2020 23:05:48 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:567adda11981f2512a0f94d11a7dec5a6c7b5228ba7201680ab13b48eb365b20`  
		Last Modified: Fri, 18 Dec 2020 23:06:36 GMT  
		Size: 61.2 MB (61239954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9350ff287a5a53e5361f17be9e444e73de4f199489e81fb1f08ad9a13ccf3aa0`  
		Last Modified: Fri, 18 Dec 2020 23:06:16 GMT  
		Size: 8.2 KB (8212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d3099e6180b6edb8800de12e463bd98aa87148a3dfe086a5e93aad417baa214`  
		Last Modified: Fri, 18 Dec 2020 23:06:17 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bd7e08a776745e17b0736c5cf416ca1cbef73ec835a9995cef031938fd0e583`  
		Last Modified: Fri, 18 Dec 2020 23:06:17 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8b8cab4641727c725ad37dfb802e7f58b88c0494b815f11a3f522ae94149f4c`  
		Last Modified: Wed, 30 Dec 2020 00:47:56 GMT  
		Size: 4.4 KB (4393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
