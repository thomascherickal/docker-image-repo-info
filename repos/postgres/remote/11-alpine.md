## `postgres:11-alpine`

```console
$ docker pull postgres@sha256:310d4458efb289a29e581f9ee3e1efc0efd2b07d84767be43e97e249753d3c88
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
$ docker pull postgres@sha256:f4246390b7506d49fd5a8308bf0b2a240f26f0f3e7697eb17d4548898d63ffe1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.2 MB (59224560 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b41b79676e63162918a5edd3b4de10390b8f637d0ca0026e35d36e0335b8495d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Sat, 18 Jan 2020 01:19:37 GMT
ADD file:e69d441d729412d24675dcd33e04580885df99981cec43de8c9b24015313ff8e in / 
# Sat, 18 Jan 2020 01:19:37 GMT
CMD ["/bin/sh"]
# Thu, 30 Jan 2020 03:19:59 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 30 Jan 2020 03:19:59 GMT
ENV LANG=en_US.utf8
# Thu, 30 Jan 2020 03:20:00 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 30 Jan 2020 03:25:33 GMT
ENV PG_MAJOR=11
# Fri, 14 Feb 2020 17:27:22 GMT
ENV PG_VERSION=11.7
# Fri, 14 Feb 2020 17:27:22 GMT
ENV PG_SHA256=324ae93a8846fbb6a25d562d271bc441ffa8794654c5b2839384834de220a313
# Fri, 14 Feb 2020 17:32:39 GMT
RUN set -ex 		&& apk add --no-cache --virtual .fetch-deps 		ca-certificates 		openssl 		tar 		&& wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2" 	&& echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c - 	&& mkdir -p /usr/src/postgresql 	&& tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	&& rm postgresql.tar.bz2 		&& apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm9-dev clang g++ 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 		&& cd /usr/src/postgresql 	&& awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new 	&& grep '/var/run/postgresql' src/include/pg_config_manual.h.new 	&& mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& ./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	&& make -j "$(nproc)" world 	&& make install-world 	&& make -C contrib install 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	&& apk del .fetch-deps .build-deps 	&& cd / 	&& rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	&& find /usr/local -name '*.a' -delete
# Fri, 14 Feb 2020 17:32:40 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Fri, 14 Feb 2020 17:32:41 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 14 Feb 2020 17:32:41 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 14 Feb 2020 17:32:41 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 14 Feb 2020 17:32:42 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 14 Feb 2020 17:32:42 GMT
COPY file:7d708673b2130c7c27f9df46864fa71f6dc27527edb4acc7a5365f8cf885d4af in /usr/local/bin/ 
# Fri, 14 Feb 2020 17:32:43 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 14 Feb 2020 17:32:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 14 Feb 2020 17:32:43 GMT
EXPOSE 5432
# Fri, 14 Feb 2020 17:32:43 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:c9b1b535fdd91a9855fb7f82348177e5f019329a58c53c47272962dd60f71fc9`  
		Last Modified: Fri, 17 Jan 2020 08:04:01 GMT  
		Size: 2.8 MB (2802957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1030c456d04636112fa347ddc5296036cddf70c8085be2e3f3fb481898f18fe`  
		Last Modified: Thu, 30 Jan 2020 03:42:56 GMT  
		Size: 1.2 KB (1247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1d0211bbd9a4fd28f739a797600d78394b15d947a30f55f70cfd5daf0f9e443`  
		Last Modified: Thu, 30 Jan 2020 03:42:55 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fb6a7c48f4710fa2306c843ffbdcf99d8dcc136cb4357726d47d1ce83d05364`  
		Last Modified: Fri, 14 Feb 2020 17:52:53 GMT  
		Size: 56.4 MB (56408078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4feeaa95cfef356494be08617734aff45e8ee45c1f0041ab1bb9a0c74e24d9ed`  
		Last Modified: Fri, 14 Feb 2020 17:52:37 GMT  
		Size: 7.6 KB (7568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d670ed1adf136244d7f26656f29c355698681a7f674a45975dd3fca0f59bf91`  
		Last Modified: Fri, 14 Feb 2020 17:52:37 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12390eb4089492acbf32f25b49ec8104470a1f6a1c69f20f634308ebed330cc2`  
		Last Modified: Fri, 14 Feb 2020 17:52:37 GMT  
		Size: 165.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69c17c7edd1d245d69a71eb5045a6d3e45b22bccaaf23cfc54d8245460a41f06`  
		Last Modified: Fri, 14 Feb 2020 17:52:37 GMT  
		Size: 4.2 KB (4180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4df0b59148284a3be2321cfa76c8cc86eaee55093846d3270e306d8268ecba1e`  
		Last Modified: Fri, 14 Feb 2020 17:52:38 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:11-alpine` - linux; arm variant v6

```console
$ docker pull postgres@sha256:09dde11b47cbeb5463153a3c6ef53371b16198959a2457d345a5264de3c92514
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.6 MB (57585963 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c3f2556955ab5047435d6c4016b91fa47d1bea58ac2c0ff8ad44957e6f1001c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Sat, 18 Jan 2020 01:53:16 GMT
ADD file:a1906f14a4e217a498b550f86a3d17c9012c02a6df0668043b63848c8fa44b9b in / 
# Sat, 18 Jan 2020 01:53:17 GMT
CMD ["/bin/sh"]
# Fri, 21 Feb 2020 00:42:27 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Fri, 21 Feb 2020 00:42:28 GMT
ENV LANG=en_US.utf8
# Fri, 21 Feb 2020 00:42:32 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 21 Feb 2020 00:48:35 GMT
ENV PG_MAJOR=11
# Fri, 21 Feb 2020 00:48:39 GMT
ENV PG_VERSION=11.7
# Fri, 21 Feb 2020 00:48:48 GMT
ENV PG_SHA256=324ae93a8846fbb6a25d562d271bc441ffa8794654c5b2839384834de220a313
# Fri, 21 Feb 2020 00:55:06 GMT
RUN set -ex 		&& apk add --no-cache --virtual .fetch-deps 		ca-certificates 		openssl 		tar 		&& wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2" 	&& echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c - 	&& mkdir -p /usr/src/postgresql 	&& tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	&& rm postgresql.tar.bz2 		&& apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm9-dev clang g++ 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 		&& cd /usr/src/postgresql 	&& awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new 	&& grep '/var/run/postgresql' src/include/pg_config_manual.h.new 	&& mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& ./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	&& make -j "$(nproc)" world 	&& make install-world 	&& make -C contrib install 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	&& apk del .fetch-deps .build-deps 	&& cd / 	&& rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	&& find /usr/local -name '*.a' -delete
# Fri, 21 Feb 2020 00:55:16 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Fri, 21 Feb 2020 00:55:25 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 21 Feb 2020 00:55:30 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 21 Feb 2020 00:55:34 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 21 Feb 2020 00:55:36 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 21 Feb 2020 00:55:37 GMT
COPY file:fa1ca76844f23c5beb98bdf3620414d012eb44eabdb324f0cce0bd5b0b913477 in /usr/local/bin/ 
# Fri, 21 Feb 2020 00:55:43 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 21 Feb 2020 00:55:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 21 Feb 2020 00:55:49 GMT
EXPOSE 5432
# Fri, 21 Feb 2020 00:55:52 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:832e07764099264ef96e50a1e5e41c52d6b0809bd054e29508a6878aa59d156d`  
		Last Modified: Sat, 18 Jan 2020 01:53:52 GMT  
		Size: 2.6 MB (2617562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c288e93ef5b01ac6124357c0936a9a28b458e8b331cfb2234bba3d58a80b8c35`  
		Last Modified: Fri, 21 Feb 2020 01:07:27 GMT  
		Size: 1.3 KB (1278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95e9b75c81caf8fead15ad12a8b5a6104156da54990def5f42fab50a350445e5`  
		Last Modified: Fri, 21 Feb 2020 01:07:26 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b26676086e198c81d43c953d792cbba38679793beaadd8e5727eec75689cfcb2`  
		Last Modified: Fri, 21 Feb 2020 01:08:19 GMT  
		Size: 55.0 MB (54954709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d0b7e44020ed81138bdb8ff77db2288eec516fbea04f127ce15f90ad3108314`  
		Last Modified: Fri, 21 Feb 2020 01:08:00 GMT  
		Size: 7.6 KB (7572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9f4f7d268fc2f54fff255411a593546560e2d7d2e6f0c2075e59400a841d80f`  
		Last Modified: Fri, 21 Feb 2020 01:08:00 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0e8566cc4c9bc7e1d5ab370ae0bc98d0d4f82aed6da6c8c9d3c35de1cfe2a02`  
		Last Modified: Fri, 21 Feb 2020 01:08:00 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ae73c649dedc462ed32bb9f7cee1074032b66e8bb0124a566fba6d47ba183c6`  
		Last Modified: Fri, 21 Feb 2020 01:08:00 GMT  
		Size: 4.2 KB (4219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5f538b9284d54b5c79bb9a8463163dde4dc5326832a77898787f2af9a076879`  
		Last Modified: Fri, 21 Feb 2020 01:08:00 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:11-alpine` - linux; arm variant v7

```console
$ docker pull postgres@sha256:a8cb781bb3a08f1d287383410a2bd9c88b76de3fd61dc6ee161f321b7698e8a6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.9 MB (54877367 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:095d9ed79f87957d5317ea0561acb44203ae3ac5705d17f1229d5f51f0d45f50`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Sat, 18 Jan 2020 02:03:19 GMT
ADD file:4c815f4461ff3b8d481f43d84eb2548cb1adbb3015d370cab86dd7f4d3d94279 in / 
# Sat, 18 Jan 2020 02:03:22 GMT
CMD ["/bin/sh"]
# Thu, 30 Jan 2020 03:00:10 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 30 Jan 2020 03:00:13 GMT
ENV LANG=en_US.utf8
# Thu, 30 Jan 2020 03:00:15 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 30 Jan 2020 03:03:58 GMT
ENV PG_MAJOR=11
# Fri, 14 Feb 2020 17:43:28 GMT
ENV PG_VERSION=11.7
# Fri, 14 Feb 2020 17:43:29 GMT
ENV PG_SHA256=324ae93a8846fbb6a25d562d271bc441ffa8794654c5b2839384834de220a313
# Fri, 14 Feb 2020 17:46:14 GMT
RUN set -ex 		&& apk add --no-cache --virtual .fetch-deps 		ca-certificates 		openssl 		tar 		&& wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2" 	&& echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c - 	&& mkdir -p /usr/src/postgresql 	&& tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	&& rm postgresql.tar.bz2 		&& apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm9-dev clang g++ 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 		&& cd /usr/src/postgresql 	&& awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new 	&& grep '/var/run/postgresql' src/include/pg_config_manual.h.new 	&& mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& ./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	&& make -j "$(nproc)" world 	&& make install-world 	&& make -C contrib install 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	&& apk del .fetch-deps .build-deps 	&& cd / 	&& rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	&& find /usr/local -name '*.a' -delete
# Fri, 14 Feb 2020 17:46:17 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Fri, 14 Feb 2020 17:46:19 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 14 Feb 2020 17:46:19 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 14 Feb 2020 17:46:21 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 14 Feb 2020 17:46:22 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 14 Feb 2020 17:46:22 GMT
COPY file:7d708673b2130c7c27f9df46864fa71f6dc27527edb4acc7a5365f8cf885d4af in /usr/local/bin/ 
# Fri, 14 Feb 2020 17:46:24 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 14 Feb 2020 17:46:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 14 Feb 2020 17:46:25 GMT
EXPOSE 5432
# Fri, 14 Feb 2020 17:46:26 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:3a2c5e3c37b2e3d749405512ef3793aa45a2f5c11615d9e9efa80179262cdf27`  
		Last Modified: Sat, 18 Jan 2020 02:04:05 GMT  
		Size: 2.4 MB (2419554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:572777a7d0992ea05b14f2ba3230ce906c753dd21eb73ac2b6018551250312db`  
		Last Modified: Thu, 30 Jan 2020 03:18:34 GMT  
		Size: 1.3 KB (1273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e8810228251d658112d3dbf2b9b1719f402a0c3477bf2eceaa5a20341bba3f5`  
		Last Modified: Thu, 30 Jan 2020 03:18:34 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c0ef0ccfb2681d3d8eeba2b8ae0b217739171ce879cfb40222573131fdf41aa`  
		Last Modified: Fri, 14 Feb 2020 19:13:24 GMT  
		Size: 52.4 MB (52444163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:182b90dc3da004ffd47a3d8865ecbd43c5d197f108f8f117ced1adc110be057e`  
		Last Modified: Fri, 14 Feb 2020 19:13:05 GMT  
		Size: 7.6 KB (7569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07ad5d88850fb8b82cac3d1f112ae4125e531fd2fa74f6d1ec8ed7617a116634`  
		Last Modified: Fri, 14 Feb 2020 19:13:05 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eca1c8d9524475d9f873913465ddab8ad2d18ca7c7bf2fe283c0be37e4de4096`  
		Last Modified: Fri, 14 Feb 2020 19:13:05 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c661ebf749719601475e362c9925fe575c6fd30c85f16210efa7e9b45e116ec0`  
		Last Modified: Fri, 14 Feb 2020 19:13:05 GMT  
		Size: 4.2 KB (4183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9d6a611826243230c767212f34c8d475ab4df802f8fa2bd3c0f944e9c0d1d1a`  
		Last Modified: Fri, 14 Feb 2020 19:13:05 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:11-alpine` - linux; arm64 variant v8

```console
$ docker pull postgres@sha256:67886481161d2c6c634932fa2c53f184e3fc055816e30fd366ca9fc0a72f706c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.8 MB (58823536 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b1d405b493b592773be57535c2162b842e9df81afb2850f8eb365f93fb2d1318`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Sat, 18 Jan 2020 01:39:43 GMT
ADD file:4109fa86dd80850e84c689ff9e6a3243e30ab1bbcc00c765969b3011bfbb43e1 in / 
# Sat, 18 Jan 2020 01:39:43 GMT
CMD ["/bin/sh"]
# Thu, 30 Jan 2020 02:40:27 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 30 Jan 2020 02:40:28 GMT
ENV LANG=en_US.utf8
# Thu, 30 Jan 2020 02:40:29 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 30 Jan 2020 02:44:03 GMT
ENV PG_MAJOR=11
# Fri, 14 Feb 2020 18:30:00 GMT
ENV PG_VERSION=11.7
# Fri, 14 Feb 2020 18:30:00 GMT
ENV PG_SHA256=324ae93a8846fbb6a25d562d271bc441ffa8794654c5b2839384834de220a313
# Fri, 14 Feb 2020 18:33:10 GMT
RUN set -ex 		&& apk add --no-cache --virtual .fetch-deps 		ca-certificates 		openssl 		tar 		&& wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2" 	&& echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c - 	&& mkdir -p /usr/src/postgresql 	&& tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	&& rm postgresql.tar.bz2 		&& apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm9-dev clang g++ 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 		&& cd /usr/src/postgresql 	&& awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new 	&& grep '/var/run/postgresql' src/include/pg_config_manual.h.new 	&& mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& ./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	&& make -j "$(nproc)" world 	&& make install-world 	&& make -C contrib install 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	&& apk del .fetch-deps .build-deps 	&& cd / 	&& rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	&& find /usr/local -name '*.a' -delete
# Fri, 14 Feb 2020 18:33:15 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Fri, 14 Feb 2020 18:33:17 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 14 Feb 2020 18:33:18 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 14 Feb 2020 18:33:20 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 14 Feb 2020 18:33:21 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 14 Feb 2020 18:33:21 GMT
COPY file:7d708673b2130c7c27f9df46864fa71f6dc27527edb4acc7a5365f8cf885d4af in /usr/local/bin/ 
# Fri, 14 Feb 2020 18:33:23 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 14 Feb 2020 18:33:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 14 Feb 2020 18:33:24 GMT
EXPOSE 5432
# Fri, 14 Feb 2020 18:33:25 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:8fa90b21c985a6fcfff966bdfbde81cdd088de0aa8af38110057f6ac408f4408`  
		Last Modified: Sat, 18 Jan 2020 01:40:23 GMT  
		Size: 2.7 MB (2723075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9db837ff5778a13ace9e439e3bff33c317ecca84803a142a4ee4e05d2af54def`  
		Last Modified: Thu, 30 Jan 2020 02:59:49 GMT  
		Size: 1.3 KB (1273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c92b445ab1ef4ba9a6120e5cc359b70cb88b74a46dee803f2709cb873a7be79`  
		Last Modified: Thu, 30 Jan 2020 02:59:49 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d8d2e30cc6ec07f3d310ab87760836c1db08392d33b31b846abcd35c03e900a`  
		Last Modified: Fri, 14 Feb 2020 19:58:38 GMT  
		Size: 56.1 MB (56086810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31d1e2e2f8b7ca8d90647087705fec99bb689115090ea5aa1b4d9c0fe284ea9a`  
		Last Modified: Fri, 14 Feb 2020 19:58:21 GMT  
		Size: 7.6 KB (7575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:023e3a5f745914538cc665b3fe08e75f1e55d587d3b6ac55f75c1dac661e7295`  
		Last Modified: Fri, 14 Feb 2020 19:58:21 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb1088834a395babdab7c75abc297a28e6be850a48993e6f0179dec621912184`  
		Last Modified: Fri, 14 Feb 2020 19:58:21 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46078b5dda57c656884c436fffd1888604c6ade8d37ab41362e63f550a3f47e4`  
		Last Modified: Fri, 14 Feb 2020 19:58:21 GMT  
		Size: 4.2 KB (4180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf93719ab48025086dee49b9813b10adea951cfda943a5657522126d49d428e1`  
		Last Modified: Fri, 14 Feb 2020 19:58:21 GMT  
		Size: 118.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:11-alpine` - linux; 386

```console
$ docker pull postgres@sha256:8f840386991c7a0dbe20f3debecdc13c18aa04819ec4dd6c1ce567f8f455991f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.4 MB (62422658 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9dda53383795a167a6b4f9d0c0c528e3181dd2f65bcd00c51c484db7295086bf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Sat, 18 Jan 2020 01:38:44 GMT
ADD file:381b617b92fe699ad4ef4f30e0d9599f89e43e252883348c420ebe2a0cccbd63 in / 
# Sat, 18 Jan 2020 01:38:45 GMT
CMD ["/bin/sh"]
# Thu, 30 Jan 2020 02:38:44 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 30 Jan 2020 02:38:44 GMT
ENV LANG=en_US.utf8
# Thu, 30 Jan 2020 02:38:45 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 30 Jan 2020 02:45:34 GMT
ENV PG_MAJOR=11
# Fri, 14 Feb 2020 17:51:16 GMT
ENV PG_VERSION=11.7
# Fri, 14 Feb 2020 17:51:16 GMT
ENV PG_SHA256=324ae93a8846fbb6a25d562d271bc441ffa8794654c5b2839384834de220a313
# Fri, 14 Feb 2020 17:58:16 GMT
RUN set -ex 		&& apk add --no-cache --virtual .fetch-deps 		ca-certificates 		openssl 		tar 		&& wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2" 	&& echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c - 	&& mkdir -p /usr/src/postgresql 	&& tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	&& rm postgresql.tar.bz2 		&& apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm9-dev clang g++ 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 		&& cd /usr/src/postgresql 	&& awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new 	&& grep '/var/run/postgresql' src/include/pg_config_manual.h.new 	&& mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& ./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	&& make -j "$(nproc)" world 	&& make install-world 	&& make -C contrib install 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	&& apk del .fetch-deps .build-deps 	&& cd / 	&& rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	&& find /usr/local -name '*.a' -delete
# Fri, 14 Feb 2020 17:58:17 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Fri, 14 Feb 2020 17:58:17 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 14 Feb 2020 17:58:18 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 14 Feb 2020 17:58:18 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 14 Feb 2020 17:58:18 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 14 Feb 2020 17:58:19 GMT
COPY file:7d708673b2130c7c27f9df46864fa71f6dc27527edb4acc7a5365f8cf885d4af in /usr/local/bin/ 
# Fri, 14 Feb 2020 17:58:19 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 14 Feb 2020 17:58:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 14 Feb 2020 17:58:20 GMT
EXPOSE 5432
# Fri, 14 Feb 2020 17:58:20 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:f024b1263dc58db07a458b73ae1a2dca02ca55bef1ccd1fa3fd50656551fadf2`  
		Last Modified: Sat, 18 Jan 2020 01:39:18 GMT  
		Size: 2.8 MB (2806560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b2cb8463eb063fd24e3d29bd4ca5b9ba1590717acda7415cb45da3e7560f0dd`  
		Last Modified: Thu, 30 Jan 2020 03:07:21 GMT  
		Size: 1.2 KB (1245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b023c33adbfeb9b779f40edac1617b4514e1fb0b976b5b201dd0f7dc688f5e60`  
		Last Modified: Thu, 30 Jan 2020 03:07:21 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c452dfb6d7458b49bc87f46bf0930b3d5aaf23e54c457286485535cb0ae5b60`  
		Last Modified: Fri, 14 Feb 2020 18:17:46 GMT  
		Size: 59.6 MB (59602580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e65f4726c7069d109fffae24a17035ad98f6f97c00a8b7fda0172c41b5b69e73`  
		Last Modified: Fri, 14 Feb 2020 18:17:32 GMT  
		Size: 7.6 KB (7565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1814059009365e1af2f6508f1505e857f093ad582c6a5533b13a415199ea6005`  
		Last Modified: Fri, 14 Feb 2020 18:17:32 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dd85de98888cd565ed6498d6ff157756e0ba3fa3cd40d288ea48a7e1816152b`  
		Last Modified: Fri, 14 Feb 2020 18:17:33 GMT  
		Size: 164.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f77209323c4bcd4bab94960643bbea14adfe93d155d6549dff04a68d8da4b394`  
		Last Modified: Fri, 14 Feb 2020 18:17:32 GMT  
		Size: 4.2 KB (4180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:537b9ae83aa31705c5d325846a1ebcad4887852b02347d68ae35853e6b525c3c`  
		Last Modified: Fri, 14 Feb 2020 18:17:32 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:11-alpine` - linux; ppc64le

```console
$ docker pull postgres@sha256:e57cdb3f3511137dc22409f707518d7e5dbc3076e673a27f5241bd091050a9d2
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.5 MB (61456959 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b5e52927c4aca8b4b7ff3a6d4ff1763dba119d95c41a284a9d558cc9f11d2bc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Sat, 18 Jan 2020 02:20:41 GMT
ADD file:32ddb3d5255071cca51573ceee2464dd5a87c8d1cce514ae965b6e824d9ef24b in / 
# Sat, 18 Jan 2020 02:20:45 GMT
CMD ["/bin/sh"]
# Thu, 30 Jan 2020 03:20:01 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 30 Jan 2020 03:20:03 GMT
ENV LANG=en_US.utf8
# Thu, 30 Jan 2020 03:20:07 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 30 Jan 2020 03:29:13 GMT
ENV PG_MAJOR=11
# Fri, 14 Feb 2020 17:31:18 GMT
ENV PG_VERSION=11.7
# Fri, 14 Feb 2020 17:31:21 GMT
ENV PG_SHA256=324ae93a8846fbb6a25d562d271bc441ffa8794654c5b2839384834de220a313
# Fri, 14 Feb 2020 17:36:18 GMT
RUN set -ex 		&& apk add --no-cache --virtual .fetch-deps 		ca-certificates 		openssl 		tar 		&& wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2" 	&& echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c - 	&& mkdir -p /usr/src/postgresql 	&& tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	&& rm postgresql.tar.bz2 		&& apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm9-dev clang g++ 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 		&& cd /usr/src/postgresql 	&& awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new 	&& grep '/var/run/postgresql' src/include/pg_config_manual.h.new 	&& mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& ./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	&& make -j "$(nproc)" world 	&& make install-world 	&& make -C contrib install 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	&& apk del .fetch-deps .build-deps 	&& cd / 	&& rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	&& find /usr/local -name '*.a' -delete
# Fri, 14 Feb 2020 17:36:24 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Fri, 14 Feb 2020 17:36:29 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 14 Feb 2020 17:36:30 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 14 Feb 2020 17:36:36 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 14 Feb 2020 17:36:38 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 14 Feb 2020 17:36:39 GMT
COPY file:7d708673b2130c7c27f9df46864fa71f6dc27527edb4acc7a5365f8cf885d4af in /usr/local/bin/ 
# Fri, 14 Feb 2020 17:36:43 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 14 Feb 2020 17:36:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 14 Feb 2020 17:36:48 GMT
EXPOSE 5432
# Fri, 14 Feb 2020 17:36:50 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:cd95c8a93e39dcaa0634a65d5b86a88bcd5c3092adb1f96504a7030faa165123`  
		Last Modified: Sat, 18 Jan 2020 02:21:25 GMT  
		Size: 2.8 MB (2822125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fa8af198a4c612619984a3d16dc2a9fb3f15835dfbf5269a9eab9a345ed4f14`  
		Last Modified: Thu, 30 Jan 2020 03:53:26 GMT  
		Size: 1.3 KB (1275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7852af7c4759ead6b82b170b6d34d124532026b41ec5d7dc4ec99bd6705f633a`  
		Last Modified: Thu, 30 Jan 2020 03:53:26 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f85197cd1f1760f4d4518db57a6467a3639094ef356dcc0b3e36213546ed236`  
		Last Modified: Fri, 14 Feb 2020 18:12:27 GMT  
		Size: 58.6 MB (58621184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46035bc60c808cfcc6917eadbeaa99deb8048ff1eb96563716c13abe8bfbd391`  
		Last Modified: Fri, 14 Feb 2020 18:12:10 GMT  
		Size: 7.6 KB (7567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14f1d9938a7df8a7c36633b8561b5a18d08f3ec8bcee060fa8244cba6ee061d4`  
		Last Modified: Fri, 14 Feb 2020 18:12:10 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b91a6891d42114f0801ed7e72546c1d9aeec892b6654fc1e087ccd0c7b390c7`  
		Last Modified: Fri, 14 Feb 2020 18:12:10 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:484ff21b418d04582ca63432eec23ce059f83007bca9a98ead83075d23408530`  
		Last Modified: Fri, 14 Feb 2020 18:12:10 GMT  
		Size: 4.2 KB (4184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c8c838f2a6906a95b68e325d369988b823c3ddfc7e299b9526522c59e22e04f`  
		Last Modified: Fri, 14 Feb 2020 18:12:10 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:11-alpine` - linux; s390x

```console
$ docker pull postgres@sha256:72ceac7f4688c868e413889fe9e77acbf75888837cb37637fe4577d954080264
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.2 MB (61181069 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c373a80e3c023d2288854a69da089951c4372471f837880d786bea59e1b73b9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Sat, 18 Jan 2020 01:41:33 GMT
ADD file:a6f8b7d4ba199527053ef1ac710b5e318135cb6903cb9ad6fae4fe42e6ad0bf7 in / 
# Sat, 18 Jan 2020 01:41:33 GMT
CMD ["/bin/sh"]
# Fri, 21 Feb 2020 00:18:10 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Fri, 21 Feb 2020 00:18:10 GMT
ENV LANG=en_US.utf8
# Fri, 21 Feb 2020 00:18:12 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 21 Feb 2020 00:36:43 GMT
ENV PG_MAJOR=11
# Fri, 21 Feb 2020 00:36:44 GMT
ENV PG_VERSION=11.7
# Fri, 21 Feb 2020 00:36:44 GMT
ENV PG_SHA256=324ae93a8846fbb6a25d562d271bc441ffa8794654c5b2839384834de220a313
# Fri, 21 Feb 2020 00:42:56 GMT
RUN set -ex 		&& apk add --no-cache --virtual .fetch-deps 		ca-certificates 		openssl 		tar 		&& wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2" 	&& echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c - 	&& mkdir -p /usr/src/postgresql 	&& tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	&& rm postgresql.tar.bz2 		&& apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm9-dev clang g++ 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 		&& cd /usr/src/postgresql 	&& awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new 	&& grep '/var/run/postgresql' src/include/pg_config_manual.h.new 	&& mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& ./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	&& make -j "$(nproc)" world 	&& make install-world 	&& make -C contrib install 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	&& apk del .fetch-deps .build-deps 	&& cd / 	&& rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	&& find /usr/local -name '*.a' -delete
# Fri, 21 Feb 2020 00:43:05 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Fri, 21 Feb 2020 00:43:07 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 21 Feb 2020 00:43:08 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 21 Feb 2020 00:43:10 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 21 Feb 2020 00:43:11 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 21 Feb 2020 00:43:11 GMT
COPY file:fa1ca76844f23c5beb98bdf3620414d012eb44eabdb324f0cce0bd5b0b913477 in /usr/local/bin/ 
# Fri, 21 Feb 2020 00:43:13 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 21 Feb 2020 00:43:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 21 Feb 2020 00:43:14 GMT
EXPOSE 5432
# Fri, 21 Feb 2020 00:43:15 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:176bad61a3a435da03ec603d2bd8f7a69286d92f21f447b17f21f0bc4e085bde`  
		Last Modified: Sat, 18 Jan 2020 01:41:59 GMT  
		Size: 2.6 MB (2582031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:351827524ade65a9aeff2700d440f7f2bebfa06e09bfb97a7ac70bca2e59c9bd`  
		Last Modified: Fri, 21 Feb 2020 01:27:44 GMT  
		Size: 1.3 KB (1278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbb1c51f7255ecf03a8dff2b406f9fe7250980e67bb33cc0837625b64dff486b`  
		Last Modified: Fri, 21 Feb 2020 01:27:43 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a02bf8abf682be7380e3e53a908475e9416577078cf04e594bfdd43b87c19181`  
		Last Modified: Fri, 21 Feb 2020 01:28:38 GMT  
		Size: 58.6 MB (58585368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09c49f71d71bc67a87fb635686cbec5a20024ce2f769ced944c4643a2c5765d7`  
		Last Modified: Fri, 21 Feb 2020 01:28:27 GMT  
		Size: 7.6 KB (7561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1724b145ebf5a2d15fbb30d01105aad5880d7abeb4a7e4d424d167759cb0b0c5`  
		Last Modified: Fri, 21 Feb 2020 01:28:28 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04e611e96d794306aa53e19085c0b81278afb4f8af0f6b5b8812ddbb929c9dce`  
		Last Modified: Fri, 21 Feb 2020 01:28:43 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1231cf56feba0da40bdb65b95443ea8ba71cb52877368d0baf1eb76af531dc3b`  
		Last Modified: Fri, 21 Feb 2020 01:28:43 GMT  
		Size: 4.2 KB (4212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f62b5559ce4398bc23118fe76d74d36ff60d67252628c872f71cf685849065c`  
		Last Modified: Fri, 21 Feb 2020 01:28:43 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
