## `postgres:10-alpine`

```console
$ docker pull postgres@sha256:39982740182c62a8ca398bf21bba9e1204d8a680dad22d1da6533fbb2f41e389
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
$ docker pull postgres@sha256:ca5a9b56a25e16cc99b81e2afa7ee8db31bc4a0fe70120e7f39de4a4d78c6675
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.6 MB (28603130 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6993b3a4e0a8598f1e16f30209b57ab0dc42e63e6f7815625e271bc443233024`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 25 Mar 2021 22:19:32 GMT
ADD file:6b081cabb4b256ee07587d249c4989b5b679375529542b81550a65b6f19f274e in / 
# Thu, 25 Mar 2021 22:19:32 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 01:13:38 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Fri, 26 Mar 2021 01:13:38 GMT
ENV LANG=en_US.utf8
# Fri, 26 Mar 2021 01:13:39 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 26 Mar 2021 01:34:40 GMT
ENV PG_MAJOR=10
# Fri, 26 Mar 2021 01:34:40 GMT
ENV PG_VERSION=10.16
# Fri, 26 Mar 2021 01:34:41 GMT
ENV PG_SHA256=a35c718b1b6690e01c69626d467edb933784f8d1d6741e21fe6cce0738467bb3
# Fri, 26 Mar 2021 01:38:01 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Fri, 26 Mar 2021 01:38:03 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Fri, 26 Mar 2021 01:38:04 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 26 Mar 2021 01:38:04 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 26 Mar 2021 01:38:06 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 26 Mar 2021 01:38:06 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 26 Mar 2021 01:38:06 GMT
COPY file:ad28506adc606e446eefc263bc99d4cb809e608d4f550956143bf13c82c91f85 in /usr/local/bin/ 
# Fri, 26 Mar 2021 01:38:07 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 26 Mar 2021 01:38:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 01:38:08 GMT
STOPSIGNAL SIGINT
# Fri, 26 Mar 2021 01:38:08 GMT
EXPOSE 5432
# Fri, 26 Mar 2021 01:38:08 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:9aae54b2144e5b2b00c610f8805128f4f86822e1e52d3714c463744a431f0f4a`  
		Last Modified: Thu, 25 Mar 2021 22:20:18 GMT  
		Size: 2.8 MB (2811681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:685d662498eadee2c5a3d6886968b26b1f090422a2d94212fce0de8078e9906a`  
		Last Modified: Fri, 26 Mar 2021 01:47:42 GMT  
		Size: 1.3 KB (1275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6952eb90a4e9be7a0703f381031d1fefc454fd8fd9e9211b4351d2c8c7472a5b`  
		Last Modified: Fri, 26 Mar 2021 01:47:42 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c349367892415ee98f11ac79c7f93e9e3ddcda38a86694ec610a997df1d0fef2`  
		Last Modified: Fri, 26 Mar 2021 01:49:02 GMT  
		Size: 25.8 MB (25777791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba9b1a4751eef4d6bf1968900dbf235502c8206d1b4f4bed71ef408d60eab7c2`  
		Last Modified: Fri, 26 Mar 2021 01:48:54 GMT  
		Size: 7.4 KB (7353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d5477c0a057a8ff6b8401dda7b13e3fa8a391bb427a2f60721d634b6ecb0f99`  
		Last Modified: Fri, 26 Mar 2021 01:48:54 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96857fc4892b8fb84685bf0b7472e2d9fa85ca1e489e431ea26bd06c394ab0ac`  
		Last Modified: Fri, 26 Mar 2021 01:48:54 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9708a1eb69835c867e7309a9d084c537c7683726a034450173cff9d77b97658a`  
		Last Modified: Fri, 26 Mar 2021 01:48:54 GMT  
		Size: 4.4 KB (4405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5462d1da2a65fb018a9a7a2c5ff5c1b11fd1c7306c890c77502bfdeadfd23afb`  
		Last Modified: Fri, 26 Mar 2021 01:48:54 GMT  
		Size: 119.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:10-alpine` - linux; arm variant v6

```console
$ docker pull postgres@sha256:5fb94e3c2d75daa18c83fe1132bb2eff31ba515d52a99fd5ba1317c2d7bcd560
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.7 MB (27731527 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b49d04682a8ac48d4eaa23de33b042f4b06e9aba0c6aab91046aa3635173dfcb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Wed, 31 Mar 2021 17:18:49 GMT
ADD file:988879d74f643b89539e5a0b6d74221621f19f4f87f722614addadc46ce47200 in / 
# Wed, 31 Mar 2021 17:18:50 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 00:09:28 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 01 Apr 2021 00:09:29 GMT
ENV LANG=en_US.utf8
# Thu, 01 Apr 2021 00:09:34 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 01 Apr 2021 00:29:30 GMT
ENV PG_MAJOR=10
# Thu, 01 Apr 2021 00:29:33 GMT
ENV PG_VERSION=10.16
# Thu, 01 Apr 2021 00:29:40 GMT
ENV PG_SHA256=a35c718b1b6690e01c69626d467edb933784f8d1d6741e21fe6cce0738467bb3
# Thu, 01 Apr 2021 00:33:00 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Thu, 01 Apr 2021 00:33:04 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Thu, 01 Apr 2021 00:33:07 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 01 Apr 2021 00:33:08 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 01 Apr 2021 00:33:10 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 01 Apr 2021 00:33:11 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 01 Apr 2021 00:33:12 GMT
COPY file:ad28506adc606e446eefc263bc99d4cb809e608d4f550956143bf13c82c91f85 in /usr/local/bin/ 
# Thu, 01 Apr 2021 00:33:14 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 01 Apr 2021 00:33:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Apr 2021 00:33:16 GMT
STOPSIGNAL SIGINT
# Thu, 01 Apr 2021 00:33:16 GMT
EXPOSE 5432
# Thu, 01 Apr 2021 00:33:17 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:bb87125c6ee1ce30c6b33d2c96a9fbe46da4a290f7cb1dd73fd62d4e06503699`  
		Last Modified: Wed, 31 Mar 2021 17:19:55 GMT  
		Size: 2.6 MB (2622116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a8ef9aade831ec2952a74875bbd6d6e1a7fa389739078a55e74fe9fcd4129dc`  
		Last Modified: Thu, 01 Apr 2021 00:42:38 GMT  
		Size: 1.3 KB (1276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9928d1bc98142f86c1b21ad1f2bf086dd6be1bf4b65bad782dc061bca4dc2b9`  
		Last Modified: Thu, 01 Apr 2021 00:42:37 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a90095cea43d84b22e68446dd03a7cf5f9f6a2beed6a9bf5051a590ce44ed2f1`  
		Last Modified: Thu, 01 Apr 2021 00:44:28 GMT  
		Size: 25.1 MB (25095749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3746047641030cea8e745f8d385299fee4f255da5c28bc748792daafdb169f1a`  
		Last Modified: Thu, 01 Apr 2021 00:44:18 GMT  
		Size: 7.4 KB (7353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c758e94c03a10284c1a96a4c45b2094069eedf3cc2e56d5b1b97cc172aecf23`  
		Last Modified: Thu, 01 Apr 2021 00:44:18 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6320180c7bf123efb349f6fc822d9326a810843f8d7a2c2646bc706dc9034de`  
		Last Modified: Thu, 01 Apr 2021 00:44:18 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63b1708d1a2d72c745d1aacc6eb217f6f49f51f184b34c249e80ef2fdcaa9d2f`  
		Last Modified: Thu, 01 Apr 2021 00:44:18 GMT  
		Size: 4.4 KB (4408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b337896e6d311bc345b8d3b04135f8c833459deeb3ebcd6945f8966b871ecb7e`  
		Last Modified: Thu, 01 Apr 2021 00:44:18 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:10-alpine` - linux; arm variant v7

```console
$ docker pull postgres@sha256:5a3d3a97da5fd3c000f9f2d50b6e2f45952838fd682192cfd621b3402746bf14
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.7 MB (26665577 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e6787a6bd22c76c06727c4fa3a38f46a508a2bb7752ea82a9bbe9171c134b806`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 25 Mar 2021 22:05:53 GMT
ADD file:44ef6cff6e7d37a67c5846eb792fec65025702c00c56ff96801ac79bf81b0cc3 in / 
# Thu, 25 Mar 2021 22:05:55 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 01:53:48 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Fri, 26 Mar 2021 01:53:49 GMT
ENV LANG=en_US.utf8
# Fri, 26 Mar 2021 01:53:56 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 26 Mar 2021 02:10:15 GMT
ENV PG_MAJOR=10
# Fri, 26 Mar 2021 02:10:17 GMT
ENV PG_VERSION=10.16
# Fri, 26 Mar 2021 02:10:20 GMT
ENV PG_SHA256=a35c718b1b6690e01c69626d467edb933784f8d1d6741e21fe6cce0738467bb3
# Fri, 26 Mar 2021 02:13:10 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Fri, 26 Mar 2021 02:13:13 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Fri, 26 Mar 2021 02:13:15 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 26 Mar 2021 02:13:15 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 26 Mar 2021 02:13:17 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 26 Mar 2021 02:13:18 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 26 Mar 2021 02:13:19 GMT
COPY file:ad28506adc606e446eefc263bc99d4cb809e608d4f550956143bf13c82c91f85 in /usr/local/bin/ 
# Fri, 26 Mar 2021 02:13:21 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 26 Mar 2021 02:13:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 02:13:23 GMT
STOPSIGNAL SIGINT
# Fri, 26 Mar 2021 02:13:23 GMT
EXPOSE 5432
# Fri, 26 Mar 2021 02:13:24 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:6c1162af251f0d5ab4945f8506f3265b86d0a03cda37f703c2446a71a233bc20`  
		Last Modified: Thu, 25 Mar 2021 22:07:21 GMT  
		Size: 2.4 MB (2423999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:686fbcccead7b8176944ecbd7b1588b7ff1b1b192c4aa91d70ba1e99cfa3204a`  
		Last Modified: Fri, 26 Mar 2021 02:21:36 GMT  
		Size: 1.3 KB (1277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bc2b54cd5d349bc58c5f736abac730cd43f808eab4e3974f0e524226fc14fb1`  
		Last Modified: Fri, 26 Mar 2021 02:21:36 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6693bf6f3332f579ca13f47f257066e97238ca9707f3ab2b0f7c0634f5df0147`  
		Last Modified: Fri, 26 Mar 2021 02:22:58 GMT  
		Size: 24.2 MB (24227920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:beb85fc2c4893b62441274ed94e44450df6b1c4fdfbfe93d6348b9ef53373496`  
		Last Modified: Fri, 26 Mar 2021 02:22:49 GMT  
		Size: 7.4 KB (7354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddee3bc388e6bb7030441aafe2f2b1522cdb5e7b27f4365a0cc4e8031e546ecf`  
		Last Modified: Fri, 26 Mar 2021 02:22:49 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e54349b7bc143876095ba8e4653b734bc1e41436e97d3dda551b6cdd3fc1f124`  
		Last Modified: Fri, 26 Mar 2021 02:22:49 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:535959459a6f226fceb15659524d6a4f7e94c98f5f4106a538db751f46f70239`  
		Last Modified: Fri, 26 Mar 2021 02:22:49 GMT  
		Size: 4.4 KB (4404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec2095527f83177fac0ffbd00a71d3aea79f3b43f40bd4237ce0be568dab8675`  
		Last Modified: Fri, 26 Mar 2021 02:22:49 GMT  
		Size: 118.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:10-alpine` - linux; arm64 variant v8

```console
$ docker pull postgres@sha256:7401b62f18e62961ac32ca6aea4aa643ebc89cb9abd05b3173a71ca60fcafe1b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.3 MB (28310296 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e78142a0478d428458d17e92e1bab33b5c20f2cd96c6df0c4ce04868498ce5e2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 25 Mar 2021 22:40:10 GMT
ADD file:8d7431f7e3e42b162a1626e7abf4ef7605146671dccc753d490de6b7fe429261 in / 
# Thu, 25 Mar 2021 22:40:23 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 05:48:03 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Fri, 26 Mar 2021 05:48:05 GMT
ENV LANG=en_US.utf8
# Fri, 26 Mar 2021 05:48:07 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 26 Mar 2021 06:04:19 GMT
ENV PG_MAJOR=10
# Fri, 26 Mar 2021 06:04:20 GMT
ENV PG_VERSION=10.16
# Fri, 26 Mar 2021 06:04:21 GMT
ENV PG_SHA256=a35c718b1b6690e01c69626d467edb933784f8d1d6741e21fe6cce0738467bb3
# Fri, 26 Mar 2021 06:07:12 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Fri, 26 Mar 2021 06:07:15 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Fri, 26 Mar 2021 06:07:18 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 26 Mar 2021 06:07:19 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 26 Mar 2021 06:07:23 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 26 Mar 2021 06:07:25 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 26 Mar 2021 06:07:26 GMT
COPY file:ad28506adc606e446eefc263bc99d4cb809e608d4f550956143bf13c82c91f85 in /usr/local/bin/ 
# Fri, 26 Mar 2021 06:07:30 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 26 Mar 2021 06:07:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 06:07:33 GMT
STOPSIGNAL SIGINT
# Fri, 26 Mar 2021 06:07:34 GMT
EXPOSE 5432
# Fri, 26 Mar 2021 06:07:35 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:5ceb5101e3b0d54efb5f18318982508a04b181b4d5ae52b096dd35dea3a006cc`  
		Last Modified: Thu, 25 Mar 2021 22:44:41 GMT  
		Size: 2.7 MB (2711898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fbf3db8f794d2076e679b1475530e6a0aacc443280d47e3624510cd68b8f9d0`  
		Last Modified: Fri, 26 Mar 2021 06:15:46 GMT  
		Size: 1.3 KB (1276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:446616bc8c18b7bb633e1a7d7fcb31293d94086c04dd90576b39832ed97c50f6`  
		Last Modified: Fri, 26 Mar 2021 06:15:46 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cc216a7687e39725ab044653203a8c8adf373c88253f8720e884d38101789b1`  
		Last Modified: Fri, 26 Mar 2021 06:17:10 GMT  
		Size: 25.6 MB (25584737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a82817e357bc8c9c72b6c1572bda6c2c088ebb5f6d86452e51275ff047ad6b0`  
		Last Modified: Fri, 26 Mar 2021 06:17:02 GMT  
		Size: 7.4 KB (7355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76b23e0eb63a10997cd791428fc56170974c2f8f066ad59818a108aaca816b65`  
		Last Modified: Fri, 26 Mar 2021 06:17:02 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ca7b1cbfe769bfe4d4d67d45d85ab871bb13e88e649ff8c6fc86f56a4c3b643`  
		Last Modified: Fri, 26 Mar 2021 06:17:02 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02192371b985895c2fb2abec3b9e2ed6930f15429e95189fa4283868f5015428`  
		Last Modified: Fri, 26 Mar 2021 06:17:02 GMT  
		Size: 4.4 KB (4406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91ccda318f7a500e45e3dea1f3f7e3f45473100ffd21a3ea1ac5bf0ceb1b5cb7`  
		Last Modified: Fri, 26 Mar 2021 06:17:02 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:10-alpine` - linux; 386

```console
$ docker pull postgres@sha256:03f3cc7a6e4a11d9c77c991ce2b66001739b01f661d0c1aa7ba1483fbce31576
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.5 MB (29534825 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:558ef6db78acbef7bf773e1d1c567ad674f9d447df3c2f83c95d97d533a58865`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 25 Mar 2021 22:38:25 GMT
ADD file:8953415d4b98f486af17a39ba53b38f7262aa590734c18ff9318927e5a705baf in / 
# Thu, 25 Mar 2021 22:38:26 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 10:52:21 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Fri, 26 Mar 2021 10:52:22 GMT
ENV LANG=en_US.utf8
# Fri, 26 Mar 2021 10:52:23 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 26 Mar 2021 11:12:32 GMT
ENV PG_MAJOR=10
# Fri, 26 Mar 2021 11:12:32 GMT
ENV PG_VERSION=10.16
# Fri, 26 Mar 2021 11:12:32 GMT
ENV PG_SHA256=a35c718b1b6690e01c69626d467edb933784f8d1d6741e21fe6cce0738467bb3
# Fri, 26 Mar 2021 11:16:04 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Fri, 26 Mar 2021 11:16:05 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Fri, 26 Mar 2021 11:16:06 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 26 Mar 2021 11:16:06 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 26 Mar 2021 11:16:07 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 26 Mar 2021 11:16:07 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 26 Mar 2021 11:16:07 GMT
COPY file:ad28506adc606e446eefc263bc99d4cb809e608d4f550956143bf13c82c91f85 in /usr/local/bin/ 
# Fri, 26 Mar 2021 11:16:08 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 26 Mar 2021 11:16:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 11:16:08 GMT
STOPSIGNAL SIGINT
# Fri, 26 Mar 2021 11:16:09 GMT
EXPOSE 5432
# Fri, 26 Mar 2021 11:16:09 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:1fbd1c9912b638ce64a4740e3af7a3a03452f8705b8103950d677f1d79ae8164`  
		Last Modified: Thu, 25 Mar 2021 22:39:34 GMT  
		Size: 2.8 MB (2818129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f3f924c48908289f345953f253adaa361874b5113b36e5cbb8aae77b810b23f`  
		Last Modified: Fri, 26 Mar 2021 11:24:59 GMT  
		Size: 1.3 KB (1272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d77e766b950efc06c2b91414816eb3780dca398cd9e27a9648bc2940b10499b4`  
		Last Modified: Fri, 26 Mar 2021 11:25:01 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f6752058e192c5ba9c6bc5946c253dfd5d8bfb8c303e04d02bb26a09c1004c8`  
		Last Modified: Fri, 26 Mar 2021 11:26:37 GMT  
		Size: 26.7 MB (26703047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e078a689e24a682c30277b5345c93a32582a4c8a225c1e0fb6d7953ac036b0a7`  
		Last Modified: Fri, 26 Mar 2021 11:26:29 GMT  
		Size: 7.3 KB (7348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8b2732ab41794c2c24d5493695e36f4fa002184b515947643c4ee7a7395ac23`  
		Last Modified: Fri, 26 Mar 2021 11:26:29 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bbd3c250c22a1caf49ce50c9388842d6ea315bf51ce1d56145dbb83b752d863`  
		Last Modified: Fri, 26 Mar 2021 11:26:29 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba786e7968ff7e6efb29d0f40e05e80d9c50f55942467a8bb79e05bd5a8b6f96`  
		Last Modified: Fri, 26 Mar 2021 11:26:29 GMT  
		Size: 4.4 KB (4402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97733a201d85f028ff15423ec5126a3572d4e85635bc9e036dc01d5a8c528aaf`  
		Last Modified: Fri, 26 Mar 2021 11:26:29 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:10-alpine` - linux; ppc64le

```console
$ docker pull postgres@sha256:44013b843735921416272d94e95dbebcbcd1020cbcb89e279a4f83a0e966a408
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.8 MB (29798314 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d003200916f94b85cfc969da6c9875caed3beaa394ee0623587a6d322b8fb9af`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 25 Mar 2021 22:22:28 GMT
ADD file:f91f8e0aa646cb847f6e210056280f9332382ad2f8d6a8839fd9aa69b81c4a2a in / 
# Thu, 25 Mar 2021 22:22:30 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 01:48:04 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Fri, 26 Mar 2021 01:48:07 GMT
ENV LANG=en_US.utf8
# Fri, 26 Mar 2021 01:48:12 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 26 Mar 2021 02:06:12 GMT
ENV PG_MAJOR=10
# Fri, 26 Mar 2021 02:06:17 GMT
ENV PG_VERSION=10.16
# Fri, 26 Mar 2021 02:06:23 GMT
ENV PG_SHA256=a35c718b1b6690e01c69626d467edb933784f8d1d6741e21fe6cce0738467bb3
# Fri, 26 Mar 2021 02:09:19 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Fri, 26 Mar 2021 02:09:36 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Fri, 26 Mar 2021 02:09:51 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 26 Mar 2021 02:09:58 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 26 Mar 2021 02:10:12 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 26 Mar 2021 02:10:19 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 26 Mar 2021 02:10:23 GMT
COPY file:ad28506adc606e446eefc263bc99d4cb809e608d4f550956143bf13c82c91f85 in /usr/local/bin/ 
# Fri, 26 Mar 2021 02:10:35 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 26 Mar 2021 02:10:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 02:10:49 GMT
STOPSIGNAL SIGINT
# Fri, 26 Mar 2021 02:10:57 GMT
EXPOSE 5432
# Fri, 26 Mar 2021 02:11:08 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:f3b2866c25f0a9167af050d646a7a740ccc88d46e068c90ff28a5c2ec2ee0030`  
		Last Modified: Thu, 25 Mar 2021 22:24:08 GMT  
		Size: 2.8 MB (2813115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed8dbeea72bbbd5311c12e548996b438d21b7b9f0bbc23e4b5dc5e4becf541a2`  
		Last Modified: Fri, 26 Mar 2021 02:22:52 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48ad6573569f171ac7316a0d4139d7e2cad9414b96ff1b984ea6e0c26bdd991d`  
		Last Modified: Fri, 26 Mar 2021 02:22:50 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:688fb38b3f433d04aee0c605b79dfc5f86e8707e528c086a1d5c1c3683b8fded`  
		Last Modified: Fri, 26 Mar 2021 02:24:36 GMT  
		Size: 27.0 MB (26971532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adca68d6263131b8cb3fd94b0a3e1d80e890b9b5f819b300ab04fb123d0fde1f`  
		Last Modified: Fri, 26 Mar 2021 02:24:19 GMT  
		Size: 7.4 KB (7351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8481af2b8803b7bda84b995f90a0ffbef1d03d2785042570fb6f5c4550b68da`  
		Last Modified: Fri, 26 Mar 2021 02:24:19 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:498a5146e50fcd78d38a755a905e83b628430b46d151938691aff337b7d9006c`  
		Last Modified: Fri, 26 Mar 2021 02:24:19 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:630e621651c3f1189ce7786a69e2c3766a9f0e34f42d6eb6e4ba4b123ac0035b`  
		Last Modified: Fri, 26 Mar 2021 02:24:19 GMT  
		Size: 4.4 KB (4405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2935da16f751eae9ba80b36c81255781e59d6793038b0689cb6daf291bbf0a2`  
		Last Modified: Fri, 26 Mar 2021 02:24:19 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:10-alpine` - linux; s390x

```console
$ docker pull postgres@sha256:40095d0f4a52bb2b1c54f9bedad9014accfc3e71b8be7bf48c36764bd920a790
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.5 MB (28460049 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:71f0e0e445dbddbdc7d1126e2ac3f284c3f07319e3fa304477319cc0f965a4b3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Wed, 31 Mar 2021 17:14:58 GMT
ADD file:3f5fe04867af3c9f2cfc5b315d97097145ae11343399985386321a8db21d7786 in / 
# Wed, 31 Mar 2021 17:14:58 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 02:32:03 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 01 Apr 2021 02:32:03 GMT
ENV LANG=en_US.utf8
# Thu, 01 Apr 2021 02:32:04 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 01 Apr 2021 02:43:23 GMT
ENV PG_MAJOR=10
# Thu, 01 Apr 2021 02:43:23 GMT
ENV PG_VERSION=10.16
# Thu, 01 Apr 2021 02:43:23 GMT
ENV PG_SHA256=a35c718b1b6690e01c69626d467edb933784f8d1d6741e21fe6cce0738467bb3
# Thu, 01 Apr 2021 02:45:36 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Thu, 01 Apr 2021 02:45:38 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Thu, 01 Apr 2021 02:45:38 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 01 Apr 2021 02:45:39 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 01 Apr 2021 02:45:39 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 01 Apr 2021 02:45:40 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 01 Apr 2021 02:45:40 GMT
COPY file:ad28506adc606e446eefc263bc99d4cb809e608d4f550956143bf13c82c91f85 in /usr/local/bin/ 
# Thu, 01 Apr 2021 02:45:40 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 01 Apr 2021 02:45:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Apr 2021 02:45:41 GMT
STOPSIGNAL SIGINT
# Thu, 01 Apr 2021 02:45:41 GMT
EXPOSE 5432
# Thu, 01 Apr 2021 02:45:41 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:1d4058bbeedf5296bcaf5ae8f37c8cd58152acad3ec45a536e08b83f5d3abe83`  
		Last Modified: Wed, 31 Mar 2021 17:15:36 GMT  
		Size: 2.6 MB (2602591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eefbd2fe9b0bd78991d6dbe99b6736ed824fba505223f670a84ef4c1cae7d848`  
		Last Modified: Thu, 01 Apr 2021 02:50:58 GMT  
		Size: 1.3 KB (1283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5672c36514f991c9ff38b8525344da27d649a892d978d50fe890833642f39491`  
		Last Modified: Thu, 01 Apr 2021 02:50:58 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18fb4634544c5fb94a460c410484f76e9f8ec104c84417ed57bdd30f0308fb53`  
		Last Modified: Thu, 01 Apr 2021 02:51:51 GMT  
		Size: 25.8 MB (25843793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe4e83226eda605ed2e179016ea3dc2c1efe05655b2b119768756e051318f445`  
		Last Modified: Thu, 01 Apr 2021 02:51:48 GMT  
		Size: 7.4 KB (7351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e73ca6b020a032c7b2aca92e277c175b2f4571f16b7d57eba75b1159fb096fb`  
		Last Modified: Thu, 01 Apr 2021 02:51:49 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7117f60aad1a6cfa9a83fd5c0119ee75c860c54e92f468f18f293276181c63ab`  
		Last Modified: Thu, 01 Apr 2021 02:51:46 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7579b3ceaf277e28e5ce8c3684d832e1f12ddab6d5f4972e8f89000f765dadde`  
		Last Modified: Thu, 01 Apr 2021 02:51:48 GMT  
		Size: 4.4 KB (4405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5242fb3cec92918b53170491b917a900cb1295cea9e9b2fd874a3f74fb414769`  
		Last Modified: Thu, 01 Apr 2021 02:51:48 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
