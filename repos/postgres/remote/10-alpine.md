## `postgres:10-alpine`

```console
$ docker pull postgres@sha256:5671bb6418f5bc488ad5773ba810728e0711d3491cdd2121aa8c554d3be44b3e
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

### `postgres:10-alpine` - linux; amd64

```console
$ docker pull postgres@sha256:3d37c3a047a67e6aa2837fdb5bd9c5d11c0e61327a333030ceb8335d32cb453c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.6 MB (28600999 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c9192ffc3b869e6e12ec10dbeb95395046d6b1b9f7318277a2023bc79868a8ef`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 28 Jan 2021 23:19:38 GMT
ADD file:0e2d487cd80773e947c8aae6daad3d565b7bb019a954af2b8bff188681c00d81 in / 
# Thu, 28 Jan 2021 23:19:38 GMT
CMD ["/bin/sh"]
# Fri, 29 Jan 2021 02:53:55 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Fri, 29 Jan 2021 02:53:55 GMT
ENV LANG=en_US.utf8
# Fri, 29 Jan 2021 02:53:56 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 29 Jan 2021 03:22:39 GMT
ENV PG_MAJOR=10
# Fri, 29 Jan 2021 03:22:40 GMT
ENV PG_VERSION=10.15
# Fri, 29 Jan 2021 03:22:40 GMT
ENV PG_SHA256=5956bce0becffa77883c41594c95a23110b94f10cd66a1157e373c3575921f7e
# Fri, 29 Jan 2021 03:29:06 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Fri, 29 Jan 2021 03:29:07 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Fri, 29 Jan 2021 03:29:08 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 29 Jan 2021 03:29:08 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 29 Jan 2021 03:29:09 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 29 Jan 2021 03:29:09 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 29 Jan 2021 03:29:10 GMT
COPY file:ad28506adc606e446eefc263bc99d4cb809e608d4f550956143bf13c82c91f85 in /usr/local/bin/ 
# Fri, 29 Jan 2021 03:29:11 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 29 Jan 2021 03:29:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 29 Jan 2021 03:29:11 GMT
STOPSIGNAL SIGINT
# Fri, 29 Jan 2021 03:29:11 GMT
EXPOSE 5432
# Fri, 29 Jan 2021 03:29:12 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:4c0d98bf9879488e0407f897d9dd4bf758555a78e39675e72b5124ccf12c2580`  
		Last Modified: Thu, 28 Jan 2021 23:20:08 GMT  
		Size: 2.8 MB (2811321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ff5918c11c3ab1f2763192c7c033f5dfe60b30d369a8aa483d65326974b637a`  
		Last Modified: Fri, 29 Jan 2021 03:42:07 GMT  
		Size: 1.2 KB (1248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c393806625cde0c68d6881aaeb6a8305d841ad1ec4e6152fe5dde27a6c7b4af8`  
		Last Modified: Fri, 29 Jan 2021 03:42:07 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca23c666401dffe77bf2556afb4d90da83dccfed83491b6da2ed25f234940c72`  
		Last Modified: Fri, 29 Jan 2021 03:43:18 GMT  
		Size: 25.8 MB (25776146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1502401f7b9200eb58436d9dc7c166653660eae726bd4848796f9d47a00cc59`  
		Last Modified: Fri, 29 Jan 2021 03:43:10 GMT  
		Size: 7.4 KB (7352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e8d15facca0af6b9cb7b6e425ac982c3e6cc251da3260494a55c76e43b6885b`  
		Last Modified: Fri, 29 Jan 2021 03:43:10 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5817b27484002c36f06d49e46bafbfb56c62c12071c715a4245a65538adc256b`  
		Last Modified: Fri, 29 Jan 2021 03:43:10 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0831f4af2123cfe641af3ef82c36fbda5e5bec81e285acb5f293599faf394ab`  
		Last Modified: Fri, 29 Jan 2021 03:43:10 GMT  
		Size: 4.4 KB (4404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea75e91d2311977bc1eac61358a9492507a0b70b464665eb94afb08c2d533335`  
		Last Modified: Fri, 29 Jan 2021 03:43:10 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:10-alpine` - linux; arm variant v6

```console
$ docker pull postgres@sha256:6cdf2b5660276257b6a631ff452057639174a17c491380b349904b961c1c95e4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.7 MB (27727985 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad6a0099b4951f46645a4b07afaadbed50713e9b79637952ef3838738fa1e5f0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 28 Jan 2021 23:49:59 GMT
ADD file:c197324e4979e2a7b257ad683d20dd9cbdae525a076bd68fe6aa0e0b126875df in / 
# Thu, 28 Jan 2021 23:49:59 GMT
CMD ["/bin/sh"]
# Fri, 29 Jan 2021 01:09:22 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Fri, 29 Jan 2021 01:09:23 GMT
ENV LANG=en_US.utf8
# Fri, 29 Jan 2021 01:09:25 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 29 Jan 2021 01:21:53 GMT
ENV PG_MAJOR=10
# Fri, 29 Jan 2021 01:21:54 GMT
ENV PG_VERSION=10.15
# Fri, 29 Jan 2021 01:21:55 GMT
ENV PG_SHA256=5956bce0becffa77883c41594c95a23110b94f10cd66a1157e373c3575921f7e
# Fri, 29 Jan 2021 01:24:52 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Fri, 29 Jan 2021 01:24:54 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Fri, 29 Jan 2021 01:24:56 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 29 Jan 2021 01:24:57 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 29 Jan 2021 01:25:02 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 29 Jan 2021 01:25:03 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 29 Jan 2021 01:25:04 GMT
COPY file:ad28506adc606e446eefc263bc99d4cb809e608d4f550956143bf13c82c91f85 in /usr/local/bin/ 
# Fri, 29 Jan 2021 01:25:06 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 29 Jan 2021 01:25:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 29 Jan 2021 01:25:07 GMT
STOPSIGNAL SIGINT
# Fri, 29 Jan 2021 01:25:08 GMT
EXPOSE 5432
# Fri, 29 Jan 2021 01:25:08 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:a66f440da051140fefcb0a520bdeb69d763b1eb4fd1b2ed46b4c0a168e335108`  
		Last Modified: Thu, 28 Jan 2021 23:50:33 GMT  
		Size: 2.6 MB (2621759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47814bcbfb45802646b189af4a9bc3e4510a538b55fd2808df448ec5e6491cff`  
		Last Modified: Fri, 29 Jan 2021 01:32:14 GMT  
		Size: 1.3 KB (1277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c6e4686dd674a32664773b275c120c9879a27454fb70c89ea4663315c3b84c6`  
		Last Modified: Fri, 29 Jan 2021 01:32:14 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db42f7907653e40a030fa547a79f883a24186581a398c0bff8dda012bdf572fd`  
		Last Modified: Fri, 29 Jan 2021 01:33:46 GMT  
		Size: 25.1 MB (25092565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb9dc901c92e8051f54f58df00f7fb11faafa1dbde265abe53b5c6401d171ec7`  
		Last Modified: Fri, 29 Jan 2021 01:33:36 GMT  
		Size: 7.4 KB (7356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:834f5570c7834f5a31a96d3844eecc75cd3547d148dfbcc5e01cf5e89b3b3d35`  
		Last Modified: Fri, 29 Jan 2021 01:33:36 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3814bea37ba6ef9d811b63a4231a0dd19938f8132d3080190a3fc69705c60ed1`  
		Last Modified: Fri, 29 Jan 2021 01:33:36 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34c5d6b2b2882e2b1df0edcae1f31c45a3d0f278a06ac4addcc5b084389606c4`  
		Last Modified: Fri, 29 Jan 2021 01:33:37 GMT  
		Size: 4.4 KB (4404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c10da2472460da8c48feda6cc7f04a95d9836980955825166f9ae0e095c340dc`  
		Last Modified: Fri, 29 Jan 2021 01:33:36 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:10-alpine` - linux; arm variant v7

```console
$ docker pull postgres@sha256:5c45b3d5bc5a00b5f27decbe47b836619fc10616056dfad1519effac01eff021
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.7 MB (26666229 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd5d19cc645fc3333023e75e676d5eb7816730b5d02df4d6a5706f73ba8e827f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 28 Jan 2021 23:58:03 GMT
ADD file:98a89b90a8b442eed5301790dd2bd3a27391c5e4426126eed9d1cf44e70f8857 in / 
# Thu, 28 Jan 2021 23:58:04 GMT
CMD ["/bin/sh"]
# Fri, 29 Jan 2021 01:46:41 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Fri, 29 Jan 2021 01:46:42 GMT
ENV LANG=en_US.utf8
# Fri, 29 Jan 2021 01:46:44 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 29 Jan 2021 01:59:26 GMT
ENV PG_MAJOR=10
# Fri, 29 Jan 2021 01:59:27 GMT
ENV PG_VERSION=10.15
# Fri, 29 Jan 2021 01:59:28 GMT
ENV PG_SHA256=5956bce0becffa77883c41594c95a23110b94f10cd66a1157e373c3575921f7e
# Fri, 29 Jan 2021 02:02:21 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Fri, 29 Jan 2021 02:02:24 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Fri, 29 Jan 2021 02:02:26 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 29 Jan 2021 02:02:26 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 29 Jan 2021 02:02:28 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 29 Jan 2021 02:02:29 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 29 Jan 2021 02:02:30 GMT
COPY file:ad28506adc606e446eefc263bc99d4cb809e608d4f550956143bf13c82c91f85 in /usr/local/bin/ 
# Fri, 29 Jan 2021 02:02:32 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 29 Jan 2021 02:02:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 29 Jan 2021 02:02:34 GMT
STOPSIGNAL SIGINT
# Fri, 29 Jan 2021 02:02:34 GMT
EXPOSE 5432
# Fri, 29 Jan 2021 02:02:35 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:9b1db703a337d301b1d50292acfbabd5fb3796511b962410c554420b85cd78dc`  
		Last Modified: Thu, 28 Jan 2021 23:58:38 GMT  
		Size: 2.4 MB (2423559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7fa668b3d0ed9168e26ae186f3e531d3ae1e280d94f950446b3683eaaab37c8`  
		Last Modified: Fri, 29 Jan 2021 02:09:19 GMT  
		Size: 1.3 KB (1274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61f921cd3d5ba006be49bcfc3c119ff3d8f5d35fbc011e764afbbce4ee5b61b4`  
		Last Modified: Fri, 29 Jan 2021 02:09:18 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f2032fcf6a526a10c71c788dbe7dfb90e232d455ff91328c5b519aab35af137`  
		Last Modified: Fri, 29 Jan 2021 02:10:57 GMT  
		Size: 24.2 MB (24229010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b80794d77d1d723b864db550c6868a4b2fb53292071b7f63310866c2a24c6019`  
		Last Modified: Fri, 29 Jan 2021 02:10:48 GMT  
		Size: 7.4 KB (7354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e5b51e549456fcdb4448f7db51e298c0a214d11214c59779280561989027e1e`  
		Last Modified: Fri, 29 Jan 2021 02:10:48 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abe9ed53f7c5ff4d16781cc8a6e479a7b59f10063cb5781f78c6e49e9d340ed9`  
		Last Modified: Fri, 29 Jan 2021 02:10:48 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a9e87bd4989f5bd69d36889c7516abaf0b2279287eb1581198b1aca8ed4c0d0`  
		Last Modified: Fri, 29 Jan 2021 02:10:48 GMT  
		Size: 4.4 KB (4408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51f0956cff6dab4e1f1ae80eb1bc986c064d01fa88f1ec9998406f2ce634f775`  
		Last Modified: Fri, 29 Jan 2021 02:10:48 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:10-alpine` - linux; arm64 variant v8

```console
$ docker pull postgres@sha256:2a0213e8b6fb04ea24ddbf640524de112e4867ef26ea8efb166e289f80ba0ab5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.3 MB (28307255 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe2755e09258c3e5c4df85fbe3fc13949d16055c34d3694de0184d0eccaefc91`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 28 Jan 2021 23:39:33 GMT
ADD file:fecabe41deaeb72acdd63023566d87ae48b013ef80c97fdd993b55d6c727da93 in / 
# Thu, 28 Jan 2021 23:39:34 GMT
CMD ["/bin/sh"]
# Fri, 29 Jan 2021 00:52:23 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Fri, 29 Jan 2021 00:52:24 GMT
ENV LANG=en_US.utf8
# Fri, 29 Jan 2021 00:52:26 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 29 Jan 2021 01:05:12 GMT
ENV PG_MAJOR=10
# Fri, 29 Jan 2021 01:05:12 GMT
ENV PG_VERSION=10.15
# Fri, 29 Jan 2021 01:05:13 GMT
ENV PG_SHA256=5956bce0becffa77883c41594c95a23110b94f10cd66a1157e373c3575921f7e
# Fri, 29 Jan 2021 01:08:15 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Fri, 29 Jan 2021 01:08:19 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Fri, 29 Jan 2021 01:08:21 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 29 Jan 2021 01:08:22 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 29 Jan 2021 01:08:24 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 29 Jan 2021 01:08:25 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 29 Jan 2021 01:08:26 GMT
COPY file:ad28506adc606e446eefc263bc99d4cb809e608d4f550956143bf13c82c91f85 in /usr/local/bin/ 
# Fri, 29 Jan 2021 01:08:28 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 29 Jan 2021 01:08:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 29 Jan 2021 01:08:30 GMT
STOPSIGNAL SIGINT
# Fri, 29 Jan 2021 01:08:30 GMT
EXPOSE 5432
# Fri, 29 Jan 2021 01:08:31 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:2914792bc417803b2106001990194cc00cdd4b6fd97cd21a368f26148bc8e722`  
		Last Modified: Thu, 28 Jan 2021 23:40:10 GMT  
		Size: 2.7 MB (2711261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84190c434223807f9b123dbab6b871f4d978fc7fcfb7bd372aae021a3f90b9cf`  
		Last Modified: Fri, 29 Jan 2021 01:16:24 GMT  
		Size: 1.3 KB (1278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a23887416d5dd038d93a43a59a6bc616f68e5f6805f3aadcedb9577d2274a5f0`  
		Last Modified: Fri, 29 Jan 2021 01:16:24 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc7629eb55466d1c1d9acf0787b15833972d3be605b555fb6999edc52c3844f9`  
		Last Modified: Fri, 29 Jan 2021 01:17:44 GMT  
		Size: 25.6 MB (25582333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fadaab76d780a994f451645480c45d01d017ee87bfac1b046b0456a8868e1973`  
		Last Modified: Fri, 29 Jan 2021 01:17:36 GMT  
		Size: 7.4 KB (7356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54aa33ec72372af3e42df69717cd8681bb9baf38b0700923550f54903ee00a77`  
		Last Modified: Fri, 29 Jan 2021 01:17:36 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aac298dafa9c0219d705098bff72a72c6fc30d39a6349ee9d64882e411d1796`  
		Last Modified: Fri, 29 Jan 2021 01:17:36 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1d05059b49eedf6ecd3f40f628e9891dbd4f886012f153d2861c1b544814984`  
		Last Modified: Fri, 29 Jan 2021 01:17:36 GMT  
		Size: 4.4 KB (4404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f59edc9022155e0f5ca62d023863de7ecb670e77cd4201a4695b39e4e90f6da`  
		Last Modified: Fri, 29 Jan 2021 01:17:36 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:10-alpine` - linux; 386

```console
$ docker pull postgres@sha256:7e41e2a920da0344c0b712ac662122a49d5a8ec0989ed97b504c772bf104c87c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.5 MB (29531556 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:559fc73d577388e30944967bbed55a9ed6c9d840920edcea3693baeb20cd8094`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 28 Jan 2021 23:38:31 GMT
ADD file:c0e9ea135d66ad6504c77915a7a48b3bead60892d155d3258b746cb4945981c0 in / 
# Thu, 28 Jan 2021 23:38:31 GMT
CMD ["/bin/sh"]
# Fri, 29 Jan 2021 03:03:57 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Fri, 29 Jan 2021 03:03:58 GMT
ENV LANG=en_US.utf8
# Fri, 29 Jan 2021 03:03:59 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 29 Jan 2021 03:41:30 GMT
ENV PG_MAJOR=10
# Fri, 29 Jan 2021 03:41:31 GMT
ENV PG_VERSION=10.15
# Fri, 29 Jan 2021 03:41:31 GMT
ENV PG_SHA256=5956bce0becffa77883c41594c95a23110b94f10cd66a1157e373c3575921f7e
# Fri, 29 Jan 2021 03:46:16 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Fri, 29 Jan 2021 03:46:17 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Fri, 29 Jan 2021 03:46:18 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 29 Jan 2021 03:46:18 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 29 Jan 2021 03:46:19 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 29 Jan 2021 03:46:19 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 29 Jan 2021 03:46:19 GMT
COPY file:ad28506adc606e446eefc263bc99d4cb809e608d4f550956143bf13c82c91f85 in /usr/local/bin/ 
# Fri, 29 Jan 2021 03:46:20 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 29 Jan 2021 03:46:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 29 Jan 2021 03:46:20 GMT
STOPSIGNAL SIGINT
# Fri, 29 Jan 2021 03:46:21 GMT
EXPOSE 5432
# Fri, 29 Jan 2021 03:46:21 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:3fea00a81341ce917db671eb3ad24ef5750cb6928b7f760e3ce4dab619eeb1fa`  
		Last Modified: Thu, 28 Jan 2021 23:39:02 GMT  
		Size: 2.8 MB (2817627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6577fee13210fe1c3f4549f1ef86d700f99fac79b2fdd5b840c7e298d9ff5899`  
		Last Modified: Fri, 29 Jan 2021 03:55:44 GMT  
		Size: 1.2 KB (1247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa4cc8bff7850ed45d5f7c08b1b4f9325ba2867fd9e91d3cbfa84e30234509ce`  
		Last Modified: Fri, 29 Jan 2021 03:55:44 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a73b7dcf6aa42fa89e8c81549de69f66f71dc3497f903b6f1d02d304456f326a`  
		Last Modified: Fri, 29 Jan 2021 03:56:53 GMT  
		Size: 26.7 MB (26700402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d10100541cb0ad2f55796111bb09723237277be96c814f2e7e957bcf9cb18e5b`  
		Last Modified: Fri, 29 Jan 2021 03:56:46 GMT  
		Size: 7.3 KB (7350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcada12fd49d3141b3fef53e2bf75fb304af7132f0b88862b52a17dc6e3f9cfb`  
		Last Modified: Fri, 29 Jan 2021 03:56:46 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62442906453d5fbbedab6b0131ecbeb34549c97cc7a6032f724165f60712914c`  
		Last Modified: Fri, 29 Jan 2021 03:56:46 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f044b493b2939a1a00d30a57d30e79bfc2f1998673ea713fabae49e0eb070310`  
		Last Modified: Fri, 29 Jan 2021 03:56:46 GMT  
		Size: 4.4 KB (4403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6902ed6bb616327da9fbf277fa38794710fed1f486ea21483bd5e86caa7588a`  
		Last Modified: Fri, 29 Jan 2021 03:56:46 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:10-alpine` - linux; ppc64le

```console
$ docker pull postgres@sha256:e4511e918d7fa74adbf4595aaca388ad77c15f25f4ba33bd196fdf874eb81a77
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.8 MB (29795843 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d9c5627b6fb40c282480cfe6e635a85d82ca57067e6ceafec50c2bdf1c5bbc01`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 28 Jan 2021 23:55:50 GMT
ADD file:b14fd5f3f7fcd16e2b4ec6932d3e9c07c7400c577cee5fdcb88b0795a70a7bfb in / 
# Thu, 28 Jan 2021 23:55:52 GMT
CMD ["/bin/sh"]
# Fri, 29 Jan 2021 01:48:47 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Fri, 29 Jan 2021 01:48:55 GMT
ENV LANG=en_US.utf8
# Fri, 29 Jan 2021 01:49:10 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 29 Jan 2021 02:09:49 GMT
ENV PG_MAJOR=10
# Fri, 29 Jan 2021 02:09:55 GMT
ENV PG_VERSION=10.15
# Fri, 29 Jan 2021 02:10:04 GMT
ENV PG_SHA256=5956bce0becffa77883c41594c95a23110b94f10cd66a1157e373c3575921f7e
# Fri, 29 Jan 2021 02:12:56 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Fri, 29 Jan 2021 02:13:11 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Fri, 29 Jan 2021 02:13:26 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 29 Jan 2021 02:13:31 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 29 Jan 2021 02:13:45 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 29 Jan 2021 02:13:48 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 29 Jan 2021 02:13:49 GMT
COPY file:ad28506adc606e446eefc263bc99d4cb809e608d4f550956143bf13c82c91f85 in /usr/local/bin/ 
# Fri, 29 Jan 2021 02:13:59 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 29 Jan 2021 02:14:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 29 Jan 2021 02:14:17 GMT
STOPSIGNAL SIGINT
# Fri, 29 Jan 2021 02:14:29 GMT
EXPOSE 5432
# Fri, 29 Jan 2021 02:14:44 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:f3b94a1d8d591af02f1b419642bee91066ecbb9c65099d6903deed310fd1c2ff`  
		Last Modified: Thu, 28 Jan 2021 23:56:32 GMT  
		Size: 2.8 MB (2812517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff06bd42b80b365bb0c19fbbbe316a95812c98b5963e0930ea89cc0c684a2833`  
		Last Modified: Fri, 29 Jan 2021 02:26:17 GMT  
		Size: 1.3 KB (1283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf320aafe224f5aad678f29f514b47d6d4aefcd42e80b7041098c1da820f8c23`  
		Last Modified: Fri, 29 Jan 2021 02:26:15 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae51640867957bd42ae6cdfc599550e9f7a4671f5f8d4dd442228a4e9559bc00`  
		Last Modified: Fri, 29 Jan 2021 02:27:40 GMT  
		Size: 27.0 MB (26969657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6c00e1f5fc529de558faac20e0db96b6fc774bc7540b1b894809bf9567d58f9`  
		Last Modified: Fri, 29 Jan 2021 02:27:31 GMT  
		Size: 7.4 KB (7355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:352632a8716965994b72d91f6b0b1e443cfc4e09cd4c6aee88aec92ca98cc05a`  
		Last Modified: Fri, 29 Jan 2021 02:27:31 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82eaac3292d852ef6f349736c63028f7d3b44e264eaa75823a32c454ae27cd31`  
		Last Modified: Fri, 29 Jan 2021 02:27:31 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3cf1f83a912999bde46490ae0ff87c725f30a09cfc72905843896c8b24be1ea`  
		Last Modified: Fri, 29 Jan 2021 02:27:31 GMT  
		Size: 4.4 KB (4405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:960de3f9271e0b1bcdb6455d84670e72009d74f88002e318c292f2100fd47848`  
		Last Modified: Fri, 29 Jan 2021 02:27:31 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:10-alpine` - linux; s390x

```console
$ docker pull postgres@sha256:7e60dfbf1d92138bbd2265b73a527cf6e8b92b539ccf91d4989af064d4ac3c73
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.5 MB (28457650 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:daae02091e869fb709830f1ab862abf1555bf04b635e4963ad18f2bf668a20a8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 28 Jan 2021 23:41:35 GMT
ADD file:d97e6c37df0fb8306b072d9c0a32f68f5aff583ba849303926644deacfa25eb9 in / 
# Thu, 28 Jan 2021 23:41:36 GMT
CMD ["/bin/sh"]
# Fri, 29 Jan 2021 01:28:50 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Fri, 29 Jan 2021 01:28:50 GMT
ENV LANG=en_US.utf8
# Fri, 29 Jan 2021 01:28:52 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 29 Jan 2021 01:42:12 GMT
ENV PG_MAJOR=10
# Fri, 29 Jan 2021 01:42:13 GMT
ENV PG_VERSION=10.15
# Fri, 29 Jan 2021 01:42:13 GMT
ENV PG_SHA256=5956bce0becffa77883c41594c95a23110b94f10cd66a1157e373c3575921f7e
# Fri, 29 Jan 2021 01:44:37 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Fri, 29 Jan 2021 01:44:41 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Fri, 29 Jan 2021 01:44:42 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 29 Jan 2021 01:44:43 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 29 Jan 2021 01:44:44 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 29 Jan 2021 01:44:44 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 29 Jan 2021 01:44:45 GMT
COPY file:ad28506adc606e446eefc263bc99d4cb809e608d4f550956143bf13c82c91f85 in /usr/local/bin/ 
# Fri, 29 Jan 2021 01:44:46 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 29 Jan 2021 01:44:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 29 Jan 2021 01:44:47 GMT
STOPSIGNAL SIGINT
# Fri, 29 Jan 2021 01:44:48 GMT
EXPOSE 5432
# Fri, 29 Jan 2021 01:44:48 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:43901f1af0ef9db6b0bf30ac6f6dacd78bf1ecfeb47ad0a93aa2370fa8e62407`  
		Last Modified: Thu, 28 Jan 2021 23:42:09 GMT  
		Size: 2.6 MB (2602059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddb7987d6a49388c77e555f2547e538d557a90c40b705e0fe10a7ef952d82326`  
		Last Modified: Fri, 29 Jan 2021 01:50:33 GMT  
		Size: 1.3 KB (1277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7d07431bbbdfa6c1540603fded3d65695c350f29a3aa77a1e475296db695a5a`  
		Last Modified: Fri, 29 Jan 2021 01:50:33 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3793cce03eadecb73b6dbf5b34eb6a67cc01eacbe31ff3a3974721e06b0b89f6`  
		Last Modified: Fri, 29 Jan 2021 01:51:35 GMT  
		Size: 25.8 MB (25841923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d73b9b5491c95f50cabe422aad7a8b98d2423dead2006d1bfb674a12eed0f03`  
		Last Modified: Fri, 29 Jan 2021 01:51:30 GMT  
		Size: 7.4 KB (7356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6734291eeea407bc62ed37eb02ad3cdadc847d5cb585991a3104e63d2ea69ac`  
		Last Modified: Fri, 29 Jan 2021 01:51:30 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af00f8e7ba724c6a88974b558250616ef116cfd35637013a80cc79b6d17d5a10`  
		Last Modified: Fri, 29 Jan 2021 01:51:30 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a55cf0bf03a47187620ea2e012ebdd448cd41baf447c6cea6502248eeaa3ebc`  
		Last Modified: Fri, 29 Jan 2021 01:51:30 GMT  
		Size: 4.4 KB (4408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e02096a48f4d83a5a22c6e3fe9bb4c969cb680b5baf6304453c23df2185dd956`  
		Last Modified: Fri, 29 Jan 2021 01:51:30 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
