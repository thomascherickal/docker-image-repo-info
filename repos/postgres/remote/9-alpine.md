## `postgres:9-alpine`

```console
$ docker pull postgres@sha256:d82fb8a5f9ae2eb536400e69d4189270dabd987740894fd3949cc7f17e0bd621
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
$ docker pull postgres@sha256:464302478f968dce124eb9b90bab2e30d4ec366862d1bbd5f5406f250f18b7af
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.5 MB (14540913 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b92e85d5d39e614045d5567c87d90f269a098acfe3e79544c300027db73ff63`
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
# Thu, 23 Jan 2020 21:54:51 GMT
ENV PG_MAJOR=9.6
# Thu, 23 Jan 2020 21:54:51 GMT
ENV PG_VERSION=9.6.16
# Thu, 23 Jan 2020 21:54:52 GMT
ENV PG_SHA256=5c6cba9cc0df70ba2b128c4a87d0babfce7c0e2b888f70a9c8485745f66b22e7
# Thu, 23 Jan 2020 22:00:06 GMT
RUN set -ex 		&& apk add --no-cache --virtual .fetch-deps 		ca-certificates 		openssl 		tar 		&& wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2" 	&& echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c - 	&& mkdir -p /usr/src/postgresql 	&& tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	&& rm postgresql.tar.bz2 		&& apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		&& cd /usr/src/postgresql 	&& awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new 	&& grep '/var/run/postgresql' src/include/pg_config_manual.h.new 	&& mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& ./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 	&& make -j "$(nproc)" world 	&& make install-world 	&& make -C contrib install 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	&& apk del .fetch-deps .build-deps 	&& cd / 	&& rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	&& find /usr/local -name '*.a' -delete
# Thu, 23 Jan 2020 22:00:08 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Thu, 23 Jan 2020 22:00:09 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 23 Jan 2020 22:00:10 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 23 Jan 2020 22:00:11 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 23 Jan 2020 22:00:12 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 23 Jan 2020 22:00:12 GMT
COPY file:abc85c5ac9d748ac5df3a643ab618de050dd65e8ef159dbdcdfe1a720ab1142b in /usr/local/bin/ 
# Thu, 23 Jan 2020 22:00:13 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 23 Jan 2020 22:00:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jan 2020 22:00:14 GMT
EXPOSE 5432
# Thu, 23 Jan 2020 22:00:14 GMT
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
	-	`sha256:b4184112eeaed710046a2e989201470736c67ec16c93dc0f99537bd597681a7f`  
		Last Modified: Thu, 23 Jan 2020 22:13:05 GMT  
		Size: 11.7 MB (11742283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50634a031f773da9bfa0c61252937b35b8bd2d3a1e3a808a8e06521d919f6b9e`  
		Last Modified: Thu, 23 Jan 2020 22:13:02 GMT  
		Size: 7.2 KB (7155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf5601d968e8d777416a9fe0041dedd8c63bc2de312a931e577981711f31047f`  
		Last Modified: Thu, 23 Jan 2020 22:13:02 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eaa021b2bedb7ef9bb8e5ed5d9aafce27910458735e94237777a0c74d49c70c`  
		Last Modified: Thu, 23 Jan 2020 22:13:02 GMT  
		Size: 164.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2135b1524d0cd2a9fedd09f53b11a1cf8db550e327a6bc34242588368dc0fa8f`  
		Last Modified: Thu, 23 Jan 2020 22:13:02 GMT  
		Size: 3.8 KB (3838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bf70c06d10bb97e80fa905852eb01e1aa30154d5474c0ec158d3c9de3b41952`  
		Last Modified: Thu, 23 Jan 2020 22:13:02 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:9-alpine` - linux; arm variant v6

```console
$ docker pull postgres@sha256:15b2ea2fe5f8324562fde0a53c571c9a3df36faa710098ac1159bf3549408720
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.9 MB (13875284 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ffc3036107a43db0489ae8c98f086ac612080c5639192e283fe257d00402d1e1`
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
# Thu, 23 Jan 2020 20:02:53 GMT
ENV PG_MAJOR=9.6
# Thu, 23 Jan 2020 20:02:54 GMT
ENV PG_VERSION=9.6.16
# Thu, 23 Jan 2020 20:02:55 GMT
ENV PG_SHA256=5c6cba9cc0df70ba2b128c4a87d0babfce7c0e2b888f70a9c8485745f66b22e7
# Thu, 23 Jan 2020 20:04:44 GMT
RUN set -ex 		&& apk add --no-cache --virtual .fetch-deps 		ca-certificates 		openssl 		tar 		&& wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2" 	&& echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c - 	&& mkdir -p /usr/src/postgresql 	&& tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	&& rm postgresql.tar.bz2 		&& apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		&& cd /usr/src/postgresql 	&& awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new 	&& grep '/var/run/postgresql' src/include/pg_config_manual.h.new 	&& mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& ./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 	&& make -j "$(nproc)" world 	&& make install-world 	&& make -C contrib install 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	&& apk del .fetch-deps .build-deps 	&& cd / 	&& rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	&& find /usr/local -name '*.a' -delete
# Thu, 23 Jan 2020 20:04:46 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Thu, 23 Jan 2020 20:04:48 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 23 Jan 2020 20:04:48 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 23 Jan 2020 20:04:50 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 23 Jan 2020 20:04:52 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 23 Jan 2020 20:04:53 GMT
COPY file:abc85c5ac9d748ac5df3a643ab618de050dd65e8ef159dbdcdfe1a720ab1142b in /usr/local/bin/ 
# Thu, 23 Jan 2020 20:04:57 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 23 Jan 2020 20:04:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jan 2020 20:04:59 GMT
EXPOSE 5432
# Thu, 23 Jan 2020 20:04:59 GMT
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
	-	`sha256:a982841b2c23706a76b4db2233d841901f1cf7e0323e8fbfd5a32c7f18234d38`  
		Last Modified: Thu, 23 Jan 2020 20:11:31 GMT  
		Size: 11.3 MB (11292078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb8c8eef8a0e219b5fb7537b7606602b0b29a07c7f80c1155b90e8774459d9fc`  
		Last Modified: Thu, 23 Jan 2020 20:11:26 GMT  
		Size: 7.2 KB (7161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e171f42d14fd3ed7ae50d44e718985517e2e6f72cc0d862908878a5101812146`  
		Last Modified: Thu, 23 Jan 2020 20:11:25 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62944870c4536f15ef66ea7cc98239f2867780a869636218a722405c4b858e21`  
		Last Modified: Thu, 23 Jan 2020 20:11:25 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d4b12cb135f04548c0d8898279ca2b82b18d4a222bb557206ec261b98ef5931`  
		Last Modified: Thu, 23 Jan 2020 20:11:25 GMT  
		Size: 3.8 KB (3832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8ea611cfe6ebd24f6b41648825b1cf70a3fc53868344a071f358e3a05059a74`  
		Last Modified: Thu, 23 Jan 2020 20:11:25 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:9-alpine` - linux; arm variant v7

```console
$ docker pull postgres@sha256:6f4558fdf64708f674fc55bee73b9ae2cee6f987509fc71662441f8d9a101a26
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.0 MB (13044671 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:32f5475ea67e09ce58d71cdb56e7ded48160f63767d999782444efe249900513`
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
# Thu, 23 Jan 2020 17:45:23 GMT
ENV PG_MAJOR=9.6
# Thu, 23 Jan 2020 17:45:24 GMT
ENV PG_VERSION=9.6.16
# Thu, 23 Jan 2020 17:45:24 GMT
ENV PG_SHA256=5c6cba9cc0df70ba2b128c4a87d0babfce7c0e2b888f70a9c8485745f66b22e7
# Thu, 23 Jan 2020 17:47:12 GMT
RUN set -ex 		&& apk add --no-cache --virtual .fetch-deps 		ca-certificates 		openssl 		tar 		&& wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2" 	&& echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c - 	&& mkdir -p /usr/src/postgresql 	&& tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	&& rm postgresql.tar.bz2 		&& apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		&& cd /usr/src/postgresql 	&& awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new 	&& grep '/var/run/postgresql' src/include/pg_config_manual.h.new 	&& mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& ./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 	&& make -j "$(nproc)" world 	&& make install-world 	&& make -C contrib install 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	&& apk del .fetch-deps .build-deps 	&& cd / 	&& rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	&& find /usr/local -name '*.a' -delete
# Thu, 23 Jan 2020 17:47:15 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Thu, 23 Jan 2020 17:47:18 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 23 Jan 2020 17:47:19 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 23 Jan 2020 17:47:21 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 23 Jan 2020 17:47:22 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 23 Jan 2020 17:47:23 GMT
COPY file:abc85c5ac9d748ac5df3a643ab618de050dd65e8ef159dbdcdfe1a720ab1142b in /usr/local/bin/ 
# Thu, 23 Jan 2020 17:47:26 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 23 Jan 2020 17:47:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jan 2020 17:47:27 GMT
EXPOSE 5432
# Thu, 23 Jan 2020 17:47:28 GMT
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
	-	`sha256:2d9e91717c5aa9cebee2d9d09aca868765ade6c2935191054a857bb642f02b39`  
		Last Modified: Thu, 23 Jan 2020 17:54:36 GMT  
		Size: 10.7 MB (10654465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdc2990c07650915523b740942674412b7e943f4d2a142f0d6a6abd2ed206851`  
		Last Modified: Thu, 23 Jan 2020 17:54:30 GMT  
		Size: 7.2 KB (7158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:119b174bcb97f926a662381ce5202c0bd442cf1ab45251551c20c288fa70538a`  
		Last Modified: Thu, 23 Jan 2020 17:54:31 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:436f93ef78e4e37dc4594d8d1858e1e62cf91e290662f57e1410289314af6a98`  
		Last Modified: Thu, 23 Jan 2020 17:54:30 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb6208e1bf50dff6201f1acdca8cf1460b44c1f19003e30d8aaf724e4a5b9e0b`  
		Last Modified: Thu, 23 Jan 2020 17:54:30 GMT  
		Size: 3.8 KB (3837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d90764e321327bdfac99e27d847329505fecfbabec1f29b6d7465f6f0d48ae55`  
		Last Modified: Thu, 23 Jan 2020 17:54:30 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:9-alpine` - linux; arm64 variant v8

```console
$ docker pull postgres@sha256:d75e784de93d9628f15604c1d71d5983386ac2e967fdebb2b934e7dd7b0cff47
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.4 MB (14379284 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e2ab6e2513145d9eb2217e22ae8e9fa8e29baf17edb5047277db756c73c5f6cf`
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
# Thu, 23 Jan 2020 20:47:42 GMT
ENV PG_MAJOR=9.6
# Thu, 23 Jan 2020 20:47:42 GMT
ENV PG_VERSION=9.6.16
# Thu, 23 Jan 2020 20:47:43 GMT
ENV PG_SHA256=5c6cba9cc0df70ba2b128c4a87d0babfce7c0e2b888f70a9c8485745f66b22e7
# Thu, 23 Jan 2020 20:49:58 GMT
RUN set -ex 		&& apk add --no-cache --virtual .fetch-deps 		ca-certificates 		openssl 		tar 		&& wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2" 	&& echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c - 	&& mkdir -p /usr/src/postgresql 	&& tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	&& rm postgresql.tar.bz2 		&& apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		&& cd /usr/src/postgresql 	&& awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new 	&& grep '/var/run/postgresql' src/include/pg_config_manual.h.new 	&& mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& ./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 	&& make -j "$(nproc)" world 	&& make install-world 	&& make -C contrib install 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	&& apk del .fetch-deps .build-deps 	&& cd / 	&& rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	&& find /usr/local -name '*.a' -delete
# Thu, 23 Jan 2020 20:50:00 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Thu, 23 Jan 2020 20:50:02 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 23 Jan 2020 20:50:03 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 23 Jan 2020 20:50:05 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 23 Jan 2020 20:50:06 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 23 Jan 2020 20:50:06 GMT
COPY file:abc85c5ac9d748ac5df3a643ab618de050dd65e8ef159dbdcdfe1a720ab1142b in /usr/local/bin/ 
# Thu, 23 Jan 2020 20:50:08 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 23 Jan 2020 20:50:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jan 2020 20:50:10 GMT
EXPOSE 5432
# Thu, 23 Jan 2020 20:50:11 GMT
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
	-	`sha256:61553b6f0ebd16ed34bd1c8fe4441d4cf019acbe38961b669b683cc219d248c8`  
		Last Modified: Thu, 23 Jan 2020 20:58:59 GMT  
		Size: 11.6 MB (11649753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:347d8c87c3a9792aadbaeed41f5168e54544a935da71b6d41aac02c5ef5b6006`  
		Last Modified: Thu, 23 Jan 2020 20:58:36 GMT  
		Size: 7.2 KB (7156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:945ce60ac21ad699d7489930d6e8fac081576b45e432c242013063b71aebca7e`  
		Last Modified: Thu, 23 Jan 2020 20:58:37 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3727c6eab6f04d0dc0dd2a64f4aa1c1769577f7bc6e4e8bcd2b79c15c9e5b867`  
		Last Modified: Thu, 23 Jan 2020 20:58:36 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2de4b675eadee3b87d479ec9cf40f92c4be07435f8278fb358072c724828379d`  
		Last Modified: Thu, 23 Jan 2020 20:58:36 GMT  
		Size: 3.8 KB (3839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13d85cbfde3f0de04667f001f4f26ce991ca6cdf536ab23eb6829a1fb0751ddd`  
		Last Modified: Thu, 23 Jan 2020 20:58:36 GMT  
		Size: 118.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:9-alpine` - linux; 386

```console
$ docker pull postgres@sha256:3562f732d4a1dbe8a7fc5d0f7f25b2a20442e1ebed019667a0045acfd3577ce6
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.1 MB (15128039 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df77ec21042c7ef42612a3c0fbb8a8dc3813deaf4d15107c6cbd1fa41dd389d1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 23 Jan 2020 16:52:57 GMT
ADD file:8c429ecc11f3cadcecc39922ce15df6b51a649929959b331fed8d1f42d722474 in / 
# Thu, 23 Jan 2020 16:52:57 GMT
CMD ["/bin/sh"]
# Fri, 24 Jan 2020 04:06:09 GMT
RUN set -ex; 	postgresHome="$(getent passwd postgres)"; 	postgresHome="$(echo "$postgresHome" | cut -d: -f6)"; 	[ "$postgresHome" = '/var/lib/postgresql' ]; 	mkdir -p "$postgresHome"; 	chown -R postgres:postgres "$postgresHome"
# Fri, 24 Jan 2020 04:06:09 GMT
ENV LANG=en_US.utf8
# Fri, 24 Jan 2020 04:06:10 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 24 Jan 2020 04:21:22 GMT
ENV PG_MAJOR=9.6
# Fri, 24 Jan 2020 04:21:22 GMT
ENV PG_VERSION=9.6.16
# Fri, 24 Jan 2020 04:21:22 GMT
ENV PG_SHA256=5c6cba9cc0df70ba2b128c4a87d0babfce7c0e2b888f70a9c8485745f66b22e7
# Fri, 24 Jan 2020 04:24:20 GMT
RUN set -ex 		&& apk add --no-cache --virtual .fetch-deps 		ca-certificates 		openssl 		tar 		&& wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2" 	&& echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c - 	&& mkdir -p /usr/src/postgresql 	&& tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	&& rm postgresql.tar.bz2 		&& apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		&& cd /usr/src/postgresql 	&& awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new 	&& grep '/var/run/postgresql' src/include/pg_config_manual.h.new 	&& mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& ./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 	&& make -j "$(nproc)" world 	&& make install-world 	&& make -C contrib install 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	&& apk del .fetch-deps .build-deps 	&& cd / 	&& rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	&& find /usr/local -name '*.a' -delete
# Fri, 24 Jan 2020 04:24:21 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Fri, 24 Jan 2020 04:24:22 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 24 Jan 2020 04:24:22 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 24 Jan 2020 04:24:23 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 24 Jan 2020 04:24:23 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 24 Jan 2020 04:24:23 GMT
COPY file:abc85c5ac9d748ac5df3a643ab618de050dd65e8ef159dbdcdfe1a720ab1142b in /usr/local/bin/ 
# Fri, 24 Jan 2020 04:24:24 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 24 Jan 2020 04:24:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Jan 2020 04:24:24 GMT
EXPOSE 5432
# Fri, 24 Jan 2020 04:24:24 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:8ad089020f8a1fd366fb13feb183e2f4c7410e2232c54b40f6a54fd56029fdf3`  
		Last Modified: Thu, 23 Jan 2020 16:53:22 GMT  
		Size: 2.8 MB (2785861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1b012d65d8f9e0e9c38ee5d9e6e45ce7ec254d0ef8e3072f783e94920a6eb46`  
		Last Modified: Fri, 24 Jan 2020 04:30:37 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf84274289b60a12540d26136a35cb800cebfac738337398c7e48b591435bbea`  
		Last Modified: Fri, 24 Jan 2020 04:30:37 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab6d15a030db0503472731d84552ba758f3cf65cba25e6a33129b21cad097b0d`  
		Last Modified: Fri, 24 Jan 2020 04:31:53 GMT  
		Size: 12.3 MB (12330509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e052a54dc1388ed140771b49327d2a828ba40cac57eeea0a607028634e4d6ef`  
		Last Modified: Fri, 24 Jan 2020 04:31:48 GMT  
		Size: 7.2 KB (7157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9858007c79d083816c07ec5aad23d8ffc67e2b62747f3e4033560ca7179b1073`  
		Last Modified: Fri, 24 Jan 2020 04:31:49 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3cf6b780f594ce5fc77a300ba8bc0325fb8a8b20737b3cc93882baf2c059c9b`  
		Last Modified: Fri, 24 Jan 2020 04:31:48 GMT  
		Size: 164.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7507e54b8b619ad2709c41c2e9e46a7b2c91f46a54ca431da80f75b47ce81b9`  
		Last Modified: Fri, 24 Jan 2020 04:31:48 GMT  
		Size: 3.8 KB (3836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb123a0740d122d4edcc5e47ae06a5ae8ffe53921dd05cb14662e3f3a49ce4ea`  
		Last Modified: Fri, 24 Jan 2020 04:31:49 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:9-alpine` - linux; ppc64le

```console
$ docker pull postgres@sha256:47f5639764221a4c215b474f35497e3cf32e9ab73eeeecc9911d2b7514dfe28e
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.6 MB (15644503 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:391ce19e4c14d474e844c91e511c3c5fe0ae89858a542095e47dd34d53f3571c`
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
# Thu, 23 Jan 2020 18:08:43 GMT
ENV PG_MAJOR=9.6
# Thu, 23 Jan 2020 18:08:46 GMT
ENV PG_VERSION=9.6.16
# Thu, 23 Jan 2020 18:08:49 GMT
ENV PG_SHA256=5c6cba9cc0df70ba2b128c4a87d0babfce7c0e2b888f70a9c8485745f66b22e7
# Thu, 23 Jan 2020 18:11:17 GMT
RUN set -ex 		&& apk add --no-cache --virtual .fetch-deps 		ca-certificates 		openssl 		tar 		&& wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2" 	&& echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c - 	&& mkdir -p /usr/src/postgresql 	&& tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	&& rm postgresql.tar.bz2 		&& apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		&& cd /usr/src/postgresql 	&& awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new 	&& grep '/var/run/postgresql' src/include/pg_config_manual.h.new 	&& mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& ./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 	&& make -j "$(nproc)" world 	&& make install-world 	&& make -C contrib install 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	&& apk del .fetch-deps .build-deps 	&& cd / 	&& rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	&& find /usr/local -name '*.a' -delete
# Thu, 23 Jan 2020 18:11:26 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Thu, 23 Jan 2020 18:11:32 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 23 Jan 2020 18:11:34 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 23 Jan 2020 18:11:38 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 23 Jan 2020 18:11:41 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 23 Jan 2020 18:11:42 GMT
COPY file:abc85c5ac9d748ac5df3a643ab618de050dd65e8ef159dbdcdfe1a720ab1142b in /usr/local/bin/ 
# Thu, 23 Jan 2020 18:11:50 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 23 Jan 2020 18:11:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jan 2020 18:11:59 GMT
EXPOSE 5432
# Thu, 23 Jan 2020 18:12:03 GMT
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
	-	`sha256:3ed39ae7a6a55f9a6408ce5a28bc205ce32a91899f8e621c58b1c2fdf4e3193b`  
		Last Modified: Thu, 23 Jan 2020 18:22:55 GMT  
		Size: 12.8 MB (12824168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc4696a59c7553776642388409e4c0d52f35dcb4beb9332f9b204d7e72ad87ff`  
		Last Modified: Thu, 23 Jan 2020 18:22:43 GMT  
		Size: 7.2 KB (7159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:870f8f9a2fcb47bcb66f47402db7a69d012ffdaff33befed4ab6677e290e4c9f`  
		Last Modified: Thu, 23 Jan 2020 18:22:43 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09b6a82d030f9a8c26e787c1295d33cbe29b20dd086e4c7a973ae4f66051c37e`  
		Last Modified: Thu, 23 Jan 2020 18:22:43 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2cfade0449989f341ba74c6571770874464fea11005829a2a572a8b79cf20ec`  
		Last Modified: Thu, 23 Jan 2020 18:22:43 GMT  
		Size: 3.8 KB (3839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc3f3dc428a97251938620ccee44723ab3e1317c49b4ef26ddabb58e9252fc36`  
		Last Modified: Thu, 23 Jan 2020 18:22:43 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:9-alpine` - linux; s390x

```console
$ docker pull postgres@sha256:3d21af897c55b818e1df0c01a05aae029fa03f5001dce30555dc30963f4cc7fb
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.2 MB (14188850 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7922fda853a012cd7d51518630bb510c121ad1f0590e3a16964a3e2bd42c7fe6`
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
# Thu, 23 Jan 2020 19:09:35 GMT
ENV PG_MAJOR=9.6
# Thu, 23 Jan 2020 19:09:35 GMT
ENV PG_VERSION=9.6.16
# Thu, 23 Jan 2020 19:09:35 GMT
ENV PG_SHA256=5c6cba9cc0df70ba2b128c4a87d0babfce7c0e2b888f70a9c8485745f66b22e7
# Thu, 23 Jan 2020 19:11:23 GMT
RUN set -ex 		&& apk add --no-cache --virtual .fetch-deps 		ca-certificates 		openssl 		tar 		&& wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2" 	&& echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c - 	&& mkdir -p /usr/src/postgresql 	&& tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	&& rm postgresql.tar.bz2 		&& apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		&& cd /usr/src/postgresql 	&& awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new 	&& grep '/var/run/postgresql' src/include/pg_config_manual.h.new 	&& mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& ./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 	&& make -j "$(nproc)" world 	&& make install-world 	&& make -C contrib install 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	&& apk del .fetch-deps .build-deps 	&& cd / 	&& rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	&& find /usr/local -name '*.a' -delete
# Thu, 23 Jan 2020 19:11:24 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Thu, 23 Jan 2020 19:11:24 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 23 Jan 2020 19:11:25 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 23 Jan 2020 19:11:25 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 23 Jan 2020 19:11:26 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 23 Jan 2020 19:11:26 GMT
COPY file:abc85c5ac9d748ac5df3a643ab618de050dd65e8ef159dbdcdfe1a720ab1142b in /usr/local/bin/ 
# Thu, 23 Jan 2020 19:11:26 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 23 Jan 2020 19:11:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jan 2020 19:11:27 GMT
EXPOSE 5432
# Thu, 23 Jan 2020 19:11:27 GMT
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
	-	`sha256:28b423d89f0e9b52819cfcfd5241174dc96637dee57c6188723096d5cbdb27ac`  
		Last Modified: Thu, 23 Jan 2020 19:18:01 GMT  
		Size: 11.6 MB (11603562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a742de784b7e580fe782dc1747c8cd9704670133522f56945a2a5ebb37b9f8e`  
		Last Modified: Thu, 23 Jan 2020 19:17:58 GMT  
		Size: 7.2 KB (7157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb2a97b4456d480e7206297c45e6980c288fa20a6036725b867a627d3f2d7ada`  
		Last Modified: Thu, 23 Jan 2020 19:17:58 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e634c823083bdfb4d255e11e2e7a31d223c1a42d9a8aa9af2116b23fe3d835f1`  
		Last Modified: Thu, 23 Jan 2020 19:17:58 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f66a50822914e2e29e063a0f31f804cf8bcbb903c023371eabd98e3d8b2af504`  
		Last Modified: Thu, 23 Jan 2020 19:17:58 GMT  
		Size: 3.8 KB (3836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24d6bae88d62f083f426db58768af268fe49ab1d716f4be394232eed12a431ea`  
		Last Modified: Thu, 23 Jan 2020 19:17:58 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
