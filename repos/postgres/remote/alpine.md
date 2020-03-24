## `postgres:alpine`

```console
$ docker pull postgres@sha256:d9b999bd62f3bab382983a659813918625e30b9e5f762ecdd14ae13efa21a7e3
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
$ docker pull postgres@sha256:0126e9cc00a7a25b238c0aa34a4600158fcf631fd43f7d248a063c943e3e57a3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.8 MB (59784986 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ecb176ff304a4db995d98f4704711b1a966a12f93df026d233affd1644e8a37d`
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
# Mon, 23 Mar 2020 23:47:59 GMT
ENV PG_MAJOR=12
# Mon, 23 Mar 2020 23:47:59 GMT
ENV PG_VERSION=12.2
# Mon, 23 Mar 2020 23:47:59 GMT
ENV PG_SHA256=ad1dcc4c4fc500786b745635a9e1eba950195ce20b8913f50345bb7d5369b5de
# Mon, 23 Mar 2020 23:58:03 GMT
RUN set -ex 		&& apk add --no-cache --virtual .fetch-deps 		ca-certificates 		openssl 		tar 		&& wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2" 	&& echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c - 	&& mkdir -p /usr/src/postgresql 	&& tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	&& rm postgresql.tar.bz2 		&& apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm9-dev clang g++ 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 		&& cd /usr/src/postgresql 	&& awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new 	&& grep '/var/run/postgresql' src/include/pg_config_manual.h.new 	&& mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& ./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	&& make -j "$(nproc)" world 	&& make install-world 	&& make -C contrib install 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	&& apk del .fetch-deps .build-deps 	&& cd / 	&& rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	&& find /usr/local -name '*.a' -delete
# Mon, 23 Mar 2020 23:58:05 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Mon, 23 Mar 2020 23:58:06 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Mon, 23 Mar 2020 23:58:07 GMT
ENV PGDATA=/var/lib/postgresql/data
# Mon, 23 Mar 2020 23:58:08 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Mon, 23 Mar 2020 23:58:09 GMT
VOLUME [/var/lib/postgresql/data]
# Mon, 23 Mar 2020 23:58:09 GMT
COPY file:33e6fc6ab9ea2b87183e496ad72f1df7f682913ffd781b1451fd178b0c7d745a in /usr/local/bin/ 
# Mon, 23 Mar 2020 23:58:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 23 Mar 2020 23:58:10 GMT
EXPOSE 5432
# Mon, 23 Mar 2020 23:58:10 GMT
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
	-	`sha256:48e4532f784aae9d0d7813d3cf1ba9af1bcf04ec6f5793370b953878cbc6af9a`  
		Last Modified: Tue, 24 Mar 2020 00:28:31 GMT  
		Size: 57.0 MB (56967604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e7e92e65f6ae62cb18ad81041c742908e661506ba95950a8137e488f89a89ba`  
		Last Modified: Tue, 24 Mar 2020 00:28:14 GMT  
		Size: 8.2 KB (8210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5f366a1c147f00abb6544fd808804892f8dcb63180db9d55da6e9bd0c9abe4f`  
		Last Modified: Tue, 24 Mar 2020 00:28:15 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b33682350b13528d392d008134376276b8a229c2fe54ccf82fdb9a89acc34aa9`  
		Last Modified: Tue, 24 Mar 2020 00:28:14 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0204b658ab83d9167b3562983f05f73f3ed3f075cbcfa0a07db1929c12f15c2f`  
		Last Modified: Tue, 24 Mar 2020 00:28:15 GMT  
		Size: 4.3 KB (4265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:alpine` - linux; arm variant v6

```console
$ docker pull postgres@sha256:17fe1b56120e70f8a9cc5b12e72276e71430cef4848c9a971dd2e90363e3dadd
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.2 MB (58196472 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4bd338a2bcca8e1d998c8e5c6122e3f528b72e6d219d93913aa4fede256b865f`
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
# Mon, 23 Mar 2020 23:26:20 GMT
ENV PG_MAJOR=12
# Mon, 23 Mar 2020 23:26:21 GMT
ENV PG_VERSION=12.2
# Mon, 23 Mar 2020 23:26:22 GMT
ENV PG_SHA256=ad1dcc4c4fc500786b745635a9e1eba950195ce20b8913f50345bb7d5369b5de
# Mon, 23 Mar 2020 23:30:54 GMT
RUN set -ex 		&& apk add --no-cache --virtual .fetch-deps 		ca-certificates 		openssl 		tar 		&& wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2" 	&& echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c - 	&& mkdir -p /usr/src/postgresql 	&& tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	&& rm postgresql.tar.bz2 		&& apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm9-dev clang g++ 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 		&& cd /usr/src/postgresql 	&& awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new 	&& grep '/var/run/postgresql' src/include/pg_config_manual.h.new 	&& mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& ./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	&& make -j "$(nproc)" world 	&& make install-world 	&& make -C contrib install 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	&& apk del .fetch-deps .build-deps 	&& cd / 	&& rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	&& find /usr/local -name '*.a' -delete
# Mon, 23 Mar 2020 23:30:58 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Mon, 23 Mar 2020 23:31:00 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Mon, 23 Mar 2020 23:31:01 GMT
ENV PGDATA=/var/lib/postgresql/data
# Mon, 23 Mar 2020 23:31:03 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Mon, 23 Mar 2020 23:31:03 GMT
VOLUME [/var/lib/postgresql/data]
# Mon, 23 Mar 2020 23:31:04 GMT
COPY file:33e6fc6ab9ea2b87183e496ad72f1df7f682913ffd781b1451fd178b0c7d745a in /usr/local/bin/ 
# Mon, 23 Mar 2020 23:31:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 23 Mar 2020 23:31:06 GMT
EXPOSE 5432
# Mon, 23 Mar 2020 23:31:06 GMT
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
	-	`sha256:f20646682be91d55a247022c1609697ae2fb8ea08cb9a4eb8e18131edddc5649`  
		Last Modified: Mon, 23 Mar 2020 23:45:38 GMT  
		Size: 55.6 MB (55563635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:124c1411a70b1ad450844599fa0c8870576ba3619ebdbc1992d6d458fa8602cb`  
		Last Modified: Mon, 23 Mar 2020 23:45:20 GMT  
		Size: 8.2 KB (8211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b923df2a8698a6f4dbce199cb4c6c5ae9476c9bff7a7bd83446aa4c41eac9e69`  
		Last Modified: Mon, 23 Mar 2020 23:45:20 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96cbc8773213e9e21dfaa1cff469d57f698e1aca920d2eb11531b43acaa62683`  
		Last Modified: Mon, 23 Mar 2020 23:45:20 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25f6d762bfa3a5832e284a85a3d6322ca1455b809c1149817e5ab86d6388a7a6`  
		Last Modified: Mon, 23 Mar 2020 23:45:20 GMT  
		Size: 4.3 KB (4265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:alpine` - linux; arm variant v7

```console
$ docker pull postgres@sha256:ed9d39c1b2aa675299f26427702ac30b2595270f08773dfba5d038224057c91e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.5 MB (55464900 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4385641ad9ce738e86ebc036fd738531fed71b2a9e3c3cd3fbaf99b0be010369`
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
# Mon, 23 Mar 2020 22:43:24 GMT
ENV PG_MAJOR=12
# Mon, 23 Mar 2020 22:43:24 GMT
ENV PG_VERSION=12.2
# Mon, 23 Mar 2020 22:43:25 GMT
ENV PG_SHA256=ad1dcc4c4fc500786b745635a9e1eba950195ce20b8913f50345bb7d5369b5de
# Mon, 23 Mar 2020 22:46:41 GMT
RUN set -ex 		&& apk add --no-cache --virtual .fetch-deps 		ca-certificates 		openssl 		tar 		&& wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2" 	&& echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c - 	&& mkdir -p /usr/src/postgresql 	&& tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	&& rm postgresql.tar.bz2 		&& apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm9-dev clang g++ 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 		&& cd /usr/src/postgresql 	&& awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new 	&& grep '/var/run/postgresql' src/include/pg_config_manual.h.new 	&& mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& ./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	&& make -j "$(nproc)" world 	&& make install-world 	&& make -C contrib install 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	&& apk del .fetch-deps .build-deps 	&& cd / 	&& rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	&& find /usr/local -name '*.a' -delete
# Mon, 23 Mar 2020 22:47:28 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Mon, 23 Mar 2020 22:48:05 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Mon, 23 Mar 2020 22:48:10 GMT
ENV PGDATA=/var/lib/postgresql/data
# Mon, 23 Mar 2020 22:48:25 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Mon, 23 Mar 2020 22:48:30 GMT
VOLUME [/var/lib/postgresql/data]
# Mon, 23 Mar 2020 22:48:33 GMT
COPY file:33e6fc6ab9ea2b87183e496ad72f1df7f682913ffd781b1451fd178b0c7d745a in /usr/local/bin/ 
# Mon, 23 Mar 2020 22:48:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 23 Mar 2020 22:48:41 GMT
EXPOSE 5432
# Mon, 23 Mar 2020 22:48:42 GMT
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
	-	`sha256:76a49a1deba11c5c2c753c925fb43a397a77dfc6a74ceb8d3259230d379a416f`  
		Last Modified: Mon, 23 Mar 2020 23:02:23 GMT  
		Size: 53.0 MB (53030159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10663994ec5825307dbee4329681ac782002291406f7eb4201c01c7cdf324d41`  
		Last Modified: Mon, 23 Mar 2020 23:02:09 GMT  
		Size: 8.2 KB (8206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a333a362a916930fc5cda97a84c7f058f84bafce52144b53c6fe7976e91682c1`  
		Last Modified: Mon, 23 Mar 2020 23:02:09 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da1275c985f6cccb539f5434b8544ed744eb38f16e794a2d2ee696a231c926b3`  
		Last Modified: Mon, 23 Mar 2020 23:02:09 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7510c6c2454284448399d386b03cc7086678490161b31c85a8d79df9bcc0fb81`  
		Last Modified: Mon, 23 Mar 2020 23:02:09 GMT  
		Size: 4.3 KB (4260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:alpine` - linux; arm64 variant v8

```console
$ docker pull postgres@sha256:c3119edf27c366039db1a675b13005636b3637ca8935de7dbbc98f33fd460020
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.4 MB (59391824 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c17c57631758e0ff63c26ddfeddeeb9e9b5127f11f1622ddd911b4ae8da827b8`
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
# Mon, 23 Mar 2020 23:26:21 GMT
ENV PG_MAJOR=12
# Mon, 23 Mar 2020 23:26:22 GMT
ENV PG_VERSION=12.2
# Mon, 23 Mar 2020 23:26:24 GMT
ENV PG_SHA256=ad1dcc4c4fc500786b745635a9e1eba950195ce20b8913f50345bb7d5369b5de
# Mon, 23 Mar 2020 23:29:45 GMT
RUN set -ex 		&& apk add --no-cache --virtual .fetch-deps 		ca-certificates 		openssl 		tar 		&& wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2" 	&& echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c - 	&& mkdir -p /usr/src/postgresql 	&& tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	&& rm postgresql.tar.bz2 		&& apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm9-dev clang g++ 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 		&& cd /usr/src/postgresql 	&& awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new 	&& grep '/var/run/postgresql' src/include/pg_config_manual.h.new 	&& mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& ./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	&& make -j "$(nproc)" world 	&& make install-world 	&& make -C contrib install 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	&& apk del .fetch-deps .build-deps 	&& cd / 	&& rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	&& find /usr/local -name '*.a' -delete
# Mon, 23 Mar 2020 23:29:48 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Mon, 23 Mar 2020 23:29:50 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Mon, 23 Mar 2020 23:29:51 GMT
ENV PGDATA=/var/lib/postgresql/data
# Mon, 23 Mar 2020 23:29:53 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Mon, 23 Mar 2020 23:29:53 GMT
VOLUME [/var/lib/postgresql/data]
# Mon, 23 Mar 2020 23:29:54 GMT
COPY file:33e6fc6ab9ea2b87183e496ad72f1df7f682913ffd781b1451fd178b0c7d745a in /usr/local/bin/ 
# Mon, 23 Mar 2020 23:29:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 23 Mar 2020 23:29:55 GMT
EXPOSE 5432
# Mon, 23 Mar 2020 23:29:56 GMT
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
	-	`sha256:ce79e3a441dffccea4413886d4be4df402da0ae5e6561dbd705b5d1d81b84d80`  
		Last Modified: Mon, 23 Mar 2020 23:44:12 GMT  
		Size: 56.7 MB (56654424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:507cb5a68cbd3d1b16fa6f1afb70e51af2db0db227680f5e0c646f1231149406`  
		Last Modified: Mon, 23 Mar 2020 23:44:00 GMT  
		Size: 8.2 KB (8214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:908ab8174e12bd74032ee41e537b750aacfa46b5f65bd3873c900acf2ce3d6f9`  
		Last Modified: Mon, 23 Mar 2020 23:44:00 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cc9561591bdeac28857993f6e75cbce391e9cd1073f2b5ad94c8a79f4929f94`  
		Last Modified: Mon, 23 Mar 2020 23:44:00 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3c7a46ba014b2d5e2eb9595bdf99cdd4b51e40d257b49c32afb60c614ce3c00`  
		Last Modified: Mon, 23 Mar 2020 23:44:00 GMT  
		Size: 4.3 KB (4262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:alpine` - linux; 386

```console
$ docker pull postgres@sha256:e0fe21641a9d4308455c8f640f7ab250f15fcab6022590c3ade43770a5e965c4
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.5 MB (63508441 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:415afb796093bc75f57a305af354012e45f01f31f60b31c774456e5bc4e44d0d`
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
# Fri, 21 Feb 2020 03:30:18 GMT
ENV PG_MAJOR=12
# Fri, 21 Feb 2020 03:30:18 GMT
ENV PG_VERSION=12.2
# Fri, 21 Feb 2020 03:30:19 GMT
ENV PG_SHA256=ad1dcc4c4fc500786b745635a9e1eba950195ce20b8913f50345bb7d5369b5de
# Fri, 21 Feb 2020 03:40:16 GMT
RUN set -ex 		&& apk add --no-cache --virtual .fetch-deps 		ca-certificates 		openssl 		tar 		&& wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2" 	&& echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c - 	&& mkdir -p /usr/src/postgresql 	&& tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	&& rm postgresql.tar.bz2 		&& apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm9-dev clang g++ 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 		&& cd /usr/src/postgresql 	&& awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new 	&& grep '/var/run/postgresql' src/include/pg_config_manual.h.new 	&& mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& ./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	&& make -j "$(nproc)" world 	&& make install-world 	&& make -C contrib install 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	&& apk del .fetch-deps .build-deps 	&& cd / 	&& rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	&& find /usr/local -name '*.a' -delete
# Fri, 21 Feb 2020 03:40:17 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Fri, 21 Feb 2020 03:40:18 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 21 Feb 2020 03:40:18 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 21 Feb 2020 03:40:19 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 21 Feb 2020 03:40:19 GMT
VOLUME [/var/lib/postgresql/data]
# Wed, 04 Mar 2020 17:53:26 GMT
COPY file:33e6fc6ab9ea2b87183e496ad72f1df7f682913ffd781b1451fd178b0c7d745a in /usr/local/bin/ 
# Wed, 04 Mar 2020 17:53:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 04 Mar 2020 17:53:27 GMT
EXPOSE 5432
# Wed, 04 Mar 2020 17:53:27 GMT
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
	-	`sha256:8138de729ca4b07667790038724cb11d8c1a981e6174bdf092d3cf616814f986`  
		Last Modified: Fri, 21 Feb 2020 04:13:37 GMT  
		Size: 60.7 MB (60687756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9602bea59c307478ca001ea71d8be957a2bfb086bec914a67f6b305b733df663`  
		Last Modified: Fri, 21 Feb 2020 04:13:09 GMT  
		Size: 8.2 KB (8206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26b7a57f34297110077dea3dfd7045a01fc278630b9690f2337957bcb205e8a8`  
		Last Modified: Fri, 21 Feb 2020 04:13:09 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46799e46dcd512bc57a8e566a3dea73ae3ac1db4d39e599c92fae6b5ed6f0c2f`  
		Last Modified: Fri, 21 Feb 2020 04:13:08 GMT  
		Size: 165.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35c9c1ec41ce7bd485e47e2e2489f868a640b019afd0824120f013440bcad6df`  
		Last Modified: Wed, 04 Mar 2020 17:54:25 GMT  
		Size: 4.3 KB (4261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:alpine` - linux; ppc64le

```console
$ docker pull postgres@sha256:4ba5f0a07f2ee051fcf9c79547f505936e408b53d019ca1bb5ed1862a753dcc0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.1 MB (62059215 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f78e642fe7083cd8bd681d5f18393bff732ea49cb35effa0f4d9adf01ee29a12`
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
# Mon, 23 Mar 2020 23:33:10 GMT
ENV PG_MAJOR=12
# Mon, 23 Mar 2020 23:33:13 GMT
ENV PG_VERSION=12.2
# Mon, 23 Mar 2020 23:33:16 GMT
ENV PG_SHA256=ad1dcc4c4fc500786b745635a9e1eba950195ce20b8913f50345bb7d5369b5de
# Mon, 23 Mar 2020 23:38:41 GMT
RUN set -ex 		&& apk add --no-cache --virtual .fetch-deps 		ca-certificates 		openssl 		tar 		&& wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2" 	&& echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c - 	&& mkdir -p /usr/src/postgresql 	&& tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	&& rm postgresql.tar.bz2 		&& apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm9-dev clang g++ 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 		&& cd /usr/src/postgresql 	&& awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new 	&& grep '/var/run/postgresql' src/include/pg_config_manual.h.new 	&& mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& ./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	&& make -j "$(nproc)" world 	&& make install-world 	&& make -C contrib install 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	&& apk del .fetch-deps .build-deps 	&& cd / 	&& rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	&& find /usr/local -name '*.a' -delete
# Mon, 23 Mar 2020 23:38:56 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Mon, 23 Mar 2020 23:39:07 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Mon, 23 Mar 2020 23:39:11 GMT
ENV PGDATA=/var/lib/postgresql/data
# Mon, 23 Mar 2020 23:39:17 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Mon, 23 Mar 2020 23:39:21 GMT
VOLUME [/var/lib/postgresql/data]
# Mon, 23 Mar 2020 23:39:23 GMT
COPY file:33e6fc6ab9ea2b87183e496ad72f1df7f682913ffd781b1451fd178b0c7d745a in /usr/local/bin/ 
# Mon, 23 Mar 2020 23:39:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 23 Mar 2020 23:39:32 GMT
EXPOSE 5432
# Mon, 23 Mar 2020 23:39:37 GMT
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
	-	`sha256:1ef3c9876a75e74590634e7d346c50dbdb951d970ac625f0014b470e6e396d65`  
		Last Modified: Tue, 24 Mar 2020 00:00:08 GMT  
		Size: 59.2 MB (59224910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ecbccc30158a14aedd240825b2987144e6ec51096e77039d5d304687e78639c`  
		Last Modified: Mon, 23 Mar 2020 23:59:55 GMT  
		Size: 8.2 KB (8211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:927e4ea8bb15c74eb340a7a055bbfe379bf45bf3fef1bb50dee27be1283de461`  
		Last Modified: Mon, 23 Mar 2020 23:59:55 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:671c69f9b0ec4c72d4273cba928db795ec57ef0c3b89ec54f23eba3ee7798d4a`  
		Last Modified: Mon, 23 Mar 2020 23:59:55 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddfcfff72fddcefc8231a52fe3a398ca2eca345d9352272e57639c011fa9e98e`  
		Last Modified: Mon, 23 Mar 2020 23:59:55 GMT  
		Size: 4.3 KB (4260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:alpine` - linux; s390x

```console
$ docker pull postgres@sha256:9e7d8bbef9e01ffa81fe41bc70349797eef4a59a1da2da50be983397443b52e1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.0 MB (61975890 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c7d0119f5a02f35b2bc769134a448cfe289be5aa7b7b86bcb2ce2c1b9bc92e8b`
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
# Mon, 23 Mar 2020 22:34:56 GMT
ENV PG_MAJOR=12
# Mon, 23 Mar 2020 22:34:57 GMT
ENV PG_VERSION=12.2
# Mon, 23 Mar 2020 22:34:57 GMT
ENV PG_SHA256=ad1dcc4c4fc500786b745635a9e1eba950195ce20b8913f50345bb7d5369b5de
# Mon, 23 Mar 2020 22:39:55 GMT
RUN set -ex 		&& apk add --no-cache --virtual .fetch-deps 		ca-certificates 		openssl 		tar 		&& wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2" 	&& echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c - 	&& mkdir -p /usr/src/postgresql 	&& tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	&& rm postgresql.tar.bz2 		&& apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm9-dev clang g++ 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 		&& cd /usr/src/postgresql 	&& awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new 	&& grep '/var/run/postgresql' src/include/pg_config_manual.h.new 	&& mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& ./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	&& make -j "$(nproc)" world 	&& make install-world 	&& make -C contrib install 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	&& apk del .fetch-deps .build-deps 	&& cd / 	&& rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	&& find /usr/local -name '*.a' -delete
# Mon, 23 Mar 2020 22:40:05 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Mon, 23 Mar 2020 22:40:07 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Mon, 23 Mar 2020 22:40:08 GMT
ENV PGDATA=/var/lib/postgresql/data
# Mon, 23 Mar 2020 22:40:10 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Mon, 23 Mar 2020 22:40:11 GMT
VOLUME [/var/lib/postgresql/data]
# Mon, 23 Mar 2020 22:40:11 GMT
COPY file:33e6fc6ab9ea2b87183e496ad72f1df7f682913ffd781b1451fd178b0c7d745a in /usr/local/bin/ 
# Mon, 23 Mar 2020 22:40:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 23 Mar 2020 22:40:13 GMT
EXPOSE 5432
# Mon, 23 Mar 2020 22:40:13 GMT
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
	-	`sha256:b3261891971420ea3ce2e78a2449bdee386d183e7bec3d9d5690a890162916a2`  
		Last Modified: Mon, 23 Mar 2020 22:56:18 GMT  
		Size: 59.4 MB (59379568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfb607b80a17a98a5256d52b2fde3a70b8ec321e407fb1688ebc3e2270250ae3`  
		Last Modified: Mon, 23 Mar 2020 22:56:25 GMT  
		Size: 8.2 KB (8208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c1d631f632ab6c4bb38d1fcc1a0ef2fed329407bac9b0de9c33f72762e02d06`  
		Last Modified: Mon, 23 Mar 2020 22:56:26 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f079ad7e756d2ff6eca5f2b4e185751a8703bb9eb649c08858da354fd2b86ce4`  
		Last Modified: Mon, 23 Mar 2020 22:56:25 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:015878e6a4848a08c3faa949a92dd034720fa73414be3783f898c0cd870f29ce`  
		Last Modified: Mon, 23 Mar 2020 22:56:09 GMT  
		Size: 4.3 KB (4260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
