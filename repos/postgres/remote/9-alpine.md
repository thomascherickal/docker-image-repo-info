## `postgres:9-alpine`

```console
$ docker pull postgres@sha256:14261ff7942debcb1b80378698f8b0b24f6e1f7243c43fe7aeba088cbbcf7472
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

### `postgres:9-alpine` - linux; amd64

```console
$ docker pull postgres@sha256:605e911ed92f9e1c41b88bfa55828986e92c8a953703a45659aab04aafc3ed03
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.2 MB (14220704 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c0d2dcd3fa66768e7190f58b213103f51f86a26e38961db9616fddbf9bd3f721`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Mon, 23 Mar 2020 21:19:34 GMT
ADD file:0c4555f363c2672e350001f1293e689875a3760afe7b3f9146886afe67121cba in / 
# Mon, 23 Mar 2020 21:19:34 GMT
CMD ["/bin/sh"]
# Mon, 23 Mar 2020 23:47:57 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Mon, 23 Mar 2020 23:47:57 GMT
ENV LANG=en_US.utf8
# Mon, 23 Mar 2020 23:47:58 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 24 Mar 2020 00:15:56 GMT
ENV PG_MAJOR=9.6
# Tue, 24 Mar 2020 00:15:57 GMT
ENV PG_VERSION=9.6.17
# Tue, 24 Mar 2020 00:15:57 GMT
ENV PG_SHA256=f6e1e32d32545f97c066f3c19f4d58dfab1205c01252cf85c5c92294ace1a0c2
# Tue, 24 Mar 2020 00:21:26 GMT
RUN set -ex 		&& apk add --no-cache --virtual .fetch-deps 		ca-certificates 		openssl 		tar 		&& wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2" 	&& echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c - 	&& mkdir -p /usr/src/postgresql 	&& tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	&& rm postgresql.tar.bz2 		&& apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		&& cd /usr/src/postgresql 	&& awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new 	&& grep '/var/run/postgresql' src/include/pg_config_manual.h.new 	&& mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& ./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 	&& make -j "$(nproc)" world 	&& make install-world 	&& make -C contrib install 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	&& apk del .fetch-deps .build-deps 	&& cd / 	&& rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	&& find /usr/local -name '*.a' -delete
# Tue, 24 Mar 2020 00:21:27 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Tue, 24 Mar 2020 00:21:29 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 24 Mar 2020 00:21:29 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 24 Mar 2020 00:21:31 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 24 Mar 2020 00:21:31 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 24 Mar 2020 00:21:32 GMT
COPY file:8241ba12b253167d267d2d8aba237bf478f6de0a6f29aa61515376f105626d03 in /usr/local/bin/ 
# Tue, 24 Mar 2020 00:21:33 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Tue, 24 Mar 2020 00:21:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 24 Mar 2020 00:21:34 GMT
EXPOSE 5432
# Tue, 24 Mar 2020 00:21:34 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:aad63a9339440e7c3e1fff2b988991b9bfb81280042fa7f39a5e327023056819`  
		Last Modified: Mon, 23 Mar 2020 21:19:53 GMT  
		Size: 2.8 MB (2803255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5b4c973b808455b5a0f405abb1ae54c769bf4a42a7af686fc96b4469b3444e5`  
		Last Modified: Tue, 24 Mar 2020 00:28:16 GMT  
		Size: 1.2 KB (1246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:074a034a3a7aef9e887181bce1bf5fcf938f0c6d5ac8929d6139853efa4c850b`  
		Last Modified: Tue, 24 Mar 2020 00:28:16 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0cc5c471b463226efd69d3833052aa09d9ea90bb3d523221288aa250a22249e`  
		Last Modified: Tue, 24 Mar 2020 00:29:18 GMT  
		Size: 11.4 MB (11404257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b515caa102b90c3f4872556993275d76ae270e11b45256cbca6559e2ee9f06f`  
		Last Modified: Tue, 24 Mar 2020 00:29:14 GMT  
		Size: 7.2 KB (7154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff417e23115a0b32178392ca1e7c9c4d15adac4d6f9bfeca7c44b9f08381434b`  
		Last Modified: Tue, 24 Mar 2020 00:29:13 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15675b8430d7a68f6d88f5faa2f49975a88aa19ea0eacdbfc467712437bdcede`  
		Last Modified: Tue, 24 Mar 2020 00:29:14 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a92cb200dd03b523b0a676b45c51799cd7329a34255a531ec750f4a074a98b0e`  
		Last Modified: Tue, 24 Mar 2020 00:29:13 GMT  
		Size: 4.3 KB (4264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:056ca6be8aefeff7674fe3a59ca95feeeea3f7a9eef2b34b13d600a9fb1f87d2`  
		Last Modified: Tue, 24 Mar 2020 00:29:13 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:9-alpine` - linux; arm variant v6

```console
$ docker pull postgres@sha256:b353078319add7865c23f1ae9ffaf86dd4a445c72ad93b73b86a29c61772d75a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.6 MB (13617014 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b23d6273b6624e38054573d84f483976b2f8f94e3b4ca6efe3278b83b3f76f08`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Mon, 23 Mar 2020 21:49:26 GMT
ADD file:e2fdfc637b534345942caf4097883508a5ed23be97d85ccc3357b8277aaa5430 in / 
# Mon, 23 Mar 2020 21:49:27 GMT
CMD ["/bin/sh"]
# Mon, 23 Mar 2020 23:26:16 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Mon, 23 Mar 2020 23:26:17 GMT
ENV LANG=en_US.utf8
# Mon, 23 Mar 2020 23:26:19 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Mon, 23 Mar 2020 23:39:23 GMT
ENV PG_MAJOR=9.6
# Mon, 23 Mar 2020 23:39:24 GMT
ENV PG_VERSION=9.6.17
# Mon, 23 Mar 2020 23:39:25 GMT
ENV PG_SHA256=f6e1e32d32545f97c066f3c19f4d58dfab1205c01252cf85c5c92294ace1a0c2
# Mon, 23 Mar 2020 23:42:04 GMT
RUN set -ex 		&& apk add --no-cache --virtual .fetch-deps 		ca-certificates 		openssl 		tar 		&& wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2" 	&& echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c - 	&& mkdir -p /usr/src/postgresql 	&& tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	&& rm postgresql.tar.bz2 		&& apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		&& cd /usr/src/postgresql 	&& awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new 	&& grep '/var/run/postgresql' src/include/pg_config_manual.h.new 	&& mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& ./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 	&& make -j "$(nproc)" world 	&& make install-world 	&& make -C contrib install 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	&& apk del .fetch-deps .build-deps 	&& cd / 	&& rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	&& find /usr/local -name '*.a' -delete
# Mon, 23 Mar 2020 23:42:06 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Mon, 23 Mar 2020 23:42:09 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Mon, 23 Mar 2020 23:42:10 GMT
ENV PGDATA=/var/lib/postgresql/data
# Mon, 23 Mar 2020 23:42:12 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Mon, 23 Mar 2020 23:42:13 GMT
VOLUME [/var/lib/postgresql/data]
# Mon, 23 Mar 2020 23:42:14 GMT
COPY file:8241ba12b253167d267d2d8aba237bf478f6de0a6f29aa61515376f105626d03 in /usr/local/bin/ 
# Mon, 23 Mar 2020 23:42:16 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Mon, 23 Mar 2020 23:42:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 23 Mar 2020 23:42:18 GMT
EXPOSE 5432
# Mon, 23 Mar 2020 23:42:19 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:0776aeec3430c5a5ba3f43937f0ee6a7770a1fe81a318c9d94cc76512e5375e9`  
		Last Modified: Mon, 23 Mar 2020 21:49:50 GMT  
		Size: 2.6 MB (2618579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d97752a4ca8f8fc42bf0639a04a1c8bb9244ebdf4bf1c009b9aa4e4f5f3bcd7`  
		Last Modified: Mon, 23 Mar 2020 23:45:21 GMT  
		Size: 1.3 KB (1276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ae682c8811415ca60e2e25e0806be8a3ce9ca960ca7a0d4d0b0c86a0a274956`  
		Last Modified: Mon, 23 Mar 2020 23:44:01 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f827abf4bf4c411d515c269d203e1e88e23f2b0440896e811456309406edd080`  
		Last Modified: Mon, 23 Mar 2020 23:46:34 GMT  
		Size: 11.0 MB (10985112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e906e65471f0e2dd737431a6a38ebf8ed611349e6fc4327a421d95b6cc940ed5`  
		Last Modified: Mon, 23 Mar 2020 23:46:27 GMT  
		Size: 7.2 KB (7159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da368a2e4f52374bfcf48fe231bdfaf8d15304bca5bdce97ab454d076e718519`  
		Last Modified: Mon, 23 Mar 2020 23:46:27 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fd42d9182f7f5a77f25e05edefdc991942280ef4cd367ac20004c354c4d1f3e`  
		Last Modified: Mon, 23 Mar 2020 23:46:27 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e442dcf5d1577c0965649e5d3a31c3d93e701b93eec9e98af1d2655eef4b6f0f`  
		Last Modified: Mon, 23 Mar 2020 23:46:27 GMT  
		Size: 4.3 KB (4261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9220e4d8bee2fabd21825c4d5d23616b5b0d437084c3f99fd9d4d26d1827fb3d`  
		Last Modified: Mon, 23 Mar 2020 23:46:27 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:9-alpine` - linux; arm variant v7

```console
$ docker pull postgres@sha256:56f34be438d8e1f9ecdb0e04842c998dbd3756bb79ca7de7107a3ddf0f76efe2
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **12.8 MB (12779989 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ed1ae3eb81323408db7ece34408d43a3bc1be546edac5994429bdec9fc50aa1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Mon, 23 Mar 2020 21:57:55 GMT
ADD file:3bde6b6fd06efbf24e66446c6d32f72294fc749ae9ee6191776242e92b2f8ab4 in / 
# Mon, 23 Mar 2020 21:57:56 GMT
CMD ["/bin/sh"]
# Mon, 23 Mar 2020 22:43:21 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Mon, 23 Mar 2020 22:43:21 GMT
ENV LANG=en_US.utf8
# Mon, 23 Mar 2020 22:43:23 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Mon, 23 Mar 2020 22:56:34 GMT
ENV PG_MAJOR=9.6
# Mon, 23 Mar 2020 22:56:35 GMT
ENV PG_VERSION=9.6.17
# Mon, 23 Mar 2020 22:56:36 GMT
ENV PG_SHA256=f6e1e32d32545f97c066f3c19f4d58dfab1205c01252cf85c5c92294ace1a0c2
# Mon, 23 Mar 2020 22:58:43 GMT
RUN set -ex 		&& apk add --no-cache --virtual .fetch-deps 		ca-certificates 		openssl 		tar 		&& wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2" 	&& echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c - 	&& mkdir -p /usr/src/postgresql 	&& tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	&& rm postgresql.tar.bz2 		&& apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		&& cd /usr/src/postgresql 	&& awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new 	&& grep '/var/run/postgresql' src/include/pg_config_manual.h.new 	&& mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& ./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 	&& make -j "$(nproc)" world 	&& make install-world 	&& make -C contrib install 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	&& apk del .fetch-deps .build-deps 	&& cd / 	&& rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	&& find /usr/local -name '*.a' -delete
# Mon, 23 Mar 2020 22:58:46 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Mon, 23 Mar 2020 22:58:48 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Mon, 23 Mar 2020 22:58:49 GMT
ENV PGDATA=/var/lib/postgresql/data
# Mon, 23 Mar 2020 22:58:50 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Mon, 23 Mar 2020 22:58:51 GMT
VOLUME [/var/lib/postgresql/data]
# Mon, 23 Mar 2020 22:58:52 GMT
COPY file:8241ba12b253167d267d2d8aba237bf478f6de0a6f29aa61515376f105626d03 in /usr/local/bin/ 
# Mon, 23 Mar 2020 22:58:54 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Mon, 23 Mar 2020 22:58:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 23 Mar 2020 22:58:55 GMT
EXPOSE 5432
# Mon, 23 Mar 2020 22:58:56 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:d9bf605ce3d4449f4b90035c3e21d691806324781d43a5287b1da25a01779d6b`  
		Last Modified: Mon, 23 Mar 2020 21:58:16 GMT  
		Size: 2.4 MB (2420493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d48d9b30ccc2f0daa550064546b02eddaa410c0a5ff36be31fc55c747b40e0ad`  
		Last Modified: Mon, 23 Mar 2020 23:02:11 GMT  
		Size: 1.3 KB (1277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a59176775d1234d40a9b589b93b12933263fc13cde3b8672653317d01d4203e6`  
		Last Modified: Mon, 23 Mar 2020 23:02:11 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f09f9534d64f96d217d9259df44c8becc6d3a35fde8bc0371ed5963ae147e96`  
		Last Modified: Mon, 23 Mar 2020 23:03:20 GMT  
		Size: 10.3 MB (10346168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af936862cc0c16467f42190d2c53ec07fb515be12152fc1889ff517579848f92`  
		Last Modified: Mon, 23 Mar 2020 23:03:13 GMT  
		Size: 7.2 KB (7158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4346e494999457bb035b20477fa6acd602d458cb1c777e77eeb3f931e66023e1`  
		Last Modified: Mon, 23 Mar 2020 23:03:13 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:068c355f26e00e6cfebfa0f307a9d5767c9fe15c9feb9ff71811c7b9c1bc3f1e`  
		Last Modified: Mon, 23 Mar 2020 23:03:13 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ee050838026f74f3731860860c70acf7abca4f59e7b7e89063de6004c0d53b0`  
		Last Modified: Mon, 23 Mar 2020 23:03:13 GMT  
		Size: 4.3 KB (4264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d13dc10adf9994aa5bb5b0ce93aaed98f69f54e4520991a18198d169f435e36`  
		Last Modified: Mon, 23 Mar 2020 23:03:13 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:9-alpine` - linux; arm64 variant v8

```console
$ docker pull postgres@sha256:6ba0936298f3f05dc7d4c0b166b7aa1642bcaf786a6c8ea7a40a39a1f81cae5b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.0 MB (13982942 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ff679aa72810ed878b17ca206945a534df3677245dd1e5c1c69f923c124a923b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Mon, 23 Mar 2020 21:39:52 GMT
ADD file:746a5c3838a898d6acf7877552ff13d1ab40d0036ace7a662e7c747018315ddb in / 
# Mon, 23 Mar 2020 21:39:53 GMT
CMD ["/bin/sh"]
# Mon, 23 Mar 2020 23:26:16 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Mon, 23 Mar 2020 23:26:17 GMT
ENV LANG=en_US.utf8
# Mon, 23 Mar 2020 23:26:20 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Mon, 23 Mar 2020 23:37:37 GMT
ENV PG_MAJOR=9.6
# Mon, 23 Mar 2020 23:37:37 GMT
ENV PG_VERSION=9.6.17
# Mon, 23 Mar 2020 23:37:37 GMT
ENV PG_SHA256=f6e1e32d32545f97c066f3c19f4d58dfab1205c01252cf85c5c92294ace1a0c2
# Mon, 23 Mar 2020 23:39:56 GMT
RUN set -ex 		&& apk add --no-cache --virtual .fetch-deps 		ca-certificates 		openssl 		tar 		&& wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2" 	&& echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c - 	&& mkdir -p /usr/src/postgresql 	&& tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	&& rm postgresql.tar.bz2 		&& apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		&& cd /usr/src/postgresql 	&& awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new 	&& grep '/var/run/postgresql' src/include/pg_config_manual.h.new 	&& mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& ./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 	&& make -j "$(nproc)" world 	&& make install-world 	&& make -C contrib install 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	&& apk del .fetch-deps .build-deps 	&& cd / 	&& rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	&& find /usr/local -name '*.a' -delete
# Mon, 23 Mar 2020 23:40:01 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Mon, 23 Mar 2020 23:40:04 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Mon, 23 Mar 2020 23:40:04 GMT
ENV PGDATA=/var/lib/postgresql/data
# Mon, 23 Mar 2020 23:40:07 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Mon, 23 Mar 2020 23:40:08 GMT
VOLUME [/var/lib/postgresql/data]
# Mon, 23 Mar 2020 23:40:09 GMT
COPY file:8241ba12b253167d267d2d8aba237bf478f6de0a6f29aa61515376f105626d03 in /usr/local/bin/ 
# Mon, 23 Mar 2020 23:40:18 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Mon, 23 Mar 2020 23:40:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 23 Mar 2020 23:40:22 GMT
EXPOSE 5432
# Mon, 23 Mar 2020 23:40:24 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:8a0637ca1ac98db4cf29f7632449c92801adc80cf0da2cd9c9e39882ce466561`  
		Last Modified: Mon, 23 Mar 2020 21:40:19 GMT  
		Size: 2.7 MB (2723139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bf70ccdbfa7098e9140b79b24406b2b9d982a82a0a28d57d23a96773cb603b5`  
		Last Modified: Mon, 23 Mar 2020 23:44:02 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ae682c8811415ca60e2e25e0806be8a3ce9ca960ca7a0d4d0b0c86a0a274956`  
		Last Modified: Mon, 23 Mar 2020 23:44:01 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9adfa96fba6df66ee4ab0bfa7595f6f82860d6a8d00cf147e83e8bae7949881e`  
		Last Modified: Mon, 23 Mar 2020 23:45:05 GMT  
		Size: 11.2 MB (11246470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d570b549ca162a597a7e6c15c9b40fe6f27f9d0b9d5f8ec0f13b5b1186671680`  
		Last Modified: Mon, 23 Mar 2020 23:44:59 GMT  
		Size: 7.2 KB (7161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99bcbf3d317c9656a5d857fb1eb7d77b294a6d86089c416bb9fa4016448d0704`  
		Last Modified: Mon, 23 Mar 2020 23:45:00 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:651bb0012510f2f993b23123c66f2d559d0c8f9de6feb5362021c35cbd9f8a96`  
		Last Modified: Mon, 23 Mar 2020 23:44:59 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:440ed7011c25fc1630965e5017ced2e0a7b09b1a7b353a3ee376c0f402fef29e`  
		Last Modified: Mon, 23 Mar 2020 23:44:59 GMT  
		Size: 4.3 KB (4263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aca6b3eee4c91e066403cba3ca8b8d86962bceec9c21ec7a07cde2ed94458a0`  
		Last Modified: Mon, 23 Mar 2020 23:44:59 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:9-alpine` - linux; 386

```console
$ docker pull postgres@sha256:c4113aa31160bad1febf867170f6a814394e124c32ea04a585da3616c467d8f3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.3 MB (15277848 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f40813f294b4832de3244841e20edd9f4b6cf0cb752acc228fcadc5e2cccd9a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Sat, 18 Jan 2020 01:38:44 GMT
ADD file:381b617b92fe699ad4ef4f30e0d9599f89e43e252883348c420ebe2a0cccbd63 in / 
# Sat, 18 Jan 2020 01:38:45 GMT
CMD ["/bin/sh"]
# Fri, 21 Feb 2020 03:30:16 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Fri, 21 Feb 2020 03:30:16 GMT
ENV LANG=en_US.utf8
# Fri, 21 Feb 2020 03:30:18 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 21 Feb 2020 03:58:59 GMT
ENV PG_MAJOR=9.6
# Fri, 21 Feb 2020 03:59:00 GMT
ENV PG_VERSION=9.6.17
# Fri, 21 Feb 2020 03:59:00 GMT
ENV PG_SHA256=f6e1e32d32545f97c066f3c19f4d58dfab1205c01252cf85c5c92294ace1a0c2
# Fri, 21 Feb 2020 04:05:14 GMT
RUN set -ex 		&& apk add --no-cache --virtual .fetch-deps 		ca-certificates 		openssl 		tar 		&& wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2" 	&& echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c - 	&& mkdir -p /usr/src/postgresql 	&& tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	&& rm postgresql.tar.bz2 		&& apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		&& cd /usr/src/postgresql 	&& awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new 	&& grep '/var/run/postgresql' src/include/pg_config_manual.h.new 	&& mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& ./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 	&& make -j "$(nproc)" world 	&& make install-world 	&& make -C contrib install 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	&& apk del .fetch-deps .build-deps 	&& cd / 	&& rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	&& find /usr/local -name '*.a' -delete
# Fri, 21 Feb 2020 04:05:15 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Fri, 21 Feb 2020 04:05:17 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 21 Feb 2020 04:05:17 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 21 Feb 2020 04:05:18 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 21 Feb 2020 04:05:18 GMT
VOLUME [/var/lib/postgresql/data]
# Wed, 04 Mar 2020 17:53:57 GMT
COPY file:8241ba12b253167d267d2d8aba237bf478f6de0a6f29aa61515376f105626d03 in /usr/local/bin/ 
# Wed, 04 Mar 2020 17:53:57 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 04 Mar 2020 17:53:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 04 Mar 2020 17:53:58 GMT
EXPOSE 5432
# Wed, 04 Mar 2020 17:53:58 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:f024b1263dc58db07a458b73ae1a2dca02ca55bef1ccd1fa3fd50656551fadf2`  
		Last Modified: Sat, 18 Jan 2020 01:39:18 GMT  
		Size: 2.8 MB (2806560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:959a23ad99210023932b0a65eae572206908695baed873ef3d83466df1b9ef9f`  
		Last Modified: Fri, 21 Feb 2020 04:13:10 GMT  
		Size: 1.2 KB (1249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f7b6dcfa29bbafa44252daa9ebfba486bf13fd4e291a15a1212477d86c8e69d`  
		Last Modified: Fri, 21 Feb 2020 04:13:10 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06bad073153323bc0de6a4081f0e97d5b73047714053bca03849f4f831810083`  
		Last Modified: Fri, 21 Feb 2020 04:16:22 GMT  
		Size: 12.5 MB (12458084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84007019d34f860d6b5858edb4c34f50477c1535da2bde66bf8d2f2df6466123`  
		Last Modified: Fri, 21 Feb 2020 04:16:16 GMT  
		Size: 7.2 KB (7160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ad72a544e5d9512a293b99da6a601efaf4674d65997dafdd5b877fc7a9fe458`  
		Last Modified: Fri, 21 Feb 2020 04:16:16 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df440bbee638b0fad5f969dd4a9a333028bbd9c08022e7c090cdcc24dc593eaf`  
		Last Modified: Fri, 21 Feb 2020 04:16:16 GMT  
		Size: 164.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9f6f50fc1cfb066a821fbd2334e6c64b0cbcf18576975fc5e988beb0e02b4ed`  
		Last Modified: Wed, 04 Mar 2020 17:54:49 GMT  
		Size: 4.3 KB (4267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f709205b485093222183199e85afdbc57d8e7f5f8de86e414e14170aebe0da0`  
		Last Modified: Wed, 04 Mar 2020 17:54:49 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:9-alpine` - linux; ppc64le

```console
$ docker pull postgres@sha256:7ca0b7aa71398154f362bf27abfe721467dfc9354554606e5d2478340f61c98c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.1 MB (15133174 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2577ba89c098a0b505a84ca24ea54a4113271463bd531c2c10d8b3f085419700`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Mon, 23 Mar 2020 21:21:29 GMT
ADD file:4b35131542b9682214e1c2c72fe3cea215a10e2f775e87befecd80fe2228d5a0 in / 
# Mon, 23 Mar 2020 21:21:32 GMT
CMD ["/bin/sh"]
# Mon, 23 Mar 2020 23:32:56 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Mon, 23 Mar 2020 23:32:58 GMT
ENV LANG=en_US.utf8
# Mon, 23 Mar 2020 23:33:07 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Mon, 23 Mar 2020 23:51:32 GMT
ENV PG_MAJOR=9.6
# Mon, 23 Mar 2020 23:51:37 GMT
ENV PG_VERSION=9.6.17
# Mon, 23 Mar 2020 23:51:40 GMT
ENV PG_SHA256=f6e1e32d32545f97c066f3c19f4d58dfab1205c01252cf85c5c92294ace1a0c2
# Mon, 23 Mar 2020 23:54:25 GMT
RUN set -ex 		&& apk add --no-cache --virtual .fetch-deps 		ca-certificates 		openssl 		tar 		&& wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2" 	&& echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c - 	&& mkdir -p /usr/src/postgresql 	&& tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	&& rm postgresql.tar.bz2 		&& apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		&& cd /usr/src/postgresql 	&& awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new 	&& grep '/var/run/postgresql' src/include/pg_config_manual.h.new 	&& mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& ./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 	&& make -j "$(nproc)" world 	&& make install-world 	&& make -C contrib install 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	&& apk del .fetch-deps .build-deps 	&& cd / 	&& rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	&& find /usr/local -name '*.a' -delete
# Mon, 23 Mar 2020 23:54:33 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Mon, 23 Mar 2020 23:54:41 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Mon, 23 Mar 2020 23:54:44 GMT
ENV PGDATA=/var/lib/postgresql/data
# Mon, 23 Mar 2020 23:54:49 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Mon, 23 Mar 2020 23:54:52 GMT
VOLUME [/var/lib/postgresql/data]
# Mon, 23 Mar 2020 23:54:53 GMT
COPY file:8241ba12b253167d267d2d8aba237bf478f6de0a6f29aa61515376f105626d03 in /usr/local/bin/ 
# Mon, 23 Mar 2020 23:55:00 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Mon, 23 Mar 2020 23:55:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 23 Mar 2020 23:55:08 GMT
EXPOSE 5432
# Mon, 23 Mar 2020 23:55:11 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:bc1c99f4ba60de0d3ca52dc6855483e24c91884e33df71f502bbff6eb909d9b9`  
		Last Modified: Mon, 23 Mar 2020 21:22:12 GMT  
		Size: 2.8 MB (2820052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18e24e77bb4bdf10a12615b518d92fce4871d89df08c615afd1a51053ecd5c06`  
		Last Modified: Mon, 23 Mar 2020 23:59:59 GMT  
		Size: 1.3 KB (1277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b08df00f3eac9768a1a5e068c9cb9a8c20ffd792fb8c287b085bf72dd4cf362`  
		Last Modified: Mon, 23 Mar 2020 23:59:59 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3ded904133877c0e07dea8bf66b515c5fe67088ee7b7b5069f35ca5c207259f`  
		Last Modified: Tue, 24 Mar 2020 00:01:18 GMT  
		Size: 12.3 MB (12299804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d7831c929e34e9f254e9e7659ba0afe94a344674177e6418db563d73aab68e4`  
		Last Modified: Tue, 24 Mar 2020 00:01:12 GMT  
		Size: 7.2 KB (7156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88f4c2272b21224a870151caebe6dfa6a24560588b89927bae616bed842b9bde`  
		Last Modified: Tue, 24 Mar 2020 00:01:12 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c5bb5683271f187d4b5749184d899cb4c648246ef6fa050f9ef69179b84bb05`  
		Last Modified: Tue, 24 Mar 2020 00:01:12 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0c73d91e2e72a7e9c353f6a1b78d2916a624f50862da607524c1feb5fa7821c`  
		Last Modified: Tue, 24 Mar 2020 00:01:12 GMT  
		Size: 4.3 KB (4260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e70c28af94262d6c3b750ce0d62240de20cecf9ad0b830653f03fd41c05df05`  
		Last Modified: Tue, 24 Mar 2020 00:01:11 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:9-alpine` - linux; s390x

```console
$ docker pull postgres@sha256:0e97685f36882e0060ba2b7d50fe28056fbb34acb5a98e9d12fc184981195f07
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.8 MB (13822965 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:44e3d974d14cc7cc5f164dd83dfe7206668d983ecad6a258d097deaa3d54a90b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Mon, 23 Mar 2020 21:41:34 GMT
ADD file:b6d4ad8fd0ec7f66e6d54b8cd8937ba7821b44096806af78692b4cab6d087a9c in / 
# Mon, 23 Mar 2020 21:41:34 GMT
CMD ["/bin/sh"]
# Mon, 23 Mar 2020 22:34:53 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Mon, 23 Mar 2020 22:34:54 GMT
ENV LANG=en_US.utf8
# Mon, 23 Mar 2020 22:34:56 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Mon, 23 Mar 2020 22:50:20 GMT
ENV PG_MAJOR=9.6
# Mon, 23 Mar 2020 22:50:20 GMT
ENV PG_VERSION=9.6.17
# Mon, 23 Mar 2020 22:50:21 GMT
ENV PG_SHA256=f6e1e32d32545f97c066f3c19f4d58dfab1205c01252cf85c5c92294ace1a0c2
# Mon, 23 Mar 2020 22:53:07 GMT
RUN set -ex 		&& apk add --no-cache --virtual .fetch-deps 		ca-certificates 		openssl 		tar 		&& wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2" 	&& echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c - 	&& mkdir -p /usr/src/postgresql 	&& tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	&& rm postgresql.tar.bz2 		&& apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		&& cd /usr/src/postgresql 	&& awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new 	&& grep '/var/run/postgresql' src/include/pg_config_manual.h.new 	&& mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& ./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 	&& make -j "$(nproc)" world 	&& make install-world 	&& make -C contrib install 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	&& apk del .fetch-deps .build-deps 	&& cd / 	&& rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	&& find /usr/local -name '*.a' -delete
# Mon, 23 Mar 2020 22:53:10 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Mon, 23 Mar 2020 22:53:12 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Mon, 23 Mar 2020 22:53:13 GMT
ENV PGDATA=/var/lib/postgresql/data
# Mon, 23 Mar 2020 22:53:14 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Mon, 23 Mar 2020 22:53:14 GMT
VOLUME [/var/lib/postgresql/data]
# Mon, 23 Mar 2020 22:53:15 GMT
COPY file:8241ba12b253167d267d2d8aba237bf478f6de0a6f29aa61515376f105626d03 in /usr/local/bin/ 
# Mon, 23 Mar 2020 22:53:17 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Mon, 23 Mar 2020 22:53:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 23 Mar 2020 22:53:18 GMT
EXPOSE 5432
# Mon, 23 Mar 2020 22:53:19 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:ca1c6795bfb97df28a926fd646127ba4944b69beb1cea7b00d62787b8b3c0108`  
		Last Modified: Mon, 23 Mar 2020 21:41:56 GMT  
		Size: 2.6 MB (2582073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:096988d6f0d7fbd4d835bbdd287617d11694ddc413c08e121fb9e04ac568179e`  
		Last Modified: Mon, 23 Mar 2020 22:56:13 GMT  
		Size: 1.3 KB (1275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ac69069693ec79fe32bc3463632dd40d67b35b256844d6a7bd05a596226684d`  
		Last Modified: Mon, 23 Mar 2020 22:56:11 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cd86d3c5aa3197b9b44b9a772389aab729614f2b05f0f983ff7aabd102ef504`  
		Last Modified: Mon, 23 Mar 2020 22:57:04 GMT  
		Size: 11.2 MB (11227572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e279cd42df2ed5e85125bf2929fa38232bcd76432f968c17da989f43d21bf12d`  
		Last Modified: Mon, 23 Mar 2020 22:57:00 GMT  
		Size: 7.2 KB (7159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1556100f02d5b69e94e644a4099faef27ab6dded4a713c3bbde3974279464cb3`  
		Last Modified: Mon, 23 Mar 2020 22:57:06 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d4249181f48839d3e53f001847c2c855e80ac02146b39768fcb3961b1a5f16b`  
		Last Modified: Mon, 23 Mar 2020 22:57:00 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40d9e4c92a7a8704074c734887a67c419a6acfa8442961aef9428cf51e5b1b30`  
		Last Modified: Mon, 23 Mar 2020 22:57:00 GMT  
		Size: 4.3 KB (4258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97890ee1f1e386dd0a1584fa2df7c727faf7aa299ca2a1a3d86f6b8680403311`  
		Last Modified: Mon, 23 Mar 2020 22:57:06 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
