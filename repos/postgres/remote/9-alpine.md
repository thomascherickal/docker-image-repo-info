## `postgres:9-alpine`

```console
$ docker pull postgres@sha256:e32c43a515b32f8caad7fea4e53d44066409616986c59f0ee34daa494616b026
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
$ docker pull postgres@sha256:377bf07044d71ace1856a46ef10274e44f42021312f6273108db2cdfa280b8a9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.7 MB (14651834 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b1adbeb9895f6ec18760a82d85e7a00e678c1ace00261c76242c60270ecdf45f`
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
# Thu, 30 Jan 2020 03:34:11 GMT
ENV PG_MAJOR=9.6
# Fri, 14 Feb 2020 17:37:15 GMT
ENV PG_VERSION=9.6.17
# Fri, 14 Feb 2020 17:37:15 GMT
ENV PG_SHA256=f6e1e32d32545f97c066f3c19f4d58dfab1205c01252cf85c5c92294ace1a0c2
# Fri, 14 Feb 2020 17:40:07 GMT
RUN set -ex 		&& apk add --no-cache --virtual .fetch-deps 		ca-certificates 		openssl 		tar 		&& wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2" 	&& echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c - 	&& mkdir -p /usr/src/postgresql 	&& tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	&& rm postgresql.tar.bz2 		&& apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		&& cd /usr/src/postgresql 	&& awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new 	&& grep '/var/run/postgresql' src/include/pg_config_manual.h.new 	&& mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& ./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 	&& make -j "$(nproc)" world 	&& make install-world 	&& make -C contrib install 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	&& apk del .fetch-deps .build-deps 	&& cd / 	&& rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	&& find /usr/local -name '*.a' -delete
# Fri, 14 Feb 2020 17:40:08 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Fri, 14 Feb 2020 17:40:09 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 14 Feb 2020 17:40:09 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 14 Feb 2020 17:40:10 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 14 Feb 2020 17:40:10 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 14 Feb 2020 17:40:10 GMT
COPY file:dfac98688c352f175c627102a0e4369c11bf8cbed107e8d5861aac37a67fd519 in /usr/local/bin/ 
# Fri, 14 Feb 2020 17:40:11 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 14 Feb 2020 17:40:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 14 Feb 2020 17:40:11 GMT
EXPOSE 5432
# Fri, 14 Feb 2020 17:40:11 GMT
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
	-	`sha256:47f23bc347431204e7ad21b644e0af7503d5cd75f67d419fc242196a22de558b`  
		Last Modified: Fri, 14 Feb 2020 17:54:18 GMT  
		Size: 11.8 MB (11835761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d7cd959e4aa4e0135cfe00216a86021f2b99992180c269df4cba54f8e227476`  
		Last Modified: Fri, 14 Feb 2020 17:54:14 GMT  
		Size: 7.2 KB (7161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6abc2d0fcb791eb9d7745ffe32554141f1aaf404be1b801d3f746ba02e84484`  
		Last Modified: Fri, 14 Feb 2020 17:54:14 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5217c1d54cfee7f87832ffd24811c5dedd9d8e27f40a22d83d1eb6484f03381`  
		Last Modified: Fri, 14 Feb 2020 17:54:14 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5b75b6486bad0db2700bf16448f498e6c14793b7618b50cde10ffd09abe8bf3`  
		Last Modified: Fri, 14 Feb 2020 17:54:14 GMT  
		Size: 4.2 KB (4180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ed495d36332764b7e77a72b4a70094fef25bd2a51836e80c2796b68baab472b`  
		Last Modified: Fri, 14 Feb 2020 17:54:14 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:9-alpine` - linux; arm variant v6

```console
$ docker pull postgres@sha256:12c8d1c0034c9e78a5368c979bb9e98b09bd8f918a246fe3a4e172510b3f40a4
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.0 MB (14044057 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:596a3e2788cbe97a017294cdf97a5ab938be0b571530cc43fdc67e7adb66ffb7`
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
# Fri, 21 Feb 2020 01:00:11 GMT
ENV PG_MAJOR=9.6
# Fri, 21 Feb 2020 01:00:15 GMT
ENV PG_VERSION=9.6.17
# Fri, 21 Feb 2020 01:00:16 GMT
ENV PG_SHA256=f6e1e32d32545f97c066f3c19f4d58dfab1205c01252cf85c5c92294ace1a0c2
# Fri, 21 Feb 2020 01:03:23 GMT
RUN set -ex 		&& apk add --no-cache --virtual .fetch-deps 		ca-certificates 		openssl 		tar 		&& wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2" 	&& echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c - 	&& mkdir -p /usr/src/postgresql 	&& tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	&& rm postgresql.tar.bz2 		&& apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		&& cd /usr/src/postgresql 	&& awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new 	&& grep '/var/run/postgresql' src/include/pg_config_manual.h.new 	&& mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& ./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 	&& make -j "$(nproc)" world 	&& make install-world 	&& make -C contrib install 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	&& apk del .fetch-deps .build-deps 	&& cd / 	&& rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	&& find /usr/local -name '*.a' -delete
# Fri, 21 Feb 2020 01:03:26 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Fri, 21 Feb 2020 01:03:28 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 21 Feb 2020 01:03:28 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 21 Feb 2020 01:03:30 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 21 Feb 2020 01:03:31 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 21 Feb 2020 01:03:32 GMT
COPY file:903758287828b43a3d11c897391be0dabdd9c333d7812ff67698fddb1fe8b8b1 in /usr/local/bin/ 
# Fri, 21 Feb 2020 01:03:37 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 21 Feb 2020 01:03:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 21 Feb 2020 01:03:39 GMT
EXPOSE 5432
# Fri, 21 Feb 2020 01:03:39 GMT
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
	-	`sha256:11e4854e5b9eb9bfc601e0b031b07bc3366b51645aef1fc136168868348e44e5`  
		Last Modified: Fri, 21 Feb 2020 01:08:55 GMT  
		Size: 11.4 MB (11413216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b84930f6996f752ada4cc4807ce89b18143b69a7fec4ae81475998e55617a22`  
		Last Modified: Fri, 21 Feb 2020 01:08:47 GMT  
		Size: 7.2 KB (7161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:419bf1b67ce5f8eb3062b01d3b541176a25c3c80f71b4c69fc0376ff4760bd5c`  
		Last Modified: Fri, 21 Feb 2020 01:08:47 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b73ea1cf5fd6774b79f6e39604f72ffd393a60f7e59ddb9c6badd90f2b55147`  
		Last Modified: Fri, 21 Feb 2020 01:08:47 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d33237cc3c5fc852b0de45b8c71df6eb09f38d885cc795380e23965896808ce`  
		Last Modified: Fri, 21 Feb 2020 01:08:47 GMT  
		Size: 4.2 KB (4215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:290f4b28fd7c373bd158f8c358cba93f6da7cc814e10baf782325767c719093c`  
		Last Modified: Fri, 21 Feb 2020 01:08:47 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:9-alpine` - linux; arm variant v7

```console
$ docker pull postgres@sha256:c46eb1e0553c0744cf22b99ccb84111631db9f36d02489333e9cc3e90bc1509e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.2 MB (13210842 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b0f15904c76fef208f493dbb83cecc6eb8daf42972ce6e90cf1a2c7640f5d5a`
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
# Thu, 30 Jan 2020 03:10:24 GMT
ENV PG_MAJOR=9.6
# Fri, 14 Feb 2020 18:28:39 GMT
ENV PG_VERSION=9.6.17
# Fri, 14 Feb 2020 18:28:40 GMT
ENV PG_SHA256=f6e1e32d32545f97c066f3c19f4d58dfab1205c01252cf85c5c92294ace1a0c2
# Fri, 14 Feb 2020 18:30:50 GMT
RUN set -ex 		&& apk add --no-cache --virtual .fetch-deps 		ca-certificates 		openssl 		tar 		&& wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2" 	&& echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c - 	&& mkdir -p /usr/src/postgresql 	&& tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	&& rm postgresql.tar.bz2 		&& apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		&& cd /usr/src/postgresql 	&& awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new 	&& grep '/var/run/postgresql' src/include/pg_config_manual.h.new 	&& mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& ./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 	&& make -j "$(nproc)" world 	&& make install-world 	&& make -C contrib install 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	&& apk del .fetch-deps .build-deps 	&& cd / 	&& rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	&& find /usr/local -name '*.a' -delete
# Fri, 14 Feb 2020 18:31:00 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Fri, 14 Feb 2020 18:31:05 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 14 Feb 2020 18:31:07 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 14 Feb 2020 18:31:09 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 14 Feb 2020 18:31:10 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 14 Feb 2020 18:31:11 GMT
COPY file:dfac98688c352f175c627102a0e4369c11bf8cbed107e8d5861aac37a67fd519 in /usr/local/bin/ 
# Fri, 14 Feb 2020 18:31:13 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 14 Feb 2020 18:31:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 14 Feb 2020 18:31:15 GMT
EXPOSE 5432
# Fri, 14 Feb 2020 18:31:15 GMT
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
	-	`sha256:b3b3eac7ea05c5396f66bdd48b2af7c9748638c608f5695e6b116a7ae7272e4e`  
		Last Modified: Fri, 14 Feb 2020 19:14:46 GMT  
		Size: 10.8 MB (10778046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d64946e01a7354a1266ffdd0d37210d8d5e3d687fba0397e1973ef71c781edf3`  
		Last Modified: Fri, 14 Feb 2020 19:14:40 GMT  
		Size: 7.2 KB (7158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d844ecb6927feebd46d4dae4d86f9ef88906d9b979eb1ac738c1a95df09e654`  
		Last Modified: Fri, 14 Feb 2020 19:14:40 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c3800d216860c04cbb03924ce47abf81a9270ad4323645b920001f9c565da02`  
		Last Modified: Fri, 14 Feb 2020 19:14:40 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f009f42fd112610ed90b09d89fb7be86bce281e0abd9ddeba291993a9bde622`  
		Last Modified: Fri, 14 Feb 2020 19:14:40 GMT  
		Size: 4.2 KB (4184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43521f903112f8e4d80bc2285b8387d11e57225797b3ee9abb06222d8554fdc7`  
		Last Modified: Fri, 14 Feb 2020 19:14:41 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:9-alpine` - linux; arm64 variant v8

```console
$ docker pull postgres@sha256:4a6c34d73307ef5823391408d7fb82c73d61cba703cb24deea8eaddfc6c37a08
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.4 MB (14415333 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3fd28811a8bbc65606a9dce014c9a216cf843da00f9f190f6a5297d77505e5a7`
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
# Thu, 30 Jan 2020 02:50:49 GMT
ENV PG_MAJOR=9.6
# Fri, 14 Feb 2020 19:14:38 GMT
ENV PG_VERSION=9.6.17
# Fri, 14 Feb 2020 19:14:38 GMT
ENV PG_SHA256=f6e1e32d32545f97c066f3c19f4d58dfab1205c01252cf85c5c92294ace1a0c2
# Fri, 14 Feb 2020 19:16:58 GMT
RUN set -ex 		&& apk add --no-cache --virtual .fetch-deps 		ca-certificates 		openssl 		tar 		&& wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2" 	&& echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c - 	&& mkdir -p /usr/src/postgresql 	&& tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	&& rm postgresql.tar.bz2 		&& apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		&& cd /usr/src/postgresql 	&& awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new 	&& grep '/var/run/postgresql' src/include/pg_config_manual.h.new 	&& mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& ./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 	&& make -j "$(nproc)" world 	&& make install-world 	&& make -C contrib install 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	&& apk del .fetch-deps .build-deps 	&& cd / 	&& rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	&& find /usr/local -name '*.a' -delete
# Fri, 14 Feb 2020 19:17:02 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Fri, 14 Feb 2020 19:17:04 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 14 Feb 2020 19:17:04 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 14 Feb 2020 19:17:06 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 14 Feb 2020 19:17:07 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 14 Feb 2020 19:17:08 GMT
COPY file:dfac98688c352f175c627102a0e4369c11bf8cbed107e8d5861aac37a67fd519 in /usr/local/bin/ 
# Fri, 14 Feb 2020 19:17:10 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 14 Feb 2020 19:17:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 14 Feb 2020 19:17:11 GMT
EXPOSE 5432
# Fri, 14 Feb 2020 19:17:12 GMT
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
	-	`sha256:6130959c2e1552544c6b329a834e1afd585ee393f7b1b648543be04594e48637`  
		Last Modified: Fri, 14 Feb 2020 20:00:05 GMT  
		Size: 11.7 MB (11679020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03c19fdc70b94fa0df9ae82423b6f5e26c60ee140d36f2c18dfdd64dd043de67`  
		Last Modified: Fri, 14 Feb 2020 20:00:00 GMT  
		Size: 7.2 KB (7158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a54a6021b037c8f1e51fa33db72cc36c2140d18883c1f6f18be43ccb249ed48`  
		Last Modified: Fri, 14 Feb 2020 19:59:59 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab785fc22f91ebb888a2006f17023d98cab2ca69652ad96ec65d23db2a9d136b`  
		Last Modified: Fri, 14 Feb 2020 20:00:00 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa2593a3bde1c5807e10e88c76d2a1d39492042e37166f407e5d9bd28de2cf77`  
		Last Modified: Fri, 14 Feb 2020 20:00:00 GMT  
		Size: 4.2 KB (4183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff3d05e9a538c9dcfadeb0ed5fb11bcde8bfb3df02070641a07e18b9ff2b248a`  
		Last Modified: Fri, 14 Feb 2020 20:00:00 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:9-alpine` - linux; 386

```console
$ docker pull postgres@sha256:c48c87e19b1c9bdc9d1de8a0f53fa1c7f91f887ecc06d0c2efd3f3425090b6c0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.3 MB (15277710 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:534f8f1da62596abc82568d0568f339401b8f74bc8198855a300c27d507adc6c`
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
# Thu, 30 Jan 2020 02:56:13 GMT
ENV PG_MAJOR=9.6
# Fri, 14 Feb 2020 18:03:52 GMT
ENV PG_VERSION=9.6.17
# Fri, 14 Feb 2020 18:03:52 GMT
ENV PG_SHA256=f6e1e32d32545f97c066f3c19f4d58dfab1205c01252cf85c5c92294ace1a0c2
# Fri, 14 Feb 2020 18:07:24 GMT
RUN set -ex 		&& apk add --no-cache --virtual .fetch-deps 		ca-certificates 		openssl 		tar 		&& wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2" 	&& echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c - 	&& mkdir -p /usr/src/postgresql 	&& tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	&& rm postgresql.tar.bz2 		&& apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		&& cd /usr/src/postgresql 	&& awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new 	&& grep '/var/run/postgresql' src/include/pg_config_manual.h.new 	&& mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& ./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 	&& make -j "$(nproc)" world 	&& make install-world 	&& make -C contrib install 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	&& apk del .fetch-deps .build-deps 	&& cd / 	&& rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	&& find /usr/local -name '*.a' -delete
# Fri, 14 Feb 2020 18:07:25 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Fri, 14 Feb 2020 18:07:26 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 14 Feb 2020 18:07:26 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 14 Feb 2020 18:07:27 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 14 Feb 2020 18:07:27 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 14 Feb 2020 18:07:27 GMT
COPY file:dfac98688c352f175c627102a0e4369c11bf8cbed107e8d5861aac37a67fd519 in /usr/local/bin/ 
# Fri, 14 Feb 2020 18:07:28 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 14 Feb 2020 18:07:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 14 Feb 2020 18:07:28 GMT
EXPOSE 5432
# Fri, 14 Feb 2020 18:07:29 GMT
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
	-	`sha256:240d0230ad0bab841840ccb2509f358cf6961476dfd79ef0ddb6dd4f46652d93`  
		Last Modified: Fri, 14 Feb 2020 18:18:45 GMT  
		Size: 12.5 MB (12458038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:226172319d6d76e29368546bcbcba9f56b25228aa1d314f54820ee9a3ae280a0`  
		Last Modified: Fri, 14 Feb 2020 18:18:41 GMT  
		Size: 7.2 KB (7159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df1b1148c571227b450dad6a3cdb947968178c44bbb072b0530d3e8c98dbd306`  
		Last Modified: Fri, 14 Feb 2020 18:18:41 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b43ff1304aba5aa74b9c4d42d36acd282c4f45d8de7580c82eb12d7f8e070919`  
		Last Modified: Fri, 14 Feb 2020 18:18:41 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b305d96510bd5de5b62a7530e3bf1b5c070181a42f0434a586ac624a5303a495`  
		Last Modified: Fri, 14 Feb 2020 18:18:41 GMT  
		Size: 4.2 KB (4181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa822d5e7b3cf37d3bf8be37cf33f1c70dbffd721a6a375d91abd817e4ecc197`  
		Last Modified: Fri, 14 Feb 2020 18:18:41 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:9-alpine` - linux; ppc64le

```console
$ docker pull postgres@sha256:e7030cf16aa0382de657b6aa6691f1d4e0ba364e96f9e72ec5785c7b5d7a843f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.6 MB (15561832 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7d1ff13a689a8c92c1d761a85519b2d96ffae46883dfd65266e8f98d5a2dea90`
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
# Thu, 30 Jan 2020 03:40:19 GMT
ENV PG_MAJOR=9.6
# Fri, 14 Feb 2020 17:49:11 GMT
ENV PG_VERSION=9.6.17
# Fri, 14 Feb 2020 17:49:14 GMT
ENV PG_SHA256=f6e1e32d32545f97c066f3c19f4d58dfab1205c01252cf85c5c92294ace1a0c2
# Fri, 14 Feb 2020 17:52:17 GMT
RUN set -ex 		&& apk add --no-cache --virtual .fetch-deps 		ca-certificates 		openssl 		tar 		&& wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2" 	&& echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c - 	&& mkdir -p /usr/src/postgresql 	&& tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	&& rm postgresql.tar.bz2 		&& apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		&& cd /usr/src/postgresql 	&& awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new 	&& grep '/var/run/postgresql' src/include/pg_config_manual.h.new 	&& mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& ./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 	&& make -j "$(nproc)" world 	&& make install-world 	&& make -C contrib install 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	&& apk del .fetch-deps .build-deps 	&& cd / 	&& rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	&& find /usr/local -name '*.a' -delete
# Fri, 14 Feb 2020 17:52:24 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Fri, 14 Feb 2020 17:52:31 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 14 Feb 2020 17:52:35 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 14 Feb 2020 17:52:44 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 14 Feb 2020 17:52:46 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 14 Feb 2020 17:52:47 GMT
COPY file:dfac98688c352f175c627102a0e4369c11bf8cbed107e8d5861aac37a67fd519 in /usr/local/bin/ 
# Fri, 14 Feb 2020 17:52:51 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 14 Feb 2020 17:52:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 14 Feb 2020 17:52:58 GMT
EXPOSE 5432
# Fri, 14 Feb 2020 17:53:01 GMT
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
	-	`sha256:0808bb27f8645a3926f2e3dac8c4e3ee0bb2a0cc52e9996ea3e5f0059dfaaa0a`  
		Last Modified: Fri, 14 Feb 2020 18:14:13 GMT  
		Size: 12.7 MB (12726465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1ba53891d7368c9480c2afce812cb83425ed70d9bbb5c48b4007c69bccdbf2a`  
		Last Modified: Fri, 14 Feb 2020 18:14:06 GMT  
		Size: 7.2 KB (7159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:334835b098489afd2dbabb95e0bea2c5536ce02be3ffe1bacaa2e2f2b5e5d8fa`  
		Last Modified: Fri, 14 Feb 2020 18:14:06 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcef79167649d2cbed5769025b2df9a0679c51f8a01c7887b342b115924878dd`  
		Last Modified: Fri, 14 Feb 2020 18:14:06 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32c7ed0e45f284729b3e1c6bbd8127853cba1f0e8c81dfff1110febb0be2240a`  
		Last Modified: Fri, 14 Feb 2020 18:14:06 GMT  
		Size: 4.2 KB (4183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce80da0b09daafe8757e7f2803382fba6a0692a943126fcc43fe8e680a4e6390`  
		Last Modified: Fri, 14 Feb 2020 18:14:06 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:9-alpine` - linux; s390x

```console
$ docker pull postgres@sha256:886c31aebfe6a9338b018b22e1c8a16dafd49edde839bf1369c0d43f3ada1cd4
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.2 MB (14249779 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e8e98444554f58a2976872f6cdbdfa3865339e4ad6f151362d96bc187b57448`
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
# Fri, 21 Feb 2020 01:08:01 GMT
ENV PG_MAJOR=9.6
# Fri, 21 Feb 2020 01:08:01 GMT
ENV PG_VERSION=9.6.17
# Fri, 21 Feb 2020 01:08:01 GMT
ENV PG_SHA256=f6e1e32d32545f97c066f3c19f4d58dfab1205c01252cf85c5c92294ace1a0c2
# Fri, 21 Feb 2020 01:12:07 GMT
RUN set -ex 		&& apk add --no-cache --virtual .fetch-deps 		ca-certificates 		openssl 		tar 		&& wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2" 	&& echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c - 	&& mkdir -p /usr/src/postgresql 	&& tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	&& rm postgresql.tar.bz2 		&& apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		&& cd /usr/src/postgresql 	&& awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new 	&& grep '/var/run/postgresql' src/include/pg_config_manual.h.new 	&& mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& ./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 	&& make -j "$(nproc)" world 	&& make install-world 	&& make -C contrib install 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	&& apk del .fetch-deps .build-deps 	&& cd / 	&& rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	&& find /usr/local -name '*.a' -delete
# Fri, 21 Feb 2020 01:12:10 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Fri, 21 Feb 2020 01:12:11 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 21 Feb 2020 01:12:12 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 21 Feb 2020 01:12:13 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 21 Feb 2020 01:12:13 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 21 Feb 2020 01:12:13 GMT
COPY file:903758287828b43a3d11c897391be0dabdd9c333d7812ff67698fddb1fe8b8b1 in /usr/local/bin/ 
# Fri, 21 Feb 2020 01:12:15 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 21 Feb 2020 01:12:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 21 Feb 2020 01:12:16 GMT
EXPOSE 5432
# Fri, 21 Feb 2020 01:12:16 GMT
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
	-	`sha256:3534d410bf53a06cece86891ef5c86d5a4912da510767eea19b9f506c0c99902`  
		Last Modified: Fri, 21 Feb 2020 01:30:19 GMT  
		Size: 11.7 MB (11654466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:859994308f416b51c93fac0882465d66bebb5a835bd397397a516094437fcb10`  
		Last Modified: Fri, 21 Feb 2020 01:30:15 GMT  
		Size: 7.2 KB (7158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9541da379ddb64ea931ed2fb517aea1f4372adecb37e08a29a599740b99a2a29`  
		Last Modified: Fri, 21 Feb 2020 01:30:15 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5f548599fb2b1e8796226a71f4b71d5426dfb07ac1d11925c88dcccda876927`  
		Last Modified: Fri, 21 Feb 2020 01:30:16 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce5a82faaa80b5b85b6143c2844ce7a75faed6a540526e9680cf94e9837f2bf7`  
		Last Modified: Fri, 21 Feb 2020 01:30:21 GMT  
		Size: 4.2 KB (4219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2714ca9831616e476f24835681b36fa6663660a516ab97b43bfd2fb8936a06a2`  
		Last Modified: Fri, 21 Feb 2020 01:30:21 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
