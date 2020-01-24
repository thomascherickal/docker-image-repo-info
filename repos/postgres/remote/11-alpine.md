## `postgres:11-alpine`

```console
$ docker pull postgres@sha256:4bf07d54b0eb6d6b4005197ab967c03de3f1143ef193d12d46c2c4eb4804ee91
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

### `postgres:11-alpine` - linux; amd64

```console
$ docker pull postgres@sha256:675acd96488b2d7b241108a94415e48c9ea9d8fa6c15a84829b247746792101a
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.3 MB (57289429 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3e2839111783e0a1b76aa14a2eac5a26c73ac4be05ba65d0d50246b40b21c29f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:06 GMT
ADD file:d48cac34fac385cbc1de6adfdd88300f76f9bbe346cd17e64fd834d042a98326 in / 
# Thu, 23 Jan 2020 16:53:06 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 21:29:09 GMT
RUN set -ex; 	postgresHome="$(getent passwd postgres)"; 	postgresHome="$(echo "$postgresHome" | cut -d: -f6)"; 	[ "$postgresHome" = '/var/lib/postgresql' ]; 	mkdir -p "$postgresHome"; 	chown -R postgres:postgres "$postgresHome"
# Thu, 23 Jan 2020 21:29:10 GMT
ENV LANG=en_US.utf8
# Thu, 23 Jan 2020 21:29:11 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 23 Jan 2020 21:38:48 GMT
ENV PG_MAJOR=11
# Thu, 23 Jan 2020 21:38:48 GMT
ENV PG_VERSION=11.6
# Thu, 23 Jan 2020 21:38:48 GMT
ENV PG_SHA256=49924f7ff92965fdb20c86e0696f2dc9f8553e1563124ead7beedf8910c13170
# Thu, 23 Jan 2020 21:48:26 GMT
RUN set -ex 		&& apk add --no-cache --virtual .fetch-deps 		ca-certificates 		openssl 		tar 		&& wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2" 	&& echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c - 	&& mkdir -p /usr/src/postgresql 	&& tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	&& rm postgresql.tar.bz2 		&& apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm8-dev clang g++ 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 		&& cd /usr/src/postgresql 	&& awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new 	&& grep '/var/run/postgresql' src/include/pg_config_manual.h.new 	&& mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& ./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	&& make -j "$(nproc)" world 	&& make install-world 	&& make -C contrib install 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	&& apk del .fetch-deps .build-deps 	&& cd / 	&& rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	&& find /usr/local -name '*.a' -delete
# Thu, 23 Jan 2020 21:48:28 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Thu, 23 Jan 2020 21:48:29 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 23 Jan 2020 21:48:29 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 23 Jan 2020 21:48:31 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 23 Jan 2020 21:48:31 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 23 Jan 2020 21:48:32 GMT
COPY file:74700c51dbcbbad39fbd303750c2ac04ac10f59a73a55171e1fd0dbae6c2f311 in /usr/local/bin/ 
# Thu, 23 Jan 2020 21:48:33 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 23 Jan 2020 21:48:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jan 2020 21:48:34 GMT
EXPOSE 5432
# Thu, 23 Jan 2020 21:48:34 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:4167d3e149762ea326c26fc2fd4e36fdeb7d4e639408ad30f37b8f25ac285a98`  
		Last Modified: Thu, 23 Jan 2020 16:53:38 GMT  
		Size: 2.8 MB (2786962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:153ce209e2ba06d723d54d083b4d327d810d39100855700c14a102336c77cf61`  
		Last Modified: Thu, 23 Jan 2020 22:11:36 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5e6278dc07d3b84c7765b1bdd5ab2b3031176cd6ea57357845a8c217a1979c1`  
		Last Modified: Thu, 23 Jan 2020 22:11:36 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c90a26635629277ef1f7067ae1d13f0c23e5f4b641336c359016e29c2dd0f60`  
		Last Modified: Thu, 23 Jan 2020 22:12:45 GMT  
		Size: 54.5 MB (54490386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87e204d8e0aa64abf2e19f5c6fb170243d14b27a0fcdc13c5daeb67055b1009f`  
		Last Modified: Thu, 23 Jan 2020 22:12:12 GMT  
		Size: 7.6 KB (7568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:254ebbae56903160a9eb0a4ccc329278eddeae4caa2d7d5cf909a3981477a52b`  
		Last Modified: Thu, 23 Jan 2020 22:12:12 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adb8bbd1e3db11fff161697d1c8a6ec4385a94f5caca55fa05b708cc4cd04d53`  
		Last Modified: Thu, 23 Jan 2020 22:12:11 GMT  
		Size: 164.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17bb79a0412d30036d4aec4cbbc57d3a1041587ff4ae10413f81e9e90942f551`  
		Last Modified: Thu, 23 Jan 2020 22:12:11 GMT  
		Size: 3.8 KB (3836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c1ef549e53f638570106b9a1700e45f53a5df1ed857f0e5f16c61b0d5586e00`  
		Last Modified: Thu, 23 Jan 2020 22:12:12 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:11-alpine` - linux; arm variant v6

```console
$ docker pull postgres@sha256:a9af429505cb8c80bf42b9cd4ba8e8d2b01a91760b0f5417a74a40ae3ca24444
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.3 MB (55261819 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bba0dcfd75184cad29b191b38e6ac4bcebf67892821603161c886133d10f27fa`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:27 GMT
ADD file:2aa80d52585a6b34b2cc5811d46965a084e50cfb8cd183f1a88b2b1bc6556e1f in / 
# Thu, 23 Jan 2020 16:53:28 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 19:53:02 GMT
RUN set -ex; 	postgresHome="$(getent passwd postgres)"; 	postgresHome="$(echo "$postgresHome" | cut -d: -f6)"; 	[ "$postgresHome" = '/var/lib/postgresql' ]; 	mkdir -p "$postgresHome"; 	chown -R postgres:postgres "$postgresHome"
# Thu, 23 Jan 2020 19:53:03 GMT
ENV LANG=en_US.utf8
# Thu, 23 Jan 2020 19:53:05 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 23 Jan 2020 19:56:34 GMT
ENV PG_MAJOR=11
# Thu, 23 Jan 2020 19:56:35 GMT
ENV PG_VERSION=11.6
# Thu, 23 Jan 2020 19:56:35 GMT
ENV PG_SHA256=49924f7ff92965fdb20c86e0696f2dc9f8553e1563124ead7beedf8910c13170
# Thu, 23 Jan 2020 19:59:43 GMT
RUN set -ex 		&& apk add --no-cache --virtual .fetch-deps 		ca-certificates 		openssl 		tar 		&& wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2" 	&& echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c - 	&& mkdir -p /usr/src/postgresql 	&& tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	&& rm postgresql.tar.bz2 		&& apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm8-dev clang g++ 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 		&& cd /usr/src/postgresql 	&& awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new 	&& grep '/var/run/postgresql' src/include/pg_config_manual.h.new 	&& mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& ./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	&& make -j "$(nproc)" world 	&& make install-world 	&& make -C contrib install 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	&& apk del .fetch-deps .build-deps 	&& cd / 	&& rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	&& find /usr/local -name '*.a' -delete
# Thu, 23 Jan 2020 19:59:50 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Thu, 23 Jan 2020 19:59:53 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 23 Jan 2020 19:59:54 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 23 Jan 2020 19:59:56 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 23 Jan 2020 19:59:57 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 23 Jan 2020 19:59:58 GMT
COPY file:74700c51dbcbbad39fbd303750c2ac04ac10f59a73a55171e1fd0dbae6c2f311 in /usr/local/bin/ 
# Thu, 23 Jan 2020 20:00:00 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 23 Jan 2020 20:00:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jan 2020 20:00:02 GMT
EXPOSE 5432
# Thu, 23 Jan 2020 20:00:03 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:896868b7b9168cabb308702db96dc9769d10c23e20fc66f5f4abedf4c75d7642`  
		Last Modified: Thu, 23 Jan 2020 16:54:07 GMT  
		Size: 2.6 MB (2571407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c1dfea7b5ef394243de77186565b9885db2299f51fa267004f88c996fb15373`  
		Last Modified: Thu, 23 Jan 2020 20:09:52 GMT  
		Size: 179.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca2662a9d9cf0269ee05d7c3956f243450b70970a8b4ec9a88e552a830bf2b31`  
		Last Modified: Thu, 23 Jan 2020 20:09:51 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed662eb249fa089fdc93eb24d909f5d7b8c386f58e9c64567eb4fec48977906d`  
		Last Modified: Thu, 23 Jan 2020 20:11:02 GMT  
		Size: 52.7 MB (52678205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b411f495c4ba5c521160b7488580aaed0f697cf9c45e15a3c61241aa7955bc35`  
		Last Modified: Thu, 23 Jan 2020 20:10:43 GMT  
		Size: 7.6 KB (7567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0958e7395f5d344d6f331a8a91ba5886d3368b9641240a4dcfd14b439ca1a434`  
		Last Modified: Thu, 23 Jan 2020 20:10:43 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7dc1c9a1673c92c8c761127ddbdc1f5e52c3e26d6861c493e1b49b63cd9d40e`  
		Last Modified: Thu, 23 Jan 2020 20:10:43 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fa7aef942e694c8a2e3e5b91313fefd28e8dcee618b249c78f996d738eb44f6`  
		Last Modified: Thu, 23 Jan 2020 20:10:43 GMT  
		Size: 3.8 KB (3837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02dfa4e6cf3653be426bb61380ad36138df4b58dc5eabdb20bebdb9c1df00e48`  
		Last Modified: Thu, 23 Jan 2020 20:10:43 GMT  
		Size: 119.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:11-alpine` - linux; arm variant v7

```console
$ docker pull postgres@sha256:8c514209975888adf2b8e7ec4515447a3c647dcf08dc64859479d22403ea74c5
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.8 MB (52758607 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7d8ed954399301e50ae485cae6b27f952cf5a9b338eb4fd9a2441244906aa82e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:31 GMT
ADD file:d05c9f9143d11d12045d4faef882e5985e6b38fabe52237dd8d8c0627a9620ab in / 
# Thu, 23 Jan 2020 16:53:32 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 17:36:51 GMT
RUN set -ex; 	postgresHome="$(getent passwd postgres)"; 	postgresHome="$(echo "$postgresHome" | cut -d: -f6)"; 	[ "$postgresHome" = '/var/lib/postgresql' ]; 	mkdir -p "$postgresHome"; 	chown -R postgres:postgres "$postgresHome"
# Thu, 23 Jan 2020 17:36:52 GMT
ENV LANG=en_US.utf8
# Thu, 23 Jan 2020 17:36:54 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 23 Jan 2020 17:39:56 GMT
ENV PG_MAJOR=11
# Thu, 23 Jan 2020 17:39:57 GMT
ENV PG_VERSION=11.6
# Thu, 23 Jan 2020 17:39:57 GMT
ENV PG_SHA256=49924f7ff92965fdb20c86e0696f2dc9f8553e1563124ead7beedf8910c13170
# Thu, 23 Jan 2020 17:42:19 GMT
RUN set -ex 		&& apk add --no-cache --virtual .fetch-deps 		ca-certificates 		openssl 		tar 		&& wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2" 	&& echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c - 	&& mkdir -p /usr/src/postgresql 	&& tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	&& rm postgresql.tar.bz2 		&& apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm8-dev clang g++ 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 		&& cd /usr/src/postgresql 	&& awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new 	&& grep '/var/run/postgresql' src/include/pg_config_manual.h.new 	&& mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& ./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	&& make -j "$(nproc)" world 	&& make install-world 	&& make -C contrib install 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	&& apk del .fetch-deps .build-deps 	&& cd / 	&& rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	&& find /usr/local -name '*.a' -delete
# Thu, 23 Jan 2020 17:42:25 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Thu, 23 Jan 2020 17:42:28 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 23 Jan 2020 17:42:28 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 23 Jan 2020 17:42:31 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 23 Jan 2020 17:42:32 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 23 Jan 2020 17:42:32 GMT
COPY file:74700c51dbcbbad39fbd303750c2ac04ac10f59a73a55171e1fd0dbae6c2f311 in /usr/local/bin/ 
# Thu, 23 Jan 2020 17:42:34 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 23 Jan 2020 17:42:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jan 2020 17:42:36 GMT
EXPOSE 5432
# Thu, 23 Jan 2020 17:42:36 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:4e972d957a606327b0b6c2e8aa4a6045c263b7496a536298aaebf690e9d85f1d`  
		Last Modified: Thu, 23 Jan 2020 16:53:59 GMT  
		Size: 2.4 MB (2378408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edb5efececf79046d139464b5e2862622e506df6c0d3c1def4c1baac66e6c684`  
		Last Modified: Thu, 23 Jan 2020 17:52:42 GMT  
		Size: 179.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59d75c78c7d825098c01c4ecbe8a67dbcd2d96cddddc5e65366016e2584cb1c7`  
		Last Modified: Thu, 23 Jan 2020 17:52:41 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e09ea3e3cd66c026359e892a897380b4ce5b68b0637e33da4f7e636669f8a55`  
		Last Modified: Thu, 23 Jan 2020 17:54:05 GMT  
		Size: 50.4 MB (50367994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea20399c64017948bbe449e55cca9ad319604f76db7393baadc9b4cf3b6252b8`  
		Last Modified: Thu, 23 Jan 2020 17:53:21 GMT  
		Size: 7.6 KB (7568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:845750b4e28ddce22c2ccd07b8e734bb50e85d96ed363ab921857d9f31adef05`  
		Last Modified: Thu, 23 Jan 2020 17:53:21 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f175fb0ef42e4805157707d6b6517df9f376eeb98e0beac6a61810fd8a6a7ee`  
		Last Modified: Thu, 23 Jan 2020 17:53:21 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cee838b7550fb8cf8976a278e2ed2a5fd01d91375ffe19c4e793d6a6e1a4dad4`  
		Last Modified: Thu, 23 Jan 2020 17:53:22 GMT  
		Size: 3.8 KB (3834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56f511a701537fbb70ef8d397de1567570d90ee33f7b364ce4b10bb3a71902bb`  
		Last Modified: Thu, 23 Jan 2020 17:53:21 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:11-alpine` - linux; arm64 variant v8

```console
$ docker pull postgres@sha256:1e0d01f548d99ef0b65a33bb0e09a29286eedbb92bcfc002a457b7046db50cc9
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.1 MB (57095136 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:266649f128636431a853e3c5ad3c4f1675e44468dd3c4e8d41e0cfc312d8692c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 23 Jan 2020 16:54:39 GMT
ADD file:bdfbd4b0dfb53eecc80bac65894d1e2fcfafb27dcf24ab019176e2c9f60b9a39 in / 
# Thu, 23 Jan 2020 16:54:40 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 20:35:18 GMT
RUN set -ex; 	postgresHome="$(getent passwd postgres)"; 	postgresHome="$(echo "$postgresHome" | cut -d: -f6)"; 	[ "$postgresHome" = '/var/lib/postgresql' ]; 	mkdir -p "$postgresHome"; 	chown -R postgres:postgres "$postgresHome"
# Thu, 23 Jan 2020 20:35:19 GMT
ENV LANG=en_US.utf8
# Thu, 23 Jan 2020 20:35:21 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 23 Jan 2020 20:39:56 GMT
ENV PG_MAJOR=11
# Thu, 23 Jan 2020 20:39:59 GMT
ENV PG_VERSION=11.6
# Thu, 23 Jan 2020 20:40:00 GMT
ENV PG_SHA256=49924f7ff92965fdb20c86e0696f2dc9f8553e1563124ead7beedf8910c13170
# Thu, 23 Jan 2020 20:43:34 GMT
RUN set -ex 		&& apk add --no-cache --virtual .fetch-deps 		ca-certificates 		openssl 		tar 		&& wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2" 	&& echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c - 	&& mkdir -p /usr/src/postgresql 	&& tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	&& rm postgresql.tar.bz2 		&& apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm8-dev clang g++ 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 		&& cd /usr/src/postgresql 	&& awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new 	&& grep '/var/run/postgresql' src/include/pg_config_manual.h.new 	&& mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& ./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	&& make -j "$(nproc)" world 	&& make install-world 	&& make -C contrib install 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	&& apk del .fetch-deps .build-deps 	&& cd / 	&& rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	&& find /usr/local -name '*.a' -delete
# Thu, 23 Jan 2020 20:43:37 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Thu, 23 Jan 2020 20:43:40 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 23 Jan 2020 20:43:41 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 23 Jan 2020 20:43:43 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 23 Jan 2020 20:43:44 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 23 Jan 2020 20:43:44 GMT
COPY file:74700c51dbcbbad39fbd303750c2ac04ac10f59a73a55171e1fd0dbae6c2f311 in /usr/local/bin/ 
# Thu, 23 Jan 2020 20:43:46 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 23 Jan 2020 20:43:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jan 2020 20:43:48 GMT
EXPOSE 5432
# Thu, 23 Jan 2020 20:43:49 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:f07e4bcf42b862c240f4c00f2f7ed362d7d93ca15151de547beda593f3b669e5`  
		Last Modified: Thu, 23 Jan 2020 16:55:24 GMT  
		Size: 2.7 MB (2717732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e53dca8fb1762a2f08191229e77dfced9229619775bc2f4b0bb20b014fbb18f`  
		Last Modified: Thu, 23 Jan 2020 20:56:29 GMT  
		Size: 179.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52e8dbad5d0192ce93934cf76723cc96e80a06017d43a8a63bda7e0911dc0b3d`  
		Last Modified: Thu, 23 Jan 2020 20:56:29 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a14b36d8ad6134181776cbb740e06b43aaf03f165b60ab4170a9c21abd6a10c`  
		Last Modified: Thu, 23 Jan 2020 20:57:55 GMT  
		Size: 54.4 MB (54365195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b09daf35db3cb08a0de7b3659fa832fe313bd67fedb2372b369e15e242e8ce30`  
		Last Modified: Thu, 23 Jan 2020 20:57:25 GMT  
		Size: 7.6 KB (7569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7b19d92909aeb753ea3787c6304bc957089c52e47cbf7e81f4b4ee0d9fcdce3`  
		Last Modified: Thu, 23 Jan 2020 20:57:25 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f0db89363c82280b29ef517dd5d17b058b91b1977d7b3b90f033a033db8c453`  
		Last Modified: Thu, 23 Jan 2020 20:57:25 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d785a9a9a3cb2b74f1e73351ce33660b4a44ae20e132bd7ed437a3153c6c1f1f`  
		Last Modified: Thu, 23 Jan 2020 20:57:25 GMT  
		Size: 3.8 KB (3836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ab6f7921b11292c27f0a8a18ada9babd3abf158d09eaceede8a797940644ae6`  
		Last Modified: Thu, 23 Jan 2020 20:57:25 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:11-alpine` - linux; 386

```console
$ docker pull postgres@sha256:ec079a02631657e55fb5f88580c83e262f4d03234262f087f25e52bc29902662
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.2 MB (60219327 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:191132eb362fb021fcd16da1b59153c4de769ef3c8ff624dbb799dd162ffcfd9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Mon, 21 Oct 2019 16:46:04 GMT
ADD file:dd3b3676fd9c1e0983ade68242b9b9ac5c477f3e4bfc97c2e78fd5db93a441c9 in / 
# Mon, 21 Oct 2019 16:46:04 GMT
CMD ["/bin/sh"]
# Tue, 22 Oct 2019 00:38:40 GMT
RUN set -ex; 	postgresHome="$(getent passwd postgres)"; 	postgresHome="$(echo "$postgresHome" | cut -d: -f6)"; 	[ "$postgresHome" = '/var/lib/postgresql' ]; 	mkdir -p "$postgresHome"; 	chown -R postgres:postgres "$postgresHome"
# Tue, 22 Oct 2019 00:38:40 GMT
ENV LANG=en_US.utf8
# Tue, 22 Oct 2019 00:38:42 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 22 Oct 2019 00:46:03 GMT
ENV PG_MAJOR=11
# Mon, 18 Nov 2019 20:43:49 GMT
ENV PG_VERSION=11.6
# Mon, 18 Nov 2019 20:43:50 GMT
ENV PG_SHA256=49924f7ff92965fdb20c86e0696f2dc9f8553e1563124ead7beedf8910c13170
# Thu, 28 Nov 2019 16:51:08 GMT
RUN set -ex 		&& apk add --no-cache --virtual .fetch-deps 		ca-certificates 		openssl 		tar 		&& wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2" 	&& echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c - 	&& mkdir -p /usr/src/postgresql 	&& tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	&& rm postgresql.tar.bz2 		&& apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm8-dev clang g++ 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 		&& cd /usr/src/postgresql 	&& awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new 	&& grep '/var/run/postgresql' src/include/pg_config_manual.h.new 	&& mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& ./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	&& make -j "$(nproc)" world 	&& make install-world 	&& make -C contrib install 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	&& apk del .fetch-deps .build-deps 	&& cd / 	&& rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	&& find /usr/local -name '*.a' -delete
# Thu, 28 Nov 2019 16:51:09 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Thu, 28 Nov 2019 16:51:09 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 28 Nov 2019 16:51:10 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 28 Nov 2019 16:51:10 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 28 Nov 2019 16:51:10 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 03 Dec 2019 23:46:42 GMT
COPY file:74700c51dbcbbad39fbd303750c2ac04ac10f59a73a55171e1fd0dbae6c2f311 in /usr/local/bin/ 
# Tue, 03 Dec 2019 23:46:43 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Tue, 03 Dec 2019 23:46:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 03 Dec 2019 23:46:43 GMT
EXPOSE 5432
# Tue, 03 Dec 2019 23:46:43 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:f913bd05bf684aaa4bc173d73cfbb58abb45587962d74f0aa71df36b6b489def`  
		Last Modified: Mon, 21 Oct 2019 16:46:25 GMT  
		Size: 2.8 MB (2785939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f34d8b3207fc27ae3e199da966892810baab60a35d1f13fb8caba72c79d10107`  
		Last Modified: Tue, 22 Oct 2019 01:18:45 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:700ba88931304f86992d61359c40d19c27f8c56955a3a0a52598ca6a55ea7cdc`  
		Last Modified: Tue, 22 Oct 2019 01:18:44 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5bc8c82ac4211deb452a97eba171006b033127c2f48a85bd908f6361752be99`  
		Last Modified: Thu, 28 Nov 2019 16:52:34 GMT  
		Size: 57.4 MB (57421295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b20350d841ed004f0e5228ef88c981c185a074f9885035efb9b8b717a8b6adbb`  
		Last Modified: Thu, 28 Nov 2019 16:52:21 GMT  
		Size: 7.6 KB (7574 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc817b3a20bd5d1d6e090b1235f714c8984e9b0b08592b287ee7e735c8131d18`  
		Last Modified: Thu, 28 Nov 2019 16:52:21 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ea7af15a9602903e3d0f5da8c7ad86b2166ead2bfabd0ee8cd1369d38d3befc`  
		Last Modified: Thu, 28 Nov 2019 16:52:21 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ba6de6e842da9f7d48a7638c3aa0cb5381038ae0062d4726d607f0236925004`  
		Last Modified: Tue, 03 Dec 2019 23:47:55 GMT  
		Size: 3.8 KB (3844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfd614c2dc80cef76dac76fad23dcb1bb63ed3140ce754dac937e62e3316567f`  
		Last Modified: Tue, 03 Dec 2019 23:47:55 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:11-alpine` - linux; ppc64le

```console
$ docker pull postgres@sha256:c7d3c4a278fa411c8740f8e551edc588da204c0de4d5f7e2bd2dccf4014c6034
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.8 MB (59750672 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f237bfb4711486c8a43d5ca65041cc49f72d71be0f874f1a0abd952c7ab59c37`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 23 Jan 2020 16:57:54 GMT
ADD file:5e383dfaf3281b9cc17caf519d1aeba934fa92632c10afb8cc189f6ba12d9f64 in / 
# Thu, 23 Jan 2020 16:57:58 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 17:51:08 GMT
RUN set -ex; 	postgresHome="$(getent passwd postgres)"; 	postgresHome="$(echo "$postgresHome" | cut -d: -f6)"; 	[ "$postgresHome" = '/var/lib/postgresql' ]; 	mkdir -p "$postgresHome"; 	chown -R postgres:postgres "$postgresHome"
# Thu, 23 Jan 2020 17:51:12 GMT
ENV LANG=en_US.utf8
# Thu, 23 Jan 2020 17:51:24 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 23 Jan 2020 17:57:38 GMT
ENV PG_MAJOR=11
# Thu, 23 Jan 2020 17:57:41 GMT
ENV PG_VERSION=11.6
# Thu, 23 Jan 2020 17:57:44 GMT
ENV PG_SHA256=49924f7ff92965fdb20c86e0696f2dc9f8553e1563124ead7beedf8910c13170
# Thu, 23 Jan 2020 18:02:26 GMT
RUN set -ex 		&& apk add --no-cache --virtual .fetch-deps 		ca-certificates 		openssl 		tar 		&& wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2" 	&& echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c - 	&& mkdir -p /usr/src/postgresql 	&& tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	&& rm postgresql.tar.bz2 		&& apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm8-dev clang g++ 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 		&& cd /usr/src/postgresql 	&& awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new 	&& grep '/var/run/postgresql' src/include/pg_config_manual.h.new 	&& mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& ./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	&& make -j "$(nproc)" world 	&& make install-world 	&& make -C contrib install 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	&& apk del .fetch-deps .build-deps 	&& cd / 	&& rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	&& find /usr/local -name '*.a' -delete
# Thu, 23 Jan 2020 18:02:37 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Thu, 23 Jan 2020 18:02:49 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 23 Jan 2020 18:02:53 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 23 Jan 2020 18:03:00 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 23 Jan 2020 18:03:04 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 23 Jan 2020 18:03:08 GMT
COPY file:74700c51dbcbbad39fbd303750c2ac04ac10f59a73a55171e1fd0dbae6c2f311 in /usr/local/bin/ 
# Thu, 23 Jan 2020 18:03:17 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 23 Jan 2020 18:03:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jan 2020 18:03:23 GMT
EXPOSE 5432
# Thu, 23 Jan 2020 18:03:26 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:4ae00dedbff84a762d4b8b9176da2beee50017c43fe09a5ae92c2417d5634510`  
		Last Modified: Thu, 23 Jan 2020 16:58:43 GMT  
		Size: 2.8 MB (2808535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90f922a74c22acbd054a4d8bcafa004abdfe4f8476fa0e24e831ed5fe57ffaae`  
		Last Modified: Thu, 23 Jan 2020 18:20:23 GMT  
		Size: 178.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e709390f04f9b91990fafd468b6b2f7e222ffbda714a9b80bfeeba40479091f4`  
		Last Modified: Thu, 23 Jan 2020 18:20:22 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ce4ecbced2d40ffb7418f9e707b420f812e97df95a30b582e7a1b6a2e96dcb8`  
		Last Modified: Thu, 23 Jan 2020 18:22:10 GMT  
		Size: 56.9 MB (56929927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6e4fbca9caae04a338b094b9699bc01637399145daa49362a3f45d7521fae4f`  
		Last Modified: Thu, 23 Jan 2020 18:21:29 GMT  
		Size: 7.6 KB (7569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0ad37155ac3552fe28e437d0fe9d3da9e343a2171d32e85c29c3982f9829a31`  
		Last Modified: Thu, 23 Jan 2020 18:21:29 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4059f7fb82a32e06a15a0da59930f09b3103820fd3190ed17eced1bd3e36bb8f`  
		Last Modified: Thu, 23 Jan 2020 18:21:29 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e69135333f3a12a0a45ddb2006081227e0c45d25917fef1952be2892ad322b5e`  
		Last Modified: Thu, 23 Jan 2020 18:21:29 GMT  
		Size: 3.8 KB (3837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8cdc8caef271ebb4e458e41f4cf375c79101cb960c522feb6f3e9099ac3da19`  
		Last Modified: Thu, 23 Jan 2020 18:21:29 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:11-alpine` - linux; s390x

```console
$ docker pull postgres@sha256:c7a74e0bf83e0daa77ffacaa26eb1eb4fc0ba63eb0011a4a9f7042643179d101
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.3 MB (59264133 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d8444a3ba2d7eee1ae9d6dac3d2524e903c42792c5d1d40375971f778041fa7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 23 Jan 2020 16:52:43 GMT
ADD file:922e12714922ae035a33d6ceb8d2683ad3e454deca21ad02b699db908443342b in / 
# Thu, 23 Jan 2020 16:52:44 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 18:59:13 GMT
RUN set -ex; 	postgresHome="$(getent passwd postgres)"; 	postgresHome="$(echo "$postgresHome" | cut -d: -f6)"; 	[ "$postgresHome" = '/var/lib/postgresql' ]; 	mkdir -p "$postgresHome"; 	chown -R postgres:postgres "$postgresHome"
# Thu, 23 Jan 2020 18:59:13 GMT
ENV LANG=en_US.utf8
# Thu, 23 Jan 2020 18:59:14 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 23 Jan 2020 19:03:21 GMT
ENV PG_MAJOR=11
# Thu, 23 Jan 2020 19:03:21 GMT
ENV PG_VERSION=11.6
# Thu, 23 Jan 2020 19:03:21 GMT
ENV PG_SHA256=49924f7ff92965fdb20c86e0696f2dc9f8553e1563124ead7beedf8910c13170
# Thu, 23 Jan 2020 19:07:15 GMT
RUN set -ex 		&& apk add --no-cache --virtual .fetch-deps 		ca-certificates 		openssl 		tar 		&& wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2" 	&& echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c - 	&& mkdir -p /usr/src/postgresql 	&& tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	&& rm postgresql.tar.bz2 		&& apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm8-dev clang g++ 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 		&& cd /usr/src/postgresql 	&& awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new 	&& grep '/var/run/postgresql' src/include/pg_config_manual.h.new 	&& mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& ./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	&& make -j "$(nproc)" world 	&& make install-world 	&& make -C contrib install 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	&& apk del .fetch-deps .build-deps 	&& cd / 	&& rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	&& find /usr/local -name '*.a' -delete
# Thu, 23 Jan 2020 19:07:16 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Thu, 23 Jan 2020 19:07:16 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 23 Jan 2020 19:07:17 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 23 Jan 2020 19:07:17 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 23 Jan 2020 19:07:17 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 23 Jan 2020 19:07:18 GMT
COPY file:74700c51dbcbbad39fbd303750c2ac04ac10f59a73a55171e1fd0dbae6c2f311 in /usr/local/bin/ 
# Thu, 23 Jan 2020 19:07:18 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 23 Jan 2020 19:07:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jan 2020 19:07:19 GMT
EXPOSE 5432
# Thu, 23 Jan 2020 19:07:19 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:0449d076b2977b7e7ce4c35b0fe5199d86cabaf453e869da73b2efb66d6282dd`  
		Last Modified: Thu, 23 Jan 2020 16:53:07 GMT  
		Size: 2.6 MB (2573620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8cf14e46e1291c410abfc2822ada2f5ffe82474444f96894667d345465314f9`  
		Last Modified: Thu, 23 Jan 2020 19:16:14 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c5042a1c357b2db6445aba8b5204887abca909890912de154fe349d0336b644`  
		Last Modified: Thu, 23 Jan 2020 19:16:14 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f323c3073f908ae8b3a5d4d77e631a0353b6f080e93655846578adc94f333b2`  
		Last Modified: Thu, 23 Jan 2020 19:17:41 GMT  
		Size: 56.7 MB (56678434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04a1f9ca0aacd73ece022a927e68b40ae06735f85699bac548aee4315c7c0708`  
		Last Modified: Thu, 23 Jan 2020 19:16:59 GMT  
		Size: 7.6 KB (7568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94d341fbf9ff4d2c55fdbaae23552e7324b44ef0ff11742c71ea1da129bfc78b`  
		Last Modified: Thu, 23 Jan 2020 19:16:58 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe839c7beb5104a0ed31e7e8082429d2d0eaa07c26742ed13f2fb1637684bec4`  
		Last Modified: Thu, 23 Jan 2020 19:16:58 GMT  
		Size: 164.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cea123cd009063feac72c0a99b07cbcfd954f43dc07db1ce6484b3fa7b4fbc84`  
		Last Modified: Thu, 23 Jan 2020 19:16:59 GMT  
		Size: 3.8 KB (3835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4f89e4fee7a9a27dc79543fd3298685a583b81e47a0b9bb80e448c9935a13c3`  
		Last Modified: Thu, 23 Jan 2020 19:16:58 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
