## `postgres:10-alpine`

```console
$ docker pull postgres@sha256:affdbd0e93fd45dfdf694dc82b1ceb2c91a272765578b9acc3d3dfa84c35aa2c
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
$ docker pull postgres@sha256:6c8b332d1f0c266fe72fddc5170010adcb7bee90ff00182de0d9aa534590de1b
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.0 MB (28029677 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7e845e60ed355c5993b84b26821a3a5cc9bcce5595c64fe2695920cab82e0d7e`
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
# Thu, 23 Jan 2020 21:48:43 GMT
ENV PG_MAJOR=10
# Thu, 23 Jan 2020 21:48:43 GMT
ENV PG_VERSION=10.11
# Thu, 23 Jan 2020 21:48:44 GMT
ENV PG_SHA256=0d5d14ff6b075655f4421038fbde3a5d7b418c26a249a187a4175600d7aecc09
# Thu, 23 Jan 2020 21:54:29 GMT
RUN set -ex 		&& apk add --no-cache --virtual .fetch-deps 		ca-certificates 		openssl 		tar 		&& wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2" 	&& echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c - 	&& mkdir -p /usr/src/postgresql 	&& tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	&& rm postgresql.tar.bz2 		&& apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 		&& cd /usr/src/postgresql 	&& awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new 	&& grep '/var/run/postgresql' src/include/pg_config_manual.h.new 	&& mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& ./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 	&& make -j "$(nproc)" world 	&& make install-world 	&& make -C contrib install 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	&& apk del .fetch-deps .build-deps 	&& cd / 	&& rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	&& find /usr/local -name '*.a' -delete
# Thu, 23 Jan 2020 21:54:31 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Thu, 23 Jan 2020 21:54:32 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 23 Jan 2020 21:54:32 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 23 Jan 2020 21:54:34 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 23 Jan 2020 21:54:34 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 23 Jan 2020 21:54:34 GMT
COPY file:74700c51dbcbbad39fbd303750c2ac04ac10f59a73a55171e1fd0dbae6c2f311 in /usr/local/bin/ 
# Thu, 23 Jan 2020 21:54:36 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 23 Jan 2020 21:54:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jan 2020 21:54:36 GMT
EXPOSE 5432
# Thu, 23 Jan 2020 21:54:37 GMT
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
	-	`sha256:9306e42bb4e526adfffcbfe9398529215f0fb5f6872a933ef5c0e2de2dba317c`  
		Last Modified: Thu, 23 Jan 2020 22:12:57 GMT  
		Size: 25.2 MB (25230850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdc6ba040e582b331f6511768fd59795cadb2271861849bdf34521df5053bdad`  
		Last Modified: Thu, 23 Jan 2020 22:12:51 GMT  
		Size: 7.4 KB (7352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:211cc9467b5645768fc2f0c37f09c3336774bbda5ff875fc7420d7a9dc8aa58c`  
		Last Modified: Thu, 23 Jan 2020 22:12:51 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c2bbd8f95555fa085a139f34301e65d2cc6eb3b6a23e200047e95b281ab4842`  
		Last Modified: Thu, 23 Jan 2020 22:12:51 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03bd14ff27dd29258fed01f965bdbe2e2efa9728c3c40080809794144d211017`  
		Last Modified: Thu, 23 Jan 2020 22:12:51 GMT  
		Size: 3.8 KB (3838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fbf5e4e276b9c2beadadf3b9484b746f70d9fc106f05e82bde2717a3d5c5b5e`  
		Last Modified: Thu, 23 Jan 2020 22:12:51 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:10-alpine` - linux; arm variant v6

```console
$ docker pull postgres@sha256:314f23d21081ec89f73b9f64e8ea59e901a1d374cb1c383f1a16475d6a971b05
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.1 MB (27080764 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:51751a2c2a88a720237f99202729b5bdb28497e2d12a6aa9bb738b5fcb88c52f`
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
# Thu, 23 Jan 2020 20:00:21 GMT
ENV PG_MAJOR=10
# Thu, 23 Jan 2020 20:00:22 GMT
ENV PG_VERSION=10.11
# Thu, 23 Jan 2020 20:00:22 GMT
ENV PG_SHA256=0d5d14ff6b075655f4421038fbde3a5d7b418c26a249a187a4175600d7aecc09
# Thu, 23 Jan 2020 20:02:27 GMT
RUN set -ex 		&& apk add --no-cache --virtual .fetch-deps 		ca-certificates 		openssl 		tar 		&& wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2" 	&& echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c - 	&& mkdir -p /usr/src/postgresql 	&& tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	&& rm postgresql.tar.bz2 		&& apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 		&& cd /usr/src/postgresql 	&& awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new 	&& grep '/var/run/postgresql' src/include/pg_config_manual.h.new 	&& mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& ./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 	&& make -j "$(nproc)" world 	&& make install-world 	&& make -C contrib install 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	&& apk del .fetch-deps .build-deps 	&& cd / 	&& rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	&& find /usr/local -name '*.a' -delete
# Thu, 23 Jan 2020 20:02:31 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Thu, 23 Jan 2020 20:02:33 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 23 Jan 2020 20:02:33 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 23 Jan 2020 20:02:36 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 23 Jan 2020 20:02:37 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 23 Jan 2020 20:02:37 GMT
COPY file:74700c51dbcbbad39fbd303750c2ac04ac10f59a73a55171e1fd0dbae6c2f311 in /usr/local/bin/ 
# Thu, 23 Jan 2020 20:02:39 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 23 Jan 2020 20:02:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jan 2020 20:02:41 GMT
EXPOSE 5432
# Thu, 23 Jan 2020 20:02:42 GMT
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
	-	`sha256:11413c5459c3d4f55701422ab2ffc01bd7c09bf419aa26e234a916615de6c054`  
		Last Modified: Thu, 23 Jan 2020 20:11:19 GMT  
		Size: 24.5 MB (24497365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acd180f21d10bd05ae13917f579fea5a7981c1d73a7b8eb6cff74b4e2da7e988`  
		Last Modified: Thu, 23 Jan 2020 20:11:08 GMT  
		Size: 7.3 KB (7349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae2fe878e366634013548c0e541118157b4ce902424891727004b196f22ae185`  
		Last Modified: Thu, 23 Jan 2020 20:11:09 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eaf6325cda75f7a059414d6e317389bfcdb747bc84d7429df4b5d081bf759290`  
		Last Modified: Thu, 23 Jan 2020 20:11:09 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2af1a918ab430c9f5b67b5bb928dea18265f45772a8f758e8819ea01962a5b92`  
		Last Modified: Thu, 23 Jan 2020 20:11:09 GMT  
		Size: 3.8 KB (3838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d508e2484c9b5221973be2c3f00ebced9288efe14ceafed37fc4af08360e6b4`  
		Last Modified: Thu, 23 Jan 2020 20:11:09 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:10-alpine` - linux; arm variant v7

```console
$ docker pull postgres@sha256:f4e139cf4895223c5cfb45477c226c1cf66b12795441f708544bdbd67cf373d3
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.1 MB (26065238 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:02e3f7f702eaa8a821c4ac48dd5bb744e37543f54872d17c9063b7c19774cd3d`
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
# Thu, 23 Jan 2020 17:42:47 GMT
ENV PG_MAJOR=10
# Thu, 23 Jan 2020 17:42:47 GMT
ENV PG_VERSION=10.11
# Thu, 23 Jan 2020 17:42:48 GMT
ENV PG_SHA256=0d5d14ff6b075655f4421038fbde3a5d7b418c26a249a187a4175600d7aecc09
# Thu, 23 Jan 2020 17:44:41 GMT
RUN set -ex 		&& apk add --no-cache --virtual .fetch-deps 		ca-certificates 		openssl 		tar 		&& wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2" 	&& echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c - 	&& mkdir -p /usr/src/postgresql 	&& tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	&& rm postgresql.tar.bz2 		&& apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 		&& cd /usr/src/postgresql 	&& awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new 	&& grep '/var/run/postgresql' src/include/pg_config_manual.h.new 	&& mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& ./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 	&& make -j "$(nproc)" world 	&& make install-world 	&& make -C contrib install 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	&& apk del .fetch-deps .build-deps 	&& cd / 	&& rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	&& find /usr/local -name '*.a' -delete
# Thu, 23 Jan 2020 17:44:46 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Thu, 23 Jan 2020 17:44:51 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 23 Jan 2020 17:44:52 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 23 Jan 2020 17:44:53 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 23 Jan 2020 17:44:54 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 23 Jan 2020 17:44:55 GMT
COPY file:74700c51dbcbbad39fbd303750c2ac04ac10f59a73a55171e1fd0dbae6c2f311 in /usr/local/bin/ 
# Thu, 23 Jan 2020 17:44:57 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 23 Jan 2020 17:44:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jan 2020 17:44:59 GMT
EXPOSE 5432
# Thu, 23 Jan 2020 17:44:59 GMT
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
	-	`sha256:3bb3d9a15869812c3ffccdee673ddea8e8782cca749883002fe9ee69f290a08d`  
		Last Modified: Thu, 23 Jan 2020 17:54:22 GMT  
		Size: 23.7 MB (23674835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7efd4fbdf0a7e7092322de145393f5fd374c27254df7022109c60ad46c7490ff`  
		Last Modified: Thu, 23 Jan 2020 17:54:13 GMT  
		Size: 7.4 KB (7353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa015699682ebc753d7a8f0f7b0aef4d0a00d6192119da2e640971ba37c56610`  
		Last Modified: Thu, 23 Jan 2020 17:54:13 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae2b91f2e761f855005ea9be1c53d8f8094c1e2dfc17ac6f61b8aa8bbbf2d0e2`  
		Last Modified: Thu, 23 Jan 2020 17:54:14 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b6b3c2266c4df14603681b7db6c966326b95ac74a16862cb8fbee8c9211ce14`  
		Last Modified: Thu, 23 Jan 2020 17:54:13 GMT  
		Size: 3.8 KB (3836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb707a5123b217e8d8cf995949d8bbeb420045da0f7ea1a2bab2e05628946bd7`  
		Last Modified: Thu, 23 Jan 2020 17:54:13 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:10-alpine` - linux; arm64 variant v8

```console
$ docker pull postgres@sha256:c8e6380464952f75f6a7f09517571006a7bae90c9c9e26697f44d7451fe0339f
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.9 MB (27904784 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:be639ef6e1ca67844c75ec5a009503801cd30a8ace24efbabe6b563c56508925`
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
# Thu, 23 Jan 2020 20:44:04 GMT
ENV PG_MAJOR=10
# Thu, 23 Jan 2020 20:44:05 GMT
ENV PG_VERSION=10.11
# Thu, 23 Jan 2020 20:44:07 GMT
ENV PG_SHA256=0d5d14ff6b075655f4421038fbde3a5d7b418c26a249a187a4175600d7aecc09
# Thu, 23 Jan 2020 20:47:02 GMT
RUN set -ex 		&& apk add --no-cache --virtual .fetch-deps 		ca-certificates 		openssl 		tar 		&& wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2" 	&& echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c - 	&& mkdir -p /usr/src/postgresql 	&& tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	&& rm postgresql.tar.bz2 		&& apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 		&& cd /usr/src/postgresql 	&& awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new 	&& grep '/var/run/postgresql' src/include/pg_config_manual.h.new 	&& mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& ./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 	&& make -j "$(nproc)" world 	&& make install-world 	&& make -C contrib install 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	&& apk del .fetch-deps .build-deps 	&& cd / 	&& rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	&& find /usr/local -name '*.a' -delete
# Thu, 23 Jan 2020 20:47:09 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Thu, 23 Jan 2020 20:47:13 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 23 Jan 2020 20:47:14 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 23 Jan 2020 20:47:17 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 23 Jan 2020 20:47:18 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 23 Jan 2020 20:47:20 GMT
COPY file:74700c51dbcbbad39fbd303750c2ac04ac10f59a73a55171e1fd0dbae6c2f311 in /usr/local/bin/ 
# Thu, 23 Jan 2020 20:47:25 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 23 Jan 2020 20:47:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jan 2020 20:47:27 GMT
EXPOSE 5432
# Thu, 23 Jan 2020 20:47:28 GMT
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
	-	`sha256:add59649f3b5934f6da8768a48850bcc00f643b1d277c8e2fbb68049cec2448e`  
		Last Modified: Thu, 23 Jan 2020 20:58:13 GMT  
		Size: 25.2 MB (25175053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9a43a03c36f47837e899d119e93bd20801806431c9934fff155752a72dac07e`  
		Last Modified: Thu, 23 Jan 2020 20:58:04 GMT  
		Size: 7.4 KB (7356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a530ea7e98f8e471fb074de9a5c7597cbfa94a9228c0260c060f43139711634`  
		Last Modified: Thu, 23 Jan 2020 20:58:03 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74742685a7409c2900444c0f33d63b5c0c50eeb30d869ca76769e3058b1bd044`  
		Last Modified: Thu, 23 Jan 2020 20:58:03 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5803e45c8d6588ccf895646282f27a42d39fc942832e245b3501da750b8e6572`  
		Last Modified: Thu, 23 Jan 2020 20:58:03 GMT  
		Size: 3.8 KB (3838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22e07b8db27a004d19e2ef176f72ab17b63142f44f2e681ecd159b7f5748e7a0`  
		Last Modified: Thu, 23 Jan 2020 20:58:03 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:10-alpine` - linux; 386

```console
$ docker pull postgres@sha256:9c68d201d067de3c7440eb59708304408bf79df1b312211204b3dde71bf41205
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.9 MB (28875993 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6855bd637a607757c1837eaaa53d1983fffeebd0724243523361f26f4b88e100`
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
# Fri, 24 Jan 2020 04:17:49 GMT
ENV PG_MAJOR=10
# Fri, 24 Jan 2020 04:17:49 GMT
ENV PG_VERSION=10.11
# Fri, 24 Jan 2020 04:17:49 GMT
ENV PG_SHA256=0d5d14ff6b075655f4421038fbde3a5d7b418c26a249a187a4175600d7aecc09
# Fri, 24 Jan 2020 04:20:59 GMT
RUN set -ex 		&& apk add --no-cache --virtual .fetch-deps 		ca-certificates 		openssl 		tar 		&& wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2" 	&& echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c - 	&& mkdir -p /usr/src/postgresql 	&& tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	&& rm postgresql.tar.bz2 		&& apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 		&& cd /usr/src/postgresql 	&& awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new 	&& grep '/var/run/postgresql' src/include/pg_config_manual.h.new 	&& mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& ./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 	&& make -j "$(nproc)" world 	&& make install-world 	&& make -C contrib install 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	&& apk del .fetch-deps .build-deps 	&& cd / 	&& rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	&& find /usr/local -name '*.a' -delete
# Fri, 24 Jan 2020 04:21:00 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Fri, 24 Jan 2020 04:21:01 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 24 Jan 2020 04:21:01 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 24 Jan 2020 04:21:01 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 24 Jan 2020 04:21:02 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 24 Jan 2020 04:21:02 GMT
COPY file:74700c51dbcbbad39fbd303750c2ac04ac10f59a73a55171e1fd0dbae6c2f311 in /usr/local/bin/ 
# Fri, 24 Jan 2020 04:21:03 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 24 Jan 2020 04:21:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Jan 2020 04:21:03 GMT
EXPOSE 5432
# Fri, 24 Jan 2020 04:21:03 GMT
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
	-	`sha256:c34025a8269d935c3e624fdb85c61463f6781d1f7b79aa8a60c836281d055330`  
		Last Modified: Fri, 24 Jan 2020 04:31:44 GMT  
		Size: 26.1 MB (26078266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9f49a395654e2916e930bc8751440f6a9d29709e8b7338e780d064aec6368d9`  
		Last Modified: Fri, 24 Jan 2020 04:31:37 GMT  
		Size: 7.4 KB (7351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0414f11f174437aa3f3f350a271c105eb0c590f7e45a2111cedab7c544315b81`  
		Last Modified: Fri, 24 Jan 2020 04:31:36 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12780c0da80ea4c592c75e8cca0be0d079c48948d5710f03ecf3f358e6c3d779`  
		Last Modified: Fri, 24 Jan 2020 04:31:36 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e118be1c3424df45f0a9dad07806b74840411c98fe6e13dd11d133294bafa36`  
		Last Modified: Fri, 24 Jan 2020 04:31:36 GMT  
		Size: 3.8 KB (3839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06fa5c5dac079f648c060cc363d27eb6e6e30f12f5a0c6ddc64fd3601343bb2a`  
		Last Modified: Fri, 24 Jan 2020 04:31:36 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:10-alpine` - linux; ppc64le

```console
$ docker pull postgres@sha256:a05a4b54a932ad52bc4a6053d4fbe561dd5f4dc9e620492caca234d8389c133f
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.3 MB (29317042 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d63b63458e2bc8357fb863300ab6157e3bf19e0a65250fef01f521f134e33a07`
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
# Thu, 23 Jan 2020 18:03:39 GMT
ENV PG_MAJOR=10
# Thu, 23 Jan 2020 18:03:42 GMT
ENV PG_VERSION=10.11
# Thu, 23 Jan 2020 18:03:47 GMT
ENV PG_SHA256=0d5d14ff6b075655f4421038fbde3a5d7b418c26a249a187a4175600d7aecc09
# Thu, 23 Jan 2020 18:06:53 GMT
RUN set -ex 		&& apk add --no-cache --virtual .fetch-deps 		ca-certificates 		openssl 		tar 		&& wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2" 	&& echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c - 	&& mkdir -p /usr/src/postgresql 	&& tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	&& rm postgresql.tar.bz2 		&& apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 		&& cd /usr/src/postgresql 	&& awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new 	&& grep '/var/run/postgresql' src/include/pg_config_manual.h.new 	&& mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& ./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 	&& make -j "$(nproc)" world 	&& make install-world 	&& make -C contrib install 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	&& apk del .fetch-deps .build-deps 	&& cd / 	&& rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	&& find /usr/local -name '*.a' -delete
# Thu, 23 Jan 2020 18:07:03 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Thu, 23 Jan 2020 18:07:13 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 23 Jan 2020 18:07:15 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 23 Jan 2020 18:07:27 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 23 Jan 2020 18:07:30 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 23 Jan 2020 18:07:33 GMT
COPY file:74700c51dbcbbad39fbd303750c2ac04ac10f59a73a55171e1fd0dbae6c2f311 in /usr/local/bin/ 
# Thu, 23 Jan 2020 18:07:45 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 23 Jan 2020 18:07:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jan 2020 18:07:58 GMT
EXPOSE 5432
# Thu, 23 Jan 2020 18:08:13 GMT
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
	-	`sha256:5a112fabb6b5a8856851c56137ab9e6c922ebbe03b23d0b066adcdeaeb1a484f`  
		Last Modified: Thu, 23 Jan 2020 18:22:31 GMT  
		Size: 26.5 MB (26496511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:284c16392870ed6b5ab17e90b8175d02c45abe7d34d0968235e686d8aacd0efb`  
		Last Modified: Thu, 23 Jan 2020 18:22:22 GMT  
		Size: 7.4 KB (7353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4214afa52a5732803b5e3226c71b84eb9797836230be63bbd8a2dd00e11b921e`  
		Last Modified: Thu, 23 Jan 2020 18:22:23 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d134167d9969e2390071d5f3d2de3e0ff98500f2a3c41553290995d69c681af`  
		Last Modified: Thu, 23 Jan 2020 18:22:22 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afa3b9fb6c03f9a9a780cc94b8b78382907668499b7f98f2f8e2c829b51e80da`  
		Last Modified: Thu, 23 Jan 2020 18:22:22 GMT  
		Size: 3.8 KB (3840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d49002f34f86a2f76ca7d05fe2cd661d1fe652333d7d78f1da2c0f4b59254493`  
		Last Modified: Thu, 23 Jan 2020 18:22:23 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:10-alpine` - linux; s390x

```console
$ docker pull postgres@sha256:d6336ce57da472068554ee8ac4933201ab75559b20b8c64cf25820414bd1c0fe
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.8 MB (27832864 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91eaa044bfcdb6ad7d7f8f5394cda1c442a2959a50e7a2468c0dbd986afb5cb8`
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
# Thu, 23 Jan 2020 19:07:29 GMT
ENV PG_MAJOR=10
# Thu, 23 Jan 2020 19:07:29 GMT
ENV PG_VERSION=10.11
# Thu, 23 Jan 2020 19:07:29 GMT
ENV PG_SHA256=0d5d14ff6b075655f4421038fbde3a5d7b418c26a249a187a4175600d7aecc09
# Thu, 23 Jan 2020 19:09:12 GMT
RUN set -ex 		&& apk add --no-cache --virtual .fetch-deps 		ca-certificates 		openssl 		tar 		&& wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2" 	&& echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c - 	&& mkdir -p /usr/src/postgresql 	&& tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	&& rm postgresql.tar.bz2 		&& apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 		&& cd /usr/src/postgresql 	&& awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new 	&& grep '/var/run/postgresql' src/include/pg_config_manual.h.new 	&& mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& ./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 	&& make -j "$(nproc)" world 	&& make install-world 	&& make -C contrib install 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	&& apk del .fetch-deps .build-deps 	&& cd / 	&& rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	&& find /usr/local -name '*.a' -delete
# Thu, 23 Jan 2020 19:09:13 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Thu, 23 Jan 2020 19:09:13 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 23 Jan 2020 19:09:13 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 23 Jan 2020 19:09:14 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 23 Jan 2020 19:09:14 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 23 Jan 2020 19:09:14 GMT
COPY file:74700c51dbcbbad39fbd303750c2ac04ac10f59a73a55171e1fd0dbae6c2f311 in /usr/local/bin/ 
# Thu, 23 Jan 2020 19:09:15 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 23 Jan 2020 19:09:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jan 2020 19:09:15 GMT
EXPOSE 5432
# Thu, 23 Jan 2020 19:09:16 GMT
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
	-	`sha256:e27660f93771bb42b70d6b550ab31a28f9254056d11810001ef5fb9494521e1b`  
		Last Modified: Thu, 23 Jan 2020 19:17:52 GMT  
		Size: 25.2 MB (25247381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:874d7afba5e3ca6a063729882918b9a14357cbae3739f59110a497db84d125f4`  
		Last Modified: Thu, 23 Jan 2020 19:17:47 GMT  
		Size: 7.4 KB (7351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2228b94a1359dcb2c748623dd52aa3fa5fdb3dce6d2d19758784bff06bd59259`  
		Last Modified: Thu, 23 Jan 2020 19:17:47 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63881d37ea2a1ea3f6846948c89dc9f96f3f5e7ca156ef436a8a1d1727c306e6`  
		Last Modified: Thu, 23 Jan 2020 19:17:46 GMT  
		Size: 165.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:678f632d9a9615ba00de65760e24b971572f6eba89f05095264e418794449425`  
		Last Modified: Thu, 23 Jan 2020 19:17:46 GMT  
		Size: 3.8 KB (3834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c87b346d14f7b738ad740b9ca3f4fbd51dbc4db5ef9181cb76dbf1b2997f47e`  
		Last Modified: Thu, 23 Jan 2020 19:17:46 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
