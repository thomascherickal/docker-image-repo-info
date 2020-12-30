## `postgres:alpine`

```console
$ docker pull postgres@sha256:0b6f8681377407396a54512812789bd311afd40b2b4e2bd66e9d98da6632bd8e
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

### `postgres:alpine` - linux; amd64

```console
$ docker pull postgres@sha256:46238011dbb12be5085afcafa6acd1cbaeb216691a2597106cffa61f08cfb489
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.1 MB (62147638 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af0d7cbad48805d9015cc3002bfaa7b0df78adb3b15e2ecf1c7d8195986f3aea`
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
# Thu, 17 Dec 2020 00:59:50 GMT
ENV PG_MAJOR=13
# Thu, 17 Dec 2020 00:59:50 GMT
ENV PG_VERSION=13.1
# Thu, 17 Dec 2020 00:59:50 GMT
ENV PG_SHA256=12345c83b89aa29808568977f5200d6da00f88a035517f925293355432ffe61f
# Thu, 17 Dec 2020 01:07:26 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm10-dev clang g++ 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Thu, 17 Dec 2020 01:07:27 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Thu, 17 Dec 2020 01:07:28 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 17 Dec 2020 01:07:29 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 17 Dec 2020 01:07:30 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 17 Dec 2020 01:07:30 GMT
VOLUME [/var/lib/postgresql/data]
# Wed, 30 Dec 2020 01:22:14 GMT
COPY file:f937c0ee3ab8736d7adeefe3108ce546c352d85751a620058fb9427c3648a82c in /usr/local/bin/ 
# Wed, 30 Dec 2020 01:22:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 30 Dec 2020 01:22:15 GMT
STOPSIGNAL SIGINT
# Wed, 30 Dec 2020 01:22:15 GMT
EXPOSE 5432
# Wed, 30 Dec 2020 01:22:15 GMT
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
	-	`sha256:3a275fa239f9449c942f63286bfe1f61077be4d7584caec0fdd4ac4e028e0da7`  
		Last Modified: Thu, 17 Dec 2020 01:35:59 GMT  
		Size: 59.3 MB (59333991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c21807b4162fd9c2bcd091d5bf7cb31d017b9871bba424fc5d3c67153afe5453`  
		Last Modified: Thu, 17 Dec 2020 01:35:44 GMT  
		Size: 8.5 KB (8535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93a017299b14c6e937ab85548274e213f3c1eaeef735bbbb1ccd827049ea54a3`  
		Last Modified: Thu, 17 Dec 2020 01:35:43 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3abc374c6f01b6e43a24fb01099ee3963fd2a971f8e01784e2836adc79e33e09`  
		Last Modified: Thu, 17 Dec 2020 01:35:43 GMT  
		Size: 164.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d9ceaad66dbe3ba82c9c069d8f9858b06508b93d9d3058b4f14d738b36f8707`  
		Last Modified: Wed, 30 Dec 2020 01:23:56 GMT  
		Size: 4.4 KB (4390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:alpine` - linux; arm variant v6

```console
$ docker pull postgres@sha256:acc4d5673f5454f9049aa84c747d2f2e67437b7aa33ec3b0a2d80508df5ce304
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.3 MB (60324677 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ef2e937e1b042c6e83f37c058e5d6d989418e384a0d4d5434b2c51a58112aad`
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
# Thu, 17 Dec 2020 05:45:19 GMT
ENV PG_MAJOR=13
# Thu, 17 Dec 2020 05:45:22 GMT
ENV PG_VERSION=13.1
# Thu, 17 Dec 2020 05:45:24 GMT
ENV PG_SHA256=12345c83b89aa29808568977f5200d6da00f88a035517f925293355432ffe61f
# Thu, 17 Dec 2020 05:49:59 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm10-dev clang g++ 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Thu, 17 Dec 2020 05:50:03 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Thu, 17 Dec 2020 05:50:05 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 17 Dec 2020 05:50:06 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 17 Dec 2020 05:50:08 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 17 Dec 2020 05:50:10 GMT
VOLUME [/var/lib/postgresql/data]
# Wed, 30 Dec 2020 00:54:59 GMT
COPY file:f937c0ee3ab8736d7adeefe3108ce546c352d85751a620058fb9427c3648a82c in /usr/local/bin/ 
# Wed, 30 Dec 2020 00:55:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 30 Dec 2020 00:55:00 GMT
STOPSIGNAL SIGINT
# Wed, 30 Dec 2020 00:55:01 GMT
EXPOSE 5432
# Wed, 30 Dec 2020 00:55:01 GMT
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
	-	`sha256:eb594a5322d81fcfefa44de4e53163ed93b9b6964d4eddf3676b3242fb94742e`  
		Last Modified: Thu, 17 Dec 2020 06:07:55 GMT  
		Size: 57.7 MB (57705801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:347019afe45ebfc73472e4fb0fea5c20c7bfa37dfa628e96ed876ebae6787a54`  
		Last Modified: Thu, 17 Dec 2020 06:07:38 GMT  
		Size: 8.5 KB (8541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9d522100c8d1d76509a0bd1608a77aec87316b85301bb6a37a24bd087aeddbb`  
		Last Modified: Thu, 17 Dec 2020 06:07:39 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:780b73fc4b543e656e96b4b32b7f7ad25a675f55be047b0ff4e04ba284f6f5ad`  
		Last Modified: Thu, 17 Dec 2020 06:07:38 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05391215f56f585cca5823f1ec4a25b54be9030d2f30f6c46a4861708dffbe34`  
		Last Modified: Wed, 30 Dec 2020 00:56:38 GMT  
		Size: 4.4 KB (4393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:alpine` - linux; arm variant v7

```console
$ docker pull postgres@sha256:e058ff761ffcd809ec4bfec33147c0c9349d1c06c573812fd7f5ecc94e02b013
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.4 MB (57431851 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8d5fafcc4941b0577b0fd76a4c28ba12371cf41006c39943d8ad10441f0ae2a3`
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
# Thu, 17 Dec 2020 05:36:06 GMT
ENV PG_MAJOR=13
# Thu, 17 Dec 2020 05:36:07 GMT
ENV PG_VERSION=13.1
# Thu, 17 Dec 2020 05:36:08 GMT
ENV PG_SHA256=12345c83b89aa29808568977f5200d6da00f88a035517f925293355432ffe61f
# Thu, 17 Dec 2020 05:39:23 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm10-dev clang g++ 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Thu, 17 Dec 2020 05:39:26 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Thu, 17 Dec 2020 05:39:28 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 17 Dec 2020 05:39:29 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 17 Dec 2020 05:39:32 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 17 Dec 2020 05:39:33 GMT
VOLUME [/var/lib/postgresql/data]
# Wed, 30 Dec 2020 01:01:31 GMT
COPY file:f937c0ee3ab8736d7adeefe3108ce546c352d85751a620058fb9427c3648a82c in /usr/local/bin/ 
# Wed, 30 Dec 2020 01:01:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 30 Dec 2020 01:01:38 GMT
STOPSIGNAL SIGINT
# Wed, 30 Dec 2020 01:01:41 GMT
EXPOSE 5432
# Wed, 30 Dec 2020 01:01:44 GMT
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
	-	`sha256:49cf38f522b2fd2e6c72e662b87b38203940909e820b2ef32561fefbb916dbdd`  
		Last Modified: Thu, 17 Dec 2020 05:59:03 GMT  
		Size: 55.0 MB (55009574 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6698b35172a4fc20b464c314531bef8430d2ba112ba3eb0861a26771a45929cf`  
		Last Modified: Thu, 17 Dec 2020 05:58:46 GMT  
		Size: 8.5 KB (8542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:639634e1734d696dda9e0927037cd3376987553d71dbc9abd197d08b55643414`  
		Last Modified: Thu, 17 Dec 2020 05:58:46 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4782a9fd2123c66e10e80e04635adb4b11d594fe8f78a331aea97dae4311a96b`  
		Last Modified: Thu, 17 Dec 2020 05:58:46 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92638f73e8cabec107f1619f8e86ee44d126d4d6ccd4b710b281da556cc229fa`  
		Last Modified: Wed, 30 Dec 2020 01:04:55 GMT  
		Size: 4.4 KB (4398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:alpine` - linux; arm64 variant v8

```console
$ docker pull postgres@sha256:00ad028fbc953c4ee916521113da71e2894b739f9c8934ed7a3c854d19a7626e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.7 MB (61685336 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66659230f7b7001d1dcb320f48b98d4b16316286bc3cdfae3cc3794e86138251`
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
# Thu, 17 Dec 2020 04:01:29 GMT
ENV PG_MAJOR=13
# Thu, 17 Dec 2020 04:01:30 GMT
ENV PG_VERSION=13.1
# Thu, 17 Dec 2020 04:01:31 GMT
ENV PG_SHA256=12345c83b89aa29808568977f5200d6da00f88a035517f925293355432ffe61f
# Thu, 17 Dec 2020 04:05:37 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm10-dev clang g++ 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Thu, 17 Dec 2020 04:05:46 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Thu, 17 Dec 2020 04:05:52 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 17 Dec 2020 04:05:55 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 17 Dec 2020 04:06:00 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 17 Dec 2020 04:06:01 GMT
VOLUME [/var/lib/postgresql/data]
# Wed, 30 Dec 2020 00:42:22 GMT
COPY file:f937c0ee3ab8736d7adeefe3108ce546c352d85751a620058fb9427c3648a82c in /usr/local/bin/ 
# Wed, 30 Dec 2020 00:42:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 30 Dec 2020 00:42:27 GMT
STOPSIGNAL SIGINT
# Wed, 30 Dec 2020 00:42:30 GMT
EXPOSE 5432
# Wed, 30 Dec 2020 00:42:38 GMT
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
	-	`sha256:c8812dbcb6a583481fae5bf941ffb3bff7aad42c81de03bcedcf1e1ce2806ec2`  
		Last Modified: Thu, 17 Dec 2020 04:28:19 GMT  
		Size: 59.0 MB (58961571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afb4f04eea5ca85153647c6188f3c9cc2635b1bebee270af77d4c18300157a8b`  
		Last Modified: Thu, 17 Dec 2020 04:28:02 GMT  
		Size: 8.5 KB (8540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f725905c09b804f3750a743577f6e304829142bb2f5d901c69c28681b7e0fc9`  
		Last Modified: Thu, 17 Dec 2020 04:28:03 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bbfc23e7ec314948eeb482b450f6cbddd81c920a30afaac4884cf09f0d6184f`  
		Last Modified: Thu, 17 Dec 2020 04:28:02 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:469ca852de68e007c80f1f64d44f407e90eff175b6d4866dc9c037f940c11310`  
		Last Modified: Wed, 30 Dec 2020 00:47:33 GMT  
		Size: 4.4 KB (4391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:alpine` - linux; 386

```console
$ docker pull postgres@sha256:aec2c5304258f4d27f7cdee5a691c1e888d6a9b8657b3db85dcab09464457020
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.7 MB (65738391 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:41b5ab92a12e5b8590e1e839618341b2157583f3472254914c56855fd0e176ae`
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
# Thu, 17 Dec 2020 05:49:57 GMT
ENV PG_MAJOR=13
# Thu, 17 Dec 2020 05:49:57 GMT
ENV PG_VERSION=13.1
# Thu, 17 Dec 2020 05:49:57 GMT
ENV PG_SHA256=12345c83b89aa29808568977f5200d6da00f88a035517f925293355432ffe61f
# Thu, 17 Dec 2020 05:57:07 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm10-dev clang g++ 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Thu, 17 Dec 2020 05:57:07 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Thu, 17 Dec 2020 05:57:08 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 17 Dec 2020 05:57:08 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 17 Dec 2020 05:57:09 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 17 Dec 2020 05:57:09 GMT
VOLUME [/var/lib/postgresql/data]
# Wed, 30 Dec 2020 00:41:11 GMT
COPY file:f937c0ee3ab8736d7adeefe3108ce546c352d85751a620058fb9427c3648a82c in /usr/local/bin/ 
# Wed, 30 Dec 2020 00:41:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 30 Dec 2020 00:41:12 GMT
STOPSIGNAL SIGINT
# Wed, 30 Dec 2020 00:41:12 GMT
EXPOSE 5432
# Wed, 30 Dec 2020 00:41:12 GMT
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
	-	`sha256:e340a56575069936b37b1ee040abaa9979da6376109bd110b202290bf505dfe2`  
		Last Modified: Thu, 17 Dec 2020 06:07:58 GMT  
		Size: 62.9 MB (62929678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e38584d9edcba293b996bbc1073a3358851aeff0ed95c324fcc0a8d7a73426f7`  
		Last Modified: Thu, 17 Dec 2020 06:07:44 GMT  
		Size: 8.5 KB (8537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bb25590214af19ac96d5030deb1ebaad7a7783deb371736039cef95fe4c1af6`  
		Last Modified: Thu, 17 Dec 2020 06:07:44 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b625691f2e5236b2d155f440becbb46ceed37be400b817cad3bcbd4ba42eda55`  
		Last Modified: Thu, 17 Dec 2020 06:07:44 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb492d00ce7ab69f967096d9ba87da3d49c3b2823d4f3f2f20c74aa5639538c6`  
		Last Modified: Wed, 30 Dec 2020 00:42:50 GMT  
		Size: 4.4 KB (4392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:alpine` - linux; ppc64le

```console
$ docker pull postgres@sha256:c5f0759c12c24f0df755e8b2af0dc5ce95d1e42bb197ee5f0c1fdc6b25372cad
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.5 MB (64546434 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fcf6f57883e60bc3d148181b3ff7162a73b689a4d1fc4b81e31c1ebe8e417d98`
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
# Thu, 17 Dec 2020 08:27:21 GMT
ENV PG_MAJOR=13
# Thu, 17 Dec 2020 08:27:27 GMT
ENV PG_VERSION=13.1
# Thu, 17 Dec 2020 08:27:29 GMT
ENV PG_SHA256=12345c83b89aa29808568977f5200d6da00f88a035517f925293355432ffe61f
# Thu, 17 Dec 2020 08:31:28 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm10-dev clang g++ 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Thu, 17 Dec 2020 08:31:42 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Thu, 17 Dec 2020 08:31:49 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 17 Dec 2020 08:31:50 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 17 Dec 2020 08:31:58 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 17 Dec 2020 08:32:01 GMT
VOLUME [/var/lib/postgresql/data]
# Wed, 30 Dec 2020 01:18:48 GMT
COPY file:f937c0ee3ab8736d7adeefe3108ce546c352d85751a620058fb9427c3648a82c in /usr/local/bin/ 
# Wed, 30 Dec 2020 01:18:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 30 Dec 2020 01:18:56 GMT
STOPSIGNAL SIGINT
# Wed, 30 Dec 2020 01:19:00 GMT
EXPOSE 5432
# Wed, 30 Dec 2020 01:19:02 GMT
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
	-	`sha256:55519394a52cd2dc8ad21ec63965bc01e96f3a1c3cbd080bd18c6f6f17dd5e4e`  
		Last Modified: Thu, 17 Dec 2020 08:55:25 GMT  
		Size: 61.7 MB (61726498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9f310f2298fed1a0890ede9fbcdedc6206da5c5290d26bb45a1411f62f87cf1`  
		Last Modified: Thu, 17 Dec 2020 08:55:13 GMT  
		Size: 8.5 KB (8535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9d4adb4ea4daef7d28935418344f7142d319ea5a47c6af899682e043dfad4d9`  
		Last Modified: Thu, 17 Dec 2020 08:55:13 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb22c16548b86b2300fb7dac1bd085ccb7d4e63e0fc777804c67924f203b7374`  
		Last Modified: Thu, 17 Dec 2020 08:55:13 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2cf05987bb92438e84f51168c996342ce55473358581d29975d2ce5dba7d10a`  
		Last Modified: Wed, 30 Dec 2020 01:22:39 GMT  
		Size: 4.4 KB (4389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:alpine` - linux; s390x

```console
$ docker pull postgres@sha256:5614c77315dade2076c38b144788af0993b8c25708ece6e225e69de7b74ce976
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.6 MB (64604197 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e22fdbd0f10687f1fbd87efbde9d2677a7142bd09b897962d898ad902bf0e94a`
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
# Thu, 17 Dec 2020 09:43:59 GMT
ENV PG_MAJOR=13
# Thu, 17 Dec 2020 09:44:00 GMT
ENV PG_VERSION=13.1
# Thu, 17 Dec 2020 09:44:01 GMT
ENV PG_SHA256=12345c83b89aa29808568977f5200d6da00f88a035517f925293355432ffe61f
# Fri, 18 Dec 2020 22:42:19 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm10-dev clang g++ 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Fri, 18 Dec 2020 22:42:29 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Fri, 18 Dec 2020 22:42:30 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 18 Dec 2020 22:42:31 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 18 Dec 2020 22:42:33 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 18 Dec 2020 22:42:33 GMT
VOLUME [/var/lib/postgresql/data]
# Wed, 30 Dec 2020 00:45:44 GMT
COPY file:f937c0ee3ab8736d7adeefe3108ce546c352d85751a620058fb9427c3648a82c in /usr/local/bin/ 
# Wed, 30 Dec 2020 00:45:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 30 Dec 2020 00:45:45 GMT
STOPSIGNAL SIGINT
# Wed, 30 Dec 2020 00:45:45 GMT
EXPOSE 5432
# Wed, 30 Dec 2020 00:45:46 GMT
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
	-	`sha256:d44e082471c4c992f8fd5ecd9867a97d90e6cdfe1b869dd98f8b473a01fc2ddf`  
		Last Modified: Fri, 18 Dec 2020 23:06:05 GMT  
		Size: 62.0 MB (62022463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cec2f81f6b94dbf52b031da2eb28c2def3949e8b609918540cbb09c793d42983`  
		Last Modified: Fri, 18 Dec 2020 23:05:47 GMT  
		Size: 8.5 KB (8534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa690081a578e4edc322d789ae53e0b4e3d73c13b997dcf938a004c3f98362aa`  
		Last Modified: Fri, 18 Dec 2020 23:05:47 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cbbcab6d197a8839fbd1f41ba79f0e8933d744c2cb0e57686368fab85bbe927`  
		Last Modified: Fri, 18 Dec 2020 23:05:46 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1bebfc3c4acc8afaa603c62f9e27137a6615c344fad4125ba15891a175f3624`  
		Last Modified: Wed, 30 Dec 2020 00:47:31 GMT  
		Size: 4.4 KB (4398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
